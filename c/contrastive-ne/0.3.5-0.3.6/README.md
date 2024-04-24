# Comparing `tmp/contrastive_ne-0.3.5.tar.gz` & `tmp/contrastive_ne-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contrastive_ne-0.3.5.tar", last modified: Fri Apr 19 13:16:02 2024, max compression
+gzip compressed data, was "contrastive_ne-0.3.6.tar", last modified: Tue Apr 23 09:51:51 2024, max compression
```

## Comparing `contrastive_ne-0.3.5.tar` & `contrastive_ne-0.3.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 sdamrich  (1000) sdamrich  (1000)        0 2024-04-19 13:16:02.536645 contrastive_ne-0.3.5/
--rwxr-xr-x   0 sdamrich  (1000) sdamrich  (1000)     1228 2022-06-03 14:04:54.000000 contrastive_ne-0.3.5/LICENSE
--rw-r--r--   0 sdamrich  (1000) sdamrich  (1000)    13540 2024-04-19 13:16:02.536645 contrastive_ne-0.3.5/PKG-INFO
--rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)        6 2024-04-19 13:11:35.000000 contrastive_ne-0.3.5/VERSION
--rwxr-xr-x   0 sdamrich  (1000) sdamrich  (1000)      842 2023-12-07 09:42:08.000000 contrastive_ne-0.3.5/pyproject.toml
--rwxrwxr-x   0 sdamrich  (1000) sdamrich  (1000)    12894 2024-01-10 09:58:06.000000 contrastive_ne-0.3.5/readme.md
--rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)       38 2024-04-19 13:16:02.536645 contrastive_ne-0.3.5/setup.cfg
-drwxrwxr-x   0 sdamrich  (1000) sdamrich  (1000)        0 2024-04-19 13:16:02.536645 contrastive_ne-0.3.5/src/
-drwxrwxr-x   0 sdamrich  (1000) sdamrich  (1000)        0 2024-04-19 13:16:02.536645 contrastive_ne-0.3.5/src/cne/
--rwxr-xr-x   0 sdamrich  (1000) sdamrich  (1000)      112 2023-11-09 09:56:09.000000 contrastive_ne-0.3.5/src/cne/__init__.py
--rwxr-xr-x   0 sdamrich  (1000) sdamrich  (1000)    14263 2024-02-28 14:17:24.000000 contrastive_ne-0.3.5/src/cne/_cne.py
--rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)     6076 2024-04-10 08:53:32.000000 contrastive_ne-0.3.5/src/cne/callbacks.py
--rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)    29379 2024-04-19 13:03:09.000000 contrastive_ne-0.3.5/src/cne/cne.py
--rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)     8899 2023-02-08 10:47:49.000000 contrastive_ne-0.3.5/src/cne/old_loss_implementation.py
-drwxrwxr-x   0 sdamrich  (1000) sdamrich  (1000)        0 2024-04-19 13:16:02.536645 contrastive_ne-0.3.5/src/contrastive_ne.egg-info/
--rw-r--r--   0 sdamrich  (1000) sdamrich  (1000)    13540 2024-04-19 13:16:02.000000 contrastive_ne-0.3.5/src/contrastive_ne.egg-info/PKG-INFO
--rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)      370 2024-04-19 13:16:02.000000 contrastive_ne-0.3.5/src/contrastive_ne.egg-info/SOURCES.txt
--rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)        1 2024-04-19 13:16:02.000000 contrastive_ne-0.3.5/src/contrastive_ne.egg-info/dependency_links.txt
--rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)       88 2024-04-19 13:16:02.000000 contrastive_ne-0.3.5/src/contrastive_ne.egg-info/requires.txt
--rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)        4 2024-04-19 13:16:02.000000 contrastive_ne-0.3.5/src/contrastive_ne.egg-info/top_level.txt
-drwxrwxr-x   0 sdamrich  (1000) sdamrich  (1000)        0 2024-04-19 13:16:02.536645 contrastive_ne-0.3.5/tests/
--rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)      654 2024-01-10 16:14:33.000000 contrastive_ne-0.3.5/tests/test.py
+drwxrwxr-x   0 sdamrich  (1000) sdamrich  (1000)        0 2024-04-23 09:51:51.963486 contrastive_ne-0.3.6/
+-rwxr-xr-x   0 sdamrich  (1000) sdamrich  (1000)     1228 2022-06-03 14:04:54.000000 contrastive_ne-0.3.6/LICENSE
+-rw-r--r--   0 sdamrich  (1000) sdamrich  (1000)    13534 2024-04-23 09:51:51.963486 contrastive_ne-0.3.6/PKG-INFO
+-rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)        6 2024-04-23 09:50:28.000000 contrastive_ne-0.3.6/VERSION
+-rwxr-xr-x   0 sdamrich  (1000) sdamrich  (1000)      836 2024-04-23 07:18:11.000000 contrastive_ne-0.3.6/pyproject.toml
+-rwxrwxr-x   0 sdamrich  (1000) sdamrich  (1000)    12894 2024-01-10 09:58:06.000000 contrastive_ne-0.3.6/readme.md
+-rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)       38 2024-04-23 09:51:51.963486 contrastive_ne-0.3.6/setup.cfg
+drwxrwxr-x   0 sdamrich  (1000) sdamrich  (1000)        0 2024-04-23 09:51:51.959486 contrastive_ne-0.3.6/src/
+drwxrwxr-x   0 sdamrich  (1000) sdamrich  (1000)        0 2024-04-23 09:51:51.959486 contrastive_ne-0.3.6/src/cne/
+-rwxr-xr-x   0 sdamrich  (1000) sdamrich  (1000)      112 2023-11-09 09:56:09.000000 contrastive_ne-0.3.6/src/cne/__init__.py
+-rwxr-xr-x   0 sdamrich  (1000) sdamrich  (1000)    14367 2024-04-23 09:43:49.000000 contrastive_ne-0.3.6/src/cne/_cne.py
+-rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)     6076 2024-04-10 08:53:32.000000 contrastive_ne-0.3.6/src/cne/callbacks.py
+-rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)    29379 2024-04-23 09:44:28.000000 contrastive_ne-0.3.6/src/cne/cne.py
+-rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)     8899 2023-02-08 10:47:49.000000 contrastive_ne-0.3.6/src/cne/old_loss_implementation.py
+drwxrwxr-x   0 sdamrich  (1000) sdamrich  (1000)        0 2024-04-23 09:51:51.963486 contrastive_ne-0.3.6/src/contrastive_ne.egg-info/
+-rw-r--r--   0 sdamrich  (1000) sdamrich  (1000)    13534 2024-04-23 09:51:51.000000 contrastive_ne-0.3.6/src/contrastive_ne.egg-info/PKG-INFO
+-rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)      370 2024-04-23 09:51:51.000000 contrastive_ne-0.3.6/src/contrastive_ne.egg-info/SOURCES.txt
+-rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)        1 2024-04-23 09:51:51.000000 contrastive_ne-0.3.6/src/contrastive_ne.egg-info/dependency_links.txt
+-rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)       88 2024-04-23 09:51:51.000000 contrastive_ne-0.3.6/src/contrastive_ne.egg-info/requires.txt
+-rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)        4 2024-04-23 09:51:51.000000 contrastive_ne-0.3.6/src/contrastive_ne.egg-info/top_level.txt
+drwxrwxr-x   0 sdamrich  (1000) sdamrich  (1000)        0 2024-04-23 09:51:51.963486 contrastive_ne-0.3.6/tests/
+-rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)      654 2024-01-10 16:14:33.000000 contrastive_ne-0.3.6/tests/test.py
```

### Comparing `contrastive_ne-0.3.5/LICENSE` & `contrastive_ne-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `contrastive_ne-0.3.5/PKG-INFO` & `contrastive_ne-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: contrastive-ne
-Version: 0.3.5
+Version: 0.3.6
 Summary: Contrastive Neighbor Embeddings
 Author-email: Sebastian Damrich <sebastian.damrich@uni-tuebingen.de>, Niklas Böhm <jan-niklas.boehm@uni-tuebingen.de>
 License: MIT
 Project-URL: homepage, https://github.com/berenslab/contrastive-ne
 Classifier: Programming Language :: Python :: 3
-Requires-Python: <3.11,>=3.8
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.17
 Requires-Dist: scikit-learn>=0.23.2
 Requires-Dist: annoy
 Requires-Dist: matplotlib
 Requires-Dist: torchvision
```

### Comparing `contrastive_ne-0.3.5/pyproject.toml` & `contrastive_ne-0.3.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "annoy",
     "matplotlib",
     "torchvision",
     "torch>=1.10",
     "scipy",
     "pykeops"
 ]
-requires-python = ">=3.8,<3.11"
+requires-python = ">=3.8"
 license = {text = "MIT"}
 
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 
 [tool.setuptools.dynamic]
```

### Comparing `contrastive_ne-0.3.5/readme.md` & `contrastive_ne-0.3.6/readme.md`

 * *Files identical despite different names*

### Comparing `contrastive_ne-0.3.5/src/cne/_cne.py` & `contrastive_ne-0.3.6/src/cne/_cne.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,21 +128,24 @@
             self.indices = torch.randperm(self.dataset_len, device=self.device)
         else:
             self.indices = None
         self.i = 0
         return self
 
     def __next__(self):
-        if self.i > self.dataset_len - self.batch_size:
+        if (self.i > self.dataset_len - self.batch_size and self.drop_last) or self.i >= self.dataset_len:
             raise StopIteration
+
+        start = self.i
+        end = np.minimum(self.i + self.batch_size, self.dataset_len)
         if self.indices is not None:
-            indices = self.indices[self.i:self.i+self.batch_size]
+            indices = self.indices[start:end]
             batch = tuple(torch.index_select(t, 0, indices) for t in self.tensors)
         else:
-            batch = tuple(t[self.i:self.i+self.batch_size] for t in self.tensors)
+            batch = tuple(t[start:end] for t in self.tensors)
         self.i += self.batch_size
         return batch
 
     def __len__(self):
         return self.n_batches
```

### Comparing `contrastive_ne-0.3.5/src/cne/callbacks.py` & `contrastive_ne-0.3.6/src/cne/callbacks.py`

 * *Files identical despite different names*

### Comparing `contrastive_ne-0.3.5/src/cne/cne.py` & `contrastive_ne-0.3.6/src/cne/cne.py`

 * *Files identical despite different names*

### Comparing `contrastive_ne-0.3.5/src/cne/old_loss_implementation.py` & `contrastive_ne-0.3.6/src/cne/old_loss_implementation.py`

 * *Files identical despite different names*

### Comparing `contrastive_ne-0.3.5/src/contrastive_ne.egg-info/PKG-INFO` & `contrastive_ne-0.3.6/src/contrastive_ne.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: contrastive-ne
-Version: 0.3.5
+Version: 0.3.6
 Summary: Contrastive Neighbor Embeddings
 Author-email: Sebastian Damrich <sebastian.damrich@uni-tuebingen.de>, Niklas Böhm <jan-niklas.boehm@uni-tuebingen.de>
 License: MIT
 Project-URL: homepage, https://github.com/berenslab/contrastive-ne
 Classifier: Programming Language :: Python :: 3
-Requires-Python: <3.11,>=3.8
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.17
 Requires-Dist: scikit-learn>=0.23.2
 Requires-Dist: annoy
 Requires-Dist: matplotlib
 Requires-Dist: torchvision
```

### Comparing `contrastive_ne-0.3.5/tests/test.py` & `contrastive_ne-0.3.6/tests/test.py`

 * *Files identical despite different names*

