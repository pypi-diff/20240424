# Comparing `tmp/toml_union-1.0.2.tar.gz` & `tmp/toml_union-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toml_union-1.0.2.tar", last modified: Wed Dec 27 11:51:51 2023, max compression
+gzip compressed data, was "toml_union-1.0.3.tar", last modified: Wed Apr 24 19:48:39 2024, max compression
```

## Comparing `toml_union-1.0.2.tar` & `toml_union-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-sr-x   0 pasa      (1002) dreamdocs   (515)        0 2023-12-27 11:51:51.429645 toml_union-1.0.2/
--rw-r--r--   0 pasa      (1002) dreamdocs   (515)     1072 2023-12-27 09:33:44.000000 toml_union-1.0.2/LICENSE
--rw-r--r--   0 pasa      (1002) dreamdocs   (515)     6467 2023-12-27 11:51:51.429645 toml_union-1.0.2/PKG-INFO
--rw-r--r--   0 pasa      (1002) dreamdocs   (515)     5893 2023-12-27 11:24:03.000000 toml_union-1.0.2/README.md
--rw-r--r--   0 pasa      (1002) dreamdocs   (515)       38 2023-12-27 11:51:51.429645 toml_union-1.0.2/setup.cfg
--rw-r--r--   0 pasa      (1002) dreamdocs   (515)     1223 2023-12-27 11:37:32.000000 toml_union-1.0.2/setup.py
-drwxr-sr-x   0 pasa      (1002) dreamdocs   (515)        0 2023-12-27 11:51:51.427645 toml_union-1.0.2/toml_union/
--rw-r--r--   0 pasa      (1002) dreamdocs   (515)      132 2023-12-27 11:00:27.000000 toml_union-1.0.2/toml_union/__init__.py
--rw-r--r--   0 pasa      (1002) dreamdocs   (515)    19753 2023-12-27 11:15:16.000000 toml_union-1.0.2/toml_union/toml_union.py
-drwxr-sr-x   0 pasa      (1002) dreamdocs   (515)        0 2023-12-27 11:51:51.429645 toml_union-1.0.2/toml_union.egg-info/
--rw-r--r--   0 pasa      (1002) dreamdocs   (515)     6467 2023-12-27 11:51:51.000000 toml_union-1.0.2/toml_union.egg-info/PKG-INFO
--rw-r--r--   0 pasa      (1002) dreamdocs   (515)      280 2023-12-27 11:51:51.000000 toml_union-1.0.2/toml_union.egg-info/SOURCES.txt
--rw-r--r--   0 pasa      (1002) dreamdocs   (515)        1 2023-12-27 11:51:51.000000 toml_union-1.0.2/toml_union.egg-info/dependency_links.txt
--rw-r--r--   0 pasa      (1002) dreamdocs   (515)       58 2023-12-27 11:51:51.000000 toml_union-1.0.2/toml_union.egg-info/entry_points.txt
--rw-r--r--   0 pasa      (1002) dreamdocs   (515)        5 2023-12-27 11:51:51.000000 toml_union-1.0.2/toml_union.egg-info/requires.txt
--rw-r--r--   0 pasa      (1002) dreamdocs   (515)       11 2023-12-27 11:51:51.000000 toml_union-1.0.2/toml_union.egg-info/top_level.txt
+drwxrwsr-x   0 pasa      (1002) dreamdocs   (515)        0 2024-04-24 19:48:39.636309 toml_union-1.0.3/
+-rw-rw-r--   0 pasa      (1002) dreamdocs   (515)     1072 2023-12-27 09:33:44.000000 toml_union-1.0.3/LICENSE
+-rw-rw-r--   0 pasa      (1002) dreamdocs   (515)     6479 2024-04-24 19:48:39.636309 toml_union-1.0.3/PKG-INFO
+-rw-r--r--   0 pasa      (1002) dreamdocs   (515)     5905 2024-02-01 18:31:05.000000 toml_union-1.0.3/README.md
+-rw-rw-r--   0 pasa      (1002) dreamdocs   (515)       38 2024-04-24 19:48:39.636309 toml_union-1.0.3/setup.cfg
+-rw-rw-r--   0 pasa      (1002) dreamdocs   (515)     1223 2023-12-27 11:59:24.000000 toml_union-1.0.3/setup.py
+drwxrwsr-x   0 pasa      (1002) dreamdocs   (515)        0 2024-04-24 19:48:39.634310 toml_union-1.0.3/toml_union/
+-rw-rw-r--   0 pasa      (1002) dreamdocs   (515)      132 2023-12-27 11:59:24.000000 toml_union-1.0.3/toml_union/__init__.py
+-rw-rw-r--   0 pasa      (1002) dreamdocs   (515)    20826 2024-04-24 19:46:36.000000 toml_union-1.0.3/toml_union/toml_union.py
+drwxrwsr-x   0 pasa      (1002) dreamdocs   (515)        0 2024-04-24 19:48:39.636309 toml_union-1.0.3/toml_union.egg-info/
+-rw-rw-r--   0 pasa      (1002) dreamdocs   (515)     6479 2024-04-24 19:48:39.000000 toml_union-1.0.3/toml_union.egg-info/PKG-INFO
+-rw-rw-r--   0 pasa      (1002) dreamdocs   (515)      280 2024-04-24 19:48:39.000000 toml_union-1.0.3/toml_union.egg-info/SOURCES.txt
+-rw-rw-r--   0 pasa      (1002) dreamdocs   (515)        1 2024-04-24 19:48:39.000000 toml_union-1.0.3/toml_union.egg-info/dependency_links.txt
+-rw-rw-r--   0 pasa      (1002) dreamdocs   (515)       58 2024-04-24 19:48:39.000000 toml_union-1.0.3/toml_union.egg-info/entry_points.txt
+-rw-rw-r--   0 pasa      (1002) dreamdocs   (515)        5 2024-04-24 19:48:39.000000 toml_union-1.0.3/toml_union.egg-info/requires.txt
+-rw-rw-r--   0 pasa      (1002) dreamdocs   (515)       11 2024-04-24 19:48:39.000000 toml_union-1.0.3/toml_union.egg-info/top_level.txt
```

### Comparing `toml_union-1.0.2/LICENSE` & `toml_union-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `toml_union-1.0.2/PKG-INFO` & `toml_union-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toml_union
-Version: 1.0.2
+Version: 1.0.3
 Summary: Utils to merge *.toml files with conflicts highlighting
 Home-page: https://github.com/PasaOpasen/toml-union
 Author: Demetry Pascal
 Author-email: qtckpuhdsa@gmail.com
 Maintainer: Demetry Pascal
 License: MIT
 Keywords: toml,merge
@@ -29,15 +29,15 @@
 
 # About
 
 ```sh
 pip install toml-union
 ```
 
-This PyPI package is located in one script and combines several `*.toml` files (usially `pyproject.toml`) into one. If it finds some conflict between items, they are kept for manual review.
+This PyPI package is indeed located in one script and combines several `*.toml` files (usially `pyproject.toml`) into one. If it finds some conflicts between items, they will be kept for manual review.
 
 It has a docker image (`docker pull pasaopasen/toml-union`) and an [example](/examples/docker-test.sh) of its usage.
 
 ## Python usage example
 
 ```python
 from pathlib import Path
```

### Comparing `toml_union-1.0.2/README.md` & `toml_union-1.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 # About
 
 ```sh
 pip install toml-union
 ```
 
-This PyPI package is located in one script and combines several `*.toml` files (usially `pyproject.toml`) into one. If it finds some conflict between items, they are kept for manual review.
+This PyPI package is indeed located in one script and combines several `*.toml` files (usially `pyproject.toml`) into one. If it finds some conflicts between items, they will be kept for manual review.
 
 It has a docker image (`docker pull pasaopasen/toml-union`) and an [example](/examples/docker-test.sh) of its usage.
 
 ## Python usage example
 
 ```python
 from pathlib import Path
```

### Comparing `toml_union-1.0.2/setup.py` & `toml_union-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `toml_union-1.0.2/toml_union/toml_union.py` & `toml_union-1.0.3/toml_union/toml_union.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from pathlib import Path
 import copy
 import json
 from collections import defaultdict
 from dataclasses import dataclass
 from functools import reduce
 import tempfile
+import pprint
 
 import argparse
 
 import toml
 
 
 #region TYPES
@@ -378,23 +379,48 @@
     """
 
     d1: DATA_DICT = copy.deepcopy(d1)
 
     for key, v2 in d2.items():
         if key in d1:
             v1 = d1[key]
-            assert type(v1) is type(v2), f"incompatible types {v1} and {v2}"
+            if type(v1) is type(v2):
 
-            if isinstance(v1, list):
-                d1[key] = TomlValue.union_list(v1 + v2)
-            elif isinstance(v1, dict):
-                d1[key] = union_2_data_dicts(v1, v2)
-            else:
-                assert isinstance(v1, TomlValue)
-                d1[key].update(v2)
+                if isinstance(v1, list):
+                    d1[key] = TomlValue.union_list(v1 + v2)
+                elif isinstance(v1, dict):
+                    d1[key] = union_2_data_dicts(v1, v2)
+                else:
+                    assert isinstance(v1, TomlValue)
+                    v1.update(v2)
+
+                continue
+
+            # special versions case like
+            #   httpx = {extras = ["socks", "brotli", "http2"], version = "^0.26"}
+            #       vs
+            #   httpx = "^0.27.0"
+            if isinstance(v1, (dict, TomlValue)) and isinstance(v2, (dict, TomlValue)):
+                # here -- on object is dict and other is TomlValue
+                if isinstance(v1, dict) and 'version' in v1:
+                    version = v1['version']
+                    if isinstance(version, TomlValue):
+                        version.update(v2)
+                        continue
+
+                if isinstance(v2, dict) and 'version' in v2:
+                    version = v2['version']
+                    if isinstance(version, TomlValue):
+                        version.update(v1)  # update version object
+                        d1[key] = v2  # assign v2 object to v1 dictionary
+                        continue
+
+            raise ValueError(
+                f"{key}: incompatible types\n{pprint.pformat(v1)}\n\tand\n{pprint.pformat(v2)}"
+            )
 
         else:
             d1[key] = v2
 
     return d1
```

### Comparing `toml_union-1.0.2/toml_union.egg-info/PKG-INFO` & `toml_union-1.0.3/toml_union.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toml-union
-Version: 1.0.2
+Version: 1.0.3
 Summary: Utils to merge *.toml files with conflicts highlighting
 Home-page: https://github.com/PasaOpasen/toml-union
 Author: Demetry Pascal
 Author-email: qtckpuhdsa@gmail.com
 Maintainer: Demetry Pascal
 License: MIT
 Keywords: toml,merge
@@ -29,15 +29,15 @@
 
 # About
 
 ```sh
 pip install toml-union
 ```
 
-This PyPI package is located in one script and combines several `*.toml` files (usially `pyproject.toml`) into one. If it finds some conflict between items, they are kept for manual review.
+This PyPI package is indeed located in one script and combines several `*.toml` files (usially `pyproject.toml`) into one. If it finds some conflicts between items, they will be kept for manual review.
 
 It has a docker image (`docker pull pasaopasen/toml-union`) and an [example](/examples/docker-test.sh) of its usage.
 
 ## Python usage example
 
 ```python
 from pathlib import Path
```

