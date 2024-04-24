# Comparing `tmp/python_partial-0.0.2.tar.gz` & `tmp/python_partial-0.0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_partial-0.0.2.tar", max compression
+gzip compressed data, was "python_partial-0.0.2.1.tar", max compression
```

## Comparing `python_partial-0.0.2.tar` & `python_partial-0.0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_partial-0.0.2/LICENSE
--rw-r--r--   0        0        0      185 2024-04-22 16:11:25.751372 python_partial-0.0.2/partial/__init__.py
--rw-r--r--   0        0        0     5091 2024-04-22 16:11:13.168870 python_partial-0.0.2/partial/partial.py
--rwxr-xr-x   0        0        0      849 2024-04-22 15:23:50.704838 python_partial-0.0.2/partial/placeholder.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_partial-0.0.2/partial/py.typed
--rw-r--r--   0        0        0     1174 2024-04-22 16:11:38.290473 python_partial-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      212 2024-04-22 15:32:04.972596 python_partial-0.0.2/readme.md
--rw-r--r--   0        0        0     1374 1970-01-01 00:00:00.000000 python_partial-0.0.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_partial-0.0.2.1/LICENSE
+-rw-r--r--   0        0        0      185 2024-04-22 16:11:25.751372 python_partial-0.0.2.1/partial/__init__.py
+-rw-r--r--   0        0        0     5113 2024-04-24 16:00:15.673641 python_partial-0.0.2.1/partial/partial.py
+-rwxr-xr-x   0        0        0      849 2024-04-22 15:23:50.704838 python_partial-0.0.2.1/partial/placeholder.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_partial-0.0.2.1/partial/py.typed
+-rw-r--r--   0        0        0     1176 2024-04-24 16:01:54.562788 python_partial-0.0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      212 2024-04-22 15:32:04.972596 python_partial-0.0.2.1/readme.md
+-rw-r--r--   0        0        0     1376 1970-01-01 00:00:00.000000 python_partial-0.0.2.1/PKG-INFO
```

### Comparing `python_partial-0.0.2/LICENSE` & `python_partial-0.0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_partial-0.0.2/partial/partial.py` & `python_partial-0.0.2.1/partial/partial.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 class ppartial(partial):
 
     def __new__(cls, func: Callable, /, *args, **kwargs):
         if isinstance(func, partial):
             args = func.args + args
             kwargs = {**func.keywords, **kwargs}
             func = func.func
-        return super().__new__(cls, func, *args, **kwargs)
+        return update_wrapper(super().__new__(cls, func, *args, **kwargs), func)
 
     def __call__(self, /, *args, **kwargs):
         args_, kwargs_ = self.args, self.keywords
 
         if _exist_placeholder(args_):
             args_it = iter(args)
             pargs = (*(next(args_it, _) if v is _ or v is undefined else v for v in args_), *args_it)
```

### Comparing `python_partial-0.0.2/partial/placeholder.py` & `python_partial-0.0.2.1/partial/placeholder.py`

 * *Files identical despite different names*

### Comparing `python_partial-0.0.2/pyproject.toml` & `python_partial-0.0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-partial"
-version = "0.0.2"
+version = "0.0.2.1"
 description = "Python partial types."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-partial"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-partial"
 keywords = ["file", "reverse", "iter"]
```

### Comparing `python_partial-0.0.2/PKG-INFO` & `python_partial-0.0.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-partial
-Version: 0.0.2
+Version: 0.0.2.1
 Summary: Python partial types.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-partial
 License: MIT
 Keywords: file,reverse,iter
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
```

