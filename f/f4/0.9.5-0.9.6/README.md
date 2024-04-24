# Comparing `tmp/f4-0.9.5.tar.gz` & `tmp/f4-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f4-0.9.5.tar", last modified: Tue Apr 23 18:15:10 2024, max compression
+gzip compressed data, was "f4-0.9.6.tar", last modified: Tue Apr 23 18:53:55 2024, max compression
```

## Comparing `f4-0.9.5.tar` & `f4-0.9.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-23 18:15:10.774664 f4-0.9.5/
--rw-r--r--   0 srp33      (503) staff       (20)    11357 2023-12-07 22:20:43.000000 f4-0.9.5/LICENSE
--rw-r--r--   0 srp33      (503) staff       (20)      711 2024-04-23 18:15:10.774606 f4-0.9.5/PKG-INFO
--rwxr-xr-x   0 srp33      (503) staff       (20)       67 2023-12-07 22:20:43.000000 f4-0.9.5/README.md
--rw-r--r--   0 srp33      (503) staff       (20)      104 2023-12-07 22:20:43.000000 f4-0.9.5/pyproject.toml
--rw-r--r--   0 srp33      (503) staff       (20)      733 2024-04-23 18:15:10.774971 f4-0.9.5/setup.cfg
-drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-23 18:15:10.770460 f4-0.9.5/src/
-drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-23 18:15:10.773333 f4-0.9.5/src/f4/
--rwxr-xr-x   0 srp33      (503) staff       (20)    43623 2024-04-19 19:32:05.000000 f4-0.9.5/src/f4/Builder.py
--rwxr-xr-x   0 srp33      (503) staff       (20)    57954 2024-04-20 14:29:06.000000 f4-0.9.5/src/f4/Parser.py
--rw-r--r--   0 srp33      (503) staff       (20)    15334 2024-04-23 18:14:14.000000 f4-0.9.5/src/f4/Transformer.py
--rwxr-xr-x   0 srp33      (503) staff       (20)     8388 2024-04-23 18:14:41.000000 f4-0.9.5/src/f4/Utilities.py
--rwxr-xr-x   0 srp33      (503) staff       (20)      390 2024-04-20 14:32:09.000000 f4-0.9.5/src/f4/__init__.py
-drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-23 18:15:10.774391 f4-0.9.5/src/f4.egg-info/
--rw-r--r--   0 srp33      (503) staff       (20)      711 2024-04-23 18:15:10.000000 f4-0.9.5/src/f4.egg-info/PKG-INFO
--rw-r--r--   0 srp33      (503) staff       (20)      300 2024-04-23 18:15:10.000000 f4-0.9.5/src/f4.egg-info/SOURCES.txt
--rw-r--r--   0 srp33      (503) staff       (20)        1 2024-04-23 18:15:10.000000 f4-0.9.5/src/f4.egg-info/dependency_links.txt
--rw-r--r--   0 srp33      (503) staff       (20)       67 2024-04-23 18:15:10.000000 f4-0.9.5/src/f4.egg-info/requires.txt
--rw-r--r--   0 srp33      (503) staff       (20)        3 2024-04-23 18:15:10.000000 f4-0.9.5/src/f4.egg-info/top_level.txt
-drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-23 18:15:10.774196 f4-0.9.5/test/
--rwxr-xr-x   0 srp33      (503) staff       (20)    55963 2024-04-23 17:55:35.000000 f4-0.9.5/test/test.py
+drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-23 18:53:55.767145 f4-0.9.6/
+-rw-r--r--   0 srp33      (503) staff       (20)    11357 2023-12-07 22:20:43.000000 f4-0.9.6/LICENSE
+-rw-r--r--   0 srp33      (503) staff       (20)      711 2024-04-23 18:53:55.767086 f4-0.9.6/PKG-INFO
+-rwxr-xr-x   0 srp33      (503) staff       (20)       67 2023-12-07 22:20:43.000000 f4-0.9.6/README.md
+-rw-r--r--   0 srp33      (503) staff       (20)      104 2023-12-07 22:20:43.000000 f4-0.9.6/pyproject.toml
+-rw-r--r--   0 srp33      (503) staff       (20)      733 2024-04-23 18:53:55.767710 f4-0.9.6/setup.cfg
+drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-23 18:53:55.762336 f4-0.9.6/src/
+drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-23 18:53:55.765272 f4-0.9.6/src/f4/
+-rwxr-xr-x   0 srp33      (503) staff       (20)    43623 2024-04-19 19:32:05.000000 f4-0.9.6/src/f4/Builder.py
+-rwxr-xr-x   0 srp33      (503) staff       (20)    57954 2024-04-20 14:29:06.000000 f4-0.9.6/src/f4/Parser.py
+-rw-r--r--   0 srp33      (503) staff       (20)    15529 2024-04-23 18:52:11.000000 f4-0.9.6/src/f4/Transformer.py
+-rwxr-xr-x   0 srp33      (503) staff       (20)     8388 2024-04-23 18:53:04.000000 f4-0.9.6/src/f4/Utilities.py
+-rwxr-xr-x   0 srp33      (503) staff       (20)      390 2024-04-20 14:32:09.000000 f4-0.9.6/src/f4/__init__.py
+drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-23 18:53:55.766876 f4-0.9.6/src/f4.egg-info/
+-rw-r--r--   0 srp33      (503) staff       (20)      711 2024-04-23 18:53:55.000000 f4-0.9.6/src/f4.egg-info/PKG-INFO
+-rw-r--r--   0 srp33      (503) staff       (20)      300 2024-04-23 18:53:55.000000 f4-0.9.6/src/f4.egg-info/SOURCES.txt
+-rw-r--r--   0 srp33      (503) staff       (20)        1 2024-04-23 18:53:55.000000 f4-0.9.6/src/f4.egg-info/dependency_links.txt
+-rw-r--r--   0 srp33      (503) staff       (20)       67 2024-04-23 18:53:55.000000 f4-0.9.6/src/f4.egg-info/requires.txt
+-rw-r--r--   0 srp33      (503) staff       (20)        3 2024-04-23 18:53:55.000000 f4-0.9.6/src/f4.egg-info/top_level.txt
+drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-23 18:53:55.766153 f4-0.9.6/test/
+-rwxr-xr-x   0 srp33      (503) staff       (20)    55963 2024-04-23 17:55:35.000000 f4-0.9.6/test/test.py
```

### Comparing `f4-0.9.5/LICENSE` & `f4-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `f4-0.9.5/PKG-INFO` & `f4-0.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f4
-Version: 0.9.5
+Version: 0.9.6
 Summary: A Python package for the Fast Fixed-width File Format (F4)
 Home-page: https://github.com/srp33/f4py
 Author: Stephen R. Piccolo
 Author-email: stephen.piccolo.byu@gmail.com
 Project-URL: Docs, https://f4py.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `f4-0.9.5/setup.cfg` & `f4-0.9.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = f4
-version = 0.9.5
+version = 0.9.6
 author = Stephen R. Piccolo
 author_email = stephen.piccolo.byu@gmail.com
 description = A Python package for the Fast Fixed-width File Format (F4)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/srp33/f4py
 project_urls =
```

### Comparing `f4-0.9.5/src/f4/Builder.py` & `f4-0.9.6/src/f4/Builder.py`

 * *Files identical despite different names*

### Comparing `f4-0.9.5/src/f4/Parser.py` & `f4-0.9.6/src/f4/Parser.py`

 * *Files identical despite different names*

### Comparing `f4-0.9.5/src/f4/Transformer.py` & `f4-0.9.6/src/f4/Transformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,14 +113,15 @@
                 for row_index in range(num_rows):
                     fw_file.write(b" " * max_column_width + b"\t")
 
                 fw_file.write(b" " * max_column_width + b"\n")
 
         new_row_width = (num_rows + 1) * (max_column_width + 1)
 
+        print_message(f"Saving new row names to temp file {tmp_fw_file_path} for chunk {chunk_number} when transposing {f4_src_file_path}.", verbose)
         cn_current, cn_end = advance_to_column_names(src_file_data, column_range[0] - 1)
         # Skip the first column name because we already wrote it in the top-left corner.
         cn_current, column_name = get_next_column_name(src_file_data, cn_current, cn_end)
 
         # We can't compress this file because we have to navigate within it.
         with open(tmp_fw_file_path, "rb+") as fw_file:
             # FYI: Using memory mapping is an option, but it can consume a lot of memory
@@ -136,15 +137,15 @@
                 # fw_handle[row_start:(row_start + len(column_name))] = column_name
                 fw_file.seek(row_start)
                 fw_file.write(column_name)
 
             # Save values in transposed orientation.
             for row_index in range(num_rows):
                 if row_index < 10 or (row_index < 100 and row_index % 10 == 0) or row_index % 100 == 0:
-                    print_message(f"Transposing {f4_src_file_path} to temporary file {tmp_fw_file_path} for row {row_index}.", verbose)
+                    print_message(f"Saving data to temp file {tmp_fw_file_path} for chunk {chunk_number} and original row {row_index}when transposing {f4_src_file_path}.", verbose)
 
                 #FYI: Retrieving all values in a row is much faster than one at a time.
                 values = parse_row_values_function(src_file_data, "", row_index, all_column_coords)
 
                 for chunk_column_index, overall_column_index in enumerate(column_range):
                     if overall_column_index == src_column_for_names_index:
                         continue
```

### Comparing `f4-0.9.5/src/f4/Utilities.py` & `f4-0.9.6/src/f4/Utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import sqlite3
 import sys
 from tempfile import mkdtemp
 from uuid import uuid4
 from zstandard import ZstdCompressor, ZstdDecompressor
 
 def get_current_version():
-    return "0.9.5"
+    return "0.9.6"
 
 #####################################################
 # Constants
 #####################################################
 
 def get_current_version_major():
     return get_current_version().split(".")[0]
```

### Comparing `f4-0.9.5/src/f4.egg-info/PKG-INFO` & `f4-0.9.6/src/f4.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f4
-Version: 0.9.5
+Version: 0.9.6
 Summary: A Python package for the Fast Fixed-width File Format (F4)
 Home-page: https://github.com/srp33/f4py
 Author: Stephen R. Piccolo
 Author-email: stephen.piccolo.byu@gmail.com
 Project-URL: Docs, https://f4py.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `f4-0.9.5/test/test.py` & `f4-0.9.6/test/test.py`

 * *Files identical despite different names*

