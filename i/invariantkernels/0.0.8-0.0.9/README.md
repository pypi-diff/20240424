# Comparing `tmp/invariantkernels-0.0.8.tar.gz` & `tmp/invariantkernels-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invariantkernels-0.0.8.tar", last modified: Mon Apr 22 11:04:03 2024, max compression
+gzip compressed data, was "invariantkernels-0.0.9.tar", last modified: Mon Apr 22 11:58:26 2024, max compression
```

## Comparing `invariantkernels-0.0.8.tar` & `invariantkernels-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 theo      (1000) theo      (1000)        0 2024-04-22 11:04:03.184344 invariantkernels-0.0.8/
--rw-rw-r--   0 theo      (1000) theo      (1000)     1071 2024-03-01 12:02:46.000000 invariantkernels-0.0.8/LICENSE
--rw-r--r--   0 theo      (1000) theo      (1000)     1081 2024-04-22 11:04:03.184344 invariantkernels-0.0.8/PKG-INFO
--rw-rw-r--   0 theo      (1000) theo      (1000)      582 2024-03-26 12:05:25.000000 invariantkernels-0.0.8/README.md
-drwxrwxr-x   0 theo      (1000) theo      (1000)        0 2024-04-22 11:04:03.184344 invariantkernels-0.0.8/invariantkernels/
--rw-rw-r--   0 theo      (1000) theo      (1000)      269 2024-04-22 11:03:21.000000 invariantkernels-0.0.8/invariantkernels/__init__.py
--rw-rw-r--   0 theo      (1000) theo      (1000)     2863 2024-04-22 11:01:01.000000 invariantkernels-0.0.8/invariantkernels/anisotropic_group_invariant_kernel.py
--rw-rw-r--   0 theo      (1000) theo      (1000)     2786 2024-04-22 11:01:03.000000 invariantkernels-0.0.8/invariantkernels/isotropic_group_invariant_kernel.py
--rw-rw-r--   0 theo      (1000) theo      (1000)     1477 2024-04-22 11:03:21.000000 invariantkernels-0.0.8/invariantkernels/transformation_groups.py
-drwxrwxr-x   0 theo      (1000) theo      (1000)        0 2024-04-22 11:04:03.184344 invariantkernels-0.0.8/invariantkernels.egg-info/
--rw-r--r--   0 theo      (1000) theo      (1000)     1081 2024-04-22 11:04:03.000000 invariantkernels-0.0.8/invariantkernels.egg-info/PKG-INFO
--rw-rw-r--   0 theo      (1000) theo      (1000)      410 2024-04-22 11:04:03.000000 invariantkernels-0.0.8/invariantkernels.egg-info/SOURCES.txt
--rw-rw-r--   0 theo      (1000) theo      (1000)        1 2024-04-22 11:04:03.000000 invariantkernels-0.0.8/invariantkernels.egg-info/dependency_links.txt
--rw-rw-r--   0 theo      (1000) theo      (1000)        9 2024-04-22 11:04:03.000000 invariantkernels-0.0.8/invariantkernels.egg-info/requires.txt
--rw-rw-r--   0 theo      (1000) theo      (1000)       17 2024-04-22 11:04:03.000000 invariantkernels-0.0.8/invariantkernels.egg-info/top_level.txt
--rw-rw-r--   0 theo      (1000) theo      (1000)      637 2024-04-22 11:02:38.000000 invariantkernels-0.0.8/pyproject.toml
--rw-rw-r--   0 theo      (1000) theo      (1000)       38 2024-04-22 11:04:03.184344 invariantkernels-0.0.8/setup.cfg
+drwxrwxr-x   0 theo      (1000) theo      (1000)        0 2024-04-22 11:58:26.384211 invariantkernels-0.0.9/
+-rw-rw-r--   0 theo      (1000) theo      (1000)     1071 2024-03-01 12:02:46.000000 invariantkernels-0.0.9/LICENSE
+-rw-r--r--   0 theo      (1000) theo      (1000)     1081 2024-04-22 11:58:26.384211 invariantkernels-0.0.9/PKG-INFO
+-rw-rw-r--   0 theo      (1000) theo      (1000)      582 2024-04-22 11:04:05.000000 invariantkernels-0.0.9/README.md
+drwxrwxr-x   0 theo      (1000) theo      (1000)        0 2024-04-22 11:58:26.384211 invariantkernels-0.0.9/invariantkernels/
+-rw-rw-r--   0 theo      (1000) theo      (1000)      234 2024-04-22 11:58:00.000000 invariantkernels-0.0.9/invariantkernels/__init__.py
+-rw-rw-r--   0 theo      (1000) theo      (1000)     2865 2024-04-22 11:56:33.000000 invariantkernels-0.0.9/invariantkernels/anisotropic_group_invariant_kernel.py
+-rw-rw-r--   0 theo      (1000) theo      (1000)     2786 2024-04-22 11:01:03.000000 invariantkernels-0.0.9/invariantkernels/isotropic_group_invariant_kernel.py
+-rw-rw-r--   0 theo      (1000) theo      (1000)     1492 2024-04-22 11:56:10.000000 invariantkernels-0.0.9/invariantkernels/transformation_groups.py
+drwxrwxr-x   0 theo      (1000) theo      (1000)        0 2024-04-22 11:58:26.384211 invariantkernels-0.0.9/invariantkernels.egg-info/
+-rw-r--r--   0 theo      (1000) theo      (1000)     1081 2024-04-22 11:58:26.000000 invariantkernels-0.0.9/invariantkernels.egg-info/PKG-INFO
+-rw-rw-r--   0 theo      (1000) theo      (1000)      410 2024-04-22 11:58:26.000000 invariantkernels-0.0.9/invariantkernels.egg-info/SOURCES.txt
+-rw-rw-r--   0 theo      (1000) theo      (1000)        1 2024-04-22 11:58:26.000000 invariantkernels-0.0.9/invariantkernels.egg-info/dependency_links.txt
+-rw-rw-r--   0 theo      (1000) theo      (1000)        9 2024-04-22 11:58:26.000000 invariantkernels-0.0.9/invariantkernels.egg-info/requires.txt
+-rw-rw-r--   0 theo      (1000) theo      (1000)       17 2024-04-22 11:58:26.000000 invariantkernels-0.0.9/invariantkernels.egg-info/top_level.txt
+-rw-rw-r--   0 theo      (1000) theo      (1000)      637 2024-04-22 11:57:33.000000 invariantkernels-0.0.9/pyproject.toml
+-rw-rw-r--   0 theo      (1000) theo      (1000)       38 2024-04-22 11:58:26.384211 invariantkernels-0.0.9/setup.cfg
```

### Comparing `invariantkernels-0.0.8/LICENSE` & `invariantkernels-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `invariantkernels-0.0.8/PKG-INFO` & `invariantkernels-0.0.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invariantkernels
-Version: 0.0.8
+Version: 0.0.9
 Summary: Transformation-invariant kernels in GPyTorch
 Author-email: Theodore Brown <theo.brown.uk@gmail.com>
 Project-URL: Homepage, https://github.com/theo-brown/invariantkernels
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
@@ -18,9 +18,9 @@
 This package provides kernels for Gaussian processes that are invariant to transformations.
 The core class is `GroupInvariantKernel`, which can be composed with other GPyTorch kernels to make them invariant to a group of transformations.
 Example groups are in [`invariant_kernels/transformation_groups`](./invariantkernels/transformation_groups.py).
 
 ## Build notes 
 1. Update the version in `pyproject.toml`
 2. Remove the old versions from `build/` and `dist/`
-3. Run `python -m` build
+3. Run `python -m build`
 4. Run `twine upload dist/*`
```

### Comparing `invariantkernels-0.0.8/README.md` & `invariantkernels-0.0.9/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -4,9 +4,9 @@
 This package provides kernels for Gaussian processes that are invariant to transformations.
 The core class is `GroupInvariantKernel`, which can be composed with other GPyTorch kernels to make them invariant to a group of transformations.
 Example groups are in [`invariant_kernels/transformation_groups`](./invariantkernels/transformation_groups.py).
 
 ## Build notes 
 1. Update the version in `pyproject.toml`
 2. Remove the old versions from `build/` and `dist/`
-3. Run `python -m` build
+3. Run `python -m build`
 4. Run `twine upload dist/*`
```

### Comparing `invariantkernels-0.0.8/invariantkernels/anisotropic_group_invariant_kernel.py` & `invariantkernels-0.0.9/invariantkernels/anisotropic_group_invariant_kernel.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     def forward(
         self, x1, x2, diag: bool = False, last_dim_is_batch: bool = False, **kwargs
     ) -> torch.tensor:
         # TODO: Use __call__, which means we need to make it lazy
 
         if last_dim_is_batch:
             raise NotImplementedError(
-                "last_dim_is_batch=True not implemented for IsotropicGroupInvariantKernel."
+                "last_dim_is_batch=True not implemented for AnisotropicGroupInvariantKernel."
             )
 
         # Note: we are optimising for memory usage first, and then performance afterwards.
         N = x1.shape[-2]
         M = x2.shape[-2]
         if len(x1.shape) == 2:
             K = torch.zeros(N, M, device=x1.device, dtype=x1.dtype)
```

### Comparing `invariantkernels-0.0.8/invariantkernels/isotropic_group_invariant_kernel.py` & `invariantkernels-0.0.9/invariantkernels/isotropic_group_invariant_kernel.py`

 * *Files identical despite different names*

### Comparing `invariantkernels-0.0.8/invariantkernels/transformation_groups.py` & `invariantkernels-0.0.9/invariantkernels/transformation_groups.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import itertools
 from typing import Iterator
 
 import torch
 
 
-def permutations(x: torch.Tensor) -> Iterator[torch.Tensor]:
+def permutation_group(x: torch.Tensor) -> Iterator[torch.Tensor]:
     """Generator that produces all permutations of the last dimension of x."""
     d = x.shape[-1]
     indices = torch.arange(0, d)
     for p in itertools.permutations(indices):
         yield x[..., p].squeeze()
 
 
-def block_permutations(x: torch.Tensor, block_size: int) -> Iterator[torch.Tensor]:
+def block_permutation_group(x: torch.Tensor, block_size: int) -> Iterator[torch.Tensor]:
     """Generator that produces all permutations of the last dimension of x in blocks of size block_size."""
     d = x.shape[-1]
     if d % block_size != 0:
         raise ValueError(
             f"Last dimension of x must be a multiple of block size (got {d} and {block_size} respectively)."
         )
     # block_indices is a tensor of shape (block_size, d // block_size)
@@ -29,9 +29,9 @@
 
     # Applying the permutations to the last dimension of block_indices
     # will give us all possible block permutations
     # e.g. for d = 6 and block_size = 2, we get
     # tensor([[0, 2, 4], [1, 3, 5]]), tensor([[2, 0, 4], [3, 1, 5]]), ...
     # Transpose and flatten to get
     # tensor([0, 2, 4, 1, 3, 5]), tensor([2, 0, 4, 3, 1, 5]), ...
-    for p in permutations(block_indices):
+    for p in permutation_group(block_indices):
         yield x[..., p.T.flatten()].squeeze()
```

### Comparing `invariantkernels-0.0.8/invariantkernels.egg-info/PKG-INFO` & `invariantkernels-0.0.9/invariantkernels.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invariantkernels
-Version: 0.0.8
+Version: 0.0.9
 Summary: Transformation-invariant kernels in GPyTorch
 Author-email: Theodore Brown <theo.brown.uk@gmail.com>
 Project-URL: Homepage, https://github.com/theo-brown/invariantkernels
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
@@ -18,9 +18,9 @@
 This package provides kernels for Gaussian processes that are invariant to transformations.
 The core class is `GroupInvariantKernel`, which can be composed with other GPyTorch kernels to make them invariant to a group of transformations.
 Example groups are in [`invariant_kernels/transformation_groups`](./invariantkernels/transformation_groups.py).
 
 ## Build notes 
 1. Update the version in `pyproject.toml`
 2. Remove the old versions from `build/` and `dist/`
-3. Run `python -m` build
+3. Run `python -m build`
 4. Run `twine upload dist/*`
```

### Comparing `invariantkernels-0.0.8/pyproject.toml` & `invariantkernels-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "invariantkernels"
-version = "0.0.8"
+version = "0.0.9"
 dependencies = [
   "gpytorch"
 ]
 description = "Transformation-invariant kernels in GPyTorch"
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [
```

