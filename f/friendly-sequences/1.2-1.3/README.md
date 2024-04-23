# Comparing `tmp/friendly_sequences-1.2.tar.gz` & `tmp/friendly_sequences-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "friendly_sequences-1.2.tar", last modified: Thu Apr 18 16:10:55 2024, max compression
+gzip compressed data, was "friendly_sequences-1.3.tar", last modified: Tue Apr 23 22:12:51 2024, max compression
```

## Comparing `friendly_sequences-1.2.tar` & `friendly_sequences-1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2024-04-18 16:10:36.620588 friendly_sequences-1.2/LICENSE
--rw-r--r--   0        0        0     1991 2024-04-18 16:10:36.620588 friendly_sequences-1.2/README.md
--rw-r--r--   0        0        0     2955 2024-04-18 16:10:36.620588 friendly_sequences-1.2/friendly_sequences/__init__.py
--rw-r--r--   0        0        0        0 2024-04-18 16:10:36.620588 friendly_sequences-1.2/friendly_sequences/py.typed
--rw-r--r--   0        0        0     2550 2024-04-18 16:10:55.060757 friendly_sequences-1.2/pyproject.toml
--rw-r--r--   0        0        0     1141 2024-04-18 16:10:36.624588 friendly_sequences-1.2/tests/test_friendly_sequences.py
--rw-r--r--   0        0        0     2342 1970-01-01 00:00:00.000000 friendly_sequences-1.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-23 22:12:27.621308 friendly_sequences-1.3/LICENSE
+-rw-r--r--   0        0        0     1991 2024-04-23 22:12:27.621308 friendly_sequences-1.3/README.md
+-rw-r--r--   0        0        0     3468 2024-04-23 22:12:27.621308 friendly_sequences-1.3/friendly_sequences/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 22:12:27.621308 friendly_sequences-1.3/friendly_sequences/py.typed
+-rw-r--r--   0        0        0     2550 2024-04-23 22:12:51.721343 friendly_sequences-1.3/pyproject.toml
+-rw-r--r--   0        0        0     1829 2024-04-23 22:12:27.625308 friendly_sequences-1.3/tests/test_friendly_sequences.py
+-rw-r--r--   0        0        0     2342 1970-01-01 00:00:00.000000 friendly_sequences-1.3/PKG-INFO
```

### Comparing `friendly_sequences-1.2/LICENSE` & `friendly_sequences-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `friendly_sequences-1.2/README.md` & `friendly_sequences-1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -87,9 +87,9 @@
     .fold(lambda left, right: f"{left}{right}", "")
 ) == "345"
 ```
 
 ## Installation
 
 ```bash
-$ pip install freindly-sequences
+$ pip install friendly-sequences
 ```
```

### Comparing `friendly_sequences-1.2/friendly_sequences/__init__.py` & `friendly_sequences-1.3/friendly_sequences/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,56 +1,59 @@
 import functools
 import itertools
 import typing as PT
 
+from collections import deque
 from collections.abc import Callable, Iterator
 
 import attrs
 
 
 __all__ = ("Seq",)
 
 IterableType1 = PT.TypeVar("IterableType1")
 IterableType2 = PT.TypeVar("IterableType2")
+IterableType3 = PT.TypeVar("IterableType3")
 ReturnIterableType1 = PT.TypeVar("ReturnIterableType1")
 ReturnIterableType2 = PT.TypeVar("ReturnIterableType2")
+ReturnIterableType3 = PT.TypeVar("ReturnIterableType3")
 
 
 @attrs.frozen(auto_attribs=True, slots=True)
-class Seq(Iterator, PT.Generic[IterableType1]):
+class Seq(Iterator[IterableType1], PT.Generic[IterableType1]):
     some: Iterator[IterableType1] = attrs.field(
         converter=lambda some: iter(some)
     )
 
     def map(
         self,
         func: Callable[
             [IterableType1],
             ReturnIterableType1,
         ],
     ) -> "Seq[ReturnIterableType1]":
         return Seq(map(func, self))
 
     def flat_map(
-        self,
+        self: "Seq[tuple[IterableType2, ...]]",
         func: Callable[
             [IterableType2],
             ReturnIterableType2,
         ],
     ) -> "Seq[ReturnIterableType2]":
         return Seq(
             map(
                 func,
                 itertools.chain.from_iterable(self),
             )
         )
 
     def flatten(
-        self,
-    ) -> "Seq[ReturnIterableType1]":
+        self: "Seq[tuple[IterableType2, ...]]",
+    ) -> "Seq[IterableType2]":
         return Seq(itertools.chain.from_iterable(self))
 
     def filter(
         self, func: Callable[[IterableType1], bool]
     ) -> "Seq[IterableType1]":
         return Seq(filter(func, self))
 
@@ -71,20 +74,20 @@
             initial,
         )
 
     def reduce(
         self,
         func: Callable[
             [
-                ReturnIterableType1,
+                IterableType1,
                 IterableType1,
             ],
-            ReturnIterableType1,
+            IterableType1,
         ],
-    ) -> ReturnIterableType1:
+    ) -> IterableType1:
         return functools.reduce(
             func,
             self,
         )
 
     def take(self, n: int = 1) -> "Seq[IterableType1]":
         return Seq(itertools.islice(self, n))
@@ -100,29 +103,40 @@
                 self,
                 key=key,
                 reverse=reverse,
             )
         )
 
     def zip(
-        self,
+        self: "Seq[IterableType1]",
         seq: "Seq[IterableType2]",
     ) -> "Seq[tuple[IterableType1, IterableType2]]":
-        return Seq(zip(self, seq, strict=False))
+        return Seq(zip(self, seq))  # noqa: B905
 
     def sum(self) -> IterableType1:
         return PT.cast(IterableType1, sum(self))
 
     def to_tuple(self) -> tuple[IterableType1, ...]:
         return tuple(self)
 
     def to_list(self) -> list[IterableType1]:
         return list(self)
 
+    def to_dict(
+        self: "Seq[tuple[IterableType2, IterableType3]]",
+    ) -> dict[IterableType2, IterableType3]:
+        return dict(self)
+
+    def exhaust(self) -> None:
+        deque(self, 0)
+
+    def consume(self) -> None:
+        return self.exhaust()  # pragma: nocover
+
     def head(self) -> IterableType1:
         return next(self.take())
 
-    def __iter__(self) -> "Seq[IterableType1]":
+    def __iter__(self) -> Iterator[IterableType1]:  # noqa: PYI034
         return self
 
     def __next__(self) -> IterableType1:
         return next(self.some)
```

### Comparing `friendly_sequences-1.2/pyproject.toml` & `friendly_sequences-1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -142,15 +142,15 @@
     { name = "zhukovgreen", email = "iam+friendly-sequences@zhukovgreen.pro" },
 ]
 dependencies = [
     "attrs>=21.3.0",
 ]
 requires-python = ">=3.10"
 readme = "README.md"
-version = "1.2"
+version = "1.3"
 
 [project.urls]
 repository = "https://github.com/zhukovgreen/friendly-sequences"
 
 [build-system]
 requires = [
     "pdm-backend",
```

### Comparing `friendly_sequences-1.2/PKG-INFO` & `friendly_sequences-1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: friendly-sequences
-Version: 1.2
+Version: 1.3
 Summary: Friendly sequences made in Python with :love:
 Author-Email: zhukovgreen <iam+friendly-sequences@zhukovgreen.pro>
 Project-URL: Repository, https://github.com/zhukovgreen/friendly-sequences
 Requires-Python: >=3.10
 Requires-Dist: attrs>=21.3.0
 Description-Content-Type: text/markdown
 
@@ -97,9 +97,9 @@
     .fold(lambda left, right: f"{left}{right}", "")
 ) == "345"
 ```
 
 ## Installation
 
 ```bash
-$ pip install freindly-sequences
+$ pip install friendly-sequences
 ```
```

