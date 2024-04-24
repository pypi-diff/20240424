# Comparing `tmp/kiddo_python_bindings-0.1.1.tar.gz` & `tmp/kiddo_python_bindings-0.1.2.tar.gz`

## Comparing `kiddo_python_bindings-0.1.1.tar` & `kiddo_python_bindings-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      344 1970-01-01 00:00:00.000000 kiddo_python_bindings-0.1.1/Cargo.toml
--rw-r--r--   0      501       20     3526 2024-04-22 18:49:14.000000 kiddo_python_bindings-0.1.1/.github/workflows/CI.yml
--rw-r--r--   0      501       20      686 2024-04-22 18:49:14.000000 kiddo_python_bindings-0.1.1/.gitignore
--rw-r--r--   0      501       20     1275 2024-04-23 12:19:52.000000 kiddo_python_bindings-0.1.1/README.md
--rw-r--r--   0      501       20      396 2024-04-23 12:17:00.000000 kiddo_python_bindings-0.1.1/example.py
--rw-r--r--   0      501       20     1275 2024-04-23 12:19:52.000000 kiddo_python_bindings-0.1.1/readme.md
--rw-r--r--   0      501       20     3169 2024-04-23 12:14:15.000000 kiddo_python_bindings-0.1.1/src/lib.rs
--rw-r--r--   0      501       20    17860 2024-04-23 12:21:47.000000 kiddo_python_bindings-0.1.1/Cargo.lock
--rw-r--r--   0      501       20      401 2024-04-23 12:21:44.000000 kiddo_python_bindings-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1615 1970-01-01 00:00:00.000000 kiddo_python_bindings-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      344 1970-01-01 00:00:00.000000 kiddo_python_bindings-0.1.2/Cargo.toml
+-rw-r--r--   0     1001      127     3526 2024-04-24 16:43:18.000000 kiddo_python_bindings-0.1.2/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      686 2024-04-24 16:43:18.000000 kiddo_python_bindings-0.1.2/.gitignore
+-rw-r--r--   0     1001      127     1688 2024-04-24 16:43:18.000000 kiddo_python_bindings-0.1.2/bechmark.py
+-rw-r--r--   0     1001      127      396 2024-04-24 16:43:18.000000 kiddo_python_bindings-0.1.2/example.py
+-rw-r--r--   0     1001      127     1498 2024-04-24 16:43:18.000000 kiddo_python_bindings-0.1.2/readme.md
+-rw-r--r--   0     1001      127     3206 2024-04-24 16:43:18.000000 kiddo_python_bindings-0.1.2/src/lib.rs
+-rw-r--r--   0     1001      127    17860 2024-04-24 16:43:18.000000 kiddo_python_bindings-0.1.2/Cargo.lock
+-rw-r--r--   0     1001      127      401 2024-04-24 16:43:18.000000 kiddo_python_bindings-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      270 1970-01-01 00:00:00.000000 kiddo_python_bindings-0.1.2/PKG-INFO
```

### Comparing `kiddo_python_bindings-0.1.1/.github/workflows/CI.yml` & `kiddo_python_bindings-0.1.2/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `kiddo_python_bindings-0.1.1/.gitignore` & `kiddo_python_bindings-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `kiddo_python_bindings-0.1.1/README.md` & `kiddo_python_bindings-0.1.2/readme.md`

 * *Files 21% similar despite different names*

```diff
@@ -46,7 +46,10 @@
 Within (
     array([0, 4, 5, 6, 7, 9], dtype=uint64),
     array([0.08116178, 1.9392966 , 0.3743909 , 1.3634278 , 1.0922432 ,
        0.25775522], dtype=float32)
 )
 Num close 6
 ```
+
+> I am probably not smart, when it comes to benchmarking, but here goes nothing:
+<img width="686" alt="image" src="https://github.com/awarebayes/Kiddo-Python-Bindings/assets/42784580/4a5fe49a-3d3a-407f-8f19-433553848073">
```

### Comparing `kiddo_python_bindings-0.1.1/src/lib.rs` & `kiddo_python_bindings-0.1.2/src/lib.rs`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     py: Python<'py>,
     neighbours: Vec<NearestNeighbour<f32, u64>>,
 ) -> PyObject {
     let mut distances_vec: Vec<f32> = Vec::new();
     let mut indices_vec: Vec<u64> = Vec::new();
 
     for n in neighbours {
-        distances_vec.push(n.distance);
+        distances_vec.push(n.distance.sqrt());
         indices_vec.push(n.item);
     }
 
     let distance = PyArray1::from_vec_bound(py, distances_vec);
     let indices = PyArray1::from_vec_bound(py, indices_vec);
     PyTuple::new_bound(py, &[indices.to_object(py), distance.to_object(py)]).to_object(py)
 }
@@ -62,40 +62,40 @@
         dist: f32,
         max_neighbours: usize,
         sorted: bool,
     ) -> PyObject {
         let query_view_2 = two_d_query(query_);
         let neighbours = self.tree.nearest_n_within::<SquaredEuclidean>(
             &query_view_2,
-            dist,
+            dist.powf(2.0),
             max_neighbours,
             sorted,
         );
         let neighbours_vec = Vec::from_iter(neighbours);
         nearest_neighbours_to_object(py, neighbours_vec)
     }
 
     fn count_within<'py>(&self, query_: PyReadonlyArray1<'py, f32>, dist: f32) -> usize {
         let query_view_2 = two_d_query(query_);
         let neighbours = self
             .tree
-            .within_unsorted::<SquaredEuclidean>(&query_view_2, dist);
+            .within_unsorted::<SquaredEuclidean>(&query_view_2, dist.powf(2.0));
         neighbours.len()
     }
 
     fn within<'py>(
         &self,
         py: Python<'py>,
         query_: PyReadonlyArray1<'py, f32>,
         dist: f32,
     ) -> PyObject {
         let query_view_2 = two_d_query(query_);
         let neighbours = self
             .tree
-            .within_unsorted::<SquaredEuclidean>(&query_view_2, dist);
+            .within_unsorted::<SquaredEuclidean>(&query_view_2, dist.powf(2.0));
         let neighbours_vec = Vec::from_iter(neighbours);
         nearest_neighbours_to_object(py, neighbours_vec)
     }
 }
 
 #[pymodule]
 fn kiddo_python_bindings(_py: Python, m: &PyModule) -> PyResult<()> {
```

### Comparing `kiddo_python_bindings-0.1.1/Cargo.lock` & `kiddo_python_bindings-0.1.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -152,15 +152,15 @@
  "tracing",
  "tracing-subscriber",
  "ubyte",
 ]
 
 [[package]]
 name = "kiddo_python_bindings"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
  "kiddo",
  "numpy",
  "pyo3",
 ]
 
 [[package]]
```

