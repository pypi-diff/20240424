# Comparing `tmp/bio2zarr-0.0.5.tar.gz` & `tmp/bio2zarr-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bio2zarr-0.0.5.tar", last modified: Wed Apr 17 13:16:56 2024, max compression
+gzip compressed data, was "bio2zarr-0.0.6.tar", last modified: Wed Apr 24 11:49:53 2024, max compression
```

## Comparing `bio2zarr-0.0.5.tar` & `bio2zarr-0.0.6.tar`

### file list

```diff
@@ -1,37 +1,51 @@
-drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2024-04-17 13:16:56.277456 bio2zarr-0.0.5/
--rw-r--r--   0 jk        (1000) jk        (1000)     3078 2024-02-14 18:08:29.000000 bio2zarr-0.0.5/.gitignore
--rw-r--r--   0 jk        (1000) jk        (1000)      384 2024-04-17 09:15:58.000000 bio2zarr-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0 jk        (1000) jk        (1000)      947 2024-04-17 13:14:16.000000 bio2zarr-0.0.5/CHANGELOG.md
--rw-r--r--   0 jk        (1000) jk        (1000)    11357 2024-02-14 18:08:29.000000 bio2zarr-0.0.5/LICENSE
--rw-r--r--   0 jk        (1000) jk        (1000)       12 2024-03-27 16:08:22.000000 bio2zarr-0.0.5/MANIFEST.in
--rw-r--r--   0 jk        (1000) jk        (1000)     1076 2024-04-17 13:16:56.277456 bio2zarr-0.0.5/PKG-INFO
--rw-r--r--   0 jk        (1000) jk        (1000)     2916 2024-03-28 11:53:55.000000 bio2zarr-0.0.5/README.md
-drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2024-04-17 13:16:56.273456 bio2zarr-0.0.5/bio2zarr/
--rw-r--r--   0 jk        (1000) jk        (1000)       49 2024-04-17 09:15:58.000000 bio2zarr-0.0.5/bio2zarr/__init__.py
--rw-r--r--   0 jk        (1000) jk        (1000)      527 2024-04-17 09:15:58.000000 bio2zarr-0.0.5/bio2zarr/__main__.py
--rw-r--r--   0 jk        (1000) jk        (1000)      411 2024-04-17 13:16:56.000000 bio2zarr-0.0.5/bio2zarr/_version.py
--rw-r--r--   0 jk        (1000) jk        (1000)    11446 2024-04-17 09:15:58.000000 bio2zarr-0.0.5/bio2zarr/cli.py
--rw-r--r--   0 jk        (1000) jk        (1000)     8127 2024-04-17 09:15:58.000000 bio2zarr-0.0.5/bio2zarr/core.py
--rw-r--r--   0 jk        (1000) jk        (1000)     6768 2024-04-17 09:15:58.000000 bio2zarr-0.0.5/bio2zarr/plink.py
--rw-r--r--   0 jk        (1000) jk        (1000)      142 2024-03-22 09:36:59.000000 bio2zarr-0.0.5/bio2zarr/provenance.py
--rw-r--r--   0 jk        (1000) jk        (1000)       79 2024-04-17 09:15:58.000000 bio2zarr-0.0.5/bio2zarr/typing.py
--rw-r--r--   0 jk        (1000) jk        (1000)    74324 2024-04-17 09:15:58.000000 bio2zarr-0.0.5/bio2zarr/vcf.py
--rw-r--r--   0 jk        (1000) jk        (1000)    17307 2024-04-17 13:14:09.000000 bio2zarr-0.0.5/bio2zarr/vcf_utils.py
-drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2024-04-17 13:16:56.277456 bio2zarr-0.0.5/bio2zarr.egg-info/
--rw-r--r--   0 jk        (1000) jk        (1000)     1076 2024-04-17 13:16:56.000000 bio2zarr-0.0.5/bio2zarr.egg-info/PKG-INFO
--rw-r--r--   0 jk        (1000) jk        (1000)      640 2024-04-17 13:16:56.000000 bio2zarr-0.0.5/bio2zarr.egg-info/SOURCES.txt
--rw-r--r--   0 jk        (1000) jk        (1000)        1 2024-04-17 13:16:56.000000 bio2zarr-0.0.5/bio2zarr.egg-info/dependency_links.txt
--rw-r--r--   0 jk        (1000) jk        (1000)      131 2024-04-17 13:16:56.000000 bio2zarr-0.0.5/bio2zarr.egg-info/entry_points.txt
--rw-r--r--   0 jk        (1000) jk        (1000)        1 2024-03-06 15:57:50.000000 bio2zarr-0.0.5/bio2zarr.egg-info/not-zip-safe
--rw-r--r--   0 jk        (1000) jk        (1000)       69 2024-04-17 13:16:56.000000 bio2zarr-0.0.5/bio2zarr.egg-info/requires.txt
--rw-r--r--   0 jk        (1000) jk        (1000)        9 2024-04-17 13:16:56.000000 bio2zarr-0.0.5/bio2zarr.egg-info/top_level.txt
--rw-r--r--   0 jk        (1000) jk        (1000)      305 2024-04-17 09:15:58.000000 bio2zarr-0.0.5/pyproject.toml
-drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2024-04-17 13:16:56.277456 bio2zarr-0.0.5/requirements/
--rw-r--r--   0 jk        (1000) jk        (1000)      105 2024-04-08 12:31:57.000000 bio2zarr-0.0.5/requirements/development.txt
--rw-r--r--   0 jk        (1000) jk        (1000)     1674 2024-04-17 13:16:56.277456 bio2zarr-0.0.5/setup.cfg
--rw-r--r--   0 jk        (1000) jk        (1000)      311 2024-02-26 14:12:59.000000 bio2zarr-0.0.5/setup.py
-drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2024-04-17 13:16:56.277456 bio2zarr-0.0.5/validation-data/
--rw-r--r--   0 jk        (1000) jk        (1000)     2985 2024-02-29 11:43:51.000000 bio2zarr-0.0.5/validation-data/Makefile
--rwxr-xr-x   0 jk        (1000) jk        (1000)      323 2024-02-29 11:43:51.000000 bio2zarr-0.0.5/validation-data/split.sh
--rw-r--r--   0 jk        (1000) jk        (1000)     2323 2024-04-17 09:15:58.000000 bio2zarr-0.0.5/validation.py
--rw-r--r--   0 jk        (1000) jk        (1000)      959 2024-04-17 09:17:44.000000 bio2zarr-0.0.5/vcf_generator.py
+drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2024-04-24 11:49:53.393730 bio2zarr-0.0.6/
+drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2024-04-24 11:49:53.381729 bio2zarr-0.0.6/.github/
+drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2024-04-24 11:49:53.385730 bio2zarr-0.0.6/.github/workflows/
+-rw-r--r--   0 jk        (1000) jk        (1000)     1181 2024-04-24 11:39:12.000000 bio2zarr-0.0.6/.github/workflows/docs.yml
+-rw-r--r--   0 jk        (1000) jk        (1000)      299 2024-04-19 14:35:26.000000 bio2zarr-0.0.6/.github/workflows/lint.yml
+-rw-r--r--   0 jk        (1000) jk        (1000)     3078 2024-02-14 18:08:29.000000 bio2zarr-0.0.6/.gitignore
+-rw-r--r--   0 jk        (1000) jk        (1000)      384 2024-04-17 09:15:58.000000 bio2zarr-0.0.6/.pre-commit-config.yaml
+-rw-r--r--   0 jk        (1000) jk        (1000)     1089 2024-04-24 11:39:37.000000 bio2zarr-0.0.6/CHANGELOG.md
+-rw-r--r--   0 jk        (1000) jk        (1000)    11357 2024-02-14 18:08:29.000000 bio2zarr-0.0.6/LICENSE
+-rw-r--r--   0 jk        (1000) jk        (1000)       12 2024-03-27 16:08:22.000000 bio2zarr-0.0.6/MANIFEST.in
+-rw-r--r--   0 jk        (1000) jk        (1000)     1076 2024-04-24 11:49:53.393730 bio2zarr-0.0.6/PKG-INFO
+-rw-r--r--   0 jk        (1000) jk        (1000)     2916 2024-03-28 11:53:55.000000 bio2zarr-0.0.6/README.md
+drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2024-04-24 11:49:53.389730 bio2zarr-0.0.6/bio2zarr/
+-rw-r--r--   0 jk        (1000) jk        (1000)       49 2024-04-17 09:15:58.000000 bio2zarr-0.0.6/bio2zarr/__init__.py
+-rw-r--r--   0 jk        (1000) jk        (1000)      527 2024-04-17 09:15:58.000000 bio2zarr-0.0.6/bio2zarr/__main__.py
+-rw-r--r--   0 jk        (1000) jk        (1000)      411 2024-04-24 11:49:53.000000 bio2zarr-0.0.6/bio2zarr/_version.py
+-rw-r--r--   0 jk        (1000) jk        (1000)    14397 2024-04-24 11:39:37.000000 bio2zarr-0.0.6/bio2zarr/cli.py
+-rw-r--r--   0 jk        (1000) jk        (1000)     8516 2024-04-24 11:39:37.000000 bio2zarr-0.0.6/bio2zarr/core.py
+-rw-r--r--   0 jk        (1000) jk        (1000)     6768 2024-04-17 09:15:58.000000 bio2zarr-0.0.6/bio2zarr/plink.py
+-rw-r--r--   0 jk        (1000) jk        (1000)      142 2024-03-22 09:36:59.000000 bio2zarr-0.0.6/bio2zarr/provenance.py
+-rw-r--r--   0 jk        (1000) jk        (1000)       79 2024-04-17 09:15:58.000000 bio2zarr-0.0.6/bio2zarr/typing.py
+-rw-r--r--   0 jk        (1000) jk        (1000)    83330 2024-04-24 11:39:37.000000 bio2zarr-0.0.6/bio2zarr/vcf.py
+-rw-r--r--   0 jk        (1000) jk        (1000)    17307 2024-04-17 13:14:09.000000 bio2zarr-0.0.6/bio2zarr/vcf_utils.py
+drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2024-04-24 11:49:53.389730 bio2zarr-0.0.6/bio2zarr.egg-info/
+-rw-r--r--   0 jk        (1000) jk        (1000)     1076 2024-04-24 11:49:53.000000 bio2zarr-0.0.6/bio2zarr.egg-info/PKG-INFO
+-rw-r--r--   0 jk        (1000) jk        (1000)      835 2024-04-24 11:49:53.000000 bio2zarr-0.0.6/bio2zarr.egg-info/SOURCES.txt
+-rw-r--r--   0 jk        (1000) jk        (1000)        1 2024-04-24 11:49:53.000000 bio2zarr-0.0.6/bio2zarr.egg-info/dependency_links.txt
+-rw-r--r--   0 jk        (1000) jk        (1000)      131 2024-04-24 11:49:53.000000 bio2zarr-0.0.6/bio2zarr.egg-info/entry_points.txt
+-rw-r--r--   0 jk        (1000) jk        (1000)        1 2024-03-06 15:57:50.000000 bio2zarr-0.0.6/bio2zarr.egg-info/not-zip-safe
+-rw-r--r--   0 jk        (1000) jk        (1000)       69 2024-04-24 11:49:53.000000 bio2zarr-0.0.6/bio2zarr.egg-info/requires.txt
+-rw-r--r--   0 jk        (1000) jk        (1000)        9 2024-04-24 11:49:53.000000 bio2zarr-0.0.6/bio2zarr.egg-info/top_level.txt
+drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2024-04-24 11:49:53.389730 bio2zarr-0.0.6/docs/
+-rw-r--r--   0 jk        (1000) jk        (1000)      489 2024-04-19 14:33:24.000000 bio2zarr-0.0.6/docs/Makefile
+-rw-r--r--   0 jk        (1000) jk        (1000)     1041 2024-04-19 14:33:24.000000 bio2zarr-0.0.6/docs/_config.yml
+-rw-r--r--   0 jk        (1000) jk        (1000)       50 2024-04-19 14:33:24.000000 bio2zarr-0.0.6/docs/_toc.yml
+-rwxr-xr-x   0 jk        (1000) jk        (1000)      505 2024-04-19 14:33:24.000000 bio2zarr-0.0.6/docs/build.sh
+-rw-r--r--   0 jk        (1000) jk        (1000)      182 2024-04-19 14:33:24.000000 bio2zarr-0.0.6/docs/cli.md
+-rw-r--r--   0 jk        (1000) jk        (1000)     1947 2024-04-19 14:33:24.000000 bio2zarr-0.0.6/docs/intro.md
+-rw-r--r--   0 jk        (1000) jk        (1000)   107441 2024-04-19 14:33:24.000000 bio2zarr-0.0.6/docs/logo.png
+-rw-r--r--   0 jk        (1000) jk        (1000)        9 2024-04-19 14:33:24.000000 bio2zarr-0.0.6/docs/references.bib
+-rw-r--r--   0 jk        (1000) jk        (1000)       94 2024-04-19 14:51:51.000000 bio2zarr-0.0.6/docs/requirements.txt
+-rw-r--r--   0 jk        (1000) jk        (1000)      305 2024-04-17 09:15:58.000000 bio2zarr-0.0.6/pyproject.toml
+drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2024-04-24 11:49:53.389730 bio2zarr-0.0.6/requirements/
+-rw-r--r--   0 jk        (1000) jk        (1000)      105 2024-04-08 12:31:57.000000 bio2zarr-0.0.6/requirements/development.txt
+-rw-r--r--   0 jk        (1000) jk        (1000)     1674 2024-04-24 11:49:53.393730 bio2zarr-0.0.6/setup.cfg
+-rw-r--r--   0 jk        (1000) jk        (1000)      311 2024-02-26 14:12:59.000000 bio2zarr-0.0.6/setup.py
+drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2024-04-24 11:49:53.389730 bio2zarr-0.0.6/validation-data/
+-rw-r--r--   0 jk        (1000) jk        (1000)     2985 2024-02-29 11:43:51.000000 bio2zarr-0.0.6/validation-data/Makefile
+-rwxr-xr-x   0 jk        (1000) jk        (1000)      323 2024-02-29 11:43:51.000000 bio2zarr-0.0.6/validation-data/split.sh
+-rw-r--r--   0 jk        (1000) jk        (1000)     2323 2024-04-17 09:15:58.000000 bio2zarr-0.0.6/validation.py
+-rw-r--r--   0 jk        (1000) jk        (1000)      959 2024-04-17 09:17:44.000000 bio2zarr-0.0.6/vcf_generator.py
```

### Comparing `bio2zarr-0.0.5/.gitignore` & `bio2zarr-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `bio2zarr-0.0.5/CHANGELOG.md` & `bio2zarr-0.0.6/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# 0.0.6 2024-04-24
+
+- Only use NOSHUFFLE by default on ``call_genotype`` and bool arrays.
+- Add initial implementation of distributed encode
+
 # 0.0.5 2024-04-17
 
 - Fix bug in schema handling (compressor settings ignored)
 - Move making ICF field partition directories into per-partition processing.
   Remove progress on the init mkdirs step.
 - Turn off progress monitor on dexplode-partition
 - Fix empty partition bug
```

### Comparing `bio2zarr-0.0.5/LICENSE` & `bio2zarr-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bio2zarr-0.0.5/PKG-INFO` & `bio2zarr-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bio2zarr
-Version: 0.0.5
+Version: 0.0.6
 Summary: Convert bioinformatics data to Zarr
 Home-page: https://github.com/pystatgen/bio2zarr
 Author: sgkit Developers
 Author-email: project@pystatgen.org
 License: Apache
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `bio2zarr-0.0.5/README.md` & `bio2zarr-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `bio2zarr-0.0.5/bio2zarr/__main__.py` & `bio2zarr-0.0.6/bio2zarr/__main__.py`

 * *Files identical despite different names*

### Comparing `bio2zarr-0.0.5/bio2zarr/cli.py` & `bio2zarr-0.0.6/bio2zarr/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 import os
 import pathlib
 import shutil
 
 import click
 import coloredlogs
+import humanfriendly
 import numcodecs
 import tabulate
 
 from . import plink, provenance, vcf, vcf_utils
 
 logger = logging.getLogger(__name__)
 
@@ -35,14 +36,22 @@
     "icf_path", type=click.Path(exists=True, file_okay=False, dir_okay=True)
 )
 
 new_zarr_path = click.argument(
     "zarr_path", type=click.Path(file_okay=False, dir_okay=True)
 )
 
+zarr_path = click.argument(
+    "zarr_path", type=click.Path(exists=True, file_okay=False, dir_okay=True)
+)
+
+num_partitions = click.argument("num_partitions", type=click.IntRange(min=1))
+
+partition = click.argument("partition", type=click.IntRange(min=0))
+
 verbose = click.option("-v", "--verbose", count=True, help="Increase verbosity")
 
 force = click.option(
     "-f",
     "--force",
     is_flag=True,
     flag_value=True,
@@ -88,14 +97,35 @@
     "-w",
     "--samples-chunk-size",
     type=int,
     default=None,
     help="Chunk size in the samples dimension",
 )
 
+schema = click.option("-s", "--schema", default=None, type=click.Path(exists=True))
+
+max_variant_chunks = click.option(
+    "-V",
+    "--max-variant-chunks",
+    type=int,
+    default=None,
+    help=(
+        "Truncate the output in the variants dimension to have "
+        "this number of chunks. Mainly intended to help with "
+        "schema tuning."
+    ),
+)
+
+max_memory = click.option(
+    "-M",
+    "--max-memory",
+    default=None,
+    help="An approximate bound on overall memory usage (e.g. 10G),",
+)
+
 
 def setup_logging(verbosity):
     level = "WARNING"
     if verbosity == 1:
         level = "INFO"
     elif verbosity >= 2:
         level = "DEBUG"
@@ -154,15 +184,15 @@
         show_progress=True,
     )
 
 
 @click.command
 @vcfs
 @new_icf_path
-@click.argument("num_partitions", type=click.IntRange(min=1))
+@num_partitions
 @force
 @column_chunk_size
 @compressor
 @verbose
 @worker_processes
 def dexplode_init(
     vcfs,
@@ -190,35 +220,35 @@
         show_progress=True,
     )
     click.echo(num_partitions)
 
 
 @click.command
 @icf_path
-@click.argument("partition", type=click.IntRange(min=0))
+@partition
 @verbose
 def dexplode_partition(icf_path, partition, verbose):
     """
     Convert a VCF partition to intermediate columnar format. Must be called *after*
     the ICF path has been initialised with dexplode_init. Partition indexes must be
     from 0 (inclusive) to the number of paritions returned by dexplode_init (exclusive).
     """
     setup_logging(verbose)
     vcf.explode_partition(icf_path, partition, show_progress=False)
 
 
 @click.command
-@click.argument("path", type=click.Path(), required=True)
+@icf_path
 @verbose
-def dexplode_finalise(path, verbose):
+def dexplode_finalise(icf_path, verbose):
     """
     Final step for distributed conversion of VCF(s) to intermediate columnar format.
     """
     setup_logging(verbose)
-    vcf.explode_finalise(path)
+    vcf.explode_finalise(icf_path)
 
 
 @click.command
 @click.argument("path", type=click.Path())
 @verbose
 def inspect(path, verbose):
     """
@@ -240,34 +270,19 @@
 
 
 @click.command
 @icf_path
 @new_zarr_path
 @force
 @verbose
-@click.option("-s", "--schema", default=None, type=click.Path(exists=True))
+@schema
 @variants_chunk_size
 @samples_chunk_size
-@click.option(
-    "-V",
-    "--max-variant-chunks",
-    type=int,
-    default=None,
-    help=(
-        "Truncate the output in the variants dimension to have "
-        "this number of chunks. Mainly intended to help with "
-        "schema tuning."
-    ),
-)
-@click.option(
-    "-M",
-    "--max-memory",
-    default=None,
-    help="An approximate bound on overall memory usage (e.g. 10G),",
-)
+@max_variant_chunks
+@max_memory
 @worker_processes
 def encode(
     icf_path,
     zarr_path,
     force,
     verbose,
     schema,
@@ -284,21 +299,104 @@
     check_overwrite_dir(zarr_path, force)
     vcf.encode(
         icf_path,
         zarr_path,
         schema_path=schema,
         variants_chunk_size=variants_chunk_size,
         samples_chunk_size=samples_chunk_size,
-        max_v_chunks=max_variant_chunks,
+        max_variant_chunks=max_variant_chunks,
         worker_processes=worker_processes,
         max_memory=max_memory,
         show_progress=True,
     )
 
 
+@click.command
+@icf_path
+@new_zarr_path
+@num_partitions
+@force
+@schema
+@variants_chunk_size
+@samples_chunk_size
+@max_variant_chunks
+@verbose
+def dencode_init(
+    icf_path,
+    zarr_path,
+    num_partitions,
+    force,
+    schema,
+    variants_chunk_size,
+    samples_chunk_size,
+    max_variant_chunks,
+    verbose,
+):
+    """
+    Initialise conversion of intermediate format to VCF Zarr. This will
+    set up the specified ZARR_PATH to perform this conversion over
+    NUM_PARTITIONS.
+
+    The output of this commmand is the actual number of partitions generated
+    (which may be less then the requested number, if there is not sufficient
+    chunks in the variants dimension) and a rough lower-bound on the amount
+    of memory required to encode a partition.
+
+    NOTE: the format of this output will likely change in subsequent releases;
+    it should not be considered machine-readable for now.
+    """
+    setup_logging(verbose)
+    check_overwrite_dir(zarr_path, force)
+    num_partitions, max_memory = vcf.encode_init(
+        icf_path,
+        zarr_path,
+        target_num_partitions=num_partitions,
+        schema_path=schema,
+        variants_chunk_size=variants_chunk_size,
+        samples_chunk_size=samples_chunk_size,
+        max_variant_chunks=max_variant_chunks,
+        show_progress=True,
+    )
+    formatted_size = humanfriendly.format_size(max_memory, binary=True)
+    # NOTE adding the size to the stdout here so that users can parse it
+    # and use in their submission scripts. This is a first pass, and
+    # will most likely change as we see what works and doesn't.
+    # NOTE we probably want to format this as a table, which lists
+    # some other properties, line by line
+    # NOTE This size number is also not quite enough, you need a bit of
+    # headroom with it (probably 10% or so). We should include this.
+    click.echo(f"{num_partitions}\t{formatted_size}")
+
+
+@click.command
+@zarr_path
+@partition
+@verbose
+def dencode_partition(zarr_path, partition, verbose):
+    """
+    Convert a partition from intermediate columnar format to VCF Zarr.
+    Must be called *after* the Zarr path has been initialised with dencode_init.
+    Partition indexes must be from 0 (inclusive) to the number of paritions
+    returned by dencode_init (exclusive).
+    """
+    setup_logging(verbose)
+    vcf.encode_partition(zarr_path, partition)
+
+
+@click.command
+@zarr_path
+@verbose
+def dencode_finalise(zarr_path, verbose):
+    """
+    Final step for distributed conversion of ICF to VCF Zarr.
+    """
+    setup_logging(verbose)
+    vcf.encode_finalise(zarr_path, show_progress=True)
+
+
 @click.command(name="convert")
 @vcfs
 @new_zarr_path
 @variants_chunk_size
 @samples_chunk_size
 @verbose
 @worker_processes
@@ -378,14 +476,17 @@
 vcf2zarr.add_command(inspect)
 vcf2zarr.add_command(explode)
 vcf2zarr.add_command(mkschema)
 vcf2zarr.add_command(encode)
 vcf2zarr.add_command(dexplode_init)
 vcf2zarr.add_command(dexplode_partition)
 vcf2zarr.add_command(dexplode_finalise)
+vcf2zarr.add_command(dencode_init)
+vcf2zarr.add_command(dencode_partition)
+vcf2zarr.add_command(dencode_finalise)
 
 
 @click.command(name="convert")
 @click.argument("in_path", type=click.Path())
 @click.argument("zarr_path", type=click.Path())
 @worker_processes
 @verbose
```

### Comparing `bio2zarr-0.0.5/bio2zarr/core.py` & `bio2zarr-0.0.6/bio2zarr/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,24 @@
 import zarr
 
 logger = logging.getLogger(__name__)
 
 numcodecs.blosc.use_threads = False
 
 
+def min_int_dtype(min_value, max_value):
+    if min_value > max_value:
+        raise ValueError("min_value must be <= max_value")
+    for a_dtype in ["i1", "i2", "i4", "i8"]:
+        info = np.iinfo(a_dtype)
+        if info.min <= min_value and max_value <= info.max:
+            return a_dtype
+    raise OverflowError("Integer cannot be represented")
+
+
 def chunk_aligned_slices(z, n, max_chunks=None):
     """
     Returns at n slices in the specified zarr array, aligned
     with its chunks
     """
     chunk_size = z.chunks[0]
     num_chunks = int(np.ceil(z.shape[0] / chunk_size))
@@ -96,14 +106,15 @@
                 sync_flush_1d_array(
                     self.buff[: self.buffer_row], self.array, self.array_offset
                 )
             else:
                 sync_flush_2d_array(
                     self.buff[: self.buffer_row], self.array, self.array_offset
                 )
+            # FIXME the array.name doesn't seem to be working here for some reason
             logger.debug(
                 f"Flushed <{self.array.name} {self.array.shape} "
                 f"{self.array.dtype}> "
                 f"{self.array_offset}:{self.array_offset + self.buffer_row}"
                 f"{self.buff.nbytes / 2**20: .2f}Mb"
             )
             self.array_offset += self.variants_chunk_size
@@ -117,16 +128,15 @@
 
 def sync_flush_2d_array(np_buffer, zarr_array, offset):
     # Write chunks in the second dimension 1-by-1 to make progress more
     # incremental, and to avoid large memcopies in the underlying
     # encoder implementations.
     s = slice(offset, offset + np_buffer.shape[0])
     samples_chunk_size = zarr_array.chunks[1]
-    # TODO use zarr chunks here to support non-uniform chunking later
-    # and for simplicity
+    # TODO use zarr chunks here for simplicity
     zarr_array_width = zarr_array.shape[1]
     start = 0
     while start < zarr_array_width:
         stop = min(start + samples_chunk_size, zarr_array_width)
         chunk_buffer = np_buffer[:, start:stop]
         zarr_array[s, start:stop] = chunk_buffer
         update_progress(chunk_buffer.nbytes)
@@ -178,15 +188,15 @@
 
         set_progress(0)
         if progress_config is None:
             progress_config = ProgressConfig()
         self.progress_config = progress_config
         self.progress_bar = tqdm.tqdm(
             total=progress_config.total,
-            desc=f"{progress_config.title:>7}",
+            desc=f"{progress_config.title:>8}",
             unit_scale=True,
             unit=progress_config.units,
             smoothing=0.1,
             disable=not progress_config.show,
         )
         self.completed = False
         self.completed_lock = threading.Lock()
```

### Comparing `bio2zarr-0.0.5/bio2zarr/plink.py` & `bio2zarr-0.0.6/bio2zarr/plink.py`

 * *Files identical despite different names*

### Comparing `bio2zarr-0.0.5/bio2zarr/vcf.py` & `bio2zarr-0.0.6/bio2zarr/vcf.py`

 * *Files 8% similar despite different names*

```diff
@@ -107,33 +107,30 @@
 
     @property
     def full_name(self):
         if self.category == "fixed":
             return self.name
         return f"{self.category}/{self.name}"
 
-    # TODO add method here to choose a good set compressor and
-    # filters default here for this field.
-
     def smallest_dtype(self):
         """
         Returns the smallest dtype suitable for this field based
         on type, and values.
         """
         s = self.summary
         if self.vcf_type == "Float":
             ret = "f4"
         elif self.vcf_type == "Integer":
-            dtype = "i4"
-            for a_dtype in ["i1", "i2"]:
-                info = np.iinfo(a_dtype)
-                if info.min <= s.min_value and s.max_value <= info.max:
-                    dtype = a_dtype
-                    break
-            ret = dtype
+            if not math.isfinite(s.max_value):
+                # All missing values; use i1. Note we should have some API to
+                # check more explicitly for missingness:
+                # https://github.com/sgkit-dev/bio2zarr/issues/131
+                ret = "i1"
+            else:
+                ret = core.min_int_dtype(s.min_value, s.max_value)
         elif self.vcf_type == "Flag":
             ret = "bool"
         elif self.vcf_type == "Character":
             ret = "U1"
         else:
             assert self.vcf_type == "String"
             ret = "O"
@@ -148,14 +145,18 @@
 
 
 ICF_METADATA_FORMAT_VERSION = "0.2"
 ICF_DEFAULT_COMPRESSOR = numcodecs.Blosc(
     cname="zstd", clevel=7, shuffle=numcodecs.Blosc.NOSHUFFLE
 )
 
+# TODO refactor this to have embedded Contig dataclass, Filters
+# and Samples dataclasses to allow for more information to be
+# retained and forward compatibility.
+
 
 @dataclasses.dataclass
 class IcfMetadata:
     samples: list
     contig_names: list
     contig_record_counts: dict
     filters: list
@@ -180,14 +181,22 @@
         fields = []
         for field in self.fields:
             if field.category == "FORMAT":
                 fields.append(field)
         return fields
 
     @property
+    def num_contigs(self):
+        return len(self.contig_names)
+
+    @property
+    def num_filters(self):
+        return len(self.filters)
+
+    @property
     def num_records(self):
         return sum(self.contig_record_counts.values())
 
     @staticmethod
     def fromdict(d):
         if d["format_version"] != ICF_METADATA_FORMAT_VERSION:
             raise ValueError(
@@ -1238,33 +1247,92 @@
     def new(**kwargs):
         spec = ZarrColumnSpec(
             **kwargs, compressor=DEFAULT_ZARR_COMPRESSOR.get_config(), filters=[]
         )
         spec._choose_compressor_settings()
         return spec
 
+    @staticmethod
+    def from_field(
+        vcf_field,
+        *,
+        num_variants,
+        num_samples,
+        variants_chunk_size,
+        samples_chunk_size,
+        variable_name=None,
+    ):
+        shape = [num_variants]
+        prefix = "variant_"
+        dimensions = ["variants"]
+        chunks = [variants_chunk_size]
+        if vcf_field.category == "FORMAT":
+            prefix = "call_"
+            shape.append(num_samples)
+            chunks.append(samples_chunk_size)
+            dimensions.append("samples")
+        if variable_name is None:
+            variable_name = prefix + vcf_field.name
+        # TODO make an option to add in the empty extra dimension
+        if vcf_field.summary.max_number > 1:
+            shape.append(vcf_field.summary.max_number)
+            # TODO we should really be checking this to see if the named dimensions
+            # are actually correct.
+            if vcf_field.vcf_number == "R":
+                dimensions.append("alleles")
+            elif vcf_field.vcf_number == "A":
+                dimensions.append("alt_alleles")
+            elif vcf_field.vcf_number == "G":
+                dimensions.append("genotypes")
+            else:
+                dimensions.append(f"{vcf_field.category}_{vcf_field.name}_dim")
+        return ZarrColumnSpec.new(
+            vcf_field=vcf_field.full_name,
+            name=variable_name,
+            dtype=vcf_field.smallest_dtype(),
+            shape=shape,
+            chunks=chunks,
+            dimensions=dimensions,
+            description=vcf_field.description,
+        )
+
     def _choose_compressor_settings(self):
         """
         Choose compressor and filter settings based on the size and
         type of the array, plus some hueristics from observed properties
         of VCFs.
 
         See https://github.com/pystatgen/bio2zarr/discussions/74
         """
-        dt = np.dtype(self.dtype)
         # Default is to not shuffle, because autoshuffle isn't recognised
         # by many Zarr implementations, and shuffling can lead to worse
         # performance in some cases anyway. Turning on shuffle should be a
         # deliberate choice.
         shuffle = numcodecs.Blosc.NOSHUFFLE
-        if dt.itemsize == 1:
-            # Any 1 byte field gets BITSHUFFLE by default
+        if self.name == "call_genotype" and self.dtype == "i1":
+            # call_genotype gets BITSHUFFLE by default as it gets
+            # significantly better compression (at a cost of slower
+            # decoding)
             shuffle = numcodecs.Blosc.BITSHUFFLE
+        elif self.dtype == "bool":
+            shuffle = numcodecs.Blosc.BITSHUFFLE
+
         self.compressor["shuffle"] = shuffle
 
+    @property
+    def variant_chunk_nbytes(self):
+        """
+        Returns the nbytes for a single variant chunk of this array.
+        """
+        chunk_items = self.chunks[0]
+        for size in self.shape[1:]:
+            chunk_items *= size
+        dt = np.dtype(self.dtype)
+        return chunk_items * dt.itemsize
+
 
 ZARR_SCHEMA_FORMAT_VERSION = "0.2"
 
 
 @dataclasses.dataclass
 class VcfZarrSchema:
     format_version: str
@@ -1309,14 +1377,24 @@
             samples_chunk_size = 1000
         if variants_chunk_size is None:
             variants_chunk_size = 10_000
         logger.info(
             f"Generating schema with chunks={variants_chunk_size, samples_chunk_size}"
         )
 
+        def spec_from_field(field, variable_name=None):
+            return ZarrColumnSpec.from_field(
+                field,
+                num_samples=n,
+                num_variants=m,
+                samples_chunk_size=samples_chunk_size,
+                variants_chunk_size=variants_chunk_size,
+                variable_name=variable_name,
+            )
+
         def fixed_field_spec(
             name, dtype, vcf_field=None, shape=(m,), dimensions=("variants",)
         ):
             return ZarrColumnSpec.new(
                 vcf_field=vcf_field,
                 name=name,
                 dtype=dtype,
@@ -1324,103 +1402,64 @@
                 description="",
                 dimensions=dimensions,
                 chunks=[variants_chunk_size],
             )
 
         alt_col = icf.columns["ALT"]
         max_alleles = alt_col.vcf_field.summary.max_number + 1
-        num_filters = len(icf.metadata.filters)
 
-        # # FIXME get dtype from lookup table
         colspecs = [
             fixed_field_spec(
                 name="variant_contig",
-                dtype="i2",  # FIXME
+                dtype=core.min_int_dtype(0, icf.metadata.num_contigs),
             ),
             fixed_field_spec(
                 name="variant_filter",
                 dtype="bool",
-                shape=(m, num_filters),
+                shape=(m, icf.metadata.num_filters),
                 dimensions=["variants", "filters"],
             ),
             fixed_field_spec(
                 name="variant_allele",
                 dtype="str",
-                shape=[m, max_alleles],
+                shape=(m, max_alleles),
                 dimensions=["variants", "alleles"],
             ),
             fixed_field_spec(
-                vcf_field="POS",
-                name="variant_position",
-                dtype="i4",
-            ),
-            fixed_field_spec(
-                vcf_field=None,
                 name="variant_id",
                 dtype="str",
             ),
             fixed_field_spec(
-                vcf_field=None,
                 name="variant_id_mask",
                 dtype="bool",
             ),
-            fixed_field_spec(
-                vcf_field="QUAL",
-                name="variant_quality",
-                dtype="f4",
-            ),
         ]
+        name_map = {field.full_name: field for field in icf.metadata.fields}
+
+        # Only two of the fixed fields have a direct one-to-one mapping.
+        colspecs.extend(
+            [
+                spec_from_field(name_map["QUAL"], variable_name="variant_quality"),
+                spec_from_field(name_map["POS"], variable_name="variant_position"),
+            ]
+        )
+        colspecs.extend([spec_from_field(field) for field in icf.metadata.info_fields])
 
         gt_field = None
-        for field in icf.metadata.fields:
-            if field.category == "fixed":
-                continue
+        for field in icf.metadata.format_fields:
             if field.name == "GT":
                 gt_field = field
                 continue
-            shape = [m]
-            prefix = "variant_"
-            dimensions = ["variants"]
-            chunks = [variants_chunk_size]
-            if field.category == "FORMAT":
-                prefix = "call_"
-                shape.append(n)
-                chunks.append(samples_chunk_size)
-                dimensions.append("samples")
-            # TODO make an option to add in the empty extra dimension
-            if field.summary.max_number > 1:
-                shape.append(field.summary.max_number)
-                # TODO we should really be checking this to see if the named dimensions
-                # are actually correct.
-                if field.vcf_number == "R":
-                    dimensions.append("alleles")
-                elif field.vcf_number == "A":
-                    dimensions.append("alt_alleles")
-                elif field.vcf_number == "G":
-                    dimensions.append("genotypes")
-                else:
-                    dimensions.append(f"{field.category}_{field.name}_dim")
-            variable_name = prefix + field.name
-            colspec = ZarrColumnSpec.new(
-                vcf_field=field.full_name,
-                name=variable_name,
-                dtype=field.smallest_dtype(),
-                shape=shape,
-                chunks=chunks,
-                dimensions=dimensions,
-                description=field.description,
-            )
-            colspecs.append(colspec)
+            colspecs.append(spec_from_field(field))
 
         if gt_field is not None:
             ploidy = gt_field.summary.max_number - 1
             shape = [m, n]
             chunks = [variants_chunk_size, samples_chunk_size]
             dimensions = ["variants", "samples"]
-
             colspecs.append(
                 ZarrColumnSpec.new(
                     vcf_field=None,
                     name="call_genotype_phased",
                     dtype="bool",
                     shape=list(shape),
                     chunks=list(chunks),
@@ -1494,401 +1533,595 @@
                 "compressor": str(array.compressor),
                 "filters": str(array.filters),
             }
             data.append(d)
         return data
 
 
-@dataclasses.dataclass
-class EncodingWork:
-    func: callable = dataclasses.field(repr=False)
-    start: int
-    stop: int
-    columns: list[str]
-    memory: int = 0
-
-
 def parse_max_memory(max_memory):
     if max_memory is None:
         # Effectively unbounded
         return 2**63
     if isinstance(max_memory, str):
         max_memory = humanfriendly.parse_size(max_memory)
     logger.info(f"Set memory budget to {display_size(max_memory)}")
     return max_memory
 
 
+@dataclasses.dataclass
+class VcfZarrPartition:
+    start_index: int
+    stop_index: int
+    start_chunk: int
+    stop_chunk: int
+
+    @staticmethod
+    def generate_partitions(num_records, chunk_size, num_partitions, max_chunks=None):
+        num_chunks = int(np.ceil(num_records / chunk_size))
+        if max_chunks is not None:
+            num_chunks = min(num_chunks, max_chunks)
+        partitions = []
+        splits = np.array_split(np.arange(num_chunks), min(num_partitions, num_chunks))
+        for chunk_slice in splits:
+            start_chunk = int(chunk_slice[0])
+            stop_chunk = int(chunk_slice[-1]) + 1
+            start_index = start_chunk * chunk_size
+            stop_index = min(stop_chunk * chunk_size, num_records)
+            partitions.append(
+                VcfZarrPartition(start_index, stop_index, start_chunk, stop_chunk)
+            )
+        return partitions
+
+
+VZW_METADATA_FORMAT_VERSION = "0.1"
+
+
+@dataclasses.dataclass
+class VcfZarrWriterMetadata:
+    format_version: str
+    icf_path: str
+    schema: VcfZarrSchema
+    dimension_separator: str
+    partitions: list
+    provenance: dict
+
+    def asdict(self):
+        return dataclasses.asdict(self)
+
+    @staticmethod
+    def fromdict(d):
+        if d["format_version"] != VZW_METADATA_FORMAT_VERSION:
+            raise ValueError(
+                "VcfZarrWriter  format version mismatch: "
+                f"{d['format_version']} != {VZW_METADATA_FORMAT_VERSION}"
+            )
+        ret = VcfZarrWriterMetadata(**d)
+        ret.schema = VcfZarrSchema.fromdict(ret.schema)
+        ret.partitions = [VcfZarrPartition(**p) for p in ret.partitions]
+        return ret
+
+
 class VcfZarrWriter:
-    def __init__(self, path, icf, schema, dimension_separator=None):
+    def __init__(self, path):
         self.path = pathlib.Path(path)
+        self.wip_path = self.path / "wip"
+        self.arrays_path = self.wip_path / "arrays"
+        self.partitions_path = self.wip_path / "partitions"
+        self.metadata = None
+        self.icf = None
+
+    @property
+    def schema(self):
+        return self.metadata.schema
+
+    @property
+    def num_partitions(self):
+        return len(self.metadata.partitions)
+
+    #######################
+    # init
+    #######################
+
+    def init(
+        self,
+        icf,
+        *,
+        target_num_partitions,
+        schema,
+        dimension_separator=None,
+        max_variant_chunks=None,
+    ):
         self.icf = icf
-        self.schema = schema
+        if self.path.exists():
+            raise ValueError("Zarr path already exists")  # NEEDS TEST
+        partitions = VcfZarrPartition.generate_partitions(
+            self.icf.num_records,
+            schema.variants_chunk_size,
+            target_num_partitions,
+            max_chunks=max_variant_chunks,
+        )
         # Default to using nested directories following the Zarr v3 default.
         # This seems to require version 2.17+ to work properly
-        self.dimension_separator = (
+        dimension_separator = (
             "/" if dimension_separator is None else dimension_separator
         )
+        self.metadata = VcfZarrWriterMetadata(
+            format_version=VZW_METADATA_FORMAT_VERSION,
+            icf_path=str(self.icf.path),
+            schema=schema,
+            dimension_separator=dimension_separator,
+            partitions=partitions,
+            # Bare minimum here for provenance - see comments above
+            provenance={"source": f"bio2zarr-{provenance.__version__}"},
+        )
+
+        self.path.mkdir()
         store = zarr.DirectoryStore(self.path)
-        self.root = zarr.group(store=store)
+        root = zarr.group(store=store)
+        root.attrs.update(
+            {
+                "vcf_zarr_version": "0.2",
+                "vcf_header": self.icf.vcf_header,
+                "source": f"bio2zarr-{provenance.__version__}",
+            }
+        )
+        # Doing this syncronously - this is fine surely
+        self.encode_samples(root)
+        self.encode_filter_id(root)
+        self.encode_contig_id(root)
+
+        self.wip_path.mkdir()
+        self.arrays_path.mkdir()
+        self.partitions_path.mkdir()
+        store = zarr.DirectoryStore(self.arrays_path)
+        root = zarr.group(store=store)
+
+        for column in self.schema.columns.values():
+            self.init_array(root, column, partitions[-1].stop_index)
+
+        logger.info("Writing WIP metadata")
+        with open(self.wip_path / "metadata.json", "w") as f:
+            json.dump(self.metadata.asdict(), f, indent=4)
+        return len(partitions)
+
+    def encode_samples(self, root):
+        if not np.array_equal(self.schema.sample_id, self.icf.metadata.samples):
+            raise ValueError(
+                "Subsetting or reordering samples not supported currently"
+            )  # NEEDS TEST
+        array = root.array(
+            "sample_id",
+            self.schema.sample_id,
+            dtype="str",
+            compressor=DEFAULT_ZARR_COMPRESSOR,
+            chunks=(self.schema.samples_chunk_size,),
+        )
+        array.attrs["_ARRAY_DIMENSIONS"] = ["samples"]
+        logger.debug("Samples done")
 
-    def init_array(self, variable):
+    def encode_contig_id(self, root):
+        array = root.array(
+            "contig_id",
+            self.schema.contig_id,
+            dtype="str",
+            compressor=DEFAULT_ZARR_COMPRESSOR,
+        )
+        array.attrs["_ARRAY_DIMENSIONS"] = ["contigs"]
+        if self.schema.contig_length is not None:
+            array = root.array(
+                "contig_length",
+                self.schema.contig_length,
+                dtype=np.int64,
+                compressor=DEFAULT_ZARR_COMPRESSOR,
+            )
+            array.attrs["_ARRAY_DIMENSIONS"] = ["contigs"]
+
+    def encode_filter_id(self, root):
+        array = root.array(
+            "filter_id",
+            self.schema.filter_id,
+            dtype="str",
+            compressor=DEFAULT_ZARR_COMPRESSOR,
+        )
+        array.attrs["_ARRAY_DIMENSIONS"] = ["filters"]
+
+    def init_array(self, root, variable, variants_dim_size):
         object_codec = None
         if variable.dtype == "O":
             object_codec = numcodecs.VLenUTF8()
-        a = self.root.empty(
-            "wip_" + variable.name,
-            shape=variable.shape,
+        shape = list(variable.shape)
+        # Truncate the variants dimension is max_variant_chunks was specified
+        shape[0] = variants_dim_size
+        a = root.empty(
+            variable.name,
+            shape=shape,
             chunks=variable.chunks,
             dtype=variable.dtype,
             compressor=numcodecs.get_codec(variable.compressor),
             filters=[numcodecs.get_codec(filt) for filt in variable.filters],
             object_codec=object_codec,
-            dimension_separator=self.dimension_separator,
+            dimension_separator=self.metadata.dimension_separator,
+        )
+        a.attrs.update(
+            {
+                "description": variable.description,
+                # Dimension names are part of the spec in Zarr v3
+                "_ARRAY_DIMENSIONS": variable.dimensions,
+            }
         )
-        # Dimension names are part of the spec in Zarr v3
-        a.attrs["_ARRAY_DIMENSIONS"] = variable.dimensions
+        logger.debug(f"Initialised {a}")
 
-    def get_array(self, name):
-        return self.root["wip_" + name]
+    #######################
+    # encode_partition
+    #######################
 
-    def finalise_array(self, variable_name):
-        source = self.path / ("wip_" + variable_name)
-        dest = self.path / variable_name
+    def load_metadata(self):
+        if self.metadata is None:
+            with open(self.wip_path / "metadata.json") as f:
+                self.metadata = VcfZarrWriterMetadata.fromdict(json.load(f))
+            self.icf = IntermediateColumnarFormat(self.metadata.icf_path)
+
+    def partition_path(self, partition_index):
+        return self.partitions_path / f"p{partition_index}"
+
+    def wip_partition_array_path(self, partition_index, name):
+        return self.partition_path(partition_index) / f"wip_{name}"
+
+    def partition_array_path(self, partition_index, name):
+        return self.partition_path(partition_index) / name
+
+    def encode_partition(self, partition_index):
+        self.load_metadata()
+        partition_path = self.partition_path(partition_index)
+        partition_path.mkdir(exist_ok=True)
+        logger.info(f"Encoding partition {partition_index} to {partition_path}")
+
+        self.encode_alleles_partition(partition_index)
+        self.encode_id_partition(partition_index)
+        self.encode_filters_partition(partition_index)
+        self.encode_contig_partition(partition_index)
+        for col in self.schema.columns.values():
+            if col.vcf_field is not None:
+                self.encode_array_partition(col, partition_index)
+        if "call_genotype" in self.schema.columns:
+            self.encode_genotypes_partition(partition_index)
+
+    def init_partition_array(self, partition_index, name):
+        wip_path = self.wip_partition_array_path(partition_index, name)
+        # Create an empty array like the definition
+        src = self.arrays_path / name
+        # Overwrite any existing WIP files
+        shutil.copytree(src, wip_path, dirs_exist_ok=True)
+        array = zarr.open(wip_path)
+        logger.debug(f"Opened empty array {array} @ {wip_path}")
+        return array
+
+    def finalise_partition_array(self, partition_index, name):
+        wip_path = self.wip_partition_array_path(partition_index, name)
+        final_path = self.partition_array_path(partition_index, name)
+        if final_path.exists():
+            # NEEDS TEST
+            logger.warning(f"Removing existing {final_path}")
+            shutil.rmtree(final_path)
         # Atomic swap
-        os.rename(source, dest)
-        logger.info(f"Finalised {variable_name}")
+        os.rename(wip_path, final_path)
+        logger.debug(f"Encoded {name} partition {partition_index}")
+
+    def encode_array_partition(self, column, partition_index):
+        array = self.init_partition_array(partition_index, column.name)
 
-    def encode_array_slice(self, column, start, stop):
+        partition = self.metadata.partitions[partition_index]
+        ba = core.BufferedArray(array, partition.start_index)
         source_col = self.icf.columns[column.vcf_field]
-        array = self.get_array(column.name)
-        ba = core.BufferedArray(array, start)
         sanitiser = source_col.sanitiser_factory(ba.buff.shape)
 
-        for value in source_col.iter_values(start, stop):
+        for value in source_col.iter_values(
+            partition.start_index, partition.stop_index
+        ):
             # We write directly into the buffer in the sanitiser function
             # to make it easier to reason about dimension padding
             j = ba.next_buffer_row()
             sanitiser(ba.buff, j, value)
         ba.flush()
-        logger.debug(f"Encoded {column.name} slice {start}:{stop}")
+        self.finalise_partition_array(partition_index, column.name)
 
-    def encode_genotypes_slice(self, start, stop):
-        source_col = self.icf.columns["FORMAT/GT"]
-        gt = core.BufferedArray(self.get_array("call_genotype"), start)
-        gt_mask = core.BufferedArray(self.get_array("call_genotype_mask"), start)
-        gt_phased = core.BufferedArray(self.get_array("call_genotype_phased"), start)
+    def encode_genotypes_partition(self, partition_index):
+        gt_array = self.init_partition_array(partition_index, "call_genotype")
+        gt_mask_array = self.init_partition_array(partition_index, "call_genotype_mask")
+        gt_phased_array = self.init_partition_array(
+            partition_index, "call_genotype_phased"
+        )
+
+        partition = self.metadata.partitions[partition_index]
+        gt = core.BufferedArray(gt_array, partition.start_index)
+        gt_mask = core.BufferedArray(gt_mask_array, partition.start_index)
+        gt_phased = core.BufferedArray(gt_phased_array, partition.start_index)
 
-        for value in source_col.iter_values(start, stop):
+        source_col = self.icf.columns["FORMAT/GT"]
+        for value in source_col.iter_values(
+            partition.start_index, partition.stop_index
+        ):
             j = gt.next_buffer_row()
             sanitise_value_int_2d(gt.buff, j, value[:, :-1])
             j = gt_phased.next_buffer_row()
             sanitise_value_int_1d(gt_phased.buff, j, value[:, -1])
             # TODO check is this the correct semantics when we are padding
             # with mixed ploidies?
             j = gt_mask.next_buffer_row()
             gt_mask.buff[j] = gt.buff[j] < 0
         gt.flush()
         gt_phased.flush()
         gt_mask.flush()
-        logger.debug(f"Encoded GT slice {start}:{stop}")
 
-    def encode_alleles_slice(self, start, stop):
+        self.finalise_partition_array(partition_index, "call_genotype")
+        self.finalise_partition_array(partition_index, "call_genotype_mask")
+        self.finalise_partition_array(partition_index, "call_genotype_phased")
+
+    def encode_alleles_partition(self, partition_index):
+        array_name = "variant_allele"
+        alleles_array = self.init_partition_array(partition_index, array_name)
+        partition = self.metadata.partitions[partition_index]
+        alleles = core.BufferedArray(alleles_array, partition.start_index)
         ref_col = self.icf.columns["REF"]
         alt_col = self.icf.columns["ALT"]
-        alleles = core.BufferedArray(self.get_array("variant_allele"), start)
 
         for ref, alt in zip(
-            ref_col.iter_values(start, stop), alt_col.iter_values(start, stop)
+            ref_col.iter_values(partition.start_index, partition.stop_index),
+            alt_col.iter_values(partition.start_index, partition.stop_index),
         ):
             j = alleles.next_buffer_row()
             alleles.buff[j, :] = STR_FILL
             alleles.buff[j, 0] = ref[0]
             alleles.buff[j, 1 : 1 + len(alt)] = alt
         alleles.flush()
-        logger.debug(f"Encoded alleles slice {start}:{stop}")
 
-    def encode_id_slice(self, start, stop):
+        self.finalise_partition_array(partition_index, array_name)
+
+    def encode_id_partition(self, partition_index):
+        vid_array = self.init_partition_array(partition_index, "variant_id")
+        vid_mask_array = self.init_partition_array(partition_index, "variant_id_mask")
+        partition = self.metadata.partitions[partition_index]
+        vid = core.BufferedArray(vid_array, partition.start_index)
+        vid_mask = core.BufferedArray(vid_mask_array, partition.start_index)
         col = self.icf.columns["ID"]
-        vid = core.BufferedArray(self.get_array("variant_id"), start)
-        vid_mask = core.BufferedArray(self.get_array("variant_id_mask"), start)
 
-        for value in col.iter_values(start, stop):
+        for value in col.iter_values(partition.start_index, partition.stop_index):
             j = vid.next_buffer_row()
             k = vid_mask.next_buffer_row()
             assert j == k
             if value is not None:
                 vid.buff[j] = value[0]
                 vid_mask.buff[j] = False
             else:
                 vid.buff[j] = STR_MISSING
                 vid_mask.buff[j] = True
         vid.flush()
         vid_mask.flush()
-        logger.debug(f"Encoded ID slice {start}:{stop}")
 
-    def encode_filters_slice(self, lookup, start, stop):
-        col = self.icf.columns["FILTERS"]
-        var_filter = core.BufferedArray(self.get_array("variant_filter"), start)
+        self.finalise_partition_array(partition_index, "variant_id")
+        self.finalise_partition_array(partition_index, "variant_id_mask")
+
+    def encode_filters_partition(self, partition_index):
+        lookup = {filt: index for index, filt in enumerate(self.schema.filter_id)}
+        array_name = "variant_filter"
+        array = self.init_partition_array(partition_index, array_name)
+        partition = self.metadata.partitions[partition_index]
+        var_filter = core.BufferedArray(array, partition.start_index)
 
-        for value in col.iter_values(start, stop):
+        col = self.icf.columns["FILTERS"]
+        for value in col.iter_values(partition.start_index, partition.stop_index):
             j = var_filter.next_buffer_row()
             var_filter.buff[j] = False
             for f in value:
                 try:
                     var_filter.buff[j, lookup[f]] = True
                 except KeyError:
                     raise ValueError(
-                        f"Filter '{f}' was not defined " f"in the header."
+                        f"Filter '{f}' was not defined in the header."
                     ) from None
         var_filter.flush()
-        logger.debug(f"Encoded FILTERS slice {start}:{stop}")
 
-    def encode_contig_slice(self, lookup, start, stop):
+        self.finalise_partition_array(partition_index, array_name)
+
+    def encode_contig_partition(self, partition_index):
+        lookup = {contig: index for index, contig in enumerate(self.schema.contig_id)}
+        array_name = "variant_contig"
+        array = self.init_partition_array(partition_index, array_name)
+        partition = self.metadata.partitions[partition_index]
+        contig = core.BufferedArray(array, partition.start_index)
         col = self.icf.columns["CHROM"]
-        contig = core.BufferedArray(self.get_array("variant_contig"), start)
 
-        for value in col.iter_values(start, stop):
+        for value in col.iter_values(partition.start_index, partition.stop_index):
             j = contig.next_buffer_row()
             # Note: because we are using the indexes to define the lookups
             # and we always have an index, it seems that we the contig lookup
             # will always succeed. However, if anyone ever does hit a KeyError
             # here, please do open an issue with a reproducible example!
             contig.buff[j] = lookup[value[0]]
         contig.flush()
-        logger.debug(f"Encoded CHROM slice {start}:{stop}")
 
-    def encode_samples(self):
-        if not np.array_equal(self.schema.sample_id, self.icf.metadata.samples):
-            raise ValueError(
-                "Subsetting or reordering samples not supported currently"
-            )  # NEEDS TEST
-        array = self.root.array(
-            "sample_id",
-            self.schema.sample_id,
-            dtype="str",
-            compressor=DEFAULT_ZARR_COMPRESSOR,
-            chunks=(self.schema.samples_chunk_size,),
-        )
-        array.attrs["_ARRAY_DIMENSIONS"] = ["samples"]
-        logger.debug("Samples done")
+        self.finalise_partition_array(partition_index, array_name)
 
-    def encode_contig_id(self):
-        array = self.root.array(
-            "contig_id",
-            self.schema.contig_id,
-            dtype="str",
-            compressor=DEFAULT_ZARR_COMPRESSOR,
-        )
-        array.attrs["_ARRAY_DIMENSIONS"] = ["contigs"]
-        if self.schema.contig_length is not None:
-            array = self.root.array(
-                "contig_length",
-                self.schema.contig_length,
-                dtype=np.int64,
-                compressor=DEFAULT_ZARR_COMPRESSOR,
+    #######################
+    # finalise
+    #######################
+
+    def finalise_array(self, name):
+        logger.info(f"Finalising {name}")
+        final_path = self.path / name
+        if final_path.exists():
+            # NEEDS TEST
+            raise ValueError(f"Array {name} already exists")
+        for partition in range(len(self.metadata.partitions)):
+            # Move all the files in partition dir to dest dir
+            src = self.partition_array_path(partition, name)
+            if not src.exists():
+                # Needs test
+                raise ValueError(f"Partition {partition} of {name} does not exist")
+            dest = self.arrays_path / name
+            # This is Zarr v2 specific. Chunks in v3 with start with "c" prefix.
+            chunk_files = [
+                path for path in src.iterdir() if not path.name.startswith(".")
+            ]
+            # TODO check for a count of then number of files. If we require a
+            # dimension_separator of "/" then we could make stronger assertions
+            # here, as we'd always have num_variant_chunks
+            logger.debug(
+                f"Moving {len(chunk_files)} chunks for {name} partition {partition}"
             )
-            array.attrs["_ARRAY_DIMENSIONS"] = ["contigs"]
-        return {v: j for j, v in enumerate(self.schema.contig_id)}
-
-    def encode_filter_id(self):
-        array = self.root.array(
-            "filter_id",
-            self.schema.filter_id,
-            dtype="str",
-            compressor=DEFAULT_ZARR_COMPRESSOR,
-        )
-        array.attrs["_ARRAY_DIMENSIONS"] = ["filters"]
-        return {v: j for j, v in enumerate(self.schema.filter_id)}
+            for chunk_file in chunk_files:
+                os.rename(chunk_file, dest / chunk_file.name)
+        # Finally, once all the chunks have moved into the arrays dir,
+        # we move it out of wip
+        os.rename(self.arrays_path / name, self.path / name)
+        core.update_progress(1)
 
-    def init(self):
-        self.root.attrs["vcf_zarr_version"] = "0.2"
-        self.root.attrs["vcf_header"] = self.icf.vcf_header
-        self.root.attrs["source"] = f"bio2zarr-{provenance.__version__}"
-        for column in self.schema.columns.values():
-            self.init_array(column)
+    def finalise(self, show_progress=False):
+        self.load_metadata()
 
-    def finalise(self):
+        progress_config = core.ProgressConfig(
+            total=len(self.schema.columns),
+            title="Finalise",
+            units="array",
+            show=show_progress,
+        )
+        # NOTE: it's not clear that adding more workers will make this quicker,
+        # as it's just going to be causing contention on the file system.
+        # Something to check empirically in some deployments.
+        # FIXME we're just using worker_processes=0 here to hook into the
+        # SynchronousExecutor which is intended for testing purposes so
+        # that we get test coverage. Should fix this either by allowing
+        # for multiple workers, or making a standard wrapper for tqdm
+        # that allows us to have a consistent look and feel.
+        with core.ParallelWorkManager(0, progress_config) as pwm:
+            for name in self.schema.columns:
+                pwm.submit(self.finalise_array, name)
         zarr.consolidate_metadata(self.path)
 
-    def encode(
-        self,
-        worker_processes=1,
-        max_v_chunks=None,
-        show_progress=False,
-        max_memory=None,
-    ):
-        max_memory = parse_max_memory(max_memory)
-
-        # TODO this will move into the setup logic later when we're making it possible
-        # to split the work by slice
-        num_slices = max(1, worker_processes * 4)
-        # Using POS arbitrarily to get the array slices
-        slices = core.chunk_aligned_slices(
-            self.get_array("variant_position"), num_slices, max_chunks=max_v_chunks
-        )
-        truncated = slices[-1][-1]
-        for array in self.root.values():
-            if array.attrs["_ARRAY_DIMENSIONS"][0] == "variants":
-                shape = list(array.shape)
-                shape[0] = truncated
-                array.resize(shape)
+    ######################
+    # encode_all_partitions
+    ######################
 
-        total_bytes = 0
-        encoding_memory_requirements = {}
-        for col in self.schema.columns.values():
-            array = self.get_array(col.name)
-            # NOTE!! this is bad, we're potentially creating quite a large
-            # numpy array for basically nothing. We can compute this.
-            variant_chunk_size = array.blocks[0].nbytes
-            encoding_memory_requirements[col.name] = variant_chunk_size
-            logger.debug(
-                f"{col.name} requires at least {display_size(variant_chunk_size)} "
-                f"per worker"
+    def get_max_encoding_memory(self):
+        """
+        Return the approximate maximum memory used to encode a variant chunk.
+        """
+        max_encoding_mem = max(
+            col.variant_chunk_nbytes for col in self.schema.columns.values()
+        )
+        gt_mem = 0
+        if "call_genotype" in self.schema.columns:
+            encoded_together = [
+                "call_genotype",
+                "call_genotype_phased",
+                "call_genotype_mask",
+            ]
+            gt_mem = sum(
+                self.schema.columns[col].variant_chunk_nbytes
+                for col in encoded_together
             )
-            total_bytes += array.nbytes
-
-        filter_id_map = self.encode_filter_id()
-        contig_id_map = self.encode_contig_id()
+        return max(max_encoding_mem, gt_mem)
 
-        work = []
-        for start, stop in slices:
-            for col in self.schema.columns.values():
-                if col.vcf_field is not None:
-                    f = functools.partial(self.encode_array_slice, col)
-                    work.append(
-                        EncodingWork(
-                            f,
-                            start,
-                            stop,
-                            [col.name],
-                            encoding_memory_requirements[col.name],
-                        )
-                    )
-            work.append(
-                EncodingWork(self.encode_alleles_slice, start, stop, ["variant_allele"])
-            )
-            work.append(
-                EncodingWork(
-                    self.encode_id_slice, start, stop, ["variant_id", "variant_id_mask"]
-                )
-            )
-            work.append(
-                EncodingWork(
-                    functools.partial(self.encode_filters_slice, filter_id_map),
-                    start,
-                    stop,
-                    ["variant_filter"],
-                )
+    def encode_all_partitions(
+        self, *, worker_processes=1, show_progress=False, max_memory=None
+    ):
+        max_memory = parse_max_memory(max_memory)
+        self.load_metadata()
+        num_partitions = self.num_partitions
+        per_worker_memory = self.get_max_encoding_memory()
+        logger.info(
+            f"Encoding Zarr over {num_partitions} partitions with "
+            f"{worker_processes} workers and {display_size(per_worker_memory)} "
+            "per worker"
+        )
+        # Each partition requires per_worker_memory bytes, so to prevent more that
+        # max_memory being used, we clamp the number of workers
+        max_num_workers = max_memory // per_worker_memory
+        if max_num_workers < worker_processes:
+            logger.warning(
+                f"Limiting number of workers to {max_num_workers} to "
+                f"keep within specified memory budget of {display_size(max_memory)}"
             )
-            work.append(
-                EncodingWork(
-                    functools.partial(self.encode_contig_slice, contig_id_map),
-                    start,
-                    stop,
-                    ["variant_contig"],
-                )
+        if max_num_workers <= 0:
+            raise ValueError(
+                f"Insufficient memory to encode a partition:"
+                f"{display_size(per_worker_memory)} > {display_size(max_memory)}"
             )
-            if "call_genotype" in self.schema.columns:
-                variables = [
-                    "call_genotype",
-                    "call_genotype_phased",
-                    "call_genotype_mask",
-                ]
-                gt_memory = sum(
-                    encoding_memory_requirements[name] for name in variables
-                )
-                work.append(
-                    EncodingWork(
-                        self.encode_genotypes_slice, start, stop, variables, gt_memory
-                    )
-                )
+        num_workers = min(max_num_workers, worker_processes)
 
-        # Fail early if we can't fit a particular column into memory
-        for wp in work:
-            if wp.memory > max_memory:
-                raise ValueError(
-                    f"Insufficient memory for {wp.columns}: "
-                    f"{display_size(wp.memory)} > {display_size(max_memory)}"
-                )
+        total_bytes = 0
+        for col in self.schema.columns.values():
+            # Open the array definition to get the total size
+            total_bytes += zarr.open(self.arrays_path / col.name).nbytes
 
         progress_config = core.ProgressConfig(
             total=total_bytes,
             title="Encode",
             units="B",
             show=show_progress,
         )
-
-        used_memory = 0
-        # We need to keep some bounds on the queue size or the memory bounds algorithm
-        # below doesn't really work.
-        max_queued = 4 * max(1, worker_processes)
-        encoded_slices = collections.Counter()
-
-        with core.ParallelWorkManager(worker_processes, progress_config) as pwm:
-            future = pwm.submit(self.encode_samples)
-            future_to_work = {future: EncodingWork(None, 0, 0, [])}
-
-            def service_completed_futures():
-                nonlocal used_memory
-
-                completed = pwm.wait_for_completed()
-                for future in completed:
-                    wp_done = future_to_work.pop(future)
-                    used_memory -= wp_done.memory
-                    logger.debug(
-                        f"Complete {wp_done}: used mem={display_size(used_memory)}"
-                    )
-                    for column in wp_done.columns:
-                        encoded_slices[column] += 1
-                        if encoded_slices[column] == len(slices):
-                            # Do this syncronously for simplicity. Should be
-                            # fine as the workers will probably be busy with
-                            # large encode tasks most of the time.
-                            self.finalise_array(column)
-
-            for wp in work:
-                while (
-                    used_memory + wp.memory > max_memory
-                    or len(future_to_work) > max_queued
-                ):
-                    logger.debug(
-                        f"Wait: mem_required={used_memory + wp.memory} "
-                        f"max_mem={max_memory} queued={len(future_to_work)} "
-                        f"max_queued={max_queued}"
-                    )
-                    service_completed_futures()
-                future = pwm.submit(wp.func, wp.start, wp.stop)
-                used_memory += wp.memory
-                logger.debug(f"Submit {wp}: used mem={display_size(used_memory)}")
-                future_to_work[future] = wp
-
-            logger.debug("All work submitted")
-            while len(future_to_work) > 0:
-                service_completed_futures()
+        with core.ParallelWorkManager(num_workers, progress_config) as pwm:
+            for partition_index in range(num_partitions):
+                pwm.submit(self.encode_partition, partition_index)
 
 
 def mkschema(if_path, out):
     icf = IntermediateColumnarFormat(if_path)
     spec = VcfZarrSchema.generate(icf)
     out.write(spec.asjson())
 
 
 def encode(
     if_path,
     zarr_path,
     schema_path=None,
     variants_chunk_size=None,
     samples_chunk_size=None,
-    max_v_chunks=None,
+    max_variant_chunks=None,
     dimension_separator=None,
     max_memory=None,
     worker_processes=1,
     show_progress=False,
 ):
-    icf = IntermediateColumnarFormat(if_path)
+    # Rough heuristic to split work up enough to keep utilisation high
+    target_num_partitions = max(1, worker_processes * 4)
+    encode_init(
+        if_path,
+        zarr_path,
+        target_num_partitions,
+        schema_path=schema_path,
+        variants_chunk_size=variants_chunk_size,
+        samples_chunk_size=samples_chunk_size,
+        max_variant_chunks=max_variant_chunks,
+        dimension_separator=dimension_separator,
+    )
+    vzw = VcfZarrWriter(zarr_path)
+    vzw.encode_all_partitions(
+        worker_processes=worker_processes,
+        show_progress=show_progress,
+        max_memory=max_memory,
+    )
+    vzw.finalise(show_progress)
+
+
+def encode_init(
+    icf_path,
+    zarr_path,
+    target_num_partitions,
+    *,
+    schema_path=None,
+    variants_chunk_size=None,
+    samples_chunk_size=None,
+    max_variant_chunks=None,
+    dimension_separator=None,
+    max_memory=None,
+    worker_processes=1,
+    show_progress=False,
+):
+    icf = IntermediateColumnarFormat(icf_path)
     if schema_path is None:
         schema = VcfZarrSchema.generate(
             icf,
             variants_chunk_size=variants_chunk_size,
             samples_chunk_size=samples_chunk_size,
         )
     else:
@@ -1896,26 +2129,33 @@
         if variants_chunk_size is not None or samples_chunk_size is not None:
             raise ValueError(
                 "Cannot specify schema along with chunk sizes"
             )  # NEEDS TEST
         with open(schema_path) as f:
             schema = VcfZarrSchema.fromjson(f.read())
     zarr_path = pathlib.Path(zarr_path)
-    if zarr_path.exists():
-        logger.warning(f"Deleting existing {zarr_path}")
-        shutil.rmtree(zarr_path)
-    vzw = VcfZarrWriter(zarr_path, icf, schema, dimension_separator=dimension_separator)
-    vzw.init()
-    vzw.encode(
-        max_v_chunks=max_v_chunks,
-        worker_processes=worker_processes,
-        max_memory=max_memory,
-        show_progress=show_progress,
+    vzw = VcfZarrWriter(zarr_path)
+    vzw.init(
+        icf,
+        target_num_partitions=target_num_partitions,
+        schema=schema,
+        dimension_separator=dimension_separator,
+        max_variant_chunks=max_variant_chunks,
     )
-    vzw.finalise()
+    return vzw.num_partitions, vzw.get_max_encoding_memory()
+
+
+def encode_partition(zarr_path, partition):
+    writer = VcfZarrWriter(zarr_path)
+    writer.encode_partition(partition)
+
+
+def encode_finalise(zarr_path, show_progress=False):
+    writer = VcfZarrWriter(zarr_path)
+    writer.finalise(show_progress=show_progress)
 
 
 def convert(
     vcfs,
     out_path,
     *,
     variants_chunk_size=None,
@@ -2117,15 +2357,15 @@
                 info_fields[name] = vcf_type, iter(root[colname])
 
     first_pos = next(vcf).POS
     start_index = np.searchsorted(pos, first_pos)
     assert pos[start_index] == first_pos
     vcf = cyvcf2.VCF(vcf_path)
     if show_progress:
-        iterator = tqdm.tqdm(vcf, desc=" Verify", total=vcf.num_records)  # NEEDS TEST
+        iterator = tqdm.tqdm(vcf, desc="  Verify", total=vcf.num_records)  # NEEDS TEST
     else:
         iterator = vcf
     for j, row in enumerate(iterator, start_index):
         assert chrom[j] == row.CHROM
         assert pos[j] == row.POS
         assert vid[j] == ("." if row.ID is None else row.ID)
         assert allele[j, 0] == row.REF
```

### Comparing `bio2zarr-0.0.5/bio2zarr/vcf_utils.py` & `bio2zarr-0.0.6/bio2zarr/vcf_utils.py`

 * *Files identical despite different names*

### Comparing `bio2zarr-0.0.5/bio2zarr.egg-info/PKG-INFO` & `bio2zarr-0.0.6/bio2zarr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bio2zarr
-Version: 0.0.5
+Version: 0.0.6
 Summary: Convert bioinformatics data to Zarr
 Home-page: https://github.com/pystatgen/bio2zarr
 Author: sgkit Developers
 Author-email: project@pystatgen.org
 License: Apache
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `bio2zarr-0.0.5/setup.cfg` & `bio2zarr-0.0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `bio2zarr-0.0.5/validation-data/Makefile` & `bio2zarr-0.0.6/validation-data/Makefile`

 * *Files identical despite different names*

### Comparing `bio2zarr-0.0.5/validation.py` & `bio2zarr-0.0.6/validation.py`

 * *Files identical despite different names*

### Comparing `bio2zarr-0.0.5/vcf_generator.py` & `bio2zarr-0.0.6/vcf_generator.py`

 * *Files identical despite different names*

