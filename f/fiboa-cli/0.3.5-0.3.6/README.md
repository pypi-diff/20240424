# Comparing `tmp/fiboa_cli-0.3.5.tar.gz` & `tmp/fiboa_cli-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiboa_cli-0.3.5.tar", last modified: Mon Apr 22 21:49:38 2024, max compression
+gzip compressed data, was "fiboa_cli-0.3.6.tar", last modified: Wed Apr 24 11:26:46 2024, max compression
```

## Comparing `fiboa_cli-0.3.5.tar` & `fiboa_cli-0.3.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:49:38.831220 fiboa_cli-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-22 21:49:34.000000 fiboa_cli-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-04-22 21:49:38.831220 fiboa_cli-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-04-22 21:49:34.000000 fiboa_cli-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:49:38.827220 fiboa_cli-0.3.5/fiboa_cli/
--rw-r--r--   0 runner    (1001) docker     (127)    10916 2024-04-22 21:49:34.000000 fiboa_cli-0.3.5/fiboa_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-22 21:49:34.000000 fiboa_cli-0.3.5/fiboa_cli/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-22 21:49:34.000000 fiboa_cli-0.3.5/fiboa_cli/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     8602 2024-04-22 21:49:34.000000 fiboa_cli-0.3.5/fiboa_cli/convert_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-22 21:49:34.000000 fiboa_cli-0.3.5/fiboa_cli/create_geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-22 21:49:34.000000 fiboa_cli-0.3.5/fiboa_cli/create_geoparquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-22 21:49:34.000000 fiboa_cli-0.3.5/fiboa_cli/describe.py
--rw-r--r--   0 runner    (1001) docker     (127)     9648 2024-04-22 21:49:34.000000 fiboa_cli-0.3.5/fiboa_cli/geopandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-04-22 21:49:34.000000 fiboa_cli-0.3.5/fiboa_cli/jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-22 21:49:34.000000 fiboa_cli-0.3.5/fiboa_cli/jsonschema_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-04-22 21:49:34.000000 fiboa_cli-0.3.5/fiboa_cli/parquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-04-22 21:49:34.000000 fiboa_cli-0.3.5/fiboa_cli/rename_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-04-22 21:49:34.000000 fiboa_cli-0.3.5/fiboa_cli/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-04-22 21:49:34.000000 fiboa_cli-0.3.5/fiboa_cli/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-04-22 21:49:34.000000 fiboa_cli-0.3.5/fiboa_cli/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-22 21:49:34.000000 fiboa_cli-0.3.5/fiboa_cli/validate_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-22 21:49:34.000000 fiboa_cli-0.3.5/fiboa_cli/validate_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-22 21:49:34.000000 fiboa_cli-0.3.5/fiboa_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:49:38.831220 fiboa_cli-0.3.5/fiboa_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-04-22 21:49:38.000000 fiboa_cli-0.3.5/fiboa_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-22 21:49:38.000000 fiboa_cli-0.3.5/fiboa_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 21:49:38.000000 fiboa_cli-0.3.5/fiboa_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-22 21:49:38.000000 fiboa_cli-0.3.5/fiboa_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-22 21:49:38.000000 fiboa_cli-0.3.5/fiboa_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-22 21:49:38.000000 fiboa_cli-0.3.5/fiboa_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 21:49:38.831220 fiboa_cli-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-22 21:49:34.000000 fiboa_cli-0.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:49:38.831220 fiboa_cli-0.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-22 21:49:34.000000 fiboa_cli-0.3.5/tests/test_jsonschema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:26:46.972685 fiboa_cli-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 11:26:42.000000 fiboa_cli-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-04-24 11:26:46.968685 fiboa_cli-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-04-24 11:26:42.000000 fiboa_cli-0.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:26:46.968685 fiboa_cli-0.3.6/fiboa_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)    12187 2024-04-24 11:26:42.000000 fiboa_cli-0.3.6/fiboa_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-24 11:26:42.000000 fiboa_cli-0.3.6/fiboa_cli/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-24 11:26:42.000000 fiboa_cli-0.3.6/fiboa_cli/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8602 2024-04-24 11:26:42.000000 fiboa_cli-0.3.6/fiboa_cli/convert_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-24 11:26:42.000000 fiboa_cli-0.3.6/fiboa_cli/create_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-24 11:26:42.000000 fiboa_cli-0.3.6/fiboa_cli/create_geoparquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-24 11:26:42.000000 fiboa_cli-0.3.6/fiboa_cli/describe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9751 2024-04-24 11:26:42.000000 fiboa_cli-0.3.6/fiboa_cli/geopandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-04-24 11:26:42.000000 fiboa_cli-0.3.6/fiboa_cli/jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-24 11:26:42.000000 fiboa_cli-0.3.6/fiboa_cli/jsonschema_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-24 11:26:42.000000 fiboa_cli-0.3.6/fiboa_cli/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-04-24 11:26:42.000000 fiboa_cli-0.3.6/fiboa_cli/rename_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-04-24 11:26:42.000000 fiboa_cli-0.3.6/fiboa_cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8967 2024-04-24 11:26:42.000000 fiboa_cli-0.3.6/fiboa_cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10355 2024-04-24 11:26:42.000000 fiboa_cli-0.3.6/fiboa_cli/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-24 11:26:42.000000 fiboa_cli-0.3.6/fiboa_cli/validate_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-24 11:26:42.000000 fiboa_cli-0.3.6/fiboa_cli/validate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-24 11:26:42.000000 fiboa_cli-0.3.6/fiboa_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:26:46.968685 fiboa_cli-0.3.6/fiboa_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-04-24 11:26:46.000000 fiboa_cli-0.3.6/fiboa_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-24 11:26:46.000000 fiboa_cli-0.3.6/fiboa_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 11:26:46.000000 fiboa_cli-0.3.6/fiboa_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-24 11:26:46.000000 fiboa_cli-0.3.6/fiboa_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-24 11:26:46.000000 fiboa_cli-0.3.6/fiboa_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-24 11:26:46.000000 fiboa_cli-0.3.6/fiboa_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 11:26:46.972685 fiboa_cli-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-24 11:26:42.000000 fiboa_cli-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:26:46.968685 fiboa_cli-0.3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-24 11:26:42.000000 fiboa_cli-0.3.6/tests/test_jsonschema.py
```

### Comparing `fiboa_cli-0.3.5/LICENSE` & `fiboa_cli-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.5/PKG-INFO` & `fiboa_cli-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiboa-cli
-Version: 0.3.5
+Version: 0.3.6
 Summary: CLI tools such as validation and file format conversion for fiboa.
 Home-page: https://github.com/fiboa/cli
 Author: Matthias Mohr
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `fiboa_cli-0.3.5/README.md` & `fiboa_cli-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.5/fiboa_cli/__init__.py` & `fiboa_cli-0.3.6/fiboa_cli/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,21 +29,38 @@
 @click.option(
     '--json', '-j',
     is_flag=True,
     type=click.BOOL,
     help='Print the JSON metadata.',
     default=False
 )
-def describe(file, json):
+@click.option(
+    '--num', '-n',
+    type=click.IntRange(min=0),
+    help='Number of rows to show. Defaults to 10.',
+    default=10
+)
+@click.option(
+    '--column', '-c',
+    type=click.STRING,
+    multiple=True,
+    help='Column names to show in the excerpt. Can be used multiple times. Shows all by default.',
+    default=[]
+)
+def describe(file, json, num = 10, column = []):
     """
     Inspects the content of a fiboa GeoParquet file.
     """
     log(f"fiboa CLI {__version__} - Describe {file}\n", "success")
     try:
-        describe_(file, json)
+        if len(column) == 0:
+            columns = None
+        else:
+            columns = list(column)
+        describe_(file, json, num, columns)
     except Exception as e:
         log(e, "error")
         sys.exit(1)
 
 
 ## VALIDATE
 @click.command()
@@ -53,27 +70,27 @@
     type=click.STRING,
     callback=valid_file_for_cli,
     help='fiboa Schema to validate against. Can be a local file or a URL. If not provided, uses the fiboa version to load the schema for the released version.'
 )
 @click.option(
     '--ext-schema', '-e',
     multiple=True,
-    callback=check_ext_schema_for_cli,
-    help='Maps a remote fiboa extension schema url to a local file. First the URL, then the local file path. Separated with a comma character. Example: https://example.com/schema.json,/path/to/schema.json',
+    callback=lambda ctx, param, value: check_ext_schema_for_cli(value, allow_none = False),
+    help='Maps a remote fiboa extension schema url to a local file. First the URL, then the local file path. Separated with a comma character. Example: https://example.com/schema.yaml,/path/to/schema.yaml',
 )
 @click.option(
     '--fiboa-version', '-f',
     type=click.STRING,
     help='The fiboa version to validate against. Default is the version given in the collection.',
     default=None
 )
 @click.option(
     '--collection', '-c',
     type=click.Path(exists=True),
-    help='Points to the STAC collection that defines the fiboa version and extensions.',
+    help='Points to the Collection that defines the fiboa version and extensions.',
     default=None
 )
 @click.option(
     '--data', '-d',
     is_flag=True,
     type=click.BOOL,
     help='EXPERIMENTAL: Validate the data in the GeoParquet file. Enabling this might be slow or exceed memory. Default is False.',
@@ -139,45 +156,59 @@
     type=click.Path(exists=False),
     help='File to write the file to.',
     required=True
 )
 @click.option(
     '--collection', '-c',
     callback=valid_file_for_cli,
-    help='Points to the STAC collection that defines the fiboa version and extensions.',
+    help='Points to the Collection that defines the fiboa version and extensions. Only applies if not provided in the GeoJSON file (embedded or as link).',
     default=None
 )
 @click.option(
     '--schema', '-s',
     type=click.Path(exists=True),
     help='fiboa Schema to work against. If not provided, uses the fiboa version from the collection to load the schema for the released version.'
 )
 @click.option(
     '--ext-schema', '-e',
     multiple=True,
-    callback=check_ext_schema_for_cli,
-    help='Maps a remote fiboa extension schema url to a local file. First the URL, then the local file path. Separated with a comma character. Example: https://example.com/schema.json,/path/to/schema.json',
+    callback=lambda ctx, param, value: check_ext_schema_for_cli(value, allow_none = True),
+    help='Applicable fiboa extensions as URLs. Can map a remote fiboa extension schema url to a local file by adding a local file path, separated by a comma. Example: https://example.com/schema.json,/path/to/schema.json',
+)
+@click.option(
+    '--fiboa-version', '-f',
+    type=click.STRING,
+    help=f'The applicable fiboa version if no collection is provided. Defaults to {fiboa_version_}.',
+    default=fiboa_version_
 )
-def create_geoparquet(files, out, collection, schema, ext_schema):
+def create_geoparquet(files, out, collection, schema, ext_schema, fiboa_version):
     """
     Create a fiboa GeoParquet file from GeoJSON file(s).
+
+    The collection metadata has the following priority order:
+    1. Read from the last GeoJSON file/feature (embedded 'fiboa' property)
+    1. Read from the last GeoJSON file/feature (link with relation type 'collection')
+    2. Read from the collection parameter
+    3. Use fiboa_version and extension_schemas parameters
     """
     log(f"fiboa CLI {__version__} - Create GeoParquet\n", "success")
     config = {
         "files": files,
         "out": out,
         "schema": schema,
         "collection": collection,
         "extension_schemas": ext_schema,
+        "fiboa_version": fiboa_version
     }
-    try:
-        create_geoparquet_(config)
-    except Exception as e:
-        log(e, "error")
-        sys.exit(1)
+    create_geoparquet_(config)
+    # try:
+    #     create_geoparquet_(config)
+    # except Exception as e:
+    #     log(e, "error")
+    #     sys.exit(1)
 
 
 ## CREATE GEOJSON
 @click.command()
 @click.argument('file', nargs=1, callback=lambda ctx, param, value: valid_file_for_cli_with_ext(value, ["parquet", "geoparquet"]))
 @click.option(
     '--out', '-o',
```

### Comparing `fiboa_cli-0.3.5/fiboa_cli/convert.py` & `fiboa_cli-0.3.6/fiboa_cli/convert.py`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.5/fiboa_cli/convert_utils.py` & `fiboa_cli-0.3.6/fiboa_cli/convert_utils.py`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.5/fiboa_cli/create_geojson.py` & `fiboa_cli-0.3.6/fiboa_cli/create_geojson.py`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.5/fiboa_cli/create_geoparquet.py` & `fiboa_cli-0.3.6/fiboa_cli/create_geoparquet.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,23 +20,33 @@
         else:
             log(f"{file}: Skipped - Unsupported GeoJSON type, must be Feature or FeatureCollection")
 
     if len(features) == 0:
         raise Exception("No valid features provided as input files")
 
     # Add a STAC collection to the fiboa property to the Parquet metadata
-    # todo: for features this loads the collection of the last feature only if not provided specifically
+    # Note: for features this loads the collection of the last feature only
+    # if not provided specifically via collection parameter
     collection = get_collection(geojson, config.get("collection"), file)
+
+    if collection is None:
+        # No collection found, create a default collection based on parameters
+        version = config.get("fiboa_version")
+        collection = {
+            "fiboa_version": version,
+            "fiboa_extensions": list(config.get("extension_schemas", {}).keys()),
+        }
+
+    # add a default id based on the output filename
     if "id" not in collection or not collection["id"]:
         collection["id"] = os.path.basename(output_file)
-    if "fiboa_version" not in collection:
-        raise Exception("No fiboa_version found in collection metadata")
-    else:
+
+    # Make the fiboa_version consistent with the collection
+    if "fiboa_version" in collection:
         config["fiboa_version"] = collection["fiboa_version"]
-    # todo: fill with more/better metadata
 
     # Get a list of the properties/columns (without duplicates)
     columns = set(["id", "geometry"])
     for feature in features:
         keys = feature["properties"].keys()
         columns.update(keys)
```

### Comparing `fiboa_cli-0.3.5/fiboa_cli/geopandas.py` & `fiboa_cli-0.3.6/fiboa_cli/geopandas.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,15 +205,15 @@
     """
     if metadata_str is None:
         return None
 
     return json.loads(metadata_str.decode("utf-8"))
 
 
-def arrow_to_geopandas(table):
+def arrow_to_geopandas(table, allow_non_geo=False):
     """
     Helper function with main, shared logic for read_parquet/read_feather.
     """
     df = table.to_pandas()
 
     metadata = table.schema.metadata
 
@@ -229,19 +229,22 @@
         raise ValueError("Missing or malformed geo metadata in Parquet/Feather file")
 
     # Find all geometry columns that were read from the file.  May
     # be a subset if 'columns' parameter is used.
     geometry_columns = df.columns.intersection(metadata["columns"])
 
     if not len(geometry_columns):
-        raise ValueError(
-            """No geometry columns are included in the columns read from
-            the Parquet/Feather file. To read this file without geometry columns,
-            use pandas.read_parquet/read_feather() instead."""
-        )
+        if allow_non_geo:
+            return df
+        else:
+            raise ValueError(
+                """No geometry columns are included in the columns read from
+                the Parquet/Feather file. To read this file without geometry columns,
+                use pandas.read_parquet/read_feather() instead."""
+            )
 
     geometry = metadata["primary_column"]
 
     # Missing geometry likely indicates a subset of columns was read;
     # promote the first available geometry to the primary geometry.
     if len(geometry_columns) and geometry not in geometry_columns:
         geometry = geometry_columns[0]
```

### Comparing `fiboa_cli-0.3.5/fiboa_cli/jsonschema.py` & `fiboa_cli-0.3.6/fiboa_cli/jsonschema.py`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.5/fiboa_cli/jsonschema_template.py` & `fiboa_cli-0.3.6/fiboa_cli/jsonschema_template.py`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.5/fiboa_cli/parquet.py` & `fiboa_cli-0.3.6/fiboa_cli/parquet.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     # Load all extension schemas
     extensions = {}
     if "fiboa_extensions" in collection and isinstance(collection["fiboa_extensions"], list):
         ext_map = config.get("extension_schemas", [])
         for ext in collection["fiboa_extensions"]:
             try:
-                if ext in ext_map:
+                if ext in ext_map and ext_map[ext] is not None:
                     path = ext_map[ext]
                     log(f"Redirecting {ext} to {path}", "info")
                 else:
                     path = ext
                 extensions[ext] = load_file(path)
                 schemas = merge_schemas(schemas, extensions[ext])
             except Exception as e:
```

### Comparing `fiboa_cli-0.3.5/fiboa_cli/rename_extension.py` & `fiboa_cli-0.3.6/fiboa_cli/rename_extension.py`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.5/fiboa_cli/types.py` & `fiboa_cli-0.3.6/fiboa_cli/types.py`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.5/fiboa_cli/util.py` & `fiboa_cli-0.3.6/fiboa_cli/util.py`

 * *Files 15% similar despite different names*

```diff
@@ -90,26 +90,33 @@
 def load_parquet_schema(uri: Union[str, NativeFile]) -> pq.ParquetSchema:
     """Load schema from Parquet file"""
     if isinstance(uri, str):
         uri = get_pyarrow_file(uri)
     return pq.read_schema(uri)
 
 
-def load_parquet_data(uri: str, nrows = None) -> pd.DataFrame:
+def load_parquet_metadata(uri: Union[str, NativeFile]) -> pq.FileMetaData:
+    """Load metadata from Parquet file"""
+    if isinstance(uri, str):
+        uri = get_pyarrow_file(uri)
+    return pq.read_metadata(uri)
+
+
+def load_parquet_data(uri: str, nrows = None, columns = None) -> pd.DataFrame:
     """Load data from Parquet file"""
     f = get_pyarrow_file(uri)
 
     if nrows is None:
-        table = pq.read_table(f)
+        table = pq.read_table(f, columns = columns)
     else:
         pf = pq.ParquetFile(f)
-        rows = next(pf.iter_batches(batch_size = nrows))
+        rows = next(pf.iter_batches(batch_size = nrows, columns = columns))
         table = pa.Table.from_batches([rows])
 
-    return arrow_to_geopandas(table)
+    return arrow_to_geopandas(table, allow_non_geo = True)
 
 
 def load_fiboa_schema(config):
     """Load fiboa schema"""
     schema_url = config.get('schema')
     schema_version = config.get('fiboa_version')
     if not schema_url:
@@ -219,22 +226,23 @@
                 href = os.path.join(os.path.dirname(basepath), href)
             return load_file(href)
 
     # No collection found
     return None
 
 
-def check_ext_schema_for_cli(ctx, param, value):
+def check_ext_schema_for_cli(value, allow_none = False):
     map = {}
     for v in value:
         try:
-            remote, local = v.split(",")
-            map[remote] = local
-        except ValueError:
-            raise click.BadParameter('Extension schema must be a URL and a local file path separated by a comma character')
+            part = v.split(",", 2)
+            map[part[0]] = None if len(part) < 2 and allow_none else part[1]
+        except IndexError:
+            optionally = "optionally " if allow_none else ""
+            raise click.BadParameter(f"Extension schema must be a URL and {optionally}a local file path separated by a comma character")
 
     return map
 
 
 def merge_schemas(*schemas):
     """Merge multiple schemas into one"""
     result = {
```

### Comparing `fiboa_cli-0.3.5/fiboa_cli/validate.py` & `fiboa_cli-0.3.6/fiboa_cli/validate.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,15 +198,15 @@
             valid = False
 
     # Validate whether the Parquet schema complies with the property schemas
     properties = schemas.get("properties", {})
     for key in parquet_schema.names:
         # Ignore fields without a schema
         if key not in properties:
-            log(f"{key}: No schema defined")
+            log(f"{key}: No schema defined", "warning")
             continue
 
         prop_schema = properties[key]
         # Make sure the schema has a data type assigned
         dtype = prop_schema.get("type")
         if dtype is None:
             log(f"{key}: No type specified", "warning")
```

### Comparing `fiboa_cli-0.3.5/fiboa_cli/validate_data.py` & `fiboa_cli-0.3.6/fiboa_cli/validate_data.py`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.5/fiboa_cli/validate_schema.py` & `fiboa_cli-0.3.6/fiboa_cli/validate_schema.py`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.5/fiboa_cli.egg-info/PKG-INFO` & `fiboa_cli-0.3.6/fiboa_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiboa-cli
-Version: 0.3.5
+Version: 0.3.6
 Summary: CLI tools such as validation and file format conversion for fiboa.
 Home-page: https://github.com/fiboa/cli
 Author: Matthias Mohr
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `fiboa_cli-0.3.5/fiboa_cli.egg-info/SOURCES.txt` & `fiboa_cli-0.3.6/fiboa_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.5/setup.py` & `fiboa_cli-0.3.6/setup.py`

 * *Files identical despite different names*

