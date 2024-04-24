# Comparing `tmp/chess2vec-0.3.3.tar.gz` & `tmp/chess2vec-0.3.3b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess2vec-0.3.3.tar", max compression
+gzip compressed data, was "chess2vec-0.3.3b1.tar", max compression
```

## Comparing `chess2vec-0.3.3.tar` & `chess2vec-0.3.3b1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2024-04-20 10:13:12.779868 chess2vec-0.3.3/README.md
--rw-r--r--   0        0        0     1869 2024-04-24 12:09:18.858049 chess2vec-0.3.3/chess2vec/__init__.py
--rw-r--r--   0        0        0     2375 2024-04-24 12:16:02.100627 chess2vec-0.3.3/chess2vec/components.py
--rw-r--r--   0        0        0      287 2024-04-23 21:18:28.472128 chess2vec-0.3.3/chess2vec/pgn.py
--rw-r--r--   0        0        0      202 2024-04-23 21:28:35.524582 chess2vec-0.3.3/chess2vec/utils/__init__.py
--rw-r--r--   0        0        0      583 2024-04-20 10:13:12.779868 chess2vec-0.3.3/chess2vec/utils/vector.py
--rw-r--r--   0        0        0      391 2024-04-24 12:16:52.810911 chess2vec-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      638 1970-01-01 00:00:00.000000 chess2vec-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-20 10:13:12.779868 chess2vec-0.3.3b1/README.md
+-rw-r--r--   0        0        0     1889 2024-04-24 13:41:37.874178 chess2vec-0.3.3b1/chess2vec/__init__.py
+-rw-r--r--   0        0        0     2375 2024-04-24 13:38:13.616449 chess2vec-0.3.3b1/chess2vec/components.py
+-rw-r--r--   0        0        0      287 2024-04-23 21:18:28.472128 chess2vec-0.3.3b1/chess2vec/pgn.py
+-rw-r--r--   0        0        0      202 2024-04-23 21:28:35.524582 chess2vec-0.3.3b1/chess2vec/utils/__init__.py
+-rw-r--r--   0        0        0      583 2024-04-20 10:13:12.779868 chess2vec-0.3.3b1/chess2vec/utils/vector.py
+-rw-r--r--   0        0        0      376 2024-04-24 13:42:41.744511 chess2vec-0.3.3b1/pyproject.toml
+-rw-r--r--   0        0        0      602 1970-01-01 00:00:00.000000 chess2vec-0.3.3b1/PKG-INFO
```

### Comparing `chess2vec-0.3.3/chess2vec/__init__.py` & `chess2vec-0.3.3b1/chess2vec/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import pickle
-from typing import Iterable, TextIO
+from typing import TextIO
 
 import chess
 import chess.pgn
 from tqdm import tqdm
 
 from chess2vec import components
+import gzip
 
 
 class Loader:
     def __init__(self, composition: components.Composition) -> None:
         self.composition = composition
         self.data = []
 
@@ -23,15 +24,15 @@
         if num_of_games is None:
             num_of_games = float("inf")
 
         if status:
             bar = tqdm(total=num_of_games)
 
         n = 0
-
+        
         while n < num_of_games:
             game = chess.pgn.read_game(pgn)
 
             if not game:
                 return False
 
             self.data.append(self.composition(game))
@@ -58,20 +59,20 @@
         return tuple(g['comp'] for g in self.data)
     
     def batched(self, batch_size):
         for idx in range(0, self.size, batch_size):
             yield self.data[idx : idx + batch_size]
 
     def save(self, file: str, *, batch_size=2**20) -> None:
-        with open(file, "wb") as f:
+        with gzip.open(file, "wb") as f:
             for batch in self.batched(batch_size):
                 pickle.dump(batch, f)
 
     def load(self, file: str) -> None:
-        with open(file, "rb") as f:
+        with gzip.open(file, "rb") as f:
             while True:
                 try:
                     self.data += pickle.load(f)
 
                 except EOFError:
                     return
```

### Comparing `chess2vec-0.3.3/chess2vec/components.py` & `chess2vec-0.3.3b1/chess2vec/components.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.3.3/chess2vec/utils/vector.py` & `chess2vec-0.3.3b1/chess2vec/utils/vector.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.3.3/PKG-INFO` & `chess2vec-0.3.3b1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: chess2vec
-Version: 0.3.3
+Version: 0.3.3b1
 Summary: 
 Author: Piotr Żarczyński
 Author-email: piotr.zarczynski.06@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: chess (>=1.10.0,<2.0.0)
-Requires-Dist: mgzip (>=0.2.1,<0.3.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: pytest (>=8.1.1,<9.0.0)
 Requires-Dist: scipy (>=1.13.0,<2.0.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Description-Content-Type: text/markdown
```

