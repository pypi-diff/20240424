# Comparing `tmp/moyopy-0.1.4.tar.gz` & `tmp/moyopy-0.1.6.tar.gz`

## Comparing `moyopy-0.1.4.tar` & `moyopy-0.1.6.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0     1001      127      903 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/Cargo.toml
--rw-r--r--   0     1001      127      245 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/README.md
--rw-r--r--   0     1001      127      703 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/benches/dataset.rs
--rw-r--r--   0     1001      127     2493 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/benches/translation_search.rs
--rw-r--r--   0     1001      127     2926 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/src/base/cell.rs
--rw-r--r--   0     1001      127     1123 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/src/base/error.rs
--rw-r--r--   0     1001      127     2932 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/src/base/lattice.rs
--rw-r--r--   0     1001      127     3830 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/src/base/operation.rs
--rw-r--r--   0     1001      127     2146 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/src/base/tolerance.rs
--rw-r--r--   0     1001      127     9891 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/src/base/transformation.rs
--rw-r--r--   0     1001      127      559 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/src/base.rs
--rw-r--r--   0     1001      127     8405 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/src/data/arithmetic_crystal_class.rs
--rw-r--r--   0     1001      127     7841 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/src/data/classification.rs
--rw-r--r--   0     1001      127    20576 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/src/data/hall_symbol.rs
--rw-r--r--   0     1001      127    81241 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/src/data/hall_symbol_database.rs
--rw-r--r--   0     1001      127     7762 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/src/data/point_group.rs
--rw-r--r--   0     1001      127     3370 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/src/data/setting.rs
--rw-r--r--   0     1001      127   201241 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/src/data/wyckoff.rs
--rw-r--r--   0     1001      127      740 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/src/data.rs
--rw-r--r--   0     1001      127    19605 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/src/identify/point_group.rs
--rw-r--r--   0     1001      127    13483 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/src/identify/space_group.rs
--rw-r--r--   0     1001      127       68 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/src/identify.rs
--rw-r--r--   0     1001      127     8765 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/src/lib.rs
--rw-r--r--   0     1001      127      901 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/src/math/cycle_checker.rs
--rw-r--r--   0     1001      127     5124 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/src/math/delaunay.rs
--rw-r--r--   0     1001      127     2284 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/src/math/elementary.rs
--rw-r--r--   0     1001      127     4148 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/src/math/hnf.rs
--rw-r--r--   0     1001      127     2440 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/src/math/integer_system.rs
--rw-r--r--   0     1001      127     7889 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/src/math/minkowski.rs
--rw-r--r--   0     1001      127    14588 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/src/math/niggli.rs
--rw-r--r--   0     1001      127     4889 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/src/math/snf.rs
--rw-r--r--   0     1001      127      344 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/src/math.rs
--rw-r--r--   0     1001      127    11991 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/src/search/primitive_cell.rs
--rw-r--r--   0     1001      127    12095 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/src/search/solve.rs
--rw-r--r--   0     1001      127    12714 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/src/search/symmetry_search.rs
--rw-r--r--   0     1001      127      250 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/src/search.rs
--rw-r--r--   0     1001      127    14886 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/src/symmetrize/standardize.rs
--rw-r--r--   0     1001      127       94 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/src/symmetrize.rs
--rw-r--r--   0     1001      127     5985 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/tests/assets/mp-1185639.json
--rw-r--r--   0     1001      127     5374 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/tests/assets/mp-1197586.json
--rw-r--r--   0     1001      127     9958 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/tests/assets/mp-1201492.json
--rw-r--r--   0     1001      127      820 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/tests/assets/mp-1221598.json
--rw-r--r--   0     1001      127      735 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/tests/assets/mp-1277787.json
--rw-r--r--   0     1001      127     3820 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/tests/assets/mp-30665.json
--rw-r--r--   0     1001      127     1370 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/tests/assets/mp-550745.json
--rw-r--r--   0     1001      127     5272 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/tests/assets/mp-569901.json
--rw-r--r--   0     1001      127    20173 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyo/tests/test_moyo_dataset.rs
--rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 moyopy-0.1.4/moyopy/Cargo.toml
--rw-r--r--   0     1001      127      315 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyopy/README.md
--rw-r--r--   0     1001      127       37 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyopy/python/moyopy/__init__.py
--rw-r--r--   0     1001      127     2504 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyopy/python/moyopy/_moyopy.pyi
--rw-r--r--   0     1001      127        0 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyopy/python/moyopy/py.typed
--rw-r--r--   0     1001      127      623 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyopy/python/tests/conftest.py
--rw-r--r--   0     1001      127      394 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyopy/python/tests/test_moyo_dataset.py
--rw-r--r--   0     1001      127     4934 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyopy/src/base.rs
--rw-r--r--   0     1001      127      704 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyopy/src/data.rs
--rw-r--r--   0     1001      127     4119 2024-04-21 02:15:24.000000 moyopy-0.1.4/moyopy/src/lib.rs
--rw-r--r--   0     1001      127    42754 2024-04-21 02:15:24.000000 moyopy-0.1.4/Cargo.lock
--rw-r--r--   0        0        0      583 1970-01-01 00:00:00.000000 moyopy-0.1.4/Cargo.toml
--rw-r--r--   0        0        0     1800 1970-01-01 00:00:00.000000 moyopy-0.1.4/pyproject.toml
--rw-r--r--   0     1001      127        0 2024-04-21 02:15:24.000000 moyopy-0.1.4/python/moyopy/py.typed
--rw-r--r--   0     1001      127       37 2024-04-21 02:15:24.000000 moyopy-0.1.4/python/moyopy/__init__.py
--rw-r--r--   0     1001      127     2504 2024-04-21 02:15:24.000000 moyopy-0.1.4/python/moyopy/_moyopy.pyi
--rw-r--r--   0     1001      127      315 2024-04-21 02:15:24.000000 moyopy-0.1.4/README.md
--rw-r--r--   0        0        0     1402 1970-01-01 00:00:00.000000 moyopy-0.1.4/PKG-INFO
+-rw-r--r--   0     1001      127      903 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/Cargo.toml
+-rw-r--r--   0     1001      127      245 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/README.md
+-rw-r--r--   0     1001      127      703 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/benches/dataset.rs
+-rw-r--r--   0     1001      127     2493 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/benches/translation_search.rs
+-rw-r--r--   0     1001      127     2926 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/src/base/cell.rs
+-rw-r--r--   0     1001      127     1123 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/src/base/error.rs
+-rw-r--r--   0     1001      127     2932 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/src/base/lattice.rs
+-rw-r--r--   0     1001      127     3830 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/src/base/operation.rs
+-rw-r--r--   0     1001      127     2146 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/src/base/tolerance.rs
+-rw-r--r--   0     1001      127     9891 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/src/base/transformation.rs
+-rw-r--r--   0     1001      127      559 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/src/base.rs
+-rw-r--r--   0     1001      127     8405 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/src/data/arithmetic_crystal_class.rs
+-rw-r--r--   0     1001      127     7841 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/src/data/classification.rs
+-rw-r--r--   0     1001      127    20576 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/src/data/hall_symbol.rs
+-rw-r--r--   0     1001      127    81241 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/src/data/hall_symbol_database.rs
+-rw-r--r--   0     1001      127     7762 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/src/data/point_group.rs
+-rw-r--r--   0     1001      127     3370 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/src/data/setting.rs
+-rw-r--r--   0     1001      127   201241 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/src/data/wyckoff.rs
+-rw-r--r--   0     1001      127      740 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/src/data.rs
+-rw-r--r--   0     1001      127    19605 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/src/identify/point_group.rs
+-rw-r--r--   0     1001      127    13483 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/src/identify/space_group.rs
+-rw-r--r--   0     1001      127       68 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/src/identify.rs
+-rw-r--r--   0     1001      127     8765 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/src/lib.rs
+-rw-r--r--   0     1001      127      901 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/src/math/cycle_checker.rs
+-rw-r--r--   0     1001      127     5124 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/src/math/delaunay.rs
+-rw-r--r--   0     1001      127     2284 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/src/math/elementary.rs
+-rw-r--r--   0     1001      127     4148 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/src/math/hnf.rs
+-rw-r--r--   0     1001      127     2440 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/src/math/integer_system.rs
+-rw-r--r--   0     1001      127     7889 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/src/math/minkowski.rs
+-rw-r--r--   0     1001      127    14588 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/src/math/niggli.rs
+-rw-r--r--   0     1001      127     4889 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/src/math/snf.rs
+-rw-r--r--   0     1001      127      344 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/src/math.rs
+-rw-r--r--   0     1001      127    11991 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/src/search/primitive_cell.rs
+-rw-r--r--   0     1001      127    12095 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/src/search/solve.rs
+-rw-r--r--   0     1001      127    12714 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/src/search/symmetry_search.rs
+-rw-r--r--   0     1001      127      250 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/src/search.rs
+-rw-r--r--   0     1001      127    14886 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/src/symmetrize/standardize.rs
+-rw-r--r--   0     1001      127       94 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/src/symmetrize.rs
+-rw-r--r--   0     1001      127     5985 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/tests/assets/mp-1185639.json
+-rw-r--r--   0     1001      127     5374 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/tests/assets/mp-1197586.json
+-rw-r--r--   0     1001      127     9958 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/tests/assets/mp-1201492.json
+-rw-r--r--   0     1001      127      820 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/tests/assets/mp-1221598.json
+-rw-r--r--   0     1001      127      735 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/tests/assets/mp-1277787.json
+-rw-r--r--   0     1001      127     3820 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/tests/assets/mp-30665.json
+-rw-r--r--   0     1001      127     1370 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/tests/assets/mp-550745.json
+-rw-r--r--   0     1001      127     5272 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/tests/assets/mp-569901.json
+-rw-r--r--   0     1001      127    20173 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyo/tests/test_moyo_dataset.rs
+-rw-r--r--   0        0        0      700 1970-01-01 00:00:00.000000 moyopy-0.1.6/moyopy/Cargo.toml
+-rw-r--r--   0     1001      127      315 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyopy/README.md
+-rw-r--r--   0     1001      127       37 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyopy/python/moyopy/__init__.py
+-rw-r--r--   0     1001      127     2504 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyopy/python/moyopy/_moyopy.pyi
+-rw-r--r--   0     1001      127        0 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyopy/python/moyopy/py.typed
+-rw-r--r--   0     1001      127      623 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyopy/python/tests/conftest.py
+-rw-r--r--   0     1001      127      394 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyopy/python/tests/test_moyo_dataset.py
+-rw-r--r--   0     1001      127     4934 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyopy/src/base.rs
+-rw-r--r--   0     1001      127      704 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyopy/src/data.rs
+-rw-r--r--   0     1001      127     4119 2024-04-24 12:04:04.000000 moyopy-0.1.6/moyopy/src/lib.rs
+-rw-r--r--   0     1001      127    42989 2024-04-24 12:04:04.000000 moyopy-0.1.6/Cargo.lock
+-rw-r--r--   0        0        0      583 1970-01-01 00:00:00.000000 moyopy-0.1.6/Cargo.toml
+-rw-r--r--   0        0        0     1800 1970-01-01 00:00:00.000000 moyopy-0.1.6/pyproject.toml
+-rw-r--r--   0     1001      127        0 2024-04-24 12:04:04.000000 moyopy-0.1.6/python/moyopy/py.typed
+-rw-r--r--   0     1001      127       37 2024-04-24 12:04:04.000000 moyopy-0.1.6/python/moyopy/__init__.py
+-rw-r--r--   0     1001      127     2504 2024-04-24 12:04:04.000000 moyopy-0.1.6/python/moyopy/_moyopy.pyi
+-rw-r--r--   0     1001      127      315 2024-04-24 12:04:04.000000 moyopy-0.1.6/README.md
+-rw-r--r--   0        0        0     1402 1970-01-01 00:00:00.000000 moyopy-0.1.6/PKG-INFO
```

### Comparing `moyopy-0.1.4/moyo/Cargo.toml` & `moyopy-0.1.6/moyo/Cargo.toml`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyo/benches/dataset.rs` & `moyopy-0.1.6/moyo/benches/dataset.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyo/benches/translation_search.rs` & `moyopy-0.1.6/moyo/benches/translation_search.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyo/src/base/cell.rs` & `moyopy-0.1.6/moyo/src/base/cell.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyo/src/base/error.rs` & `moyopy-0.1.6/moyo/src/base/error.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyo/src/base/lattice.rs` & `moyopy-0.1.6/moyo/src/base/lattice.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyo/src/base/operation.rs` & `moyopy-0.1.6/moyo/src/base/operation.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyo/src/base/tolerance.rs` & `moyopy-0.1.6/moyo/src/base/tolerance.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyo/src/base/transformation.rs` & `moyopy-0.1.6/moyo/src/base/transformation.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyo/src/base.rs` & `moyopy-0.1.6/moyo/src/base.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyo/src/data/arithmetic_crystal_class.rs` & `moyopy-0.1.6/moyo/src/data/arithmetic_crystal_class.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyo/src/data/classification.rs` & `moyopy-0.1.6/moyo/src/data/classification.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyo/src/data/hall_symbol.rs` & `moyopy-0.1.6/moyo/src/data/hall_symbol.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyo/src/data/hall_symbol_database.rs` & `moyopy-0.1.6/moyo/src/data/hall_symbol_database.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyo/src/data/point_group.rs` & `moyopy-0.1.6/moyo/src/data/point_group.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyo/src/data/setting.rs` & `moyopy-0.1.6/moyo/src/data/setting.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyo/src/data/wyckoff.rs` & `moyopy-0.1.6/moyo/src/data/wyckoff.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyo/src/data.rs` & `moyopy-0.1.6/moyo/src/data.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyo/src/identify/point_group.rs` & `moyopy-0.1.6/moyo/src/identify/point_group.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyo/src/identify/space_group.rs` & `moyopy-0.1.6/moyo/src/identify/space_group.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyo/src/lib.rs` & `moyopy-0.1.6/moyo/src/lib.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyo/src/math/cycle_checker.rs` & `moyopy-0.1.6/moyo/src/math/cycle_checker.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyo/src/math/delaunay.rs` & `moyopy-0.1.6/moyo/src/math/delaunay.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyo/src/math/elementary.rs` & `moyopy-0.1.6/moyo/src/math/elementary.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyo/src/math/hnf.rs` & `moyopy-0.1.6/moyo/src/math/hnf.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyo/src/math/integer_system.rs` & `moyopy-0.1.6/moyo/src/math/integer_system.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyo/src/math/minkowski.rs` & `moyopy-0.1.6/moyo/src/math/minkowski.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyo/src/math/niggli.rs` & `moyopy-0.1.6/moyo/src/math/niggli.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyo/src/math/snf.rs` & `moyopy-0.1.6/moyo/src/math/snf.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyo/src/search/primitive_cell.rs` & `moyopy-0.1.6/moyo/src/search/primitive_cell.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyo/src/search/solve.rs` & `moyopy-0.1.6/moyo/src/search/solve.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyo/src/search/symmetry_search.rs` & `moyopy-0.1.6/moyo/src/search/symmetry_search.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyo/src/symmetrize/standardize.rs` & `moyopy-0.1.6/moyo/src/symmetrize/standardize.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyo/tests/assets/mp-1185639.json` & `moyopy-0.1.6/moyo/tests/assets/mp-1185639.json`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyo/tests/assets/mp-1197586.json` & `moyopy-0.1.6/moyo/tests/assets/mp-1197586.json`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyo/tests/assets/mp-1201492.json` & `moyopy-0.1.6/moyo/tests/assets/mp-1201492.json`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyo/tests/assets/mp-1221598.json` & `moyopy-0.1.6/moyo/tests/assets/mp-1221598.json`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyo/tests/assets/mp-1277787.json` & `moyopy-0.1.6/moyo/tests/assets/mp-1277787.json`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyo/tests/assets/mp-30665.json` & `moyopy-0.1.6/moyo/tests/assets/mp-30665.json`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyo/tests/assets/mp-550745.json` & `moyopy-0.1.6/moyo/tests/assets/mp-550745.json`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyo/tests/assets/mp-569901.json` & `moyopy-0.1.6/moyo/tests/assets/mp-569901.json`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyo/tests/test_moyo_dataset.rs` & `moyopy-0.1.6/moyo/tests/test_moyo_dataset.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyopy/Cargo.toml` & `moyopy-0.1.6/moyopy/Cargo.toml`

 * *Files 13% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 description.workspace = true
 edition.workspace = true
 license.workspace = true
 repository.workspace = true
 version.workspace = true
 
 [package.metadata.release]
-release = false
+release = true
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "moyopy"
 crate-type = ["cdylib"]
 
 [dependencies]
-moyo = { path = "../moyo" }
+moyo = { path = "../moyo", version = "0.1.6" }
 nalgebra.workspace = true
 serde.workspace = true
 serde_json.workspace = true
 approx.workspace = true
 
 [dependencies.pyo3]
-version = "0.20.0"
+version = "0.20.3"
 # "abi3-py38" tells pyo3 (and maturin) to build using the stable ABI with minimum Python version 3.8
 features = ["abi3-py38"]
```

### Comparing `moyopy-0.1.4/moyopy/python/moyopy/_moyopy.pyi` & `moyopy-0.1.6/moyopy/python/moyopy/_moyopy.pyi`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyopy/python/tests/conftest.py` & `moyopy-0.1.6/moyopy/python/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyopy/src/base.rs` & `moyopy-0.1.6/moyopy/src/base.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyopy/src/data.rs` & `moyopy-0.1.6/moyopy/src/data.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/moyopy/src/lib.rs` & `moyopy-0.1.6/moyopy/src/lib.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/Cargo.lock` & `moyopy-0.1.6/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -101,17 +101,17 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bumpalo"
-version = "3.15.4"
+version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ff69b9dd49fd426c69a0db9fc04dd934cdb6645ff000864d98f7e2af8830eaa"
+checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
 [[package]]
 name = "bytemuck"
 version = "1.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5d6d68c57235a3a081186990eca2867354726650f42f7516ca50c28d6281fd15"
 
@@ -119,17 +119,17 @@
 name = "cast"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "37b2a672a2cb129a2e41c10b1224bb368f9f37a2b16b612598138befd7b37eb5"
 
 [[package]]
 name = "cc"
-version = "1.0.90"
+version = "1.0.95"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8cd6604a82acf3039f1144f54b8eb34e91ffba622051189e71b781822d5ee1f5"
+checksum = "d32a725bc159af97c3e629873bb9f88fb8cf8a4867175f76dc987815ea07c83b"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
@@ -264,17 +264,17 @@
 name = "doc-comment"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fea41bba32d969b513997752735605054bc0dfa92b4c56bf1189f2e174be7a10"
 
 [[package]]
 name = "either"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
+checksum = "a47c1c47d2f5964e29c61246e81db715514cd532db6b5116a25ea3c03d6780a2"
 
 [[package]]
 name = "elapsed"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6f4e5af126dafd0741c2ad62d47f68b28602550102e5f0dd45c8a97fc8b49c29"
 
@@ -366,15 +366,15 @@
 name = "futures-macro"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
@@ -420,34 +420,34 @@
  "log",
  "rustversion",
  "windows",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.13"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a06fddc2749e0528d2813f95e050e87e52c8cbbae56223b9babf73b3e53b0cc6"
+checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
 name = "glob"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
 
 [[package]]
 name = "half"
-version = "2.4.0"
+version = "2.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b5eceaaeec696539ddaf7b333340f1af35a5aa87ae3e4f3ead0532f72affab2e"
+checksum = "6dd08c532ae367adf81c312a4580bc67f1d0fe8bc9c460520283f4c0ff277888"
 dependencies = [
  "cfg-if",
  "crunchy",
 ]
 
 [[package]]
 name = "hashbrown"
@@ -614,15 +614,15 @@
 checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "moyo"
-version = "0.1.4"
+version = "0.1.6"
 dependencies = [
  "approx",
  "criterion",
  "env_logger",
  "itertools 0.11.0",
  "kiddo",
  "log",
@@ -636,15 +636,15 @@
  "test-log",
  "thiserror",
  "union-find",
 ]
 
 [[package]]
 name = "moyopy"
-version = "0.1.4"
+version = "0.1.6"
 dependencies = [
  "approx",
  "moyo",
  "nalgebra",
  "pyo3",
  "serde",
  "serde_json",
@@ -839,17 +839,17 @@
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.79"
+version = "1.0.81"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
+checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.20.3"
@@ -893,35 +893,35 @@
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.35"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -1043,32 +1043,32 @@
  "cfg-if",
  "glob",
  "proc-macro2",
  "quote",
  "regex",
  "relative-path",
  "rustc_version",
- "syn 2.0.58",
+ "syn 2.0.60",
  "unicode-ident",
 ]
 
 [[package]]
 name = "rustc_version"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustversion"
-version = "1.0.14"
+version = "1.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ffc183a10b4478d04cbbbfc96d0873219d962dd5accaff2ffbd4ceb7df837f4"
+checksum = "80af6f9131f277a45a3fba6ce8e2258037bb0477a67e610d3c1fe046ab31de47"
 
 [[package]]
 name = "ryu"
 version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
 
@@ -1100,37 +1100,37 @@
 name = "semver"
 version = "1.0.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "92d43fe69e652f3df9bdc2b85b2854a0825b86e4fb76bc44d945137d053639ca"
 
 [[package]]
 name = "serde"
-version = "1.0.197"
+version = "1.0.198"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
+checksum = "9846a40c979031340571da2545a4e5b7c4163bdae79b301d5f86d03979451fcc"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.197"
+version = "1.0.198"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
+checksum = "e88edab869b01783ba905e7d0153f9fc1a6505a96e4ad3018011eedb838566d9"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.115"
+version = "1.0.116"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
+checksum = "3e17db7126d17feb94eb3fad46bf1a96b034e8aacbc2e775fe81505f8b0b2813"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -1188,15 +1188,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "23dc1fa9ac9c169a78ba62f0b841814b7abae11bdd047b9c58f893439e309ea0"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
  "rustversion",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
@@ -1204,17 +1204,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.58"
+version = "2.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44cfb93f38070beee36b3fef7d4f5a16f27751d94b187b666a5cc5e9b0d30687"
+checksum = "909518bc7b1c9b779f1bbf07f2929d35af9f0f37e47c6e9ef7f9dddc1e1821f3"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -1237,41 +1237,41 @@
 name = "test-log-macros"
 version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c8f546451eaa38373f549093fe9fd05e7d2bade739e2ddf834b9968621d60107"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "textwrap"
 version = "0.16.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "23d434d3f8967a09480fb04132ebe0a3e088c173e6d0ee7897abbdf4eab0f8b9"
 
 [[package]]
 name = "thiserror"
-version = "1.0.58"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
+checksum = "f0126ad08bff79f29fc3ae6a55cc72352056dfff61e3ff8bb7129476d44b23aa"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.58"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
+checksum = "d1cd413b5d558b4c5bf3680e324a6fa5014e7b7c067a51e69dbdf47eb7148b66"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "thread_local"
 version = "1.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b9ef9bad013ada3808854ceac7b46812a6465ba368859a37e2100283d2d719c"
@@ -1305,15 +1305,15 @@
 name = "tracing-attributes"
 version = "0.1.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "34704c8d6ebcbc939824180af020566b01a7c01f80641264eba0999f6c2b6be7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c06d3da6113f116aaee68e4d601191614c9053067f9ab7f6edbcb161237daa54"
@@ -1422,15 +1422,15 @@
 checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1444,15 +1444,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.92"
@@ -1467,17 +1467,17 @@
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "wide"
-version = "0.7.15"
+version = "0.7.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "89beec544f246e679fc25490e3f8e08003bc4bf612068f325120dad4cea02c1c"
+checksum = "81a1851a719f11d1d2fea40e15c72f6c00de8c142d7ac47c1441cc7e4d0d5bc6"
 dependencies = [
  "bytemuck",
  "safe_arch",
 ]
 
 [[package]]
 name = "winapi"
@@ -1493,19 +1493,19 @@
 name = "winapi-i686-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
 
 [[package]]
 name = "winapi-util"
-version = "0.1.6"
+version = "0.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f29e6f9198ba0d26b4c9f07dbe6f9ed633e1f3d5b8b414090084349e46a52596"
+checksum = "134306a13c5647ad6453e8deaec55d3a44d6021970129e6188735e74bf546697"
 dependencies = [
- "winapi",
+ "windows-sys",
 ]
 
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
@@ -1521,15 +1521,15 @@
 
 [[package]]
 name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
@@ -1541,103 +1541,110 @@
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7dd37b7e5ab9018759f893a1952c9420d060016fc19a472b4bb20d1bdd694d1b"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.4",
- "windows_aarch64_msvc 0.52.4",
- "windows_i686_gnu 0.52.4",
- "windows_i686_msvc 0.52.4",
- "windows_x86_64_gnu 0.52.4",
- "windows_x86_64_gnullvm 0.52.4",
- "windows_x86_64_msvc 0.52.4",
+ "windows_aarch64_gnullvm 0.52.5",
+ "windows_aarch64_msvc 0.52.5",
+ "windows_i686_gnu 0.52.5",
+ "windows_i686_gnullvm",
+ "windows_i686_msvc 0.52.5",
+ "windows_x86_64_gnu 0.52.5",
+ "windows_x86_64_gnullvm 0.52.5",
+ "windows_x86_64_msvc 0.52.5",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bcf46cf4c365c6f2d1cc93ce535f2c8b244591df96ceee75d8e83deb70a9cac9"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da9f259dd3bcf6990b55bffd094c4f7235817ba4ceebde8e6d11cd0c5633b675"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.4"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b474d8268f99e0995f25b9f095bc7434632601028cf86590aea5c8a5cb7801d3"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1515e9a29e5bed743cb4415a9ecf5dfca648ce85ee42e15873c3cd8610ff8e02"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5eee091590e89cc02ad514ffe3ead9eb6b660aedca2183455434b93546371a03"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77ca79f2451b49fa9e2af39f0747fe999fcda4f5e241b2898624dca97a1f2177"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32b752e52a2da0ddfbdbcc6fceadfeede4c939ed16d13e648833a61dfb611ed8"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
```

### Comparing `moyopy-0.1.4/Cargo.toml` & `moyopy-0.1.6/Cargo.toml`

 * *Files 18% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 
 resolver = "2"
 
 [workspace.package]
 authors = ["Kohei Shinohara <kshinohara0508@gmail.com>"]
 description = "Library for Crystal Symmetry in Rust"
 edition = "2021"
-version = "0.1.4"
+version = "0.1.6"
 license = "MIT OR Apache-2.0"
 repository = "https://github.com/spglib/moyo"
 
 [workspace.dependencies]
-nalgebra = { version = "0.32.3", features = ["serde-serialize"] }
+nalgebra = { version = "0.32.5", features = ["serde-serialize"] }
 serde = { version = "1.0", features = ["derive"] }
 serde_json = "1.0"
 approx = "0.5.1"
 
 [workspace.metadata.release]
 allow-branch = ["main"]
 shared-version = true
```

### Comparing `moyopy-0.1.4/pyproject.toml` & `moyopy-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/python/moyopy/_moyopy.pyi` & `moyopy-0.1.6/python/moyopy/_moyopy.pyi`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.4/PKG-INFO` & `moyopy-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: moyopy
-Version: 0.1.4
+Version: 0.1.6
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

