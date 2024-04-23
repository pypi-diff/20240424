# Comparing `tmp/tsty-0.0.5.tar.gz` & `tmp/tsty-0.0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsty-0.0.5.tar", last modified: Tue Apr 23 21:26:13 2024, max compression
+gzip compressed data, was "tsty-0.0.5.1.tar", last modified: Tue Apr 23 21:38:01 2024, max compression
```

## Comparing `tsty-0.0.5.tar` & `tsty-0.0.5.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 dan        (502) staff       (20)        0 2024-04-23 21:26:13.649259 tsty-0.0.5/
--rw-r--r--   0 dan        (502) staff       (20)     2285 2024-04-23 21:26:13.648765 tsty-0.0.5/PKG-INFO
--rw-r--r--   0 dan        (502) staff       (20)     1446 2024-04-23 21:24:50.000000 tsty-0.0.5/README.md
--rw-r--r--   0 dan        (502) staff       (20)       38 2024-04-23 21:26:13.649383 tsty-0.0.5/setup.cfg
--rw-r--r--   0 dan        (502) staff       (20)     1276 2024-04-23 21:25:24.000000 tsty-0.0.5/setup.py
-drwxr-xr-x   0 dan        (502) staff       (20)        0 2024-04-23 21:26:13.642966 tsty-0.0.5/tests/
--rw-r--r--   0 dan        (502) staff       (20)      246 2024-04-23 18:27:43.000000 tsty-0.0.5/tests/test_apple.py
--rw-r--r--   0 dan        (502) staff       (20)     3938 2024-04-23 21:24:58.000000 tsty-0.0.5/tests/test_cli.py
-drwxr-xr-x   0 dan        (502) staff       (20)        0 2024-04-23 21:26:13.644630 tsty-0.0.5/tsty/
--rw-r--r--   0 dan        (502) staff       (20)        0 2024-04-23 16:04:47.000000 tsty-0.0.5/tsty/__init__.py
--rw-r--r--   0 dan        (502) staff       (20)       59 2024-04-23 16:04:47.000000 tsty-0.0.5/tsty/__main__.py
--rwxr-xr-x   0 dan        (502) staff       (20)     5565 2024-04-23 21:24:58.000000 tsty-0.0.5/tsty/cli.py
-drwxr-xr-x   0 dan        (502) staff       (20)        0 2024-04-23 21:26:13.647508 tsty-0.0.5/tsty.egg-info/
--rw-r--r--   0 dan        (502) staff       (20)     2285 2024-04-23 21:26:13.000000 tsty-0.0.5/tsty.egg-info/PKG-INFO
--rw-r--r--   0 dan        (502) staff       (20)      272 2024-04-23 21:26:13.000000 tsty-0.0.5/tsty.egg-info/SOURCES.txt
--rw-r--r--   0 dan        (502) staff       (20)        1 2024-04-23 21:26:13.000000 tsty-0.0.5/tsty.egg-info/dependency_links.txt
--rw-r--r--   0 dan        (502) staff       (20)       38 2024-04-23 21:26:13.000000 tsty-0.0.5/tsty.egg-info/entry_points.txt
--rw-r--r--   0 dan        (502) staff       (20)      146 2024-04-23 21:26:13.000000 tsty-0.0.5/tsty.egg-info/requires.txt
--rw-r--r--   0 dan        (502) staff       (20)        5 2024-04-23 21:26:13.000000 tsty-0.0.5/tsty.egg-info/top_level.txt
+drwxr-xr-x   0 dan        (502) staff       (20)        0 2024-04-23 21:38:01.908702 tsty-0.0.5.1/
+-rw-r--r--   0 dan        (502) staff       (20)     2287 2024-04-23 21:38:01.908028 tsty-0.0.5.1/PKG-INFO
+-rw-r--r--   0 dan        (502) staff       (20)     1446 2024-04-23 21:24:50.000000 tsty-0.0.5.1/README.md
+-rw-r--r--   0 dan        (502) staff       (20)       38 2024-04-23 21:38:01.908847 tsty-0.0.5.1/setup.cfg
+-rw-r--r--   0 dan        (502) staff       (20)     1278 2024-04-23 21:32:53.000000 tsty-0.0.5.1/setup.py
+drwxr-xr-x   0 dan        (502) staff       (20)        0 2024-04-23 21:38:01.899621 tsty-0.0.5.1/tests/
+-rw-r--r--   0 dan        (502) staff       (20)      246 2024-04-23 18:27:43.000000 tsty-0.0.5.1/tests/test_apple.py
+-rw-r--r--   0 dan        (502) staff       (20)     3938 2024-04-23 21:24:58.000000 tsty-0.0.5.1/tests/test_cli.py
+drwxr-xr-x   0 dan        (502) staff       (20)        0 2024-04-23 21:38:01.902057 tsty-0.0.5.1/tsty/
+-rw-r--r--   0 dan        (502) staff       (20)        0 2024-04-23 16:04:47.000000 tsty-0.0.5.1/tsty/__init__.py
+-rw-r--r--   0 dan        (502) staff       (20)       59 2024-04-23 21:31:35.000000 tsty-0.0.5.1/tsty/__main__.py
+-rwxr-xr-x   0 dan        (502) staff       (20)     5557 2024-04-23 21:32:37.000000 tsty-0.0.5.1/tsty/cli.py
+drwxr-xr-x   0 dan        (502) staff       (20)        0 2024-04-23 21:38:01.905869 tsty-0.0.5.1/tsty.egg-info/
+-rw-r--r--   0 dan        (502) staff       (20)     2287 2024-04-23 21:38:01.000000 tsty-0.0.5.1/tsty.egg-info/PKG-INFO
+-rw-r--r--   0 dan        (502) staff       (20)      272 2024-04-23 21:38:01.000000 tsty-0.0.5.1/tsty.egg-info/SOURCES.txt
+-rw-r--r--   0 dan        (502) staff       (20)        1 2024-04-23 21:38:01.000000 tsty-0.0.5.1/tsty.egg-info/dependency_links.txt
+-rw-r--r--   0 dan        (502) staff       (20)       38 2024-04-23 21:38:01.000000 tsty-0.0.5.1/tsty.egg-info/entry_points.txt
+-rw-r--r--   0 dan        (502) staff       (20)      146 2024-04-23 21:38:01.000000 tsty-0.0.5.1/tsty.egg-info/requires.txt
+-rw-r--r--   0 dan        (502) staff       (20)        5 2024-04-23 21:38:01.000000 tsty-0.0.5.1/tsty.egg-info/top_level.txt
```

### Comparing `tsty-0.0.5/PKG-INFO` & `tsty-0.0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsty
-Version: 0.0.5
+Version: 0.0.5.1
 Summary: A simple command-line utility for changing your terminal colors
 Home-page: https://github.com/dannguyen/tsty
 Author: Dan Nguyen
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.dannguyen/dannguyen/tsty/issues
 Project-URL: CI, https://github.com/dannguyen/tsty/actions
 Project-URL: Changelog, https://github.com/dannguyen/tsty/releases
```

### Comparing `tsty-0.0.5/README.md` & `tsty-0.0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `tsty-0.0.5/setup.py` & `tsty-0.0.5.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.0.5"
+VERSION = "0.0.5.1"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
```

### Comparing `tsty-0.0.5/tests/test_cli.py` & `tsty-0.0.5.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `tsty-0.0.5/tsty/cli.py` & `tsty-0.0.5.1/tsty/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 import click
 from click_default_group import DefaultGroup
 from functools import wraps
 
 from typing import Tuple, List, Union
 
-from tsty.utils import apple
-from tsty.utils.common import COLOR_PRESETS, resolve_fuzzy_color_preset_name
+from .utils import apple
+from .utils.common import COLOR_PRESETS, resolve_fuzzy_color_preset_name
 
 
 def load_quiet_option(func):
     """Decorator to add a quiet option to a command."""
 
     @click.option("--quiet", "-q", is_flag=True, help="Silence verbose stderr output.")
     @wraps(func)
```

### Comparing `tsty-0.0.5/tsty.egg-info/PKG-INFO` & `tsty-0.0.5.1/tsty.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsty
-Version: 0.0.5
+Version: 0.0.5.1
 Summary: A simple command-line utility for changing your terminal colors
 Home-page: https://github.com/dannguyen/tsty
 Author: Dan Nguyen
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.dannguyen/dannguyen/tsty/issues
 Project-URL: CI, https://github.com/dannguyen/tsty/actions
 Project-URL: Changelog, https://github.com/dannguyen/tsty/releases
```

