# Comparing `tmp/nestipy_ioc-0.1.22.tar.gz` & `tmp/nestipy_ioc-0.1.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nestipy_ioc-0.1.22.tar", max compression
+gzip compressed data, was "nestipy_ioc-0.1.23.tar", max compression
```

## Comparing `nestipy_ioc-0.1.22.tar` & `nestipy_ioc-0.1.23.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2024-04-22 13:24:07.751008 nestipy_ioc-0.1.22/README.md
--rw-r--r--   0        0        0      374 2024-04-24 06:54:35.975510 nestipy_ioc-0.1.22/pyproject.toml
--rw-r--r--   0        0        0      774 2024-04-24 06:53:58.268550 nestipy_ioc-0.1.22/src/nestipy_ioc/__init__.py
--rw-r--r--   0        0        0      122 2024-04-22 14:21:10.410610 nestipy_ioc-0.1.22/src/nestipy_ioc/annotation.py
--rw-r--r--   0        0        0    12449 2024-04-23 11:57:44.650683 nestipy_ioc-0.1.22/src/nestipy_ioc/container.py
--rw-r--r--   0        0        0     1440 2024-04-22 13:59:48.684851 nestipy_ioc-0.1.22/src/nestipy_ioc/context_container.py
--rw-r--r--   0        0        0     1701 2024-04-23 15:29:10.758786 nestipy_ioc-0.1.22/src/nestipy_ioc/dependency.py
--rw-r--r--   0        0        0      885 2024-04-22 14:30:34.353131 nestipy_ioc-0.1.22/src/nestipy_ioc/meta.py
--rw-r--r--   0        0        0     2927 2024-04-24 06:53:20.077401 nestipy_ioc-0.1.22/src/nestipy_ioc/middleware.py
--rw-r--r--   0        0        0      877 2024-04-22 14:22:54.695299 nestipy_ioc-0.1.22/src/nestipy_ioc/provider.py
--rw-r--r--   0        0        0       56 2024-04-22 13:59:03.116828 nestipy_ioc-0.1.22/src/nestipy_ioc/utils.py
--rw-r--r--   0        0        0      484 1970-01-01 00:00:00.000000 nestipy_ioc-0.1.22/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-22 13:24:07.751008 nestipy_ioc-0.1.23/README.md
+-rw-r--r--   0        0        0      374 2024-04-24 07:03:20.462273 nestipy_ioc-0.1.23/pyproject.toml
+-rw-r--r--   0        0        0      774 2024-04-24 06:53:58.268550 nestipy_ioc-0.1.23/src/nestipy_ioc/__init__.py
+-rw-r--r--   0        0        0      122 2024-04-22 14:21:10.410610 nestipy_ioc-0.1.23/src/nestipy_ioc/annotation.py
+-rw-r--r--   0        0        0    12449 2024-04-23 11:57:44.650683 nestipy_ioc-0.1.23/src/nestipy_ioc/container.py
+-rw-r--r--   0        0        0     1440 2024-04-22 13:59:48.684851 nestipy_ioc-0.1.23/src/nestipy_ioc/context_container.py
+-rw-r--r--   0        0        0     1701 2024-04-23 15:29:10.758786 nestipy_ioc-0.1.23/src/nestipy_ioc/dependency.py
+-rw-r--r--   0        0        0      885 2024-04-22 14:30:34.353131 nestipy_ioc-0.1.23/src/nestipy_ioc/meta.py
+-rw-r--r--   0        0        0     2988 2024-04-24 07:03:11.906433 nestipy_ioc-0.1.23/src/nestipy_ioc/middleware.py
+-rw-r--r--   0        0        0      877 2024-04-22 14:22:54.695299 nestipy_ioc-0.1.23/src/nestipy_ioc/provider.py
+-rw-r--r--   0        0        0       56 2024-04-22 13:59:03.116828 nestipy_ioc-0.1.23/src/nestipy_ioc/utils.py
+-rw-r--r--   0        0        0      484 1970-01-01 00:00:00.000000 nestipy_ioc-0.1.23/PKG-INFO
```

### Comparing `nestipy_ioc-0.1.22/src/nestipy_ioc/__init__.py` & `nestipy_ioc-0.1.23/src/nestipy_ioc/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy_ioc-0.1.22/src/nestipy_ioc/container.py` & `nestipy_ioc-0.1.23/src/nestipy_ioc/container.py`

 * *Files identical despite different names*

### Comparing `nestipy_ioc-0.1.22/src/nestipy_ioc/context_container.py` & `nestipy_ioc-0.1.23/src/nestipy_ioc/context_container.py`

 * *Files identical despite different names*

### Comparing `nestipy_ioc-0.1.22/src/nestipy_ioc/dependency.py` & `nestipy_ioc-0.1.23/src/nestipy_ioc/dependency.py`

 * *Files identical despite different names*

### Comparing `nestipy_ioc-0.1.22/src/nestipy_ioc/meta.py` & `nestipy_ioc-0.1.23/src/nestipy_ioc/meta.py`

 * *Files identical despite different names*

### Comparing `nestipy_ioc-0.1.22/src/nestipy_ioc/middleware.py` & `nestipy_ioc-0.1.23/src/nestipy_ioc/middleware.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from dataclasses import dataclass, field
-from http import HTTPMethod
-from typing import Union, Type, Callable
+from typing import Union, Type, Callable, Literal
 
 from nestipy_metadata import Reflect, RouteKey, ClassMetadata
 
 from .container import NestipyContainer
 
 
 @dataclass
 class MiddlewareRouteConfig:
-    method: list[HTTPMethod] = field(default_factory=lambda: ['ALL'])
+    method: list[Literal['GET', 'POST', 'PUT', 'DELETE', 'PATCH', 'HEAD', 'OPTIONS', 'ALL', 'ANY']] = field(
+        default_factory=lambda: ['ALL'])
     url: str = field(default='/')
 
 
 class MiddlewareProxy:
 
     def __init__(self, *middleware: Union[Type, Callable]):
         self.middlewares = list(middleware)
```

### Comparing `nestipy_ioc-0.1.22/src/nestipy_ioc/provider.py` & `nestipy_ioc-0.1.23/src/nestipy_ioc/provider.py`

 * *Files identical despite different names*

