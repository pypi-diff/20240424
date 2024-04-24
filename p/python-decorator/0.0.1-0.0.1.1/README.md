# Comparing `tmp/python_decorator-0.0.1.tar.gz` & `tmp/python_decorator-0.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_decorator-0.0.1.tar", max compression
+gzip compressed data, was "python_decorator-0.0.1.1.tar", max compression
```

## Comparing `python_decorator-0.0.1.tar` & `python_decorator-0.0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_decorator-0.0.1/LICENSE
--rwxr-xr-x   0        0        0     8154 2024-04-24 15:23:57.369829 python_decorator-0.0.1/decorator/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_decorator-0.0.1/decorator/py.typed
--rw-r--r--   0        0        0     1203 2024-04-22 15:56:41.393372 python_decorator-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1356 2024-04-22 15:31:25.071582 python_decorator-0.0.1/readme.md
--rw-r--r--   0        0        0     2554 1970-01-01 00:00:00.000000 python_decorator-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_decorator-0.0.1.1/LICENSE
+-rwxr-xr-x   0        0        0     8154 2024-04-24 15:23:57.369829 python_decorator-0.0.1.1/decorator/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_decorator-0.0.1.1/decorator/py.typed
+-rw-r--r--   0        0        0     1205 2024-04-24 15:28:50.051647 python_decorator-0.0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      213 2024-04-24 15:28:37.375319 python_decorator-0.0.1.1/readme.md
+-rw-r--r--   0        0        0     1413 1970-01-01 00:00:00.000000 python_decorator-0.0.1.1/PKG-INFO
```

### Comparing `python_decorator-0.0.1/LICENSE` & `python_decorator-0.0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_decorator-0.0.1/decorator/__init__.py` & `python_decorator-0.0.1.1/decorator/__init__.py`

 * *Files identical despite different names*

### Comparing `python_decorator-0.0.1/pyproject.toml` & `python_decorator-0.0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-decorator"
-version = "0.0.1"
+version = "0.0.1.1"
 description = "Python argument type."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-decorator"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-decorator"
 keywords = ["file", "reverse", "iter"]
```

### Comparing `python_decorator-0.0.1/PKG-INFO` & `python_decorator-0.0.1.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-decorator
-Version: 0.0.1
+Version: 0.0.1.1
 Summary: Python argument type.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-decorator
 License: MIT
 Keywords: file,reverse,iter
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -26,55 +26,19 @@
 Project-URL: Repository, https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-decorator
 Description-Content-Type: text/markdown
 
 # Python decorator.
 
 ## Installation
 
-You can install from [pypi](https://pypi.org/project/python3-decorator/)
+You can install from [pypi](https://pypi.org/project/python-decorator/)
 
 ```console
 pip install -U python-decorator
 ```
 
 ## Usage
 
 ```python[tool.poetry]
-name = "python-decorator"
-version = "0.0.1"
-description = "Python decorator."
-authors = ["ChenyangGao <wosiwujm@gmail.com>"]
-license = "MIT"
-readme = "readme.md"
-homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-decorator"
-repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-decorator"
-keywords = ["file", "reverse", "iter"]
-classifiers = [
-    "License :: OSI Approved :: MIT License",
-    "Development Status :: 5 - Production/Stable",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3 :: Only",
-    "Operating System :: OS Independent",
-    "Intended Audience :: Developers",
-    "Topic :: Software Development",
-    "Topic :: Software Development :: Libraries",
-    "Topic :: Software Development :: Libraries :: Python Modules",
-]
-include = [
-    "LICENSE",
-]
-
-[tool.poetry.dependencies]
-python = "^3.10"
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
-
-[[tool.poetry.packages]]
-include = "decorator"
-
 import decorator
 ```
```

