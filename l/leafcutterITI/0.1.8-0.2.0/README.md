# Comparing `tmp/leafcutterITI-0.1.8.tar.gz` & `tmp/leafcutteriti-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leafcutterITI-0.1.8.tar", last modified: Tue Mar  5 03:35:55 2024, max compression
+gzip compressed data, was "leafcutteriti-0.2.0.tar", last modified: Wed Apr 24 03:22:15 2024, max compression
```

## Comparing `leafcutterITI-0.1.8.tar` & `leafcutteriti-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-03-05 03:35:55.410625 leafcutterITI-0.1.8/
--rw-rw-rw-   0        0        0    11558 2024-03-05 00:29:30.000000 leafcutterITI-0.1.8/LICENSE
--rw-rw-rw-   0        0        0    21626 2024-03-05 03:35:55.409625 leafcutterITI-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     8086 2024-03-05 00:29:30.000000 leafcutterITI-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2024-03-05 03:35:55.392624 leafcutterITI-0.1.8/leafcutterITI/
--rw-rw-rw-   0        0        0        0 2024-03-05 01:01:00.000000 leafcutterITI-0.1.8/leafcutterITI/__init__.py
--rw-rw-rw-   0        0        0      401 2024-03-05 03:13:14.000000 leafcutterITI-0.1.8/leafcutterITI/__main__.py
-drwxrwxrwx   0        0        0        0 2024-03-05 03:35:55.402624 leafcutterITI-0.1.8/leafcutterITI/clustering/
--rw-rw-rw-   0        0        0        0 2024-03-05 01:01:00.000000 leafcutterITI-0.1.8/leafcutterITI/clustering/__init__.py
--rw-rw-rw-   0        0        0    30749 2024-03-05 03:34:44.000000 leafcutterITI-0.1.8/leafcutterITI/clustering/leafcutterITI_clustering.py
--rw-rw-rw-   0        0        0     1386 2024-02-28 04:01:27.000000 leafcutterITI-0.1.8/leafcutterITI/clustering/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-05 03:35:55.408623 leafcutterITI-0.1.8/leafcutterITI/map_gen/
--rw-rw-rw-   0        0        0        0 2024-03-05 01:01:00.000000 leafcutterITI-0.1.8/leafcutterITI/map_gen/__init__.py
--rw-rw-rw-   0        0        0    20439 2024-03-05 03:34:52.000000 leafcutterITI-0.1.8/leafcutterITI/map_gen/leafcutterITI_map_gen.py
--rw-rw-rw-   0        0        0     1386 2024-02-28 04:01:27.000000 leafcutterITI-0.1.8/leafcutterITI/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-05 03:35:55.408623 leafcutterITI-0.1.8/leafcutterITI.egg-info/
--rw-rw-rw-   0        0        0    21626 2024-03-05 03:35:55.000000 leafcutterITI-0.1.8/leafcutterITI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      545 2024-03-05 03:35:55.000000 leafcutterITI-0.1.8/leafcutterITI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-05 03:35:55.000000 leafcutterITI-0.1.8/leafcutterITI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      155 2024-03-05 03:35:55.000000 leafcutterITI-0.1.8/leafcutterITI.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       22 2024-03-05 03:35:55.000000 leafcutterITI-0.1.8/leafcutterITI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-03-05 03:35:55.000000 leafcutterITI-0.1.8/leafcutterITI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      640 2024-03-05 03:35:17.000000 leafcutterITI-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-05 03:35:55.410625 leafcutterITI-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      542 2024-03-05 03:35:28.000000 leafcutterITI-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:22:15.809575 leafcutteriti-0.2.0/
+-rw-rw-rw-   0        0        0     1084 2024-03-05 04:21:00.000000 leafcutteriti-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0    16875 2024-04-24 03:22:15.808571 leafcutteriti-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    15227 2024-04-24 03:08:45.000000 leafcutteriti-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 03:22:15.788004 leafcutteriti-0.2.0/leafcutterITI/
+-rw-rw-rw-   0        0        0        0 2024-03-05 01:01:00.000000 leafcutteriti-0.2.0/leafcutterITI/__init__.py
+-rw-rw-rw-   0        0        0      551 2024-04-23 15:55:20.000000 leafcutteriti-0.2.0/leafcutterITI/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:22:15.804061 leafcutteriti-0.2.0/leafcutterITI/clustering/
+-rw-rw-rw-   0        0        0        0 2024-03-05 01:01:00.000000 leafcutteriti-0.2.0/leafcutterITI/clustering/__init__.py
+-rw-rw-rw-   0        0        0    31348 2024-04-16 03:36:37.000000 leafcutteriti-0.2.0/leafcutterITI/clustering/leafcutterITI_clustering.py
+-rw-rw-rw-   0        0        0     1386 2024-02-28 04:01:27.000000 leafcutteriti-0.2.0/leafcutterITI/clustering/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:22:15.805060 leafcutteriti-0.2.0/leafcutterITI/map_gen/
+-rw-rw-rw-   0        0        0        0 2024-03-05 01:01:00.000000 leafcutteriti-0.2.0/leafcutterITI/map_gen/__init__.py
+-rw-rw-rw-   0        0        0    24396 2024-04-22 19:06:01.000000 leafcutteriti-0.2.0/leafcutterITI/map_gen/leafcutterITI_map_gen.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:22:15.807062 leafcutteriti-0.2.0/leafcutterITI/scITI/
+-rw-rw-rw-   0        0        0        0 2024-03-05 01:01:00.000000 leafcutteriti-0.2.0/leafcutterITI/scITI/__init__.py
+-rw-rw-rw-   0        0        0     3686 2024-04-24 00:41:55.000000 leafcutteriti-0.2.0/leafcutterITI/scITI/calcutta_functions.py
+-rw-rw-rw-   0        0        0    32530 2024-04-24 01:48:57.000000 leafcutteriti-0.2.0/leafcutterITI/scITI/leafcutterITI_scITI.py
+-rw-rw-rw-   0        0        0    15946 2024-04-23 16:59:24.000000 leafcutteriti-0.2.0/leafcutterITI/shared_functions.py
+-rw-rw-rw-   0        0        0     1386 2024-02-28 04:01:27.000000 leafcutteriti-0.2.0/leafcutterITI/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:22:15.808571 leafcutteriti-0.2.0/leafcutterITI.egg-info/
+-rw-rw-rw-   0        0        0    16875 2024-04-24 03:22:15.000000 leafcutteriti-0.2.0/leafcutterITI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      696 2024-04-24 03:22:15.000000 leafcutteriti-0.2.0/leafcutterITI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 03:22:15.000000 leafcutteriti-0.2.0/leafcutterITI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      220 2024-04-24 03:22:15.000000 leafcutteriti-0.2.0/leafcutterITI.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       28 2024-04-24 03:22:15.000000 leafcutteriti-0.2.0/leafcutterITI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-24 03:22:15.000000 leafcutteriti-0.2.0/leafcutterITI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      719 2024-04-24 03:21:56.000000 leafcutteriti-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-24 03:22:15.809575 leafcutteriti-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      632 2024-04-24 03:21:54.000000 leafcutteriti-0.2.0/setup.py
```

### Comparing `leafcutterITI-0.1.8/leafcutterITI/clustering/leafcutterITI_clustering.py` & `leafcutteriti-0.2.0/leafcutterITI/clustering/leafcutterITI_clustering.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,33 +236,33 @@
     df = pd.read_csv(intron_count_file, sep=' ')
 
     # Sort the DataFrame as required
     df.sort_values(by=['Chr', 'Start', 'End'], inplace=True)
 
     # Initialize variables for tracking clusters
     cluster_num = 1
-    cluster_gene = df.iloc[0]['Gene'] 
+    #cluster_gene = df.iloc[0]['Gene'] 
     cluster_end = df.iloc[0]['End']
     cluster_chr = df.iloc[0]['Chr']
 
     # Function to apply to each row to determine cluster
     def check_new_cluster(row):
         nonlocal cluster_num
         nonlocal cluster_chr
         nonlocal cluster_end
-        nonlocal cluster_gene #used in previous version, plan to removed in further version
+        #nonlocal cluster_gene #used in previous version, plan to removed in further version
         
 
         # Start a new cluster if the gene changes or there's no overlap with the current cluster
         # no need to check for sttart as we sort value based on Start
         if row['Chr'] != cluster_chr or row['Start'] > cluster_end:
             cluster_num += 1
-            cluster_gene = row['Gene']
             cluster_end = row['End']
             cluster_chr = row['Chr']
+            #cluster_gene = row['Gene']
             
         else:
             cluster_end = max(cluster_end, row['End'])
         return f'cluster_{cluster_num}'
 
     # Apply the function to each row in the DataFrame
     # df['Cluster'] = df.apply(check_new_cluster, axis=1)
@@ -270,16 +270,14 @@
 
     # Save the modified DataFrame back to a file
     df.to_csv(intron_count_file, sep=' ', index=False)
 
 
 
 
-
-
 @timing_decorator
 def process_clusters(init_clus_file, exon_count_file, intron_to_exon_file, out_prefix = '', mode = 3,
                      cutoff = 0.1, percent_cutoff = 0.01, min_cluster_val = 1):
     """
     
     Parameters
     ----------
@@ -302,15 +300,21 @@
 
     
     exon_count = pd.read_csv(exon_count_file, sep = ' ', index_col = 0 )
     initial_clus = pd.read_csv(init_clus_file, sep = ' ', index_col = 0)
     intron_to_exon = pd.read_csv(intron_to_exon_file, sep = ' ', index_col = 0)
     
     num_cluters = 0
-    samples = list(initial_clus.columns[5:])
+    if "Gene" in initial_clus.columns.tolist(): # deal with the result from different version
+        samples = initial_clus.columns.tolist()[5:]
+        contained_gene = True
+    else:
+        samples = initial_clus.columns.tolist()[4:]
+        contained_gene = False
+    
     output = open(f'{out_prefix}refined_cluster', 'w')
     
     out_str = ''
     for sample in samples:
         out_str += f'{sample} '
     out_str = out_str[:-1]
     print(out_str, file = output)
@@ -375,18 +379,25 @@
                 
                 for clu_intron in cluster_dic[cluster_num]:
                     
                     infor = initial_clus.loc[clu_intron[3]]
                     strand = str(intron_to_exon.loc[clu_intron[3]]['strand'])
                     
                     out_str += f'{infor.Chr}:{infor.Start}:{infor.End}:clu_{num_cluters}_{strand}'
-                    for value in list(infor)[5:-1]: # start of sample values, and not include the sum columns
-                        out_str += f' {value}'
-                        clu_val += float(value)
                     
+                    if contained_gene == True:
+                        
+                        for value in list(infor)[5:-1]: # start of sample values, and not include the sum columns
+                            out_str += f' {value}'
+                            clu_val += float(value)
+                    else:
+                        for value in list(infor)[4:-1]: # start of sample values, and not include the sum columns
+                            out_str += f' {value}'
+                            clu_val += float(value)
+                            
                     out_str += '\n'
             
                 if clu_val <= min_cluster_val:
                     continue
                 out_str = out_str[:-1] # get rid of the last \n
                 print(out_str, file = output)
                     
@@ -397,14 +408,15 @@
 
 
 
 
 
 
 
+
 
 
 def build_intron(index, row, samples, exon_count,intron_to_exon):
     """
     a helper function for process_clusters function
 
     Parameters
```

### Comparing `leafcutterITI-0.1.8/leafcutterITI/clustering/utils.py` & `leafcutteriti-0.2.0/leafcutterITI/clustering/utils.py`

 * *Files identical despite different names*

### Comparing `leafcutterITI-0.1.8/leafcutterITI/map_gen/leafcutterITI_map_gen.py` & `leafcutteriti-0.2.0/leafcutterITI/map_gen/leafcutterITI_map_gen.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import pyranges as pr
 import numpy as np
 import pandas as pd
 import sys
 import warnings
 import leafcutterITI.utils
 from leafcutterITI.utils import timing_decorator,write_options_to_file
-
+import scipy
+import scipy.sparse
+from scipy.sparse import csr_matrix, save_npz, load_npz
 from optparse import OptionParser
 
 warnings.simplefilter(action='ignore', category=pd.errors.DtypeWarning)
 
 
 
 chr_dic = {'chr1': 0,'chr2': 1,'chr3': 2,'chr4': 3,'chr5': 4,'chr6': 5,'chr7': 6,'chr8': 7,'chr9': 8,'chr10': 9,
@@ -231,14 +233,140 @@
         for exon in near_exon_dic[intron]:
             exons += f'{exon},'
         exons = exons[:-1]
         print(f'{intron} {exons} {intron_str_dic[intron]}',file = output)
     
     output.close()
     
+    
+
+
+
+def isoform_intron_exon_sparse_generation(isoform_intron_map_file, out_prefix = ''):
+    """
+    This function will generate two sparse matrices that map isoform to intron and exon     
+
+    Returns
+    -------
+    None.
+
+    """
+
+
+    df = pd.read_csv(isoform_intron_map_file, sep = ' ')
+
+
+    isoform_to_introns = dict(zip(df['Transcript'], df['support_introns']))
+    isoform_to_exons = dict(zip(df['Transcript'], df['support_exons']))
+
+
+
+    for isoform, introns in isoform_to_introns.items():
+    # Check if introns is not NaN (using pandas isna() function)
+        if pd.isna(introns):
+            isoform_to_introns[isoform] = []
+        else:
+            isoform_to_introns[isoform] = introns.split(',')
+
+
+    for isoform, exons in isoform_to_exons.items():
+    # Check if introns is not NaN (using pandas isna() function)
+        if pd.isna(exons):
+            isoform_to_exons[isoform] = []
+        else:
+            isoform_to_exons[isoform] = exons.split(',')
+
+
+
+    # Step 1: Extract unique isoforms and introns
+    all_isoforms = list(isoform_to_introns.keys())
+    
+    all_introns = set()
+    for introns in isoform_to_introns.values():
+        all_introns.update(introns)
+    all_introns = list(all_introns)    
+    
+    all_exons = set()
+    for exons in isoform_to_exons.values():
+        all_exons.update(exons)
+    all_exons = list(all_exons)
+
+
+
+    # Step 2: Create mappings to indices
+    isoform_to_index = {isoform: i for i, isoform in enumerate(all_isoforms)}
+    intron_to_index = {intron: i for i, intron in enumerate(all_introns)}
+    exon_to_index = {exon: i for i, exon in enumerate(all_exons)}
+
+
+
+
+    # Step 3: Populate the matrix
+    row_indices = []
+    col_indices = []
+    for isoform, introns in isoform_to_introns.items():
+        row_index = isoform_to_index[isoform]
+        for intron in introns:
+            col_index = intron_to_index[intron]
+            row_indices.append(row_index)
+            col_indices.append(col_index)
+
+    num_rows = len(all_isoforms)
+    num_intron_cols = len(all_introns)
+
+
+    isoform_intron_matrix = scipy.sparse.coo_matrix(
+        ( [1]*len(row_indices), (row_indices, col_indices) ),
+        shape=(num_rows, num_intron_cols)
+        )
+
+
+    row_indices = []
+    col_indices = []
+    for isoform, exons in isoform_to_exons.items():
+        row_index = isoform_to_index[isoform]
+        for exon in exons:
+            col_index = exon_to_index[exon]
+            row_indices.append(row_index)
+            col_indices.append(col_index)
+
+    num_exon_cols = len(all_exons)
+    
+    isoform_exon_matrix = scipy.sparse.coo_matrix(
+        ( [1]*len(row_indices), (row_indices, col_indices) ),
+        shape=(num_rows, num_exon_cols)
+        )
+
+
+
+    save_npz(f'{out_prefix}isoform_intron_matrix.npz', isoform_intron_matrix)
+    save_npz(f'{out_prefix}isoform_exon_matrix.npz', isoform_exon_matrix)
+
+
+    with open(f'{out_prefix}isoform_rows.txt', 'w') as output:
+        for isoform in all_isoforms:
+            print(isoform, file= output)
+
+    with open(f'{out_prefix}intron_cols.txt', 'w') as output:
+        for intron in all_introns:
+            print(intron, file= output)
+
+    with open(f'{out_prefix}exon_cols.txt', 'w') as output:
+        for exon in all_exons:
+            print(exon, file= output)
+
+
+
+
+    
+    
+    
+    
+    
+    
 ##############################################################################################
 
 #these function is some additional features, not fully tested yet
 
 def add_virtual_first_last_introns(trancript_to_intron_map, intron_to_exon_map, out_prefix = '', include_exon = False):
     """
     This is the function that use to add virtual intron 0 and -1 to capture 
@@ -405,14 +533,18 @@
     compute_transcript_intron_map(options.annot, out_prefix= options.outprefix,\
                                   annot_type = options.annot_source,\
                                   min_length = options.minintronlen,\
                                   max_length= options.maxintronlen, \
                                   quality_control= options.quality_control)
         
     out_prefix = options.outprefix    
+    
+    if options.single_cell == True:
+        isoform_intron_exon_sparse_generation(f'{out_prefix}isoform_intron_map.tsv', out_prefix)
+        
     if options.annot_source == 'gencode':
         intron_source_generation(f'{out_prefix}isoform_intron_map.tsv',out_prefix)
         
     if options.virtual_intron == True:
         
         f'{out_prefix}intron_exon_connectivity.tsv'
         f'{out_prefix}isoform_intron_map.tsv'
@@ -420,15 +552,14 @@
         add_virtual_first_last_introns(f'{out_prefix}isoform_intron_map.tsv', f'{out_prefix}intron_exon_connectivity.tsv',\
                                         out_prefix)
 
 
 
 
 
-
 if __name__ == "__main__":
 
     parser = OptionParser()
 
     parser.add_option('-a',"--annot", dest="annot", default = None,
               help="annotation source, support gencode, Stringtie \
                   (in progress, will add support to ref_seq, ensembl)")    
@@ -448,41 +579,44 @@
                   help="minimum intron length in bp (default 50bp)")
 
     parser.add_option("--quality_control", dest="quality_control", default = True,
                  help="whether to remove pseudogene, and decay transcript")
 
     parser.add_option("-v", "--virtual_intron", dest="virtual_intron", default = False,
                  help="whether to use virtual intron to capture alternative first and last exon usage")
-   
+    
+    parser.add_option("--single_cell", dest="single_cell", default = True,
+                 help="whether to build matrices for isoform to intron and exon, required if dealing with\
+                     single cell data from alevin-fry")
+    
+    
     (options, args) = parser.parse_args()
 
 
 
     if options.annot is None:
         sys.exit("Error: no annotation file provided...\n")
 
 
-    sys.stderr.write(f"Start Processing transcriptome annotation {options.annot}")
-    sys.stderr.write(f"annot source: {options.annot_source}")
-    sys.stderr.write(f"outprefix: {options.outprefix}")
-    sys.stderr.write(f"Max intron length: {options.maxintronlen}")
-    sys.stderr.write(f"Min intron length: {options.minintronlen}")
-    sys.stderr.write(f"remove pseudogene and decay transcript: {options.quality_control}")
-    sys.stderr.write(f"virtual intron: {options.virtual_intron}")
+    sys.stderr.write(f"Start Processing transcriptome annotation {options.annot}\n")
+    sys.stderr.write(f"annot source: {options.annot_source}\n")
+    sys.stderr.write(f"outprefix: {options.outprefix}\n")
+    sys.stderr.write(f"Max intron length: {options.maxintronlen}\n")
+    sys.stderr.write(f"Min intron length: {options.minintronlen}\n")
+    sys.stderr.write(f"remove pseudogene and decay transcript: {options.quality_control}\n")
+    sys.stderr.write(f"virtual intron: {options.virtual_intron}\n")
     
     record = f'{options.outprefix}map_parameters.txt'
-    sys.stderr.write(f'saving record to {record}')
+    sys.stderr.write(f'saving record to {record} \n')
     
     write_options_to_file(options, record)
 
     LeafcutterITI_map_generation(options)
     
-    sys.stderr.write('Finish building Isofrom to intron map')
-
-
+    sys.stderr.write('Finish building Isofrom to intron map \n')
```

### Comparing `leafcutterITI-0.1.8/leafcutterITI/utils.py` & `leafcutteriti-0.2.0/leafcutterITI/utils.py`

 * *Files identical despite different names*

### Comparing `leafcutterITI-0.1.8/leafcutterITI.egg-info/SOURCES.txt` & `leafcutteriti-0.2.0/leafcutterITI.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 leafcutterITI/__init__.py
 leafcutterITI/__main__.py
+leafcutterITI/shared_functions.py
 leafcutterITI/utils.py
 leafcutterITI.egg-info/PKG-INFO
 leafcutterITI.egg-info/SOURCES.txt
 leafcutterITI.egg-info/dependency_links.txt
 leafcutterITI.egg-info/entry_points.txt
 leafcutterITI.egg-info/requires.txt
 leafcutterITI.egg-info/top_level.txt
 leafcutterITI/clustering/__init__.py
 leafcutterITI/clustering/leafcutterITI_clustering.py
 leafcutterITI/clustering/utils.py
 leafcutterITI/map_gen/__init__.py
-leafcutterITI/map_gen/leafcutterITI_map_gen.py
+leafcutterITI/map_gen/leafcutterITI_map_gen.py
+leafcutterITI/scITI/__init__.py
+leafcutterITI/scITI/calcutta_functions.py
+leafcutterITI/scITI/leafcutterITI_scITI.py
```

### Comparing `leafcutterITI-0.1.8/pyproject.toml` & `leafcutteriti-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 requires = ["setuptools>=61.0"] # to support project.scripts
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "leafcutterITI"
 description='LeafcutterITI implementation'
 authors = [{name = "Xingpei Zhang"}, {name="David A Knowles"}]
-version = "0.1.8"
+version = "0.2.0"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
     "numpy",
     "pyranges",
-    "pandas"
+    "pandas",
+    "scipy"
 ]
 license= {file = "LICENSE"}
 
 [project.scripts]
-leafcutterITI-cluster = 'leafcutterITI.__main__:leafcutterITI_clustering'
 leafcutterITI-map = 'leafcutterITI.__main__:leafcutterITI_map_gen'
-
+leafcutterITI-cluster = 'leafcutterITI.__main__:leafcutterITI_clustering'
+leafcutterITI-scITI = 'leafcutterITI.__main__:leafcutterITI_scITI'
 
 [project.urls]
 Homepage = "https://github.com/XZ3149/LeafcutterITI"
```

### Comparing `leafcutterITI-0.1.8/setup.py` & `leafcutteriti-0.2.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 import setuptools
 
 
 
 setup(
         name='leafcutterITI',
         packages=find_packages(),
-        version='0.1.8',
+        version='0.2.0',
         description='LeafcutterITI implementation',
         author='Xingpei Zhang, David A Knowles',
         license='MIT',
         entry_points={
             'console_scripts': [
-                'leafcutterITI-map = leafcutter.__main__:leafcutterITI_map_gen',
-                'leafcutterITI-cluster = leafcutter.__main__:leafcutterITI_clustering'
+                'leafcutterITI-map = leafcutterITI.__main__:leafcutterITI_map_gen',
+                'leafcutterITI-cluster = leafcutterITI.__main__:leafcutterITI_clustering',
+                'leafcutterITI-scITI = leafcutterITI.__main__:leafcutterITI_scITI'
             ],
         },
     )
```

