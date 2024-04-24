# Comparing `tmp/chess2vec-0.3.3b1.tar.gz` & `tmp/chess2vec-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess2vec-0.3.3b1.tar", max compression
+gzip compressed data, was "chess2vec-0.3.4.tar", max compression
```

## Comparing `chess2vec-0.3.3b1.tar` & `chess2vec-0.3.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2024-04-20 10:13:12.779868 chess2vec-0.3.3b1/README.md
--rw-r--r--   0        0        0     1889 2024-04-24 13:41:37.874178 chess2vec-0.3.3b1/chess2vec/__init__.py
--rw-r--r--   0        0        0     2375 2024-04-24 13:38:13.616449 chess2vec-0.3.3b1/chess2vec/components.py
--rw-r--r--   0        0        0      287 2024-04-23 21:18:28.472128 chess2vec-0.3.3b1/chess2vec/pgn.py
--rw-r--r--   0        0        0      202 2024-04-23 21:28:35.524582 chess2vec-0.3.3b1/chess2vec/utils/__init__.py
--rw-r--r--   0        0        0      583 2024-04-20 10:13:12.779868 chess2vec-0.3.3b1/chess2vec/utils/vector.py
--rw-r--r--   0        0        0      376 2024-04-24 13:42:41.744511 chess2vec-0.3.3b1/pyproject.toml
--rw-r--r--   0        0        0      602 1970-01-01 00:00:00.000000 chess2vec-0.3.3b1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-20 10:13:12.779868 chess2vec-0.3.4/README.md
+-rw-r--r--   0        0        0     1925 2024-04-24 16:16:47.781522 chess2vec-0.3.4/chess2vec/__init__.py
+-rw-r--r--   0        0        0     2375 2024-04-24 13:38:13.616449 chess2vec-0.3.4/chess2vec/components.py
+-rw-r--r--   0        0        0      287 2024-04-23 21:18:28.472128 chess2vec-0.3.4/chess2vec/pgn.py
+-rw-r--r--   0        0        0      202 2024-04-23 21:28:35.524582 chess2vec-0.3.4/chess2vec/utils/__init__.py
+-rw-r--r--   0        0        0      583 2024-04-20 10:13:12.779868 chess2vec-0.3.4/chess2vec/utils/vector.py
+-rw-r--r--   0        0        0      374 2024-04-24 16:17:10.278798 chess2vec-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      600 1970-01-01 00:00:00.000000 chess2vec-0.3.4/PKG-INFO
```

### Comparing `chess2vec-0.3.3b1/chess2vec/__init__.py` & `chess2vec-0.3.4/chess2vec/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,25 +15,25 @@
         self.data = []
 
     @property
     def size(self) -> int:
         return len(self.data)
 
     def load_pgn(
-        self, pgn: TextIO, num_of_games: int = None, status: bool = False
+        self, pgn: TextIO, n_games: int = None, status: bool = False
     ) -> bool:
-        if num_of_games is None:
-            num_of_games = float("inf")
+        if n_games is None:
+            n_games = float("inf")
 
         if status:
-            bar = tqdm(total=num_of_games)
+            bar = tqdm(total=n_games)
 
         n = 0
         
-        while n < num_of_games:
+        while n < n_games:
             game = chess.pgn.read_game(pgn)
 
             if not game:
                 return False
 
             self.data.append(self.composition(game))
 
@@ -58,16 +58,18 @@
     def comp(self):
         return tuple(g['comp'] for g in self.data)
     
     def batched(self, batch_size):
         for idx in range(0, self.size, batch_size):
             yield self.data[idx : idx + batch_size]
 
-    def save(self, file: str, *, batch_size=2**20) -> None:
-        with gzip.open(file, "wb") as f:
+    def save(self, file: str, new: bool = True, batch_size=2**16) -> None:
+        mode = "wb" if new else "ab"
+        
+        with gzip.open(file, mode) as f:
             for batch in self.batched(batch_size):
                 pickle.dump(batch, f)
 
     def load(self, file: str) -> None:
         with gzip.open(file, "rb") as f:
             while True:
                 try:
```

### Comparing `chess2vec-0.3.3b1/chess2vec/components.py` & `chess2vec-0.3.4/chess2vec/components.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.3.3b1/chess2vec/utils/vector.py` & `chess2vec-0.3.4/chess2vec/utils/vector.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.3.3b1/PKG-INFO` & `chess2vec-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chess2vec
-Version: 0.3.3b1
+Version: 0.3.4
 Summary: 
 Author: Piotr Żarczyński
 Author-email: piotr.zarczynski.06@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

