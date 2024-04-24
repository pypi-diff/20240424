# Comparing `tmp/argtoml-0.4.4.tar.gz` & `tmp/argtoml-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argtoml-0.4.4.tar", last modified: Wed Jan  3 14:17:40 2024, max compression
+gzip compressed data, was "argtoml-0.5.0.tar", last modified: Wed Apr 24 13:24:24 2024, max compression
```

## Comparing `argtoml-0.4.4.tar` & `argtoml-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 gum       (1001) gum       (1001)        0 2024-01-03 14:17:40.993907 argtoml-0.4.4/
--rw-r--r--   0 gum       (1001) gum       (1001)     1069 2023-11-17 14:23:09.000000 argtoml-0.4.4/LICENSE
--rw-r--r--   0 gum       (1001) gum       (1001)     3792 2024-01-03 14:17:40.993907 argtoml-0.4.4/PKG-INFO
--rw-r--r--   0 gum       (1001) gum       (1001)     3218 2023-12-26 14:25:11.000000 argtoml-0.4.4/README.md
-drwxr-xr-x   0 gum       (1001) gum       (1001)        0 2024-01-03 14:17:40.990574 argtoml-0.4.4/argtoml/
--rw-r--r--   0 gum       (1001) gum       (1001)       92 2023-11-17 14:23:09.000000 argtoml-0.4.4/argtoml/__init__.py
--rw-r--r--   0 gum       (1001) gum       (1001)    10931 2024-01-03 14:00:13.000000 argtoml-0.4.4/argtoml/main.py
-drwxr-xr-x   0 gum       (1001) gum       (1001)        0 2024-01-03 14:17:40.993907 argtoml-0.4.4/argtoml.egg-info/
--rw-r--r--   0 gum       (1001) gum       (1001)     3792 2024-01-03 14:17:40.000000 argtoml-0.4.4/argtoml.egg-info/PKG-INFO
--rw-r--r--   0 gum       (1001) gum       (1001)      250 2024-01-03 14:17:40.000000 argtoml-0.4.4/argtoml.egg-info/SOURCES.txt
--rw-r--r--   0 gum       (1001) gum       (1001)        1 2024-01-03 14:17:40.000000 argtoml-0.4.4/argtoml.egg-info/dependency_links.txt
--rw-r--r--   0 gum       (1001) gum       (1001)       16 2024-01-03 14:17:40.000000 argtoml-0.4.4/argtoml.egg-info/requires.txt
--rw-r--r--   0 gum       (1001) gum       (1001)        8 2024-01-03 14:17:40.000000 argtoml-0.4.4/argtoml.egg-info/top_level.txt
--rw-r--r--   0 gum       (1001) gum       (1001)     1003 2024-01-03 14:01:10.000000 argtoml-0.4.4/pyproject.toml
--rw-r--r--   0 gum       (1001) gum       (1001)       38 2024-01-03 14:17:40.993907 argtoml-0.4.4/setup.cfg
--rw-r--r--   0 gum       (1001) gum       (1001)       61 2023-11-17 14:23:09.000000 argtoml-0.4.4/setup.py
-drwxr-xr-x   0 gum       (1001) gum       (1001)        0 2024-01-03 14:17:40.993907 argtoml-0.4.4/tests/
--rw-r--r--   0 gum       (1001) gum       (1001)      218 2023-11-17 14:23:09.000000 argtoml-0.4.4/tests/test_main.py
+drwxr-xr-x   0 gum       (1001) gum       (1001)        0 2024-04-24 13:24:24.796624 argtoml-0.5.0/
+-rw-r--r--   0 gum       (1001) gum       (1001)     1069 2023-11-17 14:23:09.000000 argtoml-0.5.0/LICENSE
+-rw-r--r--   0 gum       (1001) gum       (1001)     3731 2024-04-24 13:24:24.796624 argtoml-0.5.0/PKG-INFO
+-rw-r--r--   0 gum       (1001) gum       (1001)     3218 2023-12-26 14:25:11.000000 argtoml-0.5.0/README.md
+drwxr-xr-x   0 gum       (1001) gum       (1001)        0 2024-04-24 13:24:24.796624 argtoml-0.5.0/argtoml/
+-rw-r--r--   0 gum       (1001) gum       (1001)       57 2024-01-22 12:17:21.000000 argtoml-0.5.0/argtoml/__init__.py
+-rw-r--r--   0 gum       (1001) gum       (1001)     2802 2024-02-18 11:46:36.000000 argtoml-0.5.0/argtoml/__main__.py
+-rw-r--r--   0 gum       (1001) gum       (1001)     3076 2024-01-22 13:41:14.000000 argtoml-0.5.0/argtoml/locate.py
+-rw-r--r--   0 gum       (1001) gum       (1001)    10953 2024-01-21 19:47:11.000000 argtoml-0.5.0/argtoml/main.py
+-rw-r--r--   0 gum       (1001) gum       (1001)     4920 2024-01-22 15:05:51.000000 argtoml-0.5.0/argtoml/opt.py
+drwxr-xr-x   0 gum       (1001) gum       (1001)        0 2024-04-24 13:24:24.796624 argtoml-0.5.0/argtoml.egg-info/
+-rw-r--r--   0 gum       (1001) gum       (1001)     3731 2024-04-24 13:24:24.000000 argtoml-0.5.0/argtoml.egg-info/PKG-INFO
+-rw-r--r--   0 gum       (1001) gum       (1001)      273 2024-04-24 13:24:24.000000 argtoml-0.5.0/argtoml.egg-info/SOURCES.txt
+-rw-r--r--   0 gum       (1001) gum       (1001)        1 2024-04-24 13:24:24.000000 argtoml-0.5.0/argtoml.egg-info/dependency_links.txt
+-rw-r--r--   0 gum       (1001) gum       (1001)        8 2024-04-24 13:24:24.000000 argtoml-0.5.0/argtoml.egg-info/top_level.txt
+-rw-r--r--   0 gum       (1001) gum       (1001)      951 2024-01-22 12:17:53.000000 argtoml-0.5.0/pyproject.toml
+-rw-r--r--   0 gum       (1001) gum       (1001)       38 2024-04-24 13:24:24.796624 argtoml-0.5.0/setup.cfg
+-rw-r--r--   0 gum       (1001) gum       (1001)       61 2023-11-17 14:23:09.000000 argtoml-0.5.0/setup.py
+drwxr-xr-x   0 gum       (1001) gum       (1001)        0 2024-04-24 13:24:24.796624 argtoml-0.5.0/tests/
+-rw-r--r--   0 gum       (1001) gum       (1001)      218 2023-11-17 14:23:09.000000 argtoml-0.5.0/tests/test_main.py
```

### Comparing `argtoml-0.4.4/LICENSE` & `argtoml-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `argtoml-0.4.4/PKG-INFO` & `argtoml-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: argtoml
-Version: 0.4.4
+Version: 0.5.0
 Summary: Add the keys from a .toml file to your CLI as arguments. Their values default to the values in the .toml file.
 Author-email: Jochem Hölscher <a.fake@e.mail>
 Project-URL: homepage, https://github.com/JJJHolscher/argtoml
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Provides-Extra: save
-Requires-Dist: tomli_w; extra == "save"
 
 # README
 
 The `argtoml` package wraps around `argparse`.
 It adds the content of a toml file to the cli options.
 After parsing, it creates a `types.SimpleNameSpace` object.
```

### Comparing `argtoml-0.4.4/README.md` & `argtoml-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `argtoml-0.4.4/argtoml/main.py` & `argtoml-0.5.0/argtoml/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,21 @@
                 f"--{prefix}{key}",
                 required=False,
                 type=type_,
                 help=f"defaults to {value}",
             )
 
 
-def fill_toml_args(args, toml, prefix="", filled=False, path: Optional[Path] = None):
+def fill_toml_args(
+    args,
+    toml,
+    prefix="",
+    filled=False,
+    path: Optional[Path] = None
+):
     namespace = SimpleNamespace()
     for raw_key, value in toml.items():
         # Check if the user provided the same key but with dashes instead of underscores.
         key = raw_key.replace("-", "_")
         key_str = prefix + "." + key if prefix else key
         # Boolean variables have 2 arguments.
         alt_key_str = prefix + ".no_" + key if prefix else "no_" + key
```

### Comparing `argtoml-0.4.4/argtoml.egg-info/PKG-INFO` & `argtoml-0.5.0/argtoml.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: argtoml
-Version: 0.4.4
+Version: 0.5.0
 Summary: Add the keys from a .toml file to your CLI as arguments. Their values default to the values in the .toml file.
 Author-email: Jochem Hölscher <a.fake@e.mail>
 Project-URL: homepage, https://github.com/JJJHolscher/argtoml
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Provides-Extra: save
-Requires-Dist: tomli_w; extra == "save"
 
 # README
 
 The `argtoml` package wraps around `argparse`.
 It adds the content of a toml file to the cli options.
 After parsing, it creates a `types.SimpleNameSpace` object.
```

### Comparing `argtoml-0.4.4/pyproject.toml` & `argtoml-0.5.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 
 [project]
 name = "argtoml"
-version = "0.4.4"
+version = "0.5.0"
 description = "Add the keys from a .toml file to your CLI as arguments. Their values default to the values in the .toml file."
 dynamic = ["readme"]
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
-[project.optional-dependencies]
-save = ["tomli_w"]
-
 [git]
 github = "https://github.com/JJJHolscher/argtoml"
 
 [project.urls]
 homepage = "https://github.com/JJJHolscher/argtoml"
 
 [[project.authors]]
```

