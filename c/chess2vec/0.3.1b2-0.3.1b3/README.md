# Comparing `tmp/chess2vec-0.3.1b2.tar.gz` & `tmp/chess2vec-0.3.1b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess2vec-0.3.1b2.tar", max compression
+gzip compressed data, was "chess2vec-0.3.1b3.tar", max compression
```

## Comparing `chess2vec-0.3.1b2.tar` & `chess2vec-0.3.1b3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2024-04-20 10:13:12.779868 chess2vec-0.3.1b2/README.md
--rw-r--r--   0        0        0     1836 2024-04-23 21:13:10.520791 chess2vec-0.3.1b2/chess2vec/__init__.py
--rw-r--r--   0        0        0      287 2024-04-23 21:18:28.472128 chess2vec-0.3.1b2/chess2vec/pgn.py
--rw-r--r--   0        0        0      202 2024-04-23 21:17:26.179422 chess2vec-0.3.1b2/chess2vec/utils/__init__.py
--rw-r--r--   0        0        0      583 2024-04-20 10:13:12.779868 chess2vec-0.3.1b2/chess2vec/utils/vector.py
--rw-r--r--   0        0        0     1308 2024-04-23 21:17:02.920716 chess2vec-0.3.1b2/chess2vec/vectorizers.py
--rw-r--r--   0        0        0      403 2024-04-23 21:18:46.133096 chess2vec-0.3.1b2/pyproject.toml
--rw-r--r--   0        0        0      650 1970-01-01 00:00:00.000000 chess2vec-0.3.1b2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-20 10:13:12.779868 chess2vec-0.3.1b3/README.md
+-rw-r--r--   0        0        0     1848 2024-04-23 21:27:25.136469 chess2vec-0.3.1b3/chess2vec/__init__.py
+-rw-r--r--   0        0        0      287 2024-04-23 21:18:28.472128 chess2vec-0.3.1b3/chess2vec/pgn.py
+-rw-r--r--   0        0        0      202 2024-04-23 21:28:35.524582 chess2vec-0.3.1b3/chess2vec/utils/__init__.py
+-rw-r--r--   0        0        0      583 2024-04-20 10:13:12.779868 chess2vec-0.3.1b3/chess2vec/utils/vector.py
+-rw-r--r--   0        0        0     1372 2024-04-23 21:29:05.336755 chess2vec-0.3.1b3/chess2vec/vectorizers.py
+-rw-r--r--   0        0        0      403 2024-04-23 21:29:13.392297 chess2vec-0.3.1b3/pyproject.toml
+-rw-r--r--   0        0        0      650 1970-01-01 00:00:00.000000 chess2vec-0.3.1b3/PKG-INFO
```

### Comparing `chess2vec-0.3.1b2/chess2vec/__init__.py` & `chess2vec-0.3.1b3/chess2vec/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             
             board = game.board()
             self.add(board)
 
             for move in game.mainline_moves():
                 board.push(move)
                 self.add(board)
-
+            
             if status:
                 bar.update(1)
                 
             n += 1
 
         if status:
             bar.close()
```

### Comparing `chess2vec-0.3.1b2/chess2vec/utils/vector.py` & `chess2vec-0.3.1b3/chess2vec/utils/vector.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.3.1b2/chess2vec/vectorizers.py` & `chess2vec-0.3.1b3/chess2vec/vectorizers.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,28 +16,30 @@
     def __call__(self, board: chess.Board): ...
 
     def __repr__(self) -> str:
         return f"{full_classname(self)}(size={self.size}, dtype={self.dtype})"
 
 
 class ActionVectorizer(BaseVectorizer):
-    @utils.convert_return(np.array, dtype=np.uint16)
+    @utils.convert_result(np.array, dtype=np.uint16)
+    @utils.convert_result(list)
     def __call__(self, board: chess.Board):
         for move in board.legal_moves:
             pt = board.piece_type_at(move.from_square)
 
             if not board.turn:
                 move.from_square ^= 0x38
                 move.to_square ^= 0x38
 
             yield 64 * (64 * (pt - 1) + move.from_square) + move.to_square
 
 
 class PieceVectorizer(BaseVectorizer):
-    @utils.convert_return(np.array, dtype=np.uint16)
+    @utils.convert_result(np.array, dtype=np.uint16)
+    @utils.convert_result(list)
     def __call__(self, board: chess.Board):
         for sq in chess.scan_reversed(board.occupied):
             piece = board.piece_at(sq)
 
             if not board.turn:
                 sq ^= 0x38
```

### Comparing `chess2vec-0.3.1b2/PKG-INFO` & `chess2vec-0.3.1b3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chess2vec
-Version: 0.3.1b2
+Version: 0.3.1b3
 Summary: 
 Author: Piotr Żarczyński
 Author-email: piotr.zarczynski.06@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

