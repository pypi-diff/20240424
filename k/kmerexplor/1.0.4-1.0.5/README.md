# Comparing `tmp/kmerexplor-1.0.4.tar.gz` & `tmp/kmerexplor-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kmerexplor-1.0.4.tar", last modified: Tue Apr  2 07:01:43 2024, max compression
+gzip compressed data, was "kmerexplor-1.0.5.tar", last modified: Wed Apr 24 11:44:11 2024, max compression
```

## Comparing `kmerexplor-1.0.4.tar` & `kmerexplor-1.0.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2024-04-02 07:01:43.807968 kmerexplor-1.0.4/
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)      212 2023-07-19 12:51:29.000000 kmerexplor-1.0.4/MANIFEST.in
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)    14032 2024-04-02 07:01:43.803335 kmerexplor-1.0.4/PKG-INFO
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)    11137 2024-03-25 08:29:20.000000 kmerexplor-1.0.4/README.md
-drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2024-04-02 07:01:43.602276 kmerexplor-1.0.4/kmerexplor/
--rwxrwxr-x   0 benoit    (1017) bio2m     (1010)      115 2023-07-19 12:51:29.000000 kmerexplor-1.0.4/kmerexplor/__init__.py
--rwxrwxr-x   0 benoit    (1017) bio2m     (1010)     2478 2023-07-19 12:51:29.000000 kmerexplor-1.0.4/kmerexplor/checkFile.py
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)     1088 2024-03-25 08:29:20.000000 kmerexplor-1.0.4/kmerexplor/common.py
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)    11533 2024-03-13 11:14:24.000000 kmerexplor-1.0.4/kmerexplor/config.yaml
--rwxrwxr-x   0 benoit    (1017) bio2m     (1010)     6768 2024-03-25 08:29:20.000000 kmerexplor-1.0.4/kmerexplor/core.py
--rwxrwxr-x   0 benoit    (1017) bio2m     (1010)    89080 2023-07-19 12:51:29.000000 kmerexplor-1.0.4/kmerexplor/countTags
--rwxrwxr-x   0 benoit    (1017) bio2m     (1010)    14740 2024-03-25 08:29:20.000000 kmerexplor-1.0.4/kmerexplor/counts.py
--rwxrwxr-x   0 benoit    (1017) bio2m     (1010)      209 2024-04-02 07:01:23.000000 kmerexplor-1.0.4/kmerexplor/info.py
--rwxrwxr-x   0 benoit    (1017) bio2m     (1010)   658096 2024-03-25 08:29:21.000000 kmerexplor-1.0.4/kmerexplor/mk_results.py
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)    10495 2024-04-02 06:52:17.000000 kmerexplor-1.0.4/kmerexplor/options.py
--rwxrwxr-x   0 benoit    (1017) bio2m     (1010)     2659 2023-07-19 12:51:30.000000 kmerexplor-1.0.4/kmerexplor/samples.py
-drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2024-04-02 07:01:43.786089 kmerexplor-1.0.4/kmerexplor/tagsets/
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)     1198 2024-03-25 08:29:21.000000 kmerexplor-1.0.4/kmerexplor/tagsets/human-quality.md
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)  4116851 2024-03-25 17:03:22.000000 kmerexplor-1.0.4/kmerexplor/tagsets/human-quality.tsv.gz
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)    11533 2024-03-25 08:29:21.000000 kmerexplor-1.0.4/kmerexplor/tagsets/human-quality.yaml
-drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2024-04-02 07:01:43.692458 kmerexplor-1.0.4/kmerexplor.egg-info/
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)    14032 2024-04-02 07:01:43.000000 kmerexplor-1.0.4/kmerexplor.egg-info/PKG-INFO
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)      590 2024-04-02 07:01:43.000000 kmerexplor-1.0.4/kmerexplor.egg-info/SOURCES.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)        1 2024-04-02 07:01:43.000000 kmerexplor-1.0.4/kmerexplor.egg-info/dependency_links.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)       53 2024-04-02 07:01:43.000000 kmerexplor-1.0.4/kmerexplor.egg-info/entry_points.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)       16 2024-04-02 07:01:43.000000 kmerexplor-1.0.4/kmerexplor.egg-info/requires.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)       11 2024-04-02 07:01:43.000000 kmerexplor-1.0.4/kmerexplor.egg-info/top_level.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)       38 2024-04-02 07:01:43.810448 kmerexplor-1.0.4/setup.cfg
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)     1032 2023-10-20 07:36:54.000000 kmerexplor-1.0.4/setup.py
+drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2024-04-24 11:44:11.131082 kmerexplor-1.0.5/
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)      212 2023-07-19 12:51:29.000000 kmerexplor-1.0.5/MANIFEST.in
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)    14028 2024-04-24 11:44:11.126569 kmerexplor-1.0.5/PKG-INFO
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)    11133 2024-04-02 07:08:45.000000 kmerexplor-1.0.5/README.md
+drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2024-04-24 11:44:10.944190 kmerexplor-1.0.5/kmerexplor/
+-rwxrwxr-x   0 benoit    (1017) bio2m     (1010)      115 2023-07-19 12:51:29.000000 kmerexplor-1.0.5/kmerexplor/__init__.py
+-rwxrwxr-x   0 benoit    (1017) bio2m     (1010)     2478 2023-07-19 12:51:29.000000 kmerexplor-1.0.5/kmerexplor/checkFile.py
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)     1088 2024-03-25 08:29:20.000000 kmerexplor-1.0.5/kmerexplor/common.py
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)    11533 2024-03-13 11:14:24.000000 kmerexplor-1.0.5/kmerexplor/config.yaml
+-rwxrwxr-x   0 benoit    (1017) bio2m     (1010)     6359 2024-04-24 08:24:46.000000 kmerexplor-1.0.5/kmerexplor/core.py
+-rwxrwxr-x   0 benoit    (1017) bio2m     (1010)    89080 2023-07-19 12:51:29.000000 kmerexplor-1.0.5/kmerexplor/countTags
+-rwxrwxr-x   0 benoit    (1017) bio2m     (1010)    14694 2024-04-24 08:27:35.000000 kmerexplor-1.0.5/kmerexplor/counts.py
+-rwxrwxr-x   0 benoit    (1017) bio2m     (1010)      209 2024-04-24 08:25:06.000000 kmerexplor-1.0.5/kmerexplor/info.py
+-rwxrwxr-x   0 benoit    (1017) bio2m     (1010)   658096 2024-03-25 08:29:21.000000 kmerexplor-1.0.5/kmerexplor/mk_results.py
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)    10495 2024-04-02 06:52:17.000000 kmerexplor-1.0.5/kmerexplor/options.py
+-rwxrwxr-x   0 benoit    (1017) bio2m     (1010)     2659 2023-07-19 12:51:30.000000 kmerexplor-1.0.5/kmerexplor/samples.py
+drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2024-04-24 11:44:11.109303 kmerexplor-1.0.5/kmerexplor/tagsets/
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)     1198 2024-03-25 08:29:21.000000 kmerexplor-1.0.5/kmerexplor/tagsets/human-quality.md
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)  2210785 2024-04-24 08:21:09.000000 kmerexplor-1.0.5/kmerexplor/tagsets/human-quality.tsv.gz
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)    11533 2024-03-25 08:29:21.000000 kmerexplor-1.0.5/kmerexplor/tagsets/human-quality.yaml
+drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2024-04-24 11:44:11.034105 kmerexplor-1.0.5/kmerexplor.egg-info/
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)    14028 2024-04-24 11:44:10.000000 kmerexplor-1.0.5/kmerexplor.egg-info/PKG-INFO
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)      590 2024-04-24 11:44:10.000000 kmerexplor-1.0.5/kmerexplor.egg-info/SOURCES.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)        1 2024-04-24 11:44:10.000000 kmerexplor-1.0.5/kmerexplor.egg-info/dependency_links.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)       53 2024-04-24 11:44:10.000000 kmerexplor-1.0.5/kmerexplor.egg-info/entry_points.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)       16 2024-04-24 11:44:10.000000 kmerexplor-1.0.5/kmerexplor.egg-info/requires.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)       11 2024-04-24 11:44:10.000000 kmerexplor-1.0.5/kmerexplor.egg-info/top_level.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)       38 2024-04-24 11:44:11.133778 kmerexplor-1.0.5/setup.cfg
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)     1032 2023-10-20 07:36:54.000000 kmerexplor-1.0.5/setup.py
```

### Comparing `kmerexplor-1.0.4/PKG-INFO` & `kmerexplor-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmerexplor
-Version: 1.0.4
+Version: 1.0.5
 Summary: KmerExploR provides information on RNA-sequencing datasets.
 Home-page: https://github.com/Transipedia/KmerExploR
 Author: Benoit Guibert
 Author-email: benoit.guibert@free.fr
 License: GPLv3
 Description: # KmerExploR
         
@@ -122,15 +122,15 @@
         
         
         ## Usage
         
         Without options or with `--help`, `KmerExploR` returns Help
         
         ```
-        usage: kmerexplor-dev [-h] [-s] [-p] [-k <int>] [-K] [-d] [-b BUILTIN_TAGS] [-o <output_dir>] [--tmp-dir <tmp_dir>] [-C <file_name>] [-T <tag_file>] [-l]
+        usage: kmerexplor [-h] [-s] [-p] [-k <int>] [-K] [-d] [-b BUILTIN_TAGS] [-o <output_dir>] [--tmp-dir <tmp_dir>] [-C <file_name>] [-T <tag_file>] [-l]
                               [--dump-config file_name] [--show-tags] [--title <string>] [-y] [-c <int>] [-v]
                               [<file1> ... ...]
         
         positional arguments:
           <file1> ...           fastq or fastq.gz or tsv countTags output files.
         
         optional arguments:
```

### Comparing `kmerexplor-1.0.4/README.md` & `kmerexplor-1.0.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 
 
 ## Usage
 
 Without options or with `--help`, `KmerExploR` returns Help
 
 ```
-usage: kmerexplor-dev [-h] [-s] [-p] [-k <int>] [-K] [-d] [-b BUILTIN_TAGS] [-o <output_dir>] [--tmp-dir <tmp_dir>] [-C <file_name>] [-T <tag_file>] [-l]
+usage: kmerexplor [-h] [-s] [-p] [-k <int>] [-K] [-d] [-b BUILTIN_TAGS] [-o <output_dir>] [--tmp-dir <tmp_dir>] [-C <file_name>] [-T <tag_file>] [-l]
                       [--dump-config file_name] [--show-tags] [--title <string>] [-y] [-c <int>] [-v]
                       [<file1> ... ...]
 
 positional arguments:
   <file1> ...           fastq or fastq.gz or tsv countTags output files.
 
 optional arguments:
```

### Comparing `kmerexplor-1.0.4/kmerexplor/checkFile.py` & `kmerexplor-1.0.5/kmerexplor/checkFile.py`

 * *Files identical despite different names*

### Comparing `kmerexplor-1.0.4/kmerexplor/common.py` & `kmerexplor-1.0.5/kmerexplor/common.py`

 * *Files identical despite different names*

### Comparing `kmerexplor-1.0.4/kmerexplor/config.yaml` & `kmerexplor-1.0.5/kmerexplor/config.yaml`

 * *Files identical despite different names*

### Comparing `kmerexplor-1.0.4/kmerexplor/core.py` & `kmerexplor-1.0.5/kmerexplor/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,24 +53,14 @@
     ### If "ctrl C" is set, quit after executing exit_gracefully function
     try:
         run(args, config)
     except KeyboardInterrupt:
         print(f"Process interrupted by user", file=sys.stderr)
         exit_gracefully(args)
 
-'''
-def get_user_config(args, fileset):
-    if args.config:
-        fileset.config = args.config
-        if args.tags:
-            fileset.tags = args.tags
-        desc = f"{args.tags[:-len(ext)]}md"
-        if os.path.isfile(desc):
-            fileset.desc = desc
-'''
 
 def config2dict(args):
     """ Load config yaml file as dict """
     config_file = args.setfiles['config']
     try:
         with open(config_file) as stream:
             return yaml.safe_load(stream)
@@ -80,14 +70,15 @@
         sys.exit(f"Error {err}")
 
 
 def run(args, config):
     """ Function doc """
     nprocs, files = args.cores, args.files
     if args.debug: print("Arguments:", args)
+
     ### 1. Define some PATH
     # create directory for temporay files
     args.tmp_dir = tempfile.mkdtemp(prefix=info.APPNAME.lower() + "-", dir=args.tmp_dir)
     # define countTags PATH
     if args.keep_counts:
         ## If the user wants to keep the countTag counts
         args.counts_dir = os.path.join(args.output, 'countTags')
@@ -121,43 +112,40 @@
     ### 3. If fastq files, determine paired (if '--paired' argument is specified)
     if files_type == 'fastq':
         sample_list = set_sample_list(files, args, files_type)
         if not sample_list:
             print("\n Error: no samples {} found\n".format('single' if args.single else 'paired'), file=sys.stderr)
             sys.exit(exit_gracefully(args, files_type))
 
-    ### 4. Handle tags
-    # ~ tags_file = get_tags_file(args)
-    # ~ tags_file_desc = f"{os.path.splitext(tags_file.rstrip('.gz'))[0]}.md"
 
-    ### 5. If input files are fastq, run countTags (Multiprocessed)
+    ### 4. If input files are fastq, run countTags (Multiprocessed)
     if files_type == 'fastq':
         ### Compute countTags with multi processing (use --core to specify cores counts)
         sys.stdout.write("\n ✨✨ Starting countTags, please wait.\n\n")
         with multiprocessing.Pool(processes=nprocs) as pool:
             results = pool.starmap_async(do_countTags, [(sample, args) for sample in sample_list])
             results.wait()
         samples_path = [f for f in glob.glob("{}/*.tsv".format(args.counts_dir))]
     else:
         samples_path = args.files
 
-    ### 6. merge countTags tables
+    ### 5. merge countTags tables
     sys.stdout.write("\n ✨✨ Starting merge of counts.\n")
     samples_path.sort()
     counts = Counts(samples_path, args)
 
-    ### 7. Build results as html pages and tsv table
+    ### 6. Build results as html pages and tsv table
     sys.stdout.write("\n ✨✨ Build output html page.\n")
     table = TSV(counts, args)                                   # create TSV file
     charts = HTML(counts, args, info, config, args.setfiles['desc'])     # create results in html format
 
-    ### 8. show results
+    ### 7. show results
     show_res(args,counts, table.tsvfile, charts.htmlfile, files_type)
 
-    ### 9. exit gracefully program
+    ### 8. exit gracefully program
     exit_gracefully(args, files_type)
 
 
 
 def is_valid(file, args):
     """ Function doc """
     f = cf.File(file)
```

### Comparing `kmerexplor-1.0.4/kmerexplor/countTags` & `kmerexplor-1.0.5/kmerexplor/countTags`

 * *Files identical despite different names*

### Comparing `kmerexplor-1.0.4/kmerexplor/counts.py` & `kmerexplor-1.0.5/kmerexplor/counts.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,16 +96,15 @@
                     continue
                 ### split line
                 row = row.rstrip().split('\t')
                 ### The kmer can be representative of several tag names (seq-type + seq-id + queue)
                 tagnames = row[1].split(',')
                 for tagname in tagnames:
                     try:
-                        seq_type = tagname.split('-')[0]
-                        seq_id = tagname.split('-')[1]
+                        seq_type, seq_id = tagname.split('-')[:2]
                         seq_counts = row[2:]
                     except IndexError:
                         sys.exit(f"\n IndexError: missing at least one field in '{file}' file (2 fields expected, hyphen separated).")
                     ### Add sequence type if not exists (ex: sex, orientation)
                     if not seq_type in tags['counts']:
                         tags['counts'][seq_type] = {}
                     ### Add seq_id (often gene) if not exist (ex: VPS29, HIST1H2BF)
```

### Comparing `kmerexplor-1.0.4/kmerexplor/mk_results.py` & `kmerexplor-1.0.5/kmerexplor/mk_results.py`

 * *Files identical despite different names*

### Comparing `kmerexplor-1.0.4/kmerexplor/options.py` & `kmerexplor-1.0.5/kmerexplor/options.py`

 * *Files identical despite different names*

### Comparing `kmerexplor-1.0.4/kmerexplor/samples.py` & `kmerexplor-1.0.5/kmerexplor/samples.py`

 * *Files identical despite different names*

### Comparing `kmerexplor-1.0.4/kmerexplor/tagsets/human-quality.md` & `kmerexplor-1.0.5/kmerexplor/tagsets/human-quality.md`

 * *Files identical despite different names*

### Comparing `kmerexplor-1.0.4/kmerexplor/tagsets/human-quality.yaml` & `kmerexplor-1.0.5/kmerexplor/tagsets/human-quality.yaml`

 * *Files identical despite different names*

### Comparing `kmerexplor-1.0.4/kmerexplor.egg-info/PKG-INFO` & `kmerexplor-1.0.5/kmerexplor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmerexplor
-Version: 1.0.4
+Version: 1.0.5
 Summary: KmerExploR provides information on RNA-sequencing datasets.
 Home-page: https://github.com/Transipedia/KmerExploR
 Author: Benoit Guibert
 Author-email: benoit.guibert@free.fr
 License: GPLv3
 Description: # KmerExploR
         
@@ -122,15 +122,15 @@
         
         
         ## Usage
         
         Without options or with `--help`, `KmerExploR` returns Help
         
         ```
-        usage: kmerexplor-dev [-h] [-s] [-p] [-k <int>] [-K] [-d] [-b BUILTIN_TAGS] [-o <output_dir>] [--tmp-dir <tmp_dir>] [-C <file_name>] [-T <tag_file>] [-l]
+        usage: kmerexplor [-h] [-s] [-p] [-k <int>] [-K] [-d] [-b BUILTIN_TAGS] [-o <output_dir>] [--tmp-dir <tmp_dir>] [-C <file_name>] [-T <tag_file>] [-l]
                               [--dump-config file_name] [--show-tags] [--title <string>] [-y] [-c <int>] [-v]
                               [<file1> ... ...]
         
         positional arguments:
           <file1> ...           fastq or fastq.gz or tsv countTags output files.
         
         optional arguments:
```

### Comparing `kmerexplor-1.0.4/kmerexplor.egg-info/SOURCES.txt` & `kmerexplor-1.0.5/kmerexplor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kmerexplor-1.0.4/setup.py` & `kmerexplor-1.0.5/setup.py`

 * *Files identical despite different names*

