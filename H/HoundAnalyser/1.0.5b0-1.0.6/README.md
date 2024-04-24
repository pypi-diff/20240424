# Comparing `tmp/HoundAnalyser-1.0.5b0.tar.gz` & `tmp/houndanalyser-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HoundAnalyser-1.0.5b0.tar", last modified: Thu Mar 28 13:29:11 2024, max compression
+gzip compressed data, was "houndanalyser-1.0.6.tar", last modified: Wed Apr 24 20:24:05 2024, max compression
```

## Comparing `HoundAnalyser-1.0.5b0.tar` & `houndanalyser-1.0.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 carlos    (1000) carlos    (1000)        0 2024-03-28 13:29:11.515301 HoundAnalyser-1.0.5b0/
-drwxr-xr-x   0 carlos    (1000) carlos    (1000)        0 2024-03-28 13:29:11.509301 HoundAnalyser-1.0.5b0/HoundAnalyser/
--rw-r--r--   0 carlos    (1000) carlos    (1000)      762 2024-03-15 09:10:28.000000 HoundAnalyser-1.0.5b0/HoundAnalyser/__init__.py
--rwxr-xr-x   0 carlos    (1000) carlos    (1000)     6757 2024-03-19 12:50:04.000000 HoundAnalyser-1.0.5b0/HoundAnalyser/__main__.py
--rw-r--r--   0 carlos    (1000) carlos    (1000)       23 2024-03-28 13:27:57.000000 HoundAnalyser-1.0.5b0/HoundAnalyser/__version__.py
-drwxr-xr-x   0 carlos    (1000) carlos    (1000)        0 2024-03-28 13:29:11.511301 HoundAnalyser-1.0.5b0/HoundAnalyser/data_hoover/
--rw-r--r--   0 carlos    (1000) carlos    (1000)       86 2023-06-22 20:26:53.000000 HoundAnalyser-1.0.5b0/HoundAnalyser/data_hoover/__init__.py
--rw-r--r--   0 carlos    (1000) carlos    (1000)     3169 2023-12-01 14:22:35.000000 HoundAnalyser-1.0.5b0/HoundAnalyser/data_hoover/_mutant_classifier.py
--rw-r--r--   0 carlos    (1000) carlos    (1000)     2204 2024-03-20 11:15:18.000000 HoundAnalyser-1.0.5b0/HoundAnalyser/data_hoover/asmbl_finder.py
--rw-r--r--   0 carlos    (1000) carlos    (1000)     2574 2023-12-01 14:23:49.000000 HoundAnalyser-1.0.5b0/HoundAnalyser/data_hoover/coverage_analyser.py
--rw-r--r--   0 carlos    (1000) carlos    (1000)     3108 2024-03-20 11:30:37.000000 HoundAnalyser-1.0.5b0/HoundAnalyser/data_hoover/locus_finder.py
--rw-r--r--   0 carlos    (1000) carlos    (1000)    13751 2024-03-21 13:42:21.000000 HoundAnalyser-1.0.5b0/HoundAnalyser/data_hoover/main.py
--rw-r--r--   0 carlos    (1000) carlos    (1000)    28266 2024-02-06 11:46:35.000000 HoundAnalyser-1.0.5b0/HoundAnalyser/data_hoover/mutant_finder.py
-drwxr-xr-x   0 carlos    (1000) carlos    (1000)        0 2024-03-28 13:29:11.512301 HoundAnalyser-1.0.5b0/HoundAnalyser/external/
--rw-r--r--   0 carlos    (1000) carlos    (1000)        0 2023-02-02 12:28:33.000000 HoundAnalyser-1.0.5b0/HoundAnalyser/external/__init__.py
--rw-r--r--   0 carlos    (1000) carlos    (1000)     6597 2023-12-04 11:20:42.000000 HoundAnalyser-1.0.5b0/HoundAnalyser/external/plot_eteTree.py
-drwxr-xr-x   0 carlos    (1000) carlos    (1000)        0 2024-03-28 13:29:11.512301 HoundAnalyser-1.0.5b0/HoundAnalyser/genoplot/
--rw-r--r--   0 carlos    (1000) carlos    (1000)        0 2023-03-14 08:55:46.000000 HoundAnalyser-1.0.5b0/HoundAnalyser/genoplot/__init__.py
--rw-r--r--   0 carlos    (1000) carlos    (1000)    13601 2023-12-05 16:58:44.000000 HoundAnalyser-1.0.5b0/HoundAnalyser/genoplot/plot_align.py
--rwxr-xr-x   0 carlos    (1000) carlos    (1000)    14408 2024-03-21 13:40:50.000000 HoundAnalyser-1.0.5b0/HoundAnalyser/goFetch.py
-drwxr-xr-x   0 carlos    (1000) carlos    (1000)        0 2024-03-28 13:29:11.514301 HoundAnalyser-1.0.5b0/HoundAnalyser/helper_func/
--rw-r--r--   0 carlos    (1000) carlos    (1000)    18851 2024-03-20 10:30:17.000000 HoundAnalyser-1.0.5b0/HoundAnalyser/helper_func/__init__.py
--rw-r--r--   0 carlos    (1000) carlos    (1000)    13946 2024-03-20 19:06:20.000000 HoundAnalyser-1.0.5b0/HoundAnalyser/helper_func/alignment_tools.py
--rw-r--r--   0 carlos    (1000) carlos    (1000)    11699 2024-03-18 12:24:51.000000 HoundAnalyser-1.0.5b0/HoundAnalyser/helper_func/assembly_utilities.py
--rw-r--r--   0 carlos    (1000) carlos    (1000)    17482 2024-02-28 14:12:00.000000 HoundAnalyser-1.0.5b0/HoundAnalyser/helper_func/contig_merger.py
--rw-r--r--   0 carlos    (1000) carlos    (1000)      877 2024-03-19 14:05:48.000000 HoundAnalyser-1.0.5b0/HoundAnalyser/helper_func/data_organiser.py
--rw-r--r--   0 carlos    (1000) carlos    (1000)    21878 2024-01-22 16:21:12.000000 HoundAnalyser-1.0.5b0/HoundAnalyser/helper_func/ncbi.py
--rw-r--r--   0 carlos    (1000) carlos    (1000)    11214 2024-01-22 16:21:12.000000 HoundAnalyser-1.0.5b0/HoundAnalyser/helper_func/promoter_tools.py
--rw-r--r--   0 carlos    (1000) carlos    (1000)      775 2024-03-16 09:01:28.000000 HoundAnalyser-1.0.5b0/HoundAnalyser/helper_func/rtrv_reads.py
--rw-r--r--   0 carlos    (1000) carlos    (1000)     4152 2024-01-19 13:04:29.000000 HoundAnalyser-1.0.5b0/HoundAnalyser/helper_func/sundry.py
--rw-r--r--   0 carlos    (1000) carlos    (1000)     2879 2023-12-04 11:02:37.000000 HoundAnalyser-1.0.5b0/HoundAnalyser/helper_func/unalignment_tools.py
-drwxr-xr-x   0 carlos    (1000) carlos    (1000)        0 2024-03-28 13:29:11.514301 HoundAnalyser-1.0.5b0/HoundAnalyser.egg-info/
--rw-r--r--   0 carlos    (1000) carlos    (1000)     1013 2024-03-28 13:29:11.000000 HoundAnalyser-1.0.5b0/HoundAnalyser.egg-info/PKG-INFO
--rw-r--r--   0 carlos    (1000) carlos    (1000)     1216 2024-03-28 13:29:11.000000 HoundAnalyser-1.0.5b0/HoundAnalyser.egg-info/SOURCES.txt
--rw-r--r--   0 carlos    (1000) carlos    (1000)        1 2024-03-28 13:29:11.000000 HoundAnalyser-1.0.5b0/HoundAnalyser.egg-info/dependency_links.txt
--rw-r--r--   0 carlos    (1000) carlos    (1000)       62 2024-03-28 13:29:11.000000 HoundAnalyser-1.0.5b0/HoundAnalyser.egg-info/entry_points.txt
--rw-r--r--   0 carlos    (1000) carlos    (1000)       82 2024-03-28 13:29:11.000000 HoundAnalyser-1.0.5b0/HoundAnalyser.egg-info/requires.txt
--rw-r--r--   0 carlos    (1000) carlos    (1000)       14 2024-03-28 13:29:11.000000 HoundAnalyser-1.0.5b0/HoundAnalyser.egg-info/top_level.txt
--rw-r--r--   0 carlos    (1000) carlos    (1000)    26530 2023-05-27 20:25:39.000000 HoundAnalyser-1.0.5b0/LICENSE
--rw-r--r--   0 carlos    (1000) carlos    (1000)     1013 2024-03-28 13:29:11.514301 HoundAnalyser-1.0.5b0/PKG-INFO
--rw-r--r--   0 carlos    (1000) carlos    (1000)     8862 2024-03-25 15:12:42.000000 HoundAnalyser-1.0.5b0/README.rst
--rw-r--r--   0 carlos    (1000) carlos    (1000)       38 2024-03-28 13:29:11.515301 HoundAnalyser-1.0.5b0/setup.cfg
--rw-r--r--   0 carlos    (1000) carlos    (1000)     2008 2024-03-25 15:27:44.000000 HoundAnalyser-1.0.5b0/setup.py
+drwxr-xr-x   0 carlos    (1000) carlos    (1000)        0 2024-04-24 20:24:05.270673 houndanalyser-1.0.6/
+drwxr-xr-x   0 carlos    (1000) carlos    (1000)        0 2024-04-24 20:24:05.265673 houndanalyser-1.0.6/HoundAnalyser/
+-rw-r--r--   0 carlos    (1000) carlos    (1000)      762 2024-03-15 09:10:28.000000 houndanalyser-1.0.6/HoundAnalyser/__init__.py
+-rwxr-xr-x   0 carlos    (1000) carlos    (1000)     6757 2024-03-19 12:50:04.000000 houndanalyser-1.0.6/HoundAnalyser/__main__.py
+-rw-r--r--   0 carlos    (1000) carlos    (1000)       22 2024-04-24 11:21:14.000000 houndanalyser-1.0.6/HoundAnalyser/__version__.py
+drwxr-xr-x   0 carlos    (1000) carlos    (1000)        0 2024-04-24 20:24:05.267673 houndanalyser-1.0.6/HoundAnalyser/data_hoover/
+-rw-r--r--   0 carlos    (1000) carlos    (1000)       86 2023-06-22 20:26:53.000000 houndanalyser-1.0.6/HoundAnalyser/data_hoover/__init__.py
+-rw-r--r--   0 carlos    (1000) carlos    (1000)     3169 2023-12-01 14:22:35.000000 houndanalyser-1.0.6/HoundAnalyser/data_hoover/_mutant_classifier.py
+-rw-r--r--   0 carlos    (1000) carlos    (1000)     2204 2024-03-20 11:15:18.000000 houndanalyser-1.0.6/HoundAnalyser/data_hoover/asmbl_finder.py
+-rw-r--r--   0 carlos    (1000) carlos    (1000)     2574 2023-12-01 14:23:49.000000 houndanalyser-1.0.6/HoundAnalyser/data_hoover/coverage_analyser.py
+-rw-r--r--   0 carlos    (1000) carlos    (1000)     3108 2024-03-20 11:30:37.000000 houndanalyser-1.0.6/HoundAnalyser/data_hoover/locus_finder.py
+-rw-r--r--   0 carlos    (1000) carlos    (1000)    13751 2024-03-21 13:42:21.000000 houndanalyser-1.0.6/HoundAnalyser/data_hoover/main.py
+-rw-r--r--   0 carlos    (1000) carlos    (1000)    28700 2024-04-24 20:03:44.000000 houndanalyser-1.0.6/HoundAnalyser/data_hoover/mutant_finder.py
+drwxr-xr-x   0 carlos    (1000) carlos    (1000)        0 2024-04-24 20:24:05.267673 houndanalyser-1.0.6/HoundAnalyser/external/
+-rw-r--r--   0 carlos    (1000) carlos    (1000)        0 2023-02-02 12:28:33.000000 houndanalyser-1.0.6/HoundAnalyser/external/__init__.py
+-rw-r--r--   0 carlos    (1000) carlos    (1000)     6597 2023-12-04 11:20:42.000000 houndanalyser-1.0.6/HoundAnalyser/external/plot_eteTree.py
+drwxr-xr-x   0 carlos    (1000) carlos    (1000)        0 2024-04-24 20:24:05.267673 houndanalyser-1.0.6/HoundAnalyser/genoplot/
+-rw-r--r--   0 carlos    (1000) carlos    (1000)        0 2023-03-14 08:55:46.000000 houndanalyser-1.0.6/HoundAnalyser/genoplot/__init__.py
+-rw-r--r--   0 carlos    (1000) carlos    (1000)    13601 2023-12-05 16:58:44.000000 houndanalyser-1.0.6/HoundAnalyser/genoplot/plot_align.py
+-rwxr-xr-x   0 carlos    (1000) carlos    (1000)    14408 2024-03-21 13:40:50.000000 houndanalyser-1.0.6/HoundAnalyser/goFetch.py
+drwxr-xr-x   0 carlos    (1000) carlos    (1000)        0 2024-04-24 20:24:05.269673 houndanalyser-1.0.6/HoundAnalyser/helper_func/
+-rw-r--r--   0 carlos    (1000) carlos    (1000)    18851 2024-03-20 10:30:17.000000 houndanalyser-1.0.6/HoundAnalyser/helper_func/__init__.py
+-rw-r--r--   0 carlos    (1000) carlos    (1000)    13946 2024-03-20 19:06:20.000000 houndanalyser-1.0.6/HoundAnalyser/helper_func/alignment_tools.py
+-rw-r--r--   0 carlos    (1000) carlos    (1000)    11699 2024-03-18 12:24:51.000000 houndanalyser-1.0.6/HoundAnalyser/helper_func/assembly_utilities.py
+-rw-r--r--   0 carlos    (1000) carlos    (1000)    17482 2024-02-28 14:12:00.000000 houndanalyser-1.0.6/HoundAnalyser/helper_func/contig_merger.py
+-rw-r--r--   0 carlos    (1000) carlos    (1000)      877 2024-03-19 14:05:48.000000 houndanalyser-1.0.6/HoundAnalyser/helper_func/data_organiser.py
+-rw-r--r--   0 carlos    (1000) carlos    (1000)    21878 2024-01-22 16:21:12.000000 houndanalyser-1.0.6/HoundAnalyser/helper_func/ncbi.py
+-rw-r--r--   0 carlos    (1000) carlos    (1000)    11214 2024-01-22 16:21:12.000000 houndanalyser-1.0.6/HoundAnalyser/helper_func/promoter_tools.py
+-rw-r--r--   0 carlos    (1000) carlos    (1000)      775 2024-03-16 09:01:28.000000 houndanalyser-1.0.6/HoundAnalyser/helper_func/rtrv_reads.py
+-rw-r--r--   0 carlos    (1000) carlos    (1000)     4152 2024-01-19 13:04:29.000000 houndanalyser-1.0.6/HoundAnalyser/helper_func/sundry.py
+-rw-r--r--   0 carlos    (1000) carlos    (1000)     2879 2023-12-04 11:02:37.000000 houndanalyser-1.0.6/HoundAnalyser/helper_func/unalignment_tools.py
+drwxr-xr-x   0 carlos    (1000) carlos    (1000)        0 2024-04-24 20:24:05.269673 houndanalyser-1.0.6/HoundAnalyser.egg-info/
+-rw-r--r--   0 carlos    (1000) carlos    (1000)     1011 2024-04-24 20:24:05.000000 houndanalyser-1.0.6/HoundAnalyser.egg-info/PKG-INFO
+-rw-r--r--   0 carlos    (1000) carlos    (1000)     1216 2024-04-24 20:24:05.000000 houndanalyser-1.0.6/HoundAnalyser.egg-info/SOURCES.txt
+-rw-r--r--   0 carlos    (1000) carlos    (1000)        1 2024-04-24 20:24:05.000000 houndanalyser-1.0.6/HoundAnalyser.egg-info/dependency_links.txt
+-rw-r--r--   0 carlos    (1000) carlos    (1000)       62 2024-04-24 20:24:05.000000 houndanalyser-1.0.6/HoundAnalyser.egg-info/entry_points.txt
+-rw-r--r--   0 carlos    (1000) carlos    (1000)       82 2024-04-24 20:24:05.000000 houndanalyser-1.0.6/HoundAnalyser.egg-info/requires.txt
+-rw-r--r--   0 carlos    (1000) carlos    (1000)       14 2024-04-24 20:24:05.000000 houndanalyser-1.0.6/HoundAnalyser.egg-info/top_level.txt
+-rw-r--r--   0 carlos    (1000) carlos    (1000)    26530 2023-05-27 20:25:39.000000 houndanalyser-1.0.6/LICENSE
+-rw-r--r--   0 carlos    (1000) carlos    (1000)     1011 2024-04-24 20:24:05.269673 houndanalyser-1.0.6/PKG-INFO
+-rw-r--r--   0 carlos    (1000) carlos    (1000)     8862 2024-03-25 15:12:42.000000 houndanalyser-1.0.6/README.rst
+-rw-r--r--   0 carlos    (1000) carlos    (1000)       38 2024-04-24 20:24:05.270673 houndanalyser-1.0.6/setup.cfg
+-rw-r--r--   0 carlos    (1000) carlos    (1000)     2008 2024-03-25 15:27:44.000000 houndanalyser-1.0.6/setup.py
```

### Comparing `HoundAnalyser-1.0.5b0/HoundAnalyser/__init__.py` & `houndanalyser-1.0.6/HoundAnalyser/__init__.py`

 * *Files identical despite different names*

### Comparing `HoundAnalyser-1.0.5b0/HoundAnalyser/__main__.py` & `houndanalyser-1.0.6/HoundAnalyser/__main__.py`

 * *Files identical despite different names*

### Comparing `HoundAnalyser-1.0.5b0/HoundAnalyser/data_hoover/_mutant_classifier.py` & `houndanalyser-1.0.6/HoundAnalyser/data_hoover/_mutant_classifier.py`

 * *Files identical despite different names*

### Comparing `HoundAnalyser-1.0.5b0/HoundAnalyser/data_hoover/asmbl_finder.py` & `houndanalyser-1.0.6/HoundAnalyser/data_hoover/asmbl_finder.py`

 * *Files identical despite different names*

### Comparing `HoundAnalyser-1.0.5b0/HoundAnalyser/data_hoover/coverage_analyser.py` & `houndanalyser-1.0.6/HoundAnalyser/data_hoover/coverage_analyser.py`

 * *Files identical despite different names*

### Comparing `HoundAnalyser-1.0.5b0/HoundAnalyser/data_hoover/locus_finder.py` & `houndanalyser-1.0.6/HoundAnalyser/data_hoover/locus_finder.py`

 * *Files identical despite different names*

### Comparing `HoundAnalyser-1.0.5b0/HoundAnalyser/data_hoover/main.py` & `houndanalyser-1.0.6/HoundAnalyser/data_hoover/main.py`

 * *Files identical despite different names*

### Comparing `HoundAnalyser-1.0.5b0/HoundAnalyser/data_hoover/mutant_finder.py` & `houndanalyser-1.0.6/HoundAnalyser/data_hoover/mutant_finder.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,38 +147,38 @@
     """
         Screen through REFERENCE_FILE list to find which specific
         sequence needs to be used as reference sequence.
     """
     if len(REFERENCE_FILE) == 1:
         return REFERENCE_FILE[0].seq, REFERENCE_FILE[0].description
     else:
-        REFERENCE_SEQ = [s for s in REFERENCE_FILE if s.description in SEQ.description]
+        REFERENCE_SEQ = [s for s in REFERENCE_FILE if s.name in SEQ.description]
         if len(REFERENCE_SEQ) == 0:
             return None, None
         else:
             return REFERENCE_SEQ[0].seq, REFERENCE_SEQ[0].description
 
 
 def _identify_gene_organism(REFERENCE_DESC: str, REFERENCE_FNAME: str = None) -> str:
     """
         Retrieve species from reference sequence, if it exists. Otherwise,
         return the accession code used.
     """
     if REFERENCE_DESC.count(' [') > 0:  # Species included in query
         ORGANISM = REFERENCE_DESC.split('[')[-1].split(']')[0]
-        GENE_NAME = False  # GENE_NAME taken from PREFIX
+        GENE_NAME = REFERENCE_DESC.split(' ')[-2]
     elif REFERENCE_DESC.count('_') > 1 and REFERENCE_DESC.count(':') <= 1:
         # Formatted as ResFinderDB
         ACCESSION_NUMBER = REFERENCE_DESC.split('_')[-1]
         ORGANISM = str('Database used: ACCESSION ') + ACCESSION_NUMBER
         if REFERENCE_DESC.split('_')[1].isdigit():
             LOCUS_N = REFERENCE_DESC.split('_')[1]
         else:
             LOCUS_N = REFERENCE_DESC.split('_')[2]
-        if int(LOCUS_N) > 1:
+        if LOCUS_N.isnumeric() and int(LOCUS_N) > 1:
             GENE_NAME = str('_').join(REFERENCE_DESC.split('_')[:2])
         else:
             GENE_NAME = REFERENCE_DESC.split('_')[0]
     elif REFERENCE_DESC.count(':') >= 2:
         # Formatted as VirulenceFinderDB
         ACCESSION_NUMBER = REFERENCE_DESC.split(':')[-1]
         ORGANISM = str('Database used: ACCESSION ') + ACCESSION_NUMBER
@@ -190,14 +190,24 @@
         msg = str("(Hound *GROWLED*) Looks like the header in query file is \
                   from a translated nucleotide sequence and it is incomplete. \
                   Guessing metadata...")
         print(tw.fill(msg))
         # These headers don't typically contain gene name, use fname instead
         GENE_NAME = REFERENCE_FNAME.split('/')[-1].split('.')[0]
         ORGANISM = str(' ').join(REFERENCE_DESC.split(' ')[1:])
+    else:
+        msg = str("(Hound *GROWLED*) Looks like this entry was made by hand. \
+                  Guessing metadata...")
+        print(tw.fill(msg))
+        if len(REFERENCE_DESC.split(' ')) > 1:
+            GENE_NAME = REFERENCE_DESC.split(' ')[-2]
+            ORGANISM = REFERENCE_DESC.split(' ')[-1]
+        else:
+            GENE_NAME = REFERENCE_DESC
+            ORGANISM = str("Unknown (entry made by hand)")
     return GENE_NAME, ORGANISM
 
 
 def screen_mut_data(FILE: str, REF_FILE: str, PROMOTER_FILE: str = None) -> dict:
     """
         Compare each entry of the alignment in FILE to reference in REF_FILE,
         after removing gaps, to find mutations.
```

### Comparing `HoundAnalyser-1.0.5b0/HoundAnalyser/external/plot_eteTree.py` & `houndanalyser-1.0.6/HoundAnalyser/external/plot_eteTree.py`

 * *Files identical despite different names*

### Comparing `HoundAnalyser-1.0.5b0/HoundAnalyser/genoplot/plot_align.py` & `houndanalyser-1.0.6/HoundAnalyser/genoplot/plot_align.py`

 * *Files identical despite different names*

### Comparing `HoundAnalyser-1.0.5b0/HoundAnalyser/goFetch.py` & `houndanalyser-1.0.6/HoundAnalyser/goFetch.py`

 * *Files identical despite different names*

### Comparing `HoundAnalyser-1.0.5b0/HoundAnalyser/helper_func/__init__.py` & `houndanalyser-1.0.6/HoundAnalyser/helper_func/__init__.py`

 * *Files identical despite different names*

### Comparing `HoundAnalyser-1.0.5b0/HoundAnalyser/helper_func/alignment_tools.py` & `houndanalyser-1.0.6/HoundAnalyser/helper_func/alignment_tools.py`

 * *Files identical despite different names*

### Comparing `HoundAnalyser-1.0.5b0/HoundAnalyser/helper_func/assembly_utilities.py` & `houndanalyser-1.0.6/HoundAnalyser/helper_func/assembly_utilities.py`

 * *Files identical despite different names*

### Comparing `HoundAnalyser-1.0.5b0/HoundAnalyser/helper_func/contig_merger.py` & `houndanalyser-1.0.6/HoundAnalyser/helper_func/contig_merger.py`

 * *Files identical despite different names*

### Comparing `HoundAnalyser-1.0.5b0/HoundAnalyser/helper_func/data_organiser.py` & `houndanalyser-1.0.6/HoundAnalyser/helper_func/data_organiser.py`

 * *Files identical despite different names*

### Comparing `HoundAnalyser-1.0.5b0/HoundAnalyser/helper_func/ncbi.py` & `houndanalyser-1.0.6/HoundAnalyser/helper_func/ncbi.py`

 * *Files identical despite different names*

### Comparing `HoundAnalyser-1.0.5b0/HoundAnalyser/helper_func/promoter_tools.py` & `houndanalyser-1.0.6/HoundAnalyser/helper_func/promoter_tools.py`

 * *Files identical despite different names*

### Comparing `HoundAnalyser-1.0.5b0/HoundAnalyser/helper_func/rtrv_reads.py` & `houndanalyser-1.0.6/HoundAnalyser/helper_func/rtrv_reads.py`

 * *Files identical despite different names*

### Comparing `HoundAnalyser-1.0.5b0/HoundAnalyser/helper_func/sundry.py` & `houndanalyser-1.0.6/HoundAnalyser/helper_func/sundry.py`

 * *Files identical despite different names*

### Comparing `HoundAnalyser-1.0.5b0/HoundAnalyser/helper_func/unalignment_tools.py` & `houndanalyser-1.0.6/HoundAnalyser/helper_func/unalignment_tools.py`

 * *Files identical despite different names*

### Comparing `HoundAnalyser-1.0.5b0/HoundAnalyser.egg-info/PKG-INFO` & `houndanalyser-1.0.6/HoundAnalyser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HoundAnalyser
-Version: 1.0.5b0
+Version: 1.0.6
 Summary: HOUND
 Author: Carlos Reding
 Author-email: carlos.reding@bristol.ac.uk
 Project-URL: Source, https://gitlab.com/rc-reding/software/-/tree/main/Hound?ref_type=heads
 Project-URL: Homepage, https://gitlab.com/rc-reding/software/-/tree/main/Hound?ref_type=heads
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `HoundAnalyser-1.0.5b0/HoundAnalyser.egg-info/SOURCES.txt` & `houndanalyser-1.0.6/HoundAnalyser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HoundAnalyser-1.0.5b0/LICENSE` & `houndanalyser-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `HoundAnalyser-1.0.5b0/PKG-INFO` & `houndanalyser-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HoundAnalyser
-Version: 1.0.5b0
+Version: 1.0.6
 Summary: HOUND
 Author: Carlos Reding
 Author-email: carlos.reding@bristol.ac.uk
 Project-URL: Source, https://gitlab.com/rc-reding/software/-/tree/main/Hound?ref_type=heads
 Project-URL: Homepage, https://gitlab.com/rc-reding/software/-/tree/main/Hound?ref_type=heads
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `HoundAnalyser-1.0.5b0/README.rst` & `houndanalyser-1.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `HoundAnalyser-1.0.5b0/setup.py` & `houndanalyser-1.0.6/setup.py`

 * *Files identical despite different names*

