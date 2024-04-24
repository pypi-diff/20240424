# Comparing `tmp/gtdbtk-2.3.2.tar.gz` & `tmp/gtdbtk-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gtdbtk-2.3.2.tar", last modified: Wed Jul  5 22:39:36 2023, max compression
+gzip compressed data, was "gtdbtk-2.4.0.tar", last modified: Wed Apr 24 01:33:08 2024, max compression
```

## Comparing `gtdbtk-2.3.2.tar` & `gtdbtk-2.4.0.tar`

### file list

```diff
@@ -1,132 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.300113 gtdbtk-2.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35122 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-07-05 22:39:36.300113 gtdbtk-2.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.252113 gtdbtk-2.3.2/gtdbtk/
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11251 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/ani_rep.py
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/ani_screen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.260113 gtdbtk-2.3.2/gtdbtk/biolib_lite/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/biolib_lite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/biolib_lite/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/biolib_lite/custom_help_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/biolib_lite/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/biolib_lite/execute.py
--rw-r--r--   0 runner    (1001) docker     (123)    10587 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/biolib_lite/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/biolib_lite/newick.py
--rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/biolib_lite/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)    16327 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/biolib_lite/prodigal_biolib.py
--rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/biolib_lite/seq_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    30846 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/biolib_lite/taxonomy.py
--rw-r--r--   0 runner    (1001) docker     (123)   117674 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/classify.py
--rw-r--r--   0 runner    (1001) docker     (123)    24439 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.264113 gtdbtk-2.3.2/gtdbtk/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15287 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/config/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/config/output.py
--rw-r--r--   0 runner    (1001) docker     (123)    16476 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/decorate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.268113 gtdbtk-2.3.2/gtdbtk/external/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14798 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/external/fastani.py
--rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/external/fasttree.py
--rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/external/hmm_aligner.py
--rw-r--r--   0 runner    (1001) docker     (123)    12085 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/external/mash.py
--rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/external/pfam_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/external/pplacer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11043 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/external/prodigal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.268113 gtdbtk-2.3.2/gtdbtk/external/pypfam/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.268113 gtdbtk-2.3.2/gtdbtk/external/pypfam/HMM/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1812 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/external/pypfam/HMM/HMMMatch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4876 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/external/pypfam/HMM/HMMResults.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21015 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/external/pypfam/HMM/HMMResultsIO.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2241 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/external/pypfam/HMM/HMMSequence.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2066 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/external/pypfam/HMM/HMMUnit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/external/pypfam/HMM/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.272113 gtdbtk-2.3.2/gtdbtk/external/pypfam/Scan/
--rwxr-xr-x   0 runner    (1001) docker     (123)    22327 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/external/pypfam/Scan/PfamScan.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/external/pypfam/Scan/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/external/pypfam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/external/tigrfam_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.276113 gtdbtk-2.3.2/gtdbtk/files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/files/batchfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/files/classify_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/files/gtdb_radii.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.276113 gtdbtk-2.3.2/gtdbtk/files/marker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/files/marker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/files/marker/copy_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     8235 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/files/marker/tophit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/files/marker_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/files/missing_genomes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/files/pplacer_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.280113 gtdbtk-2.3.2/gtdbtk/files/prodigal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/files/prodigal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/files/prodigal/tln_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/files/prodigal/tln_table_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/files/red_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/files/stage_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/files/tree_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     8242 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/infer_ranks.py
--rw-r--r--   0 runner    (1001) docker     (123)    54256 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    34860 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/markers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12238 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.284113 gtdbtk-2.3.2/gtdbtk/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/model/enum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.284113 gtdbtk-2.3.2/gtdbtk/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/pipeline/align.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/pipeline/export_msa.py
--rw-r--r--   0 runner    (1001) docker     (123)    18011 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/relative_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/reroot_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    21477 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/split.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.240113 gtdbtk-2.3.2/gtdbtk/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.244113 gtdbtk-2.3.2/gtdbtk/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.292113 gtdbtk-2.3.2/gtdbtk/tests/data/genomes/
--rw-r--r--   0 runner    (1001) docker     (123)  2973983 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/tests/data/genomes/genome_1.fna
--rw-r--r--   0 runner    (1001) docker     (123)  1292421 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/tests/data/genomes/genome_2.fna
--rw-r--r--   0 runner    (1001) docker     (123)  1210030 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/tests/data/genomes/genome_3.fna
--rw-r--r--   0 runner    (1001) docker     (123)    15764 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/tools.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12742 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/trim_msa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.256113 gtdbtk-2.3.2/gtdbtk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-07-05 22:39:36.000000 gtdbtk-2.3.2/gtdbtk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-07-05 22:39:36.000000 gtdbtk-2.3.2/gtdbtk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 22:39:36.000000 gtdbtk-2.3.2/gtdbtk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-05 22:39:36.000000 gtdbtk-2.3.2/gtdbtk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-05 22:39:36.000000 gtdbtk-2.3.2/gtdbtk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-05 22:39:36.000000 gtdbtk-2.3.2/gtdbtk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 22:39:36.300113 gtdbtk-2.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.296113 gtdbtk-2.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/test_classify.py
--rw-r--r--   0 runner    (1001) docker     (123)    13471 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.296113 gtdbtk-2.3.2/tests/test_gtdbtk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/test_gtdbtk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14323 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/test_gtdbtk/test__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.296113 gtdbtk-2.3.2/tests/test_gtdbtk/test_biolib_lite/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/test_gtdbtk/test_biolib_lite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/test_gtdbtk/test_biolib_lite/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/test_gtdbtk/test_biolib_lite/test_newick.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/test_gtdbtk/test_biolib_lite/test_seq_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/test_gtdbtk/test_biolib_lite/test_taxonomy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.296113 gtdbtk-2.3.2/tests/test_gtdbtk/test_external/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/test_gtdbtk/test_external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/test_gtdbtk/test_external/test_fastani.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/test_gtdbtk/test_external/test_fasttree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.296113 gtdbtk-2.3.2/tests/test_gtdbtk/test_files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/test_gtdbtk/test_files/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.300113 gtdbtk-2.3.2/tests/test_gtdbtk/test_files/test_marker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/test_gtdbtk/test_files/test_marker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10671 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/test_gtdbtk/test_files/test_marker/test_copy_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     8972 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/test_gtdbtk/test_files/test_marker/test_tophit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.300113 gtdbtk-2.3.2/tests/test_gtdbtk/test_files/test_prodigal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/test_gtdbtk/test_files/test_prodigal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/test_gtdbtk/test_files/test_prodigal/test_tln_table_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    12364 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/test_gtdbtk/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/test_gtdbtk/test_markers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/test_gtdbtk/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/test_gtdbtk/test_trim_msa.py
+drwxr-xr-x   0 aaron      (501) staff       (20)        0 2024-04-24 01:33:08.620166 gtdbtk-2.4.0/
+-rw-r--r--   0 aaron      (501) staff       (20)    35122 2021-10-15 03:28:50.000000 gtdbtk-2.4.0/LICENSE
+-rw-r--r--   0 aaron      (501) staff       (20)     7420 2024-04-24 01:33:08.619685 gtdbtk-2.4.0/PKG-INFO
+-rw-r--r--   0 aaron      (501) staff       (20)     6318 2024-04-24 01:24:52.000000 gtdbtk-2.4.0/README.md
+drwxr-xr-x   0 aaron      (501) staff       (20)        0 2024-04-24 01:33:08.548601 gtdbtk-2.4.0/gtdbtk/
+-rw-r--r--   0 aaron      (501) staff       (20)     1920 2024-04-24 01:24:52.000000 gtdbtk-2.4.0/gtdbtk/__init__.py
+-rw-r--r--   0 aaron      (501) staff       (20)     5930 2023-08-24 11:57:27.000000 gtdbtk-2.4.0/gtdbtk/__main__.py
+-rw-r--r--   0 aaron      (501) staff       (20)    11207 2024-04-24 01:24:52.000000 gtdbtk-2.4.0/gtdbtk/ani_rep.py
+-rw-r--r--   0 aaron      (501) staff       (20)     6051 2024-04-24 01:24:52.000000 gtdbtk-2.4.0/gtdbtk/ani_screen.py
+drwxr-xr-x   0 aaron      (501) staff       (20)        0 2024-04-24 01:33:08.560157 gtdbtk-2.4.0/gtdbtk/biolib_lite/
+-rw-r--r--   0 aaron      (501) staff       (20)        0 2021-10-15 03:28:50.000000 gtdbtk-2.4.0/gtdbtk/biolib_lite/__init__.py
+-rw-r--r--   0 aaron      (501) staff       (20)     5241 2022-09-24 02:28:47.000000 gtdbtk-2.4.0/gtdbtk/biolib_lite/common.py
+-rw-r--r--   0 aaron      (501) staff       (20)     4533 2022-06-02 23:14:19.000000 gtdbtk-2.4.0/gtdbtk/biolib_lite/custom_help_formatter.py
+-rw-r--r--   0 aaron      (501) staff       (20)     2315 2021-10-15 03:28:50.000000 gtdbtk-2.4.0/gtdbtk/biolib_lite/exceptions.py
+-rw-r--r--   0 aaron      (501) staff       (20)     4196 2022-09-24 02:28:47.000000 gtdbtk-2.4.0/gtdbtk/biolib_lite/execute.py
+-rw-r--r--   0 aaron      (501) staff       (20)    10587 2023-08-24 11:57:27.000000 gtdbtk-2.4.0/gtdbtk/biolib_lite/logger.py
+-rw-r--r--   0 aaron      (501) staff       (20)     2877 2021-10-15 03:28:50.000000 gtdbtk-2.4.0/gtdbtk/biolib_lite/newick.py
+-rw-r--r--   0 aaron      (501) staff       (20)     9996 2021-10-15 03:28:50.000000 gtdbtk-2.4.0/gtdbtk/biolib_lite/parallel.py
+-rw-r--r--   0 aaron      (501) staff       (20)    16569 2024-04-24 01:24:52.000000 gtdbtk-2.4.0/gtdbtk/biolib_lite/prodigal_biolib.py
+-rw-r--r--   0 aaron      (501) staff       (20)     7394 2022-09-24 02:28:47.000000 gtdbtk-2.4.0/gtdbtk/biolib_lite/seq_io.py
+-rw-r--r--   0 aaron      (501) staff       (20)    30846 2022-06-02 23:14:19.000000 gtdbtk-2.4.0/gtdbtk/biolib_lite/taxonomy.py
+-rw-r--r--   0 aaron      (501) staff       (20)   121901 2024-04-24 01:24:52.000000 gtdbtk-2.4.0/gtdbtk/classify.py
+-rw-r--r--   0 aaron      (501) staff       (20)    24452 2024-04-24 01:24:52.000000 gtdbtk-2.4.0/gtdbtk/cli.py
+drwxr-xr-x   0 aaron      (501) staff       (20)        0 2024-04-24 01:33:08.562214 gtdbtk-2.4.0/gtdbtk/config/
+-rw-r--r--   0 aaron      (501) staff       (20)        0 2021-10-15 03:28:50.000000 gtdbtk-2.4.0/gtdbtk/config/__init__.py
+-rw-r--r--   0 aaron      (501) staff       (20)    14509 2024-04-24 01:24:52.000000 gtdbtk-2.4.0/gtdbtk/config/common.py
+-rw-r--r--   0 aaron      (501) staff       (20)     6167 2024-04-24 01:24:52.000000 gtdbtk-2.4.0/gtdbtk/config/output.py
+-rw-r--r--   0 aaron      (501) staff       (20)    16476 2023-02-14 00:34:47.000000 gtdbtk-2.4.0/gtdbtk/decorate.py
+-rw-r--r--   0 aaron      (501) staff       (20)     5280 2024-04-24 01:24:52.000000 gtdbtk-2.4.0/gtdbtk/exceptions.py
+drwxr-xr-x   0 aaron      (501) staff       (20)        0 2024-04-24 01:33:08.567951 gtdbtk-2.4.0/gtdbtk/external/
+-rw-r--r--   0 aaron      (501) staff       (20)        0 2021-10-15 03:28:50.000000 gtdbtk-2.4.0/gtdbtk/external/__init__.py
+-rw-r--r--   0 aaron      (501) staff       (20)    14798 2023-02-14 00:34:47.000000 gtdbtk-2.4.0/gtdbtk/external/fastani.py
+-rw-r--r--   0 aaron      (501) staff       (20)     5805 2022-09-24 02:28:47.000000 gtdbtk-2.4.0/gtdbtk/external/fasttree.py
+-rw-r--r--   0 aaron      (501) staff       (20)    13847 2023-02-14 00:34:47.000000 gtdbtk-2.4.0/gtdbtk/external/hmm_aligner.py
+-rw-r--r--   0 aaron      (501) staff       (20)    12085 2023-08-24 11:57:27.000000 gtdbtk-2.4.0/gtdbtk/external/mash.py
+-rw-r--r--   0 aaron      (501) staff       (20)     6993 2023-02-14 00:34:47.000000 gtdbtk-2.4.0/gtdbtk/external/pfam_search.py
+-rw-r--r--   0 aaron      (501) staff       (20)    10746 2024-04-24 01:24:52.000000 gtdbtk-2.4.0/gtdbtk/external/pplacer.py
+-rw-r--r--   0 aaron      (501) staff       (20)    11977 2024-04-24 01:24:52.000000 gtdbtk-2.4.0/gtdbtk/external/prodigal.py
+drwxr-xr-x   0 aaron      (501) staff       (20)        0 2024-04-24 01:33:08.568621 gtdbtk-2.4.0/gtdbtk/external/pypfam/
+drwxr-xr-x   0 aaron      (501) staff       (20)        0 2024-04-24 01:33:08.572691 gtdbtk-2.4.0/gtdbtk/external/pypfam/HMM/
+-rwxr-xr-x   0 aaron      (501) staff       (20)     1812 2022-09-12 00:19:06.000000 gtdbtk-2.4.0/gtdbtk/external/pypfam/HMM/HMMMatch.py
+-rwxr-xr-x   0 aaron      (501) staff       (20)     4876 2022-09-24 02:28:47.000000 gtdbtk-2.4.0/gtdbtk/external/pypfam/HMM/HMMResults.py
+-rwxr-xr-x   0 aaron      (501) staff       (20)    21015 2022-09-24 02:28:47.000000 gtdbtk-2.4.0/gtdbtk/external/pypfam/HMM/HMMResultsIO.py
+-rwxr-xr-x   0 aaron      (501) staff       (20)     2241 2021-10-15 03:28:50.000000 gtdbtk-2.4.0/gtdbtk/external/pypfam/HMM/HMMSequence.py
+-rwxr-xr-x   0 aaron      (501) staff       (20)     2066 2022-09-12 00:19:06.000000 gtdbtk-2.4.0/gtdbtk/external/pypfam/HMM/HMMUnit.py
+-rwxr-xr-x   0 aaron      (501) staff       (20)        0 2021-10-15 03:28:50.000000 gtdbtk-2.4.0/gtdbtk/external/pypfam/HMM/__init__.py
+drwxr-xr-x   0 aaron      (501) staff       (20)        0 2024-04-24 01:33:08.574277 gtdbtk-2.4.0/gtdbtk/external/pypfam/Scan/
+-rwxr-xr-x   0 aaron      (501) staff       (20)    22327 2023-03-23 03:58:22.000000 gtdbtk-2.4.0/gtdbtk/external/pypfam/Scan/PfamScan.py
+-rwxr-xr-x   0 aaron      (501) staff       (20)        0 2021-10-15 03:28:50.000000 gtdbtk-2.4.0/gtdbtk/external/pypfam/Scan/__init__.py
+-rwxr-xr-x   0 aaron      (501) staff       (20)        0 2021-10-15 03:28:50.000000 gtdbtk-2.4.0/gtdbtk/external/pypfam/__init__.py
+-rw-r--r--   0 aaron      (501) staff       (20)     9478 2024-04-24 01:24:52.000000 gtdbtk-2.4.0/gtdbtk/external/skani.py
+-rw-r--r--   0 aaron      (501) staff       (20)     9177 2023-02-14 00:34:47.000000 gtdbtk-2.4.0/gtdbtk/external/tigrfam_search.py
+drwxr-xr-x   0 aaron      (501) staff       (20)        0 2024-04-24 01:33:08.579345 gtdbtk-2.4.0/gtdbtk/files/
+-rw-r--r--   0 aaron      (501) staff       (20)        0 2023-02-14 00:34:47.000000 gtdbtk-2.4.0/gtdbtk/files/__init__.py
+-rw-r--r--   0 aaron      (501) staff       (20)     2344 2023-02-14 00:34:47.000000 gtdbtk-2.4.0/gtdbtk/files/batchfile.py
+-rw-r--r--   0 aaron      (501) staff       (20)     9744 2024-04-24 01:24:52.000000 gtdbtk-2.4.0/gtdbtk/files/classify_summary.py
+-rw-r--r--   0 aaron      (501) staff       (20)     2253 2023-08-24 11:57:27.000000 gtdbtk-2.4.0/gtdbtk/files/gtdb_radii.py
+drwxr-xr-x   0 aaron      (501) staff       (20)        0 2024-04-24 01:33:08.580733 gtdbtk-2.4.0/gtdbtk/files/marker/
+-rw-r--r--   0 aaron      (501) staff       (20)        0 2023-02-14 00:34:47.000000 gtdbtk-2.4.0/gtdbtk/files/marker/__init__.py
+-rw-r--r--   0 aaron      (501) staff       (20)     8581 2023-08-24 11:57:27.000000 gtdbtk-2.4.0/gtdbtk/files/marker/copy_number.py
+-rw-r--r--   0 aaron      (501) staff       (20)     8235 2023-02-14 00:34:47.000000 gtdbtk-2.4.0/gtdbtk/files/marker/tophit.py
+-rw-r--r--   0 aaron      (501) staff       (20)     4036 2023-08-24 11:57:27.000000 gtdbtk-2.4.0/gtdbtk/files/marker_info.py
+-rw-r--r--   0 aaron      (501) staff       (20)     3056 2023-02-14 00:34:47.000000 gtdbtk-2.4.0/gtdbtk/files/missing_genomes.py
+-rw-r--r--   0 aaron      (501) staff       (20)     5459 2023-02-14 00:34:47.000000 gtdbtk-2.4.0/gtdbtk/files/pplacer_classification.py
+drwxr-xr-x   0 aaron      (501) staff       (20)        0 2024-04-24 01:33:08.582097 gtdbtk-2.4.0/gtdbtk/files/prodigal/
+-rw-r--r--   0 aaron      (501) staff       (20)        0 2023-02-14 00:34:47.000000 gtdbtk-2.4.0/gtdbtk/files/prodigal/__init__.py
+-rw-r--r--   0 aaron      (501) staff       (20)     2616 2023-02-14 00:34:47.000000 gtdbtk-2.4.0/gtdbtk/files/prodigal/tln_table.py
+-rw-r--r--   0 aaron      (501) staff       (20)     2919 2023-02-14 00:34:47.000000 gtdbtk-2.4.0/gtdbtk/files/prodigal/tln_table_summary.py
+-rw-r--r--   0 aaron      (501) staff       (20)     2714 2023-08-24 11:57:27.000000 gtdbtk-2.4.0/gtdbtk/files/red_dict.py
+-rw-r--r--   0 aaron      (501) staff       (20)     7465 2024-04-24 01:24:52.000000 gtdbtk-2.4.0/gtdbtk/files/stage_logger.py
+-rw-r--r--   0 aaron      (501) staff       (20)     4261 2023-02-14 00:34:47.000000 gtdbtk-2.4.0/gtdbtk/files/tree_mapping.py
+-rw-r--r--   0 aaron      (501) staff       (20)     8242 2023-08-24 11:57:27.000000 gtdbtk-2.4.0/gtdbtk/infer_ranks.py
+-rw-r--r--   0 aaron      (501) staff       (20)    54235 2024-04-24 01:24:52.000000 gtdbtk-2.4.0/gtdbtk/main.py
+-rw-r--r--   0 aaron      (501) staff       (20)    35629 2024-04-24 01:24:52.000000 gtdbtk-2.4.0/gtdbtk/markers.py
+-rw-r--r--   0 aaron      (501) staff       (20)    12236 2024-04-24 01:24:52.000000 gtdbtk-2.4.0/gtdbtk/misc.py
+drwxr-xr-x   0 aaron      (501) staff       (20)        0 2024-04-24 01:33:08.582811 gtdbtk-2.4.0/gtdbtk/model/
+-rw-r--r--   0 aaron      (501) staff       (20)        0 2022-06-02 23:14:19.000000 gtdbtk-2.4.0/gtdbtk/model/__init__.py
+-rw-r--r--   0 aaron      (501) staff       (20)       85 2022-09-24 02:28:47.000000 gtdbtk-2.4.0/gtdbtk/model/enum.py
+drwxr-xr-x   0 aaron      (501) staff       (20)        0 2024-04-24 01:33:08.584370 gtdbtk-2.4.0/gtdbtk/pipeline/
+-rw-r--r--   0 aaron      (501) staff       (20)        0 2022-06-02 23:14:19.000000 gtdbtk-2.4.0/gtdbtk/pipeline/__init__.py
+-rw-r--r--   0 aaron      (501) staff       (20)     8520 2023-08-24 11:57:27.000000 gtdbtk-2.4.0/gtdbtk/pipeline/align.py
+-rw-r--r--   0 aaron      (501) staff       (20)      768 2023-08-24 11:57:27.000000 gtdbtk-2.4.0/gtdbtk/pipeline/export_msa.py
+-rw-r--r--   0 aaron      (501) staff       (20)    18011 2021-10-15 03:28:50.000000 gtdbtk-2.4.0/gtdbtk/relative_distance.py
+-rw-r--r--   0 aaron      (501) staff       (20)     6146 2024-04-24 01:24:52.000000 gtdbtk-2.4.0/gtdbtk/reroot_tree.py
+-rw-r--r--   0 aaron      (501) staff       (20)    21477 2023-08-24 11:57:27.000000 gtdbtk-2.4.0/gtdbtk/split.py
+drwxr-xr-x   0 aaron      (501) staff       (20)        0 2024-04-24 01:33:08.531849 gtdbtk-2.4.0/gtdbtk/tests/
+drwxr-xr-x   0 aaron      (501) staff       (20)        0 2024-04-24 01:33:08.531967 gtdbtk-2.4.0/gtdbtk/tests/data/
+drwxr-xr-x   0 aaron      (501) staff       (20)        0 2024-04-24 01:33:08.598377 gtdbtk-2.4.0/gtdbtk/tests/data/genomes/
+-rw-r--r--   0 aaron      (501) staff       (20)  2973983 2021-10-15 03:28:50.000000 gtdbtk-2.4.0/gtdbtk/tests/data/genomes/genome_1.fna
+-rw-r--r--   0 aaron      (501) staff       (20)  1292421 2021-10-15 03:28:50.000000 gtdbtk-2.4.0/gtdbtk/tests/data/genomes/genome_2.fna
+-rw-r--r--   0 aaron      (501) staff       (20)  1210030 2021-10-15 03:28:50.000000 gtdbtk-2.4.0/gtdbtk/tests/data/genomes/genome_3.fna
+-rw-r--r--   0 aaron      (501) staff       (20)    15756 2024-04-24 01:24:52.000000 gtdbtk-2.4.0/gtdbtk/tools.py
+-rwxr-xr-x   0 aaron      (501) staff       (20)    12749 2024-04-24 01:24:52.000000 gtdbtk-2.4.0/gtdbtk/trim_msa.py
+drwxr-xr-x   0 aaron      (501) staff       (20)        0 2024-04-24 01:33:08.619062 gtdbtk-2.4.0/gtdbtk.egg-info/
+-rw-r--r--   0 aaron      (501) staff       (20)     7420 2024-04-24 01:33:08.000000 gtdbtk-2.4.0/gtdbtk.egg-info/PKG-INFO
+-rw-r--r--   0 aaron      (501) staff       (20)     3387 2024-04-24 01:33:08.000000 gtdbtk-2.4.0/gtdbtk.egg-info/SOURCES.txt
+-rw-r--r--   0 aaron      (501) staff       (20)        1 2024-04-24 01:33:08.000000 gtdbtk-2.4.0/gtdbtk.egg-info/dependency_links.txt
+-rw-r--r--   0 aaron      (501) staff       (20)       48 2024-04-24 01:33:08.000000 gtdbtk-2.4.0/gtdbtk.egg-info/entry_points.txt
+-rw-r--r--   0 aaron      (501) staff       (20)       50 2024-04-24 01:33:08.000000 gtdbtk-2.4.0/gtdbtk.egg-info/requires.txt
+-rw-r--r--   0 aaron      (501) staff       (20)       13 2024-04-24 01:33:08.000000 gtdbtk-2.4.0/gtdbtk.egg-info/top_level.txt
+-rw-r--r--   0 aaron      (501) staff       (20)       38 2024-04-24 01:33:08.620279 gtdbtk-2.4.0/setup.cfg
+-rw-r--r--   0 aaron      (501) staff       (20)     1829 2024-04-24 01:24:52.000000 gtdbtk-2.4.0/setup.py
+drwxr-xr-x   0 aaron      (501) staff       (20)        0 2024-04-24 01:33:08.606315 gtdbtk-2.4.0/tests/
+-rw-r--r--   0 aaron      (501) staff       (20)        0 2021-10-15 03:28:50.000000 gtdbtk-2.4.0/tests/__init__.py
+-rw-r--r--   0 aaron      (501) staff       (20)      773 2021-10-15 03:28:50.000000 gtdbtk-2.4.0/tests/common.py
+-rw-r--r--   0 aaron      (501) staff       (20)     6862 2023-08-24 11:57:27.000000 gtdbtk-2.4.0/tests/test_classify.py
+-rw-r--r--   0 aaron      (501) staff       (20)    13471 2022-06-28 05:49:01.000000 gtdbtk-2.4.0/tests/test_cli.py
+drwxr-xr-x   0 aaron      (501) staff       (20)        0 2024-04-24 01:33:08.610941 gtdbtk-2.4.0/tests/test_gtdbtk/
+-rw-r--r--   0 aaron      (501) staff       (20)        0 2021-10-15 03:28:51.000000 gtdbtk-2.4.0/tests/test_gtdbtk/__init__.py
+-rw-r--r--   0 aaron      (501) staff       (20)    14323 2023-08-24 11:57:27.000000 gtdbtk-2.4.0/tests/test_gtdbtk/test__main__.py
+drwxr-xr-x   0 aaron      (501) staff       (20)        0 2024-04-24 01:33:08.613546 gtdbtk-2.4.0/tests/test_gtdbtk/test_biolib_lite/
+-rw-r--r--   0 aaron      (501) staff       (20)        0 2021-10-15 03:28:51.000000 gtdbtk-2.4.0/tests/test_gtdbtk/test_biolib_lite/__init__.py
+-rw-r--r--   0 aaron      (501) staff       (20)     3800 2021-10-15 03:28:51.000000 gtdbtk-2.4.0/tests/test_gtdbtk/test_biolib_lite/test_common.py
+-rw-r--r--   0 aaron      (501) staff       (20)     1839 2021-10-15 03:28:51.000000 gtdbtk-2.4.0/tests/test_gtdbtk/test_biolib_lite/test_newick.py
+-rw-r--r--   0 aaron      (501) staff       (20)     2771 2021-10-15 03:28:51.000000 gtdbtk-2.4.0/tests/test_gtdbtk/test_biolib_lite/test_seq_io.py
+-rw-r--r--   0 aaron      (501) staff       (20)     3222 2022-06-02 23:14:19.000000 gtdbtk-2.4.0/tests/test_gtdbtk/test_biolib_lite/test_taxonomy.py
+drwxr-xr-x   0 aaron      (501) staff       (20)        0 2024-04-24 01:33:08.615648 gtdbtk-2.4.0/tests/test_gtdbtk/test_external/
+-rw-r--r--   0 aaron      (501) staff       (20)        0 2021-10-15 03:28:51.000000 gtdbtk-2.4.0/tests/test_gtdbtk/test_external/__init__.py
+-rw-r--r--   0 aaron      (501) staff       (20)     4924 2023-08-24 11:57:27.000000 gtdbtk-2.4.0/tests/test_gtdbtk/test_external/test_fastani.py
+-rw-r--r--   0 aaron      (501) staff       (20)     2837 2024-04-24 01:24:52.000000 gtdbtk-2.4.0/tests/test_gtdbtk/test_external/test_fasttree.py
+-rw-r--r--   0 aaron      (501) staff       (20)     3839 2024-04-24 01:24:52.000000 gtdbtk-2.4.0/tests/test_gtdbtk/test_external/test_skani.py
+drwxr-xr-x   0 aaron      (501) staff       (20)        0 2024-04-24 01:33:08.615982 gtdbtk-2.4.0/tests/test_gtdbtk/test_files/
+-rw-r--r--   0 aaron      (501) staff       (20)        0 2023-02-14 00:34:47.000000 gtdbtk-2.4.0/tests/test_gtdbtk/test_files/__init__.py
+drwxr-xr-x   0 aaron      (501) staff       (20)        0 2024-04-24 01:33:08.617353 gtdbtk-2.4.0/tests/test_gtdbtk/test_files/test_marker/
+-rw-r--r--   0 aaron      (501) staff       (20)        0 2023-02-14 00:34:47.000000 gtdbtk-2.4.0/tests/test_gtdbtk/test_files/test_marker/__init__.py
+-rw-r--r--   0 aaron      (501) staff       (20)    10671 2023-02-14 00:34:47.000000 gtdbtk-2.4.0/tests/test_gtdbtk/test_files/test_marker/test_copy_number.py
+-rw-r--r--   0 aaron      (501) staff       (20)     8972 2023-02-14 00:34:47.000000 gtdbtk-2.4.0/tests/test_gtdbtk/test_files/test_marker/test_tophit.py
+drwxr-xr-x   0 aaron      (501) staff       (20)        0 2024-04-24 01:33:08.618488 gtdbtk-2.4.0/tests/test_gtdbtk/test_files/test_prodigal/
+-rw-r--r--   0 aaron      (501) staff       (20)        0 2023-02-14 00:34:47.000000 gtdbtk-2.4.0/tests/test_gtdbtk/test_files/test_prodigal/__init__.py
+-rw-r--r--   0 aaron      (501) staff       (20)     2707 2023-02-14 00:34:47.000000 gtdbtk-2.4.0/tests/test_gtdbtk/test_files/test_prodigal/test_tln_table_summary.py
+-rw-r--r--   0 aaron      (501) staff       (20)    12364 2022-06-02 23:14:19.000000 gtdbtk-2.4.0/tests/test_gtdbtk/test_main.py
+-rw-r--r--   0 aaron      (501) staff       (20)     3796 2021-10-15 03:28:51.000000 gtdbtk-2.4.0/tests/test_gtdbtk/test_markers.py
+-rw-r--r--   0 aaron      (501) staff       (20)     6176 2022-06-02 23:14:19.000000 gtdbtk-2.4.0/tests/test_gtdbtk/test_tools.py
+-rw-r--r--   0 aaron      (501) staff       (20)     2264 2021-10-15 03:28:51.000000 gtdbtk-2.4.0/tests/test_gtdbtk/test_trim_msa.py
```

### Comparing `gtdbtk-2.3.2/LICENSE` & `gtdbtk-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/PKG-INFO` & `gtdbtk-2.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gtdbtk
-Version: 2.3.2
+Version: 2.4.0
 Summary: A toolkit for assigning objective taxonomic classifications to bacterial and archaeal genomes.
 Home-page: https://github.com/Ecogenomics/GTDBTk
 Author: Pierre-Alain Chaumeil, Aaron Mussig and Donovan Parks
 Author-email: p.chaumeil@uq.edu.au
 Maintainer: Pierre-Alain Chaumeil, Aaron Mussig and Donovan Parks
 Maintainer-email: donovan.parks@gmail.com
 License: GPL3
@@ -16,14 +16,18 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: dendropy~=4.1
+Requires-Dist: numpy~=1.9
+Requires-Dist: tqdm~=4.35
+Requires-Dist: pydantic~=1.9
 
 # GTDB-Tk
 
 [![PyPI](https://img.shields.io/pypi/v/gtdbtk.svg)](https://pypi.python.org/pypi/gtdbtk)
 [![PyPI Downloads](https://pepy.tech/badge/gtdbtk)](https://pepy.tech/project/gtdbtk)
 [![Bioconda](https://img.shields.io/conda/vn/bioconda/gtdbtk.svg?color=43b02a)](https://anaconda.org/bioconda/gtdbtk)
 [![BioConda Downloads](https://img.shields.io/conda/dn/bioconda/gtdbtk.svg?style=flag&label=downloads&color=43b02a)](https://anaconda.org/bioconda/gtdbtk)
@@ -56,16 +60,16 @@
 ## 📖 Documentation
 
 Documentation for GTDB-Tk can be found [here](https://ecogenomics.github.io/GTDBTk/).
 
 
 ## ✨ New Features
 
-GTDB-Tk v2.3.0+ includes the following new features:
-- New functionality ``convert_to_species`` function to convert GTDB genome IDs to GTDB species names
+GTDB-Tk v2.4.0+ includes the following new features:
+- `FastANI` has been replaced by `skani` as the primary tool for computing Average Nucleotide Identity (ANI).Users may notice slight variations in the results compared to those obtained using `FastANI`.
 
 
 ## 📈 Performance
 Using ANI screen "can" reduce computation by >50%, although it depends on the set of input genomes. A set of input genomes consisting primarily of new species will not benefit from ANI screen as much as a set of genomes that are largely assigned to GTDB species clusters. In the latter case, the ANI screen will reduce the number of genomes that need to be classified by pplacer which reduces computation time substantially (between 25% and 60% in our testing).
 
 ## 📚 References
 
@@ -82,14 +86,15 @@
 * Parks DH, et al. 2018. [A standardized bacterial taxonomy based on genome phylogeny substantially revises the tree of life](https://www.nature.com/articles/nbt.4229). <i>Nature Biotechnology</i>, http://dx.doi.org/10.1038/nbt.4229.
  
 
 We strongly encourage you to cite the following 3rd party dependencies:
 
 * Matsen FA, et al. 2010. [pplacer: linear time maximum-likelihood and Bayesian phylogenetic placement of sequences onto a fixed reference tree](https://www.ncbi.nlm.nih.gov/pubmed/21034504). <i>BMC Bioinformatics</i>, 11:538.
 * Jain C, et al. 2019. [High-throughput ANI Analysis of 90K Prokaryotic Genomes Reveals Clear Species Boundaries](https://www.nature.com/articles/s41467-018-07641-9). <i>Nat. Communications</i>, doi: 10.1038/s41467-018-07641-9.
+* Shaw J. and Yu Y.W. 2023. [Fast and robust metagenomic sequence comparison through sparse chaining with skani](https://www.nature.com/articles/s41592-023-02018-3). <i>Nature Methods</i>, 20, pages1661–1665 (2023).
 * Hyatt D, et al. 2010. [Prodigal: prokaryotic gene recognition and translation initiation site identification](https://www.ncbi.nlm.nih.gov/pubmed/20211023). <i>BMC Bioinformatics</i>, 11:119. doi: 10.1186/1471-2105-11-119.
 * Price MN, et al. 2010. [FastTree 2 - Approximately Maximum-Likelihood Trees for Large Alignments](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2835736/). <i>PLoS One</i>, 5, e9490.
 * Eddy SR. 2011. [Accelerated profile HMM searches](https://www.ncbi.nlm.nih.gov/pubmed/22039361). <i>PLOS Comp. Biol.</i>, 7:e1002195.
 * Ondov BD, et al. 2016. [Mash: fast genome and metagenome distance estimation using MinHash](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-016-0997-x). <i>Genome Biol</i> 17, 132. doi: 10.1186/s13059-016-0997-x.
 
 
 ## © Copyright
```

### Comparing `gtdbtk-2.3.2/README.md` & `gtdbtk-2.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -33,16 +33,16 @@
 ## 📖 Documentation
 
 Documentation for GTDB-Tk can be found [here](https://ecogenomics.github.io/GTDBTk/).
 
 
 ## ✨ New Features
 
-GTDB-Tk v2.3.0+ includes the following new features:
-- New functionality ``convert_to_species`` function to convert GTDB genome IDs to GTDB species names
+GTDB-Tk v2.4.0+ includes the following new features:
+- `FastANI` has been replaced by `skani` as the primary tool for computing Average Nucleotide Identity (ANI).Users may notice slight variations in the results compared to those obtained using `FastANI`.
 
 
 ## 📈 Performance
 Using ANI screen "can" reduce computation by >50%, although it depends on the set of input genomes. A set of input genomes consisting primarily of new species will not benefit from ANI screen as much as a set of genomes that are largely assigned to GTDB species clusters. In the latter case, the ANI screen will reduce the number of genomes that need to be classified by pplacer which reduces computation time substantially (between 25% and 60% in our testing).
 
 ## 📚 References
 
@@ -59,14 +59,15 @@
 * Parks DH, et al. 2018. [A standardized bacterial taxonomy based on genome phylogeny substantially revises the tree of life](https://www.nature.com/articles/nbt.4229). <i>Nature Biotechnology</i>, http://dx.doi.org/10.1038/nbt.4229.
  
 
 We strongly encourage you to cite the following 3rd party dependencies:
 
 * Matsen FA, et al. 2010. [pplacer: linear time maximum-likelihood and Bayesian phylogenetic placement of sequences onto a fixed reference tree](https://www.ncbi.nlm.nih.gov/pubmed/21034504). <i>BMC Bioinformatics</i>, 11:538.
 * Jain C, et al. 2019. [High-throughput ANI Analysis of 90K Prokaryotic Genomes Reveals Clear Species Boundaries](https://www.nature.com/articles/s41467-018-07641-9). <i>Nat. Communications</i>, doi: 10.1038/s41467-018-07641-9.
+* Shaw J. and Yu Y.W. 2023. [Fast and robust metagenomic sequence comparison through sparse chaining with skani](https://www.nature.com/articles/s41592-023-02018-3). <i>Nature Methods</i>, 20, pages1661–1665 (2023).
 * Hyatt D, et al. 2010. [Prodigal: prokaryotic gene recognition and translation initiation site identification](https://www.ncbi.nlm.nih.gov/pubmed/20211023). <i>BMC Bioinformatics</i>, 11:119. doi: 10.1186/1471-2105-11-119.
 * Price MN, et al. 2010. [FastTree 2 - Approximately Maximum-Likelihood Trees for Large Alignments](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2835736/). <i>PLoS One</i>, 5, e9490.
 * Eddy SR. 2011. [Accelerated profile HMM searches](https://www.ncbi.nlm.nih.gov/pubmed/22039361). <i>PLOS Comp. Biol.</i>, 7:e1002195.
 * Ondov BD, et al. 2016. [Mash: fast genome and metagenome distance estimation using MinHash](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-016-0997-x). <i>Genome Biol</i> 17, 132. doi: 10.1186/s13059-016-0997-x.
 
 
 ## © Copyright
```

### Comparing `gtdbtk-2.3.2/gtdbtk/__init__.py` & `gtdbtk-2.4.0/gtdbtk/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 __maintainer__ = 'Pierre-Alain Chaumeil, Aaron Mussig and Donovan Parks'
 __maintainer_email__ = 'donovan.parks@gmail.com'
 __name__ = 'gtdbtk'
 __python_requires__ = '>=3.6'
 __status__ = 'Production'
 __title__ = 'GTDB-Tk'
 __url__ = 'https://github.com/Ecogenomics/GTDBTk'
-__version__ = '2.3.2'
+__version__ = '2.4.0'
```

### Comparing `gtdbtk-2.3.2/gtdbtk/__main__.py` & `gtdbtk-2.4.0/gtdbtk/__main__.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/gtdbtk/ani_rep.py` & `gtdbtk-2.4.0/gtdbtk/ani_rep.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from gtdbtk.biolib_lite.common import canonical_gid
 from gtdbtk.biolib_lite.execute import check_dependencies
 from gtdbtk.biolib_lite.taxonomy import Taxonomy
 from gtdbtk.config.common import CONFIG
 from gtdbtk.config.output import DIR_ANI_REP_INT_MASH
 from gtdbtk.exceptions import GTDBTkExit
-from gtdbtk.external.fastani import FastANI
+from gtdbtk.external.skani import SkANI
 from gtdbtk.external.mash import Mash
 from gtdbtk.files.gtdb_radii import GTDBRadiiFile
 from gtdbtk.tools import get_ref_genomes
 
 
 class ANIRep(object):
     """Computes a list of genomes to a list of representatives."""
@@ -34,15 +34,15 @@
         """Exits the system if the required programs are not on the path.
 
         Parameters
         ----------
         no_mash : bool
             True if Mash will be used, False otherwise.
         """
-        dependencies = ['fastANI']
+        dependencies = ['skani']
         if not no_mash:
             dependencies.append('mash')
         check_dependencies(dependencies)
 
 
     def run(self, genomes, no_mash, mash_d, out_dir, prefix, mash_k, mash_v, mash_s, min_af, mash_db):
         """Runs the pipeline.
@@ -67,30 +67,30 @@
             maximum number of non-redundant hashes
         min_af : float
             alignment fraction to consider the closest genomes
         mash_db : Optional[str]
             The path to read/write the pre-computed Mash reference sketch database.
         """
         max_mash_dist = mash_d
-        fastani_results = self.run_mash_fastani(genomes, no_mash, mash_d, out_dir,
+        skani_results = self.run_mash_skani(genomes, no_mash, mash_d, out_dir,
                                                 prefix, mash_k, mash_v,
                                                 mash_s, max_mash_dist, mash_db=mash_db)
 
         taxonomy = Taxonomy().read(CONFIG.TAXONOMY_FILE, canonical_ids=True)
-        ani_summary_file = ANISummaryFile(out_dir, prefix, fastani_results, taxonomy)
+        ani_summary_file = ANISummaryFile(out_dir, prefix, skani_results, taxonomy)
         ani_summary_file.write()
         ANIClosestFile(out_dir,
                        prefix,
-                       fastani_results,
+                       skani_results,
                        genomes,
                        min_af,
                        taxonomy)
 
-    def run_mash_fastani(self,genomes, no_mash, max_d, out_dir, prefix, mash_k, mash_v, mash_s, mash_max_dist=100, mash_db=None):
-        """Runs the mash and fastani pipeline.
+    def run_mash_skani(self,genomes, no_mash, max_d, out_dir, prefix, mash_k, mash_v, mash_s, mash_max_dist=100, mash_db=None):
+        """Runs the mash and skani pipeline.
         This step is separated from the run function because it is called from 2 different
         functions in the gtdbtk ( classify and ani_reps).
 
         Parameters
         ----------
         genomes : dict[str, str]
             Dict[genome_id] = fasta_path
@@ -132,33 +132,33 @@
                 d_compare[qry_gid] = d_compare[qry_gid].union(set(ref_hits.keys()))
 
         # Compare against all reference genomes.
         else:
             for qry_gid in genomes:
                 d_compare[qry_gid] = set(ref_genomes.keys())
 
-        self.logger.info(f'Calculating ANI with FastANI v{FastANI._get_version()}.')
-        fastani = FastANI(self.cpus, force_single=True)
-        fastani_results = fastani.run(d_compare, d_paths)
-        return fastani_results
+        self.logger.info(f'Calculating ANI with skani v{SkANI._get_version()}.')
+        skani = SkANI(self.cpus, force_single=True)
+        skani_results = skani.run(d_compare, d_paths)
+        return skani_results
 
 class ANISummaryFile(object):
     name = 'ani_summary.tsv'
 
     def __init__(self, root=None, prefix=None, results=None, taxonomy=None,marker_set_id=None):
         """Writes the ANI summary file generated by this pipeline.
 
         Parameters
         ----------
         root : str
             The directory to write the summary file to.
         prefix : str
             The output file prefix.
         results: dict[str, dict[str, dict[str, float]]]
-            FastANI results.
+            skani results.
         taxonomy : dict[str, tuple[str, str, str, str, str, str, str]]
             d[unique_id] -> [d__<taxon>, ..., s__<taxon>]
         """
         if marker_set_id:
             self.name = f'{marker_set_id}.ani_summary.tsv'
         if prefix is None:
             self.path = root
@@ -171,16 +171,16 @@
 
     @staticmethod
     def get_col_order(ani_screen_step=False) -> List[str]:
         """Return the column order that will be written. If a row is provided
         then format the row in that specific order."""
         cols = ['user_genome',
                    'reference_genome',
-                   'fastani_ani',
-                   'fastani_af',
+                   'skani_ani',
+                   'skani_af',
                    'reference_taxonomy']
         if ani_screen_step:
             cols += ['other_related_references(genome_id,species_name,radius,ANI,AF)']
         return cols
 
     def write(self,ani_screen_step=False):
         with open(self.path, 'w') as fh:
@@ -227,15 +227,15 @@
         Parameters
         ----------
         root : str
             The directory to write the summary file to.
         prefix : str
             The output file prefix.
         results: dict[str, dict[str, dict[str, float]]]
-            FastANI results.
+            skani results.
         genomes : dict[str, str]
             Dict[genome_id] = fasta_path
         min_af : float
             alignment fraction to consider the closest genome
         taxonomy: dict[str, tuple[str, str, str, str, str, str, str]]
             d[unique_id] -> [d__<taxon>, ..., s__<taxon>]
         """
@@ -246,15 +246,15 @@
         self.min_af = min_af
         self.taxonomy = taxonomy
         self.gtdb_radii = GTDBRadiiFile()
         self._write()
 
     def _write(self):
         with open(self.path, 'w') as fh:
-            fh.write('user_genome\treference_genome\tfastani_ani\tfastani_af\t'
+            fh.write('user_genome\treference_genome\tskani_ani\tskani_af\t'
                      'reference_taxonomy\tsatisfies_gtdb_circumscription_criteria\n')
             for gid in sorted(self.genomes):
                 if gid in self.results:
                     thresh_results = [(ref_gid, hit) for (ref_gid, hit) in
                                       self.results[gid].items() if hit['af'] >= self.min_af]
                     closest = sorted(thresh_results, key=lambda x: (-x[1]['ani'], -x[1]['af']))
                     if len(closest) > 0:
```

### Comparing `gtdbtk-2.3.2/gtdbtk/ani_screen.py` & `gtdbtk-2.4.0/gtdbtk/ani_screen.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,81 @@
 import logging
 import os
 
 from gtdbtk.ani_rep import ANIRep, ANISummaryFile
 from gtdbtk.biolib_lite.common import make_sure_path_exists, canonical_gid
+from gtdbtk.biolib_lite.seq_io import read_fasta
 
 from gtdbtk.biolib_lite.taxonomy import Taxonomy
 from gtdbtk.classify import Classify
 from gtdbtk.config.output import DIR_ANISCREEN
 
 from gtdbtk.files.gtdb_radii import GTDBRadiiFile
 from gtdbtk.config.common import CONFIG
 
 class ANIScreener(object):
     """Computes a list of genomes to a list of representatives."""
 
-    def __init__(self, cpus):
+    def __init__(self, cpus,af_threshold=None):
         """Instantiate the ANI rep class.
 
         Parameters
         ----------
         cpus : int
             The maximum number of CPUs available to this workflow.
         """
         self.logger = logging.getLogger('timestamp')
         self.cpus = cpus
+        self.af_threshold = af_threshold if af_threshold else CONFIG.AF_THRESHOLD
         self.gtdb_radii = GTDBRadiiFile()
 
     def run_aniscreen(self,genomes, no_mash,out_dir,prefix, mash_k, mash_v, mash_s, mash_max_dist, mash_db):
 
         # If prescreen is set to True, then we will first run all genomes against a mash database
         # of all genomes in the reference package. The next step will be to classify those genomes with
-        # FastANI.
-        # All genomes classified with FastANI will be removed from the input genomes list for the
+        # skani.
+        # All genomes classified with skani will be removed from the input genomes list for the
         # rest of the pipeline.
         mash_classified_user_genomes = {}
         #if mash_db finishes with a backslash, it should be considered a directory
         if mash_db.endswith('/'):
             make_sure_path_exists(mash_db)
         if os.path.isdir(mash_db):
             mash_db = os.path.join(mash_db, CONFIG.MASH_SKETCH_FILE)
 
         #we set mash_d == mash_max_dist to avoid user to run mash with impossible values
         mash_d = mash_max_dist
 
         ani_rep = ANIRep(self.cpus)
         # we store all the mash information in the classify directory
-        fastani_results = ani_rep.run_mash_fastani(genomes, no_mash, mash_d, os.path.join(out_dir, DIR_ANISCREEN),
+
+        #we createa copy of the genomes dictionary to avoid modifying it
+        genomes_copy = genomes.copy()
+        # we remove all empty files from genomes.
+        for k in list(genomes_copy.keys()):
+            if os.path.getsize(genomes_copy[k]) == 0:
+                self.logger.warning(f'Genome {k} file is invalid for Mash. It will be removed from the sketch step.')
+                del genomes_copy[k]
+            else:
+                # we check if at least one contig is longer than the kmer size
+                seqs = read_fasta(genomes_copy[k])
+                if all(len(seq) < mash_k for seq in seqs.values()):
+                    self.logger.warning(
+                        f'Genome {k} file has all fasta sequences shorter than the k-mer size ({mash_k}).It will be removed from the sketch step.')
+                    del genomes_copy[k]
+
+
+
+        skani_results = ani_rep.run_mash_skani(genomes_copy, no_mash, mash_d, os.path.join(out_dir, DIR_ANISCREEN),
                                                     prefix, mash_k, mash_v, mash_s, mash_max_dist, mash_db)
 
         taxonomy = Taxonomy().read(CONFIG.TAXONOMY_FILE, canonical_ids=True)
 
-        mash_classified_user_genomes = self.sort_fastani_ani_screen(
-             fastani_results,taxonomy)
+        mash_classified_user_genomes = self.sort_skani_ani_screen(
+             skani_results,taxonomy)
 
         #We write the results in 2 different files for each domain
         reports = {}
         if mash_classified_user_genomes:
             for domain,results in mash_classified_user_genomes.items():
                 ani_summary_file = ANISummaryFile(os.path.join(out_dir,DIR_ANISCREEN),prefix,results,taxonomy,domain)
                 ani_summary_file.write(ani_screen_step=True)
@@ -67,41 +87,41 @@
             if 'ar53' in mash_classified_user_genomes else 0
 
         self.logger.info(f'{len_mash_classified_ar53 + len_mash_classified_bac120} genome(s) have '
                          f'been classified using the ANI pre-screening step.')
 
         return mash_classified_user_genomes,reports
 
-    def sort_fastani_ani_screen(self,fastani_results,taxonomy,bac_ar_diff=None):
-        """ When run mash/FastANI on all genomes before using pplacer, we need to sort those results and store them for
+    def sort_skani_ani_screen(self,skani_results,taxonomy,bac_ar_diff=None):
+        """ When run mash/skani on all genomes before using pplacer, we need to sort those results and store them for
         a later use
 
         Parameters
         ----------
-        fastani_results : dict
-            The results of the FastANI run
+        skani_results : dict
+            The results of the skani run
         taxonomy : dict
             The taxonomy of the reference genomes
         """
         classified_user_genomes = {}
 
         # sort the dictionary by ani then af
-        for gid in fastani_results.keys():
-            thresh_results = [(ref_gid, hit) for (ref_gid, hit) in fastani_results[gid].items() if
-                              hit['af'] >= CONFIG.AF_THRESHOLD and hit['ani'] >= self.gtdb_radii.get_rep_ani(
+        for gid in skani_results.keys():
+            thresh_results = [(ref_gid, hit) for (ref_gid, hit) in skani_results[gid].items() if
+                              hit['af'] >= self.af_threshold and hit['ani'] >= self.gtdb_radii.get_rep_ani(
                                   canonical_gid(ref_gid))]
-            all_results = [(ref_gid, hit) for (ref_gid, hit) in fastani_results[gid].items()]
+            all_results = [(ref_gid, hit) for (ref_gid, hit) in skani_results[gid].items()]
             closest = sorted(thresh_results, key=lambda x: (-x[1]['ani'], -x[1]['af']))
             all_closest = sorted(all_results, key=lambda x: (-x[1]['ani'], -x[1]['af']))
             if len(closest) > 0:
                 ref_gid, hit = closest[0]
                 hit_taxonomy = taxonomy[canonical_gid(ref_gid)]
-                if len(all_closest) > 1:
+                if len(all_results) > 1:
                     other_ref = '; '.join(Classify.formatnote(
-                        closest,taxonomy,Classify.parse_radius_file(), [ref_gid]))
+                        all_results,taxonomy,Classify.parse_radius_file(), [ref_gid]))
                     if len(other_ref) > 0:
                         hit['other_related_refs'] = other_ref
 
                 if hit_taxonomy[0] == 'd__Bacteria':
                     classified_user_genomes.setdefault('bac120', {})[gid]={ref_gid:hit}
 
                 elif hit_taxonomy[0] == 'd__Archaea':
```

### Comparing `gtdbtk-2.3.2/gtdbtk/biolib_lite/common.py` & `gtdbtk-2.4.0/gtdbtk/biolib_lite/common.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/gtdbtk/biolib_lite/custom_help_formatter.py` & `gtdbtk-2.4.0/gtdbtk/biolib_lite/custom_help_formatter.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/gtdbtk/biolib_lite/exceptions.py` & `gtdbtk-2.4.0/gtdbtk/biolib_lite/exceptions.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/gtdbtk/biolib_lite/execute.py` & `gtdbtk-2.4.0/gtdbtk/biolib_lite/execute.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/gtdbtk/biolib_lite/logger.py` & `gtdbtk-2.4.0/gtdbtk/biolib_lite/logger.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/gtdbtk/biolib_lite/newick.py` & `gtdbtk-2.4.0/gtdbtk/biolib_lite/newick.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/gtdbtk/biolib_lite/parallel.py` & `gtdbtk-2.4.0/gtdbtk/biolib_lite/parallel.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/gtdbtk/biolib_lite/prodigal_biolib.py` & `gtdbtk-2.4.0/gtdbtk/biolib_lite/prodigal_biolib.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,17 @@
                       (os.path.abspath(genome_file), aa_gene_file))
         else:
             seqs = read_fasta(genome_file)
 
             if len(seqs) == 0:
                 self.logger.warning('Cannot call Prodigal on an empty genome. '
                                     'Skipped: {}'.format(genome_file))
-                return None
+                return (
+                genome_id, aa_gene_file, nt_gene_file, gff_file, best_translation_table, table_coding_density[4],
+                table_coding_density[11], True)
 
             with tempfile.TemporaryDirectory('gtdbtk_prodigal_tmp_') as tmp_dir:
 
                 # determine number of bases
                 total_bases = 0
                 for seq in seqs.values():
                     total_bases += len(seq)
@@ -176,15 +178,15 @@
                                              genome_id + '_genes.faa'), aa_gene_file)
                 shutil.copyfile(os.path.join(tmp_dir, str(best_translation_table),
                                              genome_id + '_genes.fna'), nt_gene_file)
                 shutil.copyfile(os.path.join(tmp_dir, str(best_translation_table),
                                              genome_id + '.gff'), gff_file)
 
         return (genome_id, aa_gene_file, nt_gene_file, gff_file, best_translation_table, table_coding_density[4],
-                table_coding_density[11])
+                table_coding_density[11],False)
 
     def _consumer(self, produced_data, consumer_data):
         """Consume results from producer processes.
 
          Parameters
         ----------
         produced_data : tuple
@@ -201,26 +203,27 @@
                                                     coding_density_4,
                                                     coding_density_11)
             Summary statistics of called genes for each genome.
         """
 
         ConsumerData = namedtuple(
             'ConsumerData',
-            'aa_gene_file nt_gene_file gff_file best_translation_table coding_density_4 coding_density_11')
+            'aa_gene_file nt_gene_file gff_file best_translation_table coding_density_4 coding_density_11 is_empty')
         if consumer_data is None:
             consumer_data = defaultdict(ConsumerData)
 
-        genome_id, aa_gene_file, nt_gene_file, gff_file, best_translation_table, coding_density_4, coding_density_11 = produced_data
+        genome_id, aa_gene_file, nt_gene_file, gff_file, best_translation_table, coding_density_4, coding_density_11, is_empty = produced_data
 
         consumer_data[genome_id] = ConsumerData(aa_gene_file,
                                                 nt_gene_file,
                                                 gff_file,
                                                 best_translation_table,
                                                 coding_density_4,
-                                                coding_density_11)
+                                                coding_density_11,
+                                                is_empty)
 
         return consumer_data
 
     def _progress(self, processed_items, total_items):
         """Report progress of consumer processes.
 
         Parameters
```

### Comparing `gtdbtk-2.3.2/gtdbtk/biolib_lite/seq_io.py` & `gtdbtk-2.4.0/gtdbtk/biolib_lite/seq_io.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/gtdbtk/biolib_lite/taxonomy.py` & `gtdbtk-2.4.0/gtdbtk/biolib_lite/taxonomy.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/gtdbtk/classify.py` & `gtdbtk-2.4.0/gtdbtk/classify.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,16 +33,16 @@
 from gtdbtk.biolib_lite.common import make_sure_path_exists,canonical_gid
 from gtdbtk.biolib_lite.execute import check_dependencies
 from gtdbtk.biolib_lite.newick import parse_label
 from gtdbtk.biolib_lite.seq_io import read_seq, read_fasta
 from gtdbtk.biolib_lite.taxonomy import Taxonomy
 from gtdbtk.config.output import *
 from gtdbtk.exceptions import GenomeMarkerSetUnknown, GTDBTkExit
-from gtdbtk.external.fastani import FastANI
 from gtdbtk.external.pplacer import Pplacer
+from gtdbtk.external.skani import SkANI
 
 from gtdbtk.files.classify_summary import ClassifySummaryFileAR53, ClassifySummaryFileBAC120, ClassifySummaryFileRow
 from gtdbtk.files.marker.copy_number import CopyNumberFileAR53, CopyNumberFileBAC120
 from gtdbtk.files.pplacer_classification import PplacerClassifyFileBAC120, PplacerClassifyFileAR53, \
     PplacerLowClassifyFileBAC120
 from gtdbtk.files.prodigal.tln_table_summary import TlnTableSummaryFile
 from gtdbtk.files.red_dict import REDDictFileAR53, REDDictFileBAC120
@@ -61,15 +61,15 @@
 
 class Classify(object):
     """Determine taxonomic classification of genomes by ML placement."""
 
     def __init__(self, cpus=1, pplacer_cpus=None, af_threshold=None,skip_pplacer=False):
         """Initialize."""
 
-        check_dependencies(['pplacer', 'guppy', 'fastANI'])
+        check_dependencies(['pplacer', 'guppy', 'skani'])
 
         self.skip_pplacer = skip_pplacer
 
         self.taxonomy_file = CONFIG.TAXONOMY_FILE
         self.af_threshold = af_threshold if af_threshold else CONFIG.AF_THRESHOLD
         self.gtdb_taxonomy = Taxonomy().read(self.taxonomy_file)
 
@@ -335,24 +335,25 @@
             no_mash=False,
             mash_k=CONFIG.MASH_K_VALUE,
             mash_v=CONFIG.MASH_V_VALUE,
             mash_s=CONFIG.MASH_S_VALUE,
             mash_max_dist=CONFIG.MASH_MAX_DISTANCE,
             mash_db=None,
             ani_summary_files=None,
-            all_classified_ani=False):
+            all_classified_ani=False,
+            all_failed_prodigal=False):
         """Classify genomes based on position in reference tree."""
-        if not all_classified_ani:
+        if not all_classified_ani and not all_failed_prodigal:
             _bac_gids, _ar_gids, bac_ar_diff = Markers().genome_domain(align_dir, prefix)
 
 
         # If prescreen is set to True, then we will first run all genomes against a mash database
         # of all genomes in the reference package. The next step will be to classify those genomes with
-        # FastANI.
-        # All genomes classified with FastANI will be removed from the input genomes list for the
+        # skani.
+        # All genomes classified with skani will be removed from the input genomes list for the
         # rest of the pipeline.
         mash_classified_user_genomes = {}
         if not skip_ani_screen:
             if genes:
                 self.logger.warning('The --genes flag is set to True. The ANI screening steps will be skipped.')
                 skip_ani_screen = True
             elif not no_mash:
@@ -363,37 +364,37 @@
                     mash_db = os.path.join(mash_db, CONFIG.MASH_SKETCH_FILE)
 
             # we set mash_d == mash_max_dist to avoid user to run mash with impossible values
             mash_d = mash_max_dist
 
             ani_rep = ANIRep(self.cpus)
             # we store all the mash information in the classify directory
-            fastani_results = ani_rep.run_mash_fastani(genomes, no_mash, mash_d, os.path.join(out_dir, DIR_ANISCREEN), prefix, mash_k, mash_v, mash_s,mash_max_dist, mash_db )
+            skani_results = ani_rep.run_mash_skani(genomes, no_mash, mash_d, os.path.join(out_dir, DIR_ANISCREEN), prefix, mash_k, mash_v, mash_s,mash_max_dist, mash_db )
 
-            mash_classified_user_genomes = self._sort_fastani_results_pre_pplacer(
-                fastani_results,bac_ar_diff)
+            mash_classified_user_genomes = self._sort_skani_results_pre_pplacer(
+                skani_results,bac_ar_diff)
 
             len_mash_classified_bac120 = len(mash_classified_user_genomes['bac120']) \
                 if 'bac120' in mash_classified_user_genomes else 0
 
             len_mash_classified_ar53 = len(mash_classified_user_genomes['ar53']) \
                 if 'ar53' in mash_classified_user_genomes else 0
 
 
             self.logger.info(f'{len_mash_classified_ar53+len_mash_classified_bac120} genome(s) have '
                              f'been classified using the ANI pre-screening step.')
 
         if skip_ani_screen and ani_summary_files is not None:
             # if the ani_Screen step was run, we need to load the results from the ani_summary_files
             # and use them to generate the final taxonomy file
-            mash_classified_user_genomes = self.load_fastani_results_pre_pplacer(ani_summary_files)
+            mash_classified_user_genomes = self.load_skani_results_pre_pplacer(ani_summary_files)
 
         output_files = {}
 
-        # if all genomes were classified with FastANI, we can stop here
+        # if all genomes were classified with skani, we can stop here
         # we write the summary files
         if all_classified_ani:
             # if mash_classified_user_genomes is has key marker_set_id, we
             # need to add those genomes to the summary file and remove those genomes to the list of genomes
             # to process with pplacer
             for marker_set_id in ('ar53', 'bac120'):
                 if marker_set_id == 'ar53':
@@ -412,15 +413,15 @@
                                   os.path.join(out_dir,
                                                os.path.basename(PATH_BAC120_SUMMARY_OUT.format(prefix=prefix))))
                     elif marker_set_id == 'ar53':
                         symlink_f(PATH_AR53_SUMMARY_OUT.format(prefix=prefix),
                                   os.path.join(out_dir, os.path.basename(PATH_AR53_SUMMARY_OUT.format(prefix=prefix))))
                     output_files.setdefault(marker_set_id, []).append(summary_file.path)
             return output_files
-        else:
+        elif not all_failed_prodigal:
             for marker_set_id in ('ar53', 'bac120'):
                 warning_counter, prodigal_failed_counter = 0, 0
                 if marker_set_id == 'ar53':
                     marker_summary_fh = CopyNumberFileAR53(align_dir, prefix)
                     marker_summary_fh.read()
                     if os.path.isfile(os.path.join(align_dir,
                                                    PATH_AR53_USER_MSA.format(prefix=prefix))):
@@ -473,15 +474,30 @@
                         warning_counter = self.add_filtered_genomes_to_summary(align_dir, warning_counter, summary_file,
                                                                                marker_set_id, prefix)
 
                     # we add all genomes classified with ANI
                     if mash_classified_user_genomes and marker_set_id in mash_classified_user_genomes:
                         list_summary_rows = mash_classified_user_genomes.get(marker_set_id)
                         for row in list_summary_rows:
-                            summary_file.add_row(row)
+                            # in some instance, when running the 3 classify steps independently, the genome might have been filtered out in the alignment step
+                            # but its still present in the ani screening and have a % > 95 ( this can happen with partial genomes) so Tk would try to report it twice in
+                            # the summary file, instead we report it as classify with ani, but with a warning from the alignment step
+                            # skani should reduce the number of such cases
+                            if row.gid in summary_file.rows:
+                                row_to_update = summary_file.get_row(row.gid)
+                                existing_warnings = row_to_update.warnings
+                                if existing_warnings is not None and row.warnings:
+                                    row.warnings.append(existing_warnings)
+                                elif existing_warnings is not None:
+                                    row.warnings = [existing_warnings]
+                                if row.warnings:
+                                    row.warnings = ';'.join(row.warnings)
+                                summary_file.update_row(row)
+                            else:
+                                summary_file.add_row(row)
 
                     if summary_file.has_row():
                         summary_file.write()
                         output_files.setdefault(marker_set_id, []).append(summary_file.path)
                         # Symlink to the summary file from the root
                         if marker_set_id == 'ar53':
                             symlink_f(PATH_AR53_SUMMARY_OUT.format(prefix=prefix),
@@ -733,14 +749,35 @@
 
                 # Write the summary file to disk.
                 if disappearing_genomes_file.data:
                     disappearing_genomes_file.write()
                     output_files.setdefault(marker_set_id, []).append(disappearing_genomes_file.path)
                 summary_file.write()
                 output_files.setdefault(marker_set_id, []).append(summary_file.path)
+        elif all_failed_prodigal:
+            marker_set_id ='bac120'
+            summary_file = ClassifySummaryFileBAC120(out_dir, prefix)
+
+            # Add failed genomes from prodigal and genomes with no markers in the bac120 summary file
+            # This is an executive direction: failed prodigal and genomes with no markers are not bacterial or archaeal
+            # but they need to be included in one of the summary file
+            prodigal_failed_counter = self.add_failed_genomes_to_summary(align_dir, summary_file, prefix)
+
+            if summary_file.has_row():
+                summary_file.write()
+                output_files.setdefault(marker_set_id, []).append(summary_file.path)
+                # Symlink to the summary file from the root
+                symlink_f(PATH_BAC120_SUMMARY_OUT.format(prefix=prefix),
+                              os.path.join(out_dir, os.path.basename(PATH_BAC120_SUMMARY_OUT.format(prefix=prefix))))
+                if prodigal_failed_counter > 0:
+                    self.logger.warning(f"{prodigal_failed_counter} of {len(genomes)} "
+                                        f"genome{'' if prodigal_failed_counter == 1 else 's'} "
+                                        f"ha{'s' if prodigal_failed_counter == 1 else 've'} been labeled as 'Unclassified'.")
+
+
         return output_files
 
     def _add_warning_to_row(self,row,msa_dict,
                             trans_table_dict,
                             percent_multihit_dict,
                             warning_counter):
 
@@ -790,15 +827,15 @@
                                                prefix,
                                                scratch_dir,
                                                'low', tree_iter,
                                                number_low_trees, idx_tree)
         return low_classify_tree, submsa_file_path
 
     @staticmethod
-    def _get_fastani_verification(tree, reference_ids, tt):
+    def _get_skani_verification(tree, reference_ids, tt):
         """
 
         Parameters
         ----------
         tree : dendropy.Tree
             The input tree.
 
@@ -1173,65 +1210,65 @@
 
 
         return class_level_classification,warning_counter
 
     def _parse_tree(self, tree, genomes, msa_dict, percent_multihit_dict,genes, trans_table_dict, bac_ar_diff,
                     user_msa_file, red_dict, summary_file, pplacer_taxonomy_dict,warning_counter, high_classification,
                     debug_file, debugopt, tree_mapping_file, tree_iter, tree_mapping_dict_reverse):
-        # Genomes can be classified by using FastANI or RED values
+        # Genomes can be classified by using skani or RED values
         # We go through all leaves of the tree. if the leaf is a user
         # genome we take its parent node and look at all the leaves
         # for this node.
 
         # Persist descendant information for efficient traversal.
         tt = TreeTraversal()
 
         self.logger.log(CONFIG.LOG_TASK, 'Traversing tree to determine classification method.')
         if genes:
-            fastani_verification = {}
+            skani_verification = {}
         else:
-            fastani_verification, qury_nodes = self._get_fastani_verification(tree, self.reference_ids, tt)
+            skani_verification, qury_nodes = self._get_skani_verification(tree, self.reference_ids, tt)
 
-        #DEBUG: Skip FastANI step
-        #fastani_verification = {}
+        #DEBUG: Skip skani step
+        #skani_verification = {}
 
-        # we run a fastani comparison for each user genomes against the
+        # we run a skani comparison for each user genomes against the
         # selected genomes in the same genus
-        ##if not prescreening and len(fastani_verification) > 0:
-        if len(fastani_verification) > 0:
-            fastani = FastANI(cpus=self.cpus, force_single=True)
-            d_ani_compare, d_paths = self._get_fastani_genome_path(
-                fastani_verification, genomes)
+        ##if not prescreening and len(skani_verification) > 0:
+        if len(skani_verification) > 0:
+            skani = SkANI(cpus=self.cpus, force_single=True)
+            d_ani_compare, d_paths = self._get_skani_genome_path(
+                skani_verification, genomes)
             self.logger.log(CONFIG.LOG_TASK,
                             f'Calculating average nucleotide identity using '
-                            f'FastANI (v{fastani.version}).')
-            all_fastani_dict = fastani.run(d_ani_compare, d_paths)
+                            f'skani (v{skani.version}).')
+            all_skani_dict = skani.run(d_ani_compare, d_paths)
         else:
-            all_fastani_dict = {}
+            all_skani_dict = {}
 
-        classified_user_genomes, unclassified_user_genomes,warning_counter = self._sort_fastani_results(
-            fastani_verification, pplacer_taxonomy_dict, all_fastani_dict, msa_dict, percent_multihit_dict,
+        classified_user_genomes, unclassified_user_genomes,warning_counter = self._sort_skani_results(
+            skani_verification, pplacer_taxonomy_dict, all_skani_dict, msa_dict, percent_multihit_dict,
             trans_table_dict, bac_ar_diff,warning_counter, summary_file)
         #if not prescreening:
         if not genes:
             self.logger.info(f'{len(classified_user_genomes):,} genome(s) have '
-                             f'been classified using FastANI and pplacer.')
+                             f'been classified using skani and pplacer.')
         else:
             self.logger.info('ANI classification has been skipped (--genes option used).')
 
         if tree_mapping_file:
             for genome in classified_user_genomes.keys():
                 mapping_row = GenomeMappingFileRow()
                 mapping_row.gid = genome
                 mapping_row.ani_classification = True
                 mapping_row.mapped_tree = tree_iter
                 mapping_row.rule = 'Rule 7'
                 tree_mapping_file.add_row(mapping_row)
 
-        # Iterate over each leaf node that was not classified with FastANI.
+        # Iterate over each leaf node that was not classified with skani.
         class_in_spe_tree = None
         phyla_in_spe_tree = None
         if tree_mapping_dict_reverse:
             class_in_spe_tree = tree_mapping_dict_reverse.get(tree_iter)
             phyla_in_spe_tree = self.get_authorised_rank(class_in_spe_tree,self.PHYLUM_IDX)
 
 
@@ -1390,20 +1427,36 @@
             filtered_file = os.path.join(align_dir,PATH_AR53_FILTERED_GENOMES.format(prefix=prefix))
             domain = 'Archaea'
         # if file exists:
         if os.path.exists(filtered_file):
             with open(filtered_file) as fin:
                 for line in fin:
                     infos = line.strip().split('\t')
-                    summary_row = ClassifySummaryFileRow()
-                    summary_row.gid = infos[0]
-                    summary_row.classification = f'Unclassified {domain}'
-                    summary_row.warnings = infos[1]
-                    summary_file.add_row(summary_row)
-                    warning_counter += 1
+                    # in some instance, when running the 3 classify steps independently, the genome might have been filtered out in the alignment step
+                    # but its still present in the ani screening and have a % > 95 ( this can happen with partial genomes) so Tk would try to report it twice in
+                    # the summary file, instead we report it as classified with ani, but with a warning from the alignment step
+                    # skani should reduce the number of such cases
+                    if infos[0] in summary_file.rows:
+                        row_to_update = summary_file.rows[infos[0]]
+                        # extra check
+                        if row_to_update.classification_method == 'ani_screen':
+                            existing_warnings = row_to_update.warnings
+                            if existing_warnings is not None:
+                                row_to_update.warnings = existing_warnings + ';' + infos[1]
+                            else:
+                                row_to_update.warnings = infos[1]
+                                warning_counter += 1
+                    else:
+                        summary_row = ClassifySummaryFileRow()
+                        summary_row.gid = infos[0]
+                        summary_row.classification = f'Unclassified {domain}'
+                        summary_row.warnings = infos[1]
+                        summary_file.add_row(summary_row)
+                        warning_counter += 1
+
         return warning_counter
 
     def add_failed_genomes_to_summary(self, align_dir, summary_file, prefix):
         warning_counter = 0
         prodigal_failed_file = os.path.join(align_dir, PATH_FAILS.format(prefix=prefix))
         align_failed_file = os.path.join(align_dir, PATH_FAILED_ALIGN_GENOMES.format(prefix=prefix))
         for failfile in (prodigal_failed_file, align_failed_file):
@@ -1447,108 +1500,112 @@
                                                        round(
                                                            element[1].get('ani'), 2),
                                                        round(element[1].get('af'),3))
                 note_list.append(note_str)
         return note_list
 
 
-    def _sort_fastani_results_pre_pplacer(self,fastani_results,bac_ar_diff):
-        """ When run mash/FastANI on all genomes before using pplacer, we need to sort those results and store them for
+    def _sort_skani_results_pre_pplacer(self,skani_results,bac_ar_diff):
+        """ When run mash/skani on all genomes before using pplacer, we need to sort those results and store them for
         a later use
 
         Parameters
         ----------
-        fastani_results : dictionary listing the fastani ANI for each user genomes against the potential genomes
+        skani_results : dictionary listing the skani ANI for each user genomes against the potential genomes
 
         """
         classified_user_genomes = {}
 
         # sort the dictionary by ani then af
-        for gid in fastani_results.keys():
-            thresh_results = [(ref_gid, hit) for (ref_gid, hit) in fastani_results[gid].items() if
-                              hit['af'] >= CONFIG.AF_THRESHOLD and hit['ani'] >= self.gtdb_radii.get_rep_ani(
-                                  canonical_gid(ref_gid))]
+        for gid in skani_results.keys():
+            thresh_results = [(ref_gid, hit) for (ref_gid, hit) in skani_results[gid].items() if \
+                              hit['af'] >= self.af_threshold]
             closest = sorted(thresh_results, key=lambda x: (-x[1]['ani'], -x[1]['af']))
             if len(closest) > 0:
-                summary_row = ClassifySummaryFileRow()
-                summary_row.gid = gid
-                summary_row.classification_method = 'ani_screen'
-                if len(closest) > 1:
-                    other_ref = '; '.join(self.formatnote(
-                        closest,self.gtdb_taxonomy,self.species_radius, [gid]))
-                    if len(other_ref) == 0:
-                        summary_row.other_related_refs = None
-                    else:
+                set_to_closest_rep = False
+                closest_rep,closet_rep_infos = closest[0]
+                if closet_rep_infos['ani'] >= self.gtdb_radii.get_rep_ani(canonical_gid(closest_rep)):
+                    set_to_closest_rep = True
+                    # remove the closest rep from the list
+                    trimmed_closest = closest[1:]
+                    other_ref = None
+                    summary_row = ClassifySummaryFileRow()
+                    summary_row.gid = gid
+                    summary_row.classification_method = 'ani_screen'
+
+                    if len(trimmed_closest) > 1:
+                        other_ref = '; '.join(self.formatnote(
+                            closest,self.gtdb_taxonomy,self.species_radius, [gid]))
                         summary_row.other_related_refs = other_ref
-                summary_row.note = 'classification based on ANI only'
+                    summary_row.note = 'classification based on ANI only'
 
-                fastani_matching_reference = closest[0][0]
-                current_ani = fastani_results.get(gid).get(
-                    fastani_matching_reference).get('ani')
-                current_af = fastani_results.get(gid).get(
-                    fastani_matching_reference).get('af')
-
-                summary_row.fastani_ref = fastani_matching_reference
-                summary_row.fastani_ref_radius = str(
-                    self.species_radius.get(fastani_matching_reference))
-                summary_row.fastani_tax = ";".join(self.gtdb_taxonomy.get(
-                    add_ncbi_prefix(fastani_matching_reference)))
-                summary_row.fastani_ani = round(current_ani, 2)
-                summary_row.fastani_af = round(current_af, 3)
-                taxa_str = ";".join(self.gtdb_taxonomy.get(
-                    add_ncbi_prefix(fastani_matching_reference)))
-                summary_row.classification = standardise_taxonomy(
-                    taxa_str)
+                    skani_matching_reference = closest_rep
+                    current_ani = skani_results.get(gid).get(
+                        skani_matching_reference).get('ani')
+                    current_af = skani_results.get(gid).get(
+                        skani_matching_reference).get('af')
+
+                    summary_row.closest_genome_ref = skani_matching_reference
+                    summary_row.closest_genome_ref_radius = str(
+                        self.species_radius.get(skani_matching_reference))
+                    summary_row.closest_genome_tax = ";".join(self.gtdb_taxonomy.get(
+                        add_ncbi_prefix(skani_matching_reference)))
+                    summary_row.closest_genome_ani = round(current_ani, 2)
+                    summary_row.closest_genome_af = round(current_af, 3)
+                    taxa_str = ";".join(self.gtdb_taxonomy.get(
+                        add_ncbi_prefix(skani_matching_reference)))
+                    summary_row.classification = standardise_taxonomy(
+                        taxa_str)
 
-                warnings = []
-                if gid in bac_ar_diff:
-                    warnings.append('Genome domain questionable ( {}% Bacterial, {}% Archaeal)'.format(
-                        bac_ar_diff.get(gid).get('bac120'),
-                        bac_ar_diff.get(gid).get('ar53')))
+                    warnings = []
+                    if gid in bac_ar_diff:
+                        warnings.append('Genome domain questionable ( {}% Bacterial, {}% Archaeal)'.format(
+                            bac_ar_diff.get(gid).get('bac120'),
+                            bac_ar_diff.get(gid).get('ar53')))
 
-                if len(warnings) > 0:
-                    summary_row.warnings = warnings
+                    if len(warnings) > 0:
+                        summary_row.warnings = warnings
 
-                if (taxa_str.split(';')[0]).split('__')[1] == 'Bacteria':
-                    domain = 'bac120'
-                else:
-                    domain = 'ar53'
-                classified_user_genomes.setdefault(domain, []).append(summary_row)
+                    if (taxa_str.split(';')[0]).split('__')[1] == 'Bacteria':
+                        domain = 'bac120'
+                    else:
+                        domain = 'ar53'
+                    classified_user_genomes.setdefault(domain, []).append(summary_row)
 
         return classified_user_genomes
 
 
 
 
-    def _sort_fastani_results(self, fastani_verification, pplacer_taxonomy_dict,
-                              all_fastani_dict, msa_dict, percent_multihit_dict,
+    def _sort_skani_results(self, skani_verification, pplacer_taxonomy_dict,
+                              all_skani_dict, msa_dict, percent_multihit_dict,
                               trans_table_dict, bac_ar_diff,warning_counter, summary_file):
         """Format the note field by concatenating all information in a sorted dictionary
 
         Parameters
         ----------
-        fastani_verification : dictionary listing the potential genomes associated with a user genome
+        skani_verification : dictionary listing the potential genomes associated with a user genome
         d[user_genome] = {"potential_g": [(potential_genome_in_same_genus,patristic distance)],
         "pplacer_g": genome_of_reference_selected_by_pplacer(if any)}
-        all_fastani_dict : dictionary listing the fastani ANI for each user genomes against the potential genomes
+        all_skani_dict : dictionary listing the skani ANI for each user genomes against the potential genomes
         d[user_genome]={ref_genome1:{"af":af,"ani":ani},ref_genome2:{"af":af,"ani":ani}}
         summaryfout: output file
 
         Returns
         -------
-        classified_user_genomes: list of genomes where FastANI and Placement in the reference tree have
+        classified_user_genomes: list of genomes where skani and Placement in the reference tree have
         predicted a taxonomy
-        unclassified_user_genomes: dictionary of genomes where FastANI and Placement in the reference tree have not
+        unclassified_user_genomes: dictionary of genomes where skani and Placement in the reference tree have not
         predicted a taxonomy
 
         """
         classified_user_genomes = {}
         unclassified_user_genomes = {}
 
-        for userleaf, potential_nodes in fastani_verification.items():
+        for userleaf, potential_nodes in skani_verification.items():
 
             summary_row = ClassifySummaryFileRow()
 
             warnings = []
             if userleaf.taxon.label in percent_multihit_dict:
                 warnings.append('Genome has more than {}% of markers with multiple hits'.format(
                     percent_multihit_dict.get(userleaf.taxon.label)))
@@ -1557,34 +1614,34 @@
                     bac_ar_diff.get(userleaf.taxon.label).get('bac120'),
                     bac_ar_diff.get(userleaf.taxon.label).get('ar53')))
 
             if potential_nodes.get("pplacer_g"):
                 pplacer_leafnode = potential_nodes.get("pplacer_g").taxon.label
                 if pplacer_leafnode[0:3] in ['RS_', 'GB_']:
                     pplacer_leafnode = pplacer_leafnode[3:]
-                if userleaf.taxon.label in all_fastani_dict:
+                if userleaf.taxon.label in all_skani_dict:
                     # import IPython; IPython.embed()
                     prefilter_af_reference_dictionary = {k: v for k, v in
-                                                         all_fastani_dict.get(userleaf.taxon.label).items() if v.get(
+                                                         all_skani_dict.get(userleaf.taxon.label).items() if v.get(
                             'af') >= self.af_threshold}
                     sorted_prefilter_af_dict = sorted(iter(prefilter_af_reference_dictionary.items()),
                                                       key=lambda _x_y1: (_x_y1[1]['ani'], _x_y1[1]['af']), reverse=True)
 
-                    sorted_dict = sorted(iter(all_fastani_dict.get(
+                    sorted_dict = sorted(iter(all_skani_dict.get(
                         userleaf.taxon.label).items()), key=lambda _x_y: (_x_y[1]['ani'], _x_y[1]['af']), reverse=True)
 
-                    fastani_matching_reference = None
+                    skani_matching_reference = None
                     if len(sorted_prefilter_af_dict) > 0:
                         if sorted_prefilter_af_dict[0][1].get('ani') >= self.species_radius.get(
                                 sorted_prefilter_af_dict[0][0]):
-                            fastani_matching_reference = sorted_prefilter_af_dict[0][0]
-                            current_ani = all_fastani_dict.get(userleaf.taxon.label).get(
-                                fastani_matching_reference).get('ani')
-                            current_af = all_fastani_dict.get(userleaf.taxon.label).get(
-                                fastani_matching_reference).get('af')
+                            skani_matching_reference = sorted_prefilter_af_dict[0][0]
+                            current_ani = all_skani_dict.get(userleaf.taxon.label).get(
+                                skani_matching_reference).get('ani')
+                            current_af = all_skani_dict.get(userleaf.taxon.label).get(
+                                skani_matching_reference).get('af')
                         else:
                             warnings.append(
                                 "Genome not assigned to closest species as it falls outside its pre-defined ANI radius")
 
                     taxa_str = ";".join(self.gtdb_taxonomy.get(
                         add_ncbi_prefix(pplacer_leafnode)))
 
@@ -1594,101 +1651,101 @@
                     summary_row.classification_method = 'taxonomic classification defined by topology and ANI'
                     summary_row.msa_percent = aa_percent_msa(
                         msa_dict.get(summary_row.gid))
                     summary_row.tln_table = trans_table_dict.get(summary_row.gid)
                     if len(warnings) > 0:
                         summary_row.warnings = ';'.join(warnings)
 
-                    if fastani_matching_reference is not None:
-                        summary_row.fastani_ref = fastani_matching_reference
-                        summary_row.fastani_ref_radius = str(
-                            self.species_radius.get(fastani_matching_reference))
-                        summary_row.fastani_tax = ";".join(self.gtdb_taxonomy.get(
-                            add_ncbi_prefix(fastani_matching_reference)))
-                        summary_row.fastani_ani = round(current_ani, 2)
-                        summary_row.fastani_af = round(current_af,3)
-                        if pplacer_leafnode == fastani_matching_reference:
+                    if skani_matching_reference is not None:
+                        summary_row.closest_genome_ref = skani_matching_reference
+                        summary_row.closest_genome_ref_radius = str(
+                            self.species_radius.get(skani_matching_reference))
+                        summary_row.closest_genome_tax = ";".join(self.gtdb_taxonomy.get(
+                            add_ncbi_prefix(skani_matching_reference)))
+                        summary_row.closest_genome_ani = round(current_ani, 2)
+                        summary_row.closest_genome_af = round(current_af,3)
+                        if pplacer_leafnode == skani_matching_reference:
                             if taxa_str.endswith("s__"):
                                 taxa_str = taxa_str + pplacer_leafnode
                             summary_row.classification = standardise_taxonomy(
                                 taxa_str)
-                            summary_row.closest_placement_ref = summary_row.fastani_ref
-                            summary_row.closest_placement_radius = summary_row.fastani_ref_radius
-                            summary_row.closest_placement_tax = summary_row.fastani_tax
-                            summary_row.closest_placement_ani = summary_row.fastani_ani
-                            summary_row.closest_placement_af = summary_row.fastani_af
+                            summary_row.closest_placement_ref = summary_row.closest_genome_ref
+                            summary_row.closest_placement_radius = summary_row.closest_genome_ref_radius
+                            summary_row.closest_placement_tax = summary_row.closest_genome_tax
+                            summary_row.closest_placement_ani = summary_row.closest_genome_ani
+                            summary_row.closest_placement_af = summary_row.closest_genome_af
                             summary_row.note = 'topological placement and ANI have congruent species assignments'
                             if len(sorted_dict) > 0:
                                 other_ref = '; '.join(self.formatnote(
-                                    sorted_dict,self.gtdb_taxonomy,self.species_radius, [fastani_matching_reference]))
+                                    sorted_dict,self.gtdb_taxonomy,self.species_radius, [skani_matching_reference]))
                                 if len(other_ref) == 0:
                                     summary_row.other_related_refs = None
                                 else:
                                     summary_row.other_related_refs = other_ref
 
                         else:
                             taxa_str = ";".join(self.gtdb_taxonomy.get(
-                                add_ncbi_prefix(fastani_matching_reference)))
+                                add_ncbi_prefix(skani_matching_reference)))
                             summary_row.classification = standardise_taxonomy(
                                 taxa_str)
                             summary_row.closest_placement_ref = pplacer_leafnode
                             summary_row.closest_placement_radius = str(
                                 self.species_radius.get(pplacer_leafnode))
                             summary_row.closest_placement_tax = ";".join(self.gtdb_taxonomy.get(
                                 add_ncbi_prefix(pplacer_leafnode)))
-                            if pplacer_leafnode in all_fastani_dict.get(userleaf.taxon.label):
-                                summary_row.closest_placement_ani = round(all_fastani_dict.get(
+                            if pplacer_leafnode in all_skani_dict.get(userleaf.taxon.label):
+                                summary_row.closest_placement_ani = round(all_skani_dict.get(
                                     userleaf.taxon.label).get(pplacer_leafnode).get('ani'), 2)
-                                summary_row.closest_placement_af = round(all_fastani_dict.get(
+                                summary_row.closest_placement_af = round(all_skani_dict.get(
                                     userleaf.taxon.label).get(pplacer_leafnode).get('af'),3)
-                            summary_row.classification_method = 'ANI'
+                            summary_row.classification_method = 'taxonomic classification defined by topology and ANI'
 
                             if len(sorted_dict) > 0:
                                 other_ref = '; '.join(self.formatnote(
-                                    sorted_dict,self.gtdb_taxonomy,self.species_radius, [fastani_matching_reference, pplacer_leafnode]))
+                                    sorted_dict,self.gtdb_taxonomy,self.species_radius, [skani_matching_reference, pplacer_leafnode]))
                                 if len(other_ref) == 0:
                                     summary_row.other_related_refs = None
                                 else:
                                     summary_row.other_related_refs = other_ref
                         summary_file.add_row(summary_row)
                         classified_user_genomes[userleaf.taxon.label] = standardise_taxonomy(taxa_str)
                     else:
                         summary_row.closest_placement_ref = pplacer_leafnode
                         summary_row.closest_placement_radius = str(
                             self.species_radius.get(pplacer_leafnode))
                         summary_row.closest_placement_tax = ";".join(self.gtdb_taxonomy.get(
                             add_ncbi_prefix(pplacer_leafnode)))
-                        if pplacer_leafnode in all_fastani_dict.get(userleaf.taxon.label):
-                            summary_row.closest_placement_ani = round(all_fastani_dict.get(
+                        if pplacer_leafnode in all_skani_dict.get(userleaf.taxon.label):
+                            summary_row.closest_placement_ani = round(all_skani_dict.get(
                                 userleaf.taxon.label).get(pplacer_leafnode).get('ani'), 2)
-                            summary_row.closest_placement_af = round(all_fastani_dict.get(
+                            summary_row.closest_placement_af = round(all_skani_dict.get(
                                 userleaf.taxon.label).get(pplacer_leafnode).get('af'),3)
 
                         if len(sorted_dict) > 0:
                             other_ref = '; '.join(self.formatnote(
                                 sorted_dict,self.gtdb_taxonomy,self.species_radius, [pplacer_leafnode]))
                             if len(other_ref) == 0:
                                 summary_row.other_related_refs = None
                             else:
                                 summary_row.other_related_refs = other_ref
                         unclassified_user_genomes[userleaf.taxon.label] = summary_row
 
-            elif userleaf.taxon.label in all_fastani_dict:
+            elif userleaf.taxon.label in all_skani_dict:
                 prefilter_af_reference_dictionary = {k: v for k, v in
-                                                     all_fastani_dict.get(userleaf.taxon.label).items() if v.get(
+                                                     all_skani_dict.get(userleaf.taxon.label).items() if v.get(
                         'af') >= self.af_threshold}
                 sorted_prefilter_af_dict = sorted(iter(prefilter_af_reference_dictionary.items()),
                                                   key=lambda _x_y1: (_x_y1[1]['ani'], _x_y1[1]['af']), reverse=True)
-                sorted_dict = sorted(iter(all_fastani_dict.get(
+                sorted_dict = sorted(iter(all_skani_dict.get(
                     userleaf.taxon.label).items()), key=lambda _x_y2: (_x_y2[1]['ani'], _x_y2[1]['af']), reverse=True)
 
                 summary_row.gid = userleaf.taxon.label
                 summary_row.pplacer_tax = pplacer_taxonomy_dict.get(
                     userleaf.taxon.label)
-                summary_row.classification_method = 'ANI'
+                summary_row.classification_method = 'taxonomic classification defined by topology and ANI'
                 summary_row.msa_percent = aa_percent_msa(
                     msa_dict.get(summary_row.gid))
                 summary_row.tln_table = trans_table_dict.get(summary_row.gid)
 
                 exception_genomes = []
                 if len(sorted_prefilter_af_dict) > 0:
 
@@ -1701,33 +1758,33 @@
                             summary_row.other_related_refs = other_ref
 
                     if len(warnings) > 0:
                         summary_row.warnings = ';'.join(warnings)
                         warning_counter += 1
                     if sorted_prefilter_af_dict[0][1].get('ani') >= self.species_radius.get(
                             sorted_prefilter_af_dict[0][0]):
-                        fastani_matching_reference = sorted_prefilter_af_dict[0][0]
-                        exception_genomes.append(fastani_matching_reference)
+                        skani_matching_reference = sorted_prefilter_af_dict[0][0]
+                        exception_genomes.append(skani_matching_reference)
 
                         taxa_str = ";".join(self.gtdb_taxonomy.get(
-                            add_ncbi_prefix(fastani_matching_reference)))
+                            add_ncbi_prefix(skani_matching_reference)))
                         summary_row.classification = standardise_taxonomy(
                             taxa_str)
 
-                        summary_row.fastani_ref = fastani_matching_reference
-                        summary_row.fastani_ref_radius = str(
-                            self.species_radius.get(fastani_matching_reference))
-                        summary_row.fastani_tax = ";".join(self.gtdb_taxonomy.get(
-                            add_ncbi_prefix(fastani_matching_reference)))
-                        current_ani = all_fastani_dict.get(userleaf.taxon.label).get(
-                            fastani_matching_reference).get('ani')
-                        summary_row.fastani_ani = round(current_ani, 2)
-                        current_af = all_fastani_dict.get(userleaf.taxon.label).get(
-                            fastani_matching_reference).get('af')
-                        summary_row.fastani_af = round(current_af,3)
+                        summary_row.closest_genome_ref = skani_matching_reference
+                        summary_row.closest_genome_ref_radius = str(
+                            self.species_radius.get(skani_matching_reference))
+                        summary_row.closest_genome_tax = ";".join(self.gtdb_taxonomy.get(
+                            add_ncbi_prefix(skani_matching_reference)))
+                        current_ani = all_skani_dict.get(userleaf.taxon.label).get(
+                            skani_matching_reference).get('ani')
+                        summary_row.closest_genome_ani = round(current_ani, 2)
+                        current_af = all_skani_dict.get(userleaf.taxon.label).get(
+                            skani_matching_reference).get('af')
+                        summary_row.closest_genome_af = round(current_af,3)
                         summary_row.note = 'topological placement and ANI have incongruent species assignments'
                         if len(warnings) > 0:
                             summary_row.warnings = ';'.join(warnings)
 
                         summary_file.add_row(summary_row)
                         classified_user_genomes[userleaf.taxon.label] = standardise_taxonomy(taxa_str)
                     else:
@@ -2127,15 +2184,15 @@
         # also no way to identify a node that is guaranteed to be outside the outgroup
         # clade. As such, the tree is randomly rooted on a leaf node not in the outgroup.
         # This random re-rooting is performed until the MRCA does not spans all taxa in
         # the tree.
 
         leaves_in_tree = sum([1 for _ in new_tree.leaf_node_iter()])
         while True:
-            rnd_ingroup_leaf = random.sample(ingroup_in_tree, 1)[0]
+            rnd_ingroup_leaf = random.sample(tuple(ingroup_in_tree), 1)[0]
             new_tree.reroot_at_edge(rnd_ingroup_leaf.edge,
                                     length1=0.5 * rnd_ingroup_leaf.edge_length,
                                     length2=0.5 * rnd_ingroup_leaf.edge_length)
 
             mrca = new_tree.mrca(taxa=outgroup_in_tree)
             leaves_in_mrca = sum([1 for _ in mrca.leaf_iter()])
             if leaves_in_mrca != leaves_in_tree:
@@ -2155,110 +2212,110 @@
         else:
             new_tree.reroot_at_edge(mrca.edge,
                                     length1=0.5 * mrca.edge_length,
                                     length2=0.5 * mrca.edge_length)
 
         return new_tree
 
-    def _get_fastani_genome_path(self, fastani_verification, genomes):
+    def _get_skani_genome_path(self, skani_verification, genomes):
         """Generates a queue of comparisons to be made and the paths to
         the corresponding genome id."""
         dict_compare, dict_paths = dict(), dict()
 
-        for qry_node, qry_dict in fastani_verification.items():
+        for qry_node, qry_dict in skani_verification.items():
             user_label = qry_node.taxon.label
             dict_paths[user_label] = genomes[user_label]
             dict_compare[user_label] = set()
             for node in qry_dict.get('potential_g'):
                 leafnode = node[0]
                 shortleaf = leafnode.taxon.label
                 if leafnode.taxon.label.startswith('GB_') or leafnode.taxon.label.startswith('RS_'):
                     shortleaf = leafnode.taxon.label[3:]
                 # TODEL UBA genomes
                 if shortleaf.startswith("UBA"):
                     ref_path = os.path.join(
-                        CONFIG.FASTANI_GENOMES,
+                        CONFIG.SKANI_GENOMES,
                         'UBA',
-                        shortleaf + CONFIG.FASTANI_GENOMES_EXT)
+                        shortleaf + CONFIG.SKANI_GENOMES_EXT)
                 else:
                     ref_path = os.path.join(
-                        CONFIG.FASTANI_GENOMES,
+                        CONFIG.SKANI_GENOMES,
                         self.parse_leaf_to_dir_path(shortleaf),
-                        shortleaf + CONFIG.FASTANI_GENOMES_EXT)
+                        shortleaf + CONFIG.SKANI_GENOMES_EXT)
 
                 if not os.path.isfile(ref_path):
-                    raise GTDBTkExit(f'Reference genome missing from FastANI database: {ref_path}')
+                    raise GTDBTkExit(f'Reference genome missing from skani database: {ref_path}')
 
                 dict_compare[user_label].add(shortleaf)
                 dict_paths[shortleaf] = ref_path
 
         return dict_compare, dict_paths
 
     def get_authorised_rank(self, order_in_spe_tree,rank_index):
         results = []
         for k, v in self.gtdb_taxonomy.items():
             if v[self.order_rank.index(self.rank_of_interest)] in order_in_spe_tree:
                 results.append(v[rank_index])
         return list(set(results))
 
-    def load_fastani_results_pre_pplacer(self,ani_summary_files):
-        """Load the FastANI results for the genomes classified with ANI Screen."""
-        fastani_results={}
+    def load_skani_results_pre_pplacer(self,ani_summary_files):
+        """Load the skani results for the genomes classified with ANI Screen."""
+        skani_results={}
         for domain,ani_summary_file_path in ani_summary_files.items():
             ani_summary_file = ANISummaryFile(ani_summary_file_path)
-            fastani_results[domain]=ani_summary_file.read()
+            skani_results[domain]=ani_summary_file.read()
 
         classified_user_genomes = {}
 
         # sort the dictionary by ani then af
-        for domain,fastani_results in fastani_results.items():
-            for gid,ani_results in fastani_results.items():
+        for domain,skani_results in skani_results.items():
+            for gid,ani_results in skani_results.items():
                 summary_row = ClassifySummaryFileRow()
                 summary_row.gid = gid
                 summary_row.classification_method = 'ani_screen'
                 summary_row.note = 'classification based on ANI only'
 
-                fastani_matching_reference = list(ani_results)[0]
+                skani_matching_reference = list(ani_results)[0]
 
-                if 'other_refs' in fastani_results.get(gid).get(
-                    fastani_matching_reference):
-                    other_refs = fastani_results.get(gid).get(
-                        fastani_matching_reference).get('other_refs')
+                if 'other_refs' in skani_results.get(gid).get(
+                    skani_matching_reference):
+                    other_refs = skani_results.get(gid).get(
+                        skani_matching_reference).get('other_refs')
                     if other_refs:
                         summary_row.other_related_refs = other_refs
-                current_ani = fastani_results.get(gid).get(
-                        fastani_matching_reference).get('ani')
-                current_af = fastani_results.get(gid).get(
-                        fastani_matching_reference).get('af')
-
-                summary_row.fastani_ref = fastani_matching_reference
-                summary_row.fastani_ref_radius = str(
-                        self.species_radius.get(fastani_matching_reference))
-                summary_row.fastani_tax = fastani_results.get(gid).get(
-                        fastani_matching_reference).get('taxonomy')
-                summary_row.fastani_ani = round(current_ani, 2)
-                summary_row.fastani_af = round(current_af,3)
+                current_ani = skani_results.get(gid).get(
+                        skani_matching_reference).get('ani')
+                current_af = skani_results.get(gid).get(
+                        skani_matching_reference).get('af')
+
+                summary_row.closest_genome_ref = skani_matching_reference
+                summary_row.closest_genome_ref_radius = str(
+                        self.species_radius.get(skani_matching_reference))
+                summary_row.closest_genome_tax = skani_results.get(gid).get(
+                        skani_matching_reference).get('taxonomy')
+                summary_row.closest_genome_ani = round(current_ani, 2)
+                summary_row.closest_genome_af = round(current_af,3)
                 taxa_str = ";".join(self.gtdb_taxonomy.get(
-                        add_ncbi_prefix(fastani_matching_reference)))
+                        add_ncbi_prefix(skani_matching_reference)))
                 summary_row.classification = standardise_taxonomy(
                         taxa_str)
 
                 classified_user_genomes.setdefault(domain, []).append(summary_row)
         return classified_user_genomes
 
     def convert_rows_to_dict(self,list_of_summary_rows):
         """Convert a list of rows to a dictionary."""
         dict_of_rows = {}
         for domain,rows in list_of_summary_rows.items():
             for row in rows:
                 if row.other_related_refs:
-                    infos ={row.gid:{row.fastani_ref: {'ani': row.fastani_ani,
-                                                 'af': row.fastani_af,
+                    infos ={row.gid:{row.closest_genome_ref: {'ani': row.closest_genome_ani,
+                                                 'af': row.closest_genome_af,
                                                  'other_refs': row.other_related_refs}}}
                 else:
-                    infos ={row.gid:{row.fastani_ref: {'ani': row.fastani_ani, 'af': row.fastani_af}}}
+                    infos ={row.gid:{row.closest_genome_ref: {'ani': row.closest_genome_ani, 'af': row.closest_genome_af}}}
                 dict_of_rows.setdefault(domain, {}).update(infos)
 
         return dict_of_rows
```

### Comparing `gtdbtk-2.3.2/gtdbtk/cli.py` & `gtdbtk-2.4.0/gtdbtk/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 def __temp_dir(group):
     group.add_argument('--tmpdir', action=ChangeTempAction, default=tempfile.gettempdir(),
                        help="specify alternative directory for temporary files")
 
 
 def __genes(group):
     group.add_argument('--genes', action='store_true', default=False,
-                       help='indicates input files contain called genes (skip gene calling).Warning: This flag will also skip '
-                            'the ANI comparison steps (ani_screen and classification).')
+                       help='indicates input files contain predicted proteins as amino acids (skip gene calling).'
+                            'Warning: This flag will skip the ANI comparison steps (ani_screen and classification).')
 
 
 def __genome_dir(group):
     group.add_argument(
         '--genome_dir', help="directory containing genome files in FASTA format")
 
 
@@ -72,19 +72,19 @@
 
 def __extension(group):
     group.add_argument('-x', '--extension', type=str, default='fna',
                        help='extension of files to process, ``gz`` = gzipped')
 
 def __skip_ani_screen(group):
     group.add_argument('--skip_ani_screen', action="store_true", default=False,
-                       help="Skip the ani_screening step to classify genomes using mash and FastANI ")
+                       help="Skip the ani_screening step to classify genomes using mash and skani.")
 
 def __skip_gtdb_refs(group):
     group.add_argument('--skip_gtdb_refs', action="store_true", default=False,
-                       help='do not include GTDB reference genomes in multiple sequence alignment')
+                       help='do not include GTDB reference genomes in multiple sequence alignment.')
 
 
 def __taxa_filter(group):
     group.add_argument('--taxa_filter', type=str, default=None,
                        help=('filter GTDB genomes to taxa (comma separated) within '
                              + 'specific taxonomic groups (e.g.: ``d__Bacteria`` '
                              + 'or ``p__Proteobacteria,p__Actinobacteria``)'))
@@ -540,15 +540,15 @@
         with arg_group(parser, 'optional Mash arguments') as grp:
             __no_mash(grp)
             __mash_k(grp)
             __mash_s(grp)
             __mash_d(grp)
             __mash_v(grp)
             __mash_db(grp)
-        with arg_group(parser, 'optional FastANI arguments') as grp:
+        with arg_group(parser, 'optional skani arguments') as grp:
             __min_af(grp)
         with arg_group(parser, 'optional arguments') as grp:
             __extension(grp)
             __prefix(grp)
             __cpus(grp)
             __temp_dir(grp)
             __debug(grp)
```

### Comparing `gtdbtk-2.3.2/gtdbtk/config/common.py` & `gtdbtk-2.4.0/gtdbtk/config/common.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 class __GTDBTkCommonConfig:
     """
     This class encapsulates all configuration options. It will protect against
     importing code that depends on a specific value throwing an exception
     that requires the setting of the GTDB-Tk reference data path.
     """
 
-    MIN_REF_DATA_VERSION = 'r207'
-    COMPATIBLE_REF_DATA_VERSIONS = ['r207','r214']
+    MIN_REF_DATA_VERSION = 'r220'
+    COMPATIBLE_REF_DATA_VERSIONS = ['r220']
 
     BACKBONE_PPLACER_REF_PKG = 'gtdbtk_package_backbone.refpkg'
     CLASS_LEVEL_PPLACER_REF_PKG = 'gtdbtk.package.{iter}.refpkg'
 
     # Relative Evolution Distance
     RED_INTERVAL = 0.1
     RED_MIN_SUPPORT = 0.0
@@ -84,23 +84,23 @@
     DEFAULT_MULTIHIT_THRESHOLD = 10.0
 
     # Information for aligning genomes
     DEFAULT_DOMAIN_THRESHOLD = 10.0
     AR_MARKER_COUNT = 53
     BAC_MARKER_COUNT = 120
 
-    # Information about alignment Fraction to resolve fastANI results
+    # Information about alignment Fraction to resolve skani results
     AF_THRESHOLD = 0.5
 
     PPLACER_MIN_RAM_BAC_FULL = 320
     PPLACER_MIN_RAM_BAC_SPLIT = 55
     PPLACER_MIN_RAM_ARC = 40
 
-    FASTANI_SPECIES_THRESHOLD = 95.0
-    FASTANI_GENOMES_EXT = "_genomic.fna.gz"
+    SKANI_SPECIES_THRESHOLD = 95.0
+    SKANI_GENOMES_EXT = "_genomic.fna.gz"
 
     # Mash configuration
     MASH_SKETCH_FILE = 'gtdb_ref_sketch.msh'
     MASH_K_VALUE = 16
     MASH_S_VALUE = 5000
     MASH_MAX_DISTANCE = 0.15
     MASH_D_VALUE = MASH_MAX_DISTANCE
@@ -146,16 +146,16 @@
         return os.path.join(self.GENERIC_PATH, 'masks/')
 
     @property
     def PPLACER_DIR(self):
         return os.path.join(self.GENERIC_PATH, 'pplacer/')
 
     @property
-    def FASTANI_DIR(self):
-        return os.path.join(self.GENERIC_PATH, 'fastani/')
+    def SKANI_DIR(self):
+        return os.path.join(self.GENERIC_PATH, 'skani/')
 
     @property
     def MASH_DIR(self):
         return os.path.join(self.GENERIC_PATH, 'mash/')
 
     @property
     def TAX_FOLDER(self):
@@ -309,59 +309,48 @@
         return f"gtdb_{self.VERSION_DATA}_ar53.refpkg"
 
     @property
     def PPLACER_RPS23_REF_PKG(self):
         return f"gtdb_{self.VERSION_DATA}_rps23.refpkg"
 
     @property
-    def FASTANI_GENOMES(self):
-        return os.path.join(self.FASTANI_DIR, "database/")
+    def SKANI_GENOMES(self):
+        return os.path.join(self.SKANI_DIR, "database/")
 
     @property
-    def FASTANI_GENOME_LIST(self):
-        return os.path.join(self.FASTANI_DIR, "genome_paths.tsv")
+    def SKANI_GENOME_LIST(self):
+        return os.path.join(self.SKANI_DIR, "genome_paths.tsv")
 
     @property
     def MRCA_RED_BAC120(self):
         return os.path.join(self.RED_DIR, f"gtdbtk_{self.VERSION_DATA}_bac120.tsv")
 
     @property
     def MRCA_RED_AR53(self):
         return os.path.join(self.RED_DIR, f"gtdbtk_{self.VERSION_DATA}_ar53.tsv")
 
     def get_REF_HASHES(self,version=None):
         compatible_versions = [int(x.replace('r','')) for x in CONFIG.COMPATIBLE_REF_DATA_VERSIONS]
         if version is not None and version not in compatible_versions:
             raise ValueError(f"Version {version} is not compatible with this version of GTDB-Tk. Compatible versions are {compatible_versions}")
 
-        if version is None or version==214:
+        if version is None or version==220:
             return {
-                self.PPLACER_DIR: '6786e9fc16b31db7d6eaaa9f8cfa87a8a4974434',
-                self.MASK_DIR: '8d5a2139feabbb70789c62155f3761d2aeed1601',
+                self.PPLACER_DIR: '75fdd0e093c9af6a73cb510c3d0cd2041265e093',
+                self.MASK_DIR: 'f4b8ebfa59526a7a86f09752b47e8de1efc384c7',
                 self.MARKER_DIR: '163f542c3f0a40f59df45d453aa235b39aa96e27',
-                self.RADII_DIR: '4753acc920001a1400788ee89cb4632900449055',
-                self.MSA_FOLDER: '75df495678a121497e14346b453caf42f4b03922',
-                self.METADATA_DIR: 'a089cc36bf79a40c7506019accc5f93e940d9fed',
-                self.TAX_FOLDER: '89b12cf8106f326887599dcb30ef94ebba142035',
-                self.FASTANI_DIR: 'e12824beccc15fe67a373e2aa8eee72feecf89c6',
-                self.RED_DIR: 'c24a2f48bb0c1df38f92a8f526aa846f596c94c6'
-            }
-        elif version==207:
-            return {
-                self.PPLACER_DIR: '20903925a856a58b102a7b0ce160c5cbd2cf675b',
-                self.MASK_DIR: '50e414a9de18170e8cb97f990f89ff60a0fe29d5',
-                self.MARKER_DIR: '163f542c3f0a40f59df45d453aa235b39aa96e27',
-                self.RADII_DIR: '8fd13b1c5d7a7b073ba96fb628581613b293a374',
-                self.MSA_FOLDER: '24f250d7cf0eb0bc65dccd2f3c9247e553ea322f',
-                self.METADATA_DIR: '9772fbeac1311b31e10293fa610eb33aa1ec8e15',
-                self.TAX_FOLDER: '6fb0233b05633242369b40c026fd1ee53e266afa',
-                self.FASTANI_DIR: '973c456c02f55bb82908a6811c7076e207e9b206',
-                self.RED_DIR: '7b8b67b3157204b470c9eb809d3c39c4effffabc'
+                self.RADII_DIR: '63d06ecc8b4547addd22c5b06ada4a28c5332bcc',
+                self.MSA_FOLDER: '3d5c1cf5346b244fcb0a9d48d2f1a9358a71cc7a',
+                self.METADATA_DIR: '01b8c23253cef097b1bc233d609dae9eb84c98e2',
+                self.TAX_FOLDER: '6758173fa61ae4a77f5588ec2874ea52ed345feb',
+                self.SKANI_DIR: 'ff58a1d7e0584da324d140701ee12cead4f0df9d',
+                self.RED_DIR: '206bd781997fffbac951b4437dd75e6543139fd6'
             }
 
+
     REF_HASHES = property(get_REF_HASHES)
 
 
 # Export the class for import by other modules
 @lru_cache(maxsize=1)
 def __get_config():
     return __GTDBTkCommonConfig()
```

### Comparing `gtdbtk-2.3.2/gtdbtk/config/output.py` & `gtdbtk-2.4.0/gtdbtk/config/output.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,16 +59,16 @@
 PATH_BAC120_CLASS_LEVEL_PPLACER_CLASS = join(DIR_CLASSIFY_INTERMEDIATE, '{prefix}.bac120.class_level.classification_pplacer_tree_{iter}.tsv')
 PATH_BAC120_PRESCREEN_MSA = join(DIR_CLASSIFY_INTERMEDIATE, '{prefix}.bac120.prescreened.msa.fasta')
 PATH_AR53_PRESCREEN_MSA = join(DIR_CLASSIFY_INTERMEDIATE, '{prefix}.ar53.prescreened.msa.fasta')
 
 #Command: ani_screen
 DIR_ANISCREEN = join(DIR_CLASSIFY, 'ani_screen')
 DIR_ANISCREEN_INTERMEDIATE = join(DIR_ANISCREEN, 'intermediate_results')
-PATH_BAC120_ANI_FASTANI = join(DIR_ANISCREEN, '{prefix}.bac120_fastani.summary.tsv')
-PATH_AR53_ANI_FASTANI = join(DIR_ANISCREEN, '{prefix}.ar53_fastani.summary.tsv')
+PATH_BAC120_ANI_SKANI = join(DIR_ANISCREEN, '{prefix}.bac120_skani.summary.tsv')
+PATH_AR53_ANI_SKANI = join(DIR_ANISCREEN, '{prefix}.ar53_skani.summary.tsv')
 
 
 DIR_PPLACER = join(DIR_CLASSIFY_INTERMEDIATE, 'pplacer')
 PATH_BAC120_PPLACER_OUT = join(DIR_PPLACER, 'pplacer.bac120.out')
 PATH_AR53_PPLACER_OUT = join(DIR_PPLACER, 'pplacer.ar53.out')
 PATH_BAC120_PPLACER_JSON = join(DIR_PPLACER, 'pplacer.bac120.json')
 PATH_AR53_PPLACER_JSON = join(DIR_PPLACER, 'pplacer.ar53.json')
```

### Comparing `gtdbtk-2.3.2/gtdbtk/decorate.py` & `gtdbtk-2.4.0/gtdbtk/decorate.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/gtdbtk/exceptions.py` & `gtdbtk-2.4.0/gtdbtk/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,16 +117,16 @@
 class TogException(GTDBTkException):
     """ Thrown whenever an error is encountered while running tog. """
 
     def __init__(self, message=''):
         GTDBTkException.__init__(self, message)
 
 
-class FastANIException(GTDBTkException):
-    """ Thrown when an exception is encountered while running FastANI. """
+class SkANIException(GTDBTkException):
+    """ Thrown when an exception is encountered while running skani. """
 
     def __init__(self, message=''):
         GTDBTkException.__init__(self, message)
 
 
 class FastTreeException(GTDBTkException):
     """ Thrown when an exception is encountered while running FastTree. """
```

### Comparing `gtdbtk-2.3.2/gtdbtk/external/fastani.py` & `gtdbtk-2.4.0/gtdbtk/external/fastani.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/gtdbtk/external/fasttree.py` & `gtdbtk-2.4.0/gtdbtk/external/fasttree.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/gtdbtk/external/hmm_aligner.py` & `gtdbtk-2.4.0/gtdbtk/external/hmm_aligner.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/gtdbtk/external/mash.py` & `gtdbtk-2.4.0/gtdbtk/external/mash.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/gtdbtk/external/pfam_search.py` & `gtdbtk-2.4.0/gtdbtk/external/pfam_search.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/gtdbtk/external/pplacer.py` & `gtdbtk-2.4.0/gtdbtk/external/pplacer.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 import logging
 import multiprocessing as mp
 import os
 import queue
 import re
 import subprocess
+import sys
 
 from tqdm import tqdm
 
 from gtdbtk.exceptions import PplacerException, TogException
 from gtdbtk.tools import get_proc_memory_gb
 
 
@@ -72,14 +73,16 @@
         if mmap_file:
             args.append('--mmap-file')
             args.append(mmap_file)
         self.logger.debug(' '.join(args))
 
         out_q = mp.Queue()
         pid = mp.Value('i', 0)
+        # print(f'Running pplacer with the following command: {" ".join(args)}')
+        # sys.exit(0)
         p_worker = mp.Process(target=self._worker, args=(
             args, out_q, pplacer_out, pid))
         p_writer = mp.Process(target=self._writer, args=(out_q, pid))
 
         try:
             p_worker.start()
             p_writer.start()
```

### Comparing `gtdbtk-2.3.2/gtdbtk/external/prodigal.py` & `gtdbtk-2.4.0/gtdbtk/external/prodigal.py`

 * *Files 6% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         gff_file = os.path.join(output_dir, genome_id + self.gff_file_suffix)
         out_files = (nt_gene_file, gff_file, tln_table_file.path, aa_gene_file)
 
         # Check if this genome has already been processed (skip).
         if all([file_has_checksum(x) for x in out_files]):
             tln_table_file.read()
             self.warnings.info(f'Skipped Prodigal processing for: {genome_id}')
-            return aa_gene_file, nt_gene_file, gff_file, tln_table_file.path, tln_table_file.best_tln_table, True
+            return aa_gene_file, nt_gene_file, gff_file, tln_table_file.path, tln_table_file.best_tln_table, True , False
 
         # Run Prodigal
         prodigal = BioLibProdigal(1, False)
         summary_stats = prodigal.run([fasta_path], output_dir,
                                      called_genes=False,
                                      translation_table=usr_tln_table)
 
@@ -106,33 +106,42 @@
             if self.force:
                 return None
             else:
                 raise Exception("An error was encountered while running Prodigal.")
 
         summary_stats = summary_stats[list(summary_stats.keys())[0]]
 
-        # rename output files to adhere to GTDB conventions and desired genome
-        # ID
-        shutil.move(summary_stats.aa_gene_file, aa_gene_file)
-        shutil.move(summary_stats.nt_gene_file, nt_gene_file)
-        shutil.move(summary_stats.gff_file, gff_file)
-
-        # save translation table information
-        tln_table_file.best_tln_table = summary_stats.best_translation_table
-        tln_table_file.coding_density_4 = round(summary_stats.coding_density_4 * 100, 2)
-        tln_table_file.coding_density_11 = round(summary_stats.coding_density_11 * 100, 2)
-        tln_table_file.write()
-
-        # Create a hash of each file
-        for out_file in out_files:
-            if out_file is not None:
-                with open(out_file + CHECKSUM_SUFFIX, 'w') as fh:
-                    fh.write(sha256(out_file))
+        if summary_stats.is_empty:
+            shutil.rmtree(output_dir)
+            if self.force:
+                return summary_stats
+            else:
+                raise Exception("An error was encountered while running Prodigal.")
 
-        return aa_gene_file, nt_gene_file, gff_file, tln_table_file.path, summary_stats.best_translation_table, False
+        else:
+            # rename output files to adhere to GTDB conventions and desired genome
+            # ID
+            shutil.move(summary_stats.aa_gene_file, aa_gene_file)
+            shutil.move(summary_stats.nt_gene_file, nt_gene_file)
+            shutil.move(summary_stats.gff_file, gff_file)
+
+            # save translation table information
+            tln_table_file.best_tln_table = summary_stats.best_translation_table
+            tln_table_file.coding_density_4 = round(summary_stats.coding_density_4 * 100, 2)
+            tln_table_file.coding_density_11 = round(summary_stats.coding_density_11 * 100, 2)
+            tln_table_file.write()
+
+            # Create a hash of each file
+            for out_file in out_files:
+                if out_file is not None:
+                    with open(out_file + CHECKSUM_SUFFIX, 'w') as fh:
+                        fh.write(sha256(out_file))
+
+
+        return aa_gene_file, nt_gene_file, gff_file, tln_table_file.path, summary_stats.best_translation_table, False , summary_stats.is_empty
 
     def _worker(self, out_dict, worker_queue, writer_queue, n_skipped):
         """This worker function is invoked in a process."""
 
         while True:
             data = worker_queue.get(block=True, timeout=None)
             if data is None:
@@ -140,23 +149,24 @@
 
             genome_id, file_path, usr_tln_table = data
 
             rtn_files = self._run_prodigal(genome_id, file_path, usr_tln_table)
 
             # Only proceed if an error didn't occur in BioLib Prodigal
             if rtn_files:
-                aa_gene_file, nt_gene_file, gff_file, translation_table_file, best_translation_table, was_skipped = rtn_files
+                aa_gene_file, nt_gene_file, gff_file, translation_table_file, best_translation_table, was_skipped ,is_empty = rtn_files
                 if was_skipped:
                     with n_skipped.get_lock():
                         n_skipped.value += 1
                 prodigal_infos = {"aa_gene_path": aa_gene_file,
                                   "nt_gene_path": nt_gene_file,
                                   "gff_path": gff_file,
                                   "translation_table_path": translation_table_file,
-                                  "best_translation_table": best_translation_table}
+                                  "best_translation_table": best_translation_table,
+                                  "is_empty": is_empty}
 
                 out_dict[genome_id] = prodigal_infos
             writer_queue.put(genome_id)
 
     def _writer(self, num_items, writer_queue):
         """Store or write results of worker threads in a single thread."""
         with tqdm_log(total=num_items,  unit='genome') as p_bar:
@@ -221,39 +231,50 @@
 
         # Report if any genomes were skipped due to having already been processed.
         if n_skipped.value > 0:
             genome_s = 'genome' if n_skipped.value == 1 else 'genomes'
             self.logger.warning(f'Prodigal skipped {n_skipped.value} {genome_s} '
                                 f'due to pre-existing data, see warnings.log')
 
+
         # Report on any genomes which failed to have any genes called
         result_dict = dict()
         lq_gids = list()
+        empty_gids = list()
         fails = open(self.failed_genomes_file,'w')
         for gid, gid_dict in out_dict.items():
-            if os.path.getsize(gid_dict['aa_gene_path']) <= 1:
+            if gid_dict['is_empty']:
+                empty_gids.append(gid)
+            elif os.path.getsize(gid_dict['aa_gene_path']) <= 1:
                 lq_gids.append(gid)
             else:
                 result_dict[gid] = gid_dict
 
         if len(lq_gids) > 0:
-            self.logger.warning(f'Skipping {len(lq_gids)} of {len(genomic_files)} '
+            self.logger.warning(f'Skipping {len(lq_gids+empty_gids)} of {len(genomic_files)} '
                                 f'genomes as no genes were called by Prodigal. '
                                 f'Check the genome quality (see gtdbtk.warnings.log).')
-            self.warnings.warning(f'The following {len(lq_gids)} genomes have '
+            self.warnings.warning(f'The following {len(lq_gids+empty_gids)} genomes have '
                                   f'been excluded from analysis due to Prodigal '
                                   f'failing to call any genes:')
 
 
             # If there are few low-quality genomes just output to console.
-            if len(lq_gids) > 10:
+            if len(lq_gids+empty_gids) > 10:
                 for lq_gid in lq_gids:
                     self.warnings.info(lq_gid)
                     fails.write(f'{lq_gid}\tNo genes were called by Prodigal\n')
+                for empty_gid in empty_gids:
+                    self.warnings.info(empty_gid)
+                    fails.write(f'{empty_gid}\tEmpty file\n')
             else:
                 for lq_gid in lq_gids:
                     self.logger.warning(f'Skipping: {lq_gid}')
                     self.warnings.info(lq_gid)
                     fails.write(f'{lq_gid}\tNo genes were called by Prodigal\n')
+                for empty_gid in empty_gids:
+                    self.logger.warning(f'Skipping: {empty_gid}')
+                    self.warnings.info(empty_gid)
+                    fails.write(f'{empty_gid}\tEmpty file\n')
 
         fails.close()
         return result_dict
```

### Comparing `gtdbtk-2.3.2/gtdbtk/external/pypfam/HMM/HMMMatch.py` & `gtdbtk-2.4.0/gtdbtk/external/pypfam/HMM/HMMMatch.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/gtdbtk/external/pypfam/HMM/HMMResults.py` & `gtdbtk-2.4.0/gtdbtk/external/pypfam/HMM/HMMResults.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/gtdbtk/external/pypfam/HMM/HMMResultsIO.py` & `gtdbtk-2.4.0/gtdbtk/external/pypfam/HMM/HMMResultsIO.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/gtdbtk/external/pypfam/HMM/HMMSequence.py` & `gtdbtk-2.4.0/gtdbtk/external/pypfam/HMM/HMMSequence.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/gtdbtk/external/pypfam/HMM/HMMUnit.py` & `gtdbtk-2.4.0/gtdbtk/external/pypfam/HMM/HMMUnit.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/gtdbtk/external/pypfam/Scan/PfamScan.py` & `gtdbtk-2.4.0/gtdbtk/external/pypfam/Scan/PfamScan.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/gtdbtk/external/tigrfam_search.py` & `gtdbtk-2.4.0/gtdbtk/external/tigrfam_search.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/gtdbtk/files/batchfile.py` & `gtdbtk-2.4.0/gtdbtk/files/batchfile.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/gtdbtk/files/classify_summary.py` & `gtdbtk-2.4.0/gtdbtk/files/classify_summary.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,30 +23,30 @@
 from gtdbtk.config.output import PATH_AR53_SUMMARY_OUT, PATH_BAC120_SUMMARY_OUT
 from gtdbtk.exceptions import GTDBTkExit
 
 
 class ClassifySummaryFileRow:
     """A row contained within the ClassifySummaryFile object."""
 
-    __slots__ = ('gid', 'classification', 'fastani_ref', 'fastani_ref_radius',
-                 'fastani_tax', 'fastani_ani', 'fastani_af', 'closest_placement_ref',
+    __slots__ = ('gid', 'classification', 'closest_genome_ref', 'closest_genome_ref_radius',
+                 'closest_genome_tax', 'closest_genome_ani', 'closest_genome_af', 'closest_placement_ref',
                  'closest_placement_radius', 'closest_placement_tax', 'closest_placement_ani',
                  'closest_placement_af', 'pplacer_tax', 'classification_method',
                  'note', 'other_related_refs', 'msa_percent', 'tln_table',
                  'red_value', 'warnings')
 
     def __init__(self):
         """Initialise the row, default all the values to None."""
         self.gid: Optional[str] = None
         self.classification: Optional[str] = None
-        self.fastani_ref: Optional[str] = None
-        self.fastani_ref_radius: Optional[float] = None
-        self.fastani_tax: Optional[str] = None
-        self.fastani_ani: Optional[float] = None
-        self.fastani_af: Optional[float] = None
+        self.closest_genome_ref: Optional[str] = None
+        self.closest_genome_ref_radius: Optional[float] = None
+        self.closest_genome_tax: Optional[str] = None
+        self.closest_genome_ani: Optional[float] = None
+        self.closest_genome_af: Optional[float] = None
         self.closest_placement_ref: Optional[str] = None
         self.closest_placement_radius: Optional[float] = None
         self.closest_placement_tax: Optional[str] = None
         self.closest_placement_ani: Optional[float] = None
         self.closest_placement_af: Optional[float] = None
         self.pplacer_tax: Optional[str] = None
         self.classification_method: Optional[str] = None
@@ -74,19 +74,19 @@
     def get_col_order(row: ClassifySummaryFileRow = None) -> Tuple[List[str], List[Union[str, float, int]]]:
         """Return the column order that will be written. If a row is provided
         then format the row in that specific order."""
         if row is None:
             row = ClassifySummaryFileRow()
         mapping = [('user_genome', row.gid),
                    ('classification', row.classification),
-                   ('fastani_reference', row.fastani_ref),
-                   ('fastani_reference_radius', row.fastani_ref_radius),
-                   ('fastani_taxonomy', row.fastani_tax),
-                   ('fastani_ani', row.fastani_ani),
-                   ('fastani_af', row.fastani_af),
+                   ('closest_genome_reference', row.closest_genome_ref),
+                   ('closest_genome_reference_radius', row.closest_genome_ref_radius),
+                   ('closest_genome_taxonomy', row.closest_genome_tax),
+                   ('closest_genome_ani', row.closest_genome_ani),
+                   ('closest_genome_af', row.closest_genome_af),
                    ('closest_placement_reference', row.closest_placement_ref),
                    ('closest_placement_radius', row.closest_placement_radius),
                    ('closest_placement_taxonomy', row.closest_placement_tax),
                    ('closest_placement_ani', row.closest_placement_ani),
                    ('closest_placement_af', row.closest_placement_af),
                    ('pplacer_taxonomy', row.pplacer_tax),
                    ('classification_method', row.classification_method),
@@ -103,14 +103,24 @@
         return cols, data
 
     def add_row(self, row: ClassifySummaryFileRow):
         if row.gid in self.rows:
             raise GTDBTkExit(f'Attempting to add duplicate row: {row.gid}')
         self.rows[row.gid] = row
 
+    def get_row(self, gid: str) -> ClassifySummaryFileRow:
+        if gid not in self.rows:
+            raise GTDBTkExit(f'Attempting to get non-existent row: {gid}')
+        return self.rows[gid]
+
+    def update_row(self, row: ClassifySummaryFileRow):
+        if row.gid not in self.rows:
+            raise GTDBTkExit(f'Attempting to update non-existent row: {row.gid}')
+        self.rows[row.gid] = row
+
     def has_row(self) -> bool:
         if self.rows.items():
             return True
         return False
 
     def get_gid_taxonomy(self) -> Dict[str, List[str]]:
         out = dict()
@@ -149,19 +159,19 @@
 
             # Process the data.
             for line in fh.readlines():
                 data = line.strip().split('\t')
                 row = ClassifySummaryFileRow()
                 row.gid = data[0]
                 row.classification = data[1]
-                row.fastani_ref = data[2]
-                row.fastani_ref_radius = data[3]
-                row.fastani_tax = data[4]
-                row.fastani_ani = data[5]
-                row.fastani_af = data[6]
+                row.closest_genome_ref = data[2]
+                row.closest_genome_ref_radius = data[3]
+                row.closest_genome_tax = data[4]
+                row.closest_genome_ani = data[5]
+                row.closest_genome_af = data[6]
                 row.closest_placement_ref = data[7]
                 row.closest_placement_radius = data[8]
                 row.closest_placement_tax = data[9]
                 row.closest_placement_ani = data[10]
                 row.closest_placement_af = data[11]
                 row.pplacer_tax = data[12]
                 row.classification_method = data[13]
```

### Comparing `gtdbtk-2.3.2/gtdbtk/files/gtdb_radii.py` & `gtdbtk-2.4.0/gtdbtk/files/gtdb_radii.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/gtdbtk/files/marker/copy_number.py` & `gtdbtk-2.4.0/gtdbtk/files/marker/copy_number.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/gtdbtk/files/marker/tophit.py` & `gtdbtk-2.4.0/gtdbtk/files/marker/tophit.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/gtdbtk/files/marker_info.py` & `gtdbtk-2.4.0/gtdbtk/files/marker_info.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/gtdbtk/files/missing_genomes.py` & `gtdbtk-2.4.0/gtdbtk/files/missing_genomes.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/gtdbtk/files/pplacer_classification.py` & `gtdbtk-2.4.0/gtdbtk/files/pplacer_classification.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/gtdbtk/files/prodigal/tln_table.py` & `gtdbtk-2.4.0/gtdbtk/files/prodigal/tln_table.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/gtdbtk/files/prodigal/tln_table_summary.py` & `gtdbtk-2.4.0/gtdbtk/files/prodigal/tln_table_summary.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/gtdbtk/files/red_dict.py` & `gtdbtk-2.4.0/gtdbtk/files/red_dict.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/gtdbtk/files/stage_logger.py` & `gtdbtk-2.4.0/gtdbtk/files/stage_logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     name: str = "ANI screen"
     genome_dir: Optional[str]
     batchfile: Optional[str]
     mash_k: Optional[str]
     mash_s: Optional[str]
     mash_v: Optional[str]
     mash_max_dist: Optional[str]
+    min_af: Optional[str]
     mash_db: Optional[str]
     output_files: Optional[Dict]
 
 class IdentifyStep(Steps):
     """ Information about the Identify step of GTDB-Tk"""
     name: str = "identify"
     genes: Optional[bool]
```

### Comparing `gtdbtk-2.3.2/gtdbtk/files/tree_mapping.py` & `gtdbtk-2.4.0/gtdbtk/files/tree_mapping.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/gtdbtk/infer_ranks.py` & `gtdbtk-2.4.0/gtdbtk/infer_ranks.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/gtdbtk/main.py` & `gtdbtk-2.4.0/gtdbtk/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -360,15 +360,15 @@
         align_step.outgroup_taxon = options.outgroup_taxon if hasattr(options, 'outgroup_taxon') else None
 
         check_dir_exists(options.identify_dir)
         align_step.identify_dir = options.identify_dir
         make_sure_path_exists(options.out_dir)
 
         markers = Markers(options.cpus, options.debug)
-        reports = markers.align(options.identify_dir,
+        reports,all_failed_prodigal = markers.align(options.identify_dir,
                       options.skip_gtdb_refs,
                       options.taxa_filter,
                       options.min_perc_aa,
                       options.custom_msa_filters,
                       options.skip_trimming,
                       options.rnd_seed,
                       options.cols_per_gene,
@@ -386,15 +386,15 @@
         align_step.duration = str(duration - timedelta(microseconds=duration.microseconds))
         align_step.output_files = reports
         align_step.status = 'completed'
 
         self.stage_logger.steps.append(align_step)
 
         self.logger.info('Done.')
-
+        return all_failed_prodigal
 
     def infer(self, options):
         """Infer a tree from a user specified MSA.
 
         Parameters
         ----------
         options : argparse.Namespace
@@ -532,15 +532,15 @@
         finally:
             if out_dir_fh:
                 out_dir_fh.cleanup()
 
         self.logger.info('Test has successfully finished.')
         return True
 
-    def classify(self, options,all_classified_ani=False):
+    def classify(self, options,all_classified_ani=False,all_failed_prodigal=False):
         """Determine taxonomic classification of genomes.
 
         Parameters
         ----------
         options : argparse.Namespace
             The CLI arguments input by the user.
         """
@@ -596,15 +596,16 @@
                      no_mash=options.no_mash,
                      mash_k=options.mash_k,
                      mash_v=options.mash_v,
                      mash_s=options.mash_s,
                      mash_db=options.mash_db,
                      mash_max_dist=options.mash_max_distance,
                      ani_summary_files=ani_summary_files,
-                     all_classified_ani=all_classified_ani
+                     all_classified_ani=all_classified_ani,
+                     all_failed_prodigal=all_failed_prodigal
                      )
 
         classify_step.ends_at = datetime.now()
         duration = classify_step.ends_at - classify_step.starts_at
         classify_step.output_files = reports
         #we round the duration to the nearest second
         classify_step.duration = str(duration - timedelta(microseconds=duration.microseconds))
@@ -621,15 +622,15 @@
         self.logger.info('Note that Tk classification mode is insufficient for publication of new taxonomic '
                          'designations. New designations should be based on one or more de novo trees, an '
                          'example of which can be produced by Tk in de novo mode.')
 
         self.logger.info('Done.')
 
     def ani_screen(self, options ):
-        """Run a mash/FastANI screen of all user genomes
+        """Run a mash/skani screen of all user genomes
         against the reference genomes.
 
         Parameters
         ----------
         options : argparse.Namespace
             The CLI arguments input by the user.
         """
@@ -637,38 +638,32 @@
         ani_step = ANIScreenStep()
         ani_step.starts_at = datetime.now()
         ani_step.output_dir = options.out_dir
         ani_step.mash_db = options.mash_db
         ani_step.mash_k = options.mash_k
         ani_step.mash_v = options.mash_v
         ani_step.mash_s = options.mash_s
+        ani_step.min_af = options.min_af
         ani_step.mash_max_dist = options.mash_max_distance
 
         if options.genome_dir:
             check_dir_exists(options.genome_dir)
             ani_step.genome_dir = options.genome_dir
 
         if options.batchfile:
             check_file_exists(options.batchfile)
             ani_step.batchfile = options.batchfile
 
         make_sure_path_exists(options.out_dir)
 
-        genomes, tln_tables = self._genomes_to_process(options.genome_dir,
-                                                       options.batchfile,
-                                                       options.extension)
-        self.genomes_to_process = genomes
-
-        make_sure_path_exists(options.out_dir)
-
         genomes, _ = self._genomes_to_process(options.genome_dir,
                                               options.batchfile,
                                               options.extension)
 
-        aniscreener = ANIScreener(options.cpus)
+        aniscreener = ANIScreener(options.cpus,options.min_af)
         classified_genomes,reports = aniscreener.run_aniscreen(
             genomes=genomes,
             no_mash=options.no_mash,
             out_dir=options.out_dir,
             prefix=options.prefix,
             mash_k=options.mash_k,
             mash_v=options.mash_v,
@@ -1079,15 +1074,15 @@
 
             if not options.keep_intermediates:
                 self.remove_intermediate_files(options.out_dir,'de_novo_wf')
 
         elif options.subparser_name == 'classify_wf':
 
             check_dependencies(['prodigal', 'hmmalign', 'pplacer', 'guppy',
-                                'fastANI'])
+                                'skani'])
 
             if options.write_single_copy_genes and not options.keep_intermediates:
                 self.logger.warning('--write_single_copy_genes flag is set to True,'
                                     ' but --keep_intermediates is set to False. '
                                     'The intermediate folder containing the single copy genes will be removed.')
                 if not confirm('Do you want to proceed?'):
                     self.logger.info('Exiting workflow.')
@@ -1116,15 +1111,15 @@
                 if self.stage_logger.has_stage(ANIScreenStep):
                     # we get the genomes already classified by the ani_screen step
                     previous_ani_step = self.stage_logger.get_stage(ANIScreenStep)
                     if previous_ani_step.is_complete():
                         self.logger.warning('The ani_screen step has already been completed, we load existing results.')
                         ani_summary_files = previous_ani_step.output_files
                         classify_method = Classify()
-                        classified_genomes=classify_method.load_fastani_results_pre_pplacer(ani_summary_files)
+                        classified_genomes=classify_method.load_skani_results_pre_pplacer(ani_summary_files)
                         classified_genomes = classify_method.convert_rows_to_dict(classified_genomes)
                         len_mash_classified_bac120 = len(classified_genomes['bac120']) \
                             if 'bac120' in classified_genomes else 0
 
                         len_mash_classified_ar53 = len(classified_genomes['ar53']) \
                             if 'ar53' in classified_genomes else 0
 
@@ -1157,37 +1152,38 @@
 
             if not options.skip_ani_screen:
                 all_classified_ani,classified_genomes = self.ani_screen(options)
 
             # if all genomes have been classified by the ani_screen step, we do not need to run the identify step
             options.identify_dir = options.out_dir
             options.align_dir = options.out_dir
+            all_failed_prodigal = False
             if all_classified_ani:
                 self.logger.info('All genomes have been classified by the ANI screening step, Identify and Align steps will be skipped.')
             else:
-                self.identify(options,classified_genomes)
+                self.identify(options, classified_genomes)
                 options.taxa_filter = None
                 options.custom_msa_filters = False
                 # Added here due to the other mutex argument being included above.
                 options.skip_trimming = False
                 options.min_consensus = None
                 options.min_perc_taxa = None
                 options.skip_gtdb_refs = False
                 options.cols_per_gene = None
                 options.max_consensus = None
                 options.rnd_seed = None
                 options.skip_trimming = False
 
-                self.align(options)
+                all_failed_prodigal = self.align(options)
 
             # because we run ani_screen before the identify step, we do not need to rerun the
             #ani step again, so we set the skip_aniscreen to True
             options.skip_ani_screen = True
 
-            self.classify(options,all_classified_ani= all_classified_ani)
+            self.classify(options,all_classified_ani= all_classified_ani,all_failed_prodigal=all_failed_prodigal)
             if not options.keep_intermediates:
                 self.remove_intermediate_files(options.out_dir,'classify_wf')
 
 
         elif options.subparser_name == 'identify':
             self.identify(options)
         elif options.subparser_name == 'align':
@@ -1219,15 +1215,15 @@
             self.convert_to_species(options)
         elif options.subparser_name == 'trim_msa':
             self.trim_msa(options)
         elif options.subparser_name == 'export_msa':
             self.export_msa(options)
         elif options.subparser_name == 'test':
             check_dependencies(['prodigal', 'hmmalign', 'pplacer', 'guppy',
-                                'fastANI'])
+                                'skani'])
             self.run_test(options)
         elif options.subparser_name == 'check_install':
             self.check_install(options)
         else:
             self.logger.error('Unknown GTDB-Tk command: "' +
                               options.subparser_name + '"\n')
             sys.exit(1)
```

### Comparing `gtdbtk-2.3.2/gtdbtk/markers.py` & `gtdbtk-2.4.0/gtdbtk/markers.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,19 +217,25 @@
                                           'gff_path': None}
                 # we create a symlink to the genome file in the marker gene directory
                 # so we can use this symlink in the align step
                 symlink_protein_dir = os.path.join(self.marker_gene_dir, gid)
                 make_sure_path_exists(symlink_protein_dir)
                 symlink_f(os.path.abspath(gpath), os.path.join(symlink_protein_dir,gid+self.protein_file_suffix))
 
+        gene_files = [(db_genome_id, genome_dictionary[db_genome_id]['aa_gene_path'])
+                      for db_genome_id in genome_dictionary.keys()]
+        # if gene_files is empty, we have no genomes to process
+        # we still need to write all the genomes failing the identify step to the bac120_summary file
+        if len(gene_files) == 0:
+            self.logger.warning('All genomes failed the identify step.')
+            return reports
+
         # annotated genes against TIGRFAM and Pfam databases
         self.logger.log(CONFIG.LOG_TASK,
                         'Identifying TIGRFAM protein families.')
-        gene_files = [(db_genome_id, genome_dictionary[db_genome_id]['aa_gene_path'])
-                      for db_genome_id in genome_dictionary.keys()]
         tigr_search = TigrfamSearch(self.cpus,
                                     self.tigrfam_hmms,
                                     self.protein_file_suffix,
                                     self.tigrfam_suffix,
                                     self.tigrfam_top_hit_suffix,
                                     self.checksum_suffix,
                                     self.marker_gene_dir)
@@ -477,14 +483,23 @@
             identify_dir, PATH_FAILS.format(prefix=prefix)))
         if os.path.isfile(failed_genomes_file):
             with open(failed_genomes_file) as fgf:
                 failed_genomes = [row.split()[0] for row in fgf]
         else:
             failed_genomes = list()
 
+        if failed_genomes and not os.path.isfile(TlnTableSummaryFile(identify_dir, prefix).path):
+            self.logger.warning(
+                f'Skipping align step.')
+            if identify_dir != out_dir and os.path.isfile(failed_genomes_file):
+                identify_path = os.path.join(out_dir, DIR_IDENTIFY)
+                make_sure_path_exists(identify_path)
+                copy(failed_genomes_file, identify_path)
+            return reports,True
+
         # If the user is re-running this step, check if the identify step is consistent.
         genomic_files = self._path_to_identify_data(
             identify_dir, identify_dir != out_dir)
         if genomes_to_process is not None and len(genomic_files) != len(genomes_to_process):
             if list(set(genomic_files.keys()) - set(genomes_to_process.keys())).sort() != failed_genomes.sort():
                 self.logger.error('{} are not present in the input list of genome to process.'.format(
                     list(set(genomic_files.keys()) - set(genomes_to_process.keys()))))
@@ -696,15 +711,15 @@
         if no_marker_gids:
             no_marker_filtered_genomes = os.path.join(out_dir, PATH_FAILED_ALIGN_GENOMES.format(prefix=prefix))
             with open(no_marker_filtered_genomes, 'w') as fout:
                 for no_marker_gid in no_marker_gids:
                     fout.write(f'{no_marker_gid}\tNo bacterial or archaeal marker\n')
             reports.setdefault('all', []).append(no_marker_filtered_genomes)
 
-        return reports
+        return reports,False
 
     def _write_individual_markers(self, user_msa, marker_set_id, marker_list, out_dir, prefix):
         marker_dir = join(out_dir, DIR_ALIGN_MARKERS)
         make_sure_path_exists(marker_dir)
 
         markers, total_msa_len = self._parse_marker_info_file(marker_list)
         marker_to_msa = dict()
```

### Comparing `gtdbtk-2.3.2/gtdbtk/misc.py` & `gtdbtk-2.4.0/gtdbtk/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,15 +244,15 @@
         -------
         bool
             True if the installation is complete, False otherwise.
         """
 
         # Check that all programs are on the system path.
         self.logger.info(f'Checking that all third-party software are on the system path:')
-        names = {'prodigal', 'hmmsearch', 'fastANI', 'mash', 'pplacer', 'guppy',
+        names = {'prodigal', 'hmmsearch', 'skani', 'mash', 'pplacer', 'guppy',
                  'FastTree', 'FastTreeMP', 'hmmalign'}
         for name in sorted(names):
             on_path = False
             try:
                 on_path = on_path or check_dependencies([name], exit_on_fail=False)
             except:
                 pass
```

### Comparing `gtdbtk-2.3.2/gtdbtk/pipeline/align.py` & `gtdbtk-2.4.0/gtdbtk/pipeline/align.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/gtdbtk/pipeline/export_msa.py` & `gtdbtk-2.4.0/gtdbtk/pipeline/export_msa.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/gtdbtk/relative_distance.py` & `gtdbtk-2.4.0/gtdbtk/relative_distance.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/gtdbtk/reroot_tree.py` & `gtdbtk-2.4.0/gtdbtk/reroot_tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         # selected until two of them give the same size
         # lineage. This will, likely, be the smallest
         # bipartition possible for the given outgroup though
         # this is not guaranteed.
         mrca = tree.mrca(taxa=outgroup_in_tree)
         mrca_leaves = len(mrca.leaf_nodes())
         while True:
-            rnd_ingroup = random.sample(ingroup_leaves, 1)[0]
+            rnd_ingroup = random.sample(tuple(ingroup_leaves), 1)[0]
             tree.reroot_at_edge(rnd_ingroup.edge,
                                 length1=0.5 * rnd_ingroup.edge_length,
                                 length2=0.5 * rnd_ingroup.edge_length)
 
             mrca = tree.mrca(taxa=outgroup_in_tree)
             if len(mrca.leaf_nodes()) == mrca_leaves:
                 break
```

### Comparing `gtdbtk-2.3.2/gtdbtk/split.py` & `gtdbtk-2.4.0/gtdbtk/split.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/gtdbtk/tests/data/genomes/genome_1.fna` & `gtdbtk-2.4.0/gtdbtk/tests/data/genomes/genome_1.fna`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/gtdbtk/tests/data/genomes/genome_2.fna` & `gtdbtk-2.4.0/gtdbtk/tests/data/genomes/genome_2.fna`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/gtdbtk/tests/data/genomes/genome_3.fna` & `gtdbtk-2.4.0/gtdbtk/tests/data/genomes/genome_3.fna`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/gtdbtk/tools.py` & `gtdbtk-2.4.0/gtdbtk/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,20 +49,20 @@
 
     Returns
     -------
     dict[str, str]
         Dict[genome_id] = fasta_path
     """
     ref_genomes = dict()
-    with open(CONFIG.FASTANI_GENOME_LIST) as g_path_file:
+    with open(CONFIG.SKANI_GENOME_LIST) as g_path_file:
         for line in g_path_file:
             (full_name, path) = line.strip().split()
-            if full_name.endswith(CONFIG.FASTANI_GENOMES_EXT):
-                accession = full_name.split(CONFIG.FASTANI_GENOMES_EXT)[0]
-            ref_genomes[accession] = os.path.join(CONFIG.FASTANI_DIR, path, full_name)
+            if full_name.endswith(CONFIG.SKANI_GENOMES_EXT):
+                accession = full_name.split(CONFIG.SKANI_GENOMES_EXT)[0]
+            ref_genomes[accession] = os.path.join(CONFIG.SKANI_DIR, path, full_name)
     return ref_genomes
 
 def aa_percent_msa(aa_string):
         aa_len = sum([1 for c in aa_string if c.isalpha()])
         aa_perc = float(aa_len) / len(aa_string)
         return round(aa_perc * 100, 2)
```

### Comparing `gtdbtk-2.3.2/gtdbtk/trim_msa.py` & `gtdbtk-2.4.0/gtdbtk/trim_msa.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,15 +237,15 @@
             if len(valid_cols) < self.subset:
                 self.logger.warning(
                     'Marker has <%d columns after filtering.' % self.subset)
                 lack_sufficient_cols += 1
                 lack_cols_marker_ids.append(marker_id)
 
             offset_valid_cols = [i + start for i in valid_cols]
-            sel_cols = random.sample(offset_valid_cols, min(
+            sel_cols = random.sample(tuple(offset_valid_cols), min(
                 self.subset, len(offset_valid_cols)))
             sampled_cols.extend(sel_cols)
 
             start = end
 
         mask = [1 if i in sampled_cols else 0 for i in range(alignment_length)]
```

### Comparing `gtdbtk-2.3.2/gtdbtk.egg-info/PKG-INFO` & `gtdbtk-2.4.0/gtdbtk.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gtdbtk
-Version: 2.3.2
+Version: 2.4.0
 Summary: A toolkit for assigning objective taxonomic classifications to bacterial and archaeal genomes.
 Home-page: https://github.com/Ecogenomics/GTDBTk
 Author: Pierre-Alain Chaumeil, Aaron Mussig and Donovan Parks
 Author-email: p.chaumeil@uq.edu.au
 Maintainer: Pierre-Alain Chaumeil, Aaron Mussig and Donovan Parks
 Maintainer-email: donovan.parks@gmail.com
 License: GPL3
@@ -16,14 +16,18 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: dendropy~=4.1
+Requires-Dist: numpy~=1.9
+Requires-Dist: tqdm~=4.35
+Requires-Dist: pydantic~=1.9
 
 # GTDB-Tk
 
 [![PyPI](https://img.shields.io/pypi/v/gtdbtk.svg)](https://pypi.python.org/pypi/gtdbtk)
 [![PyPI Downloads](https://pepy.tech/badge/gtdbtk)](https://pepy.tech/project/gtdbtk)
 [![Bioconda](https://img.shields.io/conda/vn/bioconda/gtdbtk.svg?color=43b02a)](https://anaconda.org/bioconda/gtdbtk)
 [![BioConda Downloads](https://img.shields.io/conda/dn/bioconda/gtdbtk.svg?style=flag&label=downloads&color=43b02a)](https://anaconda.org/bioconda/gtdbtk)
@@ -56,16 +60,16 @@
 ## 📖 Documentation
 
 Documentation for GTDB-Tk can be found [here](https://ecogenomics.github.io/GTDBTk/).
 
 
 ## ✨ New Features
 
-GTDB-Tk v2.3.0+ includes the following new features:
-- New functionality ``convert_to_species`` function to convert GTDB genome IDs to GTDB species names
+GTDB-Tk v2.4.0+ includes the following new features:
+- `FastANI` has been replaced by `skani` as the primary tool for computing Average Nucleotide Identity (ANI).Users may notice slight variations in the results compared to those obtained using `FastANI`.
 
 
 ## 📈 Performance
 Using ANI screen "can" reduce computation by >50%, although it depends on the set of input genomes. A set of input genomes consisting primarily of new species will not benefit from ANI screen as much as a set of genomes that are largely assigned to GTDB species clusters. In the latter case, the ANI screen will reduce the number of genomes that need to be classified by pplacer which reduces computation time substantially (between 25% and 60% in our testing).
 
 ## 📚 References
 
@@ -82,14 +86,15 @@
 * Parks DH, et al. 2018. [A standardized bacterial taxonomy based on genome phylogeny substantially revises the tree of life](https://www.nature.com/articles/nbt.4229). <i>Nature Biotechnology</i>, http://dx.doi.org/10.1038/nbt.4229.
  
 
 We strongly encourage you to cite the following 3rd party dependencies:
 
 * Matsen FA, et al. 2010. [pplacer: linear time maximum-likelihood and Bayesian phylogenetic placement of sequences onto a fixed reference tree](https://www.ncbi.nlm.nih.gov/pubmed/21034504). <i>BMC Bioinformatics</i>, 11:538.
 * Jain C, et al. 2019. [High-throughput ANI Analysis of 90K Prokaryotic Genomes Reveals Clear Species Boundaries](https://www.nature.com/articles/s41467-018-07641-9). <i>Nat. Communications</i>, doi: 10.1038/s41467-018-07641-9.
+* Shaw J. and Yu Y.W. 2023. [Fast and robust metagenomic sequence comparison through sparse chaining with skani](https://www.nature.com/articles/s41592-023-02018-3). <i>Nature Methods</i>, 20, pages1661–1665 (2023).
 * Hyatt D, et al. 2010. [Prodigal: prokaryotic gene recognition and translation initiation site identification](https://www.ncbi.nlm.nih.gov/pubmed/20211023). <i>BMC Bioinformatics</i>, 11:119. doi: 10.1186/1471-2105-11-119.
 * Price MN, et al. 2010. [FastTree 2 - Approximately Maximum-Likelihood Trees for Large Alignments](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2835736/). <i>PLoS One</i>, 5, e9490.
 * Eddy SR. 2011. [Accelerated profile HMM searches](https://www.ncbi.nlm.nih.gov/pubmed/22039361). <i>PLOS Comp. Biol.</i>, 7:e1002195.
 * Ondov BD, et al. 2016. [Mash: fast genome and metagenome distance estimation using MinHash](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-016-0997-x). <i>Genome Biol</i> 17, 132. doi: 10.1186/s13059-016-0997-x.
 
 
 ## © Copyright
```

### Comparing `gtdbtk-2.3.2/gtdbtk.egg-info/SOURCES.txt` & `gtdbtk-2.4.0/gtdbtk.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 gtdbtk/external/fastani.py
 gtdbtk/external/fasttree.py
 gtdbtk/external/hmm_aligner.py
 gtdbtk/external/mash.py
 gtdbtk/external/pfam_search.py
 gtdbtk/external/pplacer.py
 gtdbtk/external/prodigal.py
+gtdbtk/external/skani.py
 gtdbtk/external/tigrfam_search.py
 gtdbtk/external/pypfam/__init__.py
 gtdbtk/external/pypfam/HMM/HMMMatch.py
 gtdbtk/external/pypfam/HMM/HMMResults.py
 gtdbtk/external/pypfam/HMM/HMMResultsIO.py
 gtdbtk/external/pypfam/HMM/HMMSequence.py
 gtdbtk/external/pypfam/HMM/HMMUnit.py
@@ -94,13 +95,14 @@
 tests/test_gtdbtk/test_biolib_lite/test_common.py
 tests/test_gtdbtk/test_biolib_lite/test_newick.py
 tests/test_gtdbtk/test_biolib_lite/test_seq_io.py
 tests/test_gtdbtk/test_biolib_lite/test_taxonomy.py
 tests/test_gtdbtk/test_external/__init__.py
 tests/test_gtdbtk/test_external/test_fastani.py
 tests/test_gtdbtk/test_external/test_fasttree.py
+tests/test_gtdbtk/test_external/test_skani.py
 tests/test_gtdbtk/test_files/__init__.py
 tests/test_gtdbtk/test_files/test_marker/__init__.py
 tests/test_gtdbtk/test_files/test_marker/test_copy_number.py
 tests/test_gtdbtk/test_files/test_marker/test_tophit.py
 tests/test_gtdbtk/test_files/test_prodigal/__init__.py
 tests/test_gtdbtk/test_files/test_prodigal/test_tln_table_summary.py
```

### Comparing `gtdbtk-2.3.2/setup.py` & `gtdbtk-2.4.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     data_files=[("", ["LICENSE"])],
     description=meta['description'],
     entry_points={
         'console_scripts': [
             'gtdbtk = gtdbtk.__main__:main'
         ]
     },
-    install_requires=["dendropy>=4.1.0", 'numpy>=1.9.0', 'tqdm>=4.35.0', 'pydantic>=1.9.2,<2.0a1'],
+    install_requires=["dendropy ~= 4.1", 'numpy ~= 1.9', 'tqdm ~= 4.35', 'pydantic ~= 1.9'],
     license=meta['license'],
     long_description=readme(),
     long_description_content_type='text/markdown',
     maintainer=meta['maintainer'],
     maintainer_email=meta['maintainer_email'],
     name=meta['name'],
     packages=find_packages(),
```

### Comparing `gtdbtk-2.3.2/tests/common.py` & `gtdbtk-2.4.0/tests/common.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/tests/test_classify.py` & `gtdbtk-2.4.0/tests/test_classify.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/tests/test_cli.py` & `gtdbtk-2.4.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/tests/test_gtdbtk/test__main__.py` & `gtdbtk-2.4.0/tests/test_gtdbtk/test__main__.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/tests/test_gtdbtk/test_biolib_lite/test_common.py` & `gtdbtk-2.4.0/tests/test_gtdbtk/test_biolib_lite/test_common.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/tests/test_gtdbtk/test_biolib_lite/test_newick.py` & `gtdbtk-2.4.0/tests/test_gtdbtk/test_biolib_lite/test_newick.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/tests/test_gtdbtk/test_biolib_lite/test_seq_io.py` & `gtdbtk-2.4.0/tests/test_gtdbtk/test_biolib_lite/test_seq_io.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/tests/test_gtdbtk/test_biolib_lite/test_taxonomy.py` & `gtdbtk-2.4.0/tests/test_gtdbtk/test_biolib_lite/test_taxonomy.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/tests/test_gtdbtk/test_external/test_fastani.py` & `gtdbtk-2.4.0/tests/test_gtdbtk/test_external/test_fastani.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/tests/test_gtdbtk/test_external/test_fasttree.py` & `gtdbtk-2.4.0/tests/test_gtdbtk/test_external/test_fasttree.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 
 class TestFastTree(unittest.TestCase):
 
     def setUp(self):
         self.dir_tmp = tempfile.mkdtemp(prefix='gtdbtk_tmp_')
         self.cpus = 1
-        self.genome_root = CONFIG.FASTANI_GENOMES
+        self.genome_root = CONFIG.SKANI_GENOMES
         self.test_msa = 'tests/data/example.faa'
         self.test_msa_gz = 'tests/data/example.faa.gz'
 
     def tearDown(self):
         shutil.rmtree(self.dir_tmp)
 
     def test_run(self):
```

### Comparing `gtdbtk-2.3.2/tests/test_gtdbtk/test_files/test_marker/test_copy_number.py` & `gtdbtk-2.4.0/tests/test_gtdbtk/test_files/test_marker/test_copy_number.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/tests/test_gtdbtk/test_files/test_marker/test_tophit.py` & `gtdbtk-2.4.0/tests/test_gtdbtk/test_files/test_marker/test_tophit.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/tests/test_gtdbtk/test_files/test_prodigal/test_tln_table_summary.py` & `gtdbtk-2.4.0/tests/test_gtdbtk/test_files/test_prodigal/test_tln_table_summary.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/tests/test_gtdbtk/test_main.py` & `gtdbtk-2.4.0/tests/test_gtdbtk/test_main.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/tests/test_gtdbtk/test_markers.py` & `gtdbtk-2.4.0/tests/test_gtdbtk/test_markers.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/tests/test_gtdbtk/test_tools.py` & `gtdbtk-2.4.0/tests/test_gtdbtk/test_tools.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.2/tests/test_gtdbtk/test_trim_msa.py` & `gtdbtk-2.4.0/tests/test_gtdbtk/test_trim_msa.py`

 * *Files identical despite different names*

