# Comparing `tmp/id-1.3.0.tar.gz` & `tmp/id-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "id-1.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "id-1.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `id-1.3.0.tar` & `id-1.4.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11358 2024-01-11 22:57:35.281802 id-1.3.0/LICENSE
--rw-r--r--   0        0        0     3604 2024-01-11 22:57:35.281802 id-1.3.0/README.md
--rw-r--r--   0        0        0     2464 2024-01-11 22:57:35.281802 id-1.3.0/id/__init__.py
--rw-r--r--   0        0        0     2513 2024-01-11 22:57:35.281802 id-1.3.0/id/__main__.py
--rw-r--r--   0        0        0      585 2024-01-11 22:57:35.281802 id-1.3.0/id/_internal/oidc/__init__.py
--rw-r--r--   0        0        0    12111 2024-01-11 22:57:35.285802 id-1.3.0/id/_internal/oidc/ambient.py
--rw-r--r--   0        0        0     2238 2024-01-11 22:57:35.285802 id-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     5140 1970-01-01 00:00:00.000000 id-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-04-24 17:31:03.370067 id-1.4.0/LICENSE
+-rw-r--r--   0        0        0     3604 2024-04-24 17:31:03.370067 id-1.4.0/README.md
+-rw-r--r--   0        0        0     2464 2024-04-24 17:31:03.370067 id-1.4.0/id/__init__.py
+-rw-r--r--   0        0        0     2514 2024-04-24 17:31:03.370067 id-1.4.0/id/__main__.py
+-rw-r--r--   0        0        0      585 2024-04-24 17:31:03.370067 id-1.4.0/id/_internal/oidc/__init__.py
+-rw-r--r--   0        0        0    12111 2024-04-24 17:31:03.370067 id-1.4.0/id/_internal/oidc/ambient.py
+-rw-r--r--   0        0        0     2314 2024-04-24 17:31:03.370067 id-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5139 1970-01-01 00:00:00.000000 id-1.4.0/PKG-INFO
```

### Comparing `id-1.3.0/LICENSE` & `id-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `id-1.3.0/README.md` & `id-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `id-1.3.0/id/__init__.py` & `id-1.4.0/id/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 """
 
 from __future__ import annotations
 
 import base64
 from typing import Callable
 
-__version__ = "1.3.0"
+__version__ = "1.4.0"
 
 
 class IdentityError(Exception):
     """
     Raised on any OIDC token format or claim error.
     """
```

### Comparing `id-1.3.0/id/__main__.py` & `id-1.4.0/id/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 The `python -m id` entrypoint.
 """
+
 import argparse
 import logging
 import os
 
 from . import __version__
 
 logging.basicConfig()
```

### Comparing `id-1.3.0/id/_internal/oidc/__init__.py` & `id-1.4.0/id/_internal/oidc/__init__.py`

 * *Files identical despite different names*

### Comparing `id-1.3.0/id/_internal/oidc/ambient.py` & `id-1.4.0/id/_internal/oidc/ambient.py`

 * *Files identical despite different names*

### Comparing `id-1.3.0/pyproject.toml` & `id-1.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -34,19 +34,22 @@
 test = ["pytest", "pytest-cov", "pretend", "coverage[toml]"]
 lint = [
   "bandit",
   "interrogate",
   "mypy",
   # NOTE(ww): ruff is under active development, so we pin conservatively here
   # and let Dependabot periodically perform this update.
-  "ruff < 0.1.12",
+  "ruff < 0.4.2",
   "types-requests",
 ]
 dev = ["build", "bump >= 1.3.2", "id[test,lint]"]
 
+[project.entry-points."pipx.run"]
+id = "id.__main__:main"
+
 [tool.interrogate]
 # don't enforce documentation coverage for packaging, testing, the virtual
 # environment, or the CLI (which is documented separately).
 ignore-semiprivate = true
 ignore-private = true
 # Ignore nested classes for docstring coverage because we use them primarily
 # for pydantic model configuration.
@@ -72,8 +75,10 @@
 plugins = ["pydantic.mypy"]
 
 [tool.bandit]
 exclude_dirs = ["./test"]
 
 [tool.ruff]
 line-length = 100
+
+[tool.ruff.lint]
 select = ["I", "E", "F", "W", "UP"]
```

### Comparing `id-1.3.0/PKG-INFO` & `id-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: id
-Version: 1.3.0
+Version: 1.4.0
 Summary: A tool for generating OIDC identities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -20,15 +20,15 @@
 Requires-Dist: requests
 Requires-Dist: build ; extra == "dev"
 Requires-Dist: bump >= 1.3.2 ; extra == "dev"
 Requires-Dist: id[test,lint] ; extra == "dev"
 Requires-Dist: bandit ; extra == "lint"
 Requires-Dist: interrogate ; extra == "lint"
 Requires-Dist: mypy ; extra == "lint"
-Requires-Dist: ruff < 0.1.12 ; extra == "lint"
+Requires-Dist: ruff < 0.4.2 ; extra == "lint"
 Requires-Dist: types-requests ; extra == "lint"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: pretend ; extra == "test"
 Requires-Dist: coverage[toml] ; extra == "test"
 Project-URL: Homepage, https://pypi.org/project/id/
 Project-URL: Issues, https://github.com/di/id/issues
```

