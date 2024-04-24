# Comparing `tmp/odbc2deltalake-0.9.0.tar.gz` & `tmp/odbc2deltalake-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odbc2deltalake-0.9.0.tar", max compression
+gzip compressed data, was "odbc2deltalake-0.9.1.tar", max compression
```

## Comparing `odbc2deltalake-0.9.0.tar` & `odbc2deltalake-0.9.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1081 2024-04-23 12:52:12.356009 odbc2deltalake-0.9.0/LICENSE
--rw-r--r--   0        0        0     3563 2024-04-23 12:52:12.356009 odbc2deltalake-0.9.0/README.md
--rw-r--r--   0        0        0      571 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/odbc2deltalake/__init__.py
--rw-r--r--   0        0        0    37607 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/odbc2deltalake/db_to_delta.py
--rw-r--r--   0        0        0     4371 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/odbc2deltalake/delta_logger.py
--rw-r--r--   0        0        0       38 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/odbc2deltalake/destination/__init__.py
--rw-r--r--   0        0        0     2554 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/odbc2deltalake/destination/azure.py
--rw-r--r--   0        0        0     2923 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/odbc2deltalake/destination/azure_utils.py
--rw-r--r--   0        0        0     2541 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/odbc2deltalake/destination/databricks.py
--rw-r--r--   0        0        0     1196 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/odbc2deltalake/destination/destination.py
--rw-r--r--   0        0        0     1592 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/odbc2deltalake/destination/file_system.py
--rw-r--r--   0        0        0     5458 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/odbc2deltalake/metadata.py
--rw-r--r--   0        0        0     1221 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/odbc2deltalake/odbc_utils.py
--rw-r--r--   0        0        0     1851 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/odbc2deltalake/query.py
--rw-r--r--   0        0        0       38 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/odbc2deltalake/reader/__init__.py
--rw-r--r--   0        0        0     7295 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/odbc2deltalake/reader/odbc_reader.py
--rw-r--r--   0        0        0     1961 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/odbc2deltalake/reader/reader.py
--rw-r--r--   0        0        0     4932 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/odbc2deltalake/reader/spark_reader.py
--rw-r--r--   0        0        0     1976 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/odbc2deltalake/sql_glot_utils.py
--rw-r--r--   0        0        0     1211 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/odbc2deltalake/sql_schema.py
--rw-r--r--   0        0        0      249 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/odbc2deltalake/utils.py
--rw-r--r--   0        0        0     7829 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/odbc2deltalake/write_init.py
--rw-r--r--   0        0        0        0 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/odbc2deltalake/write_utils/__init__.py
--rw-r--r--   0        0        0     6810 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/odbc2deltalake/write_utils/restore_pk.py
--rw-r--r--   0        0        0     1393 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     4489 1970-01-01 00:00:00.000000 odbc2deltalake-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-04-23 13:47:00.780259 odbc2deltalake-0.9.1/LICENSE
+-rw-r--r--   0        0        0     3563 2024-04-23 13:47:00.780259 odbc2deltalake-0.9.1/README.md
+-rw-r--r--   0        0        0      571 2024-04-23 13:47:00.780259 odbc2deltalake-0.9.1/odbc2deltalake/__init__.py
+-rw-r--r--   0        0        0    37655 2024-04-23 13:47:00.780259 odbc2deltalake-0.9.1/odbc2deltalake/db_to_delta.py
+-rw-r--r--   0        0        0     4371 2024-04-23 13:47:00.780259 odbc2deltalake-0.9.1/odbc2deltalake/delta_logger.py
+-rw-r--r--   0        0        0       38 2024-04-23 13:47:00.780259 odbc2deltalake-0.9.1/odbc2deltalake/destination/__init__.py
+-rw-r--r--   0        0        0     2554 2024-04-23 13:47:00.780259 odbc2deltalake-0.9.1/odbc2deltalake/destination/azure.py
+-rw-r--r--   0        0        0     2923 2024-04-23 13:47:00.780259 odbc2deltalake-0.9.1/odbc2deltalake/destination/azure_utils.py
+-rw-r--r--   0        0        0     2541 2024-04-23 13:47:00.784259 odbc2deltalake-0.9.1/odbc2deltalake/destination/databricks.py
+-rw-r--r--   0        0        0     1196 2024-04-23 13:47:00.784259 odbc2deltalake-0.9.1/odbc2deltalake/destination/destination.py
+-rw-r--r--   0        0        0     1592 2024-04-23 13:47:00.784259 odbc2deltalake-0.9.1/odbc2deltalake/destination/file_system.py
+-rw-r--r--   0        0        0     5458 2024-04-23 13:47:00.784259 odbc2deltalake-0.9.1/odbc2deltalake/metadata.py
+-rw-r--r--   0        0        0     1221 2024-04-23 13:47:00.784259 odbc2deltalake-0.9.1/odbc2deltalake/odbc_utils.py
+-rw-r--r--   0        0        0     1851 2024-04-23 13:47:00.784259 odbc2deltalake-0.9.1/odbc2deltalake/query.py
+-rw-r--r--   0        0        0       38 2024-04-23 13:47:00.784259 odbc2deltalake-0.9.1/odbc2deltalake/reader/__init__.py
+-rw-r--r--   0        0        0     7295 2024-04-23 13:47:00.784259 odbc2deltalake-0.9.1/odbc2deltalake/reader/odbc_reader.py
+-rw-r--r--   0        0        0     1961 2024-04-23 13:47:00.784259 odbc2deltalake-0.9.1/odbc2deltalake/reader/reader.py
+-rw-r--r--   0        0        0     4932 2024-04-23 13:47:00.784259 odbc2deltalake-0.9.1/odbc2deltalake/reader/spark_reader.py
+-rw-r--r--   0        0        0     1976 2024-04-23 13:47:00.784259 odbc2deltalake-0.9.1/odbc2deltalake/sql_glot_utils.py
+-rw-r--r--   0        0        0     1211 2024-04-23 13:47:00.784259 odbc2deltalake-0.9.1/odbc2deltalake/sql_schema.py
+-rw-r--r--   0        0        0      249 2024-04-23 13:47:00.784259 odbc2deltalake-0.9.1/odbc2deltalake/utils.py
+-rw-r--r--   0        0        0     7829 2024-04-23 13:47:00.784259 odbc2deltalake-0.9.1/odbc2deltalake/write_init.py
+-rw-r--r--   0        0        0        0 2024-04-23 13:47:00.784259 odbc2deltalake-0.9.1/odbc2deltalake/write_utils/__init__.py
+-rw-r--r--   0        0        0     6810 2024-04-23 13:47:00.784259 odbc2deltalake-0.9.1/odbc2deltalake/write_utils/restore_pk.py
+-rw-r--r--   0        0        0     1393 2024-04-23 13:47:00.784259 odbc2deltalake-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     4489 1970-01-01 00:00:00.000000 odbc2deltalake-0.9.1/PKG-INFO
```

### Comparing `odbc2deltalake-0.9.0/LICENSE` & `odbc2deltalake-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.9.0/README.md` & `odbc2deltalake-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.9.0/odbc2deltalake/__init__.py` & `odbc2deltalake-0.9.1/odbc2deltalake/__init__.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.9.0/odbc2deltalake/db_to_delta.py` & `odbc2deltalake-0.9.1/odbc2deltalake/db_to_delta.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,17 +186,17 @@
                 do_full_load(
                     infos=infos,
                     mode="append",
                 )
             else:
                 do_delta_load(
                     infos=infos,
-                    simple=write_config.load_mode in ["simple_delta", "simple_delta_check"],
-                    simple_check=write_config.load_mode == "simple_delta_check"
-
+                    simple=write_config.load_mode
+                    in ["simple_delta", "simple_delta_check"],
+                    simple_check=write_config.load_mode == "simple_delta_check",
                 )
         lock_file_path.remove()
         _vacuum(
             source, destination / "delta_load" / DBDeltaPathConfigs.LATEST_PK_VERSION
         )
         _vacuum(source, destination / "delta_load" / DBDeltaPathConfigs.DELTA_1_NAME)
         _vacuum(source, destination / "delta_load" / DBDeltaPathConfigs.DELTA_2_NAME)
@@ -360,15 +360,15 @@
         return "temp_" + _clean(table)
     return "temp_" + "_".join((_clean(s) for s in table))
 
 
 def do_delta_load(
     infos: WriteConfigAndInfos,
     simple=False,  # a simple delta load assumes that there are no deletes and no additional updates (eg, when soft-delete is implemented in source properly)
-    simple_check = False # does a simple load and checks if the source and target counts match. If not, do a normal delta load on top
+    simple_check=False,  # does a simple load and checks if the source and target counts match. If not, do a normal delta load on top
 ):
     destination = infos.destination
     logger = infos.logger
     delta_col = infos.delta_col
     write_config = infos.write_config
     assert delta_col is not None, "Must have a delta_col for delta loads"
     reader = infos.source
@@ -472,16 +472,16 @@
             write_config=infos.write_config,
         )
         logger.info(f"{table}: Done delta load")
     else:
         _write_delta2(infos, [], mode="overwrite")  # just to create the delta_2 table
         pk_ts = destination / "delta_load" / DBDeltaPathConfigs.PRIMARY_KEYS_TS
         if pk_ts.exists():
-            pk_ts.remove()
-        
+            pk_ts.remove(True)
+
         write_latest_pk(
             reader,
             destination,
             infos.pk_cols,
             delta_col,
             write_config=write_config,
             merge_delta=True,
@@ -492,15 +492,17 @@
         )
         target_count = reader.local_execute_sql_to_py(
             sg.from_(DBDeltaPathConfigs.LATEST_PK_VERSION).select(
                 ex.Count(this=ex.Star()).as_("cnt")
             )
         )[0]["cnt"]
         if source_count != target_count:
-            logger.warning(f"Source and target count do not match. Source: {source_count}, Target: {target_count}. { 'Do a normal delta' if simple_check else ''}")
+            logger.warning(
+                f"Source and target count do not match. Source: {source_count}, Target: {target_count}. { 'Do a normal delta' if simple_check else ''}"
+            )
             if simple_check:
                 do_delta_load(infos, simple=False)
 
 
 def do_append_inserts_load(infos: WriteConfigAndInfos):
     logger = infos.logger
     write_config = infos.write_config
```

### Comparing `odbc2deltalake-0.9.0/odbc2deltalake/delta_logger.py` & `odbc2deltalake-0.9.1/odbc2deltalake/delta_logger.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.9.0/odbc2deltalake/destination/azure.py` & `odbc2deltalake-0.9.1/odbc2deltalake/destination/azure.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.9.0/odbc2deltalake/destination/azure_utils.py` & `odbc2deltalake-0.9.1/odbc2deltalake/destination/azure_utils.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.9.0/odbc2deltalake/destination/databricks.py` & `odbc2deltalake-0.9.1/odbc2deltalake/destination/databricks.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.9.0/odbc2deltalake/destination/destination.py` & `odbc2deltalake-0.9.1/odbc2deltalake/destination/destination.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.9.0/odbc2deltalake/destination/file_system.py` & `odbc2deltalake-0.9.1/odbc2deltalake/destination/file_system.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.9.0/odbc2deltalake/metadata.py` & `odbc2deltalake-0.9.1/odbc2deltalake/metadata.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.9.0/odbc2deltalake/odbc_utils.py` & `odbc2deltalake-0.9.1/odbc2deltalake/odbc_utils.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.9.0/odbc2deltalake/query.py` & `odbc2deltalake-0.9.1/odbc2deltalake/query.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.9.0/odbc2deltalake/reader/odbc_reader.py` & `odbc2deltalake-0.9.1/odbc2deltalake/reader/odbc_reader.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.9.0/odbc2deltalake/reader/reader.py` & `odbc2deltalake-0.9.1/odbc2deltalake/reader/reader.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.9.0/odbc2deltalake/reader/spark_reader.py` & `odbc2deltalake-0.9.1/odbc2deltalake/reader/spark_reader.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.9.0/odbc2deltalake/sql_glot_utils.py` & `odbc2deltalake-0.9.1/odbc2deltalake/sql_glot_utils.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.9.0/odbc2deltalake/sql_schema.py` & `odbc2deltalake-0.9.1/odbc2deltalake/sql_schema.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.9.0/odbc2deltalake/write_init.py` & `odbc2deltalake-0.9.1/odbc2deltalake/write_init.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.9.0/odbc2deltalake/write_utils/restore_pk.py` & `odbc2deltalake-0.9.1/odbc2deltalake/write_utils/restore_pk.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.9.0/pyproject.toml` & `odbc2deltalake-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "odbc2deltalake"
-version = "0.9.0"
+version = "0.9.1"
 description = ""
 authors = ["Adrian Ehrsam <adrian.ehrsam@bmsuisse.ch>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `odbc2deltalake-0.9.0/PKG-INFO` & `odbc2deltalake-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odbc2deltalake
-Version: 0.9.0
+Version: 0.9.1
 Summary: 
 License: MIT
 Author: Adrian Ehrsam
 Author-email: adrian.ehrsam@bmsuisse.ch
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

