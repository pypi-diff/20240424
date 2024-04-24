# Comparing `tmp/flytekitplugins-flyteinteractive-1.12.0b5.tar.gz` & `tmp/flytekitplugins_flyteinteractive-1.12.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-flyteinteractive-1.12.0b5.tar", last modified: Wed Apr 10 17:16:51 2024, max compression
+gzip compressed data, was "flytekitplugins_flyteinteractive-1.12.0b6.tar", last modified: Wed Apr 24 18:30:35 2024, max compression
```

## Comparing `flytekitplugins-flyteinteractive-1.12.0b5.tar` & `flytekitplugins_flyteinteractive-1.12.0b6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:16:51.699280 flytekitplugins-flyteinteractive-1.12.0b5/
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-10 17:16:51.695280 flytekitplugins-flyteinteractive-1.12.0b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4476 2024-04-10 17:16:22.000000 flytekitplugins-flyteinteractive-1.12.0b5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:16:51.691280 flytekitplugins-flyteinteractive-1.12.0b5/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:16:51.695280 flytekitplugins-flyteinteractive-1.12.0b5/flytekitplugins/flyteinteractive/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-10 17:16:22.000000 flytekitplugins-flyteinteractive-1.12.0b5/flytekitplugins/flyteinteractive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-10 17:16:22.000000 flytekitplugins-flyteinteractive-1.12.0b5/flytekitplugins/flyteinteractive/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:16:51.695280 flytekitplugins-flyteinteractive-1.12.0b5/flytekitplugins/flyteinteractive/jupyter_lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:16:22.000000 flytekitplugins-flyteinteractive-1.12.0b5/flytekitplugins/flyteinteractive/jupyter_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7683 2024-04-10 17:16:22.000000 flytekitplugins-flyteinteractive-1.12.0b5/flytekitplugins/flyteinteractive/jupyter_lib/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-10 17:16:22.000000 flytekitplugins-flyteinteractive-1.12.0b5/flytekitplugins/flyteinteractive/jupyter_lib/jupyter_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-10 17:16:22.000000 flytekitplugins-flyteinteractive-1.12.0b5/flytekitplugins/flyteinteractive/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:16:51.695280 flytekitplugins-flyteinteractive-1.12.0b5/flytekitplugins/flyteinteractive/vscode_lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:16:22.000000 flytekitplugins-flyteinteractive-1.12.0b5/flytekitplugins/flyteinteractive/vscode_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-04-10 17:16:22.000000 flytekitplugins-flyteinteractive-1.12.0b5/flytekitplugins/flyteinteractive/vscode_lib/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    18774 2024-04-10 17:16:22.000000 flytekitplugins-flyteinteractive-1.12.0b5/flytekitplugins/flyteinteractive/vscode_lib/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-10 17:16:22.000000 flytekitplugins-flyteinteractive-1.12.0b5/flytekitplugins/flyteinteractive/vscode_lib/vscode_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:16:51.695280 flytekitplugins-flyteinteractive-1.12.0b5/flytekitplugins_flyteinteractive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-10 17:16:51.000000 flytekitplugins-flyteinteractive-1.12.0b5/flytekitplugins_flyteinteractive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-10 17:16:51.000000 flytekitplugins-flyteinteractive-1.12.0b5/flytekitplugins_flyteinteractive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 17:16:51.000000 flytekitplugins-flyteinteractive-1.12.0b5/flytekitplugins_flyteinteractive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-10 17:16:51.000000 flytekitplugins-flyteinteractive-1.12.0b5/flytekitplugins_flyteinteractive.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-10 17:16:51.000000 flytekitplugins-flyteinteractive-1.12.0b5/flytekitplugins_flyteinteractive.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-10 17:16:51.000000 flytekitplugins-flyteinteractive-1.12.0b5/flytekitplugins_flyteinteractive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-10 17:16:51.000000 flytekitplugins-flyteinteractive-1.12.0b5/flytekitplugins_flyteinteractive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 17:16:51.699280 flytekitplugins-flyteinteractive-1.12.0b5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-10 17:16:47.000000 flytekitplugins-flyteinteractive-1.12.0b5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:16:51.695280 flytekitplugins-flyteinteractive-1.12.0b5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-04-10 17:16:22.000000 flytekitplugins-flyteinteractive-1.12.0b5/tests/test_flyteinteractive_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (127)    12906 2024-04-10 17:16:22.000000 flytekitplugins-flyteinteractive-1.12.0b5/tests/test_flyteinteractive_vscode.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-10 17:16:22.000000 flytekitplugins-flyteinteractive-1.12.0b5/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:35.501208 flytekitplugins_flyteinteractive-1.12.0b6/
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-24 18:30:35.501208 flytekitplugins_flyteinteractive-1.12.0b6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4476 2024-04-24 18:30:04.000000 flytekitplugins_flyteinteractive-1.12.0b6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:35.497208 flytekitplugins_flyteinteractive-1.12.0b6/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:35.497208 flytekitplugins_flyteinteractive-1.12.0b6/flytekitplugins/flyteinteractive/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-24 18:30:04.000000 flytekitplugins_flyteinteractive-1.12.0b6/flytekitplugins/flyteinteractive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-24 18:30:04.000000 flytekitplugins_flyteinteractive-1.12.0b6/flytekitplugins/flyteinteractive/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:35.497208 flytekitplugins_flyteinteractive-1.12.0b6/flytekitplugins/flyteinteractive/jupyter_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:04.000000 flytekitplugins_flyteinteractive-1.12.0b6/flytekitplugins/flyteinteractive/jupyter_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7683 2024-04-24 18:30:04.000000 flytekitplugins_flyteinteractive-1.12.0b6/flytekitplugins/flyteinteractive/jupyter_lib/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-24 18:30:04.000000 flytekitplugins_flyteinteractive-1.12.0b6/flytekitplugins/flyteinteractive/jupyter_lib/jupyter_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-24 18:30:04.000000 flytekitplugins_flyteinteractive-1.12.0b6/flytekitplugins/flyteinteractive/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:35.501208 flytekitplugins_flyteinteractive-1.12.0b6/flytekitplugins/flyteinteractive/vscode_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:04.000000 flytekitplugins_flyteinteractive-1.12.0b6/flytekitplugins/flyteinteractive/vscode_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-04-24 18:30:04.000000 flytekitplugins_flyteinteractive-1.12.0b6/flytekitplugins/flyteinteractive/vscode_lib/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18774 2024-04-24 18:30:04.000000 flytekitplugins_flyteinteractive-1.12.0b6/flytekitplugins/flyteinteractive/vscode_lib/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-24 18:30:04.000000 flytekitplugins_flyteinteractive-1.12.0b6/flytekitplugins/flyteinteractive/vscode_lib/vscode_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:35.501208 flytekitplugins_flyteinteractive-1.12.0b6/flytekitplugins_flyteinteractive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-24 18:30:35.000000 flytekitplugins_flyteinteractive-1.12.0b6/flytekitplugins_flyteinteractive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-24 18:30:35.000000 flytekitplugins_flyteinteractive-1.12.0b6/flytekitplugins_flyteinteractive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 18:30:35.000000 flytekitplugins_flyteinteractive-1.12.0b6/flytekitplugins_flyteinteractive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 18:30:35.000000 flytekitplugins_flyteinteractive-1.12.0b6/flytekitplugins_flyteinteractive.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-24 18:30:35.000000 flytekitplugins_flyteinteractive-1.12.0b6/flytekitplugins_flyteinteractive.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-24 18:30:35.000000 flytekitplugins_flyteinteractive-1.12.0b6/flytekitplugins_flyteinteractive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-24 18:30:35.000000 flytekitplugins_flyteinteractive-1.12.0b6/flytekitplugins_flyteinteractive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 18:30:35.501208 flytekitplugins_flyteinteractive-1.12.0b6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-24 18:30:31.000000 flytekitplugins_flyteinteractive-1.12.0b6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:35.501208 flytekitplugins_flyteinteractive-1.12.0b6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-04-24 18:30:04.000000 flytekitplugins_flyteinteractive-1.12.0b6/tests/test_flyteinteractive_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12906 2024-04-24 18:30:04.000000 flytekitplugins_flyteinteractive-1.12.0b6/tests/test_flyteinteractive_vscode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-24 18:30:04.000000 flytekitplugins_flyteinteractive-1.12.0b6/tests/test_utils.py
```

### Comparing `flytekitplugins-flyteinteractive-1.12.0b5/PKG-INFO` & `flytekitplugins_flyteinteractive-1.12.0b6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-flyteinteractive
-Version: 1.12.0b5
+Version: 1.12.0b6
 Summary: This package holds the flyteinteractive plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-flyteinteractive-1.12.0b5/README.md` & `flytekitplugins_flyteinteractive-1.12.0b6/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-flyteinteractive-1.12.0b5/flytekitplugins/flyteinteractive/__init__.py` & `flytekitplugins_flyteinteractive-1.12.0b6/flytekitplugins/flyteinteractive/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-flyteinteractive-1.12.0b5/flytekitplugins/flyteinteractive/jupyter_lib/decorator.py` & `flytekitplugins_flyteinteractive-1.12.0b6/flytekitplugins/flyteinteractive/jupyter_lib/decorator.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-flyteinteractive-1.12.0b5/flytekitplugins/flyteinteractive/utils.py` & `flytekitplugins_flyteinteractive-1.12.0b6/flytekitplugins/flyteinteractive/utils.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-flyteinteractive-1.12.0b5/flytekitplugins/flyteinteractive/vscode_lib/config.py` & `flytekitplugins_flyteinteractive-1.12.0b6/flytekitplugins/flyteinteractive/vscode_lib/config.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-flyteinteractive-1.12.0b5/flytekitplugins/flyteinteractive/vscode_lib/decorator.py` & `flytekitplugins_flyteinteractive-1.12.0b6/flytekitplugins/flyteinteractive/vscode_lib/decorator.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-flyteinteractive-1.12.0b5/flytekitplugins/flyteinteractive/vscode_lib/vscode_constants.py` & `flytekitplugins_flyteinteractive-1.12.0b6/flytekitplugins/flyteinteractive/vscode_lib/vscode_constants.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-flyteinteractive-1.12.0b5/flytekitplugins_flyteinteractive.egg-info/PKG-INFO` & `flytekitplugins_flyteinteractive-1.12.0b6/flytekitplugins_flyteinteractive.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-flyteinteractive
-Version: 1.12.0b5
+Version: 1.12.0b6
 Summary: This package holds the flyteinteractive plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-flyteinteractive-1.12.0b5/flytekitplugins_flyteinteractive.egg-info/SOURCES.txt` & `flytekitplugins_flyteinteractive-1.12.0b6/flytekitplugins_flyteinteractive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flytekitplugins-flyteinteractive-1.12.0b5/setup.py` & `flytekitplugins_flyteinteractive-1.12.0b6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "flyteinteractive"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.1.0b0,<2.0.0", "jupyter"]
 
-__version__ = "1.12.0b5"
+__version__ = "1.12.0b6"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This package holds the flyteinteractive plugins for flytekit",
```

### Comparing `flytekitplugins-flyteinteractive-1.12.0b5/tests/test_flyteinteractive_jupyter.py` & `flytekitplugins_flyteinteractive-1.12.0b6/tests/test_flyteinteractive_jupyter.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-flyteinteractive-1.12.0b5/tests/test_flyteinteractive_vscode.py` & `flytekitplugins_flyteinteractive-1.12.0b6/tests/test_flyteinteractive_vscode.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-flyteinteractive-1.12.0b5/tests/test_utils.py` & `flytekitplugins_flyteinteractive-1.12.0b6/tests/test_utils.py`

 * *Files identical despite different names*

