# Comparing `tmp/python_active_versions-1.9.0.tar.gz` & `tmp/python_active_versions-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_active_versions-1.9.0.tar", max compression
+gzip compressed data, was "python_active_versions-1.9.1.tar", max compression
```

## Comparing `python_active_versions-1.9.0.tar` & `python_active_versions-1.9.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0        0        0        0 2024-02-22 16:19:07.987486 python_active_versions-1.9.0/LICENSES/
--rw-r--r--   0        0        0     1257 2024-02-22 16:19:07.987486 python_active_versions-1.9.0/README.md
--rw-r--r--   0        0        0     6667 2024-02-22 16:19:07.991486 python_active_versions-1.9.0/pyproject.toml
--rw-r--r--   0        0        0      233 2024-02-22 16:19:07.991486 python_active_versions-1.9.0/python_active_versions/__init__.py
--rw-r--r--   0        0        0      144 2024-02-22 16:19:07.991486 python_active_versions-1.9.0/python_active_versions/cli_tools/__init__.py
--rw-r--r--   0        0        0     2602 2024-02-22 16:19:07.991486 python_active_versions-1.9.0/python_active_versions/cli_tools/cli.py
--rw-r--r--   0        0        0        1 2024-02-22 16:19:07.991486 python_active_versions-1.9.0/python_active_versions/py.typed
--rw-r--r--   0        0        0       77 2024-02-22 16:19:07.991486 python_active_versions-1.9.0/python_active_versions/py.typed.license
--rw-r--r--   0        0        0     2949 2024-02-22 16:19:07.991486 python_active_versions-1.9.0/python_active_versions/python_active_versions.py
--rw-r--r--   0        0        0      785 2024-02-22 16:19:07.991486 python_active_versions-1.9.0/python_active_versions/utility.py
--rw-r--r--   0        0        0      135 2024-02-22 16:19:07.991486 python_active_versions-1.9.0/tests/__init__.py
--rw-r--r--   0        0        0      368 2024-02-22 16:19:07.991486 python_active_versions-1.9.0/tests/conftest.py
--rw-r--r--   0        0        0     1471 2024-02-22 16:19:07.991486 python_active_versions-1.9.0/tests/test_python_active_versions.py
--rw-r--r--   0        0        0     1383 2024-02-22 16:19:07.991486 python_active_versions-1.9.0/tests/test_utils.py
--rw-r--r--   0        0        0     2702 1970-01-01 00:00:00.000000 python_active_versions-1.9.0/PKG-INFO
+drwxr-xr-x   0        0        0        0 2024-02-22 16:35:23.135630 python_active_versions-1.9.1/LICENSES/
+-rw-r--r--   0        0        0     1257 2024-02-22 16:35:23.135630 python_active_versions-1.9.1/README.md
+-rw-r--r--   0        0        0     6667 2024-02-22 16:35:23.135630 python_active_versions-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0      233 2024-02-22 16:35:23.135630 python_active_versions-1.9.1/python_active_versions/__init__.py
+-rw-r--r--   0        0        0      144 2024-02-22 16:35:23.135630 python_active_versions-1.9.1/python_active_versions/cli_tools/__init__.py
+-rw-r--r--   0        0        0     2598 2024-02-22 16:35:23.135630 python_active_versions-1.9.1/python_active_versions/cli_tools/cli.py
+-rw-r--r--   0        0        0        1 2024-02-22 16:35:23.135630 python_active_versions-1.9.1/python_active_versions/py.typed
+-rw-r--r--   0        0        0       77 2024-02-22 16:35:23.135630 python_active_versions-1.9.1/python_active_versions/py.typed.license
+-rw-r--r--   0        0        0     2949 2024-02-22 16:35:23.135630 python_active_versions-1.9.1/python_active_versions/python_active_versions.py
+-rw-r--r--   0        0        0      785 2024-02-22 16:35:23.135630 python_active_versions-1.9.1/python_active_versions/utility.py
+-rw-r--r--   0        0        0      135 2024-02-22 16:35:23.135630 python_active_versions-1.9.1/tests/__init__.py
+-rw-r--r--   0        0        0      368 2024-02-22 16:35:23.135630 python_active_versions-1.9.1/tests/conftest.py
+-rw-r--r--   0        0        0     1471 2024-02-22 16:35:23.135630 python_active_versions-1.9.1/tests/test_python_active_versions.py
+-rw-r--r--   0        0        0     1383 2024-02-22 16:35:23.135630 python_active_versions-1.9.1/tests/test_utils.py
+-rw-r--r--   0        0        0     2702 1970-01-01 00:00:00.000000 python_active_versions-1.9.1/PKG-INFO
```

### Comparing `python_active_versions-1.9.0/README.md` & `python_active_versions-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `python_active_versions-1.9.0/pyproject.toml` & `python_active_versions-1.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-FileCopyrightText: 2023 Gabriele Pongelli
 #
 # SPDX-License-Identifier: MIT
 
 [tool.poetry]
     name = "python-active-versions"
-    version = "1.9.0"
+    version = "1.9.1"
     homepage = "https://github.com/gpongelli/python-active-versions"
     repository = "https://github.com/gpongelli/python-active-versions"
     documentation = "https://gpongelli.github.io/python-active-versions/"
     description = "Gather active python versions."
     authors = ["Gabriele Pongelli <gabriele.pongelli@gmail.com>"]
     readme = "README.md"
     license =  "MIT"
@@ -115,15 +115,15 @@
     line_length = 120
     skip_gitignore = true
     # you can skip files as below
     #skip_glob = ["docs/conf.py", "path/*"]
 
 [tool.commitizen]
     name = "cz_conventional_commits"
-    version = "1.9.0"
+    version = "1.9.1"
     version_files = [
         "python_active_versions/__init__.py:__version__",
         "pyproject.toml:version"
     ]
     gpg_sign = true
     bump_message = 'Bump version: $current_version -> $new_version'
     update_changelog_on_bump = false
```

### Comparing `python_active_versions-1.9.0/python_active_versions/cli_tools/cli.py` & `python_active_versions-1.9.1/python_active_versions/cli_tools/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         default=False,
         show_default=True,
         help="Get Docker image info.",
     ),
 )
 @click.version_option(__version__)
 def get_python_versions(loglevel: str, docker: bool):
-    """Python extension for Code128 barcode generator library cli script.
+    """Cli script to show which are currently active python versions.
 
     Arguments:
         loglevel: set log level.
         docker: Include also info coming from docker's python active images.
     """
     _fnc_name = cast(types.FrameType, inspect.currentframe()).f_code.co_name
     _complete_doc = inspect.getdoc(eval(_fnc_name))  # pylint: disable=eval-used  # nosec B307
```

### Comparing `python_active_versions-1.9.0/python_active_versions/python_active_versions.py` & `python_active_versions-1.9.1/python_active_versions/python_active_versions.py`

 * *Files identical despite different names*

### Comparing `python_active_versions-1.9.0/python_active_versions/utility.py` & `python_active_versions-1.9.1/python_active_versions/utility.py`

 * *Files identical despite different names*

### Comparing `python_active_versions-1.9.0/tests/test_python_active_versions.py` & `python_active_versions-1.9.1/tests/test_python_active_versions.py`

 * *Files identical despite different names*

### Comparing `python_active_versions-1.9.0/tests/test_utils.py` & `python_active_versions-1.9.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `python_active_versions-1.9.0/PKG-INFO` & `python_active_versions-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-active-versions
-Version: 1.9.0
+Version: 1.9.1
 Summary: Gather active python versions.
 Home-page: https://github.com/gpongelli/python-active-versions
 License: MIT
 Author: Gabriele Pongelli
 Author-email: gabriele.pongelli@gmail.com
 Requires-Python: >=3.7.0,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

