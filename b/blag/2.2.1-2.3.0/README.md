# Comparing `tmp/blag-2.2.1.tar.gz` & `tmp/blag-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blag-2.2.1.tar", last modified: Sat Nov 11 10:04:00 2023, max compression
+gzip compressed data, was "blag-2.3.0.tar", last modified: Wed Apr 24 20:30:40 2024, max compression
```

## Comparing `blag-2.2.1.tar` & `blag-2.3.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-11-11 10:04:00.280737 blag-2.2.1/
--rw-r--r--   0 venthur   (1000) venthur   (1000)     1072 2021-02-01 20:16:23.000000 blag-2.2.1/LICENSE
--rw-r--r--   0 venthur   (1000) venthur   (1000)      100 2023-08-27 13:24:52.000000 blag-2.2.1/MANIFEST.in
--rw-r--r--   0 venthur   (1000) venthur   (1000)     3742 2023-11-11 10:04:00.280737 blag-2.2.1/PKG-INFO
--rw-r--r--   0 venthur   (1000) venthur   (1000)     1456 2023-06-17 13:20:34.000000 blag-2.2.1/README.md
-drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-11-11 10:04:00.272737 blag-2.2.1/blag/
--rw-r--r--   0 venthur   (1000) venthur   (1000)       60 2022-09-01 16:56:08.000000 blag-2.2.1/blag/__init__.py
--rw-r--r--   0 venthur   (1000) venthur   (1000)    13805 2023-10-22 12:56:49.000000 blag-2.2.1/blag/blag.py
-drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-11-11 10:04:00.276737 blag-2.2.1/blag/content/
--rw-r--r--   0 venthur   (1000) venthur   (1000)      232 2023-06-16 20:05:45.000000 blag-2.2.1/blag/content/about.md
--rw-r--r--   0 venthur   (1000) venthur   (1000)     1524 2023-06-16 20:05:45.000000 blag-2.2.1/blag/content/hello-world.md
--rw-r--r--   0 venthur   (1000) venthur   (1000)      227 2023-06-17 13:22:02.000000 blag-2.2.1/blag/content/second-post.md
--rw-r--r--   0 venthur   (1000) venthur   (1000)     1061 2023-06-16 20:05:45.000000 blag-2.2.1/blag/content/testpage.md
--rw-r--r--   0 venthur   (1000) venthur   (1000)     2624 2023-06-16 20:05:45.000000 blag-2.2.1/blag/devserver.py
--rw-r--r--   0 venthur   (1000) venthur   (1000)     3728 2023-10-22 12:56:49.000000 blag-2.2.1/blag/markdown.py
--rw-r--r--   0 venthur   (1000) venthur   (1000)     2405 2023-10-22 12:56:49.000000 blag-2.2.1/blag/quickstart.py
-drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-11-11 10:04:00.276737 blag-2.2.1/blag/static/
--rw-r--r--   0 venthur   (1000) venthur   (1000)    96105 2023-06-17 10:00:55.000000 blag-2.2.1/blag/static/blag.png
--rw-r--r--   0 venthur   (1000) venthur   (1000)     4048 2023-06-16 20:05:45.000000 blag-2.2.1/blag/static/code-dark.css
--rw-r--r--   0 venthur   (1000) venthur   (1000)     4036 2023-06-16 20:05:45.000000 blag-2.2.1/blag/static/code-light.css
--rw-r--r--   0 venthur   (1000) venthur   (1000)    15406 2023-06-16 20:05:45.000000 blag-2.2.1/blag/static/favicon.ico
--rw-r--r--   0 venthur   (1000) venthur   (1000)     2604 2023-06-24 11:12:08.000000 blag-2.2.1/blag/static/style.css
-drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-11-11 10:04:00.276737 blag-2.2.1/blag/templates/
--rw-r--r--   0 venthur   (1000) venthur   (1000)      449 2023-06-16 20:05:45.000000 blag-2.2.1/blag/templates/archive.html
--rw-r--r--   0 venthur   (1000) venthur   (1000)      558 2023-06-16 20:05:45.000000 blag-2.2.1/blag/templates/article.html
--rw-r--r--   0 venthur   (1000) venthur   (1000)     1520 2023-06-16 20:05:45.000000 blag-2.2.1/blag/templates/base.html
--rw-r--r--   0 venthur   (1000) venthur   (1000)      515 2023-06-16 20:05:45.000000 blag-2.2.1/blag/templates/index.html
--rw-r--r--   0 venthur   (1000) venthur   (1000)      124 2023-06-16 20:05:45.000000 blag-2.2.1/blag/templates/page.html
--rw-r--r--   0 venthur   (1000) venthur   (1000)      493 2023-06-16 20:05:45.000000 blag-2.2.1/blag/templates/tag.html
--rw-r--r--   0 venthur   (1000) venthur   (1000)      245 2021-02-09 20:55:37.000000 blag-2.2.1/blag/templates/tags.html
--rw-r--r--   0 venthur   (1000) venthur   (1000)       71 2023-11-11 09:57:03.000000 blag-2.2.1/blag/version.py
-drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-11-11 10:04:00.272737 blag-2.2.1/blag.egg-info/
--rw-r--r--   0 venthur   (1000) venthur   (1000)     3742 2023-11-11 10:04:00.000000 blag-2.2.1/blag.egg-info/PKG-INFO
--rw-r--r--   0 venthur   (1000) venthur   (1000)      891 2023-11-11 10:04:00.000000 blag-2.2.1/blag.egg-info/SOURCES.txt
--rw-r--r--   0 venthur   (1000) venthur   (1000)        1 2023-11-11 10:04:00.000000 blag-2.2.1/blag.egg-info/dependency_links.txt
--rw-r--r--   0 venthur   (1000) venthur   (1000)       40 2023-11-11 10:04:00.000000 blag-2.2.1/blag.egg-info/entry_points.txt
--rw-r--r--   0 venthur   (1000) venthur   (1000)      151 2023-11-11 10:04:00.000000 blag-2.2.1/blag.egg-info/requires.txt
--rw-r--r--   0 venthur   (1000) venthur   (1000)       11 2023-11-11 10:04:00.000000 blag-2.2.1/blag.egg-info/top_level.txt
--rw-r--r--   0 venthur   (1000) venthur   (1000)     1672 2023-11-05 16:06:06.000000 blag-2.2.1/pyproject.toml
--rw-r--r--   0 venthur   (1000) venthur   (1000)       38 2023-11-11 10:04:00.280737 blag-2.2.1/setup.cfg
-drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-11-11 10:04:00.276737 blag-2.2.1/tests/
--rw-r--r--   0 venthur   (1000) venthur   (1000)       22 2023-10-22 12:56:49.000000 blag-2.2.1/tests/__init__.py
--rw-r--r--   0 venthur   (1000) venthur   (1000)     2631 2023-10-22 12:56:49.000000 blag-2.2.1/tests/conftest.py
--rw-r--r--   0 venthur   (1000) venthur   (1000)     9723 2023-10-22 12:56:49.000000 blag-2.2.1/tests/test_blag.py
--rw-r--r--   0 venthur   (1000) venthur   (1000)     1981 2023-10-22 12:56:49.000000 blag-2.2.1/tests/test_devserver.py
--rw-r--r--   0 venthur   (1000) venthur   (1000)     3279 2023-10-22 12:56:49.000000 blag-2.2.1/tests/test_markdown.py
--rw-r--r--   0 venthur   (1000) venthur   (1000)     1368 2023-10-22 12:56:49.000000 blag-2.2.1/tests/test_quickstart.py
--rw-r--r--   0 venthur   (1000) venthur   (1000)     2699 2023-10-22 12:56:49.000000 blag-2.2.1/tests/test_templates.py
--rw-r--r--   0 venthur   (1000) venthur   (1000)      243 2023-10-22 12:56:49.000000 blag-2.2.1/tests/test_version.py
+drwxrwxr-x   0 venthur   (1000) venthur   (1000)        0 2024-04-24 20:30:40.421349 blag-2.3.0/
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     1072 2021-02-01 20:16:23.000000 blag-2.3.0/LICENSE
+-rw-r--r--   0 venthur   (1000) venthur   (1000)      100 2023-11-12 16:17:54.000000 blag-2.3.0/MANIFEST.in
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     3744 2024-04-24 20:30:40.421349 blag-2.3.0/PKG-INFO
+-rw-rw-r--   0 venthur   (1000) venthur   (1000)     1457 2024-04-24 20:19:39.000000 blag-2.3.0/README.md
+drwxrwxr-x   0 venthur   (1000) venthur   (1000)        0 2024-04-24 20:30:40.413349 blag-2.3.0/blag/
+-rw-r--r--   0 venthur   (1000) venthur   (1000)       60 2023-11-12 16:17:54.000000 blag-2.3.0/blag/__init__.py
+-rw-rw-r--   0 venthur   (1000) venthur   (1000)    13725 2024-04-24 20:19:39.000000 blag-2.3.0/blag/blag.py
+drwxrwxr-x   0 venthur   (1000) venthur   (1000)        0 2024-04-24 20:30:40.413349 blag-2.3.0/blag/content/
+-rw-r--r--   0 venthur   (1000) venthur   (1000)      232 2023-11-12 16:17:54.000000 blag-2.3.0/blag/content/about.md
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     1524 2023-11-12 16:17:54.000000 blag-2.3.0/blag/content/hello-world.md
+-rw-r--r--   0 venthur   (1000) venthur   (1000)      227 2023-11-12 16:17:54.000000 blag-2.3.0/blag/content/second-post.md
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     1061 2023-11-12 16:17:54.000000 blag-2.3.0/blag/content/testpage.md
+-rw-rw-r--   0 venthur   (1000) venthur   (1000)     2959 2024-04-24 20:23:39.000000 blag-2.3.0/blag/devserver.py
+-rw-rw-r--   0 venthur   (1000) venthur   (1000)     3648 2024-04-24 20:19:39.000000 blag-2.3.0/blag/markdown.py
+-rw-rw-r--   0 venthur   (1000) venthur   (1000)     2325 2024-04-24 20:19:39.000000 blag-2.3.0/blag/quickstart.py
+drwxrwxr-x   0 venthur   (1000) venthur   (1000)        0 2024-04-24 20:30:40.413349 blag-2.3.0/blag/static/
+-rw-r--r--   0 venthur   (1000) venthur   (1000)    96105 2023-11-12 16:17:54.000000 blag-2.3.0/blag/static/blag.png
+-rw-rw-r--   0 venthur   (1000) venthur   (1000)     4136 2024-04-20 13:58:43.000000 blag-2.3.0/blag/static/code-dark.css
+-rw-rw-r--   0 venthur   (1000) venthur   (1000)     4108 2024-04-20 13:58:43.000000 blag-2.3.0/blag/static/code-light.css
+-rw-r--r--   0 venthur   (1000) venthur   (1000)    15406 2023-11-12 16:17:54.000000 blag-2.3.0/blag/static/favicon.ico
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     2604 2023-11-12 16:17:54.000000 blag-2.3.0/blag/static/style.css
+drwxrwxr-x   0 venthur   (1000) venthur   (1000)        0 2024-04-24 20:30:40.417349 blag-2.3.0/blag/templates/
+-rw-r--r--   0 venthur   (1000) venthur   (1000)      449 2023-11-12 16:17:54.000000 blag-2.3.0/blag/templates/archive.html
+-rw-r--r--   0 venthur   (1000) venthur   (1000)      558 2023-11-12 16:17:54.000000 blag-2.3.0/blag/templates/article.html
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     1520 2023-11-12 16:17:54.000000 blag-2.3.0/blag/templates/base.html
+-rw-r--r--   0 venthur   (1000) venthur   (1000)      515 2023-11-12 16:17:54.000000 blag-2.3.0/blag/templates/index.html
+-rw-r--r--   0 venthur   (1000) venthur   (1000)      124 2023-11-12 16:17:54.000000 blag-2.3.0/blag/templates/page.html
+-rw-r--r--   0 venthur   (1000) venthur   (1000)      493 2023-11-12 16:17:54.000000 blag-2.3.0/blag/templates/tag.html
+-rw-r--r--   0 venthur   (1000) venthur   (1000)      245 2021-02-09 20:55:37.000000 blag-2.3.0/blag/templates/tags.html
+-rw-r--r--   0 venthur   (1000) venthur   (1000)       71 2024-04-24 20:24:57.000000 blag-2.3.0/blag/version.py
+drwxrwxr-x   0 venthur   (1000) venthur   (1000)        0 2024-04-24 20:30:40.421349 blag-2.3.0/blag.egg-info/
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     3744 2024-04-24 20:30:40.000000 blag-2.3.0/blag.egg-info/PKG-INFO
+-rw-rw-r--   0 venthur   (1000) venthur   (1000)      891 2024-04-24 20:30:40.000000 blag-2.3.0/blag.egg-info/SOURCES.txt
+-rw-rw-r--   0 venthur   (1000) venthur   (1000)        1 2024-04-24 20:30:40.000000 blag-2.3.0/blag.egg-info/dependency_links.txt
+-rw-rw-r--   0 venthur   (1000) venthur   (1000)       40 2024-04-24 20:30:40.000000 blag-2.3.0/blag.egg-info/entry_points.txt
+-rw-rw-r--   0 venthur   (1000) venthur   (1000)      151 2024-04-24 20:30:40.000000 blag-2.3.0/blag.egg-info/requires.txt
+-rw-rw-r--   0 venthur   (1000) venthur   (1000)       11 2024-04-24 20:30:40.000000 blag-2.3.0/blag.egg-info/top_level.txt
+-rw-rw-r--   0 venthur   (1000) venthur   (1000)     1679 2024-04-24 20:19:39.000000 blag-2.3.0/pyproject.toml
+-rw-rw-r--   0 venthur   (1000) venthur   (1000)       38 2024-04-24 20:30:40.421349 blag-2.3.0/setup.cfg
+drwxrwxr-x   0 venthur   (1000) venthur   (1000)        0 2024-04-24 20:30:40.417349 blag-2.3.0/tests/
+-rw-r--r--   0 venthur   (1000) venthur   (1000)       22 2023-11-12 16:17:54.000000 blag-2.3.0/tests/__init__.py
+-rw-rw-r--   0 venthur   (1000) venthur   (1000)     2559 2024-04-24 20:19:39.000000 blag-2.3.0/tests/conftest.py
+-rw-rw-r--   0 venthur   (1000) venthur   (1000)     9642 2024-04-24 20:19:39.000000 blag-2.3.0/tests/test_blag.py
+-rw-rw-r--   0 venthur   (1000) venthur   (1000)     2497 2024-04-24 20:23:39.000000 blag-2.3.0/tests/test_devserver.py
+-rw-rw-r--   0 venthur   (1000) venthur   (1000)     3198 2024-04-24 20:19:39.000000 blag-2.3.0/tests/test_markdown.py
+-rw-rw-r--   0 venthur   (1000) venthur   (1000)     1287 2024-04-24 20:19:39.000000 blag-2.3.0/tests/test_quickstart.py
+-rw-rw-r--   0 venthur   (1000) venthur   (1000)     2618 2024-04-24 20:19:39.000000 blag-2.3.0/tests/test_templates.py
+-rw-rw-r--   0 venthur   (1000) venthur   (1000)      162 2024-04-24 20:19:39.000000 blag-2.3.0/tests/test_version.py
```

### Comparing `blag-2.2.1/LICENSE` & `blag-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `blag-2.2.1/PKG-INFO` & `blag-2.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blag
-Version: 2.2.1
+Version: 2.3.0
 Summary: blog-aware, static site generator
 Author-email: Bastian Venthur <mail@venthur.de>
 License: MIT License
         
         Copyright (c) 2018 Bastian Venthur
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -25,15 +25,15 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Documentation, https://blag.readthedocs.io/
 Project-URL: Source, https://github.com/venthur/blag
 Project-URL: Changelog, https://github.com/venthur/blag/blob/master/CHANGELOG.md
 Keywords: markdown,blag,blog,static site generator,cli
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: markdown
 Requires-Dist: feedgenerator
 Requires-Dist: jinja2
 Requires-Dist: pygments
 Provides-Extra: dev
@@ -71,15 +71,15 @@
   ![Blag Screenshot](blag/static/blag.png)
 * Theming support using [Jinja2][] templates
 * Generation of Atom feeds for blog content
 * Fenced code blocks and syntax highlighting using [Pygments][]
 * Integrated devserver
 * Available on [PyPI][]
 
-blag runs on Linux, Mac and Windows and requires Python >= 3.8
+blag runs on Linux, Mac and Windows and requires Python >= 3.10
 
 [markdown]: https://daringfireball.net/projects/markdown/
 [jinja2]: https://palletsprojects.com/p/jinja/
 [pygments]: https://pygments.org/
 [pypi]: https://pypi.org/project/blag/
```

### Comparing `blag-2.2.1/README.md` & `blag-2.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
   ![Blag Screenshot](blag/static/blag.png)
 * Theming support using [Jinja2][] templates
 * Generation of Atom feeds for blog content
 * Fenced code blocks and syntax highlighting using [Pygments][]
 * Integrated devserver
 * Available on [PyPI][]
 
-blag runs on Linux, Mac and Windows and requires Python >= 3.8
+blag runs on Linux, Mac and Windows and requires Python >= 3.10
 
 [markdown]: https://daringfireball.net/projects/markdown/
 [jinja2]: https://palletsprojects.com/p/jinja/
 [pygments]: https://pygments.org/
 [pypi]: https://pypi.org/project/blag/
```

### Comparing `blag-2.2.1/blag/blag.py` & `blag-2.3.0/blag/blag.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 #!/usr/bin/env python3
 
 """blag's core methods."""
 
-# remove when we don't support py38 anymore
-from __future__ import annotations
-
 import argparse
 import configparser
 import logging
 import os
 import shutil
 import sys
 from typing import Any
```

### Comparing `blag-2.2.1/blag/content/hello-world.md` & `blag-2.3.0/blag/content/hello-world.md`

 * *Files identical despite different names*

### Comparing `blag-2.2.1/blag/content/testpage.md` & `blag-2.3.0/blag/content/testpage.md`

 * *Files identical despite different names*

### Comparing `blag-2.2.1/blag/devserver.py` & `blag-2.3.0/blag/devserver.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,17 +2,14 @@
 
 This module provides functionality for blag's development server. It
 automatically detects changes in certain directories and rebuilds the
 site if necessary.
 
 """
 
-# remove when we don't support py38 anymore
-from __future__ import annotations
-
 import argparse
 import logging
 import multiprocessing
 import os
 import time
 from functools import partial
 from http.server import HTTPServer, SimpleHTTPRequestHandler
@@ -48,42 +45,51 @@
                 mtime = os.stat(os.path.join(root, f)).st_mtime
                 if mtime > last_mtime:
                     last_mtime = mtime
 
     return last_mtime
 
 
-def autoreload(args: argparse.Namespace) -> NoReturn:
+def autoreload(args: argparse.Namespace, wait: int=1) -> NoReturn:
     """Start the autoreloader.
 
     This method monitors the given directories for changes (i.e. the
     last modified time). If the last modified time has changed, a
     rebuild is triggered.
 
     A rebuild is also performed immediately when this method is called
     to avoid serving stale contents.
 
     Parameters
     ----------
     args
         contains the input-, template- and static dir
+    wait
+        number of seconds the devsever waits before checking for updated
+        content
 
     """
     dirs = [args.input_dir, args.template_dir, args.static_dir]
     logger.info(f"Monitoring {dirs} for changes...")
     # make sure we trigger the rebuild immediately when we enter the
     # loop to avoid serving stale contents
     last_mtime = 0.0
     while True:
-        mtime = get_last_modified(dirs)
-        if mtime > last_mtime:
-            last_mtime = mtime
-            logger.info("Change detected, rebuilding...")
-            blag.build(args)
-        time.sleep(1)
+        # make sure the devsever does not crash when the build fails with an
+        # exception
+        try:
+            mtime = get_last_modified(dirs)
+            if mtime > last_mtime:
+                last_mtime = mtime
+                logger.info("Change detected, rebuilding...")
+                blag.build(args)
+            time.sleep(wait)
+        except Exception:
+            logger.exception("Error occurred during rebuild:")
+            logger.info("Devserver did not crash, you may continue editing.")
 
 
 def serve(args: argparse.Namespace) -> None:
     """Start the webserver and the autoreloader.
 
     Parameters
     ----------
```

### Comparing `blag-2.2.1/blag/markdown.py` & `blag-2.3.0/blag/markdown.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 """Markdown Processing.
 
 This module contains the methods responsible for blag's markdown
 processing.
 
 """
 
-# remove when we don't support py38 anymore
-from __future__ import annotations
-
 import logging
 from datetime import datetime
 from urllib.parse import urlsplit, urlunsplit
 from xml.etree.ElementTree import Element
 
 from markdown import Markdown
 from markdown.extensions import Extension
```

### Comparing `blag-2.2.1/blag/quickstart.py` & `blag-2.3.0/blag/quickstart.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 """Helper methods for blag's quickstart command."""
 
-# remove when we don't support py38 anymore
-from __future__ import annotations
-
 import argparse
 import configparser
 import os
 import shutil
 
 import blag
```

### Comparing `blag-2.2.1/blag/static/blag.png` & `blag-2.3.0/blag/static/blag.png`

 * *Files identical despite different names*

### Comparing `blag-2.2.1/blag/static/code-dark.css` & `blag-2.3.0/blag/static/code-dark.css`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 pre { line-height: 125%; }
 td.linenos .normal { color: inherit; background-color: transparent; padding-left: 5px; padding-right: 5px; }
 span.linenos { color: inherit; background-color: transparent; padding-left: 5px; padding-right: 5px; }
 td.linenos .special { color: #000000; background-color: #ffffc0; padding-left: 5px; padding-right: 5px; }
 span.linenos.special { color: #000000; background-color: #ffffc0; padding-left: 5px; padding-right: 5px; }
 .hll { background-color: #49483e }
-.c { color: #75715e } /* Comment */
-.err { color: #960050; background-color: #1e0010 } /* Error */
+.c { color: #959077 } /* Comment */
+.err { color: #ed007e; background-color: #1e0010 } /* Error */
 .esc { color: #f8f8f2 } /* Escape */
 .g { color: #f8f8f2 } /* Generic */
 .k { color: #66d9ef } /* Keyword */
 .l { color: #ae81ff } /* Literal */
 .n { color: #f8f8f2 } /* Name */
-.o { color: #f92672 } /* Operator */
+.o { color: #ff4689 } /* Operator */
 .x { color: #f8f8f2 } /* Other */
 .p { color: #f8f8f2 } /* Punctuation */
-.ch { color: #75715e } /* Comment.Hashbang */
-.cm { color: #75715e } /* Comment.Multiline */
-.cp { color: #75715e } /* Comment.Preproc */
-.cpf { color: #75715e } /* Comment.PreprocFile */
-.c1 { color: #75715e } /* Comment.Single */
-.cs { color: #75715e } /* Comment.Special */
-.gd { color: #f92672 } /* Generic.Deleted */
+.ch { color: #959077 } /* Comment.Hashbang */
+.cm { color: #959077 } /* Comment.Multiline */
+.cp { color: #959077 } /* Comment.Preproc */
+.cpf { color: #959077 } /* Comment.PreprocFile */
+.c1 { color: #959077 } /* Comment.Single */
+.cs { color: #959077 } /* Comment.Special */
+.gd { color: #ff4689 } /* Generic.Deleted */
 .ge { color: #f8f8f2; font-style: italic } /* Generic.Emph */
+.ges { color: #f8f8f2; font-weight: bold; font-style: italic } /* Generic.EmphStrong */
 .gr { color: #f8f8f2 } /* Generic.Error */
 .gh { color: #f8f8f2 } /* Generic.Heading */
 .gi { color: #a6e22e } /* Generic.Inserted */
 .go { color: #66d9ef } /* Generic.Output */
-.gp { color: #f92672; font-weight: bold } /* Generic.Prompt */
+.gp { color: #ff4689; font-weight: bold } /* Generic.Prompt */
 .gs { color: #f8f8f2; font-weight: bold } /* Generic.Strong */
-.gu { color: #75715e } /* Generic.Subheading */
+.gu { color: #959077 } /* Generic.Subheading */
 .gt { color: #f8f8f2 } /* Generic.Traceback */
 .kc { color: #66d9ef } /* Keyword.Constant */
 .kd { color: #66d9ef } /* Keyword.Declaration */
-.kn { color: #f92672 } /* Keyword.Namespace */
+.kn { color: #ff4689 } /* Keyword.Namespace */
 .kp { color: #66d9ef } /* Keyword.Pseudo */
 .kr { color: #66d9ef } /* Keyword.Reserved */
 .kt { color: #66d9ef } /* Keyword.Type */
 .ld { color: #e6db74 } /* Literal.Date */
 .m { color: #ae81ff } /* Literal.Number */
 .s { color: #e6db74 } /* Literal.String */
 .na { color: #a6e22e } /* Name.Attribute */
@@ -47,17 +48,17 @@
 .ni { color: #f8f8f2 } /* Name.Entity */
 .ne { color: #a6e22e } /* Name.Exception */
 .nf { color: #a6e22e } /* Name.Function */
 .nl { color: #f8f8f2 } /* Name.Label */
 .nn { color: #f8f8f2 } /* Name.Namespace */
 .nx { color: #a6e22e } /* Name.Other */
 .py { color: #f8f8f2 } /* Name.Property */
-.nt { color: #f92672 } /* Name.Tag */
+.nt { color: #ff4689 } /* Name.Tag */
 .nv { color: #f8f8f2 } /* Name.Variable */
-.ow { color: #f92672 } /* Operator.Word */
+.ow { color: #ff4689 } /* Operator.Word */
 .pm { color: #f8f8f2 } /* Punctuation.Marker */
 .w { color: #f8f8f2 } /* Text.Whitespace */
 .mb { color: #ae81ff } /* Literal.Number.Bin */
 .mf { color: #ae81ff } /* Literal.Number.Float */
 .mh { color: #ae81ff } /* Literal.Number.Hex */
 .mi { color: #ae81ff } /* Literal.Number.Integer */
 .mo { color: #ae81ff } /* Literal.Number.Oct */
```

### Comparing `blag-2.2.1/blag/static/code-light.css` & `blag-2.3.0/blag/static/code-light.css`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 .cm { color: #3D7B7B; font-style: italic } /* Comment.Multiline */
 .cp { color: #9C6500 } /* Comment.Preproc */
 .cpf { color: #3D7B7B; font-style: italic } /* Comment.PreprocFile */
 .c1 { color: #3D7B7B; font-style: italic } /* Comment.Single */
 .cs { color: #3D7B7B; font-style: italic } /* Comment.Special */
 .gd { color: #A00000 } /* Generic.Deleted */
 .ge { font-style: italic } /* Generic.Emph */
+.ges { font-weight: bold; font-style: italic } /* Generic.EmphStrong */
 .gr { color: #E40000 } /* Generic.Error */
 .gh { color: #000080; font-weight: bold } /* Generic.Heading */
 .gi { color: #008400 } /* Generic.Inserted */
 .go { color: #717171 } /* Generic.Output */
 .gp { color: #000080; font-weight: bold } /* Generic.Prompt */
 .gs { font-weight: bold } /* Generic.Strong */
 .gu { color: #800080; font-weight: bold } /* Generic.Subheading */
```

### Comparing `blag-2.2.1/blag/static/favicon.ico` & `blag-2.3.0/blag/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `blag-2.2.1/blag/static/style.css` & `blag-2.3.0/blag/static/style.css`

 * *Files identical despite different names*

### Comparing `blag-2.2.1/blag/templates/article.html` & `blag-2.3.0/blag/templates/article.html`

 * *Files identical despite different names*

### Comparing `blag-2.2.1/blag/templates/base.html` & `blag-2.3.0/blag/templates/base.html`

 * *Files identical despite different names*

### Comparing `blag-2.2.1/blag/templates/index.html` & `blag-2.3.0/blag/templates/index.html`

 * *Files identical despite different names*

### Comparing `blag-2.2.1/blag.egg-info/PKG-INFO` & `blag-2.3.0/blag.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blag
-Version: 2.2.1
+Version: 2.3.0
 Summary: blog-aware, static site generator
 Author-email: Bastian Venthur <mail@venthur.de>
 License: MIT License
         
         Copyright (c) 2018 Bastian Venthur
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -25,15 +25,15 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Documentation, https://blag.readthedocs.io/
 Project-URL: Source, https://github.com/venthur/blag
 Project-URL: Changelog, https://github.com/venthur/blag/blob/master/CHANGELOG.md
 Keywords: markdown,blag,blog,static site generator,cli
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: markdown
 Requires-Dist: feedgenerator
 Requires-Dist: jinja2
 Requires-Dist: pygments
 Provides-Extra: dev
@@ -71,15 +71,15 @@
   ![Blag Screenshot](blag/static/blag.png)
 * Theming support using [Jinja2][] templates
 * Generation of Atom feeds for blog content
 * Fenced code blocks and syntax highlighting using [Pygments][]
 * Integrated devserver
 * Available on [PyPI][]
 
-blag runs on Linux, Mac and Windows and requires Python >= 3.8
+blag runs on Linux, Mac and Windows and requires Python >= 3.10
 
 [markdown]: https://daringfireball.net/projects/markdown/
 [jinja2]: https://palletsprojects.com/p/jinja/
 [pygments]: https://pygments.org/
 [pypi]: https://pypi.org/project/blag/
```

### Comparing `blag-2.2.1/blag.egg-info/SOURCES.txt` & `blag-2.3.0/blag.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blag-2.2.1/pyproject.toml` & `blag-2.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 authors = [
     { name="Bastian Venthur", email="mail@venthur.de" },
 ]
 description = "blog-aware, static site generator"
 keywords = ["markdown", "blag", "blog", "static site generator", "cli"]
 readme = "README.md"
 license = { file="LICENSE" }
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 dynamic = ["version"]
 dependencies = [
     "markdown",
     "feedgenerator",
     "jinja2",
     "pygments",
 ]
@@ -60,27 +60,27 @@
     --cov=blag
     --cov=tests
     --cov-report=html
     --cov-report=term-missing:skip-covered
 """
 
 [tool.ruff]
+line-length = 79
+target-version = "py310"
+
+[tool.ruff.lint]
 select = [
     "F",        # pyflakes
     "E", "W",   # pycodestyle
     "C90",      # mccabe
     "I",        # isort
     "D",        # pydocstyle
     "UP"        # pyupgrade
 ]
-line-length = 79
-target-version = "py38"
-
-[tool.ruff.pydocstyle]
-convention = "numpy"
+pydocstyle.convention = "numpy"
 
 [tool.mypy]
 files = "blag,tests"
 strict = true
 
 [[tool.mypy.overrides]]
 module = "feedgenerator.*"
```

### Comparing `blag-2.2.1/tests/conftest.py` & `blag-2.3.0/tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 """Pytest fixtures."""
 
-
-# remove when we don't support py38 anymore
-from __future__ import annotations
-
 import os
 from argparse import Namespace
+from collections.abc import Callable, Iterator
 from tempfile import TemporaryDirectory
-from typing import Callable, Iterator
 
 import pytest
 from jinja2 import Environment, Template
 
 from blag import blag, quickstart
```

### Comparing `blag-2.2.1/tests/test_blag.py` & `blag-2.3.0/tests/test_blag.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 """Test blag."""
 
-
-# remove when we don't support py38 anymore
-from __future__ import annotations
-
 import os
 from argparse import Namespace
 from datetime import datetime
 from tempfile import TemporaryDirectory
 from typing import Any
 
 import pytest
```

### Comparing `blag-2.2.1/tests/test_devserver.py` & `blag-2.3.0/tests/test_devserver.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,82 +1,99 @@
 """Tests for the devserver module."""
 
-
-# remove when we don't support py38 anymore
-from __future__ import annotations
-
 import threading
 import time
 from argparse import Namespace
 
-import pytest
-
 from blag import devserver
 
+WAITTIME = 0.1
+
 
 def test_get_last_modified(cleandir: str) -> None:
     """Test get_last_modified."""
     # take initial time
     t1 = devserver.get_last_modified(["content"])
 
     # wait a bit, create a file and measure again
-    time.sleep(0.1)
+    time.sleep(WAITTIME)
     with open("content/test", "w") as fh:
         fh.write("boo")
     t2 = devserver.get_last_modified(["content"])
 
     # wait a bit and take time again
-    time.sleep(0.1)
+    time.sleep(WAITTIME)
     t3 = devserver.get_last_modified(["content"])
 
     assert t2 > t1
     assert t2 == t3
 
 
 def test_autoreload_builds_immediately(args: Namespace) -> None:
     """Test autoreload builds immediately."""
     # create a dummy file that can be build
     with open("content/test.md", "w") as fh:
         fh.write("boo")
 
     t = threading.Thread(
         target=devserver.autoreload,
-        args=(args,),
+        args=(args, WAITTIME),
         daemon=True,
     )
     t0 = devserver.get_last_modified(["build"])
     t.start()
     # try for 5 seconds...
     for i in range(5):
-        time.sleep(1)
+        time.sleep(WAITTIME)
         t1 = devserver.get_last_modified(["build"])
         print(t1)
         if t1 > t0:
             break
     assert t1 > t0
 
 
-@pytest.mark.filterwarnings(
-    "ignore::pytest.PytestUnhandledThreadExceptionWarning"
-)
 def test_autoreload(args: Namespace) -> None:
     """Test autoreload."""
     t = threading.Thread(
         target=devserver.autoreload,
-        args=(args,),
+        args=(args, WAITTIME),
         daemon=True,
     )
     t.start()
 
     t0 = devserver.get_last_modified(["build"])
 
     # create a dummy file that can be build
     with open("content/test.md", "w") as fh:
         fh.write("boo")
 
     # try for 5 seconds to see if we rebuild once...
     for i in range(5):
-        time.sleep(1)
+        time.sleep(WAITTIME)
         t1 = devserver.get_last_modified(["build"])
         if t1 > t0:
             break
     assert t1 > t0
+
+
+def test_autoreload_does_not_crash(args: Namespace) -> None:
+    """Test autoreload does not crash if build fails."""
+    t = threading.Thread(
+        target=devserver.autoreload,
+        args=(args, WAITTIME),
+        daemon=True,
+    )
+    t.start()
+
+    t0 = devserver.get_last_modified(["build"])
+
+    # create a file that causes build to crash
+    with open("content/test.md", "w") as fh:
+        fh.write("date: ")
+
+    # try for 5 seconds to see if we rebuild once...
+    for i in range(5):
+        time.sleep(WAITTIME)
+        t1 = devserver.get_last_modified(["build"])
+        if t1 > t0:
+            break
+    assert t.is_alive()
```

### Comparing `blag-2.2.1/tests/test_markdown.py` & `blag-2.3.0/tests/test_markdown.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 """Test markdown module."""
 
-
-# remove when we don't support py38 anymore
-from __future__ import annotations
-
 from datetime import datetime
 from typing import Any
 
 import markdown
 import pytest
 
 from blag.markdown import convert_markdown, markdown_factory
```

### Comparing `blag-2.2.1/tests/test_quickstart.py` & `blag-2.3.0/tests/test_quickstart.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 """Tests for the quickstart module."""
 
-
-# remove when we don't support py38 anymore
-from __future__ import annotations
-
 import os
 
 from pytest import MonkeyPatch
 
 from blag.quickstart import get_input, quickstart
```

### Comparing `blag-2.2.1/tests/test_templates.py` & `blag-2.3.0/tests/test_templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 """Test the templates."""
 
-
-# remove when we don't support py38 anymore
-from __future__ import annotations
-
 import datetime
 
 from jinja2 import Template
 
 
 def test_page(page_template: Template) -> None:
     """Test the page template."""
```

