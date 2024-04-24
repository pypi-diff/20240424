# Comparing `tmp/property_lazy-0.0.6.tar.gz` & `tmp/property_lazy-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "property_lazy-0.0.6.tar", last modified: Tue Apr 23 04:03:01 2024, max compression
+gzip compressed data, was "property_lazy-0.0.7.tar", last modified: Wed Apr 24 07:49:15 2024, max compression
```

## Comparing `property_lazy-0.0.6.tar` & `property_lazy-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 04:03:01.570325 property_lazy-0.0.6/
--rw-rw-rw-   0        0        0     1073 2024-01-17 02:05:41.000000 property_lazy-0.0.6/LICENSE
--rw-rw-rw-   0        0        0       65 2024-01-17 02:05:41.000000 property_lazy-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0      268 2024-04-23 04:03:01.568710 property_lazy-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3715 2024-01-17 02:08:18.000000 property_lazy-0.0.6/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-23 04:03:01.565711 property_lazy-0.0.6/lazy_property/
--rw-rw-rw-   0        0        0     1939 2024-04-23 03:58:17.000000 property_lazy-0.0.6/lazy_property/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 04:03:01.568710 property_lazy-0.0.6/property_lazy.egg-info/
--rw-rw-rw-   0        0        0      268 2024-04-23 04:03:01.000000 property_lazy-0.0.6/property_lazy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2024-04-23 04:03:01.000000 property_lazy-0.0.6/property_lazy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 04:03:01.000000 property_lazy-0.0.6/property_lazy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-23 04:03:01.000000 property_lazy-0.0.6/property_lazy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 04:03:01.571221 property_lazy-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      389 2024-01-17 02:13:47.000000 property_lazy-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 07:49:15.657472 property_lazy-0.0.7/
+-rw-rw-rw-   0        0        0     1073 2024-01-17 02:05:41.000000 property_lazy-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0       65 2024-01-17 02:05:41.000000 property_lazy-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      268 2024-04-24 07:49:15.657472 property_lazy-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3715 2024-01-17 02:08:18.000000 property_lazy-0.0.7/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-24 07:49:15.653466 property_lazy-0.0.7/lazy_property/
+-rw-rw-rw-   0        0        0     1953 2024-04-24 07:49:05.000000 property_lazy-0.0.7/lazy_property/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 07:49:15.656468 property_lazy-0.0.7/property_lazy.egg-info/
+-rw-rw-rw-   0        0        0      268 2024-04-24 07:49:15.000000 property_lazy-0.0.7/property_lazy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2024-04-24 07:49:15.000000 property_lazy-0.0.7/property_lazy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 07:49:15.000000 property_lazy-0.0.7/property_lazy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-24 07:49:15.000000 property_lazy-0.0.7/property_lazy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 07:49:15.657472 property_lazy-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      389 2024-01-17 02:13:47.000000 property_lazy-0.0.7/setup.py
```

### Comparing `property_lazy-0.0.6/LICENSE` & `property_lazy-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `property_lazy-0.0.6/README.rst` & `property_lazy-0.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `property_lazy-0.0.6/lazy_property/__init__.py` & `property_lazy-0.0.7/lazy_property/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-__version__ = "0.0.6"
+__version__ = "0.0.7"
 from functools import update_wrapper
 
 
 class LazyProperty(property):
     def __init__(self, method, fget=None, fset=None, fdel=None, doc=None):
         self.method = method
-        self._cache_name = "_{}".format(self.method.__name__)
+        self._cache_name = "__cache_{}".format(self.method.__name__)
 
         doc = doc or method.__doc__
         super(LazyProperty, self).__init__(fget=fget, fset=fset, fdel=fdel, doc=doc)
 
         update_wrapper(self, method)
 
     def __get__(self, instance, owner):
@@ -64,8 +64,8 @@
     def getter(self, method):
         self.fget = method
         return self
 
 
 def lazy_property_reset(instance, *names):
     for name in names:
-        delattr(instance, f"_{name}")
+        delattr(instance, f"__cache_{name}")
```

