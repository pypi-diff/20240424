# Comparing `tmp/neuromorphic_drivers-0.8.3.tar.gz` & `tmp/neuromorphic_drivers-0.9.0.tar.gz`

## Comparing `neuromorphic_drivers-0.8.3.tar` & `neuromorphic_drivers-0.9.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0      489 1970-01-01 00:00:00.000000 neuromorphic_drivers-0.8.3/local_dependencies/reflect/Cargo.toml
--rw-r--r--   0     1001      127    18887 2023-09-29 23:19:59.000000 neuromorphic_drivers-0.8.3/local_dependencies/reflect/src/de.rs
--rw-r--r--   0     1001      127     5021 2023-09-29 23:19:59.000000 neuromorphic_drivers-0.8.3/local_dependencies/reflect/src/error.rs
--rw-r--r--   0     1001      127    25754 2023-09-29 23:19:59.000000 neuromorphic_drivers-0.8.3/local_dependencies/reflect/src/format.rs
--rw-r--r--   0     1001      127    14340 2023-09-29 23:19:59.000000 neuromorphic_drivers-0.8.3/local_dependencies/reflect/src/lib.rs
--rw-r--r--   0     1001      127    14435 2023-09-29 23:19:59.000000 neuromorphic_drivers-0.8.3/local_dependencies/reflect/src/ser.rs
--rw-r--r--   0     1001      127    11374 2023-09-29 23:19:59.000000 neuromorphic_drivers-0.8.3/local_dependencies/reflect/src/trace.rs
--rw-r--r--   0     1001      127    10825 2023-09-29 23:19:59.000000 neuromorphic_drivers-0.8.3/local_dependencies/reflect/src/value.rs
--rw-r--r--   0        0        0      540 1970-01-01 00:00:00.000000 neuromorphic_drivers-0.8.3/Cargo.toml
--rw-r--r--   0     1001      127       77 2023-09-29 23:19:59.000000 neuromorphic_drivers-0.8.3/.gitignore
--rw-r--r--   0     1001      127     1102 2023-09-29 23:19:59.000000 neuromorphic_drivers-0.8.3/LICENSE
--rw-r--r--   0     1001      127      115 2023-09-29 23:19:59.000000 neuromorphic_drivers-0.8.3/README.md
--rw-r--r--   0     1001      127    37979 2023-09-29 23:19:59.000000 neuromorphic_drivers-0.8.3/build.rs
--rw-r--r--   0     1001      127     6193 2023-09-29 23:19:59.000000 neuromorphic_drivers-0.8.3/examples/any_display.py
--rw-r--r--   0     1001      127      608 2023-09-29 23:19:59.000000 neuromorphic_drivers-0.8.3/examples/any_read_many.py
--rw-r--r--   0     1001      127      336 2023-09-29 23:19:59.000000 neuromorphic_drivers-0.8.3/examples/any_read_one.py
--rw-r--r--   0     1001      127      687 2023-09-29 23:19:59.000000 neuromorphic_drivers-0.8.3/examples/any_record_raw.py
--rw-r--r--   0     1001      127     8100 2023-09-29 23:19:59.000000 neuromorphic_drivers-0.8.3/examples/evk4_dual_display.py
--rw-r--r--   0     1001      127     1961 2023-09-29 23:19:59.000000 neuromorphic_drivers-0.8.3/examples/evk4_external_synchronization.py
--rw-r--r--   0     1001      127     1439 2023-09-29 23:19:59.000000 neuromorphic_drivers-0.8.3/examples/evk4_mask.py
--rw-r--r--   0     1001      127     3479 2023-09-29 23:19:59.000000 neuromorphic_drivers-0.8.3/examples/evk4_plot_hot_pixels.py
--rw-r--r--   0     1001      127      901 2023-09-29 23:19:59.000000 neuromorphic_drivers-0.8.3/examples/evk4_update_biases.py
--rw-r--r--   0     1001      127     1087 2023-09-29 23:19:59.000000 neuromorphic_drivers-0.8.3/pyproject.toml
--rw-r--r--   0     1001      127     2765 2023-09-29 23:19:59.000000 neuromorphic_drivers-0.8.3/python/neuromorphic_drivers/__init__.py
--rw-r--r--   0     1001      127     1194 2023-09-29 23:19:59.000000 neuromorphic_drivers-0.8.3/python/neuromorphic_drivers/device.py
--rw-r--r--   0     1001      127     6389 2023-09-29 23:19:59.000000 neuromorphic_drivers-0.8.3/python/neuromorphic_drivers/generated/devices/prophesee_evk3_hd.py
--rw-r--r--   0     1001      127     7444 2023-09-29 23:19:59.000000 neuromorphic_drivers-0.8.3/python/neuromorphic_drivers/generated/devices/prophesee_evk4.py
--rw-r--r--   0     1001      127     8877 2023-09-29 23:19:59.000000 neuromorphic_drivers-0.8.3/python/neuromorphic_drivers/generated/devices_types.py
--rw-r--r--   0     1001      127      400 2023-09-29 23:19:59.000000 neuromorphic_drivers-0.8.3/python/neuromorphic_drivers/generated/enums.py
--rw-r--r--   0     1001      127     1097 2023-09-29 23:19:59.000000 neuromorphic_drivers-0.8.3/python/neuromorphic_drivers/generated/unions.py
--rw-r--r--   0     1001      127     6788 2023-09-29 23:19:59.000000 neuromorphic_drivers-0.8.3/python/neuromorphic_drivers/mask.py
--rw-r--r--   0     1001      127       91 2023-09-29 23:19:59.000000 neuromorphic_drivers-0.8.3/python/neuromorphic_drivers/serde/__init__.py
--rw-r--r--   0     1001      127    15926 2023-09-29 23:19:59.000000 neuromorphic_drivers-0.8.3/python/neuromorphic_drivers/serde/binary.py
--rw-r--r--   0     1001      127     2328 2023-09-29 23:19:59.000000 neuromorphic_drivers-0.8.3/python/neuromorphic_drivers/serde/bincode.py
--rw-r--r--   0     1001      127     1547 2023-09-29 23:19:59.000000 neuromorphic_drivers-0.8.3/python/neuromorphic_drivers/serde/type.py
--rw-r--r--   0     1001      127     1127 2023-09-29 23:19:59.000000 neuromorphic_drivers-0.8.3/python/neuromorphic_drivers/status.py
--rw-r--r--   0     1001      127     3034 2023-09-29 23:19:59.000000 neuromorphic_drivers-0.8.3/python/neuromorphic_drivers/udev.py
--rw-r--r--   0     1001      127     4497 2023-09-29 23:19:59.000000 neuromorphic_drivers-0.8.3/src/adapters.rs
--rw-r--r--   0     1001      127     1675 2023-09-29 23:19:59.000000 neuromorphic_drivers-0.8.3/src/bytes.rs
--rw-r--r--   0     1001      127    14453 2023-09-29 23:19:59.000000 neuromorphic_drivers-0.8.3/src/lib.rs
--rw-r--r--   0     1001      127     4091 2023-09-29 23:19:59.000000 neuromorphic_drivers-0.8.3/src/structured_array.rs
--rw-r--r--   0     1001      127    21276 2023-09-29 23:20:11.000000 neuromorphic_drivers-0.8.3/Cargo.lock
--rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 neuromorphic_drivers-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0      489 1970-01-01 00:00:00.000000 neuromorphic_drivers-0.9.0/local_dependencies/reflect/Cargo.toml
+-rw-r--r--   0     1001      127    18887 2023-11-06 05:30:03.000000 neuromorphic_drivers-0.9.0/local_dependencies/reflect/src/de.rs
+-rw-r--r--   0     1001      127     5021 2023-11-06 05:30:03.000000 neuromorphic_drivers-0.9.0/local_dependencies/reflect/src/error.rs
+-rw-r--r--   0     1001      127    25754 2023-11-06 05:30:03.000000 neuromorphic_drivers-0.9.0/local_dependencies/reflect/src/format.rs
+-rw-r--r--   0     1001      127    14340 2023-11-06 05:30:03.000000 neuromorphic_drivers-0.9.0/local_dependencies/reflect/src/lib.rs
+-rw-r--r--   0     1001      127    14435 2023-11-06 05:30:03.000000 neuromorphic_drivers-0.9.0/local_dependencies/reflect/src/ser.rs
+-rw-r--r--   0     1001      127    11374 2023-11-06 05:30:03.000000 neuromorphic_drivers-0.9.0/local_dependencies/reflect/src/trace.rs
+-rw-r--r--   0     1001      127    10825 2023-11-06 05:30:03.000000 neuromorphic_drivers-0.9.0/local_dependencies/reflect/src/value.rs
+-rw-r--r--   0        0        0      540 1970-01-01 00:00:00.000000 neuromorphic_drivers-0.9.0/Cargo.toml
+-rw-r--r--   0     1001      127       77 2023-11-06 05:30:03.000000 neuromorphic_drivers-0.9.0/.gitignore
+-rw-r--r--   0     1001      127     1102 2023-11-06 05:30:03.000000 neuromorphic_drivers-0.9.0/LICENSE
+-rw-r--r--   0     1001      127      115 2023-11-06 05:30:03.000000 neuromorphic_drivers-0.9.0/README.md
+-rw-r--r--   0     1001      127    37979 2023-11-06 05:30:03.000000 neuromorphic_drivers-0.9.0/build.rs
+-rw-r--r--   0     1001      127     6193 2023-11-06 05:30:03.000000 neuromorphic_drivers-0.9.0/examples/any_display.py
+-rw-r--r--   0     1001      127      608 2023-11-06 05:30:03.000000 neuromorphic_drivers-0.9.0/examples/any_read_many.py
+-rw-r--r--   0     1001      127      336 2023-11-06 05:30:03.000000 neuromorphic_drivers-0.9.0/examples/any_read_one.py
+-rw-r--r--   0     1001      127      687 2023-11-06 05:30:03.000000 neuromorphic_drivers-0.9.0/examples/any_record_raw.py
+-rw-r--r--   0     1001      127     8100 2023-11-06 05:30:03.000000 neuromorphic_drivers-0.9.0/examples/evk4_dual_display.py
+-rw-r--r--   0     1001      127     1961 2023-11-06 05:30:03.000000 neuromorphic_drivers-0.9.0/examples/evk4_external_synchronization.py
+-rw-r--r--   0     1001      127     1439 2023-11-06 05:30:03.000000 neuromorphic_drivers-0.9.0/examples/evk4_mask.py
+-rw-r--r--   0     1001      127     3479 2023-11-06 05:30:03.000000 neuromorphic_drivers-0.9.0/examples/evk4_plot_hot_pixels.py
+-rw-r--r--   0     1001      127      901 2023-11-06 05:30:03.000000 neuromorphic_drivers-0.9.0/examples/evk4_update_biases.py
+-rw-r--r--   0     1001      127     1088 2023-11-06 05:30:03.000000 neuromorphic_drivers-0.9.0/pyproject.toml
+-rw-r--r--   0     1001      127     2765 2023-11-06 05:30:03.000000 neuromorphic_drivers-0.9.0/python/neuromorphic_drivers/__init__.py
+-rw-r--r--   0     1001      127     1194 2023-11-06 05:30:03.000000 neuromorphic_drivers-0.9.0/python/neuromorphic_drivers/device.py
+-rw-r--r--   0     1001      127     6389 2023-11-06 05:30:03.000000 neuromorphic_drivers-0.9.0/python/neuromorphic_drivers/generated/devices/prophesee_evk3_hd.py
+-rw-r--r--   0     1001      127     7444 2023-11-06 05:30:03.000000 neuromorphic_drivers-0.9.0/python/neuromorphic_drivers/generated/devices/prophesee_evk4.py
+-rw-r--r--   0     1001      127     8877 2023-11-06 05:30:03.000000 neuromorphic_drivers-0.9.0/python/neuromorphic_drivers/generated/devices_types.py
+-rw-r--r--   0     1001      127      400 2023-11-06 05:30:03.000000 neuromorphic_drivers-0.9.0/python/neuromorphic_drivers/generated/enums.py
+-rw-r--r--   0     1001      127     1097 2023-11-06 05:30:03.000000 neuromorphic_drivers-0.9.0/python/neuromorphic_drivers/generated/unions.py
+-rw-r--r--   0     1001      127     6788 2023-11-06 05:30:03.000000 neuromorphic_drivers-0.9.0/python/neuromorphic_drivers/mask.py
+-rw-r--r--   0     1001      127       91 2023-11-06 05:30:03.000000 neuromorphic_drivers-0.9.0/python/neuromorphic_drivers/serde/__init__.py
+-rw-r--r--   0     1001      127    15926 2023-11-06 05:30:03.000000 neuromorphic_drivers-0.9.0/python/neuromorphic_drivers/serde/binary.py
+-rw-r--r--   0     1001      127     2328 2023-11-06 05:30:03.000000 neuromorphic_drivers-0.9.0/python/neuromorphic_drivers/serde/bincode.py
+-rw-r--r--   0     1001      127     1547 2023-11-06 05:30:03.000000 neuromorphic_drivers-0.9.0/python/neuromorphic_drivers/serde/type.py
+-rw-r--r--   0     1001      127     1127 2023-11-06 05:30:03.000000 neuromorphic_drivers-0.9.0/python/neuromorphic_drivers/status.py
+-rw-r--r--   0     1001      127     3034 2023-11-06 05:30:03.000000 neuromorphic_drivers-0.9.0/python/neuromorphic_drivers/udev.py
+-rw-r--r--   0     1001      127     4497 2023-11-06 05:30:03.000000 neuromorphic_drivers-0.9.0/src/adapters.rs
+-rw-r--r--   0     1001      127     1675 2023-11-06 05:30:03.000000 neuromorphic_drivers-0.9.0/src/bytes.rs
+-rw-r--r--   0     1001      127    14453 2023-11-06 05:30:03.000000 neuromorphic_drivers-0.9.0/src/lib.rs
+-rw-r--r--   0     1001      127     4091 2023-11-06 05:30:03.000000 neuromorphic_drivers-0.9.0/src/structured_array.rs
+-rw-r--r--   0     1001      127    21276 2023-11-06 05:30:17.000000 neuromorphic_drivers-0.9.0/Cargo.lock
+-rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 neuromorphic_drivers-0.9.0/PKG-INFO
```

### Comparing `neuromorphic_drivers-0.8.3/local_dependencies/reflect/src/de.rs` & `neuromorphic_drivers-0.9.0/local_dependencies/reflect/src/de.rs`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.8.3/local_dependencies/reflect/src/error.rs` & `neuromorphic_drivers-0.9.0/local_dependencies/reflect/src/error.rs`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.8.3/local_dependencies/reflect/src/format.rs` & `neuromorphic_drivers-0.9.0/local_dependencies/reflect/src/format.rs`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.8.3/local_dependencies/reflect/src/lib.rs` & `neuromorphic_drivers-0.9.0/local_dependencies/reflect/src/lib.rs`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.8.3/local_dependencies/reflect/src/ser.rs` & `neuromorphic_drivers-0.9.0/local_dependencies/reflect/src/ser.rs`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.8.3/local_dependencies/reflect/src/trace.rs` & `neuromorphic_drivers-0.9.0/local_dependencies/reflect/src/trace.rs`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.8.3/local_dependencies/reflect/src/value.rs` & `neuromorphic_drivers-0.9.0/local_dependencies/reflect/src/value.rs`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.8.3/Cargo.toml` & `neuromorphic_drivers-0.9.0/Cargo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [package]
 name = "python"
-version = "0.8.3"
+version = "0.9.0"
 edition = "2021"
 resolver = "2"
 
 [lib]
 name = "neuromorphic_drivers"
 crate-type = ["cdylib"]
 
 [dependencies]
-neuromorphic-drivers = "0.8.0"
+neuromorphic-drivers = "0.9.0"
 numpy = "0.19"
 paste = "1.0"
 pyo3 = {version = "0.19", features = ["extension-module"]}
 
 [build-dependencies]
 cc = "1.0"
-neuromorphic-drivers = "0.8.0"
+neuromorphic-drivers = "0.9.0"
 paste = "1.0"
 reflect = {path = "local_dependencies/reflect" }
 serde = {version = "1.0", features = ["derive"]}
 serde_json = "1.0"
 serde-generate = "0.25.1"
 toml = {version = "0.7", features = ["parse"]}
```

### Comparing `neuromorphic_drivers-0.8.3/LICENSE` & `neuromorphic_drivers-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.8.3/build.rs` & `neuromorphic_drivers-0.9.0/build.rs`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.8.3/examples/any_display.py` & `neuromorphic_drivers-0.9.0/examples/any_display.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.8.3/examples/any_read_many.py` & `neuromorphic_drivers-0.9.0/examples/any_read_many.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.8.3/examples/any_record_raw.py` & `neuromorphic_drivers-0.9.0/examples/any_record_raw.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.8.3/examples/evk4_dual_display.py` & `neuromorphic_drivers-0.9.0/examples/evk4_dual_display.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.8.3/examples/evk4_external_synchronization.py` & `neuromorphic_drivers-0.9.0/examples/evk4_external_synchronization.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.8.3/examples/evk4_mask.py` & `neuromorphic_drivers-0.9.0/examples/evk4_mask.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.8.3/examples/evk4_plot_hot_pixels.py` & `neuromorphic_drivers-0.9.0/examples/evk4_plot_hot_pixels.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.8.3/examples/evk4_update_biases.py` & `neuromorphic_drivers-0.9.0/examples/evk4_update_biases.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.8.3/pyproject.toml` & `neuromorphic_drivers-0.9.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 description = "Neuromorphic devices drivers"
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [
     {name = "International Centre for Neuromorphic Systems"},
     {name = "Alexandre Marcireau"},
 ]
-version = "0.8.3"
+version = "0.9.0"
 requires-python = ">=3.8"
 dependencies = ["numpy>=1.24"]
 
 [project.urls]
 homepage = "https://github.com/neuromorphicsystems/neuromorphic-rs/"
 repository = "https://github.com/neuromorphicsystems/neuromorphic-rs/"
 documentation = "https://github.com/neuromorphicsystems/neuromorphic-rs/"
 
 [build-system]
-requires = ["maturin>=0.12", "numpy"]
+requires = ["maturin==1.2.3", "numpy"]
 build-backend = "maturin"
 
 [tool.maturin]
 python-source = "python"
 
 [tool.black]
 extend-exclude = "python/neuromorphic_drivers/generated"
```

### Comparing `neuromorphic_drivers-0.8.3/python/neuromorphic_drivers/__init__.py` & `neuromorphic_drivers-0.9.0/python/neuromorphic_drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.8.3/python/neuromorphic_drivers/device.py` & `neuromorphic_drivers-0.9.0/python/neuromorphic_drivers/device.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.8.3/python/neuromorphic_drivers/generated/devices/prophesee_evk3_hd.py` & `neuromorphic_drivers-0.9.0/python/neuromorphic_drivers/generated/devices/prophesee_evk3_hd.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.8.3/python/neuromorphic_drivers/generated/devices/prophesee_evk4.py` & `neuromorphic_drivers-0.9.0/python/neuromorphic_drivers/generated/devices/prophesee_evk4.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.8.3/python/neuromorphic_drivers/generated/devices_types.py` & `neuromorphic_drivers-0.9.0/python/neuromorphic_drivers/generated/devices_types.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.8.3/python/neuromorphic_drivers/generated/unions.py` & `neuromorphic_drivers-0.9.0/python/neuromorphic_drivers/generated/unions.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.8.3/python/neuromorphic_drivers/mask.py` & `neuromorphic_drivers-0.9.0/python/neuromorphic_drivers/mask.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.8.3/python/neuromorphic_drivers/serde/binary.py` & `neuromorphic_drivers-0.9.0/python/neuromorphic_drivers/serde/binary.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.8.3/python/neuromorphic_drivers/serde/bincode.py` & `neuromorphic_drivers-0.9.0/python/neuromorphic_drivers/serde/bincode.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.8.3/python/neuromorphic_drivers/serde/type.py` & `neuromorphic_drivers-0.9.0/python/neuromorphic_drivers/serde/type.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.8.3/python/neuromorphic_drivers/status.py` & `neuromorphic_drivers-0.9.0/python/neuromorphic_drivers/status.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.8.3/python/neuromorphic_drivers/udev.py` & `neuromorphic_drivers-0.9.0/python/neuromorphic_drivers/udev.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.8.3/src/adapters.rs` & `neuromorphic_drivers-0.9.0/src/adapters.rs`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.8.3/src/bytes.rs` & `neuromorphic_drivers-0.9.0/src/bytes.rs`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.8.3/src/lib.rs` & `neuromorphic_drivers-0.9.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.8.3/src/structured_array.rs` & `neuromorphic_drivers-0.9.0/src/structured_array.rs`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.8.3/Cargo.lock` & `neuromorphic_drivers-0.9.0/Cargo.lock`

 * *Files 5% similar despite different names*

```diff
@@ -65,17 +65,17 @@
 name = "glob"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
 
 [[package]]
 name = "hashbrown"
-version = "0.14.1"
+version = "0.14.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7dfda62a12f55daeae5015f81b0baea145391cb4520f86c248fc615d72640d12"
+checksum = "f93e7192158dbcda357bdec5fb5788eebf8bbac027f3f33e719d29135ae84156"
 
 [[package]]
 name = "heck"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6d621efb26863f0e9924c6ac577e8275e5e6b77455db64ffa6c65c904e9e132c"
 dependencies = [
@@ -104,17 +104,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "indexmap"
-version = "2.0.2"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8adf3ddd720272c6ea8bf59463c04e0f93d0bbf7c5439b691bca2987e0270897"
+checksum = "d530e1a18b1cb4c484e6e34556a0d948706958449fca0cab753d649f2bce3d1f"
 dependencies = [
  "equivalent",
  "hashbrown",
 ]
 
 [[package]]
 name = "indoc"
@@ -126,17 +126,17 @@
 name = "itoa"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "af150ab688ff2122fcef229be89cb50dd66af9e01a4ff320cc137eecc9bacc38"
 
 [[package]]
 name = "libc"
-version = "0.2.148"
+version = "0.2.150"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9cdc71e17332e86d2e1d38c1f99edcb6288ee11b815fb1a4b049eaa2114d369b"
+checksum = "89d92a4743f9a61002fae18374ed11e7973f530cb3a3255fb354818118b2203c"
 
 [[package]]
 name = "libusb1-sys"
 version = "0.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9d0e2afce4245f2c9a418511e5af8718bcaf2fa408aefb259504d1a9cb25f27"
 dependencies = [
@@ -144,17 +144,17 @@
  "libc",
  "pkg-config",
  "vcpkg",
 ]
 
 [[package]]
 name = "lock_api"
-version = "0.4.10"
+version = "0.4.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
+checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "matrixmultiply"
@@ -164,17 +164,17 @@
 dependencies = [
  "autocfg",
  "rawpointer",
 ]
 
 [[package]]
 name = "memchr"
-version = "2.6.3"
+version = "2.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f232d6ef707e1956a43342693d2a31e72989554d58299d7a88738cc95b0d35c"
+checksum = "f665ee40bc4a3c5590afb1e9677db74a508659dfd71e126420da8274909a0167"
 
 [[package]]
 name = "memoffset"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
@@ -192,31 +192,31 @@
  "num-integer",
  "num-traits",
  "rawpointer",
 ]
 
 [[package]]
 name = "neuromorphic-drivers"
-version = "0.8.0"
+version = "0.9.0"
 dependencies = [
  "bincode",
  "libc",
  "libusb1-sys",
  "neuromorphic-types 0.4.0 (registry+https://github.com/rust-lang/crates.io-index)",
  "paste",
  "rusb",
  "serde",
  "thiserror",
 ]
 
 [[package]]
 name = "neuromorphic-drivers"
-version = "0.8.0"
+version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e33cd130daed96bbbf2f4c6c71ff62d6ced472f55899e23d97b7d3bc927fa5d4"
+checksum = "3539fcb743de175412c8e1c173f72cde7ea0ac49848017baafbf681f2ab3d3a8"
 dependencies = [
  "bincode",
  "libc",
  "libusb1-sys",
  "neuromorphic-types 0.4.0 (registry+https://github.com/rust-lang/crates.io-index)",
  "paste",
  "rusb",
@@ -251,17 +251,17 @@
 dependencies = [
  "autocfg",
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.16"
+version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f30b0abd723be7e2ffca1272140fac1a2f084c77ec3e123c192b66af1ee9e6c2"
+checksum = "39e3200413f237f41ab11ad6d161bc7239c84dcb631773ccd7de3dfe4b5c267c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "numpy"
 version = "0.19.0"
@@ -291,17 +291,17 @@
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.8"
+version = "0.9.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
+checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
  "windows-targets",
 ]
@@ -372,17 +372,17 @@
 name = "proc-macro-hack"
 version = "0.5.20+deprecated"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc375e1527247fe1a97d8b7156678dfe7c1af2fc075c9a4db3690ecd2a148068"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.67"
+version = "1.0.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d433d9f1a3e8c1263d9456598b16fec66f4acc9a74dacffd35c7bb09b3a1328"
+checksum = "134c189feb4956b20f6f547d2cf727d4c0fe06722b20a0eec87ed445a97f92da"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.19.2"
@@ -441,18 +441,18 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "python"
-version = "0.8.3"
+version = "0.9.0"
 dependencies = [
  "cc",
- "neuromorphic-drivers 0.8.0 (registry+https://github.com/rust-lang/crates.io-index)",
+ "neuromorphic-drivers 0.9.0 (registry+https://github.com/rust-lang/crates.io-index)",
  "numpy",
  "paste",
  "pyo3",
  "reflect",
  "serde",
  "serde-generate",
  "serde_json",
@@ -502,17 +502,17 @@
 name = "rawpointer"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "60a357793950651c4ed0f3f52338f53b2f809f32d83a07f72909fa13e4c6c1e3"
 
 [[package]]
 name = "redox_syscall"
-version = "0.3.5"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
+checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "reflect"
 version = "0.1.0"
@@ -548,17 +548,17 @@
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "serde"
-version = "1.0.188"
+version = "1.0.190"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cf9e0fcba69a370eed61bcf2b728575f726b50b55cba78064753d708ddc7549e"
+checksum = "91d3c334ca1ee894a2c6f6ad698fe8c435b76d504b13d436f0685d648d6d96f7"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde-generate"
 version = "0.25.1"
@@ -582,39 +582,39 @@
  "once_cell",
  "serde",
  "thiserror",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.188"
+version = "1.0.190"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4eca7ac642d82aa35b60049a6eccb4be6be75e599bd2e9adb5f875a737654af2"
+checksum = "67c5609f394e5c2bd7fc51efda478004ea80ef42fee983d5c67a65e34f32c0e3"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.37",
+ "syn 2.0.39",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.107"
+version = "1.0.108"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6b420ce6e3d8bd882e9b243c6eed35dbc9a6110c9769e74b584e0d68d1f20c65"
+checksum = "3d1c7e3eac408d115102c4c24ad393e0821bb3a5df4d506a80f85f7a742a526b"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "serde_spanned"
-version = "0.6.3"
+version = "0.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "96426c9936fd7a0124915f9185ea1d20aa9445cc9821142f0a73bc9207a2e186"
+checksum = "12022b835073e5b11e90a14f86838ceb1c8fb0325b72416845c487ac0fa95e80"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "siphasher"
 version = "0.3.11"
@@ -642,57 +642,57 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.37"
+version = "2.0.39"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7303ef2c05cd654186cb250d29049a24840ca25d2747c25c0381c8d9e2f582e8"
+checksum = "23e78b90f2fcf45d3e842032ce32e3f2d1545ba6636271dcbf24fa306d87be7a"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.11"
+version = "0.12.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9d0e916b1148c8e263850e1ebcbd046f333e0683c724876bb0da63ea4373dc8a"
+checksum = "14c39fd04924ca3a864207c66fc2cd7d22d7c016007f9ce846cbb9326331930a"
 
 [[package]]
 name = "textwrap"
 version = "0.13.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cd05616119e612a8041ef58f2b578906cc2531a6069047ae092cfb86a325d835"
 dependencies = [
  "smawk",
  "unicode-width",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.49"
+version = "1.0.50"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1177e8c6d7ede7afde3585fd2513e611227efd6481bd78d2e82ba1ce16557ed4"
+checksum = "f9a7210f5c9a7156bb50aa36aed4c95afb51df0df00713949448cf9e97d382d2"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.49"
+version = "1.0.50"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "10712f02019e9288794769fba95cd6847df9874d49d871d062172f9dd41bc4cc"
+checksum = "266b2e40bc00e5a6c09c3584011e08b06f123c00362c92b975ba9843aaaa14b8"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.37",
+ "syn 2.0.39",
 ]
 
 [[package]]
 name = "toml"
 version = "0.7.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dd79e69d3b627db300ff956027cc6c3798cef26d22526befdfcd12feeb6d2257"
@@ -701,17 +701,17 @@
  "serde_spanned",
  "toml_datetime",
  "toml_edit",
 ]
 
 [[package]]
 name = "toml_datetime"
-version = "0.6.3"
+version = "0.6.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7cda73e2f1397b1262d6dfdcef8aafae14d1de7748d66822d3bfeeb6d03e5e4b"
+checksum = "3550f4e9685620ac18a50ed434eb3aec30db8ba93b0287467bca5826ea25baf1"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "toml_edit"
 version = "0.19.15"
@@ -816,13 +816,13 @@
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "winnow"
-version = "0.5.15"
+version = "0.5.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7c2e3184b9c4e92ad5167ca73039d0c42476302ab603e2fec4487511f38ccefc"
+checksum = "829846f3e3db426d4cee4510841b71a8e58aa2a76b1132579487ae430ccd9c7b"
 dependencies = [
  "memchr",
 ]
```

### Comparing `neuromorphic_drivers-0.8.3/PKG-INFO` & `neuromorphic_drivers-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuromorphic_drivers
-Version: 0.8.3
+Version: 0.9.0
 Requires-Dist: numpy >=1.24
 License-File: LICENSE
 Summary: Neuromorphic devices drivers
 Author: International Centre for Neuromorphic Systems, Alexandre Marcireau
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: homepage, https://github.com/neuromorphicsystems/neuromorphic-rs/
```

