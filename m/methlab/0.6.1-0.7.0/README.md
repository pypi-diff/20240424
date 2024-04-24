# Comparing `tmp/methlab-0.6.1.tar.gz` & `tmp/methlab-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "methlab-0.6.1.tar", last modified: Tue Mar 19 06:20:29 2024, max compression
+gzip compressed data, was "dist/methlab-0.7.0.tar", last modified: Wed Apr 24 07:04:06 2024, max compression
```

## Comparing `methlab-0.6.1.tar` & `methlab-0.7.0.tar`

### file list

```diff
@@ -1,62 +1,59 @@
-drwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)        0 2024-03-19 06:20:29.859630 methlab-0.6.1/
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)      162 2023-06-29 11:42:57.000000 methlab-0.6.1/AUTHORS.rst
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)     3517 2023-11-21 13:34:32.000000 methlab-0.6.1/CONTRIBUTING.rst
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)     1862 2023-11-21 13:34:32.000000 methlab-0.6.1/HISTORY.rst
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)     1068 2023-06-29 11:42:57.000000 methlab-0.6.1/LICENSE
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)      262 2023-06-29 11:42:57.000000 methlab-0.6.1/MANIFEST.in
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)      747 2024-03-19 06:20:29.851086 methlab-0.6.1/PKG-INFO
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)     1479 2023-11-21 14:44:12.000000 methlab-0.6.1/README.rst
-drwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)        0 2024-03-19 06:20:29.156049 methlab-0.6.1/docs/
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)      608 2023-11-21 13:07:16.000000 methlab-0.6.1/docs/Makefile
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)       28 2023-06-29 11:42:57.000000 methlab-0.6.1/docs/authors.rst
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)     2173 2023-11-21 13:34:32.000000 methlab-0.6.1/docs/conf.py
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)       33 2023-06-29 11:42:57.000000 methlab-0.6.1/docs/contributing.rst
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)       28 2023-06-29 11:42:57.000000 methlab-0.6.1/docs/history.rst
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)      854 2023-11-21 14:52:10.000000 methlab-0.6.1/docs/index.rst
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)     1122 2023-11-21 14:44:10.000000 methlab-0.6.1/docs/installation.rst
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)      805 2023-11-21 13:07:16.000000 methlab-0.6.1/docs/make.bat
-drwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)        0 2024-03-19 06:20:29.264052 methlab-0.6.1/docs/modules/
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)     2992 2023-11-21 13:34:32.000000 methlab-0.6.1/docs/modules/BismarkSam.rst
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)     5412 2023-11-21 13:34:32.000000 methlab-0.6.1/docs/modules/CytosineCoverageFile.rst
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)     5999 2023-11-21 13:34:32.000000 methlab-0.6.1/docs/modules/align_plate_positions.rst
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)     5569 2023-11-21 13:34:32.000000 methlab-0.6.1/docs/modules/methylation_state.rst
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)       27 2023-06-29 11:42:57.000000 methlab-0.6.1/docs/readme.rst
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)       69 2023-11-21 13:07:16.000000 methlab-0.6.1/docs/usage.rst
-drwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)        0 2024-03-19 06:20:29.410375 methlab-0.6.1/methlab/
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)     3944 2023-11-21 13:34:32.000000 methlab-0.6.1/methlab/BismarkSam.py
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)    10109 2023-11-21 13:34:32.000000 methlab-0.6.1/methlab/CytosineCoverageFile.py
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)      458 2024-03-18 11:59:02.000000 methlab-0.6.1/methlab/__init__.py
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)      924 2023-11-21 13:34:32.000000 methlab-0.6.1/methlab/_alogsumexp.py
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)     6548 2024-03-18 12:13:56.000000 methlab-0.6.1/methlab/align_fastq_with_plate_positions.py
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)     1253 2023-11-21 13:34:32.000000 methlab-0.6.1/methlab/cli.py
-drwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)        0 2024-03-19 06:20:29.592120 methlab-0.6.1/methlab/data/
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)    24802 2023-11-21 13:34:32.000000 methlab-0.6.1/methlab/data/nordborg_nextera_index_sets.csv
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)     4269 2023-11-21 13:34:32.000000 methlab-0.6.1/methlab/data/plate_2022-007.csv
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)    14722 2023-11-21 13:34:32.000000 methlab-0.6.1/methlab/data/unique_nextera_dual_xt.csv
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)       19 2023-11-21 13:34:32.000000 methlab-0.6.1/methlab/epiclinestools.py
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)      588 2023-11-21 13:34:32.000000 methlab-0.6.1/methlab/estimate_beta_parameters.py
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)     5433 2023-11-21 13:34:32.000000 methlab-0.6.1/methlab/methylation_state.py
-drwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)        0 2024-03-19 06:20:29.824163 methlab-0.6.1/methlab.egg-info/
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)      747 2024-03-19 06:20:28.000000 methlab-0.6.1/methlab.egg-info/PKG-INFO
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)     1389 2024-03-19 06:20:28.000000 methlab-0.6.1/methlab.egg-info/SOURCES.txt
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)        1 2024-03-19 06:20:28.000000 methlab-0.6.1/methlab.egg-info/dependency_links.txt
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)       54 2024-03-19 06:20:28.000000 methlab-0.6.1/methlab.egg-info/entry_points.txt
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)        1 2023-06-30 12:02:04.000000 methlab-0.6.1/methlab.egg-info/not-zip-safe
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)       13 2024-03-19 06:20:28.000000 methlab-0.6.1/methlab.egg-info/requires.txt
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)        8 2024-03-19 06:20:28.000000 methlab-0.6.1/methlab.egg-info/top_level.txt
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)      533 2024-03-19 06:20:29.920060 methlab-0.6.1/setup.cfg
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)     1998 2023-11-21 13:34:32.000000 methlab-0.6.1/setup.py
-drwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)        0 2024-03-19 06:20:29.652141 methlab-0.6.1/tests/
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)       37 2023-11-21 13:34:32.000000 methlab-0.6.1/tests/__init__.py
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)     1397 2023-11-21 13:34:32.000000 methlab-0.6.1/tests/test_BismarkSam.py
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)     4475 2023-11-21 13:34:32.000000 methlab-0.6.1/tests/test_CytosineCoverageFile.py
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)     1735 2024-03-18 12:15:32.000000 methlab-0.6.1/tests/test_align_fastq_with_plate_positions.py
-drwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)        0 2024-03-19 06:20:29.794140 methlab-0.6.1/tests/test_data/
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)    46597 2023-09-12 09:25:34.000000 methlab-0.6.1/tests/test_data/chloroplast.sam
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)     1020 2023-11-13 07:31:00.000000 methlab-0.6.1/tests/test_data/gene_read_counts.csv
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)     1627 2023-11-21 13:34:32.000000 methlab-0.6.1/tests/test_data/readme.txt
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)     7657 2023-09-15 06:40:43.000000 methlab-0.6.1/tests/test_data/strandID.sam
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)      697 2023-07-24 11:02:30.000000 methlab-0.6.1/tests/test_data/test_TAIR10_GFF3_genes_transposons.gff
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)    48213 2023-07-25 08:53:20.000000 methlab-0.6.1/tests/test_data/test_coverage2cytosine.txt.gz
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)      578 2023-11-21 13:34:33.000000 methlab-0.6.1/tests/test_epiclinestools.py
--rwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)     1040 2023-11-21 13:34:33.000000 methlab-0.6.1/tests/test_methylation_state.py
+drwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)        0 2024-04-24 07:04:06.000000 methlab-0.7.0/
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)      162 2023-06-29 11:42:57.000000 methlab-0.7.0/AUTHORS.rst
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)     3517 2023-11-21 13:34:32.000000 methlab-0.7.0/CONTRIBUTING.rst
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)     1862 2023-11-21 13:34:32.000000 methlab-0.7.0/HISTORY.rst
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)     1068 2023-06-29 11:42:57.000000 methlab-0.7.0/LICENSE
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)      262 2023-06-29 11:42:57.000000 methlab-0.7.0/MANIFEST.in
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)      695 2024-04-24 07:04:06.000000 methlab-0.7.0/PKG-INFO
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)     1479 2023-11-21 14:44:12.000000 methlab-0.7.0/README.rst
+drwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)        0 2024-04-24 07:04:05.000000 methlab-0.7.0/docs/
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)      608 2023-11-21 13:07:16.000000 methlab-0.7.0/docs/Makefile
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)       28 2023-06-29 11:42:57.000000 methlab-0.7.0/docs/authors.rst
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)     2173 2023-11-21 13:34:32.000000 methlab-0.7.0/docs/conf.py
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)       33 2023-06-29 11:42:57.000000 methlab-0.7.0/docs/contributing.rst
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)       28 2023-06-29 11:42:57.000000 methlab-0.7.0/docs/history.rst
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)      854 2023-11-21 14:52:10.000000 methlab-0.7.0/docs/index.rst
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)     1122 2023-11-21 14:44:10.000000 methlab-0.7.0/docs/installation.rst
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)      805 2023-11-21 13:07:16.000000 methlab-0.7.0/docs/make.bat
+drwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)        0 2024-04-24 07:04:05.000000 methlab-0.7.0/docs/modules/
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)     2992 2023-11-21 13:34:32.000000 methlab-0.7.0/docs/modules/BismarkSam.rst
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)     5412 2023-11-21 13:34:32.000000 methlab-0.7.0/docs/modules/CytosineCoverageFile.rst
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)     5974 2024-04-19 11:57:23.000000 methlab-0.7.0/docs/modules/align_plate_positions.rst
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)     5569 2023-11-21 13:34:32.000000 methlab-0.7.0/docs/modules/methylation_state.rst
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)       27 2023-06-29 11:42:57.000000 methlab-0.7.0/docs/readme.rst
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)       69 2023-11-21 13:07:16.000000 methlab-0.7.0/docs/usage.rst
+drwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)        0 2024-04-24 07:04:05.000000 methlab-0.7.0/methlab/
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)     3944 2023-11-21 13:34:32.000000 methlab-0.7.0/methlab/BismarkSam.py
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)    10109 2023-11-21 13:34:32.000000 methlab-0.7.0/methlab/CytosineCoverageFile.py
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)      458 2024-04-18 08:16:51.000000 methlab-0.7.0/methlab/__init__.py
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)      924 2023-11-21 13:34:32.000000 methlab-0.7.0/methlab/_alogsumexp.py
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)     2843 2024-04-18 09:30:04.000000 methlab-0.7.0/methlab/align_fastq_with_plate_positions.py
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)     1253 2023-11-21 13:34:32.000000 methlab-0.7.0/methlab/cli.py
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)       19 2023-11-21 13:34:32.000000 methlab-0.7.0/methlab/epiclinestools.py
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)      588 2023-11-21 13:34:32.000000 methlab-0.7.0/methlab/estimate_beta_parameters.py
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)     5433 2023-11-21 13:34:32.000000 methlab-0.7.0/methlab/methylation_state.py
+drwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)        0 2024-04-24 07:04:06.000000 methlab-0.7.0/methlab.egg-info/
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)      695 2024-04-24 07:04:05.000000 methlab-0.7.0/methlab.egg-info/PKG-INFO
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)     1309 2024-04-24 07:04:05.000000 methlab-0.7.0/methlab.egg-info/SOURCES.txt
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)        1 2024-04-24 07:04:05.000000 methlab-0.7.0/methlab.egg-info/dependency_links.txt
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)       55 2024-04-24 07:04:05.000000 methlab-0.7.0/methlab.egg-info/entry_points.txt
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)        1 2023-06-30 12:02:04.000000 methlab-0.7.0/methlab.egg-info/not-zip-safe
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)       13 2024-04-24 07:04:05.000000 methlab-0.7.0/methlab.egg-info/requires.txt
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)        8 2024-04-24 07:04:05.000000 methlab-0.7.0/methlab.egg-info/top_level.txt
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)      533 2024-04-24 07:04:06.000000 methlab-0.7.0/setup.cfg
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)     1998 2023-11-21 13:34:32.000000 methlab-0.7.0/setup.py
+drwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)        0 2024-04-24 07:04:06.000000 methlab-0.7.0/tests/
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)       37 2023-11-21 13:34:32.000000 methlab-0.7.0/tests/__init__.py
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)     1397 2023-11-21 13:34:32.000000 methlab-0.7.0/tests/test_BismarkSam.py
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)     4475 2023-11-21 13:34:32.000000 methlab-0.7.0/tests/test_CytosineCoverageFile.py
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)     2850 2024-04-18 09:31:13.000000 methlab-0.7.0/tests/test_align_fastq_with_plate_positions.py
+drwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)        0 2024-04-24 07:04:06.000000 methlab-0.7.0/tests/test_data/
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)      339 2024-04-09 13:48:22.000000 methlab-0.7.0/tests/test_data/NGS_sample_sheet.csv
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)    46597 2023-09-12 09:25:34.000000 methlab-0.7.0/tests/test_data/chloroplast.sam
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)     1020 2023-11-13 07:31:00.000000 methlab-0.7.0/tests/test_data/gene_read_counts.csv
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)     1627 2023-11-21 13:34:32.000000 methlab-0.7.0/tests/test_data/readme.txt
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)     7657 2023-09-15 06:40:43.000000 methlab-0.7.0/tests/test_data/strandID.sam
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)      697 2023-07-24 11:02:30.000000 methlab-0.7.0/tests/test_data/test_TAIR10_GFF3_genes_transposons.gff
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)    48213 2023-07-25 08:53:20.000000 methlab-0.7.0/tests/test_data/test_coverage2cytosine.txt.gz
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)      578 2023-11-21 13:34:33.000000 methlab-0.7.0/tests/test_epiclinestools.py
+-rwxrwxrwx   0 thomas.ellis (10947) nordborg (10150)     1040 2023-11-21 13:34:33.000000 methlab-0.7.0/tests/test_methylation_state.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `methlab-0.6.1/CONTRIBUTING.rst` & `methlab-0.7.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `methlab-0.6.1/HISTORY.rst` & `methlab-0.7.0/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `methlab-0.6.1/LICENSE` & `methlab-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `methlab-0.6.1/PKG-INFO` & `methlab-0.7.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: methlab
-Version: 0.6.1
+Version: 0.7.0
 Summary: Python tools for the epiclines ERC project
 Home-page: https://github.com/ellisztamas/methlab
 Author: Tom Ellis
 Author-email: thomas.ellis@gmi.oeaw.ac.at
 License: MIT license
+Description: UNKNOWN
 Keywords: methlab
+Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
-License-File: LICENSE
-License-File: AUTHORS.rst
-Requires-Dist: pandas
-Requires-Dist: numpy
```

### Comparing `methlab-0.6.1/README.rst` & `methlab-0.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `methlab-0.6.1/docs/Makefile` & `methlab-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `methlab-0.6.1/docs/conf.py` & `methlab-0.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `methlab-0.6.1/docs/index.rst` & `methlab-0.7.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `methlab-0.6.1/docs/installation.rst` & `methlab-0.7.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `methlab-0.6.1/docs/make.bat` & `methlab-0.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `methlab-0.6.1/docs/modules/BismarkSam.rst` & `methlab-0.7.0/docs/modules/BismarkSam.rst`

 * *Files identical despite different names*

### Comparing `methlab-0.6.1/docs/modules/CytosineCoverageFile.rst` & `methlab-0.7.0/docs/modules/CytosineCoverageFile.rst`

 * *Files identical despite different names*

### Comparing `methlab-0.6.1/docs/modules/align_plate_positions.rst` & `methlab-0.7.0/docs/modules/align_plate_positions.rst`

 * *Files 17% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 .. parsed-literal::
 
     H3H7YDRXY_1#144456_ACTCGCTACGTCTAAT.bam
 
 How is one meant to determine which sample in the original plate each file is
 meant to correspond to?
 
-============================
 What do the file names mean?
 ============================
 
 Unfortunately, the naming system of files has changed through time, so they might
 not always look like the ones above. In this case at least you can see:
 
 * ``H3H7YDRXY`` is the flow cell on which sequences were run.
@@ -31,96 +30,103 @@
   facility's data on the sequencing run (in this case, for example: 
   https://ngs.vbcf.ac.at/forskalle3/samples/144456).
   Confusingly, the facility also has a 'request number', which looks very similar.
 * ``ACTCGCTACGTCTAAT`` gives the **adapter index** sequence for this sample.
   This comprises two 8-or-more nucleotide sequences that together give a unique
   identifier for the row/column position in a 96-well plate. There may be
   multiple combinations for separate plates so that these can be run on a single
-  flow cell. For example, 
-  `here <https://docs.google.com/spreadsheets/d/1gooUY2Uh23d04bDt7Ph5gGQne4GB-LlApk5h1iO8aUA/edit#gid=0>`_
-  is an example of the full set of Nextera Dual XT adapters, for up to four plates.
-  The full cornucopia of adapter sets available at the NGS facility is 
-  `here <https://ngs.vbcf.ac.at/forskalle3/account/adaptors>`_, in a format that
-  could politely be called "a data-science nightmare".
+  flow cell.
+
+Which adaptors do I have? 
+=========================
+
+For data created from 2023 or later you probably have the Nextera Dual XT
+adapters, which are four sets of 96 unique pairs of adaptors.
+You can view them 
+`here <https://docs.google.com/spreadsheets/d/1gooUY2Uh23d04bDt7Ph5gGQne4GB-LlApk5h1iO8aUA/edit#gid=0>`_.
+
+Before 2023 there was little consistency, and they could be one of many adaptor
+available.
+The full cornucopia of adapter sets available at the NGS facility is 
+`here <https://ngs.vbcf.ac.at/forskalle3/account/adaptors>`_, in a format that
+could politely be called "a data-science nightmare".
+Likely candidates are one of the eight "Nordborg Nextera INDEX" sets.
+It may be best to ask within the lab in this case.
+
+How can you determine which of the indexs was used?
+The first place to look is `Forskalle <https://ngs.vbcf.ac.at/forskalle3/>`_.
+Search (the bar is in the top right) for the sample number of your plate, then
+look under "Adaptor" under "Sample library options" in the upper left box, and
+the index set information should be displayed.
+For example, sample 144456 shows "Nordborg Nextera INDEX set 2..." in this box.
 
 ============================
 Work out which file is which
 ============================
 
-With ``methlab``
-=======================
-
 From the previous section it is clear that if you know the 16-nucleotide adapter
 sequence in the filename and which adapter set was used, you should be able to 
-work out which file corresponds to which plate position. Doing the alignment is
+work out which file corresponds to which plate position. Doing this alignment is
 fairly tedious, and there is no point in people replicating the task, so the
-function ``align_fastq_with_plate_positions`` can doe this automatically.
+function ``align_fastq_with_plate_positions`` can done this automatically.
+This function requires lists of input fastq files and a sample sheet giving the
+details of each sample, and returns a copy of the sample sheet with the paths to
+corresponding fastq files as additional columns
+
+List the fastq files
+--------------------
 
 Using Python import the modules needed and make a list of filenames.
 In this fictional example, imagine you have a folder of pairs of fastq files 
-corresponding to forward and reverse read pairs for each sample.
+corresponding to forward and reverse read pairs for each sample. Files with mate
+pair 1 and 2 are labelled ``R1`` and ``R2`` respectively. Globbing these files
+returns a python list of files names.
 
 .. code-block:: python
 
-    import pandas as pd
     from glob import glob
-    import os
     import methlab as ml
     print("Using methlab version " + ml.__version__)
     # List of fastq files
-    input_files=glob("path/to/bam_files/*fastq")
-
-Pass this list to the function ``align_fastq_with_plate_positions``.
-This function looks for a nucleotide sequence inside each file name and matches
-it to a dataframe giving row and column positions for that sequence.
-It then returns a pandas data frame with a row for each sample, giving sample
-name, and up to two file paths to the data files that correspond to it.
-Single-end data will return a single path, paired-end data return two paths,
-and more than two matches raise an exception. Note that this requires that the
-names you give it come from a single plate, and will throw an error if there are
-multiple samples matching the sample row/column combination.
-
-Sample names are returned as the row/column name; here we specify an optional
-prefix ``t4_p2_`` which adds the temperature and plate ID for these data, so
-sample names will look something like ``t4_p2_G1``.
+    mate1=glob("path/to/bam_files/*_R1_*.fastq.gz")
+    mate2=glob("path/to/bam_files/*_R2_*.fastq.gz")
 
-.. code-block:: python
-
-    ml.align_fastq_with_plate_positions(
-        input_files,
-        adapter_indices = 'nordborg', # specify that we need the Nordborg group custom nextera indices
-        prefix = "t4_p2_"
-    )
+Sample sheet 
+------------
 
-Specifying the adpator index set
-================================
+To line these filenames up with biological samples we need a sample sheet, here
+given as a CSV file and imported as a Pandas dataframe.
 
-You need to specify which adaptor index set was used.
+.. code-block:: python
 
-Since we often use the same index sets over and over again, some commonly used sets are stored internally. These data were run with the 'Nordborg Nextera INDEX' set, which you can use by passing ``nordborg`` to adapter_indices. At the time of writing (July 2023) the lab is moving towards using a single set for everything, which is likely to be the 'Unique Nextera Dual XT' set, which you can use by passing ``dualxt`` to ``adapter_indices``. Note that I have don't have data using the dual XT adapters to test this with, so do some quality control on your data to double check it's working! 
+    sample_sheet = pd.read_csv("tests/test_data/NGS_sample_sheet.csv")
 
-You can specify a custom adaptor set by creating a CSV file giving each adaptor pair.
-This file must contain at least the following columns, but may contain more:
+Here is an example of how a sample sheet might look:
 
-- row : Row letter from A to H
-- col : Column number from 1 to 12
-- seq1 : Nucleotide sequence of index 1
-- seq2 : Nucleotide sequence of index 2
+.. parsed-literal::
+  
+       plate      row  col    plantID  index_set      index1      index2
+    0  2021-007   A    1  H1.2xH2.1-1          4  TTCTCGTGCA  ATACACAGAG
+    1  2021-007   B    1  H1.2xH2.1-2          4  GCCTAACGTG  AGCTCTCAAG
+    2  2021-007   C    1  H1.2xH2.1-3          4  CATTCACGCT  GTTGTACTCA
+    3  2021-007   D    1  H1.2xH2.1-4          4  GCCATATAAC  ACACAATATC
+    4  2021-007   D    1  H1.2xH2.1-4          4  TCGTGCATTC  GCGTTGGTAT
+    5  2021-007   D    1  H1.2xH2.1-4          4  AACCAGCCAC  GCCACAGCAC
+
+This file must include columns ``index1`` and ``index2`` that give the index
+barcodes for each sample.
+See the previous section for where to find these.
+The other columns give information about each sample.
+They can include any information, as long as ``index1`` and ``index2`` are present.
+There may not be duplicate rows of ``index1`` and ``index2``, which in practical
+terms mean that you should look at one sequencing plate at a time.
 
-If the index set contains combinations for more than one plate, include an 
-additional column 'set'.
+Merge filenames and sample sheet
+--------------------------------
 
-For example, here are the first 10 rows of the index file for the Unique Nextera
-Dual XT index set:
+Pass the lists of file paths and the sample sheet to ``align_fastq_with_plate_positions``.
 
-.. parsed-literal::
+.. code-block:: python
+  new_sheet = ml.align_fastq_with_plate_positions(mate1, mate2, sample_sheet)    
 
-    set,row,col,name1,seq1,name2,seq2
-    1,A,1,7001,CGCTCAGTTC,5001,TCGTGGAGCG
-    1,A,2,7002,TATCTGACCT,5002,CTACAAGATA
-    1,A,3,7003,ATATGAGACG,5003,TATAGTAGCT
-    1,A,4,7004,CTTATGGAAT,5004,TGCCTGGTGG
-    1,A,5,7005,TAATCTCGTC,5005,ACATTATCCT
-    1,A,6,7006,GCGCGATGTT,5006,GTCCACTTGT
-    1,A,7,7007,AGAGCACTAG,5007,TGGAACAGTA
-    1,A,8,7008,TGCCTTGATC,5008,CCTTGTTAAT
-    1,A,9,7009,CTACTCAGTC,5009,GTTGATAGTG
+This function looks for a nucleotide sequence inside each filename and matches
+it to the indices in the sample sheet.
```

### Comparing `methlab-0.6.1/docs/modules/methylation_state.rst` & `methlab-0.7.0/docs/modules/methylation_state.rst`

 * *Files identical despite different names*

### Comparing `methlab-0.6.1/methlab/BismarkSam.py` & `methlab-0.7.0/methlab/BismarkSam.py`

 * *Files identical despite different names*

### Comparing `methlab-0.6.1/methlab/CytosineCoverageFile.py` & `methlab-0.7.0/methlab/CytosineCoverageFile.py`

 * *Files identical despite different names*

### Comparing `methlab-0.6.1/methlab/_alogsumexp.py` & `methlab-0.7.0/methlab/_alogsumexp.py`

 * *Files identical despite different names*

### Comparing `methlab-0.6.1/methlab/cli.py` & `methlab-0.7.0/methlab/cli.py`

 * *Files identical despite different names*

### Comparing `methlab-0.6.1/methlab/estimate_beta_parameters.py` & `methlab-0.7.0/methlab/estimate_beta_parameters.py`

 * *Files identical despite different names*

### Comparing `methlab-0.6.1/methlab/methylation_state.py` & `methlab-0.7.0/methlab/methylation_state.py`

 * *Files identical despite different names*

### Comparing `methlab-0.6.1/methlab.egg-info/PKG-INFO` & `methlab-0.7.0/methlab.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: methlab
-Version: 0.6.1
+Version: 0.7.0
 Summary: Python tools for the epiclines ERC project
 Home-page: https://github.com/ellisztamas/methlab
 Author: Tom Ellis
 Author-email: thomas.ellis@gmi.oeaw.ac.at
 License: MIT license
+Description: UNKNOWN
 Keywords: methlab
+Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
-License-File: LICENSE
-License-File: AUTHORS.rst
-Requires-Dist: pandas
-Requires-Dist: numpy
```

### Comparing `methlab-0.6.1/methlab.egg-info/SOURCES.txt` & `methlab-0.7.0/methlab.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -32,22 +32,20 @@
 methlab.egg-info/PKG-INFO
 methlab.egg-info/SOURCES.txt
 methlab.egg-info/dependency_links.txt
 methlab.egg-info/entry_points.txt
 methlab.egg-info/not-zip-safe
 methlab.egg-info/requires.txt
 methlab.egg-info/top_level.txt
-methlab/data/nordborg_nextera_index_sets.csv
-methlab/data/plate_2022-007.csv
-methlab/data/unique_nextera_dual_xt.csv
 tests/__init__.py
 tests/test_BismarkSam.py
 tests/test_CytosineCoverageFile.py
 tests/test_align_fastq_with_plate_positions.py
 tests/test_epiclinestools.py
 tests/test_methylation_state.py
+tests/test_data/NGS_sample_sheet.csv
 tests/test_data/chloroplast.sam
 tests/test_data/gene_read_counts.csv
 tests/test_data/readme.txt
 tests/test_data/strandID.sam
 tests/test_data/test_TAIR10_GFF3_genes_transposons.gff
 tests/test_data/test_coverage2cytosine.txt.gz
```

### Comparing `methlab-0.6.1/setup.cfg` & `methlab-0.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `methlab-0.6.1/setup.py` & `methlab-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `methlab-0.6.1/tests/test_BismarkSam.py` & `methlab-0.7.0/tests/test_BismarkSam.py`

 * *Files identical despite different names*

### Comparing `methlab-0.6.1/tests/test_CytosineCoverageFile.py` & `methlab-0.7.0/tests/test_CytosineCoverageFile.py`

 * *Files identical despite different names*

### Comparing `methlab-0.6.1/tests/test_data/chloroplast.sam` & `methlab-0.7.0/tests/test_data/chloroplast.sam`

 * *Files identical despite different names*

### Comparing `methlab-0.6.1/tests/test_data/gene_read_counts.csv` & `methlab-0.7.0/tests/test_data/gene_read_counts.csv`

 * *Files identical despite different names*

### Comparing `methlab-0.6.1/tests/test_data/readme.txt` & `methlab-0.7.0/tests/test_data/readme.txt`

 * *Files identical despite different names*

### Comparing `methlab-0.6.1/tests/test_data/strandID.sam` & `methlab-0.7.0/tests/test_data/strandID.sam`

 * *Files identical despite different names*

### Comparing `methlab-0.6.1/tests/test_data/test_TAIR10_GFF3_genes_transposons.gff` & `methlab-0.7.0/tests/test_data/test_TAIR10_GFF3_genes_transposons.gff`

 * *Files identical despite different names*

### Comparing `methlab-0.6.1/tests/test_data/test_coverage2cytosine.txt.gz` & `methlab-0.7.0/tests/test_data/test_coverage2cytosine.txt.gz`

 * *Files identical despite different names*

### Comparing `methlab-0.6.1/tests/test_epiclinestools.py` & `methlab-0.7.0/tests/test_epiclinestools.py`

 * *Files identical despite different names*

### Comparing `methlab-0.6.1/tests/test_methylation_state.py` & `methlab-0.7.0/tests/test_methylation_state.py`

 * *Files identical despite different names*

