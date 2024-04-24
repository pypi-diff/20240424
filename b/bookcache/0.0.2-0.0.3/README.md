# Comparing `tmp/bookcache-0.0.2.tar.gz` & `tmp/bookcache-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bookcache-0.0.2.tar", max compression
+gzip compressed data, was "bookcache-0.0.3.tar", max compression
```

## Comparing `bookcache-0.0.2.tar` & `bookcache-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0       26 2024-04-23 18:05:34.000000 bookcache-0.0.2/bookcache/__init__.py
--rw-r--r--   0        0        0     3791 2024-04-23 19:33:18.000000 bookcache-0.0.2/bookcache/cache.py
--rw-r--r--   0        0        0        0 2024-04-22 22:35:34.000000 bookcache-0.0.2/bookcache/py.typed
--rw-r--r--   0        0        0      692 2024-04-23 05:28:08.000000 bookcache-0.0.2/bookcache/types/CachedItem.py
--rw-r--r--   0        0        0      193 2024-04-23 01:38:46.000000 bookcache-0.0.2/bookcache/utils/runner.py
--rw-r--r--   0        0        0     1093 2024-04-22 23:04:48.000000 bookcache-0.0.2/LICENCE
--rw-r--r--   0        0        0      799 2024-04-23 20:31:22.000000 bookcache-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       94 2024-04-22 22:34:26.000000 bookcache-0.0.2/README.md
--rw-r--r--   0        0        0      966 1970-01-01 00:00:00.000000 bookcache-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1154 2024-04-23 20:44:56.000000 bookcache-0.0.3/bookcache/__init__.py
+-rw-r--r--   0        0        0     4197 2024-04-23 20:50:48.000000 bookcache-0.0.3/bookcache/cache.py
+-rw-r--r--   0        0        0        0 2024-04-23 20:48:23.680000 bookcache-0.0.3/bookcache/errors/KeyExists.py
+-rw-r--r--   0        0        0        0 2024-04-22 22:35:34.000000 bookcache-0.0.3/bookcache/py.typed
+-rw-r--r--   0        0        0      692 2024-04-23 05:28:08.000000 bookcache-0.0.3/bookcache/types/CachedItem.py
+-rw-r--r--   0        0        0      193 2024-04-23 01:38:46.000000 bookcache-0.0.3/bookcache/utils/runner.py
+-rw-r--r--   0        0        0     1093 2024-04-22 23:04:48.000000 bookcache-0.0.3/LICENCE
+-rw-r--r--   0        0        0      749 2024-04-23 20:54:10.000000 bookcache-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       94 2024-04-22 22:34:26.000000 bookcache-0.0.3/README.md
+-rw-r--r--   0        0        0      969 1970-01-01 00:00:00.000000 bookcache-0.0.3/PKG-INFO
```

### Comparing `bookcache-0.0.2/bookcache/cache.py` & `bookcache-0.0.3/bookcache/cache.py`

 * *Files 10% similar despite different names*

```diff
@@ -84,14 +84,29 @@
         """Initializes the librarian background functions and initializes other miscellaneous things."""
 
         # Initialize scanner function
         self._taskLibrarianScan = loop.create_task(
             periodically(self.librarianScan(), self._iterationTiming)
         )
 
+    async def Set(self, key: str, value: typing.Any, ttl: float = None):
+        """
+        Sets the entered key to a value
+
+        ----
+
+        Arguments:
+            `key` (`str`): The identifier for the key.
+            `value` (`any`): The value to store.
+            `ttl` (`float`, `none`): How many seconds till the key should expire.
+
+        Raises:
+            ...
+        """
+
     async def Get(self, key: str) -> typing.Any:
         """
         Fetches the entered key from the cache.
 
         ----
 
         Arguments:
```

### Comparing `bookcache-0.0.2/bookcache/types/CachedItem.py` & `bookcache-0.0.3/bookcache/types/CachedItem.py`

 * *Files identical despite different names*

### Comparing `bookcache-0.0.2/LICENCE` & `bookcache-0.0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `bookcache-0.0.2/pyproject.toml` & `bookcache-0.0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 [tool.poetry]
 name = "bookcache"
-version = "0.0.2"
+version = "0.0.3"
 description = "An in-memory keystore caching system."
 authors = ["NotAussie <NotAussie@duck.com>"]
 readme = "README.md"
 license = "MIT"
 keywords = ["caching", "cache", "keystore"]
 repository = "https://github.com/NotAussie/bookcache"
-homepage = "https://pypi.org/project/bookcache/"
 classifiers = [
     "Development Status :: 1 - Planning",
     "Framework :: AsyncIO",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.10",
     "Topic :: Database",
     "Intended Audience :: Developers",
```

### Comparing `bookcache-0.0.2/PKG-INFO` & `bookcache-0.0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: bookcache
-Version: 0.0.2
+Version: 0.0.3
 Summary: An in-memory keystore caching system.
-Home-page: https://pypi.org/project/bookcache/
+Home-page: https://github.com/NotAussie/bookcache
 License: MIT
 Keywords: caching,cache,keystore
 Author: NotAussie
 Author-email: NotAussie@duck.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 1 - Planning
 Classifier: Framework :: AsyncIO
```

