# Comparing `tmp/gyver_attrs-0.9.1.tar.gz` & `tmp/gyver_attrs-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gyver_attrs-0.9.1.tar", max compression
+gzip compressed data, was "gyver_attrs-0.9.2.tar", max compression
```

## Comparing `gyver_attrs-0.9.1.tar` & `gyver_attrs-0.9.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    11352 2024-03-28 22:15:25.253687 gyver_attrs-0.9.1/LICENSE
--rw-r--r--   0        0        0     5279 2024-03-28 22:15:25.253687 gyver_attrs-0.9.1/README.md
--rw-r--r--   0        0        0       80 2024-03-28 22:15:25.253687 gyver_attrs-0.9.1/gyver/__init__.py
--rw-r--r--   0        0        0      721 2024-04-16 17:08:08.551174 gyver_attrs-0.9.1/gyver/attrs/__init__.py
--rw-r--r--   0        0        0     3508 2024-04-16 17:07:30.546888 gyver_attrs-0.9.1/gyver/attrs/camel.py
--rw-r--r--   0        0        0      146 2024-03-28 22:15:25.253687 gyver_attrs-0.9.1/gyver/attrs/converters/__init__.py
--rw-r--r--   0        0        0      751 2024-03-28 22:15:25.253687 gyver_attrs-0.9.1/gyver/attrs/converters/json.py
--rw-r--r--   0        0        0     1463 2024-03-28 22:15:25.253687 gyver_attrs-0.9.1/gyver/attrs/converters/utils.py
--rw-r--r--   0        0        0     9316 2024-03-28 22:15:25.253687 gyver_attrs-0.9.1/gyver/attrs/field.py
--rw-r--r--   0        0        0     6142 2024-03-28 22:15:25.253687 gyver_attrs-0.9.1/gyver/attrs/helpers.py
--rw-r--r--   0        0        0    29147 2024-03-28 22:15:25.253687 gyver_attrs-0.9.1/gyver/attrs/main.py
--rw-r--r--   0        0        0     5072 2024-03-28 22:15:25.253687 gyver_attrs-0.9.1/gyver/attrs/methods.py
--rw-r--r--   0        0        0        0 2024-03-28 22:15:25.253687 gyver_attrs-0.9.1/gyver/attrs/py.typed
--rw-r--r--   0        0        0     4348 2024-03-28 22:15:25.253687 gyver_attrs-0.9.1/gyver/attrs/resolver.py
--rw-r--r--   0        0        0     4032 2024-03-28 22:15:25.253687 gyver_attrs-0.9.1/gyver/attrs/schema.py
--rw-r--r--   0        0        0     5653 2024-03-28 22:15:25.253687 gyver_attrs-0.9.1/gyver/attrs/shortcuts.py
--rw-r--r--   0        0        0        0 2024-03-28 22:15:25.253687 gyver_attrs-0.9.1/gyver/attrs/utils/__init__.py
--rw-r--r--   0        0        0      627 2024-03-28 22:15:25.253687 gyver_attrs-0.9.1/gyver/attrs/utils/factory.py
--rw-r--r--   0        0        0     5797 2024-04-16 17:06:15.778349 gyver_attrs-0.9.1/gyver/attrs/utils/functions.py
--rw-r--r--   0        0        0      641 2024-03-28 22:15:25.253687 gyver_attrs-0.9.1/gyver/attrs/utils/typedef.py
--rw-r--r--   0        0        0     1149 2024-04-16 17:08:08.561174 gyver_attrs-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     5920 1970-01-01 00:00:00.000000 gyver_attrs-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0    11352 2024-03-28 22:15:25.253687 gyver_attrs-0.9.2/LICENSE
+-rw-r--r--   0        0        0     5279 2024-03-28 22:15:25.253687 gyver_attrs-0.9.2/README.md
+-rw-r--r--   0        0        0       80 2024-03-28 22:15:25.253687 gyver_attrs-0.9.2/gyver/__init__.py
+-rw-r--r--   0        0        0      721 2024-04-24 16:51:22.740497 gyver_attrs-0.9.2/gyver/attrs/__init__.py
+-rw-r--r--   0        0        0     3508 2024-04-16 17:07:30.546888 gyver_attrs-0.9.2/gyver/attrs/camel.py
+-rw-r--r--   0        0        0      146 2024-03-28 22:15:25.253687 gyver_attrs-0.9.2/gyver/attrs/converters/__init__.py
+-rw-r--r--   0        0        0      751 2024-03-28 22:15:25.253687 gyver_attrs-0.9.2/gyver/attrs/converters/json.py
+-rw-r--r--   0        0        0     1463 2024-03-28 22:15:25.253687 gyver_attrs-0.9.2/gyver/attrs/converters/utils.py
+-rw-r--r--   0        0        0     9316 2024-04-17 01:24:16.620998 gyver_attrs-0.9.2/gyver/attrs/field.py
+-rw-r--r--   0        0        0     6142 2024-04-17 01:24:16.620998 gyver_attrs-0.9.2/gyver/attrs/helpers.py
+-rw-r--r--   0        0        0    29147 2024-04-17 01:24:16.620998 gyver_attrs-0.9.2/gyver/attrs/main.py
+-rw-r--r--   0        0        0     5072 2024-04-17 01:24:16.620998 gyver_attrs-0.9.2/gyver/attrs/methods.py
+-rw-r--r--   0        0        0        0 2024-03-28 22:15:25.253687 gyver_attrs-0.9.2/gyver/attrs/py.typed
+-rw-r--r--   0        0        0     4348 2024-03-28 22:15:25.253687 gyver_attrs-0.9.2/gyver/attrs/resolver.py
+-rw-r--r--   0        0        0     4032 2024-04-17 01:24:16.620998 gyver_attrs-0.9.2/gyver/attrs/schema.py
+-rw-r--r--   0        0        0     5653 2024-03-28 22:15:25.253687 gyver_attrs-0.9.2/gyver/attrs/shortcuts.py
+-rw-r--r--   0        0        0        0 2024-03-28 22:15:25.253687 gyver_attrs-0.9.2/gyver/attrs/utils/__init__.py
+-rw-r--r--   0        0        0      847 2024-04-24 16:43:28.681989 gyver_attrs-0.9.2/gyver/attrs/utils/factory.py
+-rw-r--r--   0        0        0     5797 2024-04-16 17:06:15.778349 gyver_attrs-0.9.2/gyver/attrs/utils/functions.py
+-rw-r--r--   0        0        0      641 2024-03-28 22:15:25.253687 gyver_attrs-0.9.2/gyver/attrs/utils/typedef.py
+-rw-r--r--   0        0        0     1149 2024-04-24 16:51:22.747164 gyver_attrs-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     5920 1970-01-01 00:00:00.000000 gyver_attrs-0.9.2/PKG-INFO
```

### Comparing `gyver_attrs-0.9.1/LICENSE` & `gyver_attrs-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.9.1/README.md` & `gyver_attrs-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.9.1/gyver/attrs/__init__.py` & `gyver_attrs-0.9.2/gyver/attrs/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,9 +23,9 @@
     'mutable',
     'kw_only',
     'UNINITIALIZED',
     'update_ref',
     'update_refs',
 ]
 
-__version__ = '0.9.1'
+__version__ = '0.9.2'
 __version_info__ = tuple(map(int, __version__.split('.')))
```

### Comparing `gyver_attrs-0.9.1/gyver/attrs/camel.py` & `gyver_attrs-0.9.2/gyver/attrs/camel.py`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.9.1/gyver/attrs/converters/json.py` & `gyver_attrs-0.9.2/gyver/attrs/converters/json.py`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.9.1/gyver/attrs/converters/utils.py` & `gyver_attrs-0.9.2/gyver/attrs/converters/utils.py`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.9.1/gyver/attrs/field.py` & `gyver_attrs-0.9.2/gyver/attrs/field.py`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.9.1/gyver/attrs/helpers.py` & `gyver_attrs-0.9.2/gyver/attrs/helpers.py`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.9.1/gyver/attrs/main.py` & `gyver_attrs-0.9.2/gyver/attrs/main.py`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.9.1/gyver/attrs/methods.py` & `gyver_attrs-0.9.2/gyver/attrs/methods.py`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.9.1/gyver/attrs/resolver.py` & `gyver_attrs-0.9.2/gyver/attrs/resolver.py`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.9.1/gyver/attrs/schema.py` & `gyver_attrs-0.9.2/gyver/attrs/schema.py`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.9.1/gyver/attrs/shortcuts.py` & `gyver_attrs-0.9.2/gyver/attrs/shortcuts.py`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.9.1/gyver/attrs/utils/factory.py` & `gyver_attrs-0.9.2/gyver/attrs/utils/factory.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 import typing
 from collections.abc import Callable
 
-from typing_extensions import ParamSpec
+from typing_extensions import ParamSpec, Self
 
 P = ParamSpec('P')
 T = typing.TypeVar('T')
 
 
 class Factory(typing.Generic[P, T]):
     __slots__ = ('func',)
+    func: Callable[P, T]
 
-    def __init__(self, func: Callable[P, T]) -> None:
-        self.func = func
+    def __new__(cls, func: Callable[P, T]) -> Self:
+        # Using __new__ to avoid having nested Factory instances
+        if isinstance(func, cls):
+            return func
+
+        instance = object.__new__(cls)
+        instance.func = func
+        return instance
 
     def __call__(self, *args: P.args, **kwds: P.kwargs) -> T:
         return self.func(*args, **kwds)
 
     @property
     def __name__(self):
         return self.func.__name__
```

### Comparing `gyver_attrs-0.9.1/gyver/attrs/utils/functions.py` & `gyver_attrs-0.9.2/gyver/attrs/utils/functions.py`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.9.1/gyver/attrs/utils/typedef.py` & `gyver_attrs-0.9.2/gyver/attrs/utils/typedef.py`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.9.1/pyproject.toml` & `gyver_attrs-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gyver-attrs"
-version = "0.9.1"
+version = "0.9.2"
 description = ""
 authors = ["Gustavo Cardoso <self.gustavocorrea@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "gyver" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gyver_attrs-0.9.1/PKG-INFO` & `gyver_attrs-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gyver-attrs
-Version: 0.9.1
+Version: 0.9.2
 Summary: 
 Author: Gustavo Cardoso
 Author-email: self.gustavocorrea@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

