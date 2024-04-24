# Comparing `tmp/f4-0.9.6.tar.gz` & `tmp/f4-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f4-0.9.6.tar", last modified: Tue Apr 23 18:53:55 2024, max compression
+gzip compressed data, was "f4-0.9.7.tar", last modified: Wed Apr 24 16:18:12 2024, max compression
```

## Comparing `f4-0.9.6.tar` & `f4-0.9.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-23 18:53:55.767145 f4-0.9.6/
--rw-r--r--   0 srp33      (503) staff       (20)    11357 2023-12-07 22:20:43.000000 f4-0.9.6/LICENSE
--rw-r--r--   0 srp33      (503) staff       (20)      711 2024-04-23 18:53:55.767086 f4-0.9.6/PKG-INFO
--rwxr-xr-x   0 srp33      (503) staff       (20)       67 2023-12-07 22:20:43.000000 f4-0.9.6/README.md
--rw-r--r--   0 srp33      (503) staff       (20)      104 2023-12-07 22:20:43.000000 f4-0.9.6/pyproject.toml
--rw-r--r--   0 srp33      (503) staff       (20)      733 2024-04-23 18:53:55.767710 f4-0.9.6/setup.cfg
-drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-23 18:53:55.762336 f4-0.9.6/src/
-drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-23 18:53:55.765272 f4-0.9.6/src/f4/
--rwxr-xr-x   0 srp33      (503) staff       (20)    43623 2024-04-19 19:32:05.000000 f4-0.9.6/src/f4/Builder.py
--rwxr-xr-x   0 srp33      (503) staff       (20)    57954 2024-04-20 14:29:06.000000 f4-0.9.6/src/f4/Parser.py
--rw-r--r--   0 srp33      (503) staff       (20)    15529 2024-04-23 18:52:11.000000 f4-0.9.6/src/f4/Transformer.py
--rwxr-xr-x   0 srp33      (503) staff       (20)     8388 2024-04-23 18:53:04.000000 f4-0.9.6/src/f4/Utilities.py
--rwxr-xr-x   0 srp33      (503) staff       (20)      390 2024-04-20 14:32:09.000000 f4-0.9.6/src/f4/__init__.py
-drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-23 18:53:55.766876 f4-0.9.6/src/f4.egg-info/
--rw-r--r--   0 srp33      (503) staff       (20)      711 2024-04-23 18:53:55.000000 f4-0.9.6/src/f4.egg-info/PKG-INFO
--rw-r--r--   0 srp33      (503) staff       (20)      300 2024-04-23 18:53:55.000000 f4-0.9.6/src/f4.egg-info/SOURCES.txt
--rw-r--r--   0 srp33      (503) staff       (20)        1 2024-04-23 18:53:55.000000 f4-0.9.6/src/f4.egg-info/dependency_links.txt
--rw-r--r--   0 srp33      (503) staff       (20)       67 2024-04-23 18:53:55.000000 f4-0.9.6/src/f4.egg-info/requires.txt
--rw-r--r--   0 srp33      (503) staff       (20)        3 2024-04-23 18:53:55.000000 f4-0.9.6/src/f4.egg-info/top_level.txt
-drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-23 18:53:55.766153 f4-0.9.6/test/
--rwxr-xr-x   0 srp33      (503) staff       (20)    55963 2024-04-23 17:55:35.000000 f4-0.9.6/test/test.py
+drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-24 16:18:12.439211 f4-0.9.7/
+-rw-r--r--   0 srp33      (503) staff       (20)    11357 2023-12-07 22:20:43.000000 f4-0.9.7/LICENSE
+-rw-r--r--   0 srp33      (503) staff       (20)      711 2024-04-24 16:18:12.439139 f4-0.9.7/PKG-INFO
+-rwxr-xr-x   0 srp33      (503) staff       (20)       67 2023-12-07 22:20:43.000000 f4-0.9.7/README.md
+-rw-r--r--   0 srp33      (503) staff       (20)      104 2023-12-07 22:20:43.000000 f4-0.9.7/pyproject.toml
+-rw-r--r--   0 srp33      (503) staff       (20)      733 2024-04-24 16:18:12.439539 f4-0.9.7/setup.cfg
+drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-24 16:18:12.434012 f4-0.9.7/src/
+drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-24 16:18:12.437240 f4-0.9.7/src/f4/
+-rwxr-xr-x   0 srp33      (503) staff       (20)    43623 2024-04-19 19:32:05.000000 f4-0.9.7/src/f4/Builder.py
+-rwxr-xr-x   0 srp33      (503) staff       (20)    57954 2024-04-20 14:29:06.000000 f4-0.9.7/src/f4/Parser.py
+-rw-r--r--   0 srp33      (503) staff       (20)    16410 2024-04-24 15:00:46.000000 f4-0.9.7/src/f4/Transformer.py
+-rwxr-xr-x   0 srp33      (503) staff       (20)     8388 2024-04-24 15:31:21.000000 f4-0.9.7/src/f4/Utilities.py
+-rwxr-xr-x   0 srp33      (503) staff       (20)      390 2024-04-20 14:32:09.000000 f4-0.9.7/src/f4/__init__.py
+drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-24 16:18:12.438917 f4-0.9.7/src/f4.egg-info/
+-rw-r--r--   0 srp33      (503) staff       (20)      711 2024-04-24 16:18:12.000000 f4-0.9.7/src/f4.egg-info/PKG-INFO
+-rw-r--r--   0 srp33      (503) staff       (20)      300 2024-04-24 16:18:12.000000 f4-0.9.7/src/f4.egg-info/SOURCES.txt
+-rw-r--r--   0 srp33      (503) staff       (20)        1 2024-04-24 16:18:12.000000 f4-0.9.7/src/f4.egg-info/dependency_links.txt
+-rw-r--r--   0 srp33      (503) staff       (20)       67 2024-04-24 16:18:12.000000 f4-0.9.7/src/f4.egg-info/requires.txt
+-rw-r--r--   0 srp33      (503) staff       (20)        3 2024-04-24 16:18:12.000000 f4-0.9.7/src/f4.egg-info/top_level.txt
+drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-24 16:18:12.438109 f4-0.9.7/test/
+-rwxr-xr-x   0 srp33      (503) staff       (20)    55963 2024-04-24 14:57:36.000000 f4-0.9.7/test/test.py
```

### Comparing `f4-0.9.6/LICENSE` & `f4-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `f4-0.9.6/PKG-INFO` & `f4-0.9.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f4
-Version: 0.9.6
+Version: 0.9.7
 Summary: A Python package for the Fast Fixed-width File Format (F4)
 Home-page: https://github.com/srp33/f4py
 Author: Stephen R. Piccolo
 Author-email: stephen.piccolo.byu@gmail.com
 Project-URL: Docs, https://f4py.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `f4-0.9.6/setup.cfg` & `f4-0.9.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = f4
-version = 0.9.6
+version = 0.9.7
 author = Stephen R. Piccolo
 author_email = stephen.piccolo.byu@gmail.com
 description = A Python package for the Fast Fixed-width File Format (F4)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/srp33/f4py
 project_urls =
```

### Comparing `f4-0.9.6/src/f4/Builder.py` & `f4-0.9.7/src/f4/Builder.py`

 * *Files identical despite different names*

### Comparing `f4-0.9.6/src/f4/Parser.py` & `f4-0.9.7/src/f4/Parser.py`

 * *Files identical despite different names*

### Comparing `f4-0.9.6/src/f4/Transformer.py` & `f4-0.9.7/src/f4/Transformer.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,53 +8,52 @@
     print_message(f"Finding max column width when transposing {f4_src_file_path} to {f4_dest_file_path}.", verbose)
 
     with initialize(f4_src_file_path) as src_file_data:
         num_cols = src_file_data.cache_dict["num_cols"]
         max_column_width = get_max_column_width(src_file_data)
 
     tmp_dir_path2 = prepare_tmp_dir(tmp_dir_path)
-    tmp_fw_file_path = f"{tmp_dir_path2}fw"
+    tmp_tsv_file_path = f"{tmp_dir_path2}transposed.tsv.zstd"
 
     if num_parallel == 1:
-        transpose_column_chunk(f4_src_file_path, src_column_for_names, 0, range(num_cols), max_column_width, tmp_fw_file_path, verbose)
+        transpose_column_chunk(f4_src_file_path, src_column_for_names, 0, range(num_cols), max_column_width, tmp_tsv_file_path, verbose)
     else:
-        max_cols_per_chunk = 100001
+        max_cols_per_chunk = 10001
 
         global joblib
         joblib = __import__('joblib', globals(), locals())
 
         # Transpose the data in chunks.
         joblib.Parallel(n_jobs=num_parallel)(joblib.delayed(transpose_column_chunk)(
             f4_src_file_path,
             src_column_for_names,
             chunk_number,
             chunk_range,
             max_column_width,
-            f"{tmp_dir_path2}chunk_{chunk_number}.fw",
+            f"{tmp_dir_path2}transposed_chunk_{chunk_number}.tsv.zstd",
             verbose)
                 for chunk_number, chunk_range in enumerate(generate_column_ranges(max_cols_per_chunk, num_cols, num_parallel))
         )
 
         print_message(f"Assembling chunks when transposing {f4_src_file_path} to {f4_dest_file_path}.", verbose)
 
         # Put the chunks together.
-        with open(tmp_fw_file_path, "wb") as tmp_fw_file:
+        with open_temp_file_to_compress(tmp_tsv_file_path, "wb") as tmp_tsv_file:
             for chunk_number, _ignore in enumerate(generate_column_ranges(max_cols_per_chunk, num_cols, num_parallel)):
-                chunk_file_path = f"{tmp_dir_path2}chunk_{chunk_number}.fw"
+                chunk_file_path = f"{tmp_dir_path2}transposed_chunk_{chunk_number}.tsv.zstd"
 
-                with open(chunk_file_path, "rb") as chunk_file:
-                    for line in chunk_file:
-                        tmp_fw_file.write(line)
+                for line in read_compressed_file_line_by_line(chunk_file_path):
+                    tmp_tsv_file.write(line + b"\n")
 
                 remove(chunk_file_path)
 
-    print_message(f"Converting temp file at {tmp_fw_file_path} when transposing {f4_src_file_path} to {f4_dest_file_path}.", verbose)
-    convert_delimited_file(tmp_fw_file_path, f4_dest_file_path, comment_prefix=None, compression_type=src_file_data.decompression_type, index_columns=index_columns, num_parallel=num_parallel, verbose=verbose)
+    print_message(f"Converting temp file at {tmp_tsv_file_path} when transposing {f4_src_file_path} to {f4_dest_file_path}.", verbose)
+    convert_delimited_file(tmp_tsv_file_path, f4_dest_file_path, comment_prefix=None, compression_type=src_file_data.decompression_type, index_columns=index_columns, num_parallel=num_parallel, verbose=verbose)
 
-    remove(tmp_fw_file_path)
+    remove(tmp_tsv_file_path)
     rmtree(tmp_dir_path2)
 
 def generate_column_ranges(max_cols_per_chunk, num_cols, num_parallel):
     if num_cols > max_cols_per_chunk:
         column_ranges = generate_range_chunks(num_cols, max_cols_per_chunk)
     else:
         column_ranges = generate_range_chunks(num_cols, ceil(num_cols / num_parallel))
@@ -73,42 +72,45 @@
         # Find the max width of values.
         column_coords = parse_data_coord(src_file_data, "", column_index)
         column_size = column_coords[1] - column_coords[0]
         max_column_width = max(max_column_width, column_size)
 
     return max_column_width
 
-def transpose_column_chunk(f4_src_file_path, src_column_for_names, chunk_number, column_range, max_column_width, tmp_fw_file_path, verbose):
+def transpose_column_chunk(f4_src_file_path, src_column_for_names, chunk_number, column_range, max_column_width, tmp_tsv_file_path, verbose):
+    tmp_fw_file_path = f"{tmp_tsv_file_path}.fw"
+
     with initialize(f4_src_file_path) as src_file_data:
         print_message(f"Parsing column coordinates for chunk {chunk_number} when transposing {f4_src_file_path}.", verbose)
         # Get basic meta information.
         num_rows = src_file_data.cache_dict["num_rows"]
         src_column_for_names_index = get_column_index_from_name(src_file_data, src_column_for_names.encode())
         src_column_for_names_coords = parse_data_coord(src_file_data, "", src_column_for_names_index)
         parse_row_value_function = get_parse_row_value_function(src_file_data)
         parse_row_values_function = get_parse_row_values_function(src_file_data)
 
         all_column_coords = parse_data_coords(src_file_data, "", column_range)
 
-        print_message(f"Filling temp file {tmp_fw_file_path} with empty space for chunk {chunk_number} when transposing {f4_src_file_path}.", verbose)
         # We can't compress this file because we have to navigate around it later.
         with open(tmp_fw_file_path, "wb") as fw_file:
             if chunk_number == 0:
+                print_message(f"Filling temp file {tmp_fw_file_path} with new column names for chunk {chunk_number} when transposing {f4_src_file_path}.", verbose)
                 # Write the value to the top-left cell.
                 fw_file.write(format_string_as_fixed_width(src_column_for_names.encode(), max_column_width) + b"\t")
 
                 # Write the transposed column names (except the last one).
                 for row_index in range(num_rows - 1):
                     src_column_for_names_value = parse_row_value_function(src_file_data, "", row_index, src_column_for_names_coords)
                     fw_file.write(format_string_as_fixed_width(src_column_for_names_value, max_column_width) + b"\t")
 
                 # Write the last transposed column name.
                 src_column_for_names_value = parse_row_value_function(src_file_data, "", num_rows - 1, src_column_for_names_coords)
                 fw_file.write(format_string_as_fixed_width(src_column_for_names_value, max_column_width) + b"\n")
 
+            print_message(f"Filling temp file {tmp_fw_file_path} with empty space for chunk {chunk_number} when transposing {f4_src_file_path}.", verbose)
             # Populate the rest of the file with empty space, which will later be filled in with values.
             for column_index in column_range:
                 if column_index == src_column_for_names_index:
                     continue
 
                 for row_index in range(num_rows):
                     fw_file.write(b" " * max_column_width + b"\t")
@@ -120,48 +122,57 @@
         print_message(f"Saving new row names to temp file {tmp_fw_file_path} for chunk {chunk_number} when transposing {f4_src_file_path}.", verbose)
         cn_current, cn_end = advance_to_column_names(src_file_data, column_range[0] - 1)
         # Skip the first column name because we already wrote it in the top-left corner.
         cn_current, column_name = get_next_column_name(src_file_data, cn_current, cn_end)
 
         # We can't compress this file because we have to navigate within it.
         with open(tmp_fw_file_path, "rb+") as fw_file:
-            # FYI: Using memory mapping is an option, but it can consume a lot of memory
-            #      in this context.
-            # with mmap(fw_file.fileno(), 0, prot=PROT_WRITE) as fw_handle:
-            # Save new row names.
-            for chunk_column_index, overall_column_index in enumerate(column_range):
-                if overall_column_index == src_column_for_names_index:
-                    continue
-
-                cn_current, column_name = get_next_column_name(src_file_data, cn_current, cn_end)
-                row_start = chunk_column_index * new_row_width
-                # fw_handle[row_start:(row_start + len(column_name))] = column_name
-                fw_file.seek(row_start)
-                fw_file.write(column_name)
-
-            # Save values in transposed orientation.
-            for row_index in range(num_rows):
-                if row_index < 10 or (row_index < 100 and row_index % 10 == 0) or row_index % 100 == 0:
-                    print_message(f"Saving data to temp file {tmp_fw_file_path} for chunk {chunk_number} and original row {row_index}when transposing {f4_src_file_path}.", verbose)
-
-                #FYI: Retrieving all values in a row is much faster than one at a time.
-                values = parse_row_values_function(src_file_data, "", row_index, all_column_coords)
-
+            with mmap(fw_file.fileno(), 0, prot=PROT_WRITE) as fw_handle:
+                # Save new row names.
                 for chunk_column_index, overall_column_index in enumerate(column_range):
                     if overall_column_index == src_column_for_names_index:
                         continue
 
-                    value = values[chunk_column_index]
-
+                    cn_current, column_name = get_next_column_name(src_file_data, cn_current, cn_end)
                     row_start = chunk_column_index * new_row_width
-                    value_start = row_start + (row_index + 1) * (max_column_width + 1)
+                    # fw_handle[row_start:(row_start + len(column_name))] = column_name
+                    fw_file.seek(row_start)
+                    fw_file.write(column_name)
+
+                # Save values in transposed orientation.
+                for row_index in range(num_rows):
+                    print_message(f"Saving data to temp file {tmp_fw_file_path} for chunk {chunk_number} and original row {row_index} when transposing {f4_src_file_path}.", verbose, row_index)
+
+                    #FYI: Retrieving all values in a row is much faster than one at a time.
+                    values = parse_row_values_function(src_file_data, "", row_index, all_column_coords)
+
+                    for chunk_column_index, overall_column_index in enumerate(column_range):
+                        if overall_column_index == src_column_for_names_index:
+                            continue
+
+                        value = values[chunk_column_index]
+
+                        row_start = chunk_column_index * new_row_width
+                        value_start = row_start + (row_index + 1) * (max_column_width + 1)
+
+                        # fw_handle[value_start:(value_start + len(value))] = value
+                        fw_file.seek(value_start)
+                        fw_file.write(value)
+
+        # Convert the temporary fixed-width file to TSV and compress so it doesn't take up so much disk space for temp files.
+        print_message(f"Converting fixed-width temp file at {tmp_fw_file_path} to compressed TSV when transposing {f4_src_file_path}.", verbose)
+        with open(tmp_fw_file_path, "rb") as fw_file:
+            with open_temp_file_to_compress(tmp_tsv_file_path) as tsv_file:
+            # with open(tmp_tsv_file_path, "wb") as tsv_file:
+                for line in fw_file:
+                    line_items = line.rstrip(b"\n").split(b"\t")
+                    line_items = [x.rstrip(b" ") for x in line_items]
+                    tsv_file.write(b"\t".join(line_items) + b"\n")
 
-                    # fw_handle[value_start:(value_start + len(value))] = value
-                    fw_file.seek(value_start)
-                    fw_file.write(value)
+        remove(tmp_fw_file_path)
 
 def advance_to_column_names(src_file_data, first_col_index):
     cn_current = src_file_data.file_map_dict["cn"][0]
     cn_end = src_file_data.file_map_dict["cn"][1]
 
     # Advance to the first column name for this chunk range.
     for column_index in range(first_col_index):
```

### Comparing `f4-0.9.6/src/f4/Utilities.py` & `f4-0.9.7/src/f4/Utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import sqlite3
 import sys
 from tempfile import mkdtemp
 from uuid import uuid4
 from zstandard import ZstdCompressor, ZstdDecompressor
 
 def get_current_version():
-    return "0.9.6"
+    return "0.9.7"
 
 #####################################################
 # Constants
 #####################################################
 
 def get_current_version_major():
     return get_current_version().split(".")[0]
```

### Comparing `f4-0.9.6/src/f4.egg-info/PKG-INFO` & `f4-0.9.7/src/f4.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f4
-Version: 0.9.6
+Version: 0.9.7
 Summary: A Python package for the Fast Fixed-width File Format (F4)
 Home-page: https://github.com/srp33/f4py
 Author: Stephen R. Piccolo
 Author-email: stephen.piccolo.byu@gmail.com
 Project-URL: Docs, https://f4py.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `f4-0.9.6/test/test.py` & `f4-0.9.7/test/test.py`

 * *Files 0% similar despite different names*

```diff
@@ -859,27 +859,27 @@
     num_lines = 0
     with open(out_file_path, "r", newline="\n") as out_file:
         for line in out_file:
             num_lines += 1
 
     print(f"  {elapsed_time:.2f} seconds, {num_lines} lines in output file")
 
-run_all_small_tests()
+#run_all_small_tests()
 #sys.exit()
 
 for compression_type in [None]:
 #for compression_type in ["zstd"]:
 #for compression_type in [None, "zstd"]:
     # Medium tests
 #    run_larger_tests(num_parallel=1, size="medium", extension="", discrete1_index=11, numeric1_index=21, build_outputs=True, verbose=True, compression_type=compression_type, tmp_dir_path="/tmp/medium")
 #    run_larger_tests(num_parallel=2, size="medium", extension="", discrete1_index=11, numeric1_index=21, build_outputs=True, verbose=True, compression_type=compression_type, tmp_dir_path="/tmp/medium")
 
     # Large tests
-    num_parallel = 1
-#    num_parallel = 4
+#    num_parallel = 1
+    num_parallel = 4
 #    num_parallel = 16
     build_outputs = True
     #build_outputs = False
     verbose = True
     #verbose = False
     check_outputs = True
     #check_outputs = False
@@ -899,14 +899,14 @@
 #    run_super_tests(num_parallel=num_parallel, size="super_tall", extension=".gz", compression_type=compression_type, verbose=verbose, tmp_dir_path="/tmp/super_tall")
 #    run_super_tests(num_parallel=num_parallel, size="super_wide", extension=".gz", compression_type=compression_type, verbose=verbose, tmp_dir_path="/tmp/super_wide")
 #    run_super_tests(num_parallel=num_parallel, size="hyper_tall", extension=".gz", compression_type=compression_type, verbose=verbose, tmp_dir_path="/tmp/hyper_tall")
 #    run_super_tests(num_parallel=num_parallel, size="hyper_wide", extension=".gz", compression_type=compression_type, verbose=verbose, tmp_dir_path="/tmp/hyper_wide")
 
     #Attempt this? https://community.hpe.com/t5/servers-systems-the-right/cray-graph-engine-takes-on-a-trillion-triples/ba-p/7096770
 
-#    f4.transpose("data/medium.f4", "/tmp/medium_transposed.f4", src_column_for_names="ID", num_parallel=num_parallel, verbose=verbose)
+    f4.transpose("data/medium.f4", "/tmp/medium_transposed.f4", src_column_for_names="ID", num_parallel=num_parallel, verbose=verbose)
 #    f4.transpose("data/large_tall.f4", "/tmp/large_tall_transposed.f4", src_column_for_names="ID", num_parallel=num_parallel, verbose=verbose)
 
 #    f4.inner_join("data/medium.f4", "data/medium.f4", "ID", "/tmp/medium_joined.f4", num_parallel=num_parallel, verbose=verbose)
 #    f4.inner_join("data/large_tall.f4", "data/large_wide.f4", "ID", "/tmp/large_joined.f4", num_parallel=num_parallel, verbose=verbose)
 
 print("All tests passed!!")
```

