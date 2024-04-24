# Comparing `tmp/packse-0.3.8.tar.gz` & `tmp/packse-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packse-0.3.8.tar", max compression
+gzip compressed data, was "packse-0.3.9.tar", max compression
```

## Comparing `packse-0.3.8.tar` & `packse-0.3.9.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0    11356 2024-03-14 18:02:48.770448 packse-0.3.8/LICENSE-APACHE
--rw-r--r--   0        0        0     1077 2024-03-14 18:02:48.770448 packse-0.3.8/LICENSE-MIT
--rw-r--r--   0        0        0     6310 2024-03-14 18:02:48.770448 packse-0.3.8/README.md
--rw-r--r--   0        0        0     1455 2024-03-14 18:02:57.326388 packse-0.3.8/pyproject.toml
--rw-r--r--   0        0        0      257 2024-03-14 18:02:48.770448 packse-0.3.8/src/packse/__init__.py
--rw-r--r--   0        0        0      121 2024-03-14 18:02:48.770448 packse-0.3.8/src/packse/__main__.py
--rw-r--r--   0        0        0    13116 2024-03-14 18:02:48.770448 packse-0.3.8/src/packse/build.py
--rw-r--r--   0        0        0    15562 2024-03-14 18:02:48.774448 packse-0.3.8/src/packse/cli.py
--rw-r--r--   0        0        0     3421 2024-03-14 18:02:48.774448 packse-0.3.8/src/packse/error.py
--rw-r--r--   0        0        0     2327 2024-03-14 18:02:48.774448 packse-0.3.8/src/packse/fetch.py
--rw-r--r--   0        0        0    11200 2024-03-14 18:02:48.774448 packse-0.3.8/src/packse/index.py
--rw-r--r--   0        0        0     6516 2024-03-14 18:02:48.774448 packse-0.3.8/src/packse/inspect.py
--rw-r--r--   0        0        0     2085 2024-03-14 18:02:48.774448 packse-0.3.8/src/packse/list.py
--rw-r--r--   0        0        0     7455 2024-03-14 18:02:48.774448 packse-0.3.8/src/packse/publish.py
--rw-r--r--   0        0        0     9869 2024-03-14 18:02:48.774448 packse-0.3.8/src/packse/scenario.py
--rw-r--r--   0        0        0     3439 2024-03-14 18:02:48.774448 packse-0.3.8/src/packse/serve.py
--rw-r--r--   0        0        0     2738 2024-03-14 18:02:48.774448 packse-0.3.8/src/packse/template.py
--rw-r--r--   0        0        0        0 2024-03-14 18:02:48.774448 packse-0.3.8/src/packse/templates/README.md
--rw-r--r--   0        0        0      115 2024-03-14 18:02:48.774448 packse-0.3.8/src/packse/templates/__init__.py
--rw-r--r--   0        0        0      455 2024-03-14 18:02:48.774448 packse-0.3.8/src/packse/templates/index/simple-html/[[ scenarios ]][[ packages ]]{{ name}}/index.html
--rw-r--r--   0        0        0      197 2024-03-14 18:02:48.774448 packse-0.3.8/src/packse/templates/index/simple-html/index.html
--rw-r--r--   0        0        0      108 2024-03-14 18:02:48.774448 packse-0.3.8/src/packse/templates/package/template.toml
--rw-r--r--   0        0        0      594 2024-03-14 18:02:48.774448 packse-0.3.8/src/packse/templates/package/{{ package-name }}-{{ version }}/pyproject.toml
--rw-r--r--   0        0        0       30 2024-03-14 18:02:48.774448 packse-0.3.8/src/packse/templates/package/{{ package-name }}-{{ version }}/src/{{ module-name }}/__init__.py
--rw-r--r--   0        0        0     6917 2024-03-14 18:02:48.774448 packse-0.3.8/src/packse/view.py
--rw-r--r--   0        0        0     7593 1970-01-01 00:00:00.000000 packse-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-03-14 19:46:49.347565 packse-0.3.9/LICENSE-APACHE
+-rw-r--r--   0        0        0     1077 2024-03-14 19:46:49.347565 packse-0.3.9/LICENSE-MIT
+-rw-r--r--   0        0        0     6310 2024-03-14 19:46:49.347565 packse-0.3.9/README.md
+-rw-r--r--   0        0        0     1455 2024-03-14 19:46:59.555553 packse-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0      257 2024-03-14 19:46:49.347565 packse-0.3.9/src/packse/__init__.py
+-rw-r--r--   0        0        0      121 2024-03-14 19:46:49.347565 packse-0.3.9/src/packse/__main__.py
+-rw-r--r--   0        0        0    13116 2024-03-14 19:46:49.347565 packse-0.3.9/src/packse/build.py
+-rw-r--r--   0        0        0    15562 2024-03-14 19:46:49.347565 packse-0.3.9/src/packse/cli.py
+-rw-r--r--   0        0        0     3421 2024-03-14 19:46:49.347565 packse-0.3.9/src/packse/error.py
+-rw-r--r--   0        0        0     2327 2024-03-14 19:46:49.347565 packse-0.3.9/src/packse/fetch.py
+-rw-r--r--   0        0        0    11200 2024-03-14 19:46:49.347565 packse-0.3.9/src/packse/index.py
+-rw-r--r--   0        0        0     6516 2024-03-14 19:46:49.347565 packse-0.3.9/src/packse/inspect.py
+-rw-r--r--   0        0        0     2085 2024-03-14 19:46:49.347565 packse-0.3.9/src/packse/list.py
+-rw-r--r--   0        0        0     7455 2024-03-14 19:46:49.351565 packse-0.3.9/src/packse/publish.py
+-rw-r--r--   0        0        0     9869 2024-03-14 19:46:49.351565 packse-0.3.9/src/packse/scenario.py
+-rw-r--r--   0        0        0     3439 2024-03-14 19:46:49.351565 packse-0.3.9/src/packse/serve.py
+-rw-r--r--   0        0        0     2901 2024-03-14 19:46:49.351565 packse-0.3.9/src/packse/template.py
+-rw-r--r--   0        0        0        0 2024-03-14 19:46:49.351565 packse-0.3.9/src/packse/templates/README.md
+-rw-r--r--   0        0        0      115 2024-03-14 19:46:49.351565 packse-0.3.9/src/packse/templates/__init__.py
+-rw-r--r--   0        0        0      455 2024-03-14 19:46:49.351565 packse-0.3.9/src/packse/templates/index/simple-html/[[ scenarios ]][[ packages ]]{{ name}}/index.html
+-rw-r--r--   0        0        0      197 2024-03-14 19:46:49.351565 packse-0.3.9/src/packse/templates/index/simple-html/index.html
+-rw-r--r--   0        0        0      108 2024-03-14 19:46:49.351565 packse-0.3.9/src/packse/templates/package/template.toml
+-rw-r--r--   0        0        0       18 2024-03-14 19:46:49.351565 packse-0.3.9/src/packse/templates/package/{{ package-name }}-{{ version }}/.gitignore
+-rw-r--r--   0        0        0      594 2024-03-14 19:46:49.351565 packse-0.3.9/src/packse/templates/package/{{ package-name }}-{{ version }}/pyproject.toml
+-rw-r--r--   0        0        0       30 2024-03-14 19:46:49.351565 packse-0.3.9/src/packse/templates/package/{{ package-name }}-{{ version }}/src/{{ module-name }}/__init__.py
+-rw-r--r--   0        0        0     6917 2024-03-14 19:46:49.351565 packse-0.3.9/src/packse/view.py
+-rw-r--r--   0        0        0     7593 1970-01-01 00:00:00.000000 packse-0.3.9/PKG-INFO
```

### Comparing `packse-0.3.8/LICENSE-APACHE` & `packse-0.3.9/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `packse-0.3.8/LICENSE-MIT` & `packse-0.3.9/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `packse-0.3.8/README.md` & `packse-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `packse-0.3.8/pyproject.toml` & `packse-0.3.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "packse"
-version = "0.3.8"
+version = "0.3.9"
 description = ""
 authors = ["Zanie <contact@zanie.dev>"]
 readme = "README.md"
 keywords = [
   "uv", "packse", "requirements", "packaging", "testing"
 ]
 classifiers = [
```

### Comparing `packse-0.3.8/src/packse/build.py` & `packse-0.3.9/src/packse/build.py`

 * *Files identical despite different names*

### Comparing `packse-0.3.8/src/packse/cli.py` & `packse-0.3.9/src/packse/cli.py`

 * *Files identical despite different names*

### Comparing `packse-0.3.8/src/packse/error.py` & `packse-0.3.9/src/packse/error.py`

 * *Files identical despite different names*

### Comparing `packse-0.3.8/src/packse/fetch.py` & `packse-0.3.9/src/packse/fetch.py`

 * *Files identical despite different names*

### Comparing `packse-0.3.8/src/packse/index.py` & `packse-0.3.9/src/packse/index.py`

 * *Files identical despite different names*

### Comparing `packse-0.3.8/src/packse/inspect.py` & `packse-0.3.9/src/packse/inspect.py`

 * *Files identical despite different names*

### Comparing `packse-0.3.8/src/packse/list.py` & `packse-0.3.9/src/packse/list.py`

 * *Files identical despite different names*

### Comparing `packse-0.3.8/src/packse/publish.py` & `packse-0.3.9/src/packse/publish.py`

 * *Files identical despite different names*

### Comparing `packse-0.3.8/src/packse/scenario.py` & `packse-0.3.9/src/packse/scenario.py`

 * *Files identical despite different names*

### Comparing `packse-0.3.8/src/packse/serve.py` & `packse-0.3.9/src/packse/serve.py`

 * *Files identical despite different names*

### Comparing `packse-0.3.8/src/packse/template.py` & `packse-0.3.9/src/packse/template.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import fnmatch
 import logging
 import re
 from pathlib import Path
 from typing import Any
 
 import chevron_blue
 import msgspec
@@ -29,15 +30,19 @@
 
 
 def create_from_template(
     destination: Path, template_name: str, variables: dict[str, Any]
 ) -> Path:
     template_path = __templates_path__ / template_name
     first_root = None
+    ignore_files = ["*.pyc"]
     for root, _, files in template_path.walk():
+        for ignore in ignore_files:
+            files = [file for file in files if not fnmatch.fnmatch(file, ignore)]
+
         for loop_root, scope in parse_loop(root, variables):
             # Determine the new directory path in the destination
             new_root = destination / Path(
                 chevron_blue.render(str(loop_root), scope, no_escape=True)
             ).relative_to(template_path)
 
             if new_root == destination:
```

### Comparing `packse-0.3.8/src/packse/templates/package/{{ package-name }}-{{ version }}/pyproject.toml` & `packse-0.3.9/src/packse/templates/package/{{ package-name }}-{{ version }}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `packse-0.3.8/src/packse/view.py` & `packse-0.3.9/src/packse/view.py`

 * *Files identical despite different names*

### Comparing `packse-0.3.8/PKG-INFO` & `packse-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packse
-Version: 0.3.8
+Version: 0.3.9
 Summary: 
 Keywords: uv,packse,requirements,packaging,testing
 Author: Zanie
 Author-email: contact@zanie.dev
 Requires-Python: >=3.12,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

