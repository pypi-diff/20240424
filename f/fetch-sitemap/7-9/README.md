# Comparing `tmp/fetch-sitemap-7.tar.gz` & `tmp/fetch_sitemap-9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fetch-sitemap-7.tar", last modified: Wed Oct 25 16:38:02 2023, max compression
+gzip compressed data, was "fetch_sitemap-9.tar", max compression
```

## Comparing `fetch-sitemap-7.tar` & `fetch_sitemap-9.tar`

### file list

```diff
@@ -1,17 +1,6 @@
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-10-25 16:38:02.443740 fetch-sitemap-7/
--rw-r--r--   0 martin     (501) staff       (20)     1521 2023-02-06 18:00:57.000000 fetch-sitemap-7/LICENSE
--rw-r--r--   0 martin     (501) staff       (20)     2299 2023-10-25 16:38:02.443470 fetch-sitemap-7/PKG-INFO
--rw-r--r--   0 martin     (501) staff       (20)     1679 2023-04-04 12:43:16.000000 fetch-sitemap-7/README.md
--rw-r--r--   0 martin     (501) staff       (20)   540070 2023-02-06 18:41:57.000000 fetch-sitemap-7/example.png
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-10-25 16:38:02.442419 fetch-sitemap-7/fetch_sitemap/
--rw-r--r--   0 martin     (501) staff       (20)     2150 2023-10-25 15:29:29.000000 fetch-sitemap-7/fetch_sitemap/__init__.py
--rw-r--r--   0 martin     (501) staff       (20)     8226 2023-10-25 16:36:50.000000 fetch-sitemap-7/fetch_sitemap/fetch.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-10-25 16:38:02.443221 fetch-sitemap-7/fetch_sitemap.egg-info/
--rw-r--r--   0 martin     (501) staff       (20)     2299 2023-10-25 16:38:02.000000 fetch-sitemap-7/fetch_sitemap.egg-info/PKG-INFO
--rw-r--r--   0 martin     (501) staff       (20)      317 2023-10-25 16:38:02.000000 fetch-sitemap-7/fetch_sitemap.egg-info/SOURCES.txt
--rw-r--r--   0 martin     (501) staff       (20)        1 2023-10-25 16:38:02.000000 fetch-sitemap-7/fetch_sitemap.egg-info/dependency_links.txt
--rw-r--r--   0 martin     (501) staff       (20)       53 2023-10-25 16:38:02.000000 fetch-sitemap-7/fetch_sitemap.egg-info/entry_points.txt
--rw-r--r--   0 martin     (501) staff       (20)       41 2023-10-25 16:38:02.000000 fetch-sitemap-7/fetch_sitemap.egg-info/requires.txt
--rw-r--r--   0 martin     (501) staff       (20)       14 2023-10-25 16:38:02.000000 fetch-sitemap-7/fetch_sitemap.egg-info/top_level.txt
--rw-r--r--   0 martin     (501) staff       (20)     1362 2023-10-25 16:37:49.000000 fetch-sitemap-7/pyproject.toml
--rw-r--r--   0 martin     (501) staff       (20)       38 2023-10-25 16:38:02.443806 fetch-sitemap-7/setup.cfg
+-rw-r--r--   0        0        0     1521 2024-04-23 19:16:17.627088 fetch_sitemap-9/LICENSE
+-rw-r--r--   0        0        0     1739 2024-04-23 19:33:07.330392 fetch_sitemap-9/README.md
+-rw-r--r--   0        0        0     2194 2024-04-23 19:33:57.054226 fetch_sitemap-9/fetch_sitemap/__init__.py
+-rw-r--r--   0        0        0     8353 2024-04-23 19:33:40.787927 fetch_sitemap-9/fetch_sitemap/fetch.py
+-rw-r--r--   0        0        0     1473 2024-04-24 04:38:44.294695 fetch_sitemap-9/pyproject.toml
+-rw-r--r--   0        0        0     2398 1970-01-01 00:00:00.000000 fetch_sitemap-9/PKG-INFO
```

### Comparing `fetch-sitemap-7/LICENSE` & `fetch_sitemap-9/LICENSE`

 * *Files identical despite different names*

### Comparing `fetch-sitemap-7/PKG-INFO` & `fetch_sitemap-9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: fetch-sitemap
-Version: 7
+Version: 9
 Summary: Fetch a given sitemap and retrieve all URLs in it.
-Author-email: Martin Mahner <martin@elephant.house>
-Project-URL: Homepage, https://github.com/bartTC/fetch-sitemap
-Project-URL: Bug Tracker, https://github.com/bartTC/fetch-sitemap/issues
-Classifier: Programming Language :: Python :: 3
+License: MIT
+Author: Martin Mahner
+Author-email: martin@mahner.org
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: aiohttp (>=3.9.0)
+Requires-Dist: rich (>=12)
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: aiohttp==3.9.0b0
-Requires-Dist: importlib-metadata
-Requires-Dist: rich
 
 # fetch-sitemap
 
 Retrieves all URL's of a given sitemap.xml URL and fetches each page one by one. 
 Useful for (load) testing the entire site for error responses.
 
 ![Sample Output](https://raw.githubusercontent.com/bartTC/fetch-sitemap/main/example.png)
 
-*Note:* The default concurrency limit is 10, so 10 URLs are fetched at once. 
+*Note:* The default concurrency limit is 5, so 5 URLs are fetched at once. 
 Depending on your server's worker count, this might already be enough to DoS it.
 Try `--concurrency-limit=2` and increase if you feel comfortable.
 
 ```
 usage: fetch-sitemap 
     [-h] 
     [--basic-auth BASIC_AUTH] 
@@ -44,16 +46,17 @@
 options:
   -h, --help            show this help message and exit
   --basic-auth BASIC_AUTH
                         Basic auth information. Use: 'username:password'.
   -l LIMIT, --limit LIMIT
                         Maximum number of URLs to fetch from the given sitemap.xml. Default: All
   -c CONCURRENCY_LIMIT, --concurrency-limit CONCURRENCY_LIMIT
-                        Max number of concurrent requests. Default: 10
+                        Max number of concurrent requests. Default: 5
   -t REQUEST_TIMEOUT, --request-timeout REQUEST_TIMEOUT
                         Timeout for fetching a URL in seconds. Default: 30
   --random              Append a random string like ?12334232343 to each URL to bypass frontend cache. Default: False
   --report-path REPORT_PATH
                         Store results in a CSV file. Example: ./report.csv
   -o OUTPUT, --output-dir OUTPUT
                         Store all fetched sitemap documents in this folder.
+  -v, --version         show program's version number and exit
 ```
```

### Comparing `fetch-sitemap-7/README.md` & `fetch_sitemap-9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # fetch-sitemap
 
 Retrieves all URL's of a given sitemap.xml URL and fetches each page one by one. 
 Useful for (load) testing the entire site for error responses.
 
 ![Sample Output](https://raw.githubusercontent.com/bartTC/fetch-sitemap/main/example.png)
 
-*Note:* The default concurrency limit is 10, so 10 URLs are fetched at once. 
+*Note:* The default concurrency limit is 5, so 5 URLs are fetched at once. 
 Depending on your server's worker count, this might already be enough to DoS it.
 Try `--concurrency-limit=2` and increase if you feel comfortable.
 
 ```
 usage: fetch-sitemap 
     [-h] 
     [--basic-auth BASIC_AUTH] 
@@ -27,16 +27,17 @@
 options:
   -h, --help            show this help message and exit
   --basic-auth BASIC_AUTH
                         Basic auth information. Use: 'username:password'.
   -l LIMIT, --limit LIMIT
                         Maximum number of URLs to fetch from the given sitemap.xml. Default: All
   -c CONCURRENCY_LIMIT, --concurrency-limit CONCURRENCY_LIMIT
-                        Max number of concurrent requests. Default: 10
+                        Max number of concurrent requests. Default: 5
   -t REQUEST_TIMEOUT, --request-timeout REQUEST_TIMEOUT
                         Timeout for fetching a URL in seconds. Default: 30
   --random              Append a random string like ?12334232343 to each URL to bypass frontend cache. Default: False
   --report-path REPORT_PATH
                         Store results in a CSV file. Example: ./report.csv
   -o OUTPUT, --output-dir OUTPUT
                         Store all fetched sitemap documents in this folder.
+  -v, --version         show program's version number and exit
 ```
```

### Comparing `fetch-sitemap-7/fetch_sitemap/__init__.py` & `fetch_sitemap-9/fetch_sitemap/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 import argparse
 import asyncio
+from importlib import metadata
 from pathlib import Path
 
 from .fetch import PageFetcher
 
-try:
-    from importlib import metadata
-except ImportError:  # for Python<3.8
-    import importlib_metadata as metadata
-
 __version__ = metadata.version("fetch-sitemap")
 __author__ = "Martin Mahner"
 
 
 def main() -> None:
     parser = argparse.ArgumentParser(
         prog="fetch-sitemap",
@@ -34,16 +30,16 @@
         help="Maximum number of URLs to fetch from the given sitemap.xml. Default: All",
     )
     parser.add_argument(
         "-c",
         "--concurrency-limit",
         type=int,
         required=False,
-        default=10,
-        help="Max number of concurrent requests. Default: 10",
+        default=5,
+        help="Max number of concurrent requests. Default: 5",
     )
     parser.add_argument(
         "-t",
         "--request-timeout",
         type=int,
         required=False,
         default=30,
@@ -69,14 +65,20 @@
         "-o",
         "--output-dir",
         dest="output",
         type=Path,
         required=False,
         help="Store all fetched sitemap documents in this folder.",
     )
+    parser.add_argument(
+        "-v",
+        "--version",
+        action="version",
+        version=f"%(prog)s v{__version__}",
+    )
     args = parser.parse_args()
 
     try:
         f = PageFetcher(options=args)
         asyncio.run(f.run())
     except KeyboardInterrupt:
         pass
```

### Comparing `fetch-sitemap-7/fetch_sitemap/fetch.py` & `fetch_sitemap-9/fetch_sitemap/fetch.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,22 +8,23 @@
 import re
 import sys
 import time
 from decimal import Decimal
 from http import HTTPStatus
 from random import randint
 from textwrap import dedent
-from typing import TYPE_CHECKING, Any, Awaitable, Iterable
+from typing import TYPE_CHECKING, Any
 
 from aiohttp import BasicAuth, ClientResponse, ClientSession, ClientTimeout
 from rich.console import Console
 from rich.text import Text
 
 if TYPE_CHECKING:
     import argparse
+    from collections.abc import Awaitable, Iterable
 
 LOG_ITEMS = re.compile(r"<loc>(.*?)</loc>")
 
 # Defines what a 'slow' response time is
 SLOW_THRESHOLD = int(os.getenv("SLOW_THRESHOLD", "5"))
 
 # How many 'slow' responses to show
@@ -130,18 +131,22 @@
             )
 
         end = time.time()
         self.report.total_time = Decimal(end - start)
         self.show_statistics_report()
 
         if self.options.report_path:
-            with pathlib.Path(self.options.report_path).expanduser().open(
-                "w",
-                newline="",
-            ) as csvfile:
+            with (
+                pathlib.Path(self.options.report_path)
+                .expanduser()
+                .open(
+                    "w",
+                    newline="",
+                ) as csvfile
+            ):
                 w = csv.writer(
                     csvfile,
                     delimiter=",",
                     quotechar='"',
                     quoting=csv.QUOTE_MINIMAL,
                 )
                 w.writerow(["url", "status", "response time"])
@@ -207,15 +212,15 @@
             if response.url.path in ["/", ""]:
                 path = "index"
             else:
                 path = response.url.path.lstrip("/").rstrip("/")
 
             outfile = (self.options.output / f"{path}.html").expanduser().absolute()
             outfile.parent.mkdir(parents=True, exist_ok=True)
-            with pathlib.Path(outfile).open("w") as f:
+            with pathlib.Path(outfile).open("w") as f:  # noqa: ASYNC101
                 f.write(content)
 
         self.console.print(r.info())
         return r
 
     def show_statistics_report(self) -> None:
         text = Text(
```

### Comparing `fetch-sitemap-7/pyproject.toml` & `fetch_sitemap-9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,46 @@
-[project]
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
+
+[tool.poetry]
 name = "fetch-sitemap"
-version = "7"
-authors = [
-  { name="Martin Mahner", email="martin@elephant.house" },
-]
+version = "9"
 description = "Fetch a given sitemap and retrieve all URLs in it."
+authors = ["Martin Mahner <martin@mahner.org>"]
+license = "MIT"
 readme = "README.md"
-requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-dependencies = [
-    "aiohttp==3.9.0b0",
-    "importlib-metadata",
-    "rich",
-]
+
+[tool.poetry.dependencies]
+python = "^3.9"
+aiohttp = ">=3.9.0"
+rich = ">=12"
+
+[tool.poetry.scripts]
+fetch_sitemap = "fetch_sitemap:main"
 
 [project.scripts]
 "fetch-sitemap" = "fetch_sitemap:main"
 
 [project.urls]
 "Homepage" = "https://github.com/bartTC/fetch-sitemap"
 "Bug Tracker" = "https://github.com/bartTC/fetch-sitemap/issues"
 
 [tool.black]
 target-version = ['py312']
 include = '\.pyi?$'
 exclude = "migrations"
 
 [tool.ruff]
-target-version = "py38"
+target-version = "py39"
 exclude = ["migrations"]
 select = ["ALL"]
 ignore = [
   "ANN101",   # Missing Type Annotation for "self"
   "ANN401",   # Dynamically typed expressions (typing.Any) are disallowed in `**kwargs`"
   "D",        # Missing or badly formatted docstrings
   "FBT",      # Flake Boolean Trap (don't use arg=True in functions)
```

