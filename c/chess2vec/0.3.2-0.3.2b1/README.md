# Comparing `tmp/chess2vec-0.3.2.tar.gz` & `tmp/chess2vec-0.3.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess2vec-0.3.2.tar", max compression
+gzip compressed data, was "chess2vec-0.3.2b1.tar", max compression
```

## Comparing `chess2vec-0.3.2.tar` & `chess2vec-0.3.2b1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2024-04-20 10:13:12.779868 chess2vec-0.3.2/README.md
--rw-r--r--   0        0        0     1975 2024-04-24 09:04:36.466614 chess2vec-0.3.2/chess2vec/__init__.py
--rw-r--r--   0        0        0      287 2024-04-23 21:18:28.472128 chess2vec-0.3.2/chess2vec/pgn.py
--rw-r--r--   0        0        0      202 2024-04-23 21:28:35.524582 chess2vec-0.3.2/chess2vec/utils/__init__.py
--rw-r--r--   0        0        0      583 2024-04-20 10:13:12.779868 chess2vec-0.3.2/chess2vec/utils/vector.py
--rw-r--r--   0        0        0     1372 2024-04-23 21:29:05.336755 chess2vec-0.3.2/chess2vec/vectorizers.py
--rw-r--r--   0        0        0      391 2024-04-24 09:06:10.999970 chess2vec-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      638 1970-01-01 00:00:00.000000 chess2vec-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-20 10:13:12.779868 chess2vec-0.3.2b1/README.md
+-rw-r--r--   0        0        0     1980 2024-04-24 10:05:44.890177 chess2vec-0.3.2b1/chess2vec/__init__.py
+-rw-r--r--   0        0        0      287 2024-04-23 21:18:28.472128 chess2vec-0.3.2b1/chess2vec/pgn.py
+-rw-r--r--   0        0        0      202 2024-04-23 21:28:35.524582 chess2vec-0.3.2b1/chess2vec/utils/__init__.py
+-rw-r--r--   0        0        0      583 2024-04-20 10:13:12.779868 chess2vec-0.3.2b1/chess2vec/utils/vector.py
+-rw-r--r--   0        0        0     1372 2024-04-23 21:29:05.336755 chess2vec-0.3.2b1/chess2vec/vectorizers.py
+-rw-r--r--   0        0        0      393 2024-04-24 10:05:53.473610 chess2vec-0.3.2b1/pyproject.toml
+-rw-r--r--   0        0        0      640 1970-01-01 00:00:00.000000 chess2vec-0.3.2b1/PKG-INFO
```

### Comparing `chess2vec-0.3.2/chess2vec/__init__.py` & `chess2vec-0.3.2b1/chess2vec/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import Iterable, TextIO
 
 import chess
 import chess.pgn
 from tqdm import tqdm
 
-import mgzip
 import pickle
 
 from chess2vec import vectorizers as _vec
 
 
 class PositionLoader:
     def __init__(self, vectorizers: Iterable[_vec.BaseVectorizer]) -> None:
@@ -64,18 +63,18 @@
     def get_vector(self, idx):
         return list(zip(*self.data))[idx]
 
     def batched(self, batch_size: int):
         for idx in range(0, self.size, batch_size):
             yield self.data[idx : idx + batch_size]
 
-    def save(self, file: str) -> None:
-        with mgzip.open(file, 'ab') as f:
-            for batch in self.batched(2**20):
+    def save_raw(self, file: str, *, batch_size=2**20) -> None:
+        with open(file, 'ab') as f:
+            for batch in self.batched(batch_size):
                 pickle.dump(batch, f)
 
     def load(self, file: str) -> None:
-        with mgzip.open(file, 'rb') as f:
+        with open(file, 'rb') as f:
             self.data += pickle.load(f)
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(size={self.size}, vectorizers={self.vectorizers})"
```

### Comparing `chess2vec-0.3.2/chess2vec/utils/vector.py` & `chess2vec-0.3.2b1/chess2vec/utils/vector.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.3.2/chess2vec/vectorizers.py` & `chess2vec-0.3.2b1/chess2vec/vectorizers.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.3.2/PKG-INFO` & `chess2vec-0.3.2b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chess2vec
-Version: 0.3.2
+Version: 0.3.2b1
 Summary: 
 Author: Piotr Żarczyński
 Author-email: piotr.zarczynski.06@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

