# Comparing `tmp/fast_string_match-0.1.3.tar.gz` & `tmp/fast_string_match-0.1.4.tar.gz`

## Comparing `fast_string_match-0.1.3.tar` & `fast_string_match-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      313 1970-01-01 00:00:00.000000 fast_string_match-0.1.3/Cargo.toml
--rw-r--r--   0        0        0     5745 2024-04-23 22:27:47.000000 fast_string_match-0.1.3/src/lib.rs
--rw-r--r--   0        0        0     9025 2024-04-23 22:29:22.000000 fast_string_match-0.1.3/Cargo.lock
--rw-r--r--   0        0        0      565 2024-04-23 21:18:20.000000 fast_string_match-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      422 1970-01-01 00:00:00.000000 fast_string_match-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      313 1970-01-01 00:00:00.000000 fast_string_match-0.1.4/Cargo.toml
+-rw-r--r--   0        0        0     5792 2024-04-23 23:04:25.000000 fast_string_match-0.1.4/src/lib.rs
+-rw-r--r--   0        0        0     9025 2024-04-23 23:05:13.000000 fast_string_match-0.1.4/Cargo.lock
+-rw-r--r--   0        0        0      583 2024-04-23 23:05:03.000000 fast_string_match-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      440 1970-01-01 00:00:00.000000 fast_string_match-0.1.4/PKG-INFO
```

### Comparing `fast_string_match-0.1.3/src/lib.rs` & `fast_string_match-0.1.4/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -152,27 +152,27 @@
     }
     None
 }
 
 #[pyfunction]
 fn closest_match_distance<'a>(_py: Python, query: &str, options: Vec<&'a str>) -> Option<String> {
     let mut decoded_strings = Vec::new();
-    for option in options {
-        decoded_strings.push(unidecode(option).to_string());
+    for option in &options {
+        decoded_strings.push(unidecode(option).to_string().to_lowercase());
     }
     let slice_of_string_slices: Vec<&str> = decoded_strings.iter().map(|s| s.as_str()).collect();
     let closest = find_closest_match(&unidecode(query), &slice_of_string_slices);
     
     // If a closest match is found, find the case exact match in decoded_strings
     if let Some(closest_str) = closest {
         // Iterate through decoded_strings to find the exact case match
-        for option in &decoded_strings {
-            if option == closest_str {
+        for option in &options {
+            if option.to_string().to_lowercase() == closest_str {
                 // Return the closest match as it appears in decoded_strings
-                return Some(option.clone());
+                return Some(option.to_string().clone());
             }
         }
     }
     None
 }
 #[pymodule]
 fn fast_string_match(_py: Python, m: &PyModule) -> PyResult<()> {
```

### Comparing `fast_string_match-0.1.3/Cargo.lock` & `fast_string_match-0.1.4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 name = "crossbeam-utils"
 version = "0.8.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
 
 [[package]]
 name = "fast_string_match"
-version = "0.1.3"
+version = "0.1.4"
 dependencies = [
  "pyo3",
  "rayon",
  "strsim",
  "unidecode",
 ]
```

### Comparing `fast_string_match-0.1.3/pyproject.toml` & `fast_string_match-0.1.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["maturin>=1.4,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "fast_string_match"
 description = """fast string matching built in rust for python, use would be 
-from fast_closest_match import closest_match_py
-return closest_match_py(query,values)"""
+from fast_closest_match import closest_match, closest_match_distance
+return closest_match(query,values)"""
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dynamic = ["version"]
```

