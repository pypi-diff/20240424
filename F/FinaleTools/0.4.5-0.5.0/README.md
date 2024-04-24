# Comparing `tmp/FinaleTools-0.4.5.tar.gz` & `tmp/finaletools-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FinaleTools-0.4.5.tar", last modified: Tue Apr  9 22:08:31 2024, max compression
+gzip compressed data, was "finaletools-0.5.0.tar", last modified: Wed Apr 24 06:37:57 2024, max compression
```

## Comparing `FinaleTools-0.4.5.tar` & `finaletools-0.5.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-09 22:08:31.000000 FinaleTools-0.4.5/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1067 2024-03-29 01:22:35.000000 FinaleTools-0.4.5/LICENSE
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     5911 2024-04-09 22:08:26.000000 FinaleTools-0.4.5/PKG-INFO
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     3739 2024-04-01 20:34:46.000000 FinaleTools-0.4.5/README.md
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1058 2024-04-09 22:05:26.000000 FinaleTools-0.4.5/pyproject.toml
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       38 2024-04-09 22:08:31.000000 FinaleTools-0.4.5/setup.cfg
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-09 22:07:29.000000 FinaleTools-0.4.5/src/
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-09 22:07:58.000000 FinaleTools-0.4.5/src/FinaleTools.egg-info/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     5911 2024-04-09 22:07:18.000000 FinaleTools-0.4.5/src/FinaleTools.egg-info/PKG-INFO
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1083 2024-04-09 22:07:29.000000 FinaleTools-0.4.5/src/FinaleTools.egg-info/SOURCES.txt
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)        1 2024-04-09 22:07:29.000000 FinaleTools-0.4.5/src/FinaleTools.egg-info/dependency_links.txt
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       57 2024-04-09 22:07:29.000000 FinaleTools-0.4.5/src/FinaleTools.egg-info/entry_points.txt
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)      145 2024-04-09 22:07:29.000000 FinaleTools-0.4.5/src/FinaleTools.egg-info/requires.txt
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       12 2024-04-09 22:07:29.000000 FinaleTools-0.4.5/src/FinaleTools.egg-info/top_level.txt
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-09 22:07:58.000000 FinaleTools-0.4.5/src/finaletools/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2023-06-21 12:51:49.000000 FinaleTools-0.4.5/src/finaletools/__init__.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-09 22:07:58.000000 FinaleTools-0.4.5/src/finaletools/cli/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       38 2024-03-29 01:22:38.000000 FinaleTools-0.4.5/src/finaletools/cli/__init__.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    24767 2024-04-05 16:25:39.000000 FinaleTools-0.4.5/src/finaletools/cli/main_cli.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-09 22:08:13.000000 FinaleTools-0.4.5/src/finaletools/frag/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)      509 2024-03-29 01:22:38.000000 FinaleTools-0.4.5/src/finaletools/frag/__init__.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     9664 2024-03-29 01:22:38.000000 FinaleTools-0.4.5/src/finaletools/frag/adjust_wps.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     4402 2024-03-29 01:22:38.000000 FinaleTools-0.4.5/src/finaletools/frag/agg_wps.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     9329 2024-03-29 01:49:46.000000 FinaleTools-0.4.5/src/finaletools/frag/cleavage_profile.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     7549 2024-04-09 22:05:01.000000 FinaleTools-0.4.5/src/finaletools/frag/coverage.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    14488 2024-04-01 20:23:25.000000 FinaleTools-0.4.5/src/finaletools/frag/delfi.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     3973 2024-03-29 01:22:38.000000 FinaleTools-0.4.5/src/finaletools/frag/delfi_gc_correct.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     2080 2024-04-01 20:23:25.000000 FinaleTools-0.4.5/src/finaletools/frag/delfi_merge_bins.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    24836 2024-04-09 22:02:56.000000 FinaleTools-0.4.5/src/finaletools/frag/end_motifs.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    14865 2024-03-29 02:06:16.000000 FinaleTools-0.4.5/src/finaletools/frag/frag_length.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     8466 2024-03-29 02:06:16.000000 FinaleTools-0.4.5/src/finaletools/frag/multi_wps.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     6797 2024-03-29 01:49:46.000000 FinaleTools-0.4.5/src/finaletools/frag/wps.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-09 22:08:13.000000 FinaleTools-0.4.5/src/finaletools/genome/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       37 2024-03-29 01:22:39.000000 FinaleTools-0.4.5/src/finaletools/genome/__init__.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    14339 2024-03-29 01:22:39.000000 FinaleTools-0.4.5/src/finaletools/genome/gaps.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-09 22:08:13.000000 FinaleTools-0.4.5/src/finaletools/methylation/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-03-29 01:22:39.000000 FinaleTools-0.4.5/src/finaletools/methylation/__init__.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-09 22:08:13.000000 FinaleTools-0.4.5/src/finaletools/qc/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-03-29 01:22:39.000000 FinaleTools-0.4.5/src/finaletools/qc/__init__.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-09 22:08:13.000000 FinaleTools-0.4.5/src/finaletools/too/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-03-29 01:22:39.000000 FinaleTools-0.4.5/src/finaletools/too/__init__.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-09 22:08:20.000000 FinaleTools-0.4.5/src/finaletools/utils/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       90 2024-03-29 01:22:39.000000 FinaleTools-0.4.5/src/finaletools/utils/__init__.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1649 2024-03-29 01:22:39.000000 FinaleTools-0.4.5/src/finaletools/utils/cli_hist.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     3917 2024-03-29 01:22:39.000000 FinaleTools-0.4.5/src/finaletools/utils/filter_bam.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    18436 2024-04-05 05:11:54.000000 FinaleTools-0.4.5/src/finaletools/utils/utils.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-24 06:37:57.000000 finaletools-0.5.0/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1067 2024-03-29 01:22:35.000000 finaletools-0.5.0/LICENSE
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     5911 2024-04-24 06:37:56.000000 finaletools-0.5.0/PKG-INFO
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     3739 2024-04-22 12:55:15.000000 finaletools-0.5.0/README.md
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1058 2024-04-24 06:35:59.000000 finaletools-0.5.0/pyproject.toml
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)       38 2024-04-24 06:37:57.000000 finaletools-0.5.0/setup.cfg
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-24 06:37:54.000000 finaletools-0.5.0/src/
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-24 06:37:54.000000 finaletools-0.5.0/src/FinaleTools.egg-info/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     5911 2024-04-24 06:37:32.000000 finaletools-0.5.0/src/FinaleTools.egg-info/PKG-INFO
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1083 2024-04-24 06:37:54.000000 finaletools-0.5.0/src/FinaleTools.egg-info/SOURCES.txt
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)        1 2024-04-24 06:37:53.000000 finaletools-0.5.0/src/FinaleTools.egg-info/dependency_links.txt
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)       57 2024-04-24 06:37:53.000000 finaletools-0.5.0/src/FinaleTools.egg-info/entry_points.txt
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)      145 2024-04-24 06:37:53.000000 finaletools-0.5.0/src/FinaleTools.egg-info/requires.txt
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)       12 2024-04-24 06:37:53.000000 finaletools-0.5.0/src/FinaleTools.egg-info/top_level.txt
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-24 06:37:54.000000 finaletools-0.5.0/src/finaletools/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2023-06-21 12:51:49.000000 finaletools-0.5.0/src/finaletools/__init__.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-24 06:37:54.000000 finaletools-0.5.0/src/finaletools/cli/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)       38 2024-03-29 01:22:38.000000 finaletools-0.5.0/src/finaletools/cli/__init__.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)    27956 2024-04-24 05:56:53.000000 finaletools-0.5.0/src/finaletools/cli/main_cli.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-24 06:37:55.000000 finaletools-0.5.0/src/finaletools/frag/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)      572 2024-04-24 06:06:01.000000 finaletools-0.5.0/src/finaletools/frag/__init__.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     9664 2024-03-29 01:22:38.000000 finaletools-0.5.0/src/finaletools/frag/adjust_wps.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     4402 2024-03-29 01:22:38.000000 finaletools-0.5.0/src/finaletools/frag/agg_wps.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     9329 2024-03-29 01:49:46.000000 finaletools-0.5.0/src/finaletools/frag/cleavage_profile.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     7553 2024-04-24 05:59:32.000000 finaletools-0.5.0/src/finaletools/frag/coverage.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)    14527 2024-04-24 04:05:00.000000 finaletools-0.5.0/src/finaletools/frag/delfi.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     3973 2024-03-29 01:22:38.000000 finaletools-0.5.0/src/finaletools/frag/delfi_gc_correct.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     2585 2024-04-24 04:05:00.000000 finaletools-0.5.0/src/finaletools/frag/delfi_merge_bins.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)    29182 2024-04-24 05:56:53.000000 finaletools-0.5.0/src/finaletools/frag/end_motifs.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)    14865 2024-04-22 12:55:17.000000 finaletools-0.5.0/src/finaletools/frag/frag_length.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     8466 2024-04-22 12:55:17.000000 finaletools-0.5.0/src/finaletools/frag/multi_wps.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     6797 2024-03-29 01:49:46.000000 finaletools-0.5.0/src/finaletools/frag/wps.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-24 06:37:55.000000 finaletools-0.5.0/src/finaletools/genome/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)       37 2024-03-29 01:22:39.000000 finaletools-0.5.0/src/finaletools/genome/__init__.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)    14339 2024-03-29 01:22:39.000000 finaletools-0.5.0/src/finaletools/genome/gaps.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-24 06:37:55.000000 finaletools-0.5.0/src/finaletools/methylation/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-03-29 01:22:39.000000 finaletools-0.5.0/src/finaletools/methylation/__init__.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-24 06:37:56.000000 finaletools-0.5.0/src/finaletools/qc/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-03-29 01:22:39.000000 finaletools-0.5.0/src/finaletools/qc/__init__.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-24 06:37:56.000000 finaletools-0.5.0/src/finaletools/too/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-03-29 01:22:39.000000 finaletools-0.5.0/src/finaletools/too/__init__.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-24 06:37:56.000000 finaletools-0.5.0/src/finaletools/utils/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)       90 2024-03-29 01:22:39.000000 finaletools-0.5.0/src/finaletools/utils/__init__.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1649 2024-03-29 01:22:39.000000 finaletools-0.5.0/src/finaletools/utils/cli_hist.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     3917 2024-03-29 01:22:39.000000 finaletools-0.5.0/src/finaletools/utils/filter_bam.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)    18436 2024-04-24 03:28:21.000000 finaletools-0.5.0/src/finaletools/utils/utils.py
```

### Comparing `FinaleTools-0.4.5/LICENSE` & `finaletools-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.5/PKG-INFO` & `finaletools-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FinaleTools
-Version: 0.4.5
+Version: 0.5.0
 Summary: A package and standalone program to process paired-end reads of cfDNA fragment WGS.
 Author-email: James Li <lijw21@wfu.edu>, Yaping Liu <yaping@northwestern.edu>
 License: MIT License
         
         Copyright (c) 2024 EpiFluidLab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `FinaleTools-0.4.5/README.md` & `finaletools-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.5/pyproject.toml` & `finaletools-0.5.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 include-package-data = true
 
 [project]
 name = "FinaleTools"
-version = "0.4.5"
+version = "0.5.0"
 authors = [
     {name="James Li", email="lijw21@wfu.edu"},
     {name="Yaping Liu", email="yaping@northwestern.edu"},
 ]
 description = "A package and standalone program to process paired-end reads of cfDNA fragment WGS."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `FinaleTools-0.4.5/src/FinaleTools.egg-info/PKG-INFO` & `finaletools-0.5.0/src/FinaleTools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FinaleTools
-Version: 0.4.5
+Version: 0.5.0
 Summary: A package and standalone program to process paired-end reads of cfDNA fragment WGS.
 Author-email: James Li <lijw21@wfu.edu>, Yaping Liu <yaping@northwestern.edu>
 License: MIT License
         
         Copyright (c) 2024 EpiFluidLab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `FinaleTools-0.4.5/src/FinaleTools.egg-info/SOURCES.txt` & `finaletools-0.5.0/src/FinaleTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.5/src/finaletools/cli/main_cli.py` & `finaletools-0.5.0/src/finaletools/cli/main_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 from finaletools.utils.filter_bam import filter_bam
 from finaletools.frag.coverage import coverage
 from finaletools.frag.multi_wps import multi_wps
 from finaletools.frag.delfi import delfi
 from finaletools.frag.adjust_wps import adjust_wps
 from finaletools.frag.agg_wps import agg_wps
 from finaletools.frag.delfi_gc_correct import cli_delfi_gc_correct
-from finaletools.frag.end_motifs import end_motifs, _cli_mds
+from finaletools.frag.end_motifs import (
+    end_motifs, _cli_mds, _cli_interval_mds, interval_end_motifs)
 from finaletools.frag.cleavage_profile import _cli_cleavage_profile
 from finaletools.genome.gaps import _cli_gap_bed
 
 # TODO: implement subcommands read from stdin
 # TODO: implement pipelining
 
 def main_cli_parser():
@@ -663,14 +664,83 @@
         default=0,
         action='count',
         help='Specify verbosity. Number of printed statements is proportional '
         'to number of vs.'
     )
     parser_command10.set_defaults(func=end_motifs)
 
+    # subcommand 10a: interval-end-motifs
+    parser_command10a = subparsers.add_parser(
+        'interval-end-motifs',
+        prog='finaletools-interval-end-motifs',
+        description="Measures frequency of k-mer 5' end motifs in each "
+        "region specified in a BED file and writes data into a table."
+    )
+    parser_command10a.add_argument(
+        'input_file',
+        help='SAM, BAM, or tabix-indexed file with fragment data.'
+    )
+    parser_command10a.add_argument(
+        'refseq_file',
+        help='2bit file containing reference sequence that fragments were'
+        ' aligned to.'
+    )
+    parser_command10a.add_argument(
+        'intervals',
+        help='BED file containing intervals or list of tuples'
+    )
+    parser_command10a.add_argument(
+        '-k',
+        default=4,
+        type=int,
+        help='Length of k-mer. Default is 4.'
+    )
+    parser_command10a.add_argument(
+        '-lo', '--fraction-low',
+        default=10,
+        type=int,
+        help='Smallest fragment length to consider. Default is 10'
+    )
+    parser_command10a.add_argument(
+        '-hi', '--fraction-high',
+        default=600,
+        type=int,
+        help='Longest fragment length to consider. Default is 600'
+    )
+    parser_command10a.add_argument(
+        '-o',
+        '--output-file',
+        default='-',
+        help="File path to write results to. Either tsv or csv."
+    )
+    parser_command10a.add_argument(
+        '-q',
+        '--quality-threshold',
+        default=20,
+        type=int,
+        help='Minimum MAPQ of reads. Default is 20.'
+    )
+    parser_command10a.add_argument(
+        '-w',
+        '--workers',
+        default=1,
+        type=int,
+        help='Number of subprocesses to use. Default is 1.'
+    )
+    parser_command10a.add_argument(
+        '-v',
+        '--verbose',
+        default=0,
+        action='count',
+        help='Specify verbosity. Number of printed statements is proportional '
+        'to number of vs.'
+    )
+    parser_command10a.set_defaults(func=interval_end_motifs)
+
+
     # Subcommand 11: MDS
     parser_command11 = subparsers.add_parser(
         'mds',
         prog='finaletools-mds',
         description='Reads k-mer frequencies from a file and calculates a '
         'motif diversity score (MDS) using normalized Shannon entropy as '
         'described by Jiang et al (2020). This function is generalized for '
@@ -693,15 +763,45 @@
         '--header',
         default=0,
         type=int,
         help='Number of header rows to ignore. Default is 0'
     )
     parser_command11.set_defaults(func=_cli_mds)
 
+
+    # Subcommand 11a: interval-mds
+    parser_command11a = subparsers.add_parser(
+        'interval-mds',
+        prog='finaletools-interval-mds',
+        description='Reads k-mer frequencies from a file and calculates a '
+        'motif diversity score (MDS) for each interval using normalized '
+        'Shannon entropy as '
+        'described by Jiang et al (2020). This function is generalized for '
+        'any k-mer instead of just 4-mers.'
+    )
+    parser_command11a.add_argument(
+        'file_path',
+        nargs='?',
+        default='-',
+        help='Tab-delimited or similar file containing one column for all '
+        'k-mers a one column for frequency. Reads from stdin by default.'
+    )
+    parser_command11a.add_argument(
+        '-s',
+        '--sep',
+        default=',',
+        help='Separator used in tabular file. Default is tab.'
+    )
+    parser_command11a.add_argument(
+        'file_out',
+        default='-'
+    )
+    parser_command11a.set_defaults(func=_cli_interval_mds)
     
+
     # Subcommand 12: gap bed
     parser_command12 = subparsers.add_parser(
         'gap-bed',
         prog='finaletools-gap-bed',
         description='Creates a BED4 file containing centromeres, '
         'telomeres, and short-arm intervals, similar to the gaps '
         'annotation track for hg19 found on the UCSC Genome Browser '
@@ -785,17 +885,19 @@
     return parser
 
 
 def main_cli():
     parser = main_cli_parser()
 
     args = parser.parse_args()
-    function = args.func
-    funcargs = vars(args)
-    funcargs.pop('func')
-    funcargs.pop('subcommand')
-
-    function(**funcargs)
-
-
+    try:
+        function = args.func
+        funcargs = vars(args)
+        funcargs.pop('func')
+        funcargs.pop('subcommand')
+
+        function(**funcargs)
+    except AttributeError:
+        parser.print_help()
+    
 if __name__ == '__main__':
     main_cli()
```

### Comparing `FinaleTools-0.4.5/src/finaletools/frag/adjust_wps.py` & `finaletools-0.5.0/src/finaletools/frag/adjust_wps.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.5/src/finaletools/frag/agg_wps.py` & `finaletools-0.5.0/src/finaletools/frag/agg_wps.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.5/src/finaletools/frag/cleavage_profile.py` & `finaletools-0.5.0/src/finaletools/frag/cleavage_profile.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.5/src/finaletools/frag/coverage.py` & `finaletools-0.5.0/src/finaletools/frag/coverage.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,19 +105,20 @@
 def coverage(
         input_file: Union[str, pysam.AlignmentFile],
         interval_file: str,
         output_file: str,
         scale_factor: float=1e6,
         quality_threshold: int=30,
         workers: int=1,
-        verbose: Union[bool, int]=False):
+        verbose: Union[bool, int]=False
+    ):
     """
     Return estimated fragment coverage over intervals specified in
     `intervals`. Fragments are read from `input_file` which may be
-     a SAM, BAM, CRAM, or Frag.gz file. Uses an algorithm where the midpoints of
+    a SAM, BAM, CRAM, or Frag.gz file. Uses an algorithm where the midpoints of
     fragments are calculated and coverage is tabulated from the
     midpoints that fall into the specified region. Not suitable for
     fragments of size approaching interval size.
 
     Parameters
     ----------
     input_file : str or pysam.AlignmentFile
```

### Comparing `FinaleTools-0.4.5/src/finaletools/frag/delfi.py` & `finaletools-0.5.0/src/finaletools/frag/delfi.py`

 * *Files 2% similar despite different names*

```diff
@@ -393,15 +393,15 @@
     window_df = pandas.DataFrame(
         windows,
         columns=[
             'contig', 'start', 'stop', 'arm', 'short', 'long', 'gc',
             'num_frags']
     )
     # remove remaining NOARM bins
-    trimmed_windows = window_df[window_df['arm']!='NOARM']
+    trimmed_windows = window_df.loc[window_df['arm']!='NOARM', :].copy()
 
     if (verbose):
         stderr.write(f'{trimmed_windows.shape[0]} bins remaining...\n')
 
     # calculating ratio
     if (verbose):
         stderr.write('Calculating ratio...\n')
@@ -415,15 +415,16 @@
         gc_corrected = delfi_gc_correct(trimmed_windows, 0.75, 8, verbose)
     else:
         gc_corrected = trimmed_windows
 
     if merge_bins:
         if (verbose):
             stderr.write('Merging bins...\n')
-        final_bins = delfi_merge_bins(gc_corrected, True, verbose=verbose)
+        final_bins = delfi_merge_bins(
+            gc_corrected, gc_correct, True, verbose=verbose)
     else:
         final_bins = gc_corrected
     
     # output
     if (verbose):
         stderr.write(f'{final_bins.shape[0]} bins remaining.\n')
```

### Comparing `FinaleTools-0.4.5/src/finaletools/frag/delfi_gc_correct.py` & `finaletools-0.5.0/src/finaletools/frag/delfi_gc_correct.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.5/src/finaletools/frag/delfi_merge_bins.py` & `finaletools-0.5.0/src/finaletools/frag/delfi_merge_bins.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,16 +12,17 @@
 # path to csv containing 5mb bins from delfi_scripts
 BINS_PATH: Path = (
     files(pkg_data) /'data' / 'Jan28.hg19.5mb_features_formatted.csv'
 )
 
 def delfi_merge_bins(
         hundred_kb_bins: pd.DataFrame,
-        add_chr:bool=False,
-        verbose:bool=False
+        gc_corrected: bool=True,
+        add_chr: bool=False,
+        verbose: bool=False
 ):
     #FIXME: find a way to calculate this that is not dependent on b37 format
     delfi_scripts_5mb_bins = pd.read_csv(BINS_PATH)
 
     if add_chr:
         chr_bins = hundred_kb_bins.copy()
         chr_bins['contig'] = hundred_kb_bins['contig'].apply(
@@ -46,19 +47,27 @@
         (stops_1 > starts_2)
     )
     in_same_contig = contigs_1 == contigs_2
     overlaps = np.logical_and(contig_blind_overlaps, in_same_contig)
 
     # merging bins
     ft_5mb_indices = np.arange(five_mb_bins.shape[0])
-    for i in ft_5mb_indices:
-        subset = (chr_bins.loc[overlaps[:,i],:])
-        assert subset.shape[0] == 50, "5mb bin does not have 50 100bins."
-        
-        five_mb_bins.iloc[[i],[4]] = subset['short_corrected'].sum()
-        five_mb_bins.iloc[[i],[5]] = subset['long_corrected'].sum()
-        five_mb_bins.iloc[[i],[6]] = subset['ratio_corrected'].mean()
-        five_mb_bins.iloc[[i],[7]] = subset['num_frags_corrected'].sum()
+    if gc_corrected:
+        for i in ft_5mb_indices:
+            subset = (chr_bins.loc[overlaps[:,i],:])
+            assert subset.shape[0] == 50, "5mb bin does not have 50 100bins."
+            five_mb_bins.iloc[[i],[4]] = subset['short_corrected'].sum()
+            five_mb_bins.iloc[[i],[5]] = subset['long_corrected'].sum()
+            five_mb_bins.iloc[[i],[6]] = subset['ratio_corrected'].mean()
+            five_mb_bins.iloc[[i],[7]] = subset['num_frags_corrected'].sum()
+    else:
+        for i in ft_5mb_indices:
+            subset = (chr_bins.loc[overlaps[:,i],:])
+            assert subset.shape[0] == 50, "5mb bin does not have 50 100bins."
+            five_mb_bins.iloc[[i],[4]] = subset['short'].sum()
+            five_mb_bins.iloc[[i],[5]] = subset['long'].sum()
+            five_mb_bins.iloc[[i],[6]] = subset['ratio'].mean()
+            five_mb_bins.iloc[[i],[7]] = subset['num_frags'].sum()
     
     return five_mb_bins
 
 # TODO: make binning customizable
```

### Comparing `FinaleTools-0.4.5/src/finaletools/frag/end_motifs.py` & `finaletools-0.5.0/src/finaletools/frag/end_motifs.py`

 * *Files 10% similar despite different names*

```diff
@@ -212,14 +212,63 @@
         return (interval for interval in self.intervals)
 
     def __len__(self) -> int:
         return self.intervals.__len__()
 
     def __str__(self) -> str:
         return f'EndMotifsIntervals over {len(self.intervals)} intervals.'
+    
+    @classmethod
+    def from_file(
+            cls,
+            file_path: str,
+            quality_threshold: int,
+            sep: str=',') -> EndMotifFreqs:
+        """
+        Reads kmer frequency from a tab-delimited file
+
+        Parameters
+        ---------
+        file_path : str
+            Path string containing path to file.
+        sep : str, optional
+            Delimiter used in file.
+
+        Return
+        ------
+        kmer_freqs : EndMotifFreqs
+        """
+        try:
+            # open file
+            is_file = False
+            if file_path.endswith('gz'):
+                is_file = True
+                file = gzip.open(file_path)
+            elif file_path == '-':
+                file = stdin
+            else:
+                is_file = True
+                file = open(file_path)
+
+            intervals = []
+            lines = file.readlines()
+            _,_,_,_,_,*kmers = lines[0].split(sep)
+            k = round(np.log(len(kmers))/np.log(4))
+            assert 4**k == len(kmers), f"We got k={k} but there are {len(kmers)} kmers."
+
+            for line in lines[1:]:
+                contig, start, stop, name, *freqs = line.split(sep)
+                start, stop = int(start), int(stop)
+                float_freqs = [float(freq) for freq in freqs]
+                dict_freqs = dict(zip(kmers, float_freqs))
+                intervals.append(((contig, start, stop, name), dict_freqs))
+        finally:
+            if is_file:
+                file.close()
+        return cls(intervals, k, quality_threshold)
 
     def freq(self, kmer: str) -> list[Tuple[str, int, int, float]]:
         """
         Returns a list of intervals and associated frquency for given
         kmer. Results are in the form (chrom, 0-based start, 1-based
         stop, frequency).
         """
@@ -232,19 +281,34 @@
         Calculates a motif diversity score (MDS) for each interval using
         normalized Shannon entropy as described by Jiang et al (2020). This
         function is generalized for any k instead of just 4-mers.
         """
         num_kmers = 4**self.k
         mds = []
         for interval, kmers in self.intervals:
-            freq = np.array(kmers.values())
-            interval_mds = np.sum(-freq*np.log(freq)/np.log(num_kmers))
-        mds.append((interval, interval_mds))
-
+            freq = np.array(list(kmers.values()))
+            try:
+                interval_mds = np.sum(-freq*np.log(freq))/np.log(num_kmers)
+            except RuntimeWarning:
+                interval_mds = np.NaN
+            mds.append((interval, interval_mds))
         return mds
+
+    def mds_bed(self, output_file: str, sep: str='\t'):
+        """Writes MDS for each interval to a bed/bedgraph file."""
+        mds = self.motif_diversity_score()
+        with open(output_file, 'w') as out:
+            for interval, interval_mds in mds:
+                contig, start, stop, name = interval
+                temp_str = sep.join(
+                        [contig, str(start), str(stop), name, str(interval_mds)]
+                    )
+                out.write(
+                    f"{temp_str}\n"
+                )
     
     def to_tsv(self, output_file: str, calc_freq: bool=True, sep: str='\t'):
         """
         Writes all intervals and associated frquencies to file.
         
         Parameters
         ----------
@@ -265,24 +329,25 @@
                 else:
                     output_is_file = True
                     output = open(output_file, 'w')
 
                 # write to file
                 kmers = _gen_kmers(self.k, 'ACGT')
                 # header
-                output.write(sep.join(['contig','start','stop','count',*kmers]))
+                output.write(sep.join(['contig','start','stop','name','count',*kmers]))
                 output.write('\n')
                 # data
                 for interval, freqs in self.intervals:
                     count = sum(freqs.values())
                     output.write(
                         sep.join([
                             interval[0],
                             str(interval[1]),
                             str(interval[2]),
+                            str(interval[3]),
                             str(count), 
                             *([str(freq) for freq in freqs.values()]
                              if not calc_freq
                              else [f"{(freq/count):.6f}"
                                    if count!=0
                                    else "NaN" 
                                 for freq
@@ -301,14 +366,67 @@
             self,
             kmer: str,
             output_file: str,
             calc_freq: bool=True,
             sep: str='\t'
         ):
         """
+        Take frequency of specified kmer and writes to bedgraph.
+        
+        Parameters
+        ----------
+        output_file: str
+            File to write frequencies to.
+        calc_freq: bool, optional
+            Calculates frequency of motifs if true. Otherwise, writes counts
+            for each motif. Default is true.
+        sep: str, optional
+            Separator for table. Tab-separated by default.
+        """
+        if type(output_file) == str:
+            try:
+                # open file based on name
+                output_is_file = False
+                if output_file == '-':
+                    output = stdout
+                else:
+                    output_is_file = True
+                    output = open(output_file, 'w')
+
+                # write to file
+                for interval, freqs in self.intervals:
+                    count = sum(freqs.values())
+                    output.write(
+                        sep.join([
+                            interval[0],
+                            str(interval[1]),
+                            str(interval[2]),
+                            (self.freq[kmer] if not calc_freq
+                             else f"{(freqs[kmer]/count):.6f}"
+                                if count!=0
+                                else "NaN"
+                            )
+                        ])
+                    )
+                    output.write('\n')
+
+            finally:
+                if output_is_file:
+                    output.close()
+        else:
+            raise TypeError(f'output_file must be a string.')
+        
+    def to_bed(
+            self,
+            kmer: str,
+            output_file: str,
+            calc_freq: bool=True,
+            sep: str='\t'
+        ):
+        """
         Take frequency of specified kmer and writes to BED.
         
         Parameters
         ----------
         output_file: str
             File to write frequencies to.
         calc_freq: bool, optional
@@ -331,14 +449,15 @@
                 for interval, freqs in self.intervals:
                     count = sum(freqs.values())
                     output.write(
                         sep.join([
                             interval[0],
                             str(interval[1]),
                             str(interval[2]),
+                            interval[3],
                             (self.freq[kmer] if not calc_freq
                              else f"{(freqs[kmer]/count):.6f}"
                                 if count!=0
                                 else "NaN"
                             )
                         ])
                     )
@@ -699,36 +818,30 @@
     """
     if verbose:
         start_time = time()
 
     bases='ACGT'
     kmer_list = _gen_kmers(k, bases)
 
-    # read chromosomes from py2bit
-    try:
-        refseq = py2bit.open(refseq_file, 'r')
-        chroms: dict = refseq.chroms()
-    finally:
-        refseq.close()
-
     # generate list of inputs
     if type(intervals) is str:
         with open(intervals, 'r') as interval_file:
-            intervals_tuples = [
-                (chrom, int(start), int(stop))
-                for chrom, start, stop, *_
-                in [line.split() for line in interval_file.readlines()]
-                ]
+            intervals_tuples = [    # parses file lines into a tuple generator
+                (chrom, int(start), int(stop),
+                    name[0] if len(name) > 0 else '.')
+                for chrom, start, stop, *name
+                in (line.split() for line in interval_file.readlines())
+            ]
     elif type(intervals) is tuple:
         intervals_tuples = intervals
     else:
         raise TypeError("Intervals should be string or tuple.")
     
     mp_intervals = []   # args to be fed into pool processes
-    for chrom, start, stop in intervals_tuples:
+    for chrom, start, stop, _ in intervals_tuples:
         mp_intervals.append((
             input_file,
             chrom,
             start,
             stop,
             refseq_file,
             k,
@@ -793,7 +906,22 @@
         file_path,
         30,
         sep,
         header,
     )
     mds = motifs.motif_diversity_score()
     stdout.write(f'{mds}\n')
+
+def _cli_interval_mds(
+    file_path: str,
+    file_out: str,
+    sep: str = ',',
+    header: int = 0,
+) -> float:
+    # 30 is used as a placeholder for the quality threshold. It is not
+    # used to calculate MDS and can be ignored.
+    motifs = EndMotifsIntervals.from_file(
+        file_path,
+        30,
+        sep,
+    )
+    motifs.mds_bed(file_out)
```

### Comparing `FinaleTools-0.4.5/src/finaletools/frag/frag_length.py` & `finaletools-0.5.0/src/finaletools/frag/frag_length.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.5/src/finaletools/frag/multi_wps.py` & `finaletools-0.5.0/src/finaletools/frag/multi_wps.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.5/src/finaletools/frag/wps.py` & `finaletools-0.5.0/src/finaletools/frag/wps.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.5/src/finaletools/genome/gaps.py` & `finaletools-0.5.0/src/finaletools/genome/gaps.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.5/src/finaletools/utils/cli_hist.py` & `finaletools-0.5.0/src/finaletools/utils/cli_hist.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.5/src/finaletools/utils/filter_bam.py` & `finaletools-0.5.0/src/finaletools/utils/filter_bam.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.5/src/finaletools/utils/utils.py` & `finaletools-0.5.0/src/finaletools/utils/utils.py`

 * *Files identical despite different names*

