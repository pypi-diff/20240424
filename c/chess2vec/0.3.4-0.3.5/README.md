# Comparing `tmp/chess2vec-0.3.4.tar.gz` & `tmp/chess2vec-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess2vec-0.3.4.tar", max compression
+gzip compressed data, was "chess2vec-0.3.5.tar", max compression
```

## Comparing `chess2vec-0.3.4.tar` & `chess2vec-0.3.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2024-04-20 10:13:12.779868 chess2vec-0.3.4/README.md
--rw-r--r--   0        0        0     1925 2024-04-24 16:16:47.781522 chess2vec-0.3.4/chess2vec/__init__.py
--rw-r--r--   0        0        0     2375 2024-04-24 13:38:13.616449 chess2vec-0.3.4/chess2vec/components.py
--rw-r--r--   0        0        0      287 2024-04-23 21:18:28.472128 chess2vec-0.3.4/chess2vec/pgn.py
--rw-r--r--   0        0        0      202 2024-04-23 21:28:35.524582 chess2vec-0.3.4/chess2vec/utils/__init__.py
--rw-r--r--   0        0        0      583 2024-04-20 10:13:12.779868 chess2vec-0.3.4/chess2vec/utils/vector.py
--rw-r--r--   0        0        0      374 2024-04-24 16:17:10.278798 chess2vec-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      600 1970-01-01 00:00:00.000000 chess2vec-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-20 10:13:12.779868 chess2vec-0.3.5/README.md
+-rw-r--r--   0        0        0     1659 2024-04-24 17:02:22.226590 chess2vec-0.3.5/chess2vec/__init__.py
+-rw-r--r--   0        0        0     2371 2024-04-24 16:53:32.576893 chess2vec-0.3.5/chess2vec/components.py
+-rw-r--r--   0        0        0      287 2024-04-23 21:18:28.472128 chess2vec-0.3.5/chess2vec/pgn.py
+-rw-r--r--   0        0        0      701 2024-04-24 17:02:17.210041 chess2vec-0.3.5/chess2vec/utils/__init__.py
+-rw-r--r--   0        0        0      583 2024-04-20 10:13:12.779868 chess2vec-0.3.5/chess2vec/utils/vector.py
+-rw-r--r--   0        0        0      374 2024-04-24 17:02:27.823127 chess2vec-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      600 1970-01-01 00:00:00.000000 chess2vec-0.3.5/PKG-INFO
```

### Comparing `chess2vec-0.3.4/chess2vec/__init__.py` & `chess2vec-0.3.5/chess2vec/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,37 @@
-import pickle
 from typing import TextIO
 
 import chess
 import chess.pgn
 from tqdm import tqdm
 
-from chess2vec import components
-import gzip
+from chess2vec import components, utils
 
 
 class Loader:
     def __init__(self, composition: components.Composition) -> None:
         self.composition = composition
         self.data = []
 
     @property
     def size(self) -> int:
         return len(self.data)
 
-    def load_pgn(
-        self, pgn: TextIO, n_games: int = None, status: bool = False
-    ) -> bool:
+    def __len__(self) -> int:
+        return self.size
+
+    def load_pgn(self, pgn: TextIO, n_games: int = None, status: bool = False) -> bool:
         if n_games is None:
             n_games = float("inf")
 
         if status:
             bar = tqdm(total=n_games)
 
         n = 0
-        
+
         while n < n_games:
             game = chess.pgn.read_game(pgn)
 
             if not game:
                 return False
 
             self.data.append(self.composition(game))
@@ -45,38 +44,28 @@
         if status:
             bar.close()
 
         return True
 
     def __getitem__(self, idx):
         return self.data[idx]
-    
+
     @property
     def meta(self):
-        return tuple(g['meta'] for g in self.data)
-    
+        return tuple(g["meta"] for g in self.data)
+
     @property
     def comp(self):
-        return tuple(g['comp'] for g in self.data)
-    
+        return tuple(g["comp"] for g in self.data)
+
     def batched(self, batch_size):
-        for idx in range(0, self.size, batch_size):
-            yield self.data[idx : idx + batch_size]
+        yield from utils.batched(self.data, batch_size)
 
     def save(self, file: str, new: bool = True, batch_size=2**16) -> None:
         mode = "wb" if new else "ab"
-        
-        with gzip.open(file, mode) as f:
-            for batch in self.batched(batch_size):
-                pickle.dump(batch, f)
-
-    def load(self, file: str) -> None:
-        with gzip.open(file, "rb") as f:
-            while True:
-                try:
-                    self.data += pickle.load(f)
+        utils.dump_gzip(self.data, file, mode, batch_size)
 
-                except EOFError:
-                    return
+    def load_gzip(self, file: str) -> None:
+        self.data += list(utils.load_gzip(file))
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(composition={self.composition}, size={self.size})"
```

### Comparing `chess2vec-0.3.4/chess2vec/components.py` & `chess2vec-0.3.5/chess2vec/components.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
             yield 64 * (64 * (pt - 1) + move.from_square) + move.to_square
 
 
 class Pieces(Component):
     def __init__(self, relative=True) -> None:
         self.relative = relative
-    
+
     @utils.convert_result(np.array, dtype=np.uint16)
     @utils.convert_result(list)
     def __call__(self, board):
         for sq in chess.scan_reversed(board.occupied):
             piece = board.piece_at(sq)
 
             if self.relative and not board.turn:
```

### Comparing `chess2vec-0.3.4/chess2vec/utils/vector.py` & `chess2vec-0.3.5/chess2vec/utils/vector.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.3.4/PKG-INFO` & `chess2vec-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chess2vec
-Version: 0.3.4
+Version: 0.3.5
 Summary: 
 Author: Piotr Żarczyński
 Author-email: piotr.zarczynski.06@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

