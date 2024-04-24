# Comparing `tmp/contrastive_ne-0.3.6.tar.gz` & `tmp/contrastive_ne-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contrastive_ne-0.3.6.tar", last modified: Tue Apr 23 09:51:51 2024, max compression
+gzip compressed data, was "contrastive_ne-0.3.7.tar", last modified: Wed Apr 24 08:09:25 2024, max compression
```

## Comparing `contrastive_ne-0.3.6.tar` & `contrastive_ne-0.3.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 sdamrich  (1000) sdamrich  (1000)        0 2024-04-23 09:51:51.963486 contrastive_ne-0.3.6/
--rwxr-xr-x   0 sdamrich  (1000) sdamrich  (1000)     1228 2022-06-03 14:04:54.000000 contrastive_ne-0.3.6/LICENSE
--rw-r--r--   0 sdamrich  (1000) sdamrich  (1000)    13534 2024-04-23 09:51:51.963486 contrastive_ne-0.3.6/PKG-INFO
--rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)        6 2024-04-23 09:50:28.000000 contrastive_ne-0.3.6/VERSION
--rwxr-xr-x   0 sdamrich  (1000) sdamrich  (1000)      836 2024-04-23 07:18:11.000000 contrastive_ne-0.3.6/pyproject.toml
--rwxrwxr-x   0 sdamrich  (1000) sdamrich  (1000)    12894 2024-01-10 09:58:06.000000 contrastive_ne-0.3.6/readme.md
--rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)       38 2024-04-23 09:51:51.963486 contrastive_ne-0.3.6/setup.cfg
-drwxrwxr-x   0 sdamrich  (1000) sdamrich  (1000)        0 2024-04-23 09:51:51.959486 contrastive_ne-0.3.6/src/
-drwxrwxr-x   0 sdamrich  (1000) sdamrich  (1000)        0 2024-04-23 09:51:51.959486 contrastive_ne-0.3.6/src/cne/
--rwxr-xr-x   0 sdamrich  (1000) sdamrich  (1000)      112 2023-11-09 09:56:09.000000 contrastive_ne-0.3.6/src/cne/__init__.py
--rwxr-xr-x   0 sdamrich  (1000) sdamrich  (1000)    14367 2024-04-23 09:43:49.000000 contrastive_ne-0.3.6/src/cne/_cne.py
--rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)     6076 2024-04-10 08:53:32.000000 contrastive_ne-0.3.6/src/cne/callbacks.py
--rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)    29379 2024-04-23 09:44:28.000000 contrastive_ne-0.3.6/src/cne/cne.py
--rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)     8899 2023-02-08 10:47:49.000000 contrastive_ne-0.3.6/src/cne/old_loss_implementation.py
-drwxrwxr-x   0 sdamrich  (1000) sdamrich  (1000)        0 2024-04-23 09:51:51.963486 contrastive_ne-0.3.6/src/contrastive_ne.egg-info/
--rw-r--r--   0 sdamrich  (1000) sdamrich  (1000)    13534 2024-04-23 09:51:51.000000 contrastive_ne-0.3.6/src/contrastive_ne.egg-info/PKG-INFO
--rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)      370 2024-04-23 09:51:51.000000 contrastive_ne-0.3.6/src/contrastive_ne.egg-info/SOURCES.txt
--rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)        1 2024-04-23 09:51:51.000000 contrastive_ne-0.3.6/src/contrastive_ne.egg-info/dependency_links.txt
--rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)       88 2024-04-23 09:51:51.000000 contrastive_ne-0.3.6/src/contrastive_ne.egg-info/requires.txt
--rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)        4 2024-04-23 09:51:51.000000 contrastive_ne-0.3.6/src/contrastive_ne.egg-info/top_level.txt
-drwxrwxr-x   0 sdamrich  (1000) sdamrich  (1000)        0 2024-04-23 09:51:51.963486 contrastive_ne-0.3.6/tests/
--rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)      654 2024-01-10 16:14:33.000000 contrastive_ne-0.3.6/tests/test.py
+drwxrwxr-x   0 sdamrich  (1000) sdamrich  (1000)        0 2024-04-24 08:09:25.472933 contrastive_ne-0.3.7/
+-rwxr-xr-x   0 sdamrich  (1000) sdamrich  (1000)     1228 2022-06-03 14:04:54.000000 contrastive_ne-0.3.7/LICENSE
+-rw-r--r--   0 sdamrich  (1000) sdamrich  (1000)    13534 2024-04-24 08:09:25.472933 contrastive_ne-0.3.7/PKG-INFO
+-rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)        6 2024-04-24 08:08:07.000000 contrastive_ne-0.3.7/VERSION
+-rwxr-xr-x   0 sdamrich  (1000) sdamrich  (1000)      836 2024-04-23 07:18:11.000000 contrastive_ne-0.3.7/pyproject.toml
+-rwxrwxr-x   0 sdamrich  (1000) sdamrich  (1000)    12894 2024-01-10 09:58:06.000000 contrastive_ne-0.3.7/readme.md
+-rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)       38 2024-04-24 08:09:25.472933 contrastive_ne-0.3.7/setup.cfg
+drwxrwxr-x   0 sdamrich  (1000) sdamrich  (1000)        0 2024-04-24 08:09:25.472933 contrastive_ne-0.3.7/src/
+drwxrwxr-x   0 sdamrich  (1000) sdamrich  (1000)        0 2024-04-24 08:09:25.472933 contrastive_ne-0.3.7/src/cne/
+-rwxr-xr-x   0 sdamrich  (1000) sdamrich  (1000)      112 2023-11-09 09:56:09.000000 contrastive_ne-0.3.7/src/cne/__init__.py
+-rwxr-xr-x   0 sdamrich  (1000) sdamrich  (1000)    14875 2024-04-24 08:08:48.000000 contrastive_ne-0.3.7/src/cne/_cne.py
+-rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)     6076 2024-04-10 08:53:32.000000 contrastive_ne-0.3.7/src/cne/callbacks.py
+-rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)    29379 2024-04-23 09:44:28.000000 contrastive_ne-0.3.7/src/cne/cne.py
+-rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)     8899 2023-02-08 10:47:49.000000 contrastive_ne-0.3.7/src/cne/old_loss_implementation.py
+drwxrwxr-x   0 sdamrich  (1000) sdamrich  (1000)        0 2024-04-24 08:09:25.472933 contrastive_ne-0.3.7/src/contrastive_ne.egg-info/
+-rw-r--r--   0 sdamrich  (1000) sdamrich  (1000)    13534 2024-04-24 08:09:25.000000 contrastive_ne-0.3.7/src/contrastive_ne.egg-info/PKG-INFO
+-rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)      370 2024-04-24 08:09:25.000000 contrastive_ne-0.3.7/src/contrastive_ne.egg-info/SOURCES.txt
+-rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)        1 2024-04-24 08:09:25.000000 contrastive_ne-0.3.7/src/contrastive_ne.egg-info/dependency_links.txt
+-rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)       88 2024-04-24 08:09:25.000000 contrastive_ne-0.3.7/src/contrastive_ne.egg-info/requires.txt
+-rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)        4 2024-04-24 08:09:25.000000 contrastive_ne-0.3.7/src/contrastive_ne.egg-info/top_level.txt
+drwxrwxr-x   0 sdamrich  (1000) sdamrich  (1000)        0 2024-04-24 08:09:25.472933 contrastive_ne-0.3.7/tests/
+-rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)      654 2024-04-24 08:07:31.000000 contrastive_ne-0.3.7/tests/test.py
```

### Comparing `contrastive_ne-0.3.6/LICENSE` & `contrastive_ne-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `contrastive_ne-0.3.6/PKG-INFO` & `contrastive_ne-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contrastive-ne
-Version: 0.3.6
+Version: 0.3.7
 Summary: Contrastive Neighbor Embeddings
 Author-email: Sebastian Damrich <sebastian.damrich@uni-tuebingen.de>, Niklas Böhm <jan-niklas.boehm@uni-tuebingen.de>
 License: MIT
 Project-URL: homepage, https://github.com/berenslab/contrastive-ne
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `contrastive_ne-0.3.6/pyproject.toml` & `contrastive_ne-0.3.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `contrastive_ne-0.3.6/readme.md` & `contrastive_ne-0.3.7/readme.md`

 * *Files identical despite different names*

### Comparing `contrastive_ne-0.3.6/src/cne/_cne.py` & `contrastive_ne-0.3.7/src/cne/_cne.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,47 +104,47 @@
         if data_on_gpu:
             self.device = "cuda"
             tensors = [tensor.to(self.device) for tensor in tensors]
         else:
             self.device = "cpu"
         self.tensors = tensors
 
-        self.dataset_len = self.tensors[0].shape[0]
-        self.batch_size = batch_size
+        self.dataset_len = torch.tensor(self.tensors[0].shape[0], device=self.device)
+        self.batch_size = torch.tensor(batch_size, dtype=int).to(self.device)
+
         self.shuffle = shuffle
         self.drop_last = drop_last
         self.seed = seed
         torch.manual_seed(self.seed)
 
         # Calculate number of  batches
-        n_batches, remainder = divmod(self.dataset_len, self.batch_size)
+        n_batches = torch.div(self.dataset_len, self.batch_size, rounding_mode="floor")
+        remainder = torch.remainder(self.dataset_len, self.batch_size)
         if remainder > 0 and not self.drop_last:
             n_batches += 1
         self.n_batches = n_batches
 
-        self.batch_size = torch.tensor(self.batch_size, dtype=int).to(self.device)
-
     def __iter__(self):
         if self.shuffle:
             self.indices = torch.randperm(self.dataset_len, device=self.device)
         else:
             self.indices = None
-        self.i = 0
+        self.i = torch.tensor(0, device=self.device)
         return self
 
     def __next__(self):
         if (self.i > self.dataset_len - self.batch_size and self.drop_last) or self.i >= self.dataset_len:
             raise StopIteration
 
         start = self.i
-        end = np.minimum(self.i + self.batch_size, self.dataset_len)
+        end = torch.minimum(self.i + self.batch_size, self.dataset_len)
         if self.indices is not None:
             indices = self.indices[start:end]
             batch = tuple(torch.index_select(t, 0, indices) for t in self.tensors)
-        else:
+        else:D
             batch = tuple(t[start:end] for t in self.tensors)
         self.i += self.batch_size
         return batch
 
     def __len__(self):
         return self.n_batches
 
@@ -175,31 +175,35 @@
     Manages contrastive neighbor embeddings.
     """
     def __init__(self,
                  model=None,
                  k=15,
                  parametric=False,
                  data_on_gpu="auto",
+                 use_keops=None,
                  seed=0,
                  anneal_lr=True,
                  embd_dim=2,
                  **kwargs):
         """
         :param model: Embedding model
         :param k: int Number of nearest neighbors
         :param parametric: bool If True and model=None uses a parametric embedding model
         :param data_on_gpu: bool or "auto" Load whole dataset to GPU and try to use pykeops for kNN graph if possible.
+        :param use_keops: bool If True use pykeops for kNN graph computation. If False use annoy. Supercedes the kNN
+        graph selection by data_on_gpu if not None.
         :param seed: int Random seed
         :param anneal_lr: bool If True anneal the learning rate linearly.
         :param kwargs:
         """
         self.model = model
         self.k = k
         self.parametric = parametric
         self.data_on_gpu = data_on_gpu
+        self.use_keops = use_keops
         self.kwargs = kwargs
         self.seed = seed
         self.anneal_lr = anneal_lr
         self.embd_dim = embd_dim
 
 
     def fit_transform(self, X, init=None, graph=None):
@@ -289,22 +293,26 @@
                                         seed=self.seed,
                                         anneal_lr=self.anneal_lr,
                                         **self.kwargs)
 
         # is no graph is passed, compute the similarity graph with pykeops is cuda is available and otherwise annoy
         if graph is None:
             # select annoy or pykeops depending on data_on_gpu and availability of pykeops
-            if self.cne.device == "cuda":
-                try:
-                    import pykeops
-                    graph = "pykeops"
-                except ImportError:
+            if self.use_keops is None:
+                if self.cne.device == "cuda":
+                    try:
+                        import pykeops
+                        graph = "pykeops"
+                    except ImportError:
+                        graph = "annoy"
+                else:
                     graph = "annoy"
             else:
-                graph = "annoy"
+                graph = "pykeops" if self.use_keops else "annoy"
+
 
         if isinstance(graph, str):
             if graph == "annoy":
                 print("Computing approximate kNN graph with annoy")
                 # create approximate NN search tree
                 self.annoy = AnnoyIndex(in_dim, "euclidean")
                 [self.annoy.add_item(i, x) for i, x in enumerate(X)]
```

### Comparing `contrastive_ne-0.3.6/src/cne/callbacks.py` & `contrastive_ne-0.3.7/src/cne/callbacks.py`

 * *Files identical despite different names*

### Comparing `contrastive_ne-0.3.6/src/cne/cne.py` & `contrastive_ne-0.3.7/src/cne/cne.py`

 * *Files identical despite different names*

### Comparing `contrastive_ne-0.3.6/src/cne/old_loss_implementation.py` & `contrastive_ne-0.3.7/src/cne/old_loss_implementation.py`

 * *Files identical despite different names*

### Comparing `contrastive_ne-0.3.6/src/contrastive_ne.egg-info/PKG-INFO` & `contrastive_ne-0.3.7/src/contrastive_ne.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contrastive-ne
-Version: 0.3.6
+Version: 0.3.7
 Summary: Contrastive Neighbor Embeddings
 Author-email: Sebastian Damrich <sebastian.damrich@uni-tuebingen.de>, Niklas Böhm <jan-niklas.boehm@uni-tuebingen.de>
 License: MIT
 Project-URL: homepage, https://github.com/berenslab/contrastive-ne
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `contrastive_ne-0.3.6/tests/test.py` & `contrastive_ne-0.3.7/tests/test.py`

 * *Files identical despite different names*

