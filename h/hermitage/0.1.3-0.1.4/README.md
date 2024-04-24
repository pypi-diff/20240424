# Comparing `tmp/hermitage-0.1.3.tar.gz` & `tmp/hermitage-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hermitage-0.1.3.tar", max compression
+gzip compressed data, was "hermitage-0.1.4.tar", max compression
```

## Comparing `hermitage-0.1.3.tar` & `hermitage-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       46 2024-04-15 11:34:36.787863 hermitage-0.1.3/README.md
--rw-r--r--   0        0        0      257 2024-04-13 13:50:37.630467 hermitage-0.1.3/hermitage/__init__.py
--rw-r--r--   0        0        0       24 2024-04-02 15:23:42.889513 hermitage-0.1.3/hermitage/definition/__init__.py
--rw-r--r--   0        0        0    11820 2024-04-13 13:19:43.140011 hermitage-0.1.3/hermitage/definition/contracts.py
--rw-r--r--   0        0        0       44 2024-04-02 15:23:42.889741 hermitage-0.1.3/hermitage/mappers/__init__.py
--rw-r--r--   0        0        0     1020 2024-04-13 13:50:37.613982 hermitage-0.1.3/hermitage/mappers/invoice.py
--rw-r--r--   0        0        0       31 2024-04-02 15:23:42.889934 hermitage-0.1.3/hermitage/parsers/__init__.py
--rw-r--r--   0        0        0     2836 2024-04-13 13:20:31.671188 hermitage-0.1.3/hermitage/parsers/query.py
--rw-r--r--   0        0        0      389 2024-04-15 11:34:27.345218 hermitage-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      606 1970-01-01 00:00:00.000000 hermitage-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       46 2024-04-15 11:34:36.787863 hermitage-0.1.4/README.md
+-rw-r--r--   0        0        0      257 2024-04-13 13:50:37.630467 hermitage-0.1.4/hermitage/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-02 15:23:42.889513 hermitage-0.1.4/hermitage/definition/__init__.py
+-rw-r--r--   0        0        0    11820 2024-04-13 13:19:43.140011 hermitage-0.1.4/hermitage/definition/contracts.py
+-rw-r--r--   0        0        0       44 2024-04-02 15:23:42.889741 hermitage-0.1.4/hermitage/mappers/__init__.py
+-rw-r--r--   0        0        0     1235 2024-04-24 07:28:43.056982 hermitage-0.1.4/hermitage/mappers/invoice.py
+-rw-r--r--   0        0        0       31 2024-04-02 15:23:42.889934 hermitage-0.1.4/hermitage/parsers/__init__.py
+-rw-r--r--   0        0        0     2836 2024-04-13 13:20:31.671188 hermitage-0.1.4/hermitage/parsers/query.py
+-rw-r--r--   0        0        0      361 2024-04-24 07:29:35.528391 hermitage-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      558 1970-01-01 00:00:00.000000 hermitage-0.1.4/PKG-INFO
```

### Comparing `hermitage-0.1.3/hermitage/definition/contracts.py` & `hermitage-0.1.4/hermitage/definition/contracts.py`

 * *Files identical despite different names*

### Comparing `hermitage-0.1.3/hermitage/mappers/invoice.py` & `hermitage-0.1.4/hermitage/mappers/invoice.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,28 @@
+import typing
+import enum
+
 import zodchy
-import zodchy_patterns
 from ..definition import contracts
 
+T = typing.TypeVar('T')
+
+
+class ReferenceContract(typing.Sized, typing.Protocol):
+    def __call__(self, value: enum.Enum) -> T: ...
+
+    def __getitem__(self, key: T) -> enum.Enum: ...
+
+    def get(self, key: T): ...
+
 
 class ClauseInjector:
     def __init__(
         self,
-        reference: zodchy_patterns.Reference,
+        reference: ReferenceContract,
         search_key: str,
         injection_key: str | None = None
     ):
         super().__init__()
         self._search_key = search_key
         self._injection_key = injection_key
         self._reference = reference
```

### Comparing `hermitage-0.1.3/hermitage/parsers/query.py` & `hermitage-0.1.4/hermitage/parsers/query.py`

 * *Files identical despite different names*

### Comparing `hermitage-0.1.3/PKG-INFO` & `hermitage-0.1.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: hermitage
-Version: 0.1.3
+Version: 0.1.4
 Summary: Universal storage access framework
 Home-page: https://github.com/smairon/hermitage
 Author: Smairon
 Author-email: man@smairon.ru
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: zodchy (>=0.1.0,<0.2.0)
-Requires-Dist: zodchy_patterns (>=0.1.0,<0.2.0)
 Project-URL: Repository, https://github.com/smairon/hermitage
 Description-Content-Type: text/markdown
 
 # Hermitage
 Universal storage access framework
```

