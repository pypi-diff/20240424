# Comparing `tmp/views_tensor_utilities-0.8.1.tar.gz` & `tmp/views_tensor_utilities-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "views_tensor_utilities-0.8.1.tar", max compression
+gzip compressed data, was "views_tensor_utilities-0.8.2.tar", max compression
```

## Comparing `views_tensor_utilities-0.8.1.tar` & `views_tensor_utilities-0.8.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     8303 2024-03-04 12:04:18.486295 views_tensor_utilities-0.8.1/README.md
--rw-r--r--   0        0        0      456 2024-03-18 13:50:56.547160 views_tensor_utilities-0.8.1/pyproject.toml
--rw-r--r--   0        0        0        1 2024-02-23 12:07:30.835277 views_tensor_utilities-0.8.1/views_tensor_utilities/__init__.py
--rw-r--r--   0        0        0      406 2024-03-06 13:40:55.851241 views_tensor_utilities-0.8.1/views_tensor_utilities/defaults.py
--rw-r--r--   0        0        0    17299 2024-03-18 13:47:31.883077 views_tensor_utilities-0.8.1/views_tensor_utilities/mappings.py
--rw-r--r--   0        0        0    11089 2024-03-18 09:06:12.021882 views_tensor_utilities-0.8.1/views_tensor_utilities/objects.py
--rw-r--r--   0        0        0     8754 1970-01-01 00:00:00.000000 views_tensor_utilities-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     8303 2024-03-04 12:04:18.486295 views_tensor_utilities-0.8.2/README.md
+-rw-r--r--   0        0        0      456 2024-04-23 11:50:20.074448 views_tensor_utilities-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0        1 2024-02-23 12:07:30.835277 views_tensor_utilities-0.8.2/views_tensor_utilities/__init__.py
+-rw-r--r--   0        0        0      406 2024-03-06 13:40:55.851241 views_tensor_utilities-0.8.2/views_tensor_utilities/defaults.py
+-rw-r--r--   0        0        0    17317 2024-04-05 13:30:17.282571 views_tensor_utilities-0.8.2/views_tensor_utilities/mappings.py
+-rw-r--r--   0        0        0    11099 2024-04-23 11:49:43.048800 views_tensor_utilities-0.8.2/views_tensor_utilities/objects.py
+-rw-r--r--   0        0        0     8754 1970-01-01 00:00:00.000000 views_tensor_utilities-0.8.2/PKG-INFO
```

### Comparing `views_tensor_utilities-0.8.1/README.md` & `views_tensor_utilities-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `views_tensor_utilities-0.8.1/views_tensor_utilities/mappings.py` & `views_tensor_utilities-0.8.2/views_tensor_utilities/mappings.py`

 * *Files 0% similar despite different names*

```diff
@@ -512,15 +512,15 @@
     time_space_to_panel_unstrided
 
     Convert numpy time-space-feature tensor to dataframe without using stride-tricks
     """
 
     dtype = tensor.dtype
 
-    dne = defaults.fdne if dtype == np.float64 else len(max(tensor, key=len))*'-'
+    dne = defaults.fdne if dtype in defaults.allowed_float_types else len(max(tensor, key=len))*'-'
 
     time_space = TimeSpaceIndices.from_pandas(index)
 
     nfeature = tensor.shape[-1]
 
     data = np.full((time_space.nrow, nfeature), dne)
```

### Comparing `views_tensor_utilities-0.8.1/views_tensor_utilities/objects.py` & `views_tensor_utilities-0.8.2/views_tensor_utilities/objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -258,30 +258,30 @@
 
         Get and return the numeric part of the container, if it exists
 
         """
 
         for views_tensor in self.ViewsTensors:
             tensor = views_tensor.tensor
-            if tensor.dtype in [defaults.float_type, ]:
+            if tensor.dtype in defaults.allowed_float_types:
                 return views_tensor
         else:
             return None
 
     def get_numeric_tensor(self):
         """
         get_numeric_tensor
 
         Get and return the numeric tensor from the container, if it exists
 
         """
 
         for views_tensor in self.ViewsTensors:
             tensor = views_tensor.tensor
-            if tensor.dtype in [defaults.float_type, ]:
+            if tensor.dtype in defaults.allowed_float_types:
                 return tensor
         else:
             return None
 
     def get_string_part(self):
         """
         get_string_part
```

### Comparing `views_tensor_utilities-0.8.1/PKG-INFO` & `views_tensor_utilities-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: views-tensor-utilities
-Version: 0.8.1
+Version: 0.8.2
 Summary: Classes and functions for transforming between VIEWS-compliant dfs and tensors
 Author: jimdale
 Author-email: jimdale@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.20.0)
```

