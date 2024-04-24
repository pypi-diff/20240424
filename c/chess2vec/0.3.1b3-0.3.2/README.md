# Comparing `tmp/chess2vec-0.3.1b3.tar.gz` & `tmp/chess2vec-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess2vec-0.3.1b3.tar", max compression
+gzip compressed data, was "chess2vec-0.3.2.tar", max compression
```

## Comparing `chess2vec-0.3.1b3.tar` & `chess2vec-0.3.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2024-04-20 10:13:12.779868 chess2vec-0.3.1b3/README.md
--rw-r--r--   0        0        0     1848 2024-04-23 21:27:25.136469 chess2vec-0.3.1b3/chess2vec/__init__.py
--rw-r--r--   0        0        0      287 2024-04-23 21:18:28.472128 chess2vec-0.3.1b3/chess2vec/pgn.py
--rw-r--r--   0        0        0      202 2024-04-23 21:28:35.524582 chess2vec-0.3.1b3/chess2vec/utils/__init__.py
--rw-r--r--   0        0        0      583 2024-04-20 10:13:12.779868 chess2vec-0.3.1b3/chess2vec/utils/vector.py
--rw-r--r--   0        0        0     1372 2024-04-23 21:29:05.336755 chess2vec-0.3.1b3/chess2vec/vectorizers.py
--rw-r--r--   0        0        0      403 2024-04-23 21:29:13.392297 chess2vec-0.3.1b3/pyproject.toml
--rw-r--r--   0        0        0      650 1970-01-01 00:00:00.000000 chess2vec-0.3.1b3/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-20 10:13:12.779868 chess2vec-0.3.2/README.md
+-rw-r--r--   0        0        0     1975 2024-04-24 09:04:36.466614 chess2vec-0.3.2/chess2vec/__init__.py
+-rw-r--r--   0        0        0      287 2024-04-23 21:18:28.472128 chess2vec-0.3.2/chess2vec/pgn.py
+-rw-r--r--   0        0        0      202 2024-04-23 21:28:35.524582 chess2vec-0.3.2/chess2vec/utils/__init__.py
+-rw-r--r--   0        0        0      583 2024-04-20 10:13:12.779868 chess2vec-0.3.2/chess2vec/utils/vector.py
+-rw-r--r--   0        0        0     1372 2024-04-23 21:29:05.336755 chess2vec-0.3.2/chess2vec/vectorizers.py
+-rw-r--r--   0        0        0      391 2024-04-24 09:06:10.999970 chess2vec-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      638 1970-01-01 00:00:00.000000 chess2vec-0.3.2/PKG-INFO
```

### Comparing `chess2vec-0.3.1b3/chess2vec/__init__.py` & `chess2vec-0.3.2/chess2vec/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import Iterable, TextIO
 
 import chess
 import chess.pgn
-import compress_pickle
 from tqdm import tqdm
 
+import mgzip
+import pickle
+
 from chess2vec import vectorizers as _vec
 
 
 class PositionLoader:
     def __init__(self, vectorizers: Iterable[_vec.BaseVectorizer]) -> None:
         self.vectorizers = vectorizers
         self.data = []
@@ -31,42 +33,49 @@
         if status:
             bar = tqdm(total=num_of_games)
 
         n = 0
 
         while n < num_of_games:
             game = chess.pgn.read_game(pgn)
-            
+
             if not game:
                 return False
-            
+
             board = game.board()
             self.add(board)
 
             for move in game.mainline_moves():
                 board.push(move)
                 self.add(board)
-            
+
             if status:
                 bar.update(1)
-                
+
             n += 1
 
         if status:
             bar.close()
-            
+
         return True
 
     def get_position(self, idx):
         return self.data[idx]
 
     def get_vector(self, idx):
         return list(zip(*self.data))[idx]
 
-    def save(self, file: str, compression: str = "gzip", mode="w") -> None:
-        compress_pickle.dump(self.data, file, compression=compression, mode=mode)
+    def batched(self, batch_size: int):
+        for idx in range(0, self.size, batch_size):
+            yield self.data[idx : idx + batch_size]
+
+    def save(self, file: str) -> None:
+        with mgzip.open(file, 'ab') as f:
+            for batch in self.batched(2**20):
+                pickle.dump(batch, f)
 
     def load(self, file: str) -> None:
-        self.data += compress_pickle.load(file)
+        with mgzip.open(file, 'rb') as f:
+            self.data += pickle.load(f)
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(size={self.size}, vectorizers={self.vectorizers})"
```

### Comparing `chess2vec-0.3.1b3/chess2vec/utils/vector.py` & `chess2vec-0.3.2/chess2vec/utils/vector.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.3.1b3/chess2vec/vectorizers.py` & `chess2vec-0.3.2/chess2vec/vectorizers.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.3.1b3/PKG-INFO` & `chess2vec-0.3.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: chess2vec
-Version: 0.3.1b3
+Version: 0.3.2
 Summary: 
 Author: Piotr Żarczyński
 Author-email: piotr.zarczynski.06@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: chess (>=1.10.0,<2.0.0)
-Requires-Dist: compress-pickle (>=2.1.0,<3.0.0)
+Requires-Dist: mgzip (>=0.2.1,<0.3.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: pytest (>=8.1.1,<9.0.0)
 Requires-Dist: scipy (>=1.13.0,<2.0.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Description-Content-Type: text/markdown
```

