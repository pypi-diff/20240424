# Comparing `tmp/chess2vec-0.3.2b3.tar.gz` & `tmp/chess2vec-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess2vec-0.3.2b3.tar", max compression
+gzip compressed data, was "chess2vec-0.3.3.tar", max compression
```

## Comparing `chess2vec-0.3.2b3.tar` & `chess2vec-0.3.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2024-04-20 10:13:12.779868 chess2vec-0.3.2b3/README.md
--rw-r--r--   0        0        0     2103 2024-04-24 11:00:16.746784 chess2vec-0.3.2b3/chess2vec/__init__.py
--rw-r--r--   0        0        0      287 2024-04-23 21:18:28.472128 chess2vec-0.3.2b3/chess2vec/pgn.py
--rw-r--r--   0        0        0      202 2024-04-23 21:28:35.524582 chess2vec-0.3.2b3/chess2vec/utils/__init__.py
--rw-r--r--   0        0        0      583 2024-04-20 10:13:12.779868 chess2vec-0.3.2b3/chess2vec/utils/vector.py
--rw-r--r--   0        0        0     1371 2024-04-24 10:58:28.539897 chess2vec-0.3.2b3/chess2vec/vectorizers.py
--rw-r--r--   0        0        0      393 2024-04-24 11:00:44.546849 chess2vec-0.3.2b3/pyproject.toml
--rw-r--r--   0        0        0      640 1970-01-01 00:00:00.000000 chess2vec-0.3.2b3/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-20 10:13:12.779868 chess2vec-0.3.3/README.md
+-rw-r--r--   0        0        0     1869 2024-04-24 12:09:18.858049 chess2vec-0.3.3/chess2vec/__init__.py
+-rw-r--r--   0        0        0     2375 2024-04-24 12:16:02.100627 chess2vec-0.3.3/chess2vec/components.py
+-rw-r--r--   0        0        0      287 2024-04-23 21:18:28.472128 chess2vec-0.3.3/chess2vec/pgn.py
+-rw-r--r--   0        0        0      202 2024-04-23 21:28:35.524582 chess2vec-0.3.3/chess2vec/utils/__init__.py
+-rw-r--r--   0        0        0      583 2024-04-20 10:13:12.779868 chess2vec-0.3.3/chess2vec/utils/vector.py
+-rw-r--r--   0        0        0      391 2024-04-24 12:16:52.810911 chess2vec-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      638 1970-01-01 00:00:00.000000 chess2vec-0.3.3/PKG-INFO
```

### Comparing `chess2vec-0.3.2b3/chess2vec/__init__.py` & `chess2vec-0.3.3/chess2vec/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,26 @@
-import lzma
 import pickle
 from typing import Iterable, TextIO
 
 import chess
 import chess.pgn
 from tqdm import tqdm
 
-from chess2vec import vectorizers
+from chess2vec import components
 
 
-class PositionLoader:
-    def __init__(self, vectorizers: Iterable[vectorizers.BaseVectorizer]) -> None:
-        self.vectorizers = vectorizers
+class Loader:
+    def __init__(self, composition: components.Composition) -> None:
+        self.composition = composition
         self.data = []
-        self._game_id = 0
 
     @property
     def size(self) -> int:
         return len(self.data)
 
-    def add(self, board: chess.Board) -> None:
-        self.data.append([v(board) for v in self.vectorizers] + [self._game_id])
-        self._game_id += 1
-
     def load_pgn(
         self, pgn: TextIO, num_of_games: int = None, status: bool = False
     ) -> bool:
         if num_of_games is None:
             num_of_games = float("inf")
 
         if status:
@@ -36,38 +30,38 @@
 
         while n < num_of_games:
             game = chess.pgn.read_game(pgn)
 
             if not game:
                 return False
 
-            board = game.board()
-            self.add(board)
-
-            for move in game.mainline_moves():
-                board.push(move)
-                self.add(board)
+            self.data.append(self.composition(game))
 
             if status:
                 bar.update(1)
 
             n += 1
 
         if status:
             bar.close()
 
         return True
 
-    def get_position(self, idx):
+    def __getitem__(self, idx):
         return self.data[idx]
-
-    def get_vector(self, idx):
-        return list(zip(*self.data))[idx]
-
-    def batched(self, batch_size: int):
+    
+    @property
+    def meta(self):
+        return tuple(g['meta'] for g in self.data)
+    
+    @property
+    def comp(self):
+        return tuple(g['comp'] for g in self.data)
+    
+    def batched(self, batch_size):
         for idx in range(0, self.size, batch_size):
             yield self.data[idx : idx + batch_size]
 
     def save(self, file: str, *, batch_size=2**20) -> None:
         with open(file, "wb") as f:
             for batch in self.batched(batch_size):
                 pickle.dump(batch, f)
@@ -78,8 +72,8 @@
                 try:
                     self.data += pickle.load(f)
 
                 except EOFError:
                     return
 
     def __repr__(self) -> str:
-        return f"{self.__class__.__name__}(size={self.size}, vectorizers={self.vectorizers})"
+        return f"{self.__class__.__name__}(composition={self.composition}, size={self.size})"
```

### Comparing `chess2vec-0.3.2b3/chess2vec/utils/vector.py` & `chess2vec-0.3.3/chess2vec/utils/vector.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.3.2b3/PKG-INFO` & `chess2vec-0.3.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chess2vec
-Version: 0.3.2b3
+Version: 0.3.3
 Summary: 
 Author: Piotr Żarczyński
 Author-email: piotr.zarczynski.06@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

