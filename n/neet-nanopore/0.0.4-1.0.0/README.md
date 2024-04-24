# Comparing `tmp/neet-nanopore-0.0.4.tar.gz` & `tmp/neet_nanopore-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neet-nanopore-0.0.4.tar", last modified: Fri Feb 16 09:25:03 2024, max compression
+gzip compressed data, was "neet_nanopore-1.0.0.tar", last modified: Wed Apr 24 12:47:57 2024, max compression
```

## Comparing `neet-nanopore-0.0.4.tar` & `neet_nanopore-1.0.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-02-16 09:25:03.546077 neet-nanopore-0.0.4/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    35148 2024-01-05 14:33:17.000000 neet-nanopore-0.0.4/LICENSE
--rw-r--r--   0 vincent   (1000) vincent   (1000)     2465 2024-02-16 09:25:03.546077 neet-nanopore-0.0.4/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1716 2024-01-16 14:11:19.000000 neet-nanopore-0.0.4/README.md
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-02-16 09:25:03.542077 neet-nanopore-0.0.4/neet/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2024-01-16 09:22:45.000000 neet-nanopore-0.0.4/neet/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    36602 2024-01-16 13:52:25.000000 neet-nanopore-0.0.4/neet/__main__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       19 2024-02-16 09:18:58.000000 neet-nanopore-0.0.4/neet/__version__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    10812 2024-01-16 11:09:25.000000 neet-nanopore-0.0.4/neet/bed_ops.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    15435 2024-01-16 11:09:24.000000 neet-nanopore-0.0.4/neet/filter.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     8529 2024-02-16 07:30:52.000000 neet-nanopore-0.0.4/neet/helper_functions.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    31583 2024-02-16 07:37:37.000000 neet-nanopore-0.0.4/neet/pileup_extractor.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    60621 2024-01-16 11:10:11.000000 neet-nanopore-0.0.4/neet/poi_analyzer.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    26610 2024-01-16 11:10:23.000000 neet-nanopore-0.0.4/neet/position_summary.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    47701 2024-02-16 09:13:13.000000 neet-nanopore-0.0.4/neet/summary.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-02-16 09:25:03.546077 neet-nanopore-0.0.4/neet/summary_style/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2024-01-05 14:33:17.000000 neet-nanopore-0.0.4/neet/summary_style/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)  3478174 2024-01-05 14:33:17.000000 neet-nanopore-0.0.4/neet/summary_style/plotly.js
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4276 2024-01-10 11:11:48.000000 neet-nanopore-0.0.4/neet/summary_style/style.css
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    22946 2024-01-16 11:10:38.000000 neet-nanopore-0.0.4/neet/two_sample_extractor.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-02-16 09:25:03.546077 neet-nanopore-0.0.4/neet_nanopore.egg-info/
--rw-r--r--   0 vincent   (1000) vincent   (1000)     2465 2024-02-16 09:25:03.000000 neet-nanopore-0.0.4/neet_nanopore.egg-info/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      580 2024-02-16 09:25:03.000000 neet-nanopore-0.0.4/neet_nanopore.egg-info/SOURCES.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2024-02-16 09:25:03.000000 neet-nanopore-0.0.4/neet_nanopore.egg-info/dependency_links.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       44 2024-02-16 09:25:03.000000 neet-nanopore-0.0.4/neet_nanopore.egg-info/entry_points.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      111 2024-02-16 09:25:03.000000 neet-nanopore-0.0.4/neet_nanopore.egg-info/requires.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        5 2024-02-16 09:25:03.000000 neet-nanopore-0.0.4/neet_nanopore.egg-info/top_level.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      273 2024-02-16 09:22:23.000000 neet-nanopore-0.0.4/pyproject.toml
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       38 2024-02-16 09:25:03.546077 neet-nanopore-0.0.4/setup.cfg
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1257 2024-02-16 09:18:14.000000 neet-nanopore-0.0.4/setup.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-24 12:47:57.857701 neet_nanopore-1.0.0/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    35148 2024-01-05 14:33:17.000000 neet_nanopore-1.0.0/LICENSE
+-rw-r--r--   0 vincent   (1000) vincent   (1000)     3000 2024-04-24 12:47:57.857701 neet_nanopore-1.0.0/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2157 2024-04-22 09:20:51.000000 neet_nanopore-1.0.0/README.md
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-24 12:47:57.853701 neet_nanopore-1.0.0/neet/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2024-01-16 09:22:45.000000 neet_nanopore-1.0.0/neet/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    44713 2024-04-24 12:07:29.000000 neet_nanopore-1.0.0/neet/__main__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       19 2024-04-24 12:41:23.000000 neet_nanopore-1.0.0/neet/__version__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    10915 2024-04-22 06:47:23.000000 neet_nanopore-1.0.0/neet/bed_ops.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    16111 2024-04-24 11:50:07.000000 neet_nanopore-1.0.0/neet/filter.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    16700 2024-04-22 06:47:12.000000 neet_nanopore-1.0.0/neet/helper_functions.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    45937 2024-04-24 12:04:10.000000 neet_nanopore-1.0.0/neet/pileup_extractor.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    28648 2024-04-24 11:36:35.000000 neet_nanopore-1.0.0/neet/poi_sample_comparer.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    71617 2024-04-24 11:44:59.000000 neet_nanopore-1.0.0/neet/poi_summary.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    26705 2024-04-24 12:35:42.000000 neet_nanopore-1.0.0/neet/poi_view.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    51438 2024-04-24 11:28:29.000000 neet_nanopore-1.0.0/neet/summary.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-24 12:47:57.853701 neet_nanopore-1.0.0/neet/summary_style/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2024-01-05 14:33:17.000000 neet_nanopore-1.0.0/neet/summary_style/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)  3478174 2024-01-05 14:33:17.000000 neet_nanopore-1.0.0/neet/summary_style/plotly.js
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4276 2024-04-03 08:32:40.000000 neet_nanopore-1.0.0/neet/summary_style/style.css
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    31823 2024-04-24 11:44:06.000000 neet_nanopore-1.0.0/neet/two_sample_extractor.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-24 12:47:57.853701 neet_nanopore-1.0.0/neet_nanopore.egg-info/
+-rw-r--r--   0 vincent   (1000) vincent   (1000)     3000 2024-04-24 12:47:57.000000 neet_nanopore-1.0.0/neet_nanopore.egg-info/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      599 2024-04-24 12:47:57.000000 neet_nanopore-1.0.0/neet_nanopore.egg-info/SOURCES.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2024-04-24 12:47:57.000000 neet_nanopore-1.0.0/neet_nanopore.egg-info/dependency_links.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       44 2024-04-24 12:47:57.000000 neet_nanopore-1.0.0/neet_nanopore.egg-info/entry_points.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      160 2024-04-24 12:47:57.000000 neet_nanopore-1.0.0/neet_nanopore.egg-info/requires.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        5 2024-04-24 12:47:57.000000 neet_nanopore-1.0.0/neet_nanopore.egg-info/top_level.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      273 2024-04-24 12:41:15.000000 neet_nanopore-1.0.0/pyproject.toml
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       38 2024-04-24 12:47:57.857701 neet_nanopore-1.0.0/setup.cfg
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1484 2024-04-23 08:10:04.000000 neet_nanopore-1.0.0/setup.py
```

### Comparing `neet-nanopore-0.0.4/LICENSE` & `neet_nanopore-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neet-nanopore-0.0.4/PKG-INFO` & `neet_nanopore-1.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,51 +1,71 @@
 Metadata-Version: 2.1
 Name: neet-nanopore
-Version: 0.0.4
+Version: 1.0.0
 Home-page: https://github.com/dietvin/neet
 Author: Vincent Dietrich
 Author-email: dietricv@uni-mainz.de
 License: LICENSE
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Operating System :: OS Independent
 Requires-Python: >3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: plotly==5.18.0
+Requires-Dist: kaleido==0.2.1
+Requires-Dist: numpy==1.26.2
+Requires-Dist: pandas==2.1.4
 Requires-Dist: tqdm==4.66.1
 Requires-Dist: intervaltree==3.1.0
 Requires-Dist: scipy==1.11.4
+Requires-Dist: statsmodels==0.14.1
 Requires-Dist: pyfiglet==1.0.2
 Requires-Dist: setuptools==69.0.3
-Requires-Dist: pandas==2.1.4
 
 # NEET - Nanopore Error pattern Exploration Toolkit
 
 The Nanopore Error pattern Exploration Toolkit (`NEET`) provides a range of functionalities that provide an easily accessible and interactive analysis approach for (systematic) base-calling errors in direct RNA nanopore sequencing data. The implemented modules include options for condensing, visualizing and differentiating error features contained in direct RNA sequencing data - including mismatch, deletion and insertion rates, among others.
 
 ## Installation
+
 It is recommended to use Conda/Mamba and pip for installation:
+
 ```
 conda create -y -n neet python==3.10 && conda activate neet
 pip install neet-nanopore
 neet --version
 ```
+
 For more information and alternative installation approaches refer to the [Wiki](https://github.com/dietvin/neet/wiki/01-Installation).
 
 ## General usage
+
 Once installed `NEET` can be accessed via the terminal:
+
 ```
 neet --help
 ```
+
 Individual modules can be accessed as follows:
+
 ```
 neet [MODULE] --help
 ```
-Available modules are: Pileup Extractor (`extractor`), Summary (`summmary`), Position-of-Interest Analyzer (`analyzepoi`), Two-Sample Extractor (`twosample`), Position Summary (`possummary`), Filter (`filter`) and Bedops (`bedops`). 
-The modules are interconnected to provide different workflows for different scenarios. An overview of the main workflows is given below:
+
+Available modules are:
+
+- Pileup Extractor (`extractor`): Extract data from pileup files into feature tables
+- Summary (`summmary`): Summarize and visualize feature tables
+- Position-of-Interest Summary (`poisummary`): Summarize and visualize specific positions of interest
+- Position-of-Interest View (`poiview`): Visualize positions of interest
+- Position-of-Interest  (`poicompare`): Statistically compare positions of interest
+- Two-Sample Extractor (`extractdiff`): Identify and extract positions of increased error rates between two conditions
+- Filter (`filter`): Filter feature tables by given features
+- Bedops (`bedops`): Process and manipulate bed files
+  The modules are interconnected to provide different workflows for different scenarios. An overview of the main workflows is given below:
 
 ![Main workflow overview](https://github.com/dietvin/neet/blob/main/images/workflow_overview.jpg)
 
 A detailled description of all available modules is provided in the [Wiki](https://github.com/dietvin/neet/wiki/02-Modules). The Wiki also provides [walkthroughs](https://github.com/dietvin/neet/wiki/03-Example-Workflows) for some possible use cases.
```

### Comparing `neet-nanopore-0.0.4/README.md` & `neet_nanopore-1.0.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,45 @@
 # NEET - Nanopore Error pattern Exploration Toolkit
 
 The Nanopore Error pattern Exploration Toolkit (`NEET`) provides a range of functionalities that provide an easily accessible and interactive analysis approach for (systematic) base-calling errors in direct RNA nanopore sequencing data. The implemented modules include options for condensing, visualizing and differentiating error features contained in direct RNA sequencing data - including mismatch, deletion and insertion rates, among others.
 
 ## Installation
+
 It is recommended to use Conda/Mamba and pip for installation:
+
 ```
 conda create -y -n neet python==3.10 && conda activate neet
 pip install neet-nanopore
 neet --version
 ```
+
 For more information and alternative installation approaches refer to the [Wiki](https://github.com/dietvin/neet/wiki/01-Installation).
 
 ## General usage
+
 Once installed `NEET` can be accessed via the terminal:
+
 ```
 neet --help
 ```
+
 Individual modules can be accessed as follows:
+
 ```
 neet [MODULE] --help
 ```
-Available modules are: Pileup Extractor (`extractor`), Summary (`summmary`), Position-of-Interest Analyzer (`analyzepoi`), Two-Sample Extractor (`twosample`), Position Summary (`possummary`), Filter (`filter`) and Bedops (`bedops`). 
-The modules are interconnected to provide different workflows for different scenarios. An overview of the main workflows is given below:
+
+Available modules are:
+
+- Pileup Extractor (`extractor`): Extract data from pileup files into feature tables
+- Summary (`summmary`): Summarize and visualize feature tables
+- Position-of-Interest Summary (`poisummary`): Summarize and visualize specific positions of interest
+- Position-of-Interest View (`poiview`): Visualize positions of interest
+- Position-of-Interest  (`poicompare`): Statistically compare positions of interest
+- Two-Sample Extractor (`extractdiff`): Identify and extract positions of increased error rates between two conditions
+- Filter (`filter`): Filter feature tables by given features
+- Bedops (`bedops`): Process and manipulate bed files
+  The modules are interconnected to provide different workflows for different scenarios. An overview of the main workflows is given below:
 
 ![Main workflow overview](https://github.com/dietvin/neet/blob/main/images/workflow_overview.jpg)
 
 A detailled description of all available modules is provided in the [Wiki](https://github.com/dietvin/neet/wiki/02-Modules). The Wiki also provides [walkthroughs](https://github.com/dietvin/neet/wiki/03-Example-Workflows) for some possible use cases.
```

### Comparing `neet-nanopore-0.0.4/neet/__main__.py` & `neet_nanopore-1.0.0/neet/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,38 @@
 from pyfiglet import Figlet
+from typing import Tuple
 import argparse
-from . import helper_functions as hs
-from .__version__ import __version__
-from .pileup_extractor import FeatureExtractor
-from .summary import SummaryCreator
-from .poi_analyzer import POIAnalyzer
-from .two_sample_extractor import PositionExtractor
-from .position_summary import PositionSummary
-from .filter import Filter
-from .bed_ops import tsv_to_bed, intersect_beds, add_bed_info, merge, difference
+
+try:
+    from neet import helper_functions as hs
+    from neet.__version__ import __version__
+    from neet.pileup_extractor import FeatureExtractor
+    from neet.summary import SummaryCreator
+    from neet.poi_summary import POISummary
+    from neet.two_sample_extractor import PositionExtractor
+    from neet.poi_view import POIView
+    from neet.poi_sample_comparer import PoiSampleComparer
+    from neet.filter import Filter
+    from neet.bed_ops import tsv_to_bed, intersect_beds, add_bed_info, merge, difference
+except:
+    import helper_functions as hs
+    from __version__ import __version__
+    from pileup_extractor import FeatureExtractor
+    from summary import SummaryCreator
+    from neet.poi_summary import POISummary
+    from two_sample_extractor import PositionExtractor
+    from neet.poi_view import POIView
+    from poi_sample_comparer import PoiSampleComparer
+    from filter import Filter
+    from bed_ops import tsv_to_bed, intersect_beds, add_bed_info, merge, difference
 
 def print_figlet(text: str) -> None:
     print(Figlet(font="slant").renderText(text))
 
-def setup_parsers() -> argparse.ArgumentParser:
+def setup_parsers() -> Tuple[argparse.ArgumentParser, argparse.ArgumentParser]:
     parser = argparse.ArgumentParser(prog="NEET", 
                                      description="""
                                         Nanopore Error pattern Exploration Toolkit (NEET) -- 
                                         Framework for the analysis and exploration of (direct RNA) nanopore sequencing
                                         data. Github: https://github.com/dietvin/neet
                                         """)
     
@@ -32,22 +47,20 @@
                                                 """)
 
     extractor_parser.add_argument("-i", "--input", type=str, required=True,
                                   help="""
                                   Path to the input pileup file(s). If multiple are available, 
                                   specify paths comma-separated (<pileup1>,<pileup2>,...).
                                   """)
-    extractor_parser.add_argument("-o", "--output", type=str, required=True,
+    extractor_parser.add_argument("-o", "--output", type=str, required=False,
                                   help="""
-                                  Path to output file(s) (comma-separated if multiple) or directory. 
-                                  If filename(s) are given the order corresponds to the input files. 
-                                  If a directory is given, the output files are created using the 
-                                  basename from an input file with the suffix "_extracted.tsv".
-                                  Accordingly the summary file will be created with the suffix
-                                  "_extracted_summary.html".
+                                  Path to output directory. Output files for each input file gets written to this
+                                  directory using the basename from a given input file and the suffix '_extracted.tsv'.
+                                  Accordingly the summary file will be created with the suffix "_extracted_summary.html".
+                                  If not specified, the files get written to the same directory as the input file.
                                   """)
     extractor_parser.add_argument("-r", "--ref", type=str, required=True, 
                                   help="Path to the reference file in fasta format")
     extractor_parser.add_argument("-n", "--num_reads", type=hs.positive_int, required=False,
                                   help="""
                                   Filter by minimum number of reads at a position.  A position will 
                                   be dropped of if the coverage is lower than the given value.
@@ -77,70 +90,76 @@
                                   the mean quality is lower than the given value.
                                   """)
     extractor_parser.add_argument("-g", "--genomic_region", type=str, required=False,
                                   help="""
                                   Genomic region in "CHR:START-END" format or "CHR" for whole chromosome. 
                                   Specify to only extract information from a specific region.
                                   """)
-    extractor_parser.add_argument("--use_multiprocessing", action="store_true", 
-                                  help="""
-                                  Specify whether to use multiprocessing for processing. Recommended for shorter, 
-                                  deeply sequenced data. For low coverage, whole genome data set to false for 
-                                  faster runtime.
-                                  """)
-    extractor_parser.add_argument("-t", "--num_processes", type=int, required=False, default=4,
-                                  help="Number of parallel processes to use. Default: 4")
     extractor_parser.add_argument("-nw", "--window_size", type=int, required=False, default=2,
                                   help="""
                                   Number up-/downstream positions to consider for neighbouring error search.
                                   A value w corresponds to a sliding window of site 2*w+1.  Default: w=2
                                   """)
     extractor_parser.add_argument("-nt", "--neighbour_thresh", type=hs.float_between_zero_and_one, required=False, default=0.5,
                                   help="""
                                   Error threshold for neighbourhood search. During the search a neighbour
                                   with a mismatch rate above the given value will be counted as an error.
                                   Default: 0.5
                                   """)
-    extractor_parser.add_argument("-b", "--n_bins", type=int, required=False, default=5000,
-                                  help="""Number of bins to split the data into when creating the summary report.
-                                  This only affects the plots, not the underlying feature table. Used to improve 
-                                  performance and clarity of the created plots with many outliers. Note that 
-                                  setting the value to a low number can lead to misleading plots. Set to "-1" 
-                                  to disable binning. 
-                                  Default: 5000
-                                  """)
-    extractor_parser.add_argument("--plot_alt", action="store_true", 
+    extractor_parser.add_argument("--no_summary", action="store_true", 
+                                  help="Specify to disable the automatic creation of a HTML summary.")
+    extractor_parser.add_argument("-t", "--num_processes", type=int, required=False, default=8,
+                                  help="""
+                                  Number of parallel processes to use. Note that one of the given processes is reserved 
+                                  for writing. Default: 8
+                                  """)
+    extractor_parser.add_argument("-tq", "--queue_size", type=int, required=False, default=5000,
+                                  help="""
+                                  Maximum number of elements in the processing queues from different processes. Larger values may increase
+                                  compuational time while requiring more memory. Default: 5000
+                                  """)
+    extractor_parser.add_argument("-tt", "--temp_size", type=int, required=False, default=100000,
+                                  help="""
+                                  Maximum number of lines in a temporary file written. Larger values may increase computational time
+                                  while requiring more memory. Default: 100000
+                                  """)
+    extractor_parser.add_argument("-l", "--log_level", type=str, required=False,
                                   help="""
-                                  Specify whether to use the mismatch_rate or mismatch_rate_alt values for plotting
-                                  in the summary report.
+                                  Logging level. Can be one of: DEBUG, INFO, WARNING, ERROR, CRITICAL.
+                                  Specify to enable logging to a log file.
                                   """)
-    extractor_parser.add_argument("--export_svg", action="store_true", 
+    extractor_parser.add_argument("-lf", "--log_file", type=str, required=False,
                                   help="""
-                                  Specify to export the created plots in SVG format. Files will be created in the
-                                  output directory.
+                                  Path to the log file or path to a directory where the log file should be created.
+                                  Only relevant if --log_level is specified. If logging is enabled and no path is given or if the
+                                  given path is a directory, the file with name 'neet_<current-time>.log' is created in the current
+                                  working directory or the specified directory. 
                                   """)
 
+
+
     # add parser for summary
     summary_parser = subparsers.add_parser("summary", 
                                            help="""
                                             Create a visual overview of a feature table. 
                                             """)
     summary_parser.add_argument("-i", "--input", type=str, required=True,
                                 help="""
                                 Path to the input TSV file. 
                                 """)
-    summary_parser.add_argument("-o", "--output", type=str, required=True,
+    summary_parser.add_argument("-o", "--output", type=str, required=False,
                                 help="""
-                                Path to output a output directory or file. If a directory is given, the output 
-                                files are created using the basename from an input file with the suffix 
-                                "_summary.html". If plots --export_svg is set the exported 
-                                plots will be stored in the same directory as the HTML report.                                
+                                Path to output a output directory. The output files are created using the 
+                                basename from an input file with the suffix "_summary.html". If --export_svg 
+                                is set the exported plots will be stored in the same directory as the HTML report.
+                                If not specified, the files get written to the same directory as the input file.                             
                                 """)
     summary_parser.add_argument("-b", "--n_bins", type=int, required=False, default=5000,
-                                help="""Number of bins to split the data into when creating the summary report.
+                                help="""
+                                Number of bins to split the data into when creating the summary report.
                                 This only affects the plots, not the underlying feature table. Used to improve 
                                 performance and clarity of the created plots with many outliers. Note that 
                                 setting the value to a low number can lead to misleading plots. Set to "-1" 
                                 to disable binning. 
                                 Default: 5000
                                 """)
     summary_parser.add_argument("--plot_alt", action="store_true", 
@@ -152,29 +171,28 @@
                                 help="""
                                 Specify to export the created plots in SVG format. Files will be created in the
                                 output directory.
                                 """)
 
 
     # add parser for position-of-interest analyzer
-    poi_analyzer_parser = subparsers.add_parser("analyzepoi", 
+    poi_analyzer_parser = subparsers.add_parser("poisummary", 
                                                 help="""
-                                                    Analyze and explore specific positions of interest
+                                                    Summarize and explore features at specific positions of interest.
                                                     """)
     
     poi_analyzer_parser.add_argument("-i", "--input", type=str, required=True,
                                      help="""
                                      Path to the input file. Must be of type tsv, as returned by the PileupExtractor.
                                      """)
-    poi_analyzer_parser.add_argument("-o", "--output", type=str, required=True,
+    poi_analyzer_parser.add_argument("-o", "--output", type=str, required=False,
                                      help="""
-                                     Path to the output files or directory. If files are given, one path must
-                                     be provided for each bed-category that is given. If a directory is given
-                                     a summary file will be created for each given category named
-                                     "<category>_<input-basename>_summary.html".
+                                     Path to the output directory. A summary file will be created for each given 
+                                     category named "<category>_<input-basename>_poisummary.html".
+                                     If not specified, the files get written to the same directory as the input file.
                                      """)
     poi_analyzer_parser.add_argument("-b", "--bed", type=str, required=True,
                                      help="""
                                      Path to the bed file containing information in the fourth column.
                                      """)
     poi_analyzer_parser.add_argument("-r", "--ref", type=str, required=True,
                                      help="""
@@ -187,14 +205,29 @@
                                      """)
     poi_analyzer_parser.add_argument("-cc", "--counterparts", type=str, required=False, 
                                      help="""
                                      Canonical base corresponding to each category specified in --bed_categories. 
                                      Same format as --bed_categories flag. Enables comparisons between categories
                                      and counterparts.
                                      """)
+    poi_analyzer_parser.add_argument("-nm", "--bins_seqmap", type=int, required=False, default=200,
+                                     help="""
+                                     Number of bins for the sequence map plot. For a given value n, the corrdinates along each given
+                                     sequence is split into n chunks representing the a range of coordinates. Higher values correspond 
+                                     to a higher resolution of the given sequences. Default: 200
+                                     """)
+    poi_analyzer_parser.add_argument("-n", "--n_bins", type=int, required=False, default=5000,
+                                     help="""
+                                     Number of bins to split the data into when creating the summary report.
+                                     This only affects the plots, not the underlying feature table. Used to improve 
+                                     performance and clarity of the created plots with many outliers. Note that 
+                                     setting the value to a low number can lead to misleading plots. Set to "-1" 
+                                     to disable binning. 
+                                     Default: 5000
+                                     """)
     poi_analyzer_parser.add_argument("--update_tsv", action="store_true", 
                                      help="""
                                      If specified, creates an updated feature table (TSV) containing the 
                                      information from the name column in the bed file. Suffix "_w_bed_info.tsv" 
                                      will be added to newly created file.
                                      """)
     poi_analyzer_parser.add_argument("--use_mismatch_rate_alt", action="store_true", 
@@ -203,16 +236,126 @@
                                      """)
     poi_analyzer_parser.add_argument("--export_svg", action="store_true", 
                                      help="""
                                      Specify to export the created plots in SVG format. Files will be created in the
                                      output directory.
                                      """)
 
+    # add parser for position summary
+    poi_view_parser = subparsers.add_parser("poiview", 
+                                            help="""
+                                                Visualize base compositions and error rates at individual positions
+                                                between two conditions. 
+                                                """)
+    
+    poi_view_parser.add_argument("-i", "--sample1", type=str, required=True,
+                                 help="""
+                                    Path to the input file(s). If replicates are available, 
+                                    specify paths comma-separated (<repl1.tsv>,<repl2.tsv>,...).
+                                    Must be of type tsv, as returned by the PileupExtractor.
+                                    """)
+    poi_view_parser.add_argument("-bn", "--basename1", type=str, default="sample1",
+                                 help="""
+                                    Basename of the given sample.
+                                    Default: "sample1"
+                                    """)
+    poi_view_parser.add_argument("-i2", "--sample2", type=str, required=False,
+                                 help="""
+                                    Path to the input file(s) from a second sample. If replicates are available, 
+                                    specify paths comma-separated (<repl1.tsv>,<repl2.tsv>,...).
+                                    Must be of type tsv, as returned by the PileupExtractor. 
+                                    """)
+    poi_view_parser.add_argument("-bn2", "--basename2", type=str, default="sample2",
+                                 help="""
+                                    Basename of the second sample.
+                                    Default: "sample2"
+                                    """)
+    poi_view_parser.add_argument("-b", "--bed", type=str, required=True,
+                                 help="""
+                                    Path to the input BED file.
+                                    """)
+    poi_view_parser.add_argument("-o", "--output", type=str, required=False,
+                                 help="""
+                                    Path to output directory. The output file is created using the basenames from the input samples
+                                    as follows: <basename1>_<basename2>_<basename-bed-file>_view.html
+                                    If not specified, the files get written to the same directory as the input file.
+                                    """)
+    poi_view_parser.add_argument("-n", "--n_surrounding", type=hs.positive_int, required=False, default=2,
+                                 help="""
+                                    Number of neighbouring positions to consider when plotting a position X. 
+                                    In the created plots sites X-n, ..., X, ..., X+n are shown. 
+                                    Default: 2
+                                    """)
+    poi_view_parser.add_argument("--export_svg", action="store_true", 
+                                 help="""
+                                    Specify to export the created plots in SVG format. Files will be created in a directory of the 
+                                    following format: <output_dir>/<basename1>_<basename2>_<basename-bed-file>
+                                    For each position three plots will be created. The files will be named as follows:
+                                    <chromosome>_<coordinate>_<plot-type>.svg
+                                    """)
+
+    # add parser for POI comparison
+    poi_comparer_parser = subparsers.add_parser("poicompare", 
+                                               help="""
+                                                Statistically compare error rates and quality scores at positions of interest 
+                                                between two conditions. 
+                                                """)
+    
+    poi_comparer_parser.add_argument("-i", "--sample1", type=str, required=True,
+                                    help="""
+                                    Path to the input file of the first sample. Must be of type tsv, 
+                                    as returned by the PileupExtractor.
+                                    """)
+    poi_comparer_parser.add_argument("-bn", "--basename1", type=str, default="sample1",
+                                    help="""
+                                    Basename of the given sample. Default: "sample1"
+                                    """)
+    poi_comparer_parser.add_argument("-i2", "--sample2", type=str, required=True,
+                                    help="""
+                                    Path to the input file of the second sample. Must be of type tsv, 
+                                    as returned by the PileupExtractor.
+                                    """)
+    poi_comparer_parser.add_argument("-bn2", "--basename2", type=str, default="sample2",
+                                    help="""
+                                    Basename of the second sample. Default: "sample2"
+                                    """)
+    poi_comparer_parser.add_argument("-b", "--bed", type=str, required=True,
+                                    help="""
+                                    Path to the input BED file.
+                                    """)
+    poi_comparer_parser.add_argument("-o", "--output", type=str, required=False,
+                                    help="""
+                                    Path to output directory. The output file is created using the basenames from the input samples
+                                    as follows: <basename1>_<basename2>_<basename-bed-file>_statcompare.html
+                                    If not specified, the files get written to the same directory as the input file.
+                                    """)
+    poi_comparer_parser.add_argument("-n", "--n_surrounding", type=hs.positive_int, required=False, default=2,
+                                    help="""
+                                    Number of neighbouring positions to consider during testing. For a given value n, positions
+                                    X-n, ..., X, ..., X+n are tested for differences. Default: 2
+                                    """)
+    poi_comparer_parser.add_argument("-d", "--depth", type=hs.positive_int, required=False, default=15,
+                                    help="""
+                                    Number of reads at a given position to be valid for statistical testing. POIs with a depth under 
+                                    a given threshold are excluded from the analysis. Default: 15
+                                    """)
+    poi_comparer_parser.add_argument("-a", "--alpha", type=hs.float_between_zero_and_one, required=False, default=0.01,
+                                    help="""
+                                    Signifcance level used as a cutoff during statistical testing. Default: 0.01
+                                    """)
+    poi_comparer_parser.add_argument("--export_stat", action="store_true", 
+                                    help="""
+                                    Specify to export the results of the statistical tests in TSV format. The table is written
+                                    to the output directory (--output_dir) to the file 
+                                    '<output_dir>/<basename1>_<basename2>_<basename-bed-file>_statcompare.tsv'
+                                    It contains the columns feature, relative_position, p_value, fdr, neg_log10_fdr and test_used.
+                                    """)
+
     # add parser for two sample extractor
-    two_extractor_parser = subparsers.add_parser("twosample", 
+    two_extractor_parser = subparsers.add_parser("extractdiff", 
                                                  help="""
                                                     Extract positions of differential error rates between two samples.
                                                     """)
     
     two_extractor_parser.add_argument("-i", "--sample1", type=str, required=True,
                                       help="""
                                       Path to the input file(s). If replicates are available, specify paths 
@@ -233,112 +376,67 @@
                                       """)
     two_extractor_parser.add_argument("-bn2", "--basename2", type=str, default="sample2",
                                       help="""
                                       Basename of the second sample. Used to create the pileup and extracted 
                                       features files. 
                                       Default: "sample2"
                                       """)
-    two_extractor_parser.add_argument("-o", "--output", type=str, required=True,
+    two_extractor_parser.add_argument("-o", "--output", type=str, required=False,
                                       help="""
                                       Path to output a output directory, in which all output files will be stored.
                                       The following files will be created: "<basename>_<basename2>_summary.html", 
                                       "<basename>_<basename2>.bed", "<basename>_excl.bed", "<basename2>_excl.bed"
+                                      If not specified, the files get written to the same directory as the first input
+                                      file from sample 1.
                                       """)
     two_extractor_parser.add_argument("-r", "--ref", type=str, required=True, 
                                       help="""
                                       Path to the reference file in fasta format
                                       """)
-    two_extractor_parser.add_argument("-f", "--error_feature", type=str, default="mismatch_rate_alt", 
+    two_extractor_parser.add_argument("-f", "--error_feature", type=str, default="mismatch_alt", 
                                       help="""
                                       Error feature to use during extraction. Can be one of the following: 
-                                      deletion_rate, insertion_rate, mismatch_rate, mismatch_rate_alt. 
-                                      Default: "mismatch_rate_alt"
+                                      deletion, insertion, mismatch, mismatch_alt. 
+                                      Default: "mismatch_alt"
                                       """)
     two_extractor_parser.add_argument("-e", "--error_threshold", type=hs.float_between_zero_and_one, default=0.5, 
                                       help="""
                                       Threshold to identify positions of iterest. Uses the mismatch_rate_alt feature. 
                                       Default: 0.5
                                       """)
     two_extractor_parser.add_argument("-c", "--coverage_threshold", type=hs.positive_int, default=40,
                                       help="""
                                       Minimum coverage of a position to be regarded in the extraction. 
                                       Default: 40
                                       """)
+    two_extractor_parser.add_argument("-nm", "--bins_seqmap", type=int, required=False, default=200,
+                                     help="""
+                                     Number of bins for the sequence map plot. For a given value n, the corrdinates along each given
+                                     sequence is split into n chunks representing the a range of coordinates. Higher values correspond 
+                                     to a higher resolution of the given sequences. Default: 200
+                                     """)
     two_extractor_parser.add_argument("--export_svg", action="store_true", 
                                       help="""
                                       Specify to export the created plots in SVG format. Files will be created in the
                                       output directory.
                                       """)
 
-    # add parser for position summary
-    pos_summary_parser = subparsers.add_parser("possummary", 
-                                               help="""
-                                                Visualize base compositions and error rates at individual positions
-                                                between two conditions. 
-                                                """)
-    
-    pos_summary_parser.add_argument("-i", "--sample1", type=str, required=True,
-                                    help="""
-                                    Path to the input file(s). If replicates are available, 
-                                    specify paths comma-separated (<repl1.tsv>,<repl2.tsv>,...).
-                                    Must be of type tsv, as returned by the PileupExtractor.
-                                    """)
-    pos_summary_parser.add_argument("-bn", "--basename1", type=str, default="sample1",
-                                    help="""
-                                    Basename of the given sample.
-                                    Default: "sample1"
-                                    """)
-    pos_summary_parser.add_argument("-i2", "--sample2", type=str, required=True,
-                                    help="""
-                                    Path to the input file(s) from a second sample. If replicates are available, 
-                                    specify paths comma-separated (<repl1.tsv>,<repl2.tsv>,...).
-                                    Must be of type tsv, as returned by the PileupExtractor. 
-                                    """)
-    pos_summary_parser.add_argument("-bn2", "--basename2", type=str, default="sample2",
-                                    help="""
-                                    Basename of the second sample.
-                                    Default: "sample2"
-                                    """)
-    pos_summary_parser.add_argument("-b", "--bed", type=str, required=True,
-                                    help="""
-                                    Path to the input BED file.
-                                    """)
-    pos_summary_parser.add_argument("-o", "--output_dir", type=str, required=True,
-                                    help="""
-                                    Path to output directory. The output file is created using the basenames from the input samples
-                                    as follows: <basename1>_<basename2>_<basename-bed-file>_summary.html
-                                    """)
-    pos_summary_parser.add_argument("-n", "--n_surrounding", type=hs.positive_int, required=False, default=2,
-                                    help="""
-                                    Number of neighbouring positions to consider when plotting a position X. 
-                                    In the created plots sites X-n, ..., X, ..., X+n are shown. 
-                                    Default: 2
-                                    """)
-    pos_summary_parser.add_argument("--export_svg", action="store_true", 
-                                    help="""
-                                    Specify to export the created plots in SVG format. Files will be created in a directory of the 
-                                    following format: <output_dir>/<basename1>_<basename2>_<basename-bed-file>
-                                    For each position three plots will be created. The files will be named as follows:
-                                    <chromosome>_<coordinate>_<plot-type>.svg
-                                    """)
-
-    
     # add parser for filtering
     filter_parser = subparsers.add_parser("filter", 
                                           help="""
                                             Filter a feature table on one or more features.
                                             """)
     
     filter_parser.add_argument("-i", "--input", type=str, required=True,
                                help="Path to input TSV file.")
-    filter_parser.add_argument("-o", "--output", type=str, required=True,
+    filter_parser.add_argument("-o", "--output", type=str, required=False,
                                help="""
-                               Path to output TSV file or directory. If a directory is given
-                               writes the output file with the basename of the input file
-                               + "_filtered".
+                               Path to output directory. Writes the output file with the basename of the input file
+                               and the suffix "_filtered". If not specified, the files get written to the same directory 
+                               as the first input file.
                                """)
     filter_parser.add_argument("-c", "--chromosome", type=str, required=False,
                                help="Filter by given chromosome.")
     filter_parser.add_argument("-s", "--site", type=str, required=False,
                                help="""
                                Filter by given site(s) or range. For single site: "x"; 
                                for multiple sites: "x,y,z,..."; for range: "x-y"
@@ -449,105 +547,122 @@
     difference_parser.add_argument("-i1", "--input1", type=str, required=True,
                                    help="Path to bed file 1")
     difference_parser.add_argument("-i2", "--input2", type=str, required=True,
                                    help="Path to bed file 2")
     difference_parser.add_argument("-o", "--output", type=str, required=True,
                                    help="Path to the output file")
 
-
     return parser, bedops_parser
 
-def main():
+def main() -> None:
 
     parser, bedops_parser = setup_parsers()
     args = parser.parse_args()
 
     if args.subcommand == "extractor":
         print_figlet("NEET - Pileup Extractor")
         feature_extractor = FeatureExtractor(in_paths=args.input, 
-                                             out_paths=args.output, 
+                                             out_dir=args.output, 
                                              ref_path=args.ref,
                                              num_reads=args.num_reads, 
                                              mismatch_rate=args.mismatch_rate,
                                              mismatch_rate_alt=args.mismatch_rate_alt,
                                              perc_deletion=args.perc_deletion,
                                              mean_quality=args.mean_quality,
                                              genomic_region=args.genomic_region,
-                                             use_multiprocessing=args.use_multiprocessing,
-                                             num_processes=args.num_processes,
                                              window_size=args.window_size,
                                              neighbour_error_threshold=args.neighbour_thresh,
-                                             n_bins_summary = args.n_bins,
-                                             use_alt_summary=args.plot_alt,
-                                             export_svg_summary=args.export_svg)
+                                             no_summary=args.no_summary,
+                                             num_processes=args.num_processes,
+                                             queue_size=args.queue_size,
+                                             temp_file_line_count=args.temp_size,
+                                             logging_level=args.log_level,
+                                             log_path=args.log_file)
         feature_extractor.main()
 
     elif args.subcommand == "summary":
         print_figlet("NEET - Summary")
         summary = SummaryCreator(in_path=args.input, 
                                  out_path=args.output, 
                                  n_bins=args.n_bins, 
                                  use_perc_mismatch_alt=args.plot_alt, 
                                  export_svg=args.export_svg,)
         summary.main()
 
-    elif args.subcommand == "analyzepoi":
-        print_figlet("NEET - Position-of-Interest Analyzer")
-        poi_analyzer = POIAnalyzer(in_path=args.input,
-                                   out_path=args.output,
-                                   bed_path=args.bed,
-                                   ref_path=args.ref,
-                                   categories=args.bed_categories,
-                                   canonical_counterpart=args.counterparts,
-                                   output_tsv=args.update_tsv,
-                                   use_perc_mismatch_alt=args.use_mismatch_rate_alt,
-                                   export_svg=args.export_svg)
+    elif args.subcommand == "poisummary":
+        print_figlet("NEET - POI Summary")
+        poi_analyzer = POISummary(in_path=args.input,
+                                  out_dir=args.output,
+                                  bed_path=args.bed,
+                                  ref_path=args.ref,
+                                  categories=args.bed_categories,
+                                  canonical_counterpart=args.counterparts,
+                                  output_tsv=args.update_tsv,
+                                  use_perc_mismatch_alt=args.use_mismatch_rate_alt,
+                                  export_svg=args.export_svg,
+                                  n_bins_seqmap=args.bins_seqmap,
+                                  n_bins=args.n_bins)
         poi_analyzer.main()
 
-    elif args.subcommand == "twosample":
+    elif args.subcommand == "poiview":
+        print_figlet("NEET - POI View")
+        pos_summary = POIView(paths_a = args.sample1,
+                              paths_b = args.sample2,
+                              basename_a = args.basename1,
+                              basename_b = args.basename2,
+                              bed_path = args.bed,
+                              out_dir = args.output,
+                              nb_size = args.n_surrounding,
+                              export_svg=args.export_svg)
+        pos_summary.main() 
+    
+    elif args.subcommand == "poicompare":
+        print_figlet("NEET - POI Comparison")
+        poi_compare = PoiSampleComparer(path_a = args.sample1,
+                                        path_b = args.sample2,
+                                        basename_a = args.basename1,
+                                        basename_b = args.basename2,
+                                        bed_path = args.bed,
+                                        out_dir = args.output,
+                                        num_neighbours = args.n_surrounding,
+                                        n_reads_threshold = args.depth,
+                                        alpha = args.alpha,
+                                        store_stat = args.export_stat)
+        poi_compare.main()
+
+    elif args.subcommand == "extractdiff":
         print_figlet("NEET - Two-Sample Extractor")
         posextr = PositionExtractor(in_paths_a=args.sample1, 
                                     in_paths_b=args.sample2, 
                                     out_dir=args.output, 
                                     ref_path=args.ref, 
                                     label_a=args.basename1, 
                                     label_b=args.basename2, 
                                     error_feature=args.error_feature,
                                     error_threshold=args.error_threshold, 
                                     coverage_threshold=args.coverage_threshold,
+                                    n_bins_seqmap=args.bins_seqmap,
                                     export_svg=args.export_svg)
         posextr.main()
 
-    elif args.subcommand == "possummary":
-        print_figlet("NEET - Position Summary")
-        pos_summary = PositionSummary(paths_a = args.sample1,
-                                      paths_b = args.sample2,
-                                      basename_a = args.basename1,
-                                      basename_b = args.basename2,
-                                      bed_path = args.bed,
-                                      out_path = args.output_dir,
-                                      nb_size = args.n_surrounding,
-                                      export_svg=args.export_svg)
-        pos_summary.main() 
-    
     elif args.subcommand == "filter":
         print_figlet("NEET - Filter")
         filter = Filter(input_path=args.input,
-                        output_path=args.output,
+                        out_dir=args.output,
                         chrom=args.chromosome,
                         site=args.site,
                         n_reads=args.n_reads,
                         base=args.base,
                         mismatched=args.mismatched,
                         mismatch_types=args.mismatch_types,
-                        perc_mismatched=args.percent_mismatched,
+                        perc_mismatched=args.mismatch_rate,
                         perc_mismatched_alt=args.mismatch_rate_alt,
-                        perc_deletion=args.percent_deletion,
-                        perc_insertion=args.percent_insertion,
-                        perc_refskip=args.percent_refskip,
+                        perc_deletion=args.deletion_rate,
+                        perc_insertion=args.insertion_rate,
+                        perc_refskip=args.refskip_rate,
                         motif=args.motif,
                         q_score=args.q_score,
                         bed_include=args.filter_bed,
                         bed_exclude=args.exclude_bed)
         filter.main()
     
     elif args.subcommand == "bedops":
```

### Comparing `neet-nanopore-0.0.4/neet/bed_ops.py` & `neet_nanopore-1.0.0/neet/bed_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,16 @@
-import argparse, os, csv
-from typing import List, Tuple, Dict
-from . import helper_functions as hs
+import csv
+from typing import Tuple, Dict
 from tqdm import tqdm
 
+try: # when invoked from the package
+    from neet import helper_functions as hs
+except ImportError: # when invoked directly
+    import helper_functions as hs
+
 def tsv_to_bed(in_path: str, out_path: str) -> None:
     """
     Converts a TSV (Tab-Separated Values) file to a BED (Browser Extensible Data) file format.
 
     Args:
         in_path (str): Path to the input TSV file.
         out_path (str): Path to the output BED file.
```

### Comparing `neet-nanopore-0.0.4/neet/filter.py` & `neet_nanopore-1.0.0/neet/filter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-import argparse, io, sys, re
-from . import helper_functions as hs
+import re
 from typing import List, Tuple, Callable
 from tqdm import tqdm
 import os
 
+try: # when invoked from the package
+    from neet import helper_functions as hs
+except ImportError: # when invoked directly
+    import helper_functions as hs
+
 class Filter:
     """
     Class for filtering TSV files based on specified criteria.
 
     Attributes:
         input_path (str): Path to the input TSV file.
         output_path (str): Path to the output TSV file.
@@ -62,30 +66,30 @@
         ">": lambda x, y: x > y,
         ">=": lambda x, y: x >= y,
         "==": lambda x, y: x == y
         }
 
     def __init__(self, 
                  input_path: str, 
-                 output_path: str, 
                  chrom: str, 
                  site: str,
                  n_reads: str, 
                  base: str, 
                  mismatched: bool, 
                  mismatch_types: str,
                  perc_mismatched: str, 
                  perc_mismatched_alt: str,
                  perc_deletion: str,
                  perc_insertion: str,
                  perc_refskip: str,
                  motif: str, 
                  q_score: str,
                  bed_include: str | None,
-                 bed_exclude: str | None) -> None:
+                 bed_exclude: str | None,
+                 out_dir: str | None = None) -> None:
         """
         Initializes the Filter object.
 
         Args:
             input_path (str): Path to the input TSV file.
             output_path (str): Path to the output TSV file.
             chrom (str): Filter by chromosome.
@@ -94,16 +98,26 @@
             base (str): Filter by reference base(s).
             mismatched (bool): Filter mismatched positions.
             perc_mismatched (str): Filter by percent of mismatched reads.
             motif (str): Filter by motif around position.
             q_score (str): Filter by mean quality.
         """
         hs.check_input_path(input_path, extensions=[".tsv"])
-        self.input_path = input_path
-        self.output_path = hs.process_outpath(output_path, f"{os.path.splitext(os.path.basename(input_path))[0]}_filtered.tsv", [".tsv"])
+        self.input_path = os.path.abspath(input_path)
+
+        if out_dir:
+            out_dir = os.path.abspath(out_dir)
+            ext = os.path.splitext(out_dir)[1]
+            if ext:
+                hs.print_update(f"Warning: Extension {ext} was found. Make sure to provide a single output directory.")
+            hs.check_create_dir(out_dir)
+            filename = f"{os.path.splitext(os.path.basename(self.input_path))[0]}_filtered.tsv"
+            self.output_path = os.path.join(out_dir, filename)
+        else:
+            self.output_path = f"{os.path.splitext(self.input_path)[0]}_filtered.tsv"
 
         self.chrom = chrom
         self.site = self.get_sites(site)
         self.n_reads = self.get_n_reads(n_reads)
         self.base = self.get_bases(base)
         self.mismatched = mismatched
         self.mismatch_types = self.get_mismatch_types(mismatch_types)
@@ -173,25 +187,26 @@
 
         Raises:
             Exception: If the string does not match any of the supported formats.
         """
         if n_reads_str is None:
             return None
         try:
+            # if only a number is specified, it is assumed that the filter is >=NUM
             value = int(n_reads_str)
             fun = self.OPERATORS.get(">=")
         except:
             match = re.match(r'([<>]=?|==)(\d+)', n_reads_str)
             if match:
                 value = int(match.group(2))
                 op = match.group(1)
                 fun = self.OPERATORS.get(op)
             else:
                 raise Exception(f"Could not extract information from given string '{n_reads_str}'")
-        return value, fun
+        return value, fun # type: ignore
     
     def get_bases(self, base_str: str) -> List[str]|None:
         """
         Extracts the bases from the given string.
 
         Args:
             base_str (str): The string representing the bases.
@@ -268,15 +283,15 @@
             match = re.match(r'([<>]=?|==)(\d+\.?\d*)', string)
             if match:
                 val = float(match.group(2))
                 op = match.group(1)
                 fun = self.OPERATORS.get(op)
             else:
                 raise Exception(f"Could not extract information from given string '{string}'")
-        return val, fun
+        return val, fun # type: ignore
 
     def get_bed_positions(self, bed_path: str) -> set[Tuple[str, int]]:
         """
         Retrieves genomic positions from a BED file.
 
         This method reads a BED (Browser Extensible Data) file containing genomic
         position information and returns a set of tuples, where each tuple represents
@@ -362,15 +377,15 @@
         q_score = float(row[22])
 
         if self.chrom:
             if chrom != self.chrom: return False
         if self.site: 
             if site not in self.site: return False
         if self.n_reads:
-            if not check_func(n_reads, self.n_reads): return False
+            if not check_func(n_reads, self.n_reads): return False # type: ignore
         if self.base:
             if ref_base not in self.base: return False
         if self.mismatched:
             if maj_base == ref_base: return False
         if self.mismatch_types:
             for mismatch_type in self.mismatch_types:
                 if (ref_base!=mismatch_type[0]) | (maj_base!=mismatch_type[1]):
```

### Comparing `neet-nanopore-0.0.4/neet/pileup_extractor.py` & `neet_nanopore-1.0.0/neet/poi_sample_comparer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,768 +1,531 @@
-import re, os, warnings, argparse, sys, io, random
-from typing import Dict, List, Tuple, Union, Any
+import os
+import plotly.graph_objects as go
+from collections import defaultdict
+from typing import List, Dict, Tuple, Any
+from scipy.stats import ttest_rel, wilcoxon, normaltest, bartlett
+from statsmodels.stats.multitest import fdrcorrection
+from math import log10
 from tqdm import tqdm
-import numpy as np
-from multiprocessing import Pool
-from . import helper_functions as hs
-from .summary import SummaryCreator
-class FeatureExtractor:
-
-    input_paths : List[str]
-    output_paths : List[str]
-    ref_path : str
-    ref_sequences : Dict[str, str]
-    
-    filter_num_reads: int
-    filter_perc_mismatch: float
-    filter_perc_mismatch_alt: float
-    filter_mean_quality: float
-    filter_genomic_region: Tuple[str, int, int] | None
-    num_processes: int
-    window_size: int
-    neighbour_error_threshold: float
-    n_bins_summary: int|None
-    use_alt_summary: bool
-
-    def __init__(self, 
-                 in_paths: str,
-                 out_paths: str, 
-                 ref_path: str,
-                 num_reads: int, 
-                 mismatch_rate: float | None,
-                 mismatch_rate_alt: float | None,
-                 perc_deletion: float | None,
-                 mean_quality: float | None,
-                 genomic_region: str | None,
-                 use_multiprocessing: bool,
-                 num_processes: int,
-                 window_size: int,
-                 neighbour_error_threshold: float,
-                 n_bins_summary: int,
-                 use_alt_summary: bool,
-                 export_svg_summary: bool) -> None:
-
-        self.process_paths(ref_path, in_paths, out_paths)    
-
-        # if one of the following arguments was not provided (i.e. arg=None), set variable to a value so nothing gets filtered out
-        self.filter_num_reads = num_reads if num_reads is not None else 1
-        self.filter_perc_mismatch = mismatch_rate if mismatch_rate else 0
-        self.filter_perc_mismatch_alt = mismatch_rate_alt if mismatch_rate_alt else 0
-        self.filter_perc_deletion = perc_deletion if perc_deletion else 0
-        self.filter_mean_quality = mean_quality if mean_quality else 0
-        self.filter_genomic_region = self.extract_positional_info(genomic_region) if genomic_region else None
-
-        self.use_multiprocessing = use_multiprocessing
-        self.num_processes = num_processes
-
-        self.window_size = window_size
-        self.neighbour_error_threshold = neighbour_error_threshold
-
-        self.n_bins_summary = n_bins_summary if n_bins_summary > 0 else None 
-        self.use_alt_summary = use_alt_summary
-        self.export_svg_summary = export_svg_summary
-
-    def __str__(self) -> str:
-        return ""
-
-
-    #################################################################################################################
-    #                                   Functions called during initialization                                      #
-    #################################################################################################################
-
-    def process_paths(self, ref_path: str, in_paths_str: str, out_paths: str) -> None:
-        """
-        Process input and output file paths for the data processing.
-
-        This method processes the file paths provided for reference sequence, input data,
-        and output data. It checks the validity of the paths and stores the processed
-        information in the respective instance variables.
-
-        Parameters:
-            ref_path (str): The file path to the reference fasta file.
-            in_paths (str): Comma-separated list of input file paths.
-            out_paths (str): Output file path or directory path.
 
-        Returns:
-            None
-
-        Raises:
-            FileNotFoundError: If the reference file or any of the input files do not exist.
-            Warning: If the file extension of any input file is not among the expected extensions.
-
-        Note:
-            - The reference fasta file should have one or more sequence entries in the format:
-            >chromosome_name description(optional)
-            sequence
-            - The input files are expected to have specific extensions (e.g., '.msf', '.pup', '.pileup').
-            - The output files will be generated with the '.tsv' extension.
-        """
-        # process input path(s)
-        in_paths = in_paths_str.split(",")
-        for path in in_paths: hs.check_input_path(path, [".msf", ".pup", ".pileup"])
-        self.input_paths = in_paths
-
-        # process output path(s)
-        self.output_paths = self.process_outpaths(out_paths)
-
-        # process path to reference fasta
-        hs.check_input_path(ref_path, [".fasta", ".fna", ".ffn", ".faa", ".frn", ".fa"])
-        self.ref_sequences = hs.get_references(ref_path)
-
-    def process_outpaths(self, out: str) -> List[str]:
-        """
-        Process the output file paths based on the input `out` argument.
-
-        Args:
-            out (str): The output file path or directory path. If set to "-", no output file paths
-                    will be generated, and the function will return `None`. If `out` is a
-                    directory path, output file paths will be generated using the input file
-                    names with the `.tsv` extension appended. If `out` is a comma-separated list
-                    of filenames, the function will verify if the specified files exist and if
-                    their extensions are `.tsv`.
-
-        Returns:
-            List[str] | None: A list of output file paths if `out` is a directory path or a
-                            comma-separated list of filenames. If `out` is set to "-", the
-                            function returns `None`.
-
-        Raises:
-            FileNotFoundError: If `out` is a directory path, and the directory does not exist.
-                            If `out` is a list of filenames, and the directory of any file
-                            does not exist.
-            UserWarning: If any filename in the list has an extension other than `.tsv`, a
-                        user warning will be issued to inform the user that the output file
-                        will be of type `.tsv`.
-        """
-        out_paths = out.split(",")
-        if len(out_paths) > 1:
-            for path in out_paths:
-                hs.check_create_dir(os.path.dirname(path))
-                file_extension = os.path.splitext(path)[1]
-                if file_extension != ".tsv":
-                    warnings.warn(f"Given output file has extension '{file_extension}'. Note that the output file will be of type '.tsv'.")
+try: # when invoked from the package
+    from neet import helper_functions as hs
+except ImportError: # when invoked directly
+    import helper_functions as hs
+
+SITE = Tuple[str, int]
+SAMPLE = str
+FEATURE = str
+
+class PoiSampleComparer:
+    in_path_a: str
+    in_path_b: str
+    bed_path: str
+    basename_a: str
+    basename_b: str
+    out_dir: str
+    num_neighbours: int
+    n_reads_threshold: int
+    alpha: float
+    store_stat: bool
+
+    poi_sites: Dict[SITE, List[SITE]]
+    data: Dict[SAMPLE, Dict[SITE, Dict[FEATURE, Any]|None]] # Any one of int, str, float; None if a site is not found
+    poi_sites_usable: Dict[SITE, List[SITE]] # containing only the sites that are available and sufficiently covered (as indentified in in self.get_usable_pois)
+
+    def __init__(self, path_a: str, path_b: str, bed_path: str,
+                 out_dir: str | None = None,
+                 basename_a: str = "sample_a", 
+                 basename_b: str = "sample_a", 
+                 num_neighbours: int = 2, 
+                 n_reads_threshold: int = 15, 
+                 alpha: float = 0.01, 
+                 store_stat: bool = False) -> None:
+        
+        hs.check_input_path(path_a, extensions=[".tsv"])
+        self.in_path_a = os.path.abspath(path_a)
+        hs.check_input_path(path_b, extensions=[".tsv"])
+        self.in_path_b = os.path.abspath(path_b)
+
+        hs.check_input_path(bed_path, extensions=[".bed"])
+        self.bed_path = os.path.abspath(bed_path)
+
+        if not basename_a:
+            raise Exception(f"Given basename for sample a '{basename_a}' is not valid.")
+        elif not basename_b:
+            raise Exception(f"Given basename for sample b '{basename_b}' is not valid.")
+        elif basename_a == basename_b:
+            raise Exception(f"Basenames '{basename_a}' and '{basename_b}' must differ from each other.")
+        self.basename_a = basename_a
+        self.basename_b = basename_b
+
+        if out_dir:
+            out_dir = os.path.abspath(out_dir)
+            ext = os.path.splitext(out_dir)[1]
+            if ext:
+                hs.print_update(f"Warning: Extension {ext} was found. Make sure to provide a single output directory.")
+            hs.check_create_dir(out_dir)
+            self.out_dir = out_dir
         else: 
-            hs.check_create_dir(out)
-            out_paths = []
-            for in_path in self.input_paths:
-                basename = os.path.splitext(os.path.basename(in_path))[0]
-                out_paths.append(os.path.join(out, f"{basename}_extracted.tsv"))
-        return out_paths
-
-    def extract_positional_info(self, data_string: str) -> Tuple[str, int, int] | None:
-        """
-        Extracts the chromosome name, start value, and end value from a string in the format "chromosome_name:start-end".
-
-        Parameters
-        ----------
-        data_string : str
-            The input string in the format "chromosome_name:start-end".
-
-        Returns
-        -------
-        tuple
-            A tuple containing the chromosome name (str), start value (int), and end value (int).
-        """
-        if (":" in data_string) & ("-" in data_string): 
-            chromosome, positions = data_string.split(':')
-            start_str, end_str = positions.split('-')
-            start = int(start_str.replace(',', ''))
-            end = int(end_str.replace(',', ''))
-        else:
-            chromosome = data_string
-            start = 1
-            end = len(self.ref_sequences[chromosome])
+            self.out_dir = os.path.dirname(self.in_path_a)
 
-        if self.region_is_valid(chromosome, start, end):
-            return chromosome, start, end
-    
-    def region_is_valid(self, chr, start, end) -> bool:
-        """
-        Checks if the chromosome is found in the reference sequences and if so, whether the given start and end
-        coordinates are in range of the corresponding sequence.
+        if num_neighbours <= 0:
+            raise Exception(f"Number of neighbours must be larger than 0. Given number: {num_neighbours}")
+        self.num_neighbours = num_neighbours
+
+        if n_reads_threshold <= 0:
+            raise Exception(f"Threshold for the number of reads must be larger than 0. Given number: {n_reads_threshold}")
+        self.n_reads_threshold = n_reads_threshold
+
+        if (alpha < 0) | (alpha > 1):
+            raise Exception(f"Alpha must be in range (0,1). Given number: {alpha}")
+        self.alpha = alpha
+
+        self.store_stat = store_stat
+
+        # load data
+        hs.print_update(f"Loading POIs from {bed_path}.")
+        self.load_bed_sites(bed_path)
+        hs.print_update(f"Loading data from {path_a}.")
+        data_a = self.load_data(path_a)
+        hs.print_update(f"Loading data from {path_b}.")
+        data_b = self.load_data(path_b)
+        # self.data: nested dict with 1. samples, 2. POI site, 3. feature 
+        self.data = {basename_a: data_a, basename_b: data_b}
+
+    ##############################################################################################################
+    #                                           Initialization methods                                           #
+    ##############################################################################################################
 
-        Parameters
-        ----------
-        pos_info : Tuple[str, int, int]
-            Positional information extracted in self.extract_positional_info()
-
-        Returns
-        -------
-        bool
-            True, if all information is valid
-
-        Raises
-        ------
-        Exception, if not all information is valid. 
-        """
-        # check if chromosome name is found in self.ref_sequences
-        if chr not in list(self.ref_sequences.keys()):
-            raise Exception(f"Chromosome region error: Name '{chr}' not found in reference sequences from file '{self.ref_path}'")
-        # check if start < end
-        if start >= end:
-            raise Exception(f"Chromosome region error: End position {end} must be larger than start position {start}.")
-        # check if start is in range
-        chr_len = len(self.ref_sequences[chr])
-        if start <= 0 or start > chr_len:
-            raise Exception(f"Chromosome region error: Start position {start} not in range of corrdinates 1-{chr_len} (both incl.).")
-        # check if end is in range
-        if end <= 0 or end > chr_len:
-            raise Exception(f"Chromosome region error: End position {end} not in range of corrdinates 1-{chr_len} (both incl.).")
-        return True
-
-
-    #################################################################################################################
-    #                                  Functions called during feature extraction                                   #
-    #################################################################################################################
-    def main(self) -> None:
+    def load_bed_sites(self, bed_path):
         """
-        Process multiple pairs of input and output files. Reads .pileup files and processes them in parallel using multiprocessing.
+        Loads positions of interest (POIs) and their neighboring sites from the provided BED file.
 
-        Returns:
-            None
-        """ 
-        for in_file, out_file in zip(self.input_paths, self.output_paths):
-            hs.print_update(f"Processing file '{in_file}'. Writing to '{out_file}'.")
-            self.process_file(in_file, out_file)
-            self.create_summary_file(out_file)
-
-    def process_file(self, in_file: str, out_file: str) -> None:
-        """
-        Reads a .pileup file, processes it in a sliding window to incorporate the neighbourhood search,
-        and writes the results to a new file.
-
-        Parameters
-        ----------
-        in_file : str
-            Path to the input .pileup file.
-        out_file : str
-            Path to the output tsv file.
-
-        Returns
-        -------
-        None
-        """  
-
-        def write_edge_lines(neighbourhood: List[str], outfile: io.TextIOWrapper, start: bool = True):
-            """
-            Writes the neighbourhood information for the first or last rows as returned by the process_edge method.
-
-            Args:
-                neighbourhood: A list of lines representing the current neighbourhood.
-                outfile: The output file to write the edge lines to.
-                start: A boolean indicating if it's the start or end of the neighbourhood.
-
-            Returns:
-                None
-            """
-            k = self.window_size
-            r = range(k) if start else range(k+1, 2*k+1)
-            for current_pos in r:
-                outline = self.process_edge(current_pos, neighbourhood, start)
-                outfile.write(outline)
-
-        def write_center_line(neighbourhood: List[str], outfile: io.TextIOWrapper):
-            """
-            Writes the neighbourhood information for the center position of a full-sized neighbourhood.
-
-            Args:
-                neighbourhood: A list of lines representing the current neighbourhood.
-                outfile: The output file to write the edge lines to.
-
-            Returns:
-                None
-            """
-            outline = self.process_neighbourhood(neighbourhood)
-            outfile.write(outline)
-
-        with open(in_file, "r") as i, open(out_file, "w") as o:
-            desc = "Processing pileup rows"
-            hs.print_update("Counting number of lines to process.")
-            progress_bar = tqdm(desc=desc, total=hs.get_num_lines(in_file))
-
-            header = f"chr\tsite\tn_reads\tref_base\tmajority_base\tn_a\tn_c\tn_g\tn_u\tn_del\tn_ins\tn_ref_skip\ta_rate\tc_rate\tg_rate\tu_rate\tdeletion_rate\tinsertion_rate\trefskip_rate\tmismatch_rate\tmismatch_rate_alt\tmotif\tq_mean\tq_std\tneighbour_error_pos\n"
-            o.write(header)
-            
-            nb_size_full = 1 + 2 * self.window_size
-            nb_lines = []
-            nb_first = True
-
-            if self.use_multiprocessing:
-                with Pool(processes=self.num_processes) as pool:
-                    for outline in pool.imap(self.process_position, i):
-                        if len(outline) > 0: 
-                            nb_lines.append(outline)
-
-                            if len(nb_lines) > nb_size_full:  
-                                nb_lines.pop(0)
-
-                            if len(nb_lines) == nb_size_full:
-                                if nb_first:
-                                    nb_first = False
-                                    write_edge_lines(nb_lines, o, start=True)
-                                write_center_line(nb_lines, o)
-                        progress_bar.update()
-            else:
-                for line in i:
-                    outline = self.process_position(line) # extracting the features themselves
-                    if len(outline) > 0: 
-                        nb_lines.append(outline)
-
-                        if len(nb_lines) > nb_size_full:  
-                            nb_lines.pop(0)
-
-                        if len(nb_lines) == nb_size_full:
-                            if nb_first:
-                                nb_first = False
-                                write_edge_lines(nb_lines, o, start=True)
-                            write_center_line(nb_lines, o)
-                    progress_bar.update()
-
-            if len(nb_lines) < nb_size_full:
-                for current_pos in range(len(nb_lines)):
-                    outline = self.process_small(current_pos, nb_lines)
-                    o.write(outline)
-            else:
-                write_edge_lines(nb_lines, o, start=False)
+        Parameters:
+        - bed_path (str): The file path to the BED file containing POIs.
 
-            progress_bar.update()
-            progress_bar.close()
+        Notes:
+            The BED file is expected to be tab-delimited with three columns: chromosome, start position, and end position.
+            Only the chromosome and end position are used to define POIs, and the start position is ignored.
+            Neighboring sites are defined as the specified number of bases up- and downstream from each POI.
+            The neighboring sites are stored in the 'poi_sites' attribute as a dictionary with POI sites as keys
+            and lists of neighboring sites as values.
+        """
+        with open(bed_path, "r") as f:
+            center_sites = []
+            for line in f:
+                line = line.strip().split("\t")
+                seq, site = line[0], int(line[2])
+                center_sites.append((seq,site))
+        center_sites = set(center_sites)
+        all_sites = {}
+        for site in center_sites:
+            all_sites[site] = [(site[0], site[1]+i) for i in range(-self.num_neighbours,self.num_neighbours+1)]
+        
+        self.poi_sites = all_sites
 
-    def create_summary_file(self, file_path: str) -> None:
+    def load_data(self, input_path) -> Dict[SITE, Dict[str, Any]|None]:
         """
-        Create a summary file from the newly created tsv file.
+        Loads genomic data from the specified input file and organizes it into a dictionary.
 
         Parameters:
-            file_path (str): Path to the newly created tsv output.
+        - input_path (str): The file path to the input genomic data file.
 
         Returns:
-            None
+        Dict[Tuple[str, int], Dict[str, Any]|None]: A nested dictionary containing genomic data for each POI.
+            - The outer dictionary's keys are tuples representing POI sites (chromosome, position).
+            - The inner dictionary contains genomic data for each POI, with keys representing different features.
+
+        Notes:
+        - The input file is expected to be a feature table created by the Pileup Extractor.
+        - Missing data for a POI (if any) will be represented as None in the inner dictionary.
         """
-        out_path = os.path.splitext(file_path)[0]+"_summary.html"
-        summary_creator = SummaryCreator(file_path, out_path, n_bins=self.n_bins_summary, 
-                                         use_perc_mismatch_alt=self.use_alt_summary,
-                                         export_svg=self.export_svg_summary)
-        summary_creator.main()
+        cols = ["n_reads", "ref_base", "majority_base", "deletion_rate", "insertion_rate", "refskip_rate", "mismatch_rate", "q_mean", "motif"]
+
+        col_idx = {'chr': 0, 'site': 1, 'n_reads': 2, 'ref_base': 3, 'majority_base': 4, 'n_a': 5, 'n_c': 6, 'n_g': 7, 'n_t': 8, 'n_del': 9, 'n_ins': 10, 'n_ref_skip': 11, 'a_rate': 12, 'c_rate': 13, 'g_rate': 14, 'u_rate': 15, 'deletion_rate': 16, 'insertion_rate': 17, 'refskip_rate': 18, 'mismatch_rate': 19, 'mismatch_rate_alt': 20, 'motif': 21, 'q_mean': 22, 'q_std': 23, 'neighbour_error_pos': 24}
+        dtypes = {'chr': str, 'site': int, 'n_reads': int, 'ref_base': str, 'majority_base': str, 'n_a': int, 'n_c': int, 'n_g': int, 'n_t': int, 'n_del': int, 'n_ins': int, 'n_ref_skip': int, 'a_rate': float, 'c_rate': float, 'g_rate': float, 'u_rate': float, 'deletion_rate': float, 'insertion_rate': float, 'refskip_rate': float, 'mismatch_rate': float, 'mismatch_rate_alt': float, 'motif': str, 'q_mean': float, 'q_std': float, 'neighbour_error_pos': str}
+        
+        poi_sites = []
+        for sites in self.poi_sites.values():
+            poi_sites += sites
+        data = dict(zip(poi_sites, [None]*len(poi_sites)))
+        
+        n_lines = hs.get_num_lines(input_path)
 
-    def process_position(self, line_str: str) -> str:
+        with open(input_path, "r") as f:
+            next(f)
+            for line in tqdm(f, total=n_lines):
+                line = line.strip().split("\t")
+                site = (line[0], int(line[1]))
+                if site in poi_sites:
+                    site_data = {}
+                    for col in cols:
+                        site_data[col] = dtypes[col](line[col_idx[col]])
+                    data[site] = site_data # type: ignore None is overwritten if the site is found in the feature table
+            return data # type: ignore see above
+
+    ##############################################################################################################
+    #                                           Main processing methods                                          #
+    ##############################################################################################################
+    def main(self) -> None:
         """
-        Processes a single position from the pileup data.
+        Performs the main processing steps including data loading, statistical analysis, and report generation.
 
-        Parameters:
-            pileup_data (str): A string containing tab-separated data for a single position from the pileup file.
+        Notes:
+        - This method orchestrates the entire process of statistical analysis and report generation.
+        - It sequentially calls other methods to load data, identify usable POIs, retrieve feature values,
+          calculate p-values, adjust p-values for false discovery rates, create an interactive plot,
+          optionally store statistical results in a table, and generate an HTML report.
+        - The HTML report summarizes the analysis, providing an overview of statistical results and an interactive plot.
+        """
+        hs.print_update(f"Filtering usable POIs... ", line_break=False)
+        poi_sites_overview, total, usable = self.get_usable_pois()
+        hs.print_update(f"{usable} out of {total} usable.", with_time=False)
+
+        hs.print_update("Collecting feature values and performing tests.")
+        stat_features = self.get_feature_values()
+        stat_results = self.calc_pvals(stat_features)
+        # add fdr and -log10(fdr) in place
+        hs.print_update("Adjusting p-values.")
+        self.calc_fdr(stat_results)
+        hs.print_update("Setting up plot.")
+        fig = self.create_fdr_plot(stat_results)
+
+        if self.store_stat:
+            self.write_stat_table(stat_results)
+        self.write_html(poi_sites_overview, fig)
+        
+        hs.print_update("Finished.")
 
-        Returns:
-            str: The processed line as a string.
+    def get_usable_pois(self) -> Tuple[str, int, int]:
         """
-        line = line_str.split("\t")
-        # extract elements from list
-        try:
-            chr, site, ref_base, read_bases, read_qualities = line[0], int(line[1]), line[2].replace("T", "U"), line[4], line[5]
-        except:
-            return ""
-            
-        # filter by genomic region
-        region = self.filter_genomic_region
-        if region is not None:
-            if not(chr == region[0] and site >= region[1] and site <= region[2]): # both start and end inclusive
-                return ""
-
-        # extract coverage and filter by number of reads if the standard coverage option is used 
-        n_reads = int(line[3])
-        if n_reads < self.filter_num_reads: return ""
+        Identifies usable positions of interest (POIs) based on data availability and read counts.
 
-        # get reference sequence 
-        try:
-            ref = self.ref_sequences[chr]
-        except:
-            return ""
-        # get absolute number of A, C, G, U, ins, del
-        count, ref_skip_positions = self.parse_pileup_string(read_bases, ref_base)
-
-        # get qualitiy measures
-        quality_mean, quality_std = self.get_read_quality(read_qualities, ref_skip_positions)
-        # filter by mean read quality
-        if quality_mean < self.filter_mean_quality: return ""
-
-        # in case the alternative way of calculating the coverage is specified
-        # could use if else statement and get the other case down here, but then 
-        # the count will be calculated each time, potentially wasting time in case the 
-        # filter_num_reads is used
-        n_reads_alt = count["a"]+count["c"]+count["g"]+count["u"]
-
-        # get relative number of A, C, G and U counts
-        count_rel = self.get_relative_count(count, n_reads)
-        count_rel_alt = self.get_relative_count(count, n_reads_alt)
-
-        # filter by percentage of deletions
-        if count_rel["del"] < self.filter_perc_deletion: return ""
-
-        # get allele fraction
-        mismatch_rate = self.get_mismatch_perc(count_rel, ref_base)
-        mismatch_rate_alt = self.get_mismatch_perc(count_rel_alt, ref_base)
-
-        # filter by mismatch_rate
-        if mismatch_rate < self.filter_perc_mismatch:
-            return ""
-        if mismatch_rate_alt < self.filter_perc_mismatch_alt:
-            return ""
-
-        # get majority base
-        majority_base = self.get_majority_base(count)
-
-        # get 11b motif
-        motif = self.get_motif(chr, site, ref, k=2)
-
-        out = f'{chr}\t{site}\t{n_reads}\t{ref_base}\t{majority_base}\t{count["a"]}\t{count["c"]}\t{count["g"]}\t{count["u"]}\t{count["del"]}\t{count["ins"]}\t{count["ref_skip"]}\t{count_rel["a"]}\t{count_rel["c"]}\t{count_rel["g"]}\t{count_rel["u"]}\t{count_rel["del"]}\t{count_rel["ins"]}\t{count_rel["ref_skip"]}\t{mismatch_rate}\t{mismatch_rate_alt}\t{motif}\t{quality_mean}\t{quality_std}\n'
-        return out
-
-    def remove_indels(self, pileup_string: str) -> str:
-        """
-        Takes a pileup string and removes all occurences of the following patterns:
-        '\\+[0-9]+' for insertions
-        '\\-[0-9]+' for deletions
-        In addition to the pattern itself, remove the following n characters,
-        where n is the number specified after + or -.
-
-        Parameters
-        ----------
-        pileup_string : str
-            Pileup string extracted from the fifth column of a pileup file
-
-        Returns
-        -------
-        str
-            Pileup strings with all occurences of the patterns above removed
-        """
-        pattern = "(\\+|\\-)[0-9]+"
-        
-        # get the start and end indices of all found patterns 
-        coords = []
-        for m in re.finditer(pattern, pileup_string):
-            str_len_as_str = pileup_string[m.start()+1:m.end()]
-            num_digits = len(str_len_as_str)
-            str_len = int(str_len_as_str)
-            coords.append((m.start(), m.start()+1+num_digits+str_len))
-
-        # remove the patterns by the indices
-        for start, end in reversed(coords): # reverse list as to not shift the index downstream
-            pileup_string = pileup_string[:start] + pileup_string[end:]
-
-        return pileup_string
-
-    def parse_pileup_string(self, pileup_string: str, ref_base: str) -> Tuple[Dict[str, int], List[int]]:
-        """
-        Extracts the number of each base called at a given position, as well as the number
-        of insertions and deletions. Information is extracted from a pileup string (fifth
-        column in a pileup file).
-
-        Parameters
-        ----------
-        pileup_string : str
-            Pileup string extracted from the fifth column of a pileup file
-        ref_base : str
-            reference base at the position corresponding to the pileup string
-
-        Returns
-        -------
-        dict
-            Dictionary containing the number of A, U, C, G, 
-            insertions and deletions.
-        """
-        pileup_string = pileup_string.lower()
-        # remove all occurences of a caret and the following letter (could contain a,c,g,t)
-        pileup_string = re.sub(r'\^.', '', pileup_string)
+        Returns:
+        - str: A summary string describing the number of POIs extracted from the BED file
+               and the number of POIs used in the statistical comparison.
 
-        ref_base = ref_base.lower()
-        count_dict = {"a": 0, "u": 0, "c": 0, "g": 0, "del": 0, "ins": 0}
+        Notes:
+        - This method iterates through each POI and its neighboring sites to check if the data is available
+          and the number of reads is sufficient in both samples.
+        - POIs and their neighboring sites that meet the criteria are considered usable and stored in the 'poi_sites_usable' attribute.
+        - The summary string includes information about the total number of POIs extracted from the BED file,
+          the number of usable POIs, and the criteria used for determining usability.
+        """
+        poi_sites_usable = {}
+        # for both samples, for all POIs check if the data is available and the number of reads is sufficient
+        # at the site itself AND all surrounding sites 
+        for sample in [self.basename_a, self.basename_b]:
+            for center_site, nb_sites in self.poi_sites.items():
+                usable = True
+                for nb_site in nb_sites:
+                    if self.data[sample][nb_site]:
+                        n_reads = self.data[sample][nb_site]["n_reads"] # type: ignore if statement above ensures that its not None
+                        if n_reads < self.n_reads_threshold:
+                            usable = False
+                            break # if one site in the neighbourhood is unusable, the POI at hand gets skipped
+                    else: 
+                        usable = False
+                        break # if one site in the neighbourhood is unusable, the POI at hand gets skipped
+                if usable:
+                    poi_sites_usable[center_site] = self.poi_sites[center_site]
+
+        num_center_sites = len(self.poi_sites.keys())
+        num_usable_center_sites = len(poi_sites_usable.keys())
+
+        section_str = f"""
+                    {num_center_sites} positons were extracted from {self.bed_path}. From these, {num_usable_center_sites} sites were used in the statistical
+                     comparison, as the site itself and all neighbouring sites {self.num_neighbours} bases up- and downstream have sufficient number of reads 
+                     (>= {self.n_reads_threshold}) in both sample <i>{self.basename_a}</i> and <i>{self.basename_b}</i>.
+                    """
         
-        # get number of deletions
-        count_dict["del"] = pileup_string.count("*")
-        # get number of insertions
-        count_dict["ins"] = len(re.findall(r'\+[0-9]+[ACGTNacgtn]+', pileup_string))
-
-        # remove indel patterns to count the number of mismatches correctly
-        pileup_string = self.remove_indels(pileup_string)
-
-        # get number of mismatches (i.e. [ACGT])
-        count_dict["a"] = pileup_string.count("a")
-        count_dict["u"] = pileup_string.count("t")
-        count_dict["c"] = pileup_string.count("c")
-        count_dict["g"] = pileup_string.count("g")
-
-        # get number of matches (determine where to count matches bases on ref_base)
-        n_matches = pileup_string.count('.') + pileup_string.count(',')
-        count_dict[ref_base] = n_matches
-
-        # get number of reference skips
-        n_ref_skips = pileup_string.count("<") + pileup_string.count(">")
-        count_dict["ref_skip"] = n_ref_skips
-
-        # get the indices from the > & < positions, to filter out of the quality string later on
-        # (the corresponding positions refer to the read quality, not the quality of the position on the reads)
-        pileup_string = re.sub(r'\*', "", pileup_string)
-
-        ref_skip_idc = [i for i, char in enumerate(pileup_string) if (char==">") | (char=="<")]
-
-        return count_dict, ref_skip_idc
-
-    def get_relative_count(self, count_dict: Dict[str, int], n_reads: int) -> Dict[str, float]:
-        """
-        Gets a dictionary containing the absolute counts for A, C, G and U
-        and calculates the relative proportions
-
-        Parameters
-        ----------
-        count_dict : dict[int]
-            Dictionary containing the absolute counts for A, C, G and U
-        n_reads : int
-            Number of reads at the given position
-
-        Returns
-        -------
-        dict[float]
-            Dictionary containing the relative counts for A, C, G and U
-        """
-        #n_reads = sum([count_dict["a"], count_dict["c"], count_dict["g"], count_dict["u"]])
-        rel_dict = {}
-        for category in ["a", "c", "g", "u", "del", "ins", "ref_skip"]:
-            try:
-                rel_dict[category] = count_dict[category] / n_reads
-            except:
-                rel_dict[category] = 0
-
-        return rel_dict
-
-    def get_majority_base(self, count_dict: Dict[str, int]) -> str:
-        """
-        Gets a dictionary containing the absolute counts for A, C, G and U and returns the
-        key of the one with the highest count.
-
-        Parameters
-        ----------
-        count_dict : dict
-            dictionary containing the absolute counts for A, C, G and U
-
-        Returns
-        -------
-        str
-            Key from the dictionary corresponding to the largest value
-        """
-        dict_subset = dict((k, count_dict[k]) for k in ("a", "c", "g", "u"))
-        dict_subset["-"] = count_dict["del"]
-
-        return max(dict_subset, key = lambda k: dict_subset[k]).upper()
-
-    def get_motif(self, chr: str, site: int, ref: str, k: int) -> str:
-        """
-        Extracts the motif of k bases up- and downstream from a given chromosomal site.
-        Around the start and end of a refernce sequence the missing bases are filled with
-        Ns.
-
-        Parameters
-        ----------
-        chr : str
-            name of the chromosome
-        site : int
-            position on the chromosome (1-indexed)
-        ref : str
-            reference sequence for the given chromosome 
-        k : int
-            number of bases to be regarded in both up- and downstream direction 
-            
-        Returns
-        -------
-        str
-            sequence of k bases around the center site
-        """ 
-        idx = site-1
-        n_ref = len(ref)
-
-        if idx >= 0 and idx < n_ref:
-            idx_l = idx-k
-            idx_r = idx+k+1
-            # left overhang
-            if idx_l < 0:
-                len_overhang = abs(idx_l)
-                overhang = "N" * len_overhang
-                motif = overhang + ref[:idx_r]
-            # right overhang
-            elif idx_r > n_ref:
-                len_overhang = idx_r - n_ref
-                overhang = "N" * len_overhang
-                motif = ref[idx_l:] + overhang
-            # no overhang
-            else:
-                motif = ref[idx_l:idx_r]
+        # Update the POI sites to contain only usable sites
+        self.poi_sites_usable = poi_sites_usable
+        return section_str, num_center_sites, num_usable_center_sites
 
-            return motif.replace("T", "U")
-        return ""
-        
-    def get_mismatch_perc(self, count_dict_rel: Dict[str, float], ref_base: str) -> float:
+    def get_feature_values(self) -> Dict[SAMPLE, Dict[int, Dict[FEATURE, List[float]]]]:
         """
-        Calculates the number of reads containing a mismatch, insertion or deletion 
-        at a given position.
+        Retrieves feature values for each sample at each position of interest (POI).
 
-        Parameters
-        ----------
-        count_dict : dict
-            Dictionary containing the number of occurences of A,C,G,U,ins,del for a given position
-        ref_base : str
-            reference base at the given position
-
-        Returns
-        -------
-        int
-            Number of mismatched reads a the given position
-        """
-        mismatch_perc_sum = 0
-        for b in ["a", "c", "g", "u"]:
-            if b != ref_base.lower():
-                mismatch_perc_sum += count_dict_rel[b]
-
-        return mismatch_perc_sum
-
-    def get_read_quality(self, read_qualities: str, ref_skip_positions: List[int]) -> Tuple[float, float]:
-        """
-        Calculates the mean and std from the read qualities given in the sixth row
-        of a pileup file.
-
-        Parameters
-        ----------
-        read_qualities : str
-            Read quality string from pileup file
-
-        Returns
-        -------
-        tuple[float, float]
-            Mean and standard deviation of read qualities
-        """
-        # remove quality values corresponding to reference skips
-        read_qualities_len = len(read_qualities)
-        read_qualities_list = list(read_qualities)
-        ref_skip_positions.reverse()
-        
-        for i in ref_skip_positions:
-            if i < read_qualities_len: # when >/< comes at the end, the quality values don't seem to be added to the string
-                read_qualities_list.pop(i)
-        read_qualities = "".join(read_qualities_list)
-
-        if len(read_qualities) > 0:
-            # transform string to list of corresponding phred numeric values
-            vals = [code - 33 for code in read_qualities.encode("ascii")]
-            
-            mean = np.mean(vals).astype(float)
-            std = np.std(vals).astype(float)
-        else:
-            mean = -1
-            std = -1
+        Returns:
+        - Dict[str, Dict[int, Dict[str, List[float]]]]: A nested dictionary containing feature values for each sample
+          at each relative position around POIs.
+            - The outer dictionary's keys are sample names.
+            - The inner dictionary's keys are relative positions (-num_neighbours to +num_neighbours).
+            - The innermost dictionary contains feature values as lists, with keys representing different features.
+
+        Notes:
+            - This method extracts feature values for each sample at each position of interest and its neighboring positions.
+            - Feature values are stored in lists corresponding to different features such as mismatch rate, deletion rate, etc.
+        """
+        stat_features_dict = {}
+        # extract the values for each feature at each position for each sample and store them in a list for later access and comparison
+        for sample in [self.basename_a, self.basename_b]:
+            stat_features_dict[sample] = defaultdict(lambda: {"mismatch_rate": [], "deletion_rate": [], "insertion_rate": [], "q_mean": []})
+            for nb_sites in self.poi_sites_usable.values():
+                for i, nb_site in enumerate(nb_sites, start=-self.num_neighbours):
+                    site_data = self.data[sample][nb_site]
+                    for feature in ["mismatch_rate", "deletion_rate", "insertion_rate", "q_mean"]:
+                        stat_features_dict[sample][i][feature].append(site_data[feature]) # type: ignore in self.get_usable_pois is ensured that the data is available here  
 
-        return mean, std 
+            stat_features_dict[sample] = dict(stat_features_dict[sample])
+        return stat_features_dict
     
-    #################################################################################################################
-    #                                  Functions called during neighbour search                                     #
-    #################################################################################################################
-    def process_small(self, current_pos: int, neighbourhood: List[str]) -> str:
+    def calc_pvals(self, stat_features: Dict[SAMPLE, Dict[int, Dict[FEATURE, List[float]]]]) -> Dict[FEATURE, Dict[int, Dict[str, float|str]]]:
         """
-        Process a small neighbourhood in case the full window size is smaller than the number of lines.
+        Calculates p-values for statistical tests comparing feature values between samples.
 
         Parameters:
-            current_pos (int): The current position within the neighbourhood.
-            neighbourhood (List[str]): A list of lines representing the neighbourhood.
-            n_lines (int): The total number of lines in the input.
+        - stat_features (Dict[str, Dict[int, Dict[str, List[float]]]]): A nested dictionary containing feature values for each sample
+                                                                        at each relative position around POIs.
 
         Returns:
-            str: The processed line as a string.
-        """        
-        ref_str = neighbourhood[current_pos].strip("\n")
-        nb = neighbourhood.copy()
-        ref = nb[current_pos].strip("\n").split("\t")
-        del(nb[current_pos])
-
-        nb_info = self.get_neighbour_info(ref, nb)
-        ref_str += f"\t{nb_info}\n"
-        return ref_str
+        - Dict[str, Dict[int, Dict[str, float|str]]]: A nested dictionary containing calculated p-values for each feature
+          at each relative position around POIs.
+                - The outer dictionary's keys are feature names.
+                - The inner dictionary's keys are relative positions (-num_neighbours to +num_neighbours).
+                - The innermost dictionary contains p-values and the test used for comparison.
+
+        Notes:
+            - This method performs statistical tests (t-test or Wilcoxon test) to compare feature values between two samples.
+            - The resulting p-values and the test used for comparison are stored in a nested dictionary structure.
+        """
+        stat_results = {}
+
+        for feature in ["mismatch_rate", "deletion_rate", "insertion_rate", "q_mean"]:
+            stat_results[feature] = {}
+            for rel_pos in range(-self.num_neighbours, self.num_neighbours+1):
+                pval, test_used = self.perform_test(stat_features[self.basename_a][rel_pos][feature], stat_features[self.basename_b][rel_pos][feature], alpha=self.alpha)
+                stat_results[feature][rel_pos] = {"pval": pval, "test": test_used}
+        
+        return stat_results
+ 
+    def perform_test(self, set1: List[float], set2: List[float], alpha: float = 0.01) -> Tuple[float, str]:
+        """
+        Performs a series of tests to compare two sets of data. It checks for normality in both 
+        samples and equal variances using normaltest and bartlett tests. If the conditions are
+        met, it performs an t-test for connected samples, otherwise, it performs a Wilcoxon-test for
+        connected samples. If the test fails returns None for the p-value and 'ERROR' for the test that was used.
 
-    def process_edge(self, current_pos: int, neighbourhood: List[str], start: bool = True) -> str:
+        Parameters:
+        - set1 (List[float]): The first set of data.
+        - set2 (List[float]): The second set of data.
+        - alpha (float): The significance level for the tests (default is 0.01).
+
+        Returns:
+        - float|None: p-value of the test or None if an Exception was raised
+        - str: string indicating the test that was used
         """
-        Process a neighbourhood at the beginning or the end of the input.
+        try:
+            if (normaltest(set1)[1] >= alpha) & (normaltest(set2)[1] >= alpha) & (bartlett(set1, set2)[1] >= alpha): # normal distributions in both samples + equal variances
+                return ttest_rel(a=set1, b=set2)[1], "t-test"
+            else: # normal distribution in both samples and equal variances
+                # return f"{mannwhitneyu(x=set1, y=set2)[1]:.5e} (MWU)"
+                return wilcoxon(x=set1, y=set2)[1], "Wilcoxon-test"
+        except:
+            return -1, "ERROR"
+
+    def calc_fdr(self, stat_results: Dict[FEATURE, Dict[int, Dict[str, float|str]]]) -> None:
+        """
+        Calculates false discovery rates (FDR) for each test.
 
         Parameters:
-            current_pos (int): The current position within the neighbourhood.
-            neighbourhood (List[str]): A list of lines representing the neighbourhood.
-            start (bool, optional): A boolean indicating if it's the start or end of the neighbourhood. Defaults to True.
+            - stat_results (Dict[str, Dict[int, Dict[str, float|str]]]): A nested dictionary containing calculated p-values
+                for each feature at each relative position around POIs.
 
-        Returns:
-            str: The processed line as a string.
+        Notes:
+            - This method calculates FDRs for each feature at each relative position based on the p-values obtained
+            from statistical tests.
+            - It adjusts the p-values using the Benjamini-Hochberg procedure to control the FDR.
+            - The adjusted p-values (FDR) are stored in the 'fdr' key within the inner dictionaries of 'stat_results'.
+            - Additionally, the negative logarithm of the adjusted p-values is calculated and stored as 'neg_log_fdr'.
+        """
+        pvals = []
+        features = []
+        rel_pos = []
+        for feature in stat_results.keys():
+            for pos in stat_results[feature].keys():
+                pvals.append(stat_results[feature][pos]["pval"])
+                features.append(feature)
+                rel_pos.append(pos)
+        fdrs = fdrcorrection(pvals)[1]
+        # add values in place
+        for feature, pos, fdr in zip(features, rel_pos, fdrs):
+            stat_results[feature][pos]["fdr"] = fdr
+            stat_results[feature][pos]["neg_log_fdr"] = -log10(fdr)
+
+    def create_fdr_plot(self, stat_results: Dict[FEATURE, Dict[int, Dict[str, float|str]]]) -> go.Figure:
         """
-        k = self.window_size
-        ref_str = neighbourhood[current_pos].strip("\n")
-        nb = neighbourhood.copy()
-        ref = nb[current_pos].strip("\n").split("\t")
-
-        if start:
-            nb = nb[:current_pos+k+1]
-            del(nb[current_pos])
-        else:       
-            del(nb[current_pos])
-            nb = nb[current_pos-k:]
-
-        nb_info = self.get_neighbour_info(ref, nb)
-        ref_str += f"\t{nb_info}\n"
-        return ref_str
-
-    def process_neighbourhood(self, neighbourhood: List[str]) -> str:
-        """
-        Get 2*window_size+1 rows ([row i-k, ..., row i, ..., row i+k]) that are next to each other in the tsv file and compare the row i to all 
-        remaining ones. Check if the other rows are on the same chromosome and if the relative distance between them is smaller or equal to k.
-        Create a summary string that indicates the error position relative to the center position.
-        Add new information to the row and return.
+        Creates an interactive plot visualizing adjusted p-values (-log10(FDR)) for different features at each relative position.
 
         Parameters:
-            neighbourhood (List[str]): List of k number of rows extracted from a tsv file.
+            - stat_results (Dict[str, Dict[int, Dict[str, float|str]]]): A nested dictionary containing adjusted p-values
+                (FDR) for each feature at each relative position around POIs.
 
         Returns:
-            str: New line containing the neighbourhood information for a given center position.
-        """        
-        k = self.window_size
+            - go.Figure: An interactive plotly Figure object displaying adjusted p-values (-log10(FDR)) for different features.
+
+        Notes:
+            - This method generates a plot to visualize the adjusted p-values (FDR) for each feature at each relative position.
+            - Adjusted p-values are transformed into negative logarithms for better visualization.
+            - The plot is interactive and allows users to hover over data points to see detailed information.
+            - Features are represented by different traces on the plot, with relative positions on the x-axis and
+            -log10(FDR) on the y-axis.
+        """
+        fig = hs.update_plot(go.Figure(), width=1000, height=500)
+        fig.add_hline(y=2, line_color="black", line_dash="dash", line_width=3, name=f"FDR={self.alpha}")
+        for feature, name in zip(["mismatch_rate", "deletion_rate", "insertion_rate", "q_mean"], ["Mismatch rate", "Deletion rate", "Insertion rate", "Mean q-score"]):
+            x = list(stat_results[feature].keys())
+            y = [stat_results[feature][pos]["neg_log_fdr"] for pos in x]
+            # https://stackoverflow.com/questions/59057881/how-to-customize-hover-template-on-with-what-information-to-show
+            customdata = [[round(stat_results[feature][pos]["fdr"],6), stat_results[feature][pos]["test"]] for pos in x] # type: ignore "fdr" entry is always float
+            scatter = go.Scatter(x=x, y=y, 
+                                 name=name, 
+                                 customdata=customdata, 
+                                 hovertemplate="Rel. position: %{x}<br>-log(FDR): %{y}<br>FDR: %{customdata[0]}<br>Test: %{customdata[1]}",
+                                 line_width=3, marker_size=10)
+            fig.add_trace(scatter)
+
+        fig.update_xaxes(title=f"Relative position in {2*self.num_neighbours+1}-mer", tickmode = 'array', tickvals = [i for i in range(-self.num_neighbours,self.num_neighbours+1)])
+        fig.update_yaxes(title="-log10( FDR )")
+
+        return fig
+    
+    def write_stat_table(self, stat_results: Dict[FEATURE, Dict[int, Dict[str, float | str]]]) -> None:
+        """
+        Writes statistical results including p-values, adjusted p-values (FDR), and the test used to a tab-separated file.
 
-        ref_str = neighbourhood[k].strip("\n")
-        nb = neighbourhood.copy()
+        Parameters:
+            - stat_results (Dict[str, Dict[int, Dict[str, float|str]]]): A nested dictionary containing statistical results
+                for each feature at each relative position around POIs.
 
-        ref = nb[k].strip("\n").split("\t")
-        del nb[k]
+        Notes:
+            - This method writes statistical results to a tab-separated file for further analysis or documentation.
+            - The file contains columns for feature name, relative position, p-value, adjusted p-value (FDR), negative logarithm of FDR,
+            and the test used for comparison.
+            - Each row represents statistical results for a specific feature at a specific relative position.
+        """
+        bed_name = os.path.basename(os.path.splitext(self.bed_path)[0])
+        output_path = os.path.join(self.out_dir, f"{self.basename_a}_{self.basename_b}_{bed_name}_statcompare.tsv")
+        hs.print_update(f"Writing (adjusted) p-values to {output_path}.")
+        
+        table = "feature\trelative_position\tp_value\tfdr\tneg_log10_fdr\ttest_used\n"
+        for feature in stat_results.keys():
+            for rel_pos in stat_results[feature].keys():
+                pval = str(stat_results[feature][rel_pos]["pval"])
+                test = str(stat_results[feature][rel_pos]["test"])
+                fdr = str(stat_results[feature][rel_pos]["fdr"])
+                neg_log_fdr = str(stat_results[feature][rel_pos]["neg_log_fdr"])
+                row = "\t".join([feature, str(rel_pos), pval, fdr, neg_log_fdr, test]) + "\n"
+                table += row
 
-        nb_info = self.get_neighbour_info(ref, nb)
-        ref_str += f"\t{nb_info}\n"
-        return ref_str
+        with open(output_path, "w") as o:
+            o.write(table)
 
-    def get_neighbour_info(self, ref: List[str], neighbourhood: List[str]) -> str:
+    def write_html(self, poi_sites_overview: str, fig: go.Figure) -> None:
         """
-        From a range of neighbouring lines in a file (neighbourhood), check if positions in these lines are neighbours on the reference genome 
-        (based on chromosome and site) and if close genomic positions can be regarded as errors based on the given error threshold.
+        Writes the statistical comparison results and an interactive plot to an HTML report.
 
         Parameters:
-            ref (List[str]): Line of the central position for which neighbours are searched.
-            neighbourhood (List[str]): List containing the lines surrounding the central position.
+            - poi_sites_overview (str): A summary string describing the number of POIs used in the statistical comparison.
+            - fig (go.Figure): An interactive plotly Figure object displaying adjusted p-values (-log10(FDR)) for different features.
 
-        Returns:
-            str: A string giving the relative distance to all neighbouring errors to the central position, if any were found.
-        """        
-        k = self.window_size
-        ref_chr = ref[0]
-        ref_site = int(ref[1])
-
-        nb_info = ""
-
-        # for each neighbour check if they are 1.on the same chr and 2.neighbours
-        for pos in neighbourhood:
-            pos = pos.strip("\n").split("\t")
-            chr = pos[0]
-            perc_error = float(pos[19])
-
-            if (chr == ref_chr) & (perc_error >= self.neighbour_error_threshold): # check if same chromosome & if pos is error
-                site = int(pos[1])
-                relative_pos = site - ref_site
-
-                if (abs(relative_pos) <= k): # check if pos are close to each other
-                    nb_info += str(relative_pos)+","
-        return nb_info
+        Notes:
+            - This method generates an HTML report summarizing the statistical comparison results and an interactive plot.
+            - The HTML report includes general information about the analysis, a summary of usable POIs, and an interactive plot.
+            - The interactive plot allows users to explore adjusted p-values (-log10(FDR)) for different features at each relative position.
+            - The HTML report is generated with CSS styling for better presentation and readability.
+        """
+        css_string, plotly_js_string = hs.load_html_template_str()
+        time = hs.get_time()
+        fig_str = fig.to_html(include_plotlyjs=False)
+
+        bed_name = os.path.basename(os.path.splitext(self.bed_path)[0])
+        output_path = os.path.join(self.out_dir, f"{self.basename_a}_{self.basename_b}_{bed_name}_statcompare.html")
+        hs.print_update(f"Writing HTML summary to {output_path}.")
+
+        template = f"""
+            <!DOCTYPE html>
+            <html lang="en">
+            <head>
+                <meta charset="UTF-8">
+                <meta http-equiv="X-UA-Compatible" content="IE=edge">
+                <meta name="viewport" content="width=device-width, initial-scale=1.0">
+                <title>Neet - POI comparison</title>                        
+                <style>{css_string}</style>
+            </head>
+
+            <body>
+                <script>{plotly_js_string}</script>
+
+                <header>
+                    <h1>Statistical comparison of positions of interest ({self.basename_a}-{self.basename_b})</h1>
+                    <p>Produced by <a href="https://github.com/dietvin/neet">Neet</a> on <b>{time}</b></p>
+                </header>
+                
+                <section>
+                    <p class="intro-text">
+                        This summary file was created from the extracted features in file <b>{self.in_path_a}</b> for sample <b>{self.basename_a}</b> 
+                        and <b>{self.in_path_b}</b> for sample <b>{self.basename_b}</b>. POIs were provided in <b>{self.bed_path}</b>. The plots are 
+                        interactive and allow further information by hovering, zooming and panning.
+                    </p>
+                </section>
+
+                
+                <section>
+                    <button class="collapsible">Resuls of the statistical comparison</button>
+                    <div class="collapsible-content">
+                        <h2 class="hiddentitle" id="map"></h2>
+
+                        <h3>General information</h3>
+                        <p>
+                            {poi_sites_overview}
+                        </p>
+
+                        <h3>Overview of adjusted p-values</h3>
+                        <div class="plot-container">
+                            {fig_str}
+                        </div>
+                        <p>
+                            False-discovery rates (FDR) of different error features at positions {self.num_neighbours} bases up- and downstream from
+                            positions of interest. Features were statistically compared between '{self.basename_a}' and '{self.basename_b}' using 
+                            a t-test or Wilcoxon test for connected samples. The dashed line indicates <b>alpha={self.alpha}</b>.  
+                        </p>
+
+                    </div>
+                </section>
+
+                <script>
+                    var coll = document.getElementsByClassName("collapsible");
+                    var i;
+
+                    for (i = 0; i < coll.length; i++) {{
+                    coll[i].addEventListener("click", function() {{
+                        this.classList.toggle("active");
+                        var content = this.nextElementSibling;
+                        if (content.style.display === "none") {{
+                        content.style.display = "block";
+                        }} else {{
+                        content.style.display = "none";
+                        }}
+                    }});
+                    }}
+                </script>
+
+            </body>
+            <footer></footer>
+            </html> 
+        """
+        with open(output_path, "w") as out:
+            out.write(template)
+
+
+if __name__=="__main__":
+    p = PoiSampleComparer(path_a="/home/vincent/projects/neet_project/data/45s_rrna/test/drna_cyt_extracted.tsv",
+                          path_b="/home/vincent/projects/neet_project/data/45s_rrna/test/drna_nuc_extracted.tsv",
+                          basename_a="Cytoplasm",
+                          basename_b="Nucleus",
+                          bed_path="/home/vincent/projects/neet_project/data/45s_rrna/test/psu_sites.bed",
+                          out_dir="/home/vincent/projects/neet_project/data/45s_rrna/test", 
+                          store_stat=True)
+
+    p.main()
```

### Comparing `neet-nanopore-0.0.4/neet/poi_analyzer.py` & `neet_nanopore-1.0.0/neet/poi_summary.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,119 +1,113 @@
-from typing import List, Dict, Tuple
-import os, sys, warnings
+from typing import List, Dict, Tuple, Any
+import os, math, datetime
 import plotly.graph_objects as go
 import plotly.express as px
 from plotly.subplots import make_subplots
 from plotly.io import to_html
 from intervaltree import IntervalTree
-import datetime, argparse
 from collections import defaultdict
-from statistics import median
+from statistics import median, mean
 from scipy.stats import normaltest, bartlett, ttest_ind, mannwhitneyu
-from . import helper_functions as hs
+from statsmodels.stats.multitest import fdrcorrection
+from tqdm import tqdm
 
-class POIAnalyzer():
+try: # when invoked from the package
+    from neet import helper_functions as hs
+except ImportError: # when invoked directly
+    import helper_functions as hs
+
+class POISummary():
 
     in_path: str
     bed_path: str
     ref_path: str
 
     perc_mismatch_col: str
     output_tsv: bool
     export_svg: bool
 
-    data: Dict[str, List[str]] | Dict[str, List[int]] | Dict[str, List[float]] | Dict[str, List[str | None]]
+    data: Dict[str, List[Any]] # dtypes can be str, int, float, str|None
     bed_categories: List[str]
     bed_categories_counterparts: List[str] | List[None]
     output_paths: List[str]
 
-    category_data: Dict[str, List[str]] | Dict[str, List[int]] | Dict[str, List[float]] | Dict[str, List[str | None]]
-    counterpart_data: Dict[str, List[str]] | Dict[str, List[int]] | Dict[str, List[float]] | Dict[str, List[str | None]] | None
+    category_data: Dict[str, List[Any]] # dtypes can be str, int, float, str|None
+    counterpart_data: Dict[str, List[Any]] | None
     current_category: str
     current_counterpart: str | None 
+
+    n_bins_seqmap: int
+    n_bins: int
     
-    def __init__(self, in_path: str, out_path: str, bed_path: str, ref_path: str,
+    def __init__(self, in_path: str, bed_path: str, ref_path: str,
                  categories: str,
-                 canonical_counterpart: str | None,
+                 out_dir: str | None = None, 
+                 canonical_counterpart: str | None = None,
                  output_tsv: bool = True, 
                  use_perc_mismatch_alt: bool = False,
-                 export_svg: bool = False) -> None:
+                 export_svg: bool = False,
+                 n_bins_seqmap: int = 200,
+                 n_bins: int = 5000) -> None:
         """
         Initialize an instance of the GenomicDataProcessor class.
 
-        Args:
-            in_path (str): The path to the input TSV file containing genomic data.
-            out_path (str): The path to the output directory where results will be saved.
-            bed_path (str): The path to the BED file containing genomic intervals.
-            ref_path (str): The path to the reference FASTA file.
-            categories (str): A comma-separated string containing bed categories.
-            canonical_counterpart (str): A comma-separated string containing bases corresponding to bed categories.
-            output_tsv (bool, optional): Whether to output results as a TSV file. Default is True.
-            use_perc_mismatch_alt (bool, optional): Whether to use 'mismatch_rate_alt' instead of 'mismatch_rate' column. Default is False.
-
-        Returns:
-            None
-
-        Note:
-            This constructor initializes an instance of the GenomicDataProcessor class. It sets various attributes
-            based on the provided arguments and performs necessary data processing and validation steps.
-
+        Parameters:
+        - in_path (str): The path to the input TSV file containing genomic data.
+        - out_dir (str|None): The path to the output directory where results will be saved.
+        - bed_path (str): The path to the BED file containing genomic intervals.
+        - ref_path (str): The path to the reference FASTA file.
+        - categories (str): A comma-separated string containing bed categories.
+        - canonical_counterpart (str): A comma-separated string containing bases corresponding to bed categories.
+        - output_tsv (bool, optional): Whether to output results as a TSV file. Default is True.
+        - use_perc_mismatch_alt (bool, optional): Whether to use 'mismatch_rate_alt' instead of 'mismatch_rate' column. Default is False.
         """
         self.process_path(in_path, bed_path, ref_path)
         self.load_data()
         self.add_bed_info()
         self.perc_mismatch_col = "mismatch_rate_alt" if use_perc_mismatch_alt else "mismatch_rate"
 
-        self.process_categories(categories, canonical_counterpart, out_path)
+        self.process_categories(categories, canonical_counterpart, out_dir)
+
+        # number of bins in which the coordinates of present sequences will be grouped for the sequence map plot
+        self.n_bins_seqmap = n_bins_seqmap
+        # number of data points to display in boxplots (to reduce file size for large datasets)
+        self.n_bins = n_bins
 
         self.output_tsv = output_tsv
         self.export_svg = export_svg
 
     ##############################################################################################################
     #                                           Initialization methods                                           #
     ##############################################################################################################
 
     def process_path(self, in_path: str, bed_path: str, ref_path: str) -> None:
         """
-        Process and validate input and output paths for data processing.
-
-        Args:
-            in_path (str): The path to the input TSV file containing genomic data.
-            out_path (str): The path to the output directory where results will be saved.
-            bed_path (str): The path to the BED file containing genomic intervals.
-            ref_path (str): The path to the reference FASTA file.
-
-        Returns:
-            None
-
-        Note:
-            This method validates and sets the paths required for data processing. It checks the existence and
-            file extensions of the provided paths, raising exceptions or issuing warnings as appropriate. After
-            validation, it sets the 'in_path', 'bed_path', 'ref_path', and 'output_path' attributes of the class
-            for use in subsequent processing steps.
+        Validate input paths and assign paths to member variables.
 
+        Parameters:
+        - in_path (str): The path to the input TSV file containing genomic data.
+        - bed_path (str): The path to the BED file containing genomic intervals.
+        - ref_path (str): The path to the reference FASTA file.
         """
         hs.check_input_path(in_path, [".tsv"])
-        self.in_path = in_path
+        self.in_path = os.path.abspath(in_path)
         hs.check_input_path(bed_path, [".bed"])
-        self.bed_path = bed_path
+        self.bed_path = os.path.abspath(bed_path)
         hs.check_input_path(ref_path, [".fasta", ".fa", ".fn"])
-        self.ref_path = ref_path
+        self.ref_path = os.path.abspath(ref_path)
 
     def load_data(self) -> None:
         """
-        Load data from the specified input file into the SummaryCreator instance.
+        Load data from the specified input file into the POISummary instance.
 
         Reads the data from a tab-separated values (tsv) file as created by the PileupExtractor module
         and stores it in the 'data' attribute of the class.
-
-        Returns:
-        - None
         """
-        cols = ["chr", "site", "n_reads", "ref_base", "majority_base", "a_rate", "c_rate", "g_rate", "u_rate", "deletion_rate", "insertion_rate", "refskip_rate", "mismatch_rate", "q_mean", "motif", "neighbour_error_pos"]
+        cols = ["chr", "site", "n_reads", "ref_base", "majority_base", "a_rate", "c_rate", "g_rate", "u_rate", "deletion_rate", "insertion_rate", "refskip_rate", "mismatch_rate", "mismatch_rate_alt", "q_mean", "motif", "neighbour_error_pos"]
 
         col_idx = {'chr': 0, 'site': 1, 'n_reads': 2, 'ref_base': 3, 'majority_base': 4, 'n_a': 5, 'n_c': 6, 'n_g': 7, 'n_t': 8, 'n_del': 9, 'n_ins': 10, 'n_ref_skip': 11, 'a_rate': 12, 'c_rate': 13, 'g_rate': 14, 'u_rate': 15, 'deletion_rate': 16, 'insertion_rate': 17, 'refskip_rate': 18, 'mismatch_rate': 19, 'mismatch_rate_alt': 20, 'motif': 21, 'q_mean': 22, 'q_std': 23, 'neighbour_error_pos': 24}
         dtypes = {'chr': str, 'site': int, 'n_reads': int, 'ref_base': str, 'majority_base': str, 'n_a': int, 'n_c': int, 'n_g': int, 'n_t': int, 'n_del': int, 'n_ins': int, 'n_ref_skip': int, 'a_rate': float, 'c_rate': float, 'g_rate': float, 'u_rate': float, 'deletion_rate': float, 'insertion_rate': float, 'refskip_rate': float, 'mismatch_rate': float, 'mismatch_rate_alt': float, 'motif': str, 'q_mean': float, 'q_std': float, 'neighbour_error_pos': str}
         
         with open(self.in_path, "r") as file:
             next(file)
             data = dict(zip(cols, [[] for _ in cols]))
@@ -126,91 +120,68 @@
                 else:
                     data["neighbour_error_pos"].append(line[24])
 
             self.data = data
     
     def add_bed_info(self) -> None:
         """
-        Add BED information to a DataFrame based on a BED file.
-
-        Returns:
-            pd.DataFrame: The DataFrame with an additional 'bed_name' column containing BED information.
-
-        Note:
-            This method takes a DataFrame 'data' containing genomic data and adds an additional column 'bed_name'
-            to it. The 'bed_name' column is populated by querying a previously built IntervalTree from the
-            specified 'bed_path' for each row in the DataFrame. The method returns the enriched DataFrame.
-
+        Add BED information to the data object based on a BED file.
         """
         tree = self.build_interval_tree(self.bed_path)
         self.data["bed_name"] = [self.get_name_for_position(chrom, site, tree) for chrom, site in zip(self.data["chr"], self.data["site"])]
 
     def get_name_for_position(self, chrom: str, site: int, interval_tree: IntervalTree) -> str|None:
         """
         Retrieve the name associated with a given genomic position from an interval tree.
 
-        Args:
-            position (tuple): A tuple containing the chromosome and position to query (e.g., ('chr1', 100)).
-            interval_tree (IntervalTree): An IntervalTree data structure containing genomic intervals.
+        Parameters:
+        - chrom (str): Sequence name of the given position.
+        - site (int): Coordinate on the sequence.
+        - interval_tree (IntervalTree): An IntervalTree data structure containing genomic intervals.
 
         Returns:
-            str | None: The name associated with the provided position if found, or None if not found.
-
-        Note:
-            This method queries the provided 'interval_tree' for intervals that overlap with the specified
-            genomic position. It iterates through the results and checks if the chromosome matches the
-            provided chromosome in the 'position' tuple. If a matching interval is found, the associated
-            name is returned. If no matching interval is found, None is returned.
-
+        - str | None: The name associated with the provided position if found, or None if not found.
         """
         results = interval_tree[site:site+1]  # Query the interval tree
         for interval in results:
             chromosome, name = interval.data
             if chromosome == chrom:
                 return name
         return None
 
     def build_interval_tree(self, bed_file: str) -> IntervalTree:
         """
-        Build an IntervalTree data structure from a BED file.
+        Build an IntervalTree data structure from positions in a BED file.
 
-        Args:
-            bed_file (str): The path to the BED file containing genomic intervals.
+        Parameters:
+        - bed_file (str): The path to the BED file containing genomic intervals.
 
         Returns:
-            IntervalTree: An IntervalTree data structure containing the genomic intervals from the BED file.
-
-        Note:
-            This method reads the specified BED file and extracts genomic intervals along with optional
-            associated names. It constructs an IntervalTree data structure to efficiently query and store
-            these intervals. The method accounts for the 0-based indexing convention in BED files by adding
-            1 to the start and end positions. If a name is provided in the BED file, it is associated with
-            the corresponding interval. The constructed IntervalTree is returned.
-
+        - IntervalTree: An IntervalTree data structure containing the genomic intervals from the BED file.
         """
         interval_tree = IntervalTree()
         with open(bed_file, 'r') as file:
             for line in file:
                 parts = line.strip().split('\t')
                 if len(parts) >= 3:
                     chromosome = parts[0]
                     start = int(parts[1])+1 # +1 to account for 0-index in BED files 
                     end = int(parts[2])+1 # +1 to account for 0-index in BED files
                     name = parts[3] if len(parts) >= 4 else None
                     interval_tree[start:end] = (chromosome, name)
         return interval_tree
 
-    def process_categories(self, categories: str, counterparts: str|None, out_paths: str) -> None:
+    def process_categories(self, categories: str, counterparts: str|None, out_dir: str|None) -> None:
         """
         Process categories, counterparts, and output paths.
 
         Parameters:
         - categories (str): Comma-separated string of categories to be processed.
         - counterparts (str|None): Comma-separated string of counterparts or None if not provided.
-        - out_paths (str): Comma-separated string of output paths or a single directory path.
+        - out_dir (str): Path to a single output directory.
 
         Raises:
         - Exception: If a specified category is not found in the bed file.
         - Exception: If the number of counterparts does not match the number of categories.
         - Exception: If the number of output paths does not match the number of categories.
 
         Note:
@@ -226,130 +197,167 @@
             
         # if given, process counterparts
         if counterparts:
             cou_split = counterparts.upper().split(",")
             if len(cou_split) != len(cat_split):
                 raise Exception(f"For the {len(cat_split)} categories {len(cou_split)} corresponding bases were given. Each category must have a base it corresponds to.")
         else:
-            cou_split = [None for _ in self.bed_categories]
+            cou_split = [None for _ in cat_split]
+
+        # process output paths
+        if out_dir:
+            out_dir = os.path.abspath(out_dir)
+            ext = os.path.splitext(out_dir)[1]
+            if ext:
+                hs.print_update(f"Warning: Extension {ext} was found. Make sure to provide a single output directory.")
+            hs.check_create_dir(out_dir)
+            out_paths = []
+            for category, counterpart in zip(cat_split, cou_split):
+                in_filename = os.path.splitext(os.path.basename(self.in_path))[0]
+                filename = f"{in_filename}_{category}_{counterpart}_poisummary.html" if counterpart else f"{in_filename}_{category}_poisummary.html"
+                out_paths.append(os.path.join(out_dir, filename))
+        else:
+            path_base = os.path.splitext(self.in_path)[0]
+            out_paths = []
+            for category, counterpart in zip(cat_split, cou_split):
+                filepath = f"{path_base}_{category}_{counterpart}_poisummary.html" if counterpart else f"{path_base}_{category}_poisummary.html"
+                out_paths.append(filepath)
 
-        # process ouput paths
-        out_split = out_paths.split(",")
-        if len(out_split) > 1:
-            if len(out_split) != len(cat_split): # output for each category?
-                raise Exception(f"For the {len(cat_split)} categories {len(out_split)} output paths were given. Each category must have an output path it corresponds to.")
-            else:
-                for out in out_split:
-                    hs.check_create_dir(os.path.dirname(out))
-        else: # output string must be a directory
-            dirname = out_paths
-            hs.check_create_dir(dirname)
-            in_basename = os.path.splitext(os.path.basename(self.in_path))[0]
-            out_split = [os.path.join(dirname, f"{c}_{in_basename}_summary.html") for c in cat_split]
-    
         self.bed_categories = cat_split
         self.bed_categories_counterparts = cou_split
-        self.output_paths = out_split
+        self.output_paths = out_paths
 
     ##############################################################################################################
     #                                           Main processing methods                                          #
     ##############################################################################################################
 
-    def main(self):
+    def main(self) -> None:
         """
         Main entry point of the script.
 
         This method iterates through the bed categories and their corresponding bases, processing each category using
         the `process_category` method.
-
-        Returns:
-            None: The script performs the desired processing and saves the output files.
         """
         for category, corr_base, output_path in zip(self.bed_categories, self.bed_categories_counterparts, self.output_paths):
             self.process_category(category, corr_base, output_path)
 
     def process_category(self, category: str, corresponding_base: str|None, output_path: str) -> None:
         """
         Process and analyze the data for a specific category and (optionally) corresponding base.
 
         This method generates multiple plots and saves them along with a summary HTML template. Optionally, it also
         writes the processed data to a TSV file.
 
         Parameters:
-            category (str): The category of interest.
-            corresponding_base (str): The corresponding base for the category.
-
-        Returns:
-            None: The plots and summary are saved to files, and optionally, the data is saved in TSV format.
+        - category (str): The category of interest.
+        - corresponding_base (str): The corresponding base for the category.
         """
-        hs.print_update(f"Processing {category} sites.")
+        time = hs.get_time()
 
-        hs.print_update("   - subsetting data... ", line_break=False)
+        hs.print_update(f"Processing {category} sites. Subsetting data...", line_break=False)
         self.subset_category_data(category, corresponding_base)
         if corresponding_base:
-            hs.print_update(f"Done. Found {len(self.category_data['chr'])} {category} and {len(self.counterpart_data['chr'])} {corresponding_base} sites.", with_time=False)
+            hs.print_update(f"Done. Found {len(self.category_data['chr'])} {category} and {len(self.counterpart_data['chr'])} {corresponding_base} sites.", with_time=False) # type: ignore
         else:
             hs.print_update(f"Done. Found {len(self.category_data['chr'])} {category} sites.", with_time=False)
 
-        hs.print_update("   - creating position overview... ", line_break=False)
-        plot_mod_map = self.create_map_plot()
-        hs.print_update("Done", with_time=False)
-
-        hs.print_update(f"   - creating overview of mismatch types at {category} sites... ", line_break=False)
-        plot_mism_types = self.create_mism_types_plot()
-        hs.print_update("Done", with_time=False)
-
-        hs.print_update(f"   - creating base composition plots at {category} and {corresponding_base} sites... ", line_break=False)
-        plot_comp = self.create_composition_plot()
-        hs.print_update("Done", with_time=False)
-
-        hs.print_update(f"   - creating overview of error rates at {category} and {corresponding_base} sites... ", line_break=False)
-        plot_err_rate, p_val_table = self.create_error_rate_plot()
-        hs.print_update("Done", with_time=False)
+        total = 8 if self.output_tsv else 7
+        with tqdm(desc=f"{time} | POI map", total=total) as progress: 
+            plot_mod_map = self.create_map_plot()
+            progress.update()
+
+            progress.set_description(f"{time} | Mismatch types")
+            plot_motif = self.create_motif_plot()
+            progress.update()
+
+            progress.set_description(f"{time} | Mismatch types")
+            plot_mism_types = self.create_mism_types_plot()
+            progress.update()
+
+            progress.set_description(f"{time} | Base compositions")
+            plot_comp, p_val_table_comp = self.create_composition_plot()
+            progress.update()
+
+            progress.set_description(f"{time} | Error rates")
+            plot_errrate, p_val_table_errrate = self.create_error_rate_plot()
+            progress.update()
         
-        hs.print_update(f"   - creating overview of neighbouring mismatches around {category} sites... ", line_break=False)
-        plot_nb = self.create_nb_plot()
-        hs.print_update("Done", with_time=False)
-
-        plots = [plot_mod_map, plot_mism_types, plot_comp, plot_err_rate, plot_nb]
-        tables = [p_val_table]
-
-        hs.print_update(f"  - creating HTML summary file at {output_path}... ", line_break=False)
-        self.write_template(plots, tables, output_path)
-        hs.print_update("Done", with_time=False)
-
-        if self.output_tsv:
-            hs.print_update(f"  - creating updated feature table at {self.in_path}... ", line_break=False)
-            self.write_tsv()
-            hs.print_update("Done", with_time=False)
-        hs.print_update(f"Finished processing {category}.")
+            progress.set_description(f"{time} | Neighbour mismatches")
+            plot_nb = self.create_nb_plot()
+            progress.update()
+
+            plots = [plot_mod_map, plot_motif, plot_mism_types, plot_comp, plot_errrate, plot_nb]
+            tables = [p_val_table_comp, p_val_table_errrate]
+
+            progress.set_description(f"{time} | Writing to HTML")
+            self.write_template(plots, tables, output_path)
+            progress.update()
+
+            if self.output_tsv:
+                progress.set_description(f"{time} | Updating feature table")
+                ft_path = self.write_tsv()
+                progress.update()
+                hs.print_update(f"Finished processing {category}. Wrote HTML summary to {output_path}. Wrote updated table to {ft_path}")
+        if not self.output_tsv:
+            hs.print_update(f"Finished processing {category}. Wrote output to {output_path}")
+
+        hs.print_update("Finished.")
+
 
     ##############################################################################################################
     #                                          Data preparation methods                                          #
     ##############################################################################################################
-        
-    def subset_category_data(self, category: str, counterpart: str|None) -> None:
+    def bin_data(self, data: List[int|float]) -> List[int|float]:
         """
-        Subset the data based on the given category and counterpart (if provided).
+        Bin the input data into segments and return the mean value of each segment.
 
         Parameters:
-        - category (str): The category to filter the data by.
-        - counterpart (str|None): The counterpart to filter the data by. If None, counterpart filtering is skipped.
+        - data (List[int|str|float]): The input data to be binned.
+
+        Raises:
+        - Exception: If the number of bins is larger than the length of the data.
 
         Returns:
-        None
+        - List[int|float]: List of mean values for each bin.
+        """
+        total_length = len(data)
+        num_segments = self.n_bins
+
+        if num_segments: # added to stop pylance from complaining 
+            if total_length <= num_segments:
+                return data
+            segment_length = segment_length = total_length // num_segments
+            remainder = total_length % num_segments
+            
+            start_index = 0
+            end_index = 0
+            segments = []
+            for i in range(num_segments):
+                end_index = start_index + segment_length + (1 if i < remainder else 0)
+                segments.append(data[start_index:end_index])
+                start_index = end_index
 
-        The method filters the internal data based on the provided category and counterpart values,
+            return [mean(segment) for segment in segments]
+        return data
+
+    def subset_category_data(self, category: str, counterpart: str|None) -> None:
+        """
+        Filters the internal data based on the provided category and counterpart values,
         creating two subsets: one for the specified category and another for the counterpart (if provided).
 
         It updates the following attributes:
         - self.category_data (dict): A dictionary containing subsets of data for the specified category.
         - self.counterpart_data (dict): A dictionary containing subsets of data for the specified counterpart.
         - self.current_category (str): The currently selected category.
         - self.current_counterpart (str|None): The currently selected counterpart.
+        
+        Parameters:
+        - category (str): The category to filter the data by.
+        - counterpart (str|None): The counterpart to filter the data by. If None, counterpart filtering is skipped.
+
         """
         bed_name_idx = list(self.data.keys()).index("bed_name")
         ref_base_idx = list(self.data.keys()).index("ref_base")
         data_keys = self.data.keys()
         key_idx = dict(zip([i for i in range(len(data_keys))], data_keys))
 
         subset_category = dict(zip(data_keys, [[] for _ in range(len(data_keys))]))
@@ -366,257 +374,325 @@
         
         self.category_data = subset_category
         self.counterpart_data = subset_counterpart
 
         self.current_category = category
         self.current_counterpart = counterpart
 
-    def prepare_data_map(self) -> Tuple[List[str], List[int]]:
+    def prepare_data_map(self) -> Tuple[List[float], Dict[str, List[int]], Dict[str, List[int]]]: 
         """
-        Prepare the data for the sequence map based on references and category data.
+        Prepare data for creating a chromosome map.
 
-        Returns:
-        Tuple[List[str], List[int]]:
-            A tuple containing two lists:
-            - List of chromosome names present in both references and category data.
-            - List of corresponding chromosome lengths.
+        Parameters:
+        - ref_path (str): Path to the reference file containing chromosome lengths.
+        - category_data (Dict[str, List[int]]): Dictionary containing chromosome names ('chr') and their corresponding genomic coordinates ('site').
+        - n_bins_seqmap (int, optional): Number of bins to divide each chromosome into. Default is 100.
 
-        The method reads a fasta file specified by 'ref_path' and extracts the sequences
-        along with their chromosome names. It then compares the unique chromosome names in
-        the category data with those in the references, ensuring only common ones are considered.
+        Returns:
+        - List[float]: A list of y-values representing the positions of bins along the chromosome.
+        - Dict[str, List[int]]: A dictionary containing chromosome names as keys and lists of counts of genomic coordinates falling into each bin as values.
+        - Dict[str, List[int]]: A dictionary containing chromosome names as keys and integers representing the maximum coordinate value (exclusive) that each bin may contain.
 
-        The resulting tuple contains:
-        - List of common chromosome names sorted numerically and alphabetically.
-        - List of corresponding lengths of the chromosomes.
+        Example:
+        AAAACCGCGUUGUG -> len=14, n_bins_seqmap=4 -> binsize=ceil(14/4)=ceil(3.5)=4 
+        01234567890123                     -> [4,8,12]+[15]=[4,8,12,15]
+                                        -> [1,4), [4,8), [8,12), [12,15)
+        
+        With coordinates = [1,5,6,7,14] -> counts=[1,3,0,1]
         """
-        def get_references(path: str) -> Dict[str, str]:
-            """
-            Reads a fasta file and stores the sequences in a dictionary (values) with the 
-            corresponding chromosome names (keys).
+        def custom_sort_key(item):
+            """Custom sorting key function to sort chromosome names."""
+            if item.isdigit():  # Check if the item is a digit
+                return (int(item),)  # Convert to integer and sort numerically
+            else:
+                return (float('inf'), item)  # Place non-digits at the end
 
-            Parameters
-            ----------
-            path : str
-                filepath to a fasta file
-
-            Returns
-            -------
-            dict[str]
-                Dictionary where the key is the chromosome name and the value is the sequence
-            """
-            with open(path, "r") as ref:
+        def get_ref_len(ref_path: str) -> Dict[str, int]:
+            """Reads reference file and extracts chromosome lengths."""
+            with open(ref_path, "r") as ref:
                 refs = {}
                 line = next(ref)
-                if not line.startswith(">"):
-                    raise Exception(f"Fasta format error. The first line of fasta file '{path}' does not contain a header (starting with '>').")
-                
-                chr_name = line[1:].strip().split(" ")[0]
-                seq = ""
+                seq_name = line[1:].strip().split(" ")[0]
+                seq_len = 0
+
                 for line in ref:
                     if line.startswith(">"):
-                        refs[chr_name] = seq
-                        chr_name = line[1:].strip().split(" ")[0]
-                        seq = ""
+                        refs[seq_name] = seq_len
+                        seq_name = line[1:].strip().split(" ")[0]
+                        seq_len = 0
                     else:
-                        seq += line.strip()
-                        
-                refs[chr_name] = seq # add the last dict entry
-                sys.stdout.write("\n")
+                        seq_len += len(line.strip())
+                refs[seq_name] = seq_len # add the last dict entry
             return refs
 
-        def custom_sort_key(item):
-            if item.isdigit():  # Check if the item is a digit
-                return (int(item),)  # Convert to integer and sort numerically
-            else:
-                return (float('inf'), item)  # Place non-digits at the end
+        # Calculate chromosome lengths
+        ref_lens = get_ref_len(self.ref_path)
+        present_seq = list(sorted(set(self.category_data["chr"]).intersection(ref_lens.keys()), key=custom_sort_key))
+
+        pos_count = {} # stores the values for coloring the bins
+        bin_sizes = {} 
+        max_vals = {} # stores the values for labelling the bins
+        for seq in present_seq:
+            seq_len = ref_lens[seq]
+
+            bin_size = math.ceil(seq_len / self.n_bins_seqmap)
+            bin_sizes[seq] = bin_size
+            # initialize the maximum coordinates that a bin may contain (excluded)
+            max_vals[seq] = [bin_size*i for i in range(1,self.n_bins_seqmap)] + [seq_len+1] 
+            # initialize counts for each bin with 0
+            pos_count[seq] = [0]* self.n_bins_seqmap 
+
+        # Count genomic coordinates falling into each bin
+        for seq, site in zip(self.category_data["chr"], self.category_data["site"]):
+            bin_index = site // bin_sizes[seq]
+            pos_count[seq][bin_index] += 1
+
+        # Generate y-values for bin positions along the chromosome
+        y_vals = [i/self.n_bins_seqmap for i in range(self.n_bins_seqmap)]
 
-        ref_dict = get_references(self.ref_path)
+        return y_vals, pos_count, max_vals
+    
+    def prepare_data_motif(self) -> Tuple[Dict[str, Dict[str, int]], int]:
+        """
+        Prepare data for a bar plot showing the motifs of the POIs. 
 
-        all_keys = ref_dict.keys()
-        present_chr = list(sorted(set(self.category_data["chr"]).intersection(all_keys), key=custom_sort_key))
-        chr_lens = [len(ref_dict[x]) for x in present_chr]
+        Returns:
+        - Dict[str, Dict[str, int]]: Dictionary containing the counts (int) for each relative position (second level) 
+                                     and reference base (first level)
+                                     
+        """
+        motif_len = len(self.category_data["motif"][0])
+        middle_idx = motif_len//2
+        rel_positions = [pos - middle_idx for pos in range(motif_len)]
+        counts = defaultdict(lambda: dict(zip(rel_positions, [0]*len(rel_positions))))
 
-        return present_chr, chr_lens
+        for idx, pos in enumerate(rel_positions):
+            for motif in self.category_data["motif"]:
+                base = motif[idx]
+                counts[base][pos] += 1
 
-    def prepare_data_mism_types(self) -> Tuple[List[List[int]], List[List[str]], int]:
+        return dict(counts), motif_len
+
+    def prepare_data_mism_types(self) -> Dict[str, Dict[str, int]]:
         """
         Prepare data for a confusion matrix based on mismatch counts.
 
-        Parameters:
-        - mis_count (Dict[str, int]): Dictionary containing mismatch counts for each base pair combination.
-
         Returns:
-        - Tuple[List[List[int]], List[List[str]], int]: Tuple containing matrix data, matrix labels, and the maximum value in the matrix.
+        - Dict[str, Dict[str, int]]: Dictionary containing the counts for all combination of reference and
+                                     called bases.
         """
+        mis_count = {"A": {"A": 0, "C": 0, "G": 0, "U": 0, "Del": 0}, 
+                    "C": {"A": 0, "C": 0, "G": 0, "U": 0, "Del": 0}, 
+                    "G": {"A": 0, "C": 0, "G": 0, "U": 0, "Del": 0}, 
+                    "U": {"A": 0, "C": 0, "G": 0, "U": 0, "Del": 0}}
+        for ref, maj in zip(self.category_data["ref_base"], self.category_data["majority_base"]):
+            if (ref != "args") & (maj != "N"):
+                if maj=="-": maj="Del"
+                mis_count[ref][maj] += 1
+        return mis_count
+
+    def prepare_data_composition(self) -> Tuple[Dict[str, Dict[str, float]], 
+                                                Dict[str, Dict[str, float]], 
+                                                List[str], 
+                                                Dict[Tuple[str, str], Dict[str, str]]]:
+        """
+        Prepare the data for visualizing the base composition and performs the statistical comparisons of the base
+        rates between the different groups in the data. The groups can be the following:
+        - matched POIs
+        - mismatched POIs
+
+        If a canonical counterpart base is given:
+        - matched counterpart base
+        - mismatched counterpart base
+
+        A, C, G and U rates are extracted for all given groups, the rates are statistically compared, the median of
+        the rates are calculated for each group, the median rates are scaled to add up to 1 for each group and the
+        x-values for the plotting functions are set up accordingly to the given groups. 
+        The data is stored in nested Dictionaries where the first key corresponds to the group (matched POI, ...)
+        and the second key corresponds to the feature (A-rate, ...). 
+
+        Returns:
+        - Dict[str, Dict[str, float]],         : Scaled median base rates
+        - Dict[str, Dict[str, float]],         : Median base rates
+        - List[str],                           : x-values for the plotting function
+        - Dict[Tuple[str, str], Dict[str, str]]: Results of the statistical tests (returned by the compare_groups method)
+        """
+        def get_counts_rates(for_category: bool) -> Tuple[Dict[str, int], Dict[str, Dict[str, List[float]]]]:
+            """
+            Get the A, C, G and U rates at mismatched and matched sites for either positions of interest or at canonical
+            counterpart bases (depending on for_category value). Also count the number of positions in each group.
 
-        mis_types = [f"{f} - {t}" for f in ["A", "C", "G", "U"] for t in ["A", "C", "G", "U"]]
-        mis_count = dict(zip(mis_types, [0]*len(mis_types)))
+            Parameters:
+            - for_category (bool): Boolean for specifying the group at hand.
 
-        for ref, maj in zip(self.category_data["ref_base"], self.category_data["majority_base"]):
-            if (ref != "N") & (maj != "N"):
-                mis_count[f"{ref} - {maj}"] += 1
+            Returns:
+            - Dict[str, int]: Counts of matched and mismatched sites within the given groups
+            - Dict[str, Dict[str, List[float]]]: A, C, G and U rates for each of the given groups
+            """
+            key_match, key_mismatch = ("category_match", "category_mismatch") if for_category else ("counterpart_match", "counterpart_mismatch")
+            data = self.category_data if for_category else self.counterpart_data
 
-        # prepare data for the confusion matrix
-        matrix_data = [[None]*4 for _ in range(4)]
-        matrix_labels = [[None]*4 for _ in range(4)]
-        bases = ["A", "C", "G", "U"]
-        # fill count matrix
-        for i in range(4): 
-            for j in range(4):
-                count = mis_count[f"{bases[i]} - {bases[j]}"]
-                matrix_data[i][j] = count
-                if i != j:
-                    matrix_labels[i][j] = count
-        # fill the matrix containing corresponding labels
-        vals_flat = [element for sublist in matrix_labels for element in sublist if (element is not None)]
-        vals_sum = sum(vals_flat)
-        for i in range(4): 
-            for j in range(4):
-                if matrix_labels[i][j]:
-                    matrix_labels[i][j] = f"{round(matrix_labels[i][j] / vals_sum * 100, 2)}%"
-                else: 
-                    matrix_labels[i][j] = ""
-        # get the max value
-        val_max = max(vals_flat)
-
-        return matrix_data, matrix_labels, val_max
-
-    def prepare_data_composition(self) -> Tuple[Dict[str, Tuple[float,float]|Tuple[float,float,float,float]], Dict[str, Tuple[float,float]|Tuple[float,float,float,float]], Tuple[int,int]|Tuple[int,int,int,int]]:
-        """
-        Prepare data for composition analysis, including base rates, medians, and scaled medians.
-
-        Returns:
-        Tuple[Dict[str, Tuple[float, float] | Tuple[float, float, float, float]],
-            Dict[str, Tuple[float, float] | Tuple[float, float, float, float]],
-            Tuple[int, int] | Tuple[int, int, int, int]]:
-            A tuple containing three elements:
-            1. Dictionary with scaled median rates for each base.
-            2. Dictionary with un-scaled median rates for each base.
-            3. Tuple with counts of matches and mismatches.
-
-        The method processes base rates in the category data, calculates medians,
-        and scales the medians to represent proportions. If a counterpart is specified,
-        the same process is applied, and the results are combined for further analysis.
-
-        The returned tuple includes:
-        1. Scaled median rates for each base.
-        2. Un-scaled median rates for each base.
-        3. Counts of matches and mismatches (category-match, counterpart-match, category-mismatch, counterpart-mismatch).
-        """
-        cols = ["ref_base", "majority_base", "a_rate", "c_rate", "g_rate", "u_rate"]
-
-        def get_rates(data: Dict[str, List[str|int|float]]) -> Tuple[Dict[str, Tuple[List[float], List[float]]], Tuple[int]]:
-            rate_dict = defaultdict(lambda: ([], [])) # first sublist -> match; second sublist -> mismatch
-            counts = [0, 0]
-            for ref, maj, *base_rates in zip(*(data[col] for col in cols)):
-                i = 0 if ref == maj else 1
-                counts[i] += 1
-                for j, base in enumerate(["A", "C", "G", "U"]):
-                    rate_dict[base][i].append(base_rates[j])
+            counts = {key_match: 0, key_mismatch: 0}
+            rates = {key_match: {"A": [], "C": [], "G": [], "U": []}, 
+                    key_mismatch: {"A": [], "C": [], "G": [], "U": []}}
+
+            for ref, maj, a_rate, c_rate, g_rate, u_rate in zip(*(data[col] for col in ["ref_base", "majority_base", "a_rate", "c_rate", "g_rate", "u_rate"])): # type: ignore
+                key = key_match if ref==maj else key_mismatch
+                data_select = {"A": a_rate, "C": c_rate, "G": g_rate, "U": u_rate}
+                counts[key] += 1
+                for feature in ["A", "C", "G", "U"]:
+                    rates[key][feature].append(data_select[feature])
+            return counts, rates
 
-            return dict(rate_dict), tuple(counts)
+        def get_median_rates(rate_dict: Dict[str, Dict[str, List[float]]]) -> Dict[str, Dict[str, float]]:
+            """
+            Calculates the median A, C, G and U rates for each group.
 
-        def get_median_rates(rate_dict: Dict[str, Tuple[List[float], List[float]]]) -> Dict[str, Tuple[float, float]|Tuple[float,float,float,float]]:
+            Parameters:
+            - rate_dict (Dict[str, Dict[str, List[float]]]): Dictionary containing the base rates for different groups
+                as returned by the get_counts_rates function.
+            
+            Returns:
+            - Dict[str, Dict[str, float]]: Median values of the different base rates for each group
+            """
             median_rate_dict = {}
-            for key in rate_dict.keys():
-                median_rate_dict[key] = (median(rate_dict[key][0]), median(rate_dict[key][1]))
+            for group in rate_dict.keys():
+                median_rate_dict[group] = {}
+                for subgroup in rate_dict[group].keys():
+                    median_rate_dict[group][subgroup] = median(rate_dict[group][subgroup]) if len(rate_dict[group][subgroup])>0 else 0
             return median_rate_dict
 
-        def get_scaled_median_rates(median_rate_dict: Dict[str, Tuple[float, float]|Tuple[float,float,float,float]]) -> Dict[str, Tuple[float, float]|Tuple[float,float,float,float]]:
+        def get_scaled_median_rates(median_rate_dict: Dict[str, Dict[str, float]]) -> Dict[str, Dict[str, float]]:
+            """
+            Scales the median base rates to add up to 1 for each group. Intended for visualizing different groups
+            in a bar chart of height 1. 
+
+            Parameters:
+            - Dict[str, Dict[str, float]]: Median values of the different base rates for each group (as returned
+                by get_median_rates)
+            
+            Returns:
+            - Dict[str, Dict[str, float]]: Median values of the different base rates for each group scaled to 1
+            """
             scaled_rate_dict = {}
-            # calculate the sum of the A-, C-, G- and U-rates for each x-value
-            totals = [sum(median_rates) for median_rates in zip(*(median_rate_dict[key] for key in median_rate_dict.keys()))]
-            for key, medians in median_rate_dict.items():
-                # scale each value by the corresponding x-value (rates should add up to 1)
-                scaled_rate_dict[key] = tuple(med/total for med, total in zip(medians, totals))
+            # calculate the sum of the A-, C-, G- and U-rates for each group
+            for group, medians in median_rate_dict.items():
+                scaled_rate_dict[group] = {}
+                total = sum(medians.values())
+                for feature in medians.keys():
+                    scaled_rate_dict[group][feature] = median_rate_dict[group][feature] / total if total>0 else 0
             return scaled_rate_dict
 
-        rates, counts = get_rates(self.category_data)
-        median_rates = get_median_rates(rates)
-
+        counts, rates = get_counts_rates(for_category=True)
         if self.current_counterpart:
-            rates_cou, counts_cou = get_rates(self.counterpart_data)
-            median_rates_cou = get_median_rates(rates_cou)
-            # combine count_dict and count_dict_counterpart to have the x-axis order:
-            # category-match, counterpart-match, category-mismatch, counterpart-mismatch 
-            rate_tmp = {}
-            for (base, rate), (_, rate_cou) in zip(median_rates.items(), median_rates_cou.items()):
-                rate_tmp[base] = (rate[0], rate_cou[0], rate[1], rate_cou[1])
-            median_rates = rate_tmp
-
-            counts = (counts[0], counts_cou[0], counts[1], counts_cou[1])
-
-            x_vals = [f"<i>{self.current_category}</i> match<br>(n = {counts[0]})", 
-                    f"{self.current_counterpart} match<br>(n = {counts[1]})", 
-                    f"<i>{self.current_category}</i> mismatch<br>(n = {counts[2]})", 
-                    f"{self.current_counterpart} mismatch<br>(n = {counts[3]})"]
+            counts_cou, rates_cou = get_counts_rates(for_category=False)
+            # merge dictionaries from category and counterpart
+            # https://stackoverflow.com/questions/38987/how-do-i-merge-two-dictionaries-in-a-single-expression-in-python#26853961
+            counts = counts | counts_cou
+            rates = rates | rates_cou
+            # reorder dictionary
+            counts = {k: counts[k] for k in ["category_match", "counterpart_match", "category_mismatch", "counterpart_mismatch"]}
+            rates = {k: rates[k] for k in ["category_match", "counterpart_match", "category_mismatch", "counterpart_mismatch"]}
+
+            x_vals = [f"<i>{self.current_category}</i> match<br>(n = {counts['category_match']})",
+                    f"{self.current_counterpart} match<br>(n = {counts['counterpart_match']})",
+                    f"<i>{self.current_category}</i> mismatch<br>(n = {counts['category_mismatch']})",
+                    f"{self.current_counterpart} mismatch<br>(n = {counts['counterpart_mismatch']})"]
         else:
-            x_vals = [f"<i>{self.current_category}</i> match<br>(n = {counts[0]})", 
-                    f"<i>{self.current_category}</i> mismatch<br>(n = {counts[1]})"]
+            x_vals = [f"<i>{self.current_category}</i> match<br>(n = {counts['category_match']})",
+                    f"<i>{self.current_category}</i> mismatch<br>(n = {counts['category_mismatch']})"]
 
-        return get_scaled_median_rates(median_rates), median_rates, x_vals
+        median_rates = get_median_rates(rates)
+        scaled_median_rates = get_scaled_median_rates(median_rates)
+        stat_comp_results = self.compare_groups(rates)
+
+        return scaled_median_rates, median_rates, x_vals, stat_comp_results
     
     def prepare_data_errorrates(self) -> Tuple[Dict[str, List[float]], 
-                                        Dict[str, List[float]], 
-                                        Dict[str, List[float]], 
-                                        Dict[str, List[float]], 
-                                        Dict[str, List[float]],
-                                        List[str]]:
-        """
-        Prepare error rates data for analysis.
-
-        Returns:
-        Tuple[Dict[str, List[float]], 
-            Dict[str, List[float]], 
-            Dict[str, List[float]], 
-            Dict[str, List[float]], 
-            Dict[str, List[float]],
-            List[str]]:
-            A tuple containing five dictionaries representing different error rates and a list of x-axis labels.
-
-        The method processes error rates in the category data, including mismatch,
-        deletion rate, insertion rate, reference skip rate, and mean quality score.
-        If a counterpart is specified, the same process is applied, and the results are combined for further analysis.
-
-        The returned tuple includes:
-        1. Percentage mismatch rates.
-        2. Relative deletion rates.
-        3. Relative insertion rates.
-        4. Relative reference skip rates.
-        5. Mean quality scores.
-        6. List of x-axis labels representing different conditions.
+                                        List[str], 
+                                        Dict[Tuple[str, str], Dict[str, str]]]:
         """
-        def get_rates(data: Dict[str, List[str|int|float]], x_mat: int, x_mis: int) -> Dict[str, Dict[str, List[float]]]:
-            rate_dict = defaultdict(lambda: {"x": [], "y": []})
-            cols = ["ref_base", "majority_base", self.perc_mismatch_col, "deletion_rate", "insertion_rate", "refskip_rate", "q_mean"]
-            cols_idxs = dict(zip(cols[2:], range(len(cols))))
-            for ref, maj, *rates in zip(*(data[col] for col in cols)):
-                x = x_mat if ref == maj else x_mis
-                for rate in [self.perc_mismatch_col, "deletion_rate", "insertion_rate", "refskip_rate", "q_mean"]:
-                    rate_dict[rate]["x"].append(x)
-                    rate_dict[rate]["y"].append(rates[cols_idxs[rate]])
-            return dict(rate_dict)
+        Prepare the data for visualizing the error rates and quality scores as boxplots and performs the 
+        statistical comparisons of the rates between the different groups in the data. The groups can be 
+        the following:
+        - matched POIs
+        - mismatched POIs
 
-        x_mis = 2 if self.current_counterpart else 1
-        rates = get_rates(self.category_data, x_mat=0, x_mis=x_mis)
+        If a canonical counterpart base is given:
+        - matched counterpart base
+        - mismatched counterpart base
+
+        Mismatch, deletion, insertion, reference skip rates and qualtiy scores are extracted for all given groups and
+        the rates are statistically compared. To get the data into the right shape for the plotly Box function, the 
+        x- and y-values are flattened into two long lists X and Y where position i contains a x,y pair in X[i],Y[i]. 
+
+        Returns:
+        - Dict[str, List[float]],              : Scaled median base rates
+        - List[str],                           : x-values for the plotting function
+        - Dict[Tuple[str, str], Dict[str, str]]: Results of the statistical tests (returned by the compare_groups method)
+        """
+        def get_counts_rates(for_category: bool) -> Tuple[Dict[str, int], Dict[str, Dict[str, List[float]]]]:
+            """
+            Get the mismatch, deletion, insertion and reference skip rates and mean q-scores at mismatched and matched sites for either 
+            positions of interest or at canonical counterpart bases (depending on for_category value). Also count the number of positions 
+            in each group.
+
+            Parameters:
+            - for_category (bool): Boolean for specifying the group at hand.
+
+            Returns:
+            - Dict[str, Dict[str, List[float]]]: mismatch, deletion, insertion and reference skip rates and mean q-scores for each of the 
+                                                given groups
+            """
+            key_match, key_mismatch = ("category_match", "category_mismatch") if for_category else ("counterpart_match", "counterpart_mismatch")
+            data = self.category_data if for_category else self.counterpart_data
+            
+            counts = {key_match: 0, key_mismatch: 0}
+            rates = {key_match: {"Mismatch rate": [], "Deletion rate": [], "Insertion rate": [], "Reference skip rate": [], "Mean q-score": []}, 
+                    key_mismatch: {"Mismatch rate": [], "Deletion rate": [], "Insertion rate": [], "Reference skip rate": [], "Mean q-score": []}}
+            
+            cols = ["ref_base", "majority_base", self.perc_mismatch_col, "deletion_rate", "insertion_rate", "refskip_rate", "q_mean"]
+            for ref, maj, mis_rate, del_rate, ins_rate, refskip_rate, q_mean in zip(*(data[col] for col in cols)): # type: ignore
+                key = key_match if ref==maj else key_mismatch
+                data_select = {"Mismatch rate": mis_rate, "Deletion rate": del_rate, "Insertion rate": ins_rate, "Reference skip rate": refskip_rate, "Mean q-score": q_mean}
+                counts[key] += 1
+                for feature in ["Mismatch rate", "Deletion rate", "Insertion rate", "Reference skip rate", "Mean q-score"]:
+                    rates[key][feature].append(data_select[feature])
+            return counts, rates
 
+        counts, rates = get_counts_rates(for_category=True)
         if self.current_counterpart:
-            rates_cou = get_rates(self.counterpart_data, x_mat=1, x_mis=3)
-            for key in rates.keys():
-                rates[key]["x"] += rates_cou[key]["x"]
-                rates[key]["y"] += rates_cou[key]["y"]
-            x_vals = [f"<i>{self.current_category}</i> match", 
-                    f"{self.current_counterpart} match", 
-                    f"<i>{self.current_category}</i> mismatch", 
-                    f"{self.current_counterpart} mismatch"]
+            counts_cou, rates_cou = get_counts_rates(for_category=False)
+            # merge dictionaries from category and counterpart
+            # https://stackoverflow.com/questions/38987/how-do-i-merge-two-dictionaries-in-a-single-expression-in-python#26853961
+            counts = counts | counts_cou
+            rates = rates | rates_cou
+            # reorder dictionary
+            rates = {k: rates[k] for k in ["category_match", "counterpart_match", "category_mismatch", "counterpart_mismatch"]}
+
+        # for plotly boxplots the x and y values need to be one long list containing x,y pairs at a position i in each list
+            x_vals = [f"<i>{self.current_category}</i> match"] * min(counts["category_match"], self.n_bins) + \
+                    [f"{self.current_counterpart} match"] * min(counts["counterpart_match"], self.n_bins) + \
+                    [f"<i>{self.current_category}</i> mismatch"] * min(counts["category_mismatch"], self.n_bins) + \
+                    [f"{self.current_counterpart} mismatch"] * min(counts["counterpart_mismatch"], self.n_bins)
         else:
-            x_vals = [f"<i>{self.current_category}</i> match", 
-                    f"<i>{self.current_category}</i> mismatch"]
+            x_vals = [f"<i>{self.current_category}</i> match"] * min(counts["category_match"], self.n_bins) + \
+                    [f"<i>{self.current_category}</i> mismatch"] * min(counts["category_mismatch"], self.n_bins)
 
-        return *rates.values(), x_vals
+        stat_comp_results = self.compare_groups(rates)
+
+        # flatten the counts to be compatible with the plotly boxplot function
+        # this is done here at the end so the statistical comparison can be performed beforehand
+        rates_flat = {}
+        for feature in rates["category_match"].keys():
+            rates_flat[feature] = []
+            for group in rates.keys():
+                rates_flat[feature] += self.bin_data(rates[group][feature])
+
+        return rates_flat, x_vals, stat_comp_results
 
     def prepare_nb_counts(self) -> Tuple[List[int], List[int], List[int], List[int], List[str], List[int]]:
         """
         Prepare data for analyzing neighboring error positions in a specified bed category.
 
         Returns:
             Tuple[List[int], List[int], List[int], List[int], List[str], List[int]]:
@@ -670,242 +746,346 @@
         pie_vals = [n_no_nb, n_has_nb, n_has_nb_mod]
 
         return list(counts.keys()), list(counts.values()), list(counts_mod.keys()), list(counts_mod.values()), pie_labs, pie_vals
 
     ##############################################################################################################
     #                                            p-val table methods                                             #
     ##############################################################################################################
-    def perform_test(self, set1: List[float], set2: List[float], alpha: float = 0.05) -> str:
+    def perform_test(self, set1: List[float], set2: List[float], alpha: float = 0.01) -> Tuple[float|None, str]:
         """
-        Perform a statistical test to compare two sets of data.
+        Performs a series of tests to compare two sets of data. It checks for normality in both 
+        samples and equal variances using normaltest and bartlett tests. If the conditions are
+        met, it performs an independent t-test (TT), otherwise, it performs a Mann-Whitney U test (MWU).
+        If the test fails returns None for the p-value and 'ERROR' for the test that was used.
 
         Parameters:
         - set1 (List[float]): The first set of data.
         - set2 (List[float]): The second set of data.
-        - alpha (float): The significance level for the tests (default is 0.05).
+        - alpha (float): The significance level for the tests (default is 0.01).
 
         Returns:
-        str:
-            A string representing the result of the statistical test.
-
-        The method performs a series of tests to compare two sets of data. It checks for normality
-        in both samples and equal variances using normaltest and bartlett tests. If the conditions
-        are met, it performs an independent t-test (TT), otherwise, it performs a Mann-Whitney U test (MWU).
-
-        The returned string includes the p-value of the test and the abbreviation of the test method.
-        In case of an exception during the test, it returns "ERROR".
+        - float|None: p-value of the test or None if an Exception was raised
+        - str: string indicating the test that was used
         """
         try:
             if (normaltest(set1)[1] >= alpha) & (normaltest(set2)[1] >= alpha) & (bartlett(set1, set2)[1] >= alpha): # normal distributions in both samples + equal variances
-                return f"{ttest_ind(a=set1, b=set2)[1]:.5e} (TT)"
+                # return f"{ttest_ind(a=set1, b=set2)[1]:.5e} (TT)"
+                return (ttest_ind(a=set1, b=set2)[1], "TT")
             else: # normal distribution in both samples and equal variances
-                return f"{mannwhitneyu(x=set1, y=set2)[1]:.5e} (MWU)"
+                # return f"{mannwhitneyu(x=set1, y=set2)[1]:.5e} (MWU)"
+                return (mannwhitneyu(x=set1, y=set2)[1], "MWU")
         except:
-            return "ERROR"
+            return (None, "ERROR")
 
-    def get_table_header(self) -> str:
+    def compare_groups(self, data: Dict[str, Dict[str, List[float]]]) -> Dict[Tuple[str, str], Dict[str, str]]:
         """
-        Generate an HTML table header based on the current category and counterpart.
+        Perform statistical tests between different combinations of (mis-)matched category and counterpart positions.
 
-        Returns:
-        str:
-            A string containing the HTML table header.
+        Parameters:
+        - data (Dict[str, Dict[str, List[float]]]): Dictionary containing the groups in the first level and some features for
+                                                    a given group in the second level.
 
-        The method generates an HTML table header with column labels based on the current
-        category and counterpart (if applicable). It returns a string formatted as an HTML table row.
+        Returns:
+        - Dict[Tuple[str, str], Dict[str, str]]: Adjusted p-values For each statistical comparison. The groups that have been compared are 
+                                                stored in the first level (Tuple[str,str]). The second level stores the feature (str) with
+                                                the FDR and the test that was used. 
         """
+        # get the groups that will be compared 
         if self.current_counterpart:
-            header = f"<th></th><th>{self.current_category} match vs. {self.current_counterpart} match</th><th>{self.current_category} mismatch vs. {self.current_counterpart} mismatch</th><th>{self.current_category} match vs. {self.current_category} mismatch</th><th>{self.current_counterpart} match vs. {self.current_counterpart} mismatch</th>"
-        else: 
-            header = f"<th></th><th>{self.current_category} match vs. {self.current_category} mismatch</th>"
-        return "<tr>" + header + "</tr>"
-
-    # TODO: add a second table for statistical evaluation of the base compositions
+            comparisons = [("category_match", "counterpart_match"), 
+                           ("category_mismatch", "counterpart_mismatch"), 
+                           ("category_match", "category_mismatch"), 
+                           ("counterpart_match", "counterpart_mismatch")]
+        else:
+            comparisons = [("category_match", "category_mismatch")]
+        # get the features that are present the groups in the data at hand
+        present_features = list(data["category_match"].keys())
+
+        # collect the results in a list first to perform multiple testing correction later
+        comps = []
+        features = []
+        p_vals = [] 
+        tests = []
+        comps_failed = []
+        for group1, group2 in comparisons:
+            for feature in present_features:
+                res, test = self.perform_test(data[group1][feature], data[group2][feature], alpha=0.1)
+                if res:
+                    comps.append((group1, group2))
+                    features.append(feature)
+                    p_vals.append(res)
+                    tests.append(test)
+                else:
+                    comps_failed.append((group1, group2))
+        # adjust the p-values
+        p_vals = list(fdrcorrection(p_vals)[1])
+        
+        # groups the data in a dictionary (level 1: groups that are compared, level 2: features)
+        values = [{}, {}, {}, {}] if self.current_counterpart else [{}, {}]
+        stat_results = dict(zip(comparisons, values))
+        for groups, feature, fdr, test in zip(comps, features, p_vals, tests):
+            stat_results[groups][feature] = f"{fdr:.5e} ({test})"
+        for groups in comps_failed:
+            for feature in present_features:
+                stat_results[groups][feature] = "ERROR"
+        return stat_results # type: ignore
 
-    def create_test_overview(self, datasets: List[Dict[str, List[float]]]) -> str:
+    def create_stat_table(self, pvals: Dict[Tuple[str, str], Dict[str, str]]) -> str:
         """
-        Create an HTML table summarizing statistical tests for multiple datasets.
-
+        Given a nested dictionary containing (adjusted) p-values, aggregates these into a HTML table represented in
+        a single string.
+        
         Parameters:
-        - datasets (List[Dict[str, List[float]]]): A list of datasets, each containing 'x' and 'y' lists.
+        - pvals (Dict[Tuple[str, str], Dict[str, str]]): Nested dictionary, where the first key (Tuple[str, str])
+            represents the two groups (group1, group2) to which the tests correspond. The second key corresponds
+            to the features that were tested for these groups. P-values are stored as strings with the test that
+            were used indicated behind it.
 
         Returns:
-        str:
-            A string containing the HTML table with test results.
-
-        The method generates an HTML table summarizing statistical tests for multiple datasets.
-        Each dataset should include 'x' and 'y' lists. The table includes rows for different data types
-        (Mismatch rate, Deletion rate, Insertion rate, Reference skip rate, Mean quality) and columns
-        for various comparisons based on the current category and counterpart.
-
-        The returned string contains the complete HTML table.
+        - str: String representation of the HTML table containing all p-values. Each column corresponds to a 
+            comparison between two groups. Each row corresponds to one feature. 
         """
-        table = f"<table>" + self.get_table_header()
-
-        for data_type, data in zip(["Mismatch rate", "Deletion rate", "Insertion rate", "Reference skip rate", "Mean quality"], datasets):
-        # split data by groups ("x" entry in data dict)
-            row_data = defaultdict(lambda: [])
-            for x, y in zip(data["x"], data["y"]):
-                row_data[x].append(y)
-            row_data = dict(row_data)
-
-            if self.current_counterpart:
-                row = f"<tr><td>{data_type}</td><td>{self.perform_test(row_data[0], row_data[1])}</td><td>{self.perform_test(row_data[2], row_data[3])}</td><td>{self.perform_test(row_data[0], row_data[2])}</td><td>{self.perform_test(row_data[1], row_data[3])}</td></tr>"
-            else:
-                row = f"<tr><td>{data_type}</td><td>{self.perform_test(row_data[0], row_data[1])}</td></tr>"
-
-            table += row
-
-        return table + "</table>"
+        groups = list(pvals.keys())
+        features = pvals[groups[0]].keys()
+        
+        colnames = {('category_match', 'counterpart_match'):       f"<th>{self.current_category} match vs. {self.current_counterpart} match</th>",
+                    ('category_mismatch', 'counterpart_mismatch'): f"<th>{self.current_category} mismatch vs. {self.current_counterpart} mismatch</th>",
+                    ('category_match', 'category_mismatch'):       f"<th>{self.current_category} match vs. {self.current_category} mismatch</th>",
+                    ('counterpart_match', 'counterpart_mismatch'): f"<th>{self.current_counterpart} match vs. {self.current_counterpart} mismatch</th>"}
+        header = "".join([colnames[g] for g in groups]) # type: ignore
+
+        table = "<table><thead><th></th>"+header+"</thead><tbody>"
+
+        for feature in features:
+            row = f"<tr><td>{feature}</td>"
+            for group in groups:
+                row += f"<td>{pvals[group][feature]}</td>"
+            table += row+"</tr>"
+        table += "</tbody></table>"
+        return table
 
     ##############################################################################################################
     #                                              Plotting methods                                              #
     ##############################################################################################################
 
-    def update_plot(self, fig, title: str|None = None, xlab: str|None = None, ylab: str|None = None, height: int = 500, width: int = 800):
+    def create_map_plot(self) -> go.Figure:
         """
-        Updates the layout of a Plotly figure.
+        Creates a plot showing the approximate positions of interest on the given sequences. Sequences are represented
+        by a set number of bins that group specific ranges of coordinates. The number of POIs in each of these ranges
+        is indicated by the colors. Only sequences that contains POIs are shown in the plot to keep it simple.
 
-        Args:
-            fig (go.Figure): The Plotly figure to be updated.
-            title (str|None): Title of the plot (optional).
-            xlab (str|None): Label for the x-axis (optional).
-            ylab (str|None): Label for the y-axis (optional).
-            height (int): Height of the plot (default: 500).
-            width (int): Width of the plot (default: 800).
-
-        Returns:
-            go.Figure: The updated Plotly figure.
-        """
-        fig.update_layout(template="seaborn",
-                    title = title,
-                    xaxis_title = xlab,
-                    yaxis_title = ylab,
-                    font=dict(family="Open sans, sans-serif", size=20),
-                    plot_bgcolor="white",
-                    margin=dict(l=50, r=50, t=50, b=50),
-                    height=height,  # Set the height to a constant value
-                    width=width)
-        fig.update_xaxes(showline=True, linewidth=2, linecolor='black', mirror=True, showticklabels=True, ticks='outside', showgrid=False, tickwidth=2)
-        fig.update_yaxes(showline=True, linewidth=2, linecolor='black', mirror=True, showticklabels=True, ticks='outside', showgrid=False, tickwidth=2)
+        Returns:
+            go.Figure: A Plotly figure object representing the map plot. 
+        """
+        try:
+            y_vals, pos_count, max_vals = self.prepare_data_map()
 
+            fig = go.Figure()
+            fig = hs.update_plot(fig, height=600, width=1200)
+            tickvals = []
+            ticktext = []
+            bin_height = y_vals[1]
+            # set up a map for each sequence that is present
+            for x, seq in enumerate(pos_count.keys(), start = 1):
+                tickvals.append(x)
+                ticktext.append(seq)
+                bins = []
+                # transform the counts integer into color values from 0 to the maximum count
+                max_count = max(pos_count[seq])
+                colors = px.colors.sample_colorscale("portland", [val/max_count for val in pos_count[seq]])
+                bin_start = [1]+max_vals[seq]
+                bin_end = max_vals[seq]
+                for y, color, count, lab_start, lab_end in zip(y_vals, colors, pos_count[seq], bin_start, bin_end):
+                    # create a rectangle for each bin
+                    bin = go.Scatter(x=[x-0.3, x-0.3, x+0.3, x+0.3, x-0.3], 
+                                    y=[y,y+bin_height,y+bin_height,y,y], 
+                                    name=f"{lab_start}-{lab_end} | #POIs: {count}",
+                                    fill="toself", 
+                                    fillcolor=color,
+                                    marker=dict(color=color),
+                                    showlegend=False, mode='lines')
+                    bins.append(bin)
+                # add rectangles of one sequence to figure
+                fig.add_traces(bins)
+                # surround rectangles by a shape as a border
+                fig.add_shape(type="rect",
+                            x0=x - 0.3, y0=0,
+                            x1=x + 0.3, y1=1,
+                            line=dict(color="#000000", width=3),
+                            fillcolor="rgba(0,0,0,0)",
+                            xref="x", yref="y")
+
+            fig.update_xaxes(tickmode = 'array',
+                            tickvals = tickvals,
+                            ticktext = ticktext)
+            fig.update_yaxes(tickmode = 'array',
+                            tickvals = [0,1],
+                            ticktext = ["5'", "3'"])
+            fig.update_xaxes(range=[0.5,tickvals[-1]+0.5])
+
+            # clean up hoverlabels
+            fig.update_layout(hoverlabel=dict(namelength=0)) 
+        except Exception as e:
+            fig = hs.create_error_placeholder(e)
         return fig
 
-    def create_map_plot(self) -> go.Figure: 
+    def create_motif_plot(self) -> go.Figure:
         """
-        Create a map plot visualizing chromosome lengths and category sites.
+        Create a bar plot visualizing the motifs at positions of interest.
 
         Returns:
-        go.Figure:
-            A Plotly figure representing the map plot.
-
-        The method generates a map plot that visualizes chromosome lengths as bars and
-        category sites as markers. The x-axis represents chromosomes, and the y-axis represents
-        coordinates. The plot is customized for clear visualization, including bar width,
-        scatter marker size, and layout adjustments.
-        """
-        present_chr, chr_lens = self.prepare_data_map()
-
-        width = 1200
-        bargap = 0.9
-        bar_width = 1-bargap+0.15
-        n_bars = len(present_chr)
-        scatter_size = width/n_bars*bar_width
-
-        fig = self.update_plot(go.Figure(), height = 1000, width = width, ylab="Coordinate")
-        fig.add_trace(go.Bar(x=list(present_chr), y=list(chr_lens), marker=dict(color="lightgrey", line=dict(color="black", width=2)), name="Chromosomes", showlegend=False))
-        fig.update_layout(bargap=0.5, yaxis=dict(range=[0,max(chr_lens)+0.1*max(chr_lens)]))
-        fig.add_trace(go.Scatter(x=self.category_data["chr"], y=self.category_data["site"], mode='markers', marker=dict(symbol='line-ew', color="#1f77b4", size=scatter_size, line=dict(width=1.1, color="#1f77b4")), name=f"{self.current_category} sites", hovertemplate="Chr%{x}:%{y}"))
-        fig.update_xaxes(fixedrange=True)
-
+        - go.Figure: A Plotly figure representing the motifs at positions of interest.
+        """
+        try:
+            counts, motif_len = self.prepare_data_motif()
+            fig = go.Figure()
+            fig = hs.update_plot(fig, width=1200)
+
+            colors = {"A": "#2ca02c", "C": "#1f77b4", "G": "#ff7f0e", "U": "#d62728"}
+            bars = []
+            for base in sorted(counts.keys()):
+                x_vals = list(counts[base].keys())
+                y_vals = list(counts[base].values())
+                color = colors[base] if base in colors.keys() else "#A0A0A0"
+                bar = go.Bar(x=x_vals, y=y_vals, name=base, marker=dict(color=color, line_color="#000000", line_width=2))
+                bars.append(bar)
+
+            fig.add_traces(bars)
+            fig.update_layout(barmode="stack") 
+            fig.update_xaxes(title=f"Relative {motif_len}-mer position")
+            fig.update_yaxes(title="Count")
+        except Exception as e:
+            fig = hs.create_error_placeholder(e)
         return fig
 
     def create_mism_types_plot(self) -> go.Figure:
         """
         Create a heatmap plot visualizing mismatch types.
 
         Returns:
         go.Figure:
             A Plotly figure representing the mismatch types heatmap.
 
         The method generates a heatmap plot that visualizes mismatch types between called and reference bases.
         The x-axis represents the called bases, the y-axis represents the reference bases, and the color
         represents the count of occurrences for each mismatch type. The plot is customized for clear visualization.
         """
-        matrix_data, matrix_labels, matrix_max_mism = self.prepare_data_mism_types()
+        mis_count = self.prepare_data_mism_types()
 
-        fig = px.imshow(matrix_data, labels=dict(x="Called base", y="Reference base", color="Count"), zmin=0, zmax=1.2*matrix_max_mism, color_continuous_scale="portland")
-        fig = self.update_plot(fig, None, "Called base", "Reference base", width=800)
-        fig.update_traces(text=matrix_labels, texttemplate="%{text}")
-        fig.update_xaxes(fixedrange=True, tickvals=[0,1,2,3],ticktext=["A", "C", "G", "U"])
-        fig.update_yaxes(fixedrange=True, tickvals=[0,1,2,3],ticktext=["A", "C", "G", "U"])
-        
+        try:
+            fig = go.Figure()
+            fig = hs.update_plot(fig, ylab="Reference base", xlab="Called base")
+            counts = [[mis_count[row][col] for col in ["A", "C", "G", "U", "Del"]] for row in ["A", "C", "G", "U"]]
+            heatmap = go.Heatmap(x=["A", "C", "G", "U", "Del"],
+                                y=["A", "C", "G", "U"],
+                                z=counts,
+                                colorscale="portland",
+                                hoverinfo="z",
+                                hovertemplate="%{y}-%{x}<br>Count: %{z}",
+                                name="",
+                                colorbar=dict(title="Count"))
+            heatmap.update(dict(showscale=True))
+            fig.add_trace(heatmap)
+            # Add text annotations
+            total_count = sum([sum(mis_count[row].values()) for row in mis_count.keys()])
+            annotations = []
+            for i, row in enumerate(["A", "C", "G", "U"]):
+                for j, col in enumerate(["A", "C", "G", "U", "Del"]):
+                    # add black border around each cell
+                    fig.add_shape(type="rect",
+                            x0=j - 0.5, y0=i - 0.5,
+                            x1=j + 0.5, y1=i + 0.5,
+                            line=dict(color="#000000", width=1),
+                            fillcolor="rgba(0,0,0,0)",
+                            xref="x", yref="y")
+                    # add percent values as annotations to each cell
+                    annotations.append(
+                        dict(
+                            x=j, y=i,
+                            text=f"{(mis_count[row][col] / total_count)*100:.2f}%",
+                            showarrow=False,
+                            font=dict(color="#000000"),
+                            xref="x",
+                            yref="y"
+                        )
+                    )
+            fig.update_layout(annotations=annotations)
+        except Exception as e:
+            fig = hs.create_error_placeholder(e)
         return fig
 
-    def create_composition_plot(self) -> go.Figure:
+    def create_composition_plot(self) -> Tuple[go.Figure, str]:
         """
-        Create a stacked bar plot visualizing composition rates for different bases.
+        Creates a figure displaying the base compositions at positions of interest and their corresponding
+        canonical counterpart bases (if specified). Also sets up an HTML table to display the statistical
+        comparisons between the base rates of the different groups.
 
         Returns:
-        go.Figure:
-            A Plotly figure representing the composition rates stacked bar plot.
+        - go.Figure: Base composition figure
+        - str: String representation of the HTML table containing adjusted p-values
+        """
+        median_base_rates_scaled, median_base_rates, x_vals, fdrs = self.prepare_data_composition()
+        try:
+            keys = median_base_rates_scaled.keys()
 
-        The method generates a stacked bar plot that visualizes the composition rates
-        for different bases in various conditions. The x-axis represents different conditions,
-        and the y-axis represents the relative abundance of each base. The plot is customized
-        for clear visualization, including colors, tooltips, and layout adjustments.
-        """
-        median_base_rates_scaled, median_base_rates, x_vals = self.prepare_data_composition()
-
-        bar_a = go.Bar(x=x_vals, y=median_base_rates_scaled["A"], name="A", marker=dict(color="#2ca02c"), customdata=median_base_rates["A"], hovertemplate="Scaled median rate: %{y}<br>Unscaled median rate: %{customdata}")
-        bar_c = go.Bar(x=x_vals, y=median_base_rates_scaled["C"], name="C", marker=dict(color="#1f77b4"), customdata=median_base_rates["C"], hovertemplate="Scaled median rate: %{y}<br>Unscaled median rate: %{customdata}")
-        bar_g = go.Bar(x=x_vals, y=median_base_rates_scaled["G"], name="G", marker=dict(color="#ff7f0e"), customdata=median_base_rates["G"], hovertemplate="Scaled median rate: %{y}<br>Unscaled median rate: %{customdata}")
-        bar_u = go.Bar(x=x_vals, y=median_base_rates_scaled["U"], name="U", marker=dict(color="#d62728"), customdata=median_base_rates["U"], hovertemplate="Scaled median rate: %{y}<br>Unscaled median rate: %{customdata}")
-        
-        fig = self.update_plot(go.Figure(), ylab="Relative abundance", height=600, width=1000)
-        fig.add_traces([bar_a, bar_c, bar_g, bar_u])
-        fig.update_layout(barmode="stack")
-        fig.update_traces(marker=dict(line=dict(color="black", width=1.5)))
+            fig = go.Figure()
+            fig = hs.update_plot(go.Figure(), ylab="Relative abundance", height=600, width=1200)
+
+            bars = []
+            for feature, color in [("A", "#2ca02c"), ("C", "#1f77b4"), ("G", "#ff7f0e"), ("U", "#d62728")]:
+                bar = go.Bar(x=x_vals, y=[median_base_rates_scaled[i][feature] for i in keys], name=feature, marker=dict(color=color), customdata=[median_base_rates[i][feature] for i in keys], hovertemplate="Scaled median rate: %{y}<br>Unscaled median rate: %{customdata}")
+                bars.append(bar)
+
+            fig.add_traces(bars)
+            fig.update_layout(barmode="stack")
+            fig.update_traces(marker=dict(line=dict(color="black", width=1.5)))
+        except Exception as e:
+            fig = hs.create_error_placeholder(e)
+
+        stat_results_table = self.create_stat_table(fdrs)
+
+        return fig, stat_results_table
 
-        return fig
-    
     def create_error_rate_plot(self) -> Tuple[go.Figure, str]:
         """
         Create a grouped box plot visualizing error rates and quality scores.
-
-        Returns:
-        Tuple[go.Figure, str]:
-            A tuple containing the Plotly figure representing the box plot and a string
-            with a table summarizing statistical test results.
-
-        The method generates a grouped box plot that visualizes error rates and quality scores
-        for different conditions. The x-axis represents different conditions, and the y-axis represents
-        the error rate or quality score. The plot includes statistical tests and a table summarizing
-        p-values for various comparisons.
-        """
-        data_mismatch, data_deletion, data_insertion, data_ref_skip, data_quality, x_ticks = self.prepare_data_errorrates()
-
-        p_val_table = self.create_test_overview([data_mismatch, data_deletion, data_insertion, data_ref_skip, data_quality])
-
-        box_mismatch = go.Box(x=data_mismatch["x"], y=data_mismatch["y"], name="Mismatch rate", offsetgroup=0, line=dict(color="black"), marker=dict(outliercolor="black", size=2), fillcolor="#8c564b")
-        box_deletion = go.Box(x=data_deletion["x"], y=data_deletion["y"], name="Deletion rate", offsetgroup=1, line=dict(color="black"), marker=dict(outliercolor="black", size=2), fillcolor="#e377c2")
-        box_insertion = go.Box(x=data_insertion["x"], y=data_insertion["y"], name="Insertion rate", offsetgroup=2, line=dict(color="black"), marker=dict(outliercolor="black", size=2), fillcolor="#7f7f7f")
-        box_ref_skip = go.Box(x=data_ref_skip["x"], y=data_ref_skip["y"], name="Reference skip", offsetgroup=3, line=dict(color="black"), marker=dict(outliercolor="black", size=2), fillcolor="#bcbd22")
+        Generates a grouped box plot that visualizes error rates and quality scores for different groups. 
+        The x-axis represents different conditions, and the y-axis represents the error rate or quality 
+        score.
         
-        box_quality = go.Box(x=data_quality["x"], y=data_quality["y"], name="Mean quality", offsetgroup=0, line=dict(color="black"), marker=dict(outliercolor="black", size=2), fillcolor="#17becf")
+        Returns:
+        - go.Figure: Plotly figure representing the box plots
+        - str: HTML table summarizing statistical test results
+
+        The method 
+        """
+        error_rates, x_vals, stat_comp_results = self.prepare_data_errorrates()
+        try:
+            fig = make_subplots(rows=1, cols=2, column_widths=[0.75, 0.25])
+            fig = hs.update_plot(fig, height=800, width=1200)
 
-        fig = self.update_plot(make_subplots(rows=1, cols=2, column_widths=[0.75, 0.25]), height=800, width=1200)
-        fig.add_traces([box_mismatch, box_deletion, box_insertion, box_ref_skip], rows=[1,1,1,1], cols=[1,1,1,1])
-        fig.add_trace(box_quality, row=1, col=2)
-        fig.update_layout(boxmode="group")
-        fig.update_yaxes(title_text="Error rate", row = 1, col = 1)
-        fig.update_yaxes(title_text="Quality score", row = 1, col = 2)
-        fig.update_xaxes(tickvals=[0,1,2,3],ticktext=x_ticks)
+            boxes = []
+            for offset, (feature, color) in enumerate([("Mismatch rate", "#8c564b"), ("Deletion rate", "#e377c2"), ("Insertion rate", "#7f7f7f"), ("Reference skip rate", "#bcbd22")]):
+                box = go.Box(x=x_vals, y=error_rates[feature], name=feature, offsetgroup=offset, line=dict(color="black"), marker=dict(outliercolor="black", size=2), fillcolor=color)
+                boxes.append(box)
+            fig.add_traces(boxes, rows=[1]*4, cols=[1]*4)
+
+            box = go.Box(x=x_vals, y=error_rates["Mean q-score"], name="Mean q-score", offsetgroup=0, line=dict(color="black"), marker=dict(outliercolor="black", size=2), fillcolor="#17becf")
+            fig.add_trace(box, row=1, col=2)
+
+            fig.update_layout(boxmode="group")
+            fig.update_yaxes(title_text="Error rate", row = 1, col = 1)
+            fig.update_yaxes(title_text="Quality score", row = 1, col = 2)
+        except Exception as e:
+            fig = hs.create_error_placeholder(e)
+
+        p_val_table = self.create_stat_table(stat_comp_results)
 
         return fig, p_val_table
+
     
     def create_nb_plot(self) -> go.Figure:
         """
         Create a neighbor position plot for a specified modification type.
 
         Returns:
             go.Figure: A Plotly figure representing the bar and pie plot.
@@ -914,28 +1094,30 @@
         the plot, generates stacked bar charts for neighbor positions with and without modification errors,
         as well as a pie chart showing the distribution of surrounding errors, using Plotly, and returns the
         resulting plot as HTML code.
 
         """
         x_vals, y_vals, x_vals_mod, y_vals_mod, pie_labs, pie_vals = self.prepare_nb_counts()
 
-        fig = self.update_plot(make_subplots(rows=1, cols=2, column_widths=[0.75, 0.25], specs=[[{"type": "bar"}, {"type": "pie"}]]), width=1200)
+        try:
+            fig = hs.update_plot(make_subplots(rows=1, cols=2, column_widths=[0.75, 0.25], specs=[[{"type": "bar"}, {"type": "pie"}]]), width=1200)
 
-        fig.add_trace(go.Bar(x=x_vals, y=y_vals, marker=dict(color="#d62728", line=dict(color='#000000', width=1.5)), name="nb. error"), row=1, col=1)
-        fig.add_trace(go.Bar(x=x_vals_mod, y=y_vals_mod, marker=dict(color="#dd8452", line=dict(color='#000000', width=1.5)), name="nb. mod error"), row=1, col=1)
-        fig.update_layout(barmode="stack")
+            fig.add_trace(go.Bar(x=x_vals, y=y_vals, marker=dict(color="#d62728", line=dict(color='#000000', width=1.5)), name="nb. error"), row=1, col=1)
+            fig.add_trace(go.Bar(x=x_vals_mod, y=y_vals_mod, marker=dict(color="#dd8452", line=dict(color='#000000', width=1.5)), name="nb. mod error"), row=1, col=1)
+            fig.update_layout(barmode="stack")
 
-        fig.update_xaxes(title = f"Relative position to {self.current_category} positions", row=1, col=1)
-        fig.update_yaxes(title = "Count", row=1, col=1)
+            fig.update_xaxes(title = f"Relative position to {self.current_category} positions", row=1, col=1)
+            fig.update_yaxes(title = "Count", row=1, col=1)
 
-        fig.add_trace(go.Pie(labels=pie_labs, values=pie_vals, name="", 
-                            marker=dict(colors=["#4c72b0", "#d62728", "#dd8452"], line=dict(color='#000000', width=1.5))), row=1, col=2)
+            fig.add_trace(go.Pie(labels=pie_labs, values=pie_vals, name="", 
+                                marker=dict(colors=["#4c72b0", "#d62728", "#dd8452"], line=dict(color='#000000', width=1.5))), row=1, col=2)
 
-        fig.update_layout(showlegend=False)
-        
+            fig.update_layout(showlegend=False)
+        except Exception as e:
+            fig = hs.create_error_placeholder(e)
         return fig    
     
     ##############################################################################################################
     #                                               Output methods                                               #
     ##############################################################################################################
     def write_svg(self, fig: go.Figure, name: str, output_path) -> None:
         """
@@ -1024,99 +1206,121 @@
                         with <b>{self.current_category}</b> positions extracted from file <b>{self.bed_path}</b>. 
                         The plots are interactive and allow further information by hovering, zooming and panning.
                     </p>
                 </section>
 
                 
                 <section>
-                    <button class="collapsible">{name} positions on reference sequence(s)</button>
+                    <button class="collapsible">{name} positions - general information</button>
                     <div class="collapsible-content">
                         <h2 class="hiddentitle" id="map"></h2>
 
                         <h3>Mapping of {name} positions across the reference sequences</h3>
                         <div class="plot-container">
                             {plots[0]}
                         </div>
                         <p>
-                            Positions of {name} are indicated as blue lines. Fasta file '{self.ref_path}' was used to extract
-                            reference sequence(s). Hover on positions for exact coordinates. 
+                            Map of sequences containing positions of interest. Sequences are binned into {self.n_bins_seqmap} chunks.
+                            Number of {name} positions in each chunk are indicated by the coloring. Fasta file '{self.ref_path}' 
+                            was used to extract reference sequence(s). Hover on positions for exact coordinates. 
                         </p>
+
+                        <h3>Motifs at {name} positions</h3>
+                        <div class="plot-container">
+                            {plots[1]}
+                        </div>
+                        <p>
+                            Motif compositions around {name} sites. Hover for the count of a base at each relative position in the kmer. 
+                        </p>
+
                     </div>
                 </section>
 
                 <section>
                     <button class="collapsible">Mismatch types</button>
                     <div class="collapsible-content">
                         <h2 class="hiddentitle" id="mismatch_types"></h2>
                         
                         <h3>Confusion matrix of {name} positions containing mismatch types</h3>
                         <div class="plot-container">
-                            {plots[1]}
+                            {plots[2]}
                         </div>
                         <p>
-                            Overview of all types of (mis-)matches in the data subset corresponding to {name}.
+                            Abundances of (mis-)match types at {name} sites. Hover for absolute counts.
                         </p>
                     </div>
                 </section>
 
                 <section>
                     <button class="collapsible">Base compositions</button>
                     <div class="collapsible-content">
                         <h2 class="hiddentitle" id="base_comp"></h2>
 
                         <h3>Base compositions for different {name} {f"and {self.current_counterpart} " if self.current_counterpart else ""}subsets</h3>
                         <div class="plot-container">
-                            {plots[2]}
+                            {plots[3]}
                         </div>
                         <p>
                             Each A/C/G/U element in the bars corresponds to the median count of a given base in a subset. The four medians were scaled to add up to one. 
                             {name} match: positions labelled {name} from the bed file, where the called base is equal to the reference base. 
                             {f"{self.current_counterpart} match: positions with reference base {self.current_counterpart}, where the called base is equal." if self.current_counterpart else ""}
                             {name} mismatch: positions labelled {name} from the bed file, where the called base differs from the reference base. 
                             {f"{self.current_counterpart} mismatch: positions with reference base {self.current_counterpart} , where the called base differs." if self.current_counterpart else ""}
                         </p>
+
+                        <h3>Statistical comparisons of base rates from {name} {f"and {self.current_counterpart} " if self.current_counterpart else ""}subsets</h3>
+                        <p>
+                            False discovery rates (FDRs) from statistical tests between the A, C, G and U rates of different groups. "TT"=t-test for independent samples. "MWU"=Mann-Whitney-U test.
+                            t-Tests are performed if both samples of a given comparison are normally distributed and the variances do not differ significantly.
+                        </p>
+                        <div class="table-box">
+                            {tables[0]}
+                        </div>
+
                     </div>
                 </section>
 
                 <section>
                     <button class="collapsible">Error rates</button>
                     <div class="collapsible-content">
                         <h2 class="hiddentitle" id="error_rates"></h2>
 
                         <h3>Error rates for different {name} {f"and {self.current_counterpart} " if self.current_counterpart else ""}subsets</h3>
                         <div class="plot-container">
-                            {plots[3]}
+                            {plots[4]}
                         </div>
                         
                         <p>
                             Left: Distributions of mismatch, deletion, insertion and reference skip rates for different subsets. Right: Distribution of mean quality scores for different subsets. 
                             {name} match: positions labelled {name} from the bed file, where the called base is equal to the reference base. 
                             {f"{self.current_counterpart} match: positions with reference base {self.current_counterpart}, where the called base is equal." if self.current_counterpart else ""}
                             {name} mismatch: positions labelled {name} from the bed file, where the called base differs from the reference base. 
                             {f"{self.current_counterpart} mismatch: positions with reference base {self.current_counterpart} , where the called base differs." if self.current_counterpart else ""}
                         </p>
+
+                        <h3>Statistical comparisons of error rates from {name} {f"and {self.current_counterpart} " if self.current_counterpart else ""}subsets</h3>
                         <p>
-                            The table below shows p-values for statistical tests between the four groups for different error rate
-                            the mean quality distributions. 
+                            False discovery rates (FDRs) from statistical tests between the mismatch, insertion deletion and reference skip rates of different groups. "TT"=t-test for independent 
+                            samples. "MWU"=Mann-Whitney-U test. t-Tests are performed if both samples of a given comparison are normally distributed and the variances do not differ significantly.
                         </p>
                         <div class="table-box">
-                            {tables[0]}
+                            {tables[1]}
                         </div>
 
                     </div>
                 </section>
 
                 <section>
                     <button class="collapsible">Neighbouring errors</button>
                     <div class="collapsible-content">
                         <h2 class="hiddentitle" id="nb_errors"></h2>
 
                         <h3>Count of positions with high error rate in the surrounding of {name} positions</h3>
                         <div class="plot-container">
-                            {plots[4]}
+                            {plots[5]}
                         </div>
                         <p>
                             Left: Occurences of high mismatch rates two bases up- and downstream from {name} positions.
                             Right: Pie chart shows the (relative count) of different types of central {name} positions. 
                             Red indicates errors in the surrounding positions where the position in question
                             is also of type {name}. The count of surrounding error positions that do not fall under {name}
                             are colored orange. Blue corresponds to {name} positions where no surrounding errors are found.
@@ -1145,30 +1349,39 @@
             </body>
             <footer></footer>
             </html> 
         """
         with open(output_path, "w") as out:
             out.write(template)
 
-    def write_tsv(self) -> None:
+    def write_tsv(self) -> str:
         """
         Write the processed data to a tab-separated values (TSV) file.
 
         The method writes the processed data, stored in the class attribute 'data', to a TSV file.
         The file will be named based on the input file path, and the suffix '_w_bed_info.tsv' will
         be added to indicate that bed information has been appended to the original data.
 
         Parameters:
         None
 
         Returns:
-        None
+        - str: path to the newly written file
 
         Example:
         If self.in_path = "input_folder/example.txt", the output TSV file will be named
         "input_folder/example_w_bed_info.tsv".
         """
-        with open(f"{os.path.splitext(self.in_path)[0]}_w_bed_info.tsv", "w") as out:
+        outpath = f"{os.path.splitext(self.in_path)[0]}_w_bed_info.tsv"
+        with open(outpath, "w") as out:
             out.write("\t".join(self.data.keys())+"\n")
             for vals in zip(*self.data.values()):
                 vals = [str(val) for val in vals]
-                out.write("\t".join(vals)+"\n")
+                out.write("\t".join(vals)+"\n")
+        return outpath
+
+if __name__=="__main__":
+    p = POISummary(in_path="/home/vincent/projects/neet_project/data/45s_rrna/test/drna_cyt_extracted.tsv",
+                    bed_path="/home/vincent/projects/neet_project/data/45s_rrna/rRNA_modifications_conv_cleaned.bed",
+                    ref_path="/home/vincent/projects/neet_project/data/45s_rrna/RNA45SN1.fasta",
+                    categories="psu", canonical_counterpart="U", output_tsv=False)
+    p.main()
```

### Comparing `neet-nanopore-0.0.4/neet/position_summary.py` & `neet_nanopore-1.0.0/neet/poi_view.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,85 +1,78 @@
-from . import helper_functions as hs
 from typing import Tuple, List, Dict
-import argparse, os, warnings, datetime
+import os, datetime
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
+from tqdm import tqdm
 
-class PositionSummary:
-    positions: List[Tuple[str, int]]
+try: # when invoked from the package
+    from neet import helper_functions as hs
+except ImportError: # when invoked directly
+    import helper_functions as hs
+
+SITE = Tuple[str, int]
+
+class POIView:
+    positions: List[SITE]
     nb_size: int
 
     basename_a: str
-    basename_b: str
+    basename_b: str | None
     
     paths_a: List[str]
-    paths_b: List[str]
-
+    paths_b: List[str] | None
     bed_path: str
-
     out_dir: str
-    """
-    Data structure:
-    data_sample_a
-        position1{[
-            replicate1[
-                [chr, site, ...] (pos-nb_size)
-                ...
-                [chr, site, ...] (pos)
-                ...
-                [chr, site, ...] (pos+nb_size)
-                ],
-            replicate2[
-                ...
-                ],
-            ...
-            replicaten[
-                ...
-                ]
-            ]}
-        position2{
-        ...
-        }
-        ...
-        positionn{
-        ...
-        }
-    """
-    data_sample_a: Dict[Tuple[chr, int], List[List[List[str]]]]
-    data_sample_b: Dict[Tuple[chr, int], List[List[List[str]]]]
+
+    # see get_data method for details
+    data: Dict[str, Dict[str, Dict[SITE, List[str]]]]
 
     export_svg: bool
 
     colors = {"A": "#2ca02c", "C": "#1f77b4", "G": "#ff7f0e", "U": "#d62728", 
               "match": "#9467bd", "mis": "#8c564b", "del": "#e377c2", 
               "ins": "#7f7f7f", "ref_skip": "#7f7f7f"}
 
-    def __init__(self, paths_a: str, paths_b: str, basename_a: str, basename_b: str, bed_path: str, out_path: str, nb_size: int, export_svg: bool) -> None:
+    def __init__(self, 
+                 paths_a: str, 
+                 bed_path: str, 
+                 out_dir: str | None = None, 
+                 paths_b: str | None = None,
+                 basename_a: str = "sample_a", 
+                 basename_b: str = "sample_b", 
+                 nb_size: int = 2, 
+                 export_svg: bool = False) -> None:
         
         self.basename_a = basename_a
-        self.basename_b = basename_b
-
-        hs.check_create_dir(out_path)
-        self.out_dir = out_path
+        self.basename_b = basename_b if paths_b else None
 
         hs.check_input_path(bed_path, extensions=[".bed"])
         self.get_positions(bed_path)
-        self.bed_path = bed_path
+        self.bed_path = os.path.abspath(bed_path)
         self.basename_bed = os.path.splitext(os.path.basename(bed_path))[0]
         self.nb_size = nb_size
 
         self.export_svg = export_svg
 
-        paths_a = self.process_in(paths_a)
-        paths_b = self.process_in(paths_b)
-
-        self.paths_a = paths_a
-        self.paths_b = paths_b
+        paths_a_list = self.process_in(paths_a)
+        paths_b_list = self.process_in(paths_b) if paths_b else None
+        self.paths_a = paths_a_list
+        self.paths_b = paths_b_list
+
+        if out_dir:
+            out_dir = os.path.abspath(out_dir)
+            ext = os.path.splitext(out_dir)[1]
+            if ext:
+                hs.print_update(f"Warning: Extension {ext} was found. Make sure to provide a single output directory.")
+            hs.check_create_dir(out_dir)
+            self.out_dir = out_dir
+        else:
+            self.out_dir = os.path.dirname(self.paths_a[0])
 
-        self.get_data(paths_a, paths_b)
+        self.get_data(paths_a_list, paths_b_list)
 
     ##########################################################################################################
     #                                  Methods called during initialization                                  #
     ##########################################################################################################
     def process_in(self, in_paths: str) -> List[str]:
         """
         Process a comma-separated string of input file paths.
@@ -90,15 +83,15 @@
         Returns:
         - in_list (List[str]): A list of validated input file paths.
 
         Raises:
         - Exception: If any input file does not exist or has an unexpected file extension.
         - Exception: If input files are of different kinds (either .bam or .pileup). All files must be of the same kind.
         """
-        in_list = in_paths.split(",")
+        in_list = [os.path.abspath(p) for p in in_paths.split(",")]
         extensions = []
         for path in in_list:
             ext = os.path.splitext(path)[1]
             extensions.append(ext)
             hs.check_input_path(path, extensions=[".tsv"])
 
         if len(set(extensions)) > 1:
@@ -121,146 +114,112 @@
             for line in bed_file:
                 line = line.strip().split("\t")
                 chrom, site = line[0], int(line[2])
                 positions.append((chrom, site))
             hs.print_update(f"Found {len(positions)} sites.", with_time=False)
             self.positions = positions
 
-    def get_data(self, paths_a: List[str], paths_b: List[str]) -> None:
+    def get_data(self, paths_a: List[str], paths_b: List[str] | None) -> None:
         """
-        Process input files to extract relevant data for both samples.
+        Process input files to extract relevant data for both samples. Stores the data in a nested Dictionary of 
+        the following format: Dict[str, Dict[str, Dict[Tuple[str, int], List[str]]]]
+        - first level: sample
+        - second level: replicate
+        - third level: position (seq, site)
+        
+        For example, features of site (chrA, 100) in replicate 1 and sample A can be accessed via data[A][1][(chrA,100)].
 
         Parameters:
         - paths_a (List[str]): List of input file paths for sample A.
         - paths_b (List[str]): List of input file paths for sample B.
 
         Returns:
         - None
         """
-        def process_sample(paths: List[str]) -> List[List[List[str]]]:
-            target_sites = set([(position[0], position[1]+i) for i in range(-self.nb_size, self.nb_size+1) for position in self.positions])
-
-            rep_data = []
-            for path in paths:
-                with open(path, "r") as file:
-                    data_collection = {}
+        target_sites = set([(seq, site+i) for i in range(-self.nb_size, self.nb_size+1) for seq, site in self.positions])
+        samples = [self.basename_a, self.basename_b]
+        paths = [paths_a, paths_b]
+        # collect data from given feature tables by sample (first level), replicates (second level) and position (seq, site) (third level)
+        data = {}
+        for sample, paths in zip(samples, paths):
+            if sample: # skip sample b if it is not given
+                data[sample] = {}
+                for replicate, path in [(f"{sample} {i}", path) for i, path in enumerate(paths, start=1)]:
+                    data[sample][replicate] = {}
                     hs.print_update(f"Processing file {path}")
-                    next(file)
-                    for line in file:
-                        line = line.strip().split("\t")
-                        current_pos = line[0], int(line[1])
-                        if (current_pos[0], current_pos[1]) in target_sites:
-                            data_collection[current_pos] = line
-                    rep_data.append(data_collection)
-                                
-            position_data = {}
-            for position in self.positions:
-                data_ordered = []
-                for rep in rep_data:
-                    data = [None] * (2 * self.nb_size + 1)
-
-                    sites = [position[1]+i for i in range(-self.nb_size, self.nb_size+1)]
-                    neighbour_positions = [(position[0], site) for site in sites]
-                    for neighbour_position in neighbour_positions:
-                        if neighbour_position in rep.keys():
-                            data_index = neighbour_position[1] - position[1] + self.nb_size
-                            data[data_index] = rep[neighbour_position]
-                    data_ordered.append(data)
-
-                position_data[position] = data_ordered
-            
-            return position_data
-        
-        self.data_sample_a = process_sample(paths_a)
-        self.data_sample_b = process_sample(paths_b)
+                    with open(path, "r") as file:
+                        next(file)
+                        for line in file:
+                            line = line.strip().split("\t")
+                            current_pos = line[0], int(line[1])
+                            if (current_pos[0], current_pos[1]) in target_sites:
+                                data[sample][replicate][current_pos] = line
+        self.data = data
 
     ##########################################################################################################
     #                                    Methods called for plot creation                                    #
     ##########################################################################################################
-    def update_plot(self, fig, title: str|None = None, xlab: str|None = None, ylab: str|None = None, height: int = 500, width: int = 800):
-        """
-        Updates the layout of a Plotly figure.
-
-        Args:
-            fig (go.Figure): The Plotly figure to be updated.
-            title (str|None): Title of the plot (optional).
-            xlab (str|None): Label for the x-axis (optional).
-            ylab (str|None): Label for the y-axis (optional).
-            height (int): Height of the plot (default: 500).
-            width (int): Width of the plot (default: 800).
-
-        Returns:
-            go.Figure: The updated Plotly figure.
-        """
-        fig.update_layout(template="seaborn",
-                    title = title,
-                    xaxis_title = xlab,
-                    yaxis_title = ylab,
-                    font=dict(family="Open sans, sans-serif", size=20),
-                    plot_bgcolor="white",
-                    margin=dict(l=50, r=50, t=50, b=50),
-                    height=height,  # Set the height to a constant value
-                    width=width)
-        fig.update_xaxes(showline=True, linewidth=2, linecolor='black', mirror=True, showticklabels=True, ticks='outside', showgrid=False, tickwidth=2)
-        fig.update_yaxes(showline=True, linewidth=2, linecolor='black', mirror=True, showticklabels=True, ticks='outside', showgrid=False, tickwidth=2)
-
-        return fig
-
-
-    def create_bar_trace_base_composition(self, pos_data: List[str], x: int = 0, center: bool = True, show_legend: bool = False) -> List[go.Bar]:
+    def create_bar_trace_base_composition(self, pos_data: List[str]|None, x: int = 0, center: bool = True, show_legend: bool = False) -> List[go.Bar]:
         """
         Create a list of Plotly Bar traces for base composition visualization.
 
         Parameters:
         - pos_data (List[str]): List of position data.
         - x (int, optional): X-coordinate for the bars (default is 0).
         - center (bool, optional): Whether to center the bars at the specified x-coordinate (default is True).
         - show_legend (bool, optional): Whether to display legends for the bars (default is False).
 
         Returns:
         - List[go.Bar]: List of Plotly Bar traces.
         """
-        a, c, g, u = int(pos_data[5]), int(pos_data[6]), int(pos_data[7]), int(pos_data[8])
-        cvg = a+c+g+u
-        a_rel, c_rel, g_rel, u_rel = a/cvg, c/cvg, g/cvg, u/cvg
+        if pos_data:
+            a, c, g, u = int(pos_data[5]), int(pos_data[6]), int(pos_data[7]), int(pos_data[8])
+            cvg = a+c+g+u
+            a_rel, c_rel, g_rel, u_rel = a/cvg, c/cvg, g/cvg, u/cvg
+
+        else:
+            a, c, g, u = 0, 0, 0, 0
+            a_rel, c_rel, g_rel, u_rel = 0.0, 0.0, 0.0, 0.0
+            cvg = 0
+
         a_bar = go.Bar(x = [x], y = [a_rel], name = "A", 
                     marker = dict(color = self.colors["A"], line_color="black", line_width=1.5) if center else dict(color = self.colors["A"]), 
                     legendgroup = 1, 
                     opacity = 1 if center else 0.75, 
                     showlegend = show_legend, 
                     customdata = [[[a], [round(a_rel*100, 2)], [cvg]]], 
-                    hovertemplate = "n=%{customdata[0]} (%{customdata[1]}%)<br>Cvg=%{customdata[2]}",
+                    hovertemplate = "n=%{customdata[0]} (%{customdata[1]}%)<br>Total=%{customdata[2]}",
                     width=0.75)
         c_bar = go.Bar(x = [x], y = [c_rel], name = "C", 
                     marker = dict(color = self.colors["C"], line_color="black", line_width=1.5) if center else dict(color = self.colors["C"]), 
                     legendgroup = 2, 
                     opacity = 1 if center else 0.75, 
                     showlegend = show_legend, 
                     customdata = [[[c], [round(c_rel*100, 2)], [cvg]]], 
-                    hovertemplate = "n=%{customdata[0]} (%{customdata[1]}%)<br>Cvg=%{customdata[2]}",
+                    hovertemplate = "n=%{customdata[0]} (%{customdata[1]}%)<br>Total=%{customdata[2]}",
                     width=0.75)
         g_bar = go.Bar(x = [x], y = [g_rel], name = "G", 
                     marker = dict(color = self.colors["G"], line_color="black", line_width=1.5) if center else dict(color = self.colors["G"]),
                     legendgroup = 3, 
                     opacity = 1 if center else 0.75, 
                     showlegend = show_legend, 
                     customdata = [[[g], [round(g_rel*100, 2)], [cvg]]], 
-                    hovertemplate = "n=%{customdata[0]} (%{customdata[1]}%)<br>Cvg=%{customdata[2]}",
+                    hovertemplate = "n=%{customdata[0]} (%{customdata[1]}%)<br>Total=%{customdata[2]}",
                     width=0.75)
         u_bar = go.Bar(x = [x], y = [u_rel], name = "U", 
                     marker = dict(color = self.colors["U"], line_color="black", line_width=1.5) if center else dict(color = self.colors["U"]), 
                     legendgroup = 4, 
                     opacity = 1 if center else 0.75, 
                     showlegend = show_legend, 
                     customdata = [[[u], [round(u_rel*100, 2)], [cvg]]], 
-                    hovertemplate = "n=%{customdata[0]} (%{customdata[1]}%)<br>Cvg=%{customdata[2]}",
+                    hovertemplate = "n=%{customdata[0]} (%{customdata[1]}%)<br>Total=%{customdata[2]}",
                     width=0.75)
         return [a_bar, c_bar, g_bar, u_bar]
 
-    def create_bar_trace_error_rates(self, pos_data: List[str], x: int = 0, center: bool = True, show_legend: bool = False) -> List[go.Bar]:
+    def create_bar_trace_error_rates(self, pos_data: List[str] | None, x: int = 0, center: bool = True, show_legend: bool = False) -> List[go.Bar]:
         """
         Create a list of Plotly Bar traces for error rates visualization.
 
         Parameters:
         - pos_data (List[str]): List of position data.
         - x (int, optional): X-coordinate for the bars (default is 0).
         - center (bool, optional): Whether to center the bars at the specified x-coordinate (default is True).
@@ -268,100 +227,106 @@
 
         Returns:
         - List[go.Bar]: List of Plotly Bar traces.
         """        
         base_idx_rel = {"A": 12, "C": 13, "G": 14, "U": 15}
         base_idx_abs = {"A": 5, "C": 6, "G": 7, "U": 8}
 
-        n_match = int(pos_data[base_idx_abs[pos_data[3]]])
-        n_mismatch = int(pos_data[5]) + int(pos_data[6]) + int(pos_data[7]) + int(pos_data[8])
-        n_deletion = int(pos_data[9])
-        n_refskip = int(pos_data[11])
-
-        match_rate = float(pos_data[base_idx_rel[pos_data[3]]])
-        mismatch_rate = float(pos_data[19])
-        deletion_rate = float(pos_data[16])
-        refskip_rate = float(pos_data[18])
-
-        cvg = int(pos_data[2])
+        if pos_data:
+            n_match = int(pos_data[base_idx_abs[pos_data[3]]])
+            n_mismatch = int(pos_data[5]) + int(pos_data[6]) + int(pos_data[7]) + int(pos_data[8])
+            n_deletion = int(pos_data[9])
+            n_refskip = int(pos_data[11])
+
+            match_rate = float(pos_data[base_idx_rel[pos_data[3]]])
+            mismatch_rate = float(pos_data[19])
+            deletion_rate = float(pos_data[16])
+            refskip_rate = float(pos_data[18])
 
+            cvg = n_match + n_mismatch + n_deletion + n_refskip
+        else:
+            n_match, n_mismatch, n_deletion, n_refskip = 0, 0, 0, 0
+            match_rate, mismatch_rate, deletion_rate, refskip_rate = 0.0, 0.0, 0.0, 0.0
+            cvg = 0
+            
         match_bar = go.Bar(x = [x], y = [match_rate], name = "Match", 
                         marker = dict(color = self.colors["match"], line_color="black", line_width=1.5) if center else dict(color = self.colors["match"]), 
-                        legendgroup = 1, 
+                        legendgroup = 5, 
                         opacity = 1 if center else 0.75, 
                         showlegend = show_legend, 
                         customdata = [[[n_match], [round(match_rate*100, 2)], [cvg]]], 
-                        hovertemplate = "n=%{customdata[0]} (%{customdata[1]}%)<br>Cvg=%{customdata[2]}",
+                        hovertemplate = "n=%{customdata[0]} (%{customdata[1]}%)<br>Total=%{customdata[2]}",
                         width=0.75)
         mismatch_bar = go.Bar(x = [x], y = [mismatch_rate], name = "Mismatch", 
                             marker = dict(color = self.colors["mis"], line_color="black", line_width=1.5) if center else dict(color = self.colors["mis"]), 
-                            legendgroup = 2, 
+                            legendgroup = 6, 
                             opacity = 1 if center else 0.75, 
                             showlegend = show_legend, 
                             customdata = [[[n_mismatch], [round(mismatch_rate*100, 2)], [cvg]]], 
-                            hovertemplate = "n=%{customdata[0]} (%{customdata[1]}%)<br>Cvg=%{customdata[2]}",
+                            hovertemplate = "n=%{customdata[0]} (%{customdata[1]}%)<br>Total=%{customdata[2]}",
                             width=0.75)
         deletion_bar = go.Bar(x = [x], y = [deletion_rate], name = "Deletion", 
                             marker = dict(color = self.colors["del"], line_color="black", line_width=1.5) if center else dict(color = self.colors["del"]),
-                            legendgroup = 3, 
+                            legendgroup = 7, 
                             opacity = 1 if center else 0.75, 
                             showlegend = show_legend, 
                             customdata = [[[n_deletion], [round(deletion_rate*100, 2)], [cvg]]], 
-                            hovertemplate = "n=%{customdata[0]} (%{customdata[1]}%)<br>Cvg=%{customdata[2]}",
+                            hovertemplate = "n=%{customdata[0]} (%{customdata[1]}%)<br>Total=%{customdata[2]}",
                             width=0.75)
         refskip_bar = go.Bar(x = [x], y = [refskip_rate], name = "Reference skip", 
                             marker = dict(color = self.colors["ref_skip"], line_color="black", line_width=1.5) if center else dict(color = self.colors["ref_skip"]), 
-                            legendgroup = 4, 
+                            legendgroup = 8, 
                             opacity = 1 if center else 0.75, 
                             showlegend = show_legend, 
                             customdata = [[[n_refskip], [round(refskip_rate*100, 2)], [cvg]]], 
-                            hovertemplate = "n=%{customdata[0]} (%{customdata[1]}%)<br>Cvg=%{customdata[2]}",
+                            hovertemplate = "n=%{customdata[0]} (%{customdata[1]}%)<br>Total=%{customdata[2]}",
                             width=0.75)
         return [match_bar, mismatch_bar, deletion_bar, refskip_bar]
 
-    def create_bar_trace_insertion_rate(self, pos_data: List[str], x: int = 0, center: bool = True, show_legend: bool = False) -> List[go.Bar]:
+    def create_bar_trace_insertion_rate(self, pos_data: List[str] | None, x: int = 0, center: bool = True, show_legend: bool = False) -> List[go.Bar]:
         """
         Create a list of Plotly Bar traces for insertion rate visualization.
 
         Parameters:
         - pos_data (List[str]): List of position data.
         - x (int, optional): X-coordinate for the bars (default is 0).
         - center (bool, optional): Whether to center the bars at the specified x-coordinate (default is True).
         - show_legend (bool, optional): Whether to display legends for the bars (default is False).
 
         Returns:
         - List[go.Bar]: List of Plotly Bar traces.
-        """        
-        n_ins = int(pos_data[10])
-        ins_rate = float(pos_data[17])
-
-        cvg = int(pos_data[2])
+        """     
+        if pos_data:     
+            n_ins = int(pos_data[10])
+            ins_rate = float(pos_data[17])
+        else:
+            n_ins, ins_rate = 0, 0.0
 
         ins_bar = go.Bar(x = [x], y = [ins_rate], name = "Insertion", 
                         marker = dict(color = self.colors["ins"], line_color="black", line_width=1.5) if center else dict(color = self.colors["ins"]), 
-                        legendgroup = 1, 
+                        legendgroup = 9, 
                         opacity = 1 if center else 0.75, 
                         showlegend = show_legend, 
-                        customdata = [[[n_ins], [round(ins_rate*100, 2)], [cvg]]], 
-                        hovertemplate = "n=%{customdata[0]} (%{customdata[1]}%)<br>Cvg=%{customdata[2]}",
+                        customdata = [[[n_ins], [round(ins_rate*100, 2)]]], 
+                        hovertemplate = "n=%{customdata[0]} (%{customdata[1]}%)",
                         width=0.75)
         return [ins_bar]
 
-    def get_rep_bar_traces(self, data: List[List[str]], plot_type: str, showlegend: bool = False) -> List[go.Bar]:
+    def get_rep_bar_traces(self, data: List[List[str]|None], plot_type: str, showlegend: bool = False) -> List[go.Bar]:
         """
         Get a list of Plotly Bar traces for a replicate.
 
         Parameters:
         - data (List[List[str]]): List of data for a replicate.
         - plot_type (str): Type of plot (base_composition, error_rates, insertion_rate).
         - showlegend (bool, optional): Whether to display legends for the bars (default is False).
 
         Returns:
         - List[go.Bar]: List of Plotly Bar traces.
-        """        
+        """
         x_vals = range(-self.nb_size,self.nb_size+1)
         is_center_pos = [False]*self.nb_size + [True] + [False]*self.nb_size
         show_legend = is_center_pos if showlegend else [showlegend]*(2*self.nb_size+1)
 
         if plot_type == "base_composition":
             create_bar_func = self.create_bar_trace_base_composition
         elif plot_type == "error_rates":
@@ -370,95 +335,91 @@
             create_bar_func = self.create_bar_trace_insertion_rate
         else:
             raise Exception(f"Unknown plot type given: {plot_type}. Must be one of the following: base_composition, error_rates, insertion_rate")
         
         bar_traces = [create_bar_func(d, x, c, l) for d, x, c, l in zip(data, x_vals, is_center_pos, show_legend)]
         return [item for t in bar_traces for item in t]
 
-    def create_position_plots(self, data_a: List[List[List[str]]], data_b: List[List[List[str]]]) -> Tuple[go.Figure, go.Figure, go.Figure]:
+    def create_position_plots(self, position: SITE) -> go.Figure:
         """
-        Create Plotly plots for base composition, error rates, and insertion rates for each position.
+        Create Plotly plot containing showing base compositions, error rates, and insertion rates for each position.
 
         Parameters:
-        - data_a (List[List[List[str]]]): Data for sample A.
-        - data_b (List[List[List[str]]]): Data for sample B.
+        - position (Tuple[str, int]): Position for which the plot should be created.
 
         Returns:
-        - Tuple[str]: Tuple of HTML representations of the created plots.
+        - go.Figure: Plotly figure for position
         """        
-        n_rep_a = len(data_a)
-        n_rep_b = len(data_b)
+        n_rep_a = len(self.data[self.basename_a].keys())
+        n_rep_b = len(self.data[self.basename_b].keys()) if self.basename_b else 0
         n_samples = n_rep_a+n_rep_b
 
-        figs = []
-
-        for plot_type, width in zip(["base_composition", "error_rates", "insertion_rate"], [1200, 700, 500]):
-            fig = make_subplots(cols=1, rows=n_samples, shared_xaxes=True, vertical_spacing=0.02)
-            fig = self.update_plot(fig, height=200*(n_samples), width=width)
-
+        fig = make_subplots(cols=3, rows=n_samples, shared_xaxes=True, column_widths=[2,1,1])
+        height = 225*(n_samples) if n_samples>1 else 500
+        fig = hs.update_plot(fig, height=height, width=1200)
+
+        # Three columns correspond to the features that are displayed (base_composition, error_rates, insertion_rate)
+        # Half of the rows correspond to replicates of sample A, the other half to sample B
+        rep_labels = []
+        for col, plot_type in enumerate(["base_composition", "error_rates", "insertion_rate"], start=1):
             current_row = 1
-            for rep in data_a:
-                bars = self.get_rep_bar_traces(rep, plot_type=plot_type, showlegend=True) if current_row==1 else self.get_rep_bar_traces(rep, plot_type=plot_type)
-                fig.add_traces(bars, rows=[current_row for _ in range(len(bars))], cols=[1 for _ in range(len(bars))])
-                current_row += 1
-            for rep in data_b:
-                bars = self.get_rep_bar_traces(rep, plot_type=plot_type)
-                fig.add_traces(bars, rows=[current_row for _ in range(len(bars))], cols=[1 for _ in range(len(bars))])
-                current_row += 1
-            fig.update_layout(barmode="stack")
-
-            y_labels = [f"{self.basename_a} {i}" for i in range(1,n_rep_a+1)] + [f"{self.basename_b} {i}" for i in range(1,n_rep_b+1)]
-            for i in range(n_samples):
-                fig.update_yaxes(title=y_labels[i], row=i+1, col=1)
-                
+            for sample in [self.basename_a, self.basename_b]:
+                if sample: # skip sample b if it is not given
+                    for rep in self.data[sample].keys():
+                        rep_labels.append(rep)
+                        # get the data for the position itself and nb_size number of positions up- and downstream
+                        position_data = [self.data[sample][rep][(position[0], position[1]+i)] if (position[0], position[1]+i) in self.data[sample][rep].keys() else None for i in range(-self.nb_size, self.nb_size+1)]
+                        bars = self.get_rep_bar_traces(position_data, plot_type=plot_type, showlegend=True) if current_row==1 else self.get_rep_bar_traces(position_data, plot_type=plot_type)
+                        fig.add_traces(bars, rows=[current_row]*len(bars), cols=[col]*len(bars))
+                        current_row += 1
+        fig.update_layout(barmode="stack", legend_tracegroupgap=0) # reduce spacing between legend items 
+        
+        # Update y ticklabels (show only for first column)
+        for i in range(n_samples):
+            fig.update_yaxes(title=rep_labels[i], row=i+1, col=1)
+        
+        # Update x ticklabels (show only for last row and show the bases instead of coordinates)
+        x_ticks = [d[3] if d else "N" for d in position_data] # type: ignore dont see how it can be unbound...
+        for col in range(1,4):
             for i in range(1, n_samples):
-                fig.update_xaxes(tickvals=[], ticktext=[], row=i, col=1)
-            fig.update_xaxes(tickvals=list(range(-self.nb_size,self.nb_size+1)), ticktext=[d[3] for d in data_a[0]], row=n_samples, col=1)
+                fig.update_xaxes(tickvals=[], ticktext=[], row=i, col=col)
+            fig.update_xaxes(tickvals=list(range(-self.nb_size,self.nb_size+1)), ticktext=x_ticks, row=n_samples, col=col)
 
-            figs.append(fig)
-        return tuple(figs)
-    
-    def create_html_section(self, position: Tuple[str, int], plots: Tuple[go.Figure, go.Figure, go.Figure]) -> str:
+        return fig
+
+    def create_html_section(self, position: SITE, plot: go.Figure) -> str:
         """
         Create an HTML section for a genomic position with embedded plots.
 
         Parameters:
         - position (Tuple[str, int]): Genomic position (chromosome, site).
-        - plots (Tuple[str, str, str]): Tuple of HTML representations for base composition, error rates, and insertion rates.
+        - plot (go.Figure): Plotly figure showing base composition, error rates, and insertion rates at the given position.
 
         Returns:
         - str: HTML section for the genomic position with embedded plots.
         """
         chrom, site = position[0], position[1]
     
-        plot_base_comp = plots[0].to_html(include_plotlyjs=False)
-        plot_err_rates = plots[1].to_html(include_plotlyjs=False)
-        plot_ins_rate = plots[2].to_html(include_plotlyjs=False)
+        plot_str = plot.to_html(include_plotlyjs=False)
 
         collapsible_section = f"""
             <section>
                 <button class="collapsible">{chrom}:{site}</button>
 
                 <div class="collapsible-content">
                 <h2 class="hiddentitle" id="{chrom}_{site}"></h2>
 
-                    <h3>Base compositions</h3>
-                    <div class="plot-container">
-                        {plot_base_comp}
-                    </div>
-
-                    <h3>Error rates</h3>
+                    <h3>Base compositions and error rates</h3>
                     <div class="plot-container">
-                        <div id="left">
-                            {plot_err_rates}
-                        </div>
-                        <div id="right">
-                            {plot_ins_rate}
-                        </div>
+                        {plot_str}
                     </div>
+                    <p>
+                        Base- (left) and error (middle, right) compositions {self.nb_size} bases up- and downstream around position {chrom}, {site}.
+                        Hover for detailed information about coverage, absolute and relative counts. 
+                    </p>
                 </div>
             </section>
         """
         return collapsible_section
 
     def get_file_paths(self) -> Tuple[str, str]:
         """
@@ -471,84 +432,82 @@
         def create_list(paths: List[str]):
             path_list = "<ul>"
             for path in paths:
                 path_list += f"<li>{path}</li>"
             path_list += "</ul>"
             return path_list
         
-        return create_list(self.paths_a), create_list(self.paths_b)
+        list_a = create_list(self.paths_a)
+        list_b = create_list(self.paths_b) if self.paths_b else ""
+        return list_a, list_b
 
-    def write_svg(self, figs: Tuple[go.Figure, go.Figure, go.Figure], position: Tuple[str, int], output_dir: str) -> None:
+    def write_svg(self, fig: go.Figure, position: SITE, output_dir: str) -> None:
         """
         Write the three plots (base composition, error rates and insertion rates) to three separate SVG files in
         output_dir. The name of the file is in the following format: <chr>_<coordinate>_<plot-type>.svg
         All plots are written to the directory created beforehand.
 
         Parameters:
         - figs (Tuple[go.Figure, go.Figure, go.Figure]): Plotly figures of base composition, error rates and insertion rates
         - positions (Tuple[str, int]): Genomic position (chromosome, site).
         - output_dir (str): Output directory as created beforehand in main method.
 
         Returns:
         - None
         """
-        for fig, fig_type in zip(figs, ["base_composit", "error_rates", "insertion_rates"]):
-            outpath = os.path.join(output_dir, f"{position[0]}_{position[1]}_{fig_type}.svg")
-            fig.write_image(outpath)
+        outpath = os.path.join(output_dir, f"{position[0]}_{position[1]}_overview.svg")
+        fig.write_image(outpath)
 
-    def main(self) -> str:
+    def main(self) -> None:
         """
         Main method to generate the HTML summary report.
-
-        Returns:
-        - str: File path to the generated HTML summary report.
         """
         collapsible_sections = ""
 
         if self.export_svg:
-            export_dir = os.path.join(self.out_dir, f"{self.basename_a}_{self.basename_b}_{self.basename_bed}") 
+            filename = f"{self.basename_a}_{self.basename_b}_{self.basename_bed}" if self.basename_b else f"{self.basename_a}_{self.basename_bed}"
+            export_dir = os.path.join(self.out_dir, filename) 
             os.makedirs(export_dir, exist_ok=True)
-
-        for (position_a, data_a), (position_b, data_b) in zip(self.data_sample_a.items(), self.data_sample_b.items()):
-            plots = self.create_position_plots(data_a, data_b)
+        for position in tqdm(self.positions, total=len(self.positions), desc="Creating plots"):
+            plot = self.create_position_plots(position)
             if self.export_svg:
-                self.write_svg(plots, position_a, export_dir)
-            collapsible_sections += self.create_html_section(position_a, plots) 
+                self.write_svg(plot, position, export_dir) # type: ignore if export_svg, export_dir has been specified a few lines above
+            collapsible_sections += self.create_html_section(position, plot) 
         
         time = datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
         files_a, files_b = self.get_file_paths()
         
         css_string, plotly_js_string = hs.load_html_template_str()
 
         template = f"""
             <!DOCTYPE html>
             <html lang="en">
             <head>
                 <meta charset="UTF-8">
                 <meta http-equiv="X-UA-Compatible" content="IE=edge">
                 <meta name="viewport" content="width=device-width, initial-scale=1.0">
-                <title>Neet - Position extractor summary</title>
+                <title>Neet - POI View</title>
                 <link rel="stylesheet" type="text/css" href="/home/vincent/projects/neet_project/neet/summary/style.css">
                 <style>{css_string}</style>
             </head>
 
             <body>
                 <script>{plotly_js_string}</script>
                 <header>
-                    <h1>Position extractor summary</h1>
+                    <h1>Position of Interest View</h1>
                     <p>Produced by <a href="https://github.com/dietvin/neet">Neet</a> on <b>{time}</b></p>
                 </header>
             
                 <section>
                     <p class="intro-text">
                         This summary file contains an overview of {len(self.positions)} positions found in <i>{self.bed_path}</i>. 
                     </p>
                     <p class="intro-text">Files provided for sample <i>{self.basename_a}</i>:</p>
                     {files_a}
-                    <p class="intro-text">Files provided for sample <i>{self.basename_b}</i>:</p>
+                    {f'<p class="intro-text">Files provided for sample <i>{self.basename_b}</i>:</p>' if self.basename_b else ""}
                     {files_b}
                 </section>
 
                 {collapsible_sections}
 
                 <script>
                     var coll = document.getElementsByClassName("collapsible");
@@ -566,11 +525,21 @@
                     }});
                     }}
                 </script>
             </body>
             <footer></footer>
             </html> 
             """
-        outfile = os.path.join(self.out_dir, f"{self.basename_a}_{self.basename_b}_{self.basename_bed}_summary.html")
+        filename = f"{self.basename_a}_{self.basename_b}_{self.basename_bed}_view.html" if self.basename_b else f"{self.basename_a}_{self.basename_bed}_view.html"
+        outfile = os.path.join(self.out_dir, filename)
         with open(outfile, "w") as out:
             hs.print_update(f"Writing summary file to: {outfile}")
-            out.write(template)
+            out.write(template)
+
+        hs.print_update("Finished.")
+
+if __name__=="__main__":
+    p = POIView(paths_a="/home/vincent/projects/neet_project/data/45s_rrna/feature_tables/drna_cyt_extracted.tsv",
+                paths_b="/home/vincent/projects/neet_project/data/45s_rrna/feature_tables/drna_nuc_extracted.tsv",
+                bed_path="/home/vincent/projects/neet_project/data/45s_rrna/test/sample_b_excl.bed",
+                out_dir="/home/vincent/projects/neet_project/data/45s_rrna/test")
+    p.main()
```

### Comparing `neet-nanopore-0.0.4/neet/summary.py` & `neet_nanopore-1.0.0/neet/summary.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,65 +1,75 @@
+import os, datetime
+from collections import defaultdict
+from typing import List, Tuple, Dict, Any
+from statistics import mean
 import plotly.graph_objects as go
-import plotly.express as px
 from plotly.subplots import make_subplots
 from plotly.io import to_html
-from . import helper_functions as hs
-import os, warnings, sys, datetime, argparse
-from statistics import mean
-from collections import defaultdict
-from typing import List, Tuple, Dict
+import numpy as np
+from tqdm import tqdm
+
+try: # when invoked from the package
+    from neet import helper_functions as hs
+except ImportError: # when invoked directly
+    import helper_functions as hs
 
 class SummaryCreator:
     input_path: str
     output_path: str
     n_bins: int | None
     perc_mis_col: str
-    data: Dict[str, List[str|int|float]]
+    data: Dict[str, List[Any]] # can be of type str, int, float
     export_svg: bool
 
-    def __init__(self, in_path: str, out_path: str, n_bins: int|None, use_perc_mismatch_alt: bool, export_svg: bool) -> None:
+    def __init__(self, in_path: str, out_path: str | None = None, n_bins: int|None = 5000, use_perc_mismatch_alt: bool = False, export_svg: bool = False) -> None:
         self.process_paths(in_path, out_path)
         self.n_bins = n_bins if n_bins != -1 else None
         self.perc_mis_col = "mismatch_rate_alt" if use_perc_mismatch_alt else "mismatch_rate"
         self.export_svg = export_svg
         
     #################################################################################################################
     #                                   Functions called during initialization                                      #
     #################################################################################################################
 
-    def process_paths(self, in_path: str, out_path: str) -> None:
+    def process_paths(self, in_path: str, out_dir: str|None) -> None:
         """
-        Process the input and output paths for the SummaryCreator instance.
+        Process the input and output path for the SummaryCreator instance. If no output path is given, uses the
+        input path with the added suffix "_summary.html" as output path.
 
         Parameters:
         - in_path (str): The input file path.
-        - out_path (str): The output file path or directory.
+        - out_path (str|None): The output file path or directory.
 
         Raises:
         - FileNotFoundError: If the specified input file path does not exist or if the specified output directory does not exist.
         - Warning: If the output file has an extension other than '.html'. A warning is issued, but the function continues execution.
-
-        Returns:
-        - None
         """
         # process input path
         hs.check_input_path(in_path, [".tsv"])
-        self.input_path = in_path
-        # process output path(s)
-        self.output_path = hs.process_outpath(out_path, f"{os.path.splitext(os.path.basename(in_path))[0]}_summary.html", [".html"])
-      
-    def load_data(self):
+        self.input_path = os.path.abspath(in_path)
+
+        # process output path
+        if out_dir:
+            out_dir = os.path.abspath(out_dir)
+            ext = os.path.splitext(out_dir)[1]
+            if ext:
+                hs.print_update(f"Warning: Extension {ext} was found. Make sure to provide a single output directory.")
+            hs.check_create_dir(out_dir)
+            filename = f"{os.path.splitext(os.path.basename(in_path))[0]}_summary.html"
+            self.output_path = os.path.join(out_dir, filename)
+        else:
+            self.output_path = f"{os.path.splitext(in_path)[0]}_summary.html"
+
+    def load_data(self) -> None:
         """
         Load data from the specified input file into the SummaryCreator instance.
 
         Reads the data from a tab-separated values (tsv) file as created by the PileupExtractor module
         and stores it in the 'data' attribute of the class.
-
-        Returns:
-        - None
         """
         cols = ["chr", "n_reads", "ref_base", "majority_base", "deletion_rate", "insertion_rate", "refskip_rate", "mismatch_rate", "q_mean", "motif"]
 
         col_idx = {'chr': 0, 'site': 1, 'n_reads': 2, 'ref_base': 3, 'majority_base': 4, 'n_a': 5, 'n_c': 6, 'n_g': 7, 'n_t': 8, 'n_del': 9, 'n_ins': 10, 'n_ref_skip': 11, 'a_rate': 12, 'c_rate': 13, 'g_rate': 14, 'u_rate': 15, 'deletion_rate': 16, 'insertion_rate': 17, 'refskip_rate': 18, 'mismatch_rate': 19, 'mismatch_rate_alt': 20, 'motif': 21, 'q_mean': 22, 'q_std': 23, 'neighbour_error_pos': 24}
         dtypes = {'chr': str, 'site': int, 'n_reads': int, 'ref_base': str, 'majority_base': str, 'n_a': int, 'n_c': int, 'n_g': int, 'n_t': int, 'n_del': int, 'n_ins': int, 'n_ref_skip': int, 'a_rate': float, 'c_rate': float, 'g_rate': float, 'u_rate': float, 'deletion_rate': float, 'insertion_rate': float, 'refskip_rate': float, 'mismatch_rate': float, 'mismatch_rate_alt': float, 'motif': str, 'q_mean': float, 'q_std': float, 'neighbour_error_pos': str}
         
         with open(self.input_path, "r") as file:
@@ -85,51 +95,49 @@
         3. Writes an HTML summary file containing the generated plots.
 
         Note: The function includes print statements to provide updates on the progress of each step.
 
         Raises:
             Exception: If any error occurs during the execution, an exception is raised with an
                     accompanying error message.
-
-        Returns:
-            None
         """
+        time = hs.get_time()
+
         hs.print_update(f"Starting creation of summary from file '{self.input_path}'.")
-        hs.print_update("  - loading data... ", line_break=False)
-        self.load_data()
-        n_positions = len(self.data["chr"])
-        n_chromosomes = len(set(self.data["chr"]))
 
-        hs.print_update(f"Done. Found {n_positions} sites along {n_chromosomes} sequences.", with_time=False)
+        with tqdm(desc=f"{time} | Loading data", total=6) as progress:
+            self.load_data()
+            n_positions = len(self.data["chr"])
+            n_chromosomes = len(set(self.data["chr"]))
 
-        plots = []
-        
-        hs.print_update("  - creating general summary... ", line_break=False)
-        plots.append(self.create_general_plot())
-        hs.print_update(f"Done.", with_time=False)
-
-        hs.print_update("  - creating chromosome-wise summary... ", line_break=False)
-        plots.append(self.create_chr_plot())
-        hs.print_update(f"Done.", with_time=False)
-
-        hs.print_update("  - creating general mismatch summary... ", line_break=False)
-        plots.append(self.create_mism_general_plot())
-        hs.print_update(f"Done.", with_time=False)
-
-        hs.print_update("  - creating specific mismatch type summary... ", line_break=False)
-        plots += self.create_mism_types_plots()
-        hs.print_update(f"Done.", with_time=False)
-
-        hs.print_update("  - creating motif summary... ", line_break=False)
-        plots.append(self.create_motif_plot())
-        hs.print_update(f"Done.", with_time=False)
-
-        hs.print_update(f"  - creating HTML summary file at {self.output_path}")
-        self.write_to_html(n_positions, n_chromosomes, plots)
-        hs.print_update("Finished.")
+            plots = []
+    
+            progress.update()
+            progress.set_description(f"{time} | General summary")
+            plots.append(self.create_general_plot())
+
+            progress.update()
+            progress.set_description(f"{time} | General mismatch summary")
+            plots.append(self.create_mism_general_plot())
+
+            progress.update()
+            progress.set_description(f"{time} | Specific mismatch summary")
+            plots += self.create_mism_types_plots()
+
+            progress.update()
+            progress.set_description(f"{time} | Motif summary")
+            plots += self.create_motif_plot()
+
+            progress.update()
+            progress.set_description(f"{time} | Writing to HTML")
+            self.write_to_html(n_positions, n_chromosomes, plots)
+
+            progress.update()
+
+        hs.print_update(f"Finished. Wrote output to {self.output_path}")
     
 
     ################################################################################################################
     #                                                Helper methods                                                #
     ################################################################################################################
 
     def update_plot(self, fig, title: str|None = None, xlab: str|None = None, ylab: str|None = None, height: int = 500, width: int = 800):
@@ -157,15 +165,15 @@
                     height=height,  # Set the height to a constant value
                     width=width)
         fig.update_xaxes(showline=True, linewidth=2, linecolor='black', mirror=True, showticklabels=True, ticks='outside', showgrid=False, tickwidth=2)
         fig.update_yaxes(showline=True, linewidth=2, linecolor='black', mirror=True, showticklabels=True, ticks='outside', showgrid=False, tickwidth=2)
 
         return fig
 
-    def bin_data(self, data: List[int|str|float]) -> List[int|float]:
+    def bin_data(self, data: List[int|float]) -> List[int|float]:
         """
         Bin the input data into segments and return the mean value of each segment.
 
         Parameters:
         - data (List[int|str|float]): The input data to be binned.
 
         Raises:
@@ -173,77 +181,85 @@
 
         Returns:
         - List[int|float]: List of mean values for each bin.
         """
         total_length = len(data)
         num_segments = self.n_bins
 
-        if total_length == num_segments:
-            return data
-        elif total_length < num_segments:
-            return data
-        segment_length = segment_length = total_length // num_segments
-        remainder = total_length % num_segments
-        
-        start_index = 0
-        end_index = 0
-        segments = []
-        for i in range(num_segments):
-            end_index = start_index + segment_length + (1 if i < remainder else 0)
-            segments.append(data[start_index:end_index])
-            start_index = end_index
+        if num_segments: # added to stop pylance from complaining 
+            if total_length == num_segments:
+                return data
+            elif total_length < num_segments:
+                return data
+            segment_length = segment_length = total_length // num_segments
+            remainder = total_length % num_segments
+            
+            start_index = 0
+            end_index = 0
+            segments = []
+            for i in range(num_segments):
+                end_index = start_index + segment_length + (1 if i < remainder else 0)
+                segments.append(data[start_index:end_index])
+                start_index = end_index
 
-        return [mean(segment) for segment in segments]
+            return [mean(segment) for segment in segments]
+        return data
 
     ################################################################################################################
     #                                           Data preparation methods                                           #
     ################################################################################################################
 
-    def prepare_data_general(self) -> Tuple[List[int|float], List[float]]:
-        """
-        Prepare the data for plotting general information.
-
-        Returns:
-        - Tuple[List[int|float], List[float]]: Tuple containing binned or original 'n_reads' and 'q_mean' data.
+    def prepare_data_general(self) -> Dict[str, Dict[str, Tuple[np.ndarray, np.ndarray, int]]]:
         """
-        if self.n_bins is not None:
-            n_reads = self.bin_data(self.data["n_reads"])
-            quality = self.bin_data(self.data["q_mean"])
-            return n_reads, quality
-        else:
-            return self.data["n_reads"], self.data["q_mean"]
-
-    def prepare_data_chr(self) :
-        data_grouped = defaultdict(lambda: {"n_reads": [], "q_mean": []})
+        Prepare data for plotting general features. More specifically, group the number of reads 
+        and mean quality at each given position by their reference sequence. Calculate the median 
+        for each group. The grouped data is then condensed into a set number of bins and scaled 
+        between 0 and 1 for easier comparisons. Also calculates the number of positions for each
+        sequence. 
+        If more than one sequences are found in the data, calculate each statistic for all positions.
+        Dictionary is sorted by referenece sequences.
+
+        Returns:
+        - Dict[str, Dict[str, Tuple[np.ndarray, np.ndarray, int]]]: Dictionary containing the condensed data.
+        """
+
+        data_grouped = defaultdict(lambda: {"n_reads": [], "q_mean": [], "count": 0})
+
+        # group the data by sequence names
+        for sequence_name, n_reads, q_mean in zip(self.data["chr"],
+                                            self.data["n_reads"],
+                                            self.data["q_mean"]):
+            data_grouped[sequence_name]["n_reads"].append(n_reads) # type: ignore
+            data_grouped[sequence_name]["q_mean"].append(q_mean) # type: ignore
+            data_grouped[sequence_name]["count"] += 1 # type: ignore
+
+        # add the total entry only if multiple sequences are present 
+        # otherwise the same information is show for total and the single sequence
+        if len(data_grouped.keys()) > 1:
+            data_grouped["Total"]["n_reads"] = self.data["n_reads"]
+            data_grouped["Total"]["q_mean"] = self.data["q_mean"]
+            data_grouped["Total"]["count"] = len(self.data["q_mean"])
 
-        for chr_val, n_reads, q_mean in zip(self.data['chr'],
-                                            self.data['n_reads'],
-                                            self.data['q_mean']):
-            data_grouped[chr_val]['n_reads'].append(n_reads)
-            data_grouped[chr_val]['q_mean'].append(q_mean)
         data_grouped = dict(data_grouped)
 
-        n_sites_x = list(data_grouped.keys())
-        n_sites_y = [len(chr_data["n_reads"]) for chr_data in data_grouped.values()]
-
-        chroms = []
-        n_reads = []
-        q_mean = []
-
-        for chrom, chrom_data in data_grouped.items():
-            if (self.n_bins is not None) & (len(chrom_data["n_reads"]) > self.n_bins):
-                n_reads += self.bin_data(chrom_data["n_reads"])
-                q_mean += self.bin_data(chrom_data["q_mean"])
-                chroms += [chrom] * self.n_bins
-            else:
-                n_reads += chrom_data["n_reads"]
-                q_mean += chrom_data["q_mean"]
-                chroms += [chrom] * len(chrom_data["n_reads"])
-
-        return n_sites_x, n_sites_y, chroms, n_reads, q_mean
+        # condense the data into n_bins number of bins for more compact plot size later on
+        n_bins = 100
+        
+        for sequence_name in data_grouped.keys():
+            for c in ["n_reads", "q_mean"]:
+                median = np.median(data_grouped[sequence_name][c])
+                bin_value, bin_range = np.histogram(data_grouped[sequence_name][c], bins=n_bins, density=True)
+                # scale bin values between 0 and 1
+                # https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.MinMaxScaler.html
+                bin_value_scaled = (bin_value-bin_value.min()) / (bin_value.max()-bin_value.min()) 
+                # replace the raw count by the bins, the scaled frequencies and the median value
+                data_grouped[sequence_name][c] = (bin_range, bin_value_scaled, median) # type: ignore
+        
+        # data_grouped = dict(sorted(data_grouped.items()))
+        return data_grouped # type: ignore
 
     def prepare_data_mism_general(self) -> Dict[str, Tuple[int|List[float], int|List[float], int|List[float]]]:
         """
         Prepare mismatch data for plotting general mismatch information.
 
         Returns:
         - Dict[str, Tuple[int|List[float], int|List[float]]]: Dictionary containing binned or original mismatch data.
@@ -283,166 +299,73 @@
                 if len(data_mis[mismatch_type]) > self.n_bins:
                     data_mis[mismatch_type] = self.bin_data(data_mis[mismatch_type])
                 if len(data_del[mismatch_type]) > self.n_bins:
                     data_del[mismatch_type] = self.bin_data(data_del[mismatch_type])
             data_dict[mismatch_type] = (data_mat[mismatch_type], data_mis[mismatch_type], data_del[mismatch_type])
 
         return data_dict
-    
-    def prepare_data_mism_matrix(self, mis_count: Dict[str, int]) -> Tuple[List[List[int]], List[List[str]], int]:
-        """
-        Prepare data for a confusion matrix based on mismatch counts.
-
-        Parameters:
-        - mis_count (Dict[str, int]): Dictionary containing mismatch counts for each base pair combination.
 
-        Returns:
-        - Tuple[List[List[int]], List[List[str]], int]: Tuple containing matrix data, matrix labels, and the maximum value in the matrix.
-        """
-        # prepare data for the confusion matrix
-        matrix_data = [[None]*5 for _ in range(5)]
-        matrix_labels = [[None]*5 for _ in range(5)]
-        bases = ["A", "C", "G", "U", "-"]
-        # fill count matrix
-        for i in range(5): 
-            for j in range(5):
-                count = mis_count[f"{bases[i]} - {bases[j]}"] if i<4 else 0 # 0 in case of "- - X"
-                matrix_data[i][j] = count
-                if i != j:
-                    matrix_labels[i][j] = count
-        # fill the matrix containing corresponding labels
-        vals_flat = [element for sublist in matrix_labels for element in sublist if (element is not None)]
-        vals_sum = sum(vals_flat)
-        for i in range(5): 
-            for j in range(5):
-                if matrix_labels[i][j]:
-                    matrix_labels[i][j] = f"{round(matrix_labels[i][j] / vals_sum * 100, 2)}%"
-                else: 
-                    matrix_labels[i][j] = ""
-        # get the max value
-        val_max = max(vals_flat)
-
-        return matrix_data, matrix_labels, val_max
-
-    def prepare_data_mism_pie(self, mis_count: Dict[str, int]) -> Tuple[List[int], List[str]]:
-        """
-        Prepare data for a pie chart based on mismatch counts.
-
-        Parameters:
-        - mis_count (Dict[str, int]): Dictionary containing mismatch counts for each base pair combination.
-
-        Returns:
-        - Tuple[List[int], List[str]]: Tuple containing pie chart data and labels.
-        """
-        # prepare data for the pie chart
-        pie_data = list(mis_count.values())
-        pie_labels = list(mis_count.keys())
-        pie_data = []
-        pie_labels = []
-        # remove values for matches 
-        for label, data in mis_count.items():
-            if label not in ["A - A", "C - C", "G - G", "U - U"]:
-                pie_data.append(data)
-                pie_labels.append(label)
-        return pie_data, pie_labels
-    
-    def prepare_data_mism_box(self, mis_error_rates: Dict[str, List[str|float]]) -> Dict[str, List[str|float]]:
-        """
-        Prepare data for box plots based on mismatch error rates by mismatch types.
-
-        Parameters:
-        - mis_error_rates (Dict[str, List[str|float]]): Dictionary containing mismatch error rates.
-
-        Returns:
-        - Dict[str, List[str|float]]: Dictionary containing the prepared data for the box plot.
-        """
-        if self.n_bins is not None:
-            # group the data by mismatch type and if more samples than n_bins are present in a group, 
-            # subset the data to n_bins data points
-            error_rates_by_type = defaultdict(lambda: {"mismatch_rate": [], 
-                                                    "deletion_rate": [], 
-                                                    "insertion_rate": [], 
-                                                    "refskip_rate": []})
-            mismatch_types = ["A - C","A - G","A - U",
-                            "C - A","C - G","C - U",
-                            "G - A","G - C","G - U",
-                            "U - A","U - C","U - G",
-                            "A - -", "C - -", "G - -",
-                            "U - -"]
-            for mis_type in mismatch_types:
-                mask = [mis_type == m for m in mis_error_rates["mismatch_type"]]
-                for err_type in ["mismatch_rate", "deletion_rate", "insertion_rate", "refskip_rate"]:
-                    # use mask to filter data corresponding to err_type
-                    err_type_data = [mis_error_rates[err_type][i] for i in range(len(mask)) if mask[i]]
-
-                    if len(err_type_data) > self.n_bins:
-                        error_rates_by_type[mis_type][err_type] = self.bin_data(err_type_data)
-                    else:
-                        error_rates_by_type[mis_type][err_type] = err_type_data
-            error_rates_by_type = dict(error_rates_by_type)
-
-            # transform the data into the initial format
-            mis_error_rates = {"mismatch_type": [], "mismatch_rate": [], "deletion_rate": [], "insertion_rate": [], "refskip_rate": []}
-            for err_type, err_data in error_rates_by_type.items():
-                mis_error_rates["mismatch_type"] += [err_type] * len(err_data["mismatch_rate"])
-                mis_error_rates["mismatch_rate"] += err_data["mismatch_rate"]
-                mis_error_rates["deletion_rate"] += err_data["deletion_rate"]
-                mis_error_rates["insertion_rate"] += err_data["insertion_rate"]
-                mis_error_rates["refskip_rate"] += err_data["refskip_rate"]   
-            return mis_error_rates
-        return mis_error_rates
-
-    def prepare_data_mism_types(self) -> Tuple[List[List[int]], List[List[str]], int, List[int], List[str], Dict[str, List[str|float]]]:
+    def prepare_data_mism_types(self) -> Tuple[Dict[str, Dict[str, int]], Dict[str, Dict[str, List[str|float]]]]:
         """
         Prepare general data for mismatch type plots.
 
         Returns:
-        - Tuple[List[List[int]], List[List[str]], int, List[int], List[str], Dict[str, List[str|float]]]: 
-        Tuple containing data for confusion matrix, pie chart, and box plot for mismatch types analysis.
+        - Tuple[Dict[str, Dict[str, int]], Dict[str, List[str|float]]]: 
+        Tuple containing data the heatmap and box plots for mismatch types analysis.
         """
-        mis_types = [f"{f} - {t}" for f in ["A", "C", "G", "U"] for t in ["A", "C", "G", "U", "-"]]
-        mis_count = dict(zip(mis_types, [0]*len(mis_types)))
-
-        mis_error_rates = {"mismatch_type": [],"mismatch_rate": [], "deletion_rate": [], "insertion_rate": [], "refskip_rate": []}
+        mis_count = {"A": {"A": 0, "C": 0, "G": 0, "U": 0, "Del": 0}, 
+                    "C": {"A": 0, "C": 0, "G": 0, "U": 0, "Del": 0}, 
+                    "G": {"A": 0, "C": 0, "G": 0, "U": 0, "Del": 0}, 
+                    "U": {"A": 0, "C": 0, "G": 0, "U": 0, "Del": 0}}
+        mis_rates= {"A": {"mismatch_type": [], "mismatch_rate": [], "deletion_rate": [], "insertion_rate": [], "refskip_rate": []}, 
+                    "C": {"mismatch_type": [], "mismatch_rate": [], "deletion_rate": [], "insertion_rate": [], "refskip_rate": []}, 
+                    "G": {"mismatch_type": [], "mismatch_rate": [], "deletion_rate": [], "insertion_rate": [], "refskip_rate": []}, 
+                    "U": {"mismatch_type": [], "mismatch_rate": [], "deletion_rate": [], "insertion_rate": [], "refskip_rate": []}}
 
         for ref, maj, *error_rates in zip(self.data["ref_base"], 
                                           self.data["majority_base"], 
                                           self.data["mismatch_rate"], 
                                           self.data["deletion_rate"], 
                                           self.data["insertion_rate"], 
                                           self.data["refskip_rate"]):
             if (ref != "N") & (maj != "N"):
-                mis_count[f"{ref} - {maj}"] += 1
-                # prepare error rate data for distribution plots by each error type
+                if maj=="-": maj="Del"
+                mis_count[ref][maj] += 1
                 if ref != maj:
-                    mis_error_rates["mismatch_type"].append(f"{ref} - {maj}")
-                    mis_error_rates["mismatch_rate"].append(error_rates[0])
-                    mis_error_rates["deletion_rate"].append(error_rates[1])
-                    mis_error_rates["insertion_rate"].append(error_rates[2])
-                    mis_error_rates["refskip_rate"].append(error_rates[3])
+                    mis_rates[ref]["mismatch_type"].append(f"{ref}-{maj}")
+                    mis_rates[ref]["mismatch_rate"].append(error_rates[0])
+                    mis_rates[ref]["deletion_rate"].append(error_rates[1])
+                    mis_rates[ref]["insertion_rate"].append(error_rates[2])
+                    mis_rates[ref]["refskip_rate"].append(error_rates[3])
 
-        return *self.prepare_data_mism_matrix(mis_count), *self.prepare_data_mism_pie(mis_count), self.prepare_data_mism_box(mis_error_rates)
+        return mis_count, mis_rates
 
-    def prepare_data_motifs(self) -> Dict[str, Dict[str, List[str|float]]]:
+    def prepare_data_motifs(self) -> Tuple[Dict[str, Dict[str, List[str|float]]], Dict[str, int]]:
         """
         Prepare data for motif-wise error rate plotting.
 
         Returns:
-        - Dict[str, Dict[str, List[str|float]]]: Dictionary containing error rates for each motif.
+        - Tuple[Dict[str, Dict[str, List[str|float]]], Dict[str, int]]: Dictionary containing error rates for each motif 
+            and a dictionary containing the number of occurences for each motif
         """
         motif_error_rates = defaultdict(lambda: {"mismatch_rate": [], "deletion_rate": [], "insertion_rate": [], "refskip_rate": []})
 
         # extract the data for each 3 base-pair motif; store error rates in dict by motifs
         motif_center_idx = len(self.data["motif"][0]) // 2
         for motif, *error_rates in zip(self.data["motif"], self.data["mismatch_rate"], self.data["deletion_rate"], self.data["insertion_rate"], self.data["refskip_rate"]):
             motif_3bp = motif[motif_center_idx-1:motif_center_idx+2]
             for i, err_type in enumerate(["mismatch_rate", "deletion_rate", "insertion_rate", "refskip_rate"]):
                 motif_error_rates[motif_3bp][err_type].append(error_rates[i])
         motif_error_rates = dict(motif_error_rates)
 
+        # get the count for each motif before subsetting the data
+        motif_counts = {}
+        for motif in motif_error_rates.keys():
+            motif_counts[motif] = len(motif_error_rates[motif]["mismatch_rate"])
+
         # subsample data for each error rate for each motif
         if self.n_bins is not None:
             for motif in motif_error_rates.keys():
                 if len(motif_error_rates[motif]["mismatch_rate"]) > self.n_bins:
                     for err_type in ["mismatch_rate", "deletion_rate", "insertion_rate", "refskip_rate"]:
                         motif_error_rates[motif][err_type] = self.bin_data(motif_error_rates[motif][err_type])
 
@@ -455,15 +378,15 @@
             center_base = motif[1]
             if center_base == "N": continue # only subplots for center A, C, G, U
             num_sites = len(error_rates["mismatch_rate"])
             center_base_error_rates[center_base]["motif"] += [motif] * num_sites
             for i, err_type in enumerate(["mismatch_rate", "deletion_rate", "insertion_rate", "refskip_rate"]):
                 center_base_error_rates[center_base][err_type] += error_rates[err_type]
 
-        return dict(center_base_error_rates)
+        return dict(center_base_error_rates), motif_counts
     
     ##############################################################################################################
     #                                             Plotting functions                                             #
     ##############################################################################################################
 
     def create_error_placeholder(self, e: Exception):
         """
@@ -481,83 +404,114 @@
         fig.update_layout(
             dragmode=False,  # Disable panning
             hovermode='closest',  # Maintain hover behavior
             uirevision='true'  # Disable double-click autoscale
         )
         return fig
 
-
     def create_general_plot(self) -> go.Figure:
         """
-        Create a general plot displaying total coverage and total quality distributions.
+        Create a general plot displaying coverage and quality distributions for each chromosome in a ridge plot.
+        Figure contains three subplots: 1. Horizontal bar graph showing the number of positions for each reference
+        sequence. 2. Ridge plot showing the coverage distributions for each reference sequence. 3. Ridge plot 
+        showing the quality distributions for each reference sequence.
 
         Returns:
         - go.Figure: Plotly Figure for general plot.
         """
-        try:
-            n_reads_data, quality_data = self.prepare_data_general()
 
-            fig = make_subplots(rows=1, cols=2, 
-                                subplot_titles=["Total coverage distribution", "Total quality distribtion"], 
-                                horizontal_spacing=0.1)
-            fig = self.update_plot(fig, width=1400)
-            fig.update_annotations(font_size=25) # subplot title sizes
-
-            fig.add_traces([go.Box(y=n_reads_data, name="Total"), go.Box(y=quality_data, name="Total")], rows=[1,1], cols=[1,2])
-
-            fig.update_traces(line=dict(color="black"), 
-                            marker=dict(outliercolor="black"), 
-                            fillcolor="lightgrey")
-            fig.update_layout(showlegend=False)
-            fig.update_xaxes(showticklabels=False, ticks=None)
-            fig.update_yaxes(title_text="Coverage", row=1, col=1)
-            fig.update_yaxes(title_text="Mean quality", row=1, col=2)
+        def generate_colors(n: int) -> List[str]:
+            """
+            Generate a list of n colors in hex format, progressively lighter from #0f3957 to #beddf4.
+
+            Parameters:
+                - n (int): Number of colors to generate.
+
+            Returns:
+                List[str]: A list of n colors represented in hex format.
+            """
+            if n<=1: return ["#1f77b4"]
+            start_color = (15, 57, 87)  # RGB values for #0f3957
+            end_color = (190, 221, 244) # RGB values for #beddf4
+            # Calculate the step size for each color channel
+            step_r = (end_color[0] - start_color[0]) / (n - 1)
+            step_g = (end_color[1] - start_color[1]) / (n - 1)
+            step_b = (end_color[2] - start_color[2]) / (n - 1)
+            colors = []
+            for i in range(n):
+                # Calculate the RGB values for the current step
+                r = int(start_color[0] + step_r * i)
+                g = int(start_color[1] + step_g * i)
+                b = int(start_color[2] + step_b * i)
+                # Convert the RGB values to hex format and append to the list
+                colors.append('#{:02x}{:02x}{:02x}'.format(r, g, b))
+            return colors
 
-        except Exception as e:
-            fig = self.create_error_placeholder(e)
-
-        return fig
-    
-    def create_chr_plot(self) -> go.Figure:
-        """
-        Create a chromosome plot displaying the number of positions, number of reads, and mean quality.
-
-        Returns:
-        - go.Figure: Plotly Figure for chromosome plot.
-        """
         try:
-            def custom_sort_key(item):
-                if item.isdigit():  # Check if the item is a digit
-                    return (int(item),)  # Convert to integer and sort numerically
-                else:
-                    return (float('inf'), item)  # Place non-digits at the end
+            data_grouped = self.prepare_data_general()
 
-            n_pos_x, n_pos_y, chrom, n_reads, quality = self.prepare_data_chr()
+            offset = 0.8
 
-            fig = make_subplots(rows=3, cols=1, 
-                                specs=[[{"type": "bar"}], [{"type": "box"}], [{"type": "box"}]], 
-                                shared_xaxes=True, vertical_spacing=0.02)
-            fig = self.update_plot(fig, height=1000, width=1400)
+            # Approach to figure is inspired by
+            # https://python-graph-gallery.com/ridgeline-graph-plotly/
+            fig = make_subplots(cols=3, shared_yaxes=True, horizontal_spacing = 0.01)
+
+            n_sequences = len(data_grouped.keys())
+            y_ticks = []
+            show_legend = True
+            y_offsets = [i*offset for i in range(n_sequences)][::-1]
+            colors = generate_colors(n_sequences)
+
+            fig = self.update_plot(fig, height=min(n_sequences*400, 1000), width=1200)
+
+            # iterate through all keys from the data grouped by sequence 
+            for y_offset, sequence_name, color in zip(y_offsets, data_grouped.keys(), colors):
+                y = y_offset+offset/2
+                y_ticks.append(y)
+                x = data_grouped[sequence_name]["count"]
+                # add number of positions per plot
+                bar = go.Bar(x=[x], y=[y], orientation="h", name=sequence_name, showlegend=False, width=0.5, marker=dict(color=color, line_color="black", line_width=2))
+                fig.add_trace(bar, row=1, col=1)
+
+                # add number of reads and q_mean distribution subplots
+                for col, c in zip([2,3], ["n_reads", "q_mean"]):
+                    x = data_grouped[sequence_name][c][0]
+                    y = data_grouped[sequence_name][c][1] + y_offset
+                    hover_labels = data_grouped[sequence_name][c][1]
+                    median = data_grouped[sequence_name][c][2]
+                    
+                    # line to cut off the fill color at the base (y_offset) of each distribution
+                    line = go.Scatter(x=(x.min(), x.max()), y=(y_offset, y_offset), mode="lines", line_color="white", showlegend=False)
+                    # line indicating the median value
+                    median_line = go.Scatter(x=[median, median], y=[y_offset, y_offset+1], name=f"Median", mode="lines", line = dict(color="black", width=2, dash='dot'),
+                                            legendgroup=1, showlegend=show_legend,
+                                            hovertemplate="Median: %{x}")
+                    if show_legend: show_legend = False
+
+                    # distribution itself
+                    hist = go.Scatter(x=x, y=y, fill='tonexty', name=sequence_name, customdata=hover_labels, showlegend=False, line_shape='spline', line_color="black", 
+                                    fillcolor=color, hovertemplate="<br>".join(["Coverage: %{x:.1f}", "Density: %{customdata:.5f}"]))
+
+                    fig.add_traces([line, hist, median_line], rows=[1,1,1], cols=[col, col, col])
+
+            # update axes of subplots 
+            fig.update_yaxes(showexponent = 'all',
+                            exponentformat = 'e',
+                            tickmode = "array",
+                            tickvals = y_ticks,
+                            ticktext = list(data_grouped.keys()), row=1, col=1)
+            fig.update_xaxes(title=dict(text="Number of covered positions",  font=dict(size=20)), row=1, col=1)
 
-            fig.add_trace(go.Bar(x=n_pos_x, y=n_pos_y))
-            fig.add_trace(go.Box(x=chrom, y=n_reads), row=2, col=1)
-            fig.add_trace(go.Box(x=chrom, y=quality), row=3, col=1)
+            fig.update_yaxes(tickmode = "array", tickvals = [], row=1, col=2)
+            fig.update_xaxes(title=dict(text="Number of reads",  font=dict(size=20)), row=1, col=2)
 
-            fig.update_traces(marker=dict(color='lightgrey', line=dict(color='black', width=2)), selector=dict(type='bar'))
-            fig.update_traces(marker=dict(color="black", outliercolor="black", size=2), fillcolor="lightgrey", selector=dict(type='box'))
-            
-            fig.update_xaxes(categoryorder='array', categoryarray=sorted(n_pos_x, key=custom_sort_key))
-            for i in range(1, 3):
-                fig.update_xaxes(tickvals=[], ticktext=[], row=i, col=1)
-
-            fig.update_xaxes(title_text="Chromosome", row=3, col=1)
-            fig.update_yaxes(title_text="Number of positions", row=1, col=1)
-            fig.update_yaxes(title_text="Number of reads", row=2, col=1)
-            fig.update_yaxes(title_text="Mean quality", row=3, col=1)
-            fig.update_layout(showlegend=False)
+            fig.update_yaxes(tickmode = "array", tickvals = [], row=1, col=3)
+            fig.update_xaxes(title=dict(text="Mean quality",  font=dict(size=20)), row=1, col=3)
+
+            fig.update_layout(legend=dict(orientation="h", yanchor="bottom", y=1.05, xanchor="right", x=1, bgcolor='#f5f5f5', bordercolor='#000000', borderwidth=2))
 
         except Exception as e:
             fig = self.create_error_placeholder(e)
 
         return fig
 
     def create_mism_general_plot(self) -> go.Figure:
@@ -589,15 +543,15 @@
             data_processed = self.prepare_data_mism_general()
 
             fig = make_subplots(rows=1, cols=5, 
                                 specs=[[{"type": "box"}, {"type": "box"}, {"type": "box"}, {"type": "box"}, {"type": "pie"}]], 
                                 shared_yaxes=True,
                                 horizontal_spacing=0.01,
                                 column_titles=("Mismatch frequency", "Deletion frequency", "Insertion frequency", "Reference skip frequ.", None))
-            fig = self.update_plot(fig, height=600, width=1400)
+            fig = self.update_plot(fig, height=600, width=1200)
 
             for i, (dname, legend) in enumerate(zip(["mismatch_rate", "deletion_rate", "insertion_rate", "refskip_rate"], [True, False, False, False]), start=1):
                 box_mat = boxplot(data_processed[dname][0], group="match", showlegend=legend)
                 box_mis = boxplot(data_processed[dname][1], group="mismatch", showlegend=legend)
                 box_del = boxplot(data_processed[dname][2], group="deletion", showlegend=legend)
                 fig.add_traces([box_mat, box_mis, box_del], rows=1, cols=i)
 
@@ -607,15 +561,15 @@
                         textinfo="value", 
                         textfont_size=20, 
                         marker=dict(colors=["#4c72b0", "#dd8452", "#2ca02c"], line=dict(color="#000000", width=2)), 
                         showlegend=False,
                         sort=False)
             fig.add_trace(pie, row=1, col=5)
 
-            fig.update_layout(legend=dict(orientation="h", yanchor="bottom", y=1.05, xanchor="right", x=1, bgcolor='#f5f5f5', bordercolor='#000000', borderwidth=2))
+            fig.update_layout(legend=dict(orientation="h", yanchor="bottom", y=1.1, xanchor="right", x=1, bgcolor='#f5f5f5', bordercolor='#000000', borderwidth=2))
             fig.update_annotations(font_size=21)
             fig.update_yaxes(showticklabels=False, ticks=None, row=1, col=2)
             fig.update_yaxes(showticklabels=False, ticks=None, row=1, col=3)
             fig.update_yaxes(showticklabels=False, ticks=None, row=1, col=4)
 
         except Exception as e:
             fig = self.create_error_placeholder(e)
@@ -626,109 +580,183 @@
         """
         Create mismatch type plots including a confusion matrix, a pie chart, and a box plot.
 
         Returns:
         - List[go.Figure]: List of Plotly Figures for mismatch type plots.
         """
         try:
-            matrix_data, matrix_labels, matrix_max_mism, pie_data, pie_labels, box_data = self.prepare_data_mism_types()
+            mis_count, mis_rates = self.prepare_data_mism_types()
         except Exception as e:
             fig = self.create_error_placeholder(e)
             fig = fig
             return [fig, fig, fig]
 
         try:
-            fig = px.imshow(matrix_data, labels=dict(x="Called base", y="Reference base", color="Count"), zmin=0, zmax=1.2*matrix_max_mism, color_continuous_scale="portland")
-            fig = self.update_plot(fig, None, "Called base", "Reference base", width=800)
-            fig.update_traces(text=matrix_labels, texttemplate="%{text}")
-            fig.update_xaxes(fixedrange=True, tickvals=[0,1,2,3,4], ticktext=["A", "C", "G", "U", "-"])
-            fig.update_yaxes(fixedrange=True, tickvals=[0,1,2,3,4], ticktext=["A", "C", "G", "U", "-"])
+            fig = go.Figure()
+            fig = self.update_plot(fig, ylab="Reference base", xlab="Called base")
+
+            counts = [[mis_count[row][col] for col in ["A", "C", "G", "U", "Del"]] for row in ["A", "C", "G", "U"]]
+            # excluding the colorscaling for the match counts (usually many more than mismatches --> better color scaling)
+            max_count = max([mis_count[row][col] for row in ["A", "C", "G", "U"] for col in ["A", "C", "G", "U", "Del"] if row!=col])
+            heatmap = go.Heatmap(x=["A", "C", "G", "U", "Del"],
+                                y=["A", "C", "G", "U"],
+                                z=counts,
+                                colorscale="portland",
+                                hoverinfo="z",
+                                hovertemplate="%{y}-%{x}<br>Count: %{z}",
+                                zmin=0,
+                                zmax=max_count,
+                                name="",
+                                colorbar=dict(title="Count"))
+            heatmap.update(dict(showscale=True))
+            fig.add_trace(heatmap)
+
+            # Add text annotations
+            total_count = sum([sum(mis_count[row].values()) for row in mis_count.keys()])
+            annotations = []
+            for i, row in enumerate(["A", "C", "G", "U"]):
+                for j, col in enumerate(["A", "C", "G", "U", "Del"]):
+                    # add black border around each cell
+                    fig.add_shape(type="rect",
+                            x0=j - 0.5, y0=i - 0.5,
+                            x1=j + 0.5, y1=i + 0.5,
+                            line=dict(color="#000000", width=1),
+                            fillcolor="rgba(0,0,0,0)",
+                            xref="x", yref="y")
+                    # add percent values as annotations to each cell
+                    annotations.append(
+                        dict(
+                            x=j, y=i,
+                            text=f"{(mis_count[row][col] / total_count)*100:.2f}%",
+                            showarrow=False,
+                            font=dict(color="#000000"),
+                            xref="x",
+                            yref="y"
+                        )
+                    )
+
+            fig.update_layout(annotations=annotations)
             matrix = fig
+
         except Exception as e:
             fig = self.create_error_placeholder(e)
             matrix = fig
 
         try:
-            fig = go.Figure(go.Pie(labels=pie_labels, values=pie_data, 
-                        hoverinfo='label+percent', textinfo='value', textfont_size=20, 
-                        marker=dict(line=dict(color='#000000', width=2))))
-            fig = self.update_plot(fig, width=800)
-            fig.update_layout(legend=dict(bgcolor='#f5f5f5', bordercolor='#000000', borderwidth=2))
-            pie = fig
-        except Exception as e:
-            fig = self.create_error_placeholder(e)
-            pie = fig
+            fig = make_subplots(rows=2, cols=2, shared_yaxes=True, vertical_spacing=0.1, horizontal_spacing=0.05)
+            fig = self.update_plot(fig, width=1200, height=1000)
 
-        try:
-            fig = go.Figure()
-            fig = self.update_plot(fig, ylab="Error rate", height=600, width=1400)
+            show_legend = True
+            for i, (row, col) in zip(["A", "C", "G", "U"], [(1,1), (1,2), (2,1), (2,2)]):
+                x = mis_rates[i]["mismatch_type"]
+                for group, (feature_name, feature_label, color) in enumerate([("mismatch_rate", "Mismatch rate", "#55a868"),
+                                                                            ("deletion_rate", "Deletion rate", "#c44e52"), 
+                                                                            ("insertion_rate", "Insertion rate", "#8172b3"), 
+                                                                            ("refskip_rate", "Reference skip rate", "#937860")]):
+                    # https://community.plotly.com/t/grouped-boxplots-in-subplots-have-gaps-in-the-x-axis/46736/6
+                    box = go.Box(x=x, y=mis_rates[i][feature_name], name=feature_label, showlegend=show_legend, legendgroup=group, offsetgroup=group, 
+                                line=dict(color="black"), marker=dict(outliercolor="black", size=2), fillcolor=color)
+                    fig.add_trace(box, row=row, col=col)
+
+                if show_legend: show_legend=False
+
+            fig.update_layout(boxmode="group",
+                            boxgap=0.1,
+                            boxgroupgap=0,
+                            legend=dict(orientation="h", yanchor="bottom", y=1.05, xanchor="right", x=1.0, bgcolor='#f5f5f5', bordercolor='#000000', borderwidth=2))
+
+            fig.update_xaxes(categoryorder='array', categoryarray=["A-C", "A-G", "A-U", "A-Del"], row=1, col=1)
+            fig.update_xaxes(categoryorder='array', categoryarray=["C-A", "C-G", "C-U", "C-Del"], row=1, col=2)
+            fig.update_xaxes(title="Mismatch type", categoryorder='array', categoryarray=["G-A", "G-C", "G-U", "G-Del"], row=2, col=1)
+            fig.update_xaxes(title="Mismatch type", categoryorder='array', categoryarray=["U-A", "U-C", "U-G", "U-Del"], row=2, col=2)
 
-            x = box_data["mismatch_type"]
-            for err_type, c in zip(["mismatch_rate", "deletion_rate", "insertion_rate", "refskip_rate"], ["#55a868", "#c44e52", "#8172b3", "#937860"]):
-                y = box_data[err_type]
-                fig.add_trace(go.Box(x=x, y=y, name=err_type, 
-                                    line=dict(color="black"), 
-                                    marker=dict(outliercolor="black", size=2), 
-                                    fillcolor=c))
+            fig.update_yaxes(title="Error rate", row=1, col=1)
+            fig.update_yaxes(title="Error rate", row=2, col=1)
 
-            fig.update_layout(boxmode="group", legend=dict(orientation="h", yanchor="bottom", y=1.05, xanchor="right", x=1.0, bgcolor='#f5f5f5', bordercolor='#000000', borderwidth=2))
-            fig.update_xaxes(categoryorder='array', categoryarray=pie_labels)
             box = fig
+
         except Exception as e:
             fig = self.create_error_placeholder(e)
             box = fig
 
-        return [matrix, pie, box]
-
-    def create_motif_plot(self) -> go.Figure:
+        return [matrix, box]
+    
+    def create_motif_plot(self) -> Tuple[go.Figure, go.Figure]:
         """
-        Create a plot showing error rates for different motifs.
+        Create a plot showing error rates for different motifs and a plot showing the corresponding 
+        counts for each motif. The plots are grouped into four subplots for each center base.
 
         Returns:
-        - go.Figure: Plotly Figure for the motif plot.
+        - Tuple[go.Figure, go.Figure]: Plotly Figure for the error rates by motif and the motif counts.
         """
-        try:
-            x_order = {"A": ["CAC", "CAG", "CAU", "GAC", "GAG", "GAU", "UAC", "UAG", "UAU"], 
-                    "C": ["ACA", "ACG", "ACU", "GCA", "GCG", "GCU", "UCA", "UCG", "UCU"],
-                    "G": ["AGA", "AGC", "AGU", "CGA", "CGC", "CGU", "UGA", "UGC", "UGU"],
-                    "U": ["AUA", "AUC", "AUG", "CUA", "CUC", "CUG", "GUA", "GUC", "GUG"]}
-            
-            fig = make_subplots(rows=2, cols=2, 
-                                specs=[[{"type": "box"}, {"type": "box"}], [{"type": "box"}, {"type": "box"}]], 
-                                shared_yaxes=True, 
-                                vertical_spacing=0.1, horizontal_spacing=0.05)
-            fig = self.update_plot(fig, height=900, width=1400)
-
-            motif_data = self.prepare_data_motifs()
+        try: 
+            motif_data, motif_counts = self.prepare_data_motifs()
+        except Exception as e:
+            return self.create_error_placeholder(e), self.create_error_placeholder(e)
+        
+        x_order = {"A": ["AAA", "AAC", "AAG", "AAU", "CAA", "CAC", "CAG", "CAU", "GAA", "GAC", "GAG", "GAU", "UAA", "UAC", "UAG", "UAU"], 
+                   "C": ["ACA", "ACC", "ACG", "ACU", "CCA", "CCC", "CCG", "CCU", "GCA", "GCC", "GCG", "GCU", "UCA", "UCC", "UCG", "UCU"],
+                   "G": ["AGA", "AGC", "AGG", "AGU", "CGA", "CGC", "CGG", "CGU", "GGA", "GGC", "GGG", "GGU", "UGA", "UGC", "UGG", "UGU"],
+                   "U": ["AUA", "AUC", "AUG", "AUU", "CUA", "CUC", "CUG", "CUU", "GUA", "GUC", "GUG", "GUU", "UUA", "UUC", "UUG", "UUU"]}
+        
+        # create subplots showing the error rates for different 3bp motifs
+        try:   
+            rates_fig = make_subplots(rows=2, cols=2, 
+                                    specs=[[{"type": "box"}, {"type": "box"}], [{"type": "box"}, {"type": "box"}]], 
+                                    shared_yaxes=True, 
+                                    vertical_spacing=0.1, horizontal_spacing=0.05)
+            rates_fig = self.update_plot(rates_fig, height=900, width=1200)
 
             for center_base, row, col in zip(["A", "C", "G", "U"], [1,1,2,2], [1,2,1,2]):
                 d = motif_data[center_base]
                 traces = []
                 for i, (err_type, name, color) in enumerate(zip(["mismatch_rate", "deletion_rate", "insertion_rate", "refskip_rate"], ["Mismatch", "Deletion", "Insertion", "Reference skip"], ["#55a868", "#c44e52", "#8172b3", "#937860"])):
                     trace = go.Box(x=d["motif"], y=d[err_type], name=name, 
                                 line=dict(color="black", width=1), 
                                 marker=dict(outliercolor="black", size=1), 
                                 fillcolor=color,
                                 legendgroup=i,
                                 showlegend=True if center_base == "A" else False,
                                 offsetgroup=i)
                     traces.append(trace)
 
-                fig.add_traces(traces, rows=row, cols=col)
-                fig.update_xaxes(categoryorder='array', categoryarray=x_order[center_base], row=row, col=col)
+                rates_fig.add_traces(traces, rows=row, cols=col)
+                rates_fig.update_xaxes(categoryorder='array', categoryarray=x_order[center_base], row=row, col=col)
+
+            rates_fig.update_layout(boxmode="group", boxgroupgap=0, legend=dict(orientation="h", yanchor="bottom", y=1.02, xanchor="right", x=1, bgcolor='#f5f5f5', bordercolor='#000000', borderwidth=2))
+            rates_fig.update_xaxes(title = "3bp Motif", row=2, col=1)
+            rates_fig.update_xaxes(title = "3bp Motif", row=2, col=2)
+            rates_fig.update_yaxes(title = "Error rate", row=1, col=1)
+            rates_fig.update_yaxes(title = "Error rate", row=2, col=1)
+        except Exception as e:
+            rates_fig = self.create_error_placeholder(e)
 
-            fig.update_layout(boxmode="group", boxgroupgap=0, legend=dict(orientation="h", yanchor="bottom", y=1.02, xanchor="right", x=1, bgcolor='#f5f5f5', bordercolor='#000000', borderwidth=2))
-            fig.update_xaxes(title = "3bp Motif", row=2, col=1)
-            fig.update_xaxes(title = "3bp Motif", row=2, col=2)
-            fig.update_yaxes(title = "Error rate", row=1, col=1)
-            fig.update_yaxes(title = "Error rate", row=2, col=1)
+        # create subplots showing counts of the different 3bp motifs
+        try: 
+            counts_fig = make_subplots(rows=2, cols=2, 
+                                    specs=[[{"type": "bar"}, {"type": "bar"}], [{"type": "bar"}, {"type": "bar"}]], 
+                                    shared_yaxes=True, 
+                                    vertical_spacing=0.15, horizontal_spacing=0.05)
+            counts_fig = self.update_plot(counts_fig, height=600, width=1200)
 
+            for center_base, row, col in zip(["A", "C", "G", "U"], [1,1,2,2], [1,2,1,2]):
+                x = x_order[center_base]
+                y = [motif_counts[motif] if motif in motif_counts.keys() else 0 for motif in x]
+                bar = go.Bar(x=x, y=y, name=f"Center {center_base}", showlegend=False,
+                            marker=dict(color="#A0A0A0", line_color="#000000", line_width=2))
+                counts_fig.add_trace(bar, row=row, col=col)
+
+            counts_fig.update_xaxes(title = "3bp Motif", row=2, col=1)
+            counts_fig.update_xaxes(title = "3bp Motif", row=2, col=2)
+            counts_fig.update_yaxes(title = "Count", row=1, col=1)
+            counts_fig.update_yaxes(title = "Count", row=2, col=1)
         except Exception as e:
-            fig = self.create_error_placeholder(e)            
-        return fig
+            counts_fig = self.create_error_placeholder(e)
+        
+        return rates_fig, counts_fig
 
     ################################################################################################################
     #                                               Create HTML file                                               #
     ################################################################################################################
     def write_svg(self, fig: go.Figure, name: str) -> None:
         """
         Write the Plotly Figure to an SVG file.
@@ -749,15 +777,15 @@
 
         Args:
         - plot_figs (List[go.Figure]): List of Plotly Figures.
 
         Returns:
         - List[str]: List of HTML strings representing the Plotly Figures.
         """
-        plot_str = list(map(lambda x: to_html(x, include_plotlyjs=False), plot_figs))
+        plot_str = list(map(lambda x: to_html(x, include_plotlyjs=False, full_html=False), plot_figs))
         return plot_str
 
     def write_to_html(self, n_positions, n_chr, plot_figs: List[go.Figure]) -> None:
         """
         Generate an HTML summary page with collapsible sections for different types of analysis.
         
         Parameters:
@@ -806,103 +834,96 @@
                         </header>
                     
                         <section>
                             <p class="intro-text">
                                 This summary file was created from the extracted features in file <b>{self.input_path}</b>. 
                                 {f"Data was averaged into <b>{self.n_bins}</b> bins to allow for better performance." if self.n_bins else ""}
                                 In total <b>{n_positions}</b> positions were extracted along <b>{n_chr}</b> {"sequences" if n_chr > 1 else "sequence"}. 
-                                The plots are interactive and allow further information by hovering, zooming and panning.
+                                The plots are interactive and provide further information by hovering, zooming and panning.
                             </p>
                         </section>
 
                         <section>
                             <button class="collapsible">General statistics</button>
                             <div class="collapsible-content">
                                 <h2 class="hiddentitle" id="general_statistics"></h2>
 
-                                <h3>Over all extracted position</h3>
+                                <h3>Number of covered sites, coverage- and quality distribtions of all sequences</h3>
                                 <div class="plot-container">
                                     {plots[0]}
                                 </div>
                                 <p>
-                                    Distribution of the coverage (<b>left</b>) and mean quality (<b>right</b>) of those positions.  
-                                    The mean quality at a given position x is calculated from the quality scores from all mapped reads
-                                    at this position. {data_point_descr}.
-                                </p>
-
-                                <h3>Split by each chromosome</h3>        
-                                <div class="plot-container">
-                                    {plots[1]}
-                                </div>
-                                <p>
-                                    <b>Top</b>: Number of positions that were extracted on each chromosome. <b>Middle</b>: Distribution of the number of reads on a chromosome. 
-                                    Each data point corresponds to one position. <b>Bottom</b>: Distribution of the quality scores averaged over all reads mapped
-                                    at a given position. {data_point_descr}.
+                                    For each reference sequence: Number of covered positions (<b>left</b>) and distributions of coverage (<b>middle</b>) 
+                                    and mean quality (<b>right</b>) at these positions. The distributions show the probability density scaled to values
+                                    between 0 and 1 for each sequence separately for easy comparison. The mean quality at a given position x is 
+                                    calculated from the quality scores from all mapped reads at this position.
                                 </p>
-                            </div>
                         </section>
 
                         <section>
                             <button class="collapsible">Mismatch statistics</button>
                             <div class="collapsible-content">
                                 <h2 class="hiddentitle" id="mismatch_statistics"></h2>
 
                                 <h3>Mismatch, deletetion and insertion rates for matched and mismatched positions</h3>
                                 <div class="plot-container">
-                                    {plots[2]}
+                                    {plots[1]}
                                 </div>
                                 <p>
                                     Overview of the number of mismatches and what types of errors contribute to them. Match refers to the positions where the correct base was called. 
                                     Mismatch refers to the positions where the wrong base was called. The pie chart on the right shows the number of matched and mismatched positions
                                     along all chromosomes. The boxplots on the left show the distributions of the mismatch (<b>leftmost</b>), deletion (<b>second from left</b>), insertion (<b>second from right</b>)
                                     and reference skip (<b>right</b>) rates at matched and mismatched positions. {data_point_descr}.
                                 </p>
 
                                 <h3>Abundances of different type of mismatches</h3>
 
-                                <h4>As confusion matrix</h4>
+                                <h4>Mismatch/Deletion counts</h4>
                                 <div class="plot-container">
-                                    {plots[3]}
+                                    {plots[2]}
                                 </div>
                                 <p>
                                     Abundance of matches by base (diagonal) and all types of mismatches <i>from Reference base to Called base</i>. Warmer colors indicate higher counts.
                                 </p>
                             
-                                <h4>As pie chart</h4>
-                                <div class="plot-container">
-                                    {plots[4]}
-                                </div>
-                                <p>
-                                    Relative abundances of mismatch types (<i>[FROM] - [TO]</i>). Section labels show absolute count. Relative count is shown on hovering.
-                                </p>
-
                                 <h3>Mismatch, deletion and insertion rates by type of mismatch</h3>
                                 <div class="plot-container">
-                                    {plots[5]}
+                                    {plots[3]}
                                 </div>
                                 <p>
-                                    Distribtions of Mismatch, Deletion, Insertion and Refernce skip rates for each observed mismatch type (<i>[FROM] - [TO]</i>). 
+                                    Distribtions of Mismatch, Deletion, Insertion and Refernce skip rates for each observed mismatch type (<i>[FROM] - [TO]</i>).
+                                    Plots are split by central A (<b>top left</b>), C (<b>top right</b>), G (<b>bottom left</b>) and U (<b>bottom right</b>)
                                     Each data point corresponds to one position.
                                 </p>
                             </div>
                         </section>
 
                         <section>
                             <button class="collapsible">Error rate by motifs</button>
                             <div class="collapsible-content">
                                 <h2 class="hiddentitle" id="error_motif"></h2>
 
                                 <h3>Mismatch, insertion, deletion and reference skip rates for 3bp motifs</h3>
                                 <div class="plot-container">
-                                    {plots[6]}
+                                    {plots[4]}
                                 </div>
                                 <p>
                                     Distributions of Mismatch, deletion and insertion rates for different three base motifs with center A (<b>top left</b>), C (<b>top right</b>),
                                     G (<b>bottom left</b>) and U (<b>bottom right</b>). {data_point_descr}.
                                 </p>
+
+                                <h3>Number of positions for each 3bp motif</h3>
+                                <div class="plot-container">
+                                    {plots[5]}
+                                </div>
+                                <p>
+                                    Number of positions for each three base motifs with center A (<b>top left</b>), C (<b>top right</b>),
+                                    G (<b>bottom left</b>) and U (<b>bottom right</b>).
+                                </p>
+
                             </div>
                         </section>
 
                         <script>
                             var coll = document.getElementsByClassName("collapsible");
                             var i;
 
@@ -919,8 +940,13 @@
                             }}
                         </script>
                     </body>
                     <footer></footer>
                     </html> 
                     """
         with open(self.output_path, "w") as o:
-            o.write(template)
+            o.write(template)
+
+
+if __name__=="__main__":
+    s = SummaryCreator(in_path="/home/vincent/projects/neet_project/data/45s_rrna/test/drna_cyt_extracted.tsv", export_svg=True)
+    s.main()
```

### Comparing `neet-nanopore-0.0.4/neet/summary_style/plotly.js` & `neet_nanopore-1.0.0/neet/summary_style/plotly.js`

 * *Files identical despite different names*

### Comparing `neet-nanopore-0.0.4/neet/summary_style/style.css` & `neet_nanopore-1.0.0/neet/summary_style/style.css`

 * *Files identical despite different names*

### Comparing `neet-nanopore-0.0.4/neet/two_sample_extractor.py` & `neet_nanopore-1.0.0/neet/two_sample_extractor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,74 +1,103 @@
 from typing import List, Dict, Any, Tuple, Set
-import os, warnings, sys, datetime, argparse
-from collections import Counter
-from . import helper_functions as hs
+import os, sys, datetime, math
+from collections import Counter, defaultdict
 import plotly.graph_objects as go
 from plotly.io import to_html
 
+try: # when invoked from the package
+    from neet import helper_functions as hs
+except ImportError: # when invoked directly
+    import helper_functions as hs
+
+SITE = Tuple[str, int]
+
 class PositionExtractor:
     out_dir: str
     export_svg: bool
 
     in_paths_a: List[str]
     in_paths_b: List[str]
 
     label_a: str
     label_b: str
 
     error_feature_idx: int
     error_threshold: float
     coverage_threshold: int
 
-    ref_dict: Dict[str, str]
+    ref_path: str
+    n_bins_seqmap: int
 
-    def __init__(self, in_paths_a: str, in_paths_b: str, out_dir: str, ref_path: str, error_feature: str, error_threshold: float, coverage_threshold: int, 
-                 label_a: str, label_b: str, export_svg: bool = False) -> None:
+    a_and_b: List[SITE]
+    a_excl: List[SITE]
+    b_excl: List[SITE]
+
+    def __init__(self, 
+                 in_paths_a: str, 
+                 in_paths_b: str, 
+                 ref_path: str, 
+                 out_dir: str | None = None, 
+                 error_feature: str = "mismatch_alt", 
+                 error_threshold: float = 0.5, 
+                 coverage_threshold: int = 40, 
+                 label_a: str = "sample_a", 
+                 label_b: str = "sample_b", 
+                 export_svg: bool = False, 
+                 n_bins_seqmap: int = 200) -> None:
         """
         Initialize the PositionExtractor object with input parameters.
 
         Parameters:
         - in_paths_a (str): Comma-separated string of file paths for dataset A.
         - in_paths_b (str): Comma-separated string of file paths for dataset B.
         - out_dir (str): Output directory for the extracted data.
         - ref_path (str): File path to the reference data in FASTA format.
-        - error_feature (str): The type of error feature to be analyzed.
-        - error_threshold (float): Threshold for the specified error feature.
-        - coverage_threshold (int): Threshold for the coverage of positions to be considered.
-        - label_a (str): Label for dataset A.
-        - label_b (str): Label for dataset B.
-        - export_svg (bool, optional): Flag indicating whether to export SVG plots (default is False).
+        - error_feature (str): The type of error feature to be analyzed. One of: mismatch, mismatch_alt, deletion, insertion. (Default: "mismatch")
+        - error_threshold (float): Threshold for the specified error feature. (Default: 0.5)
+        - coverage_threshold (int): Threshold for the coverage of positions to be considered. (Default: 10)
+        - label_a (str): Label for dataset A. (Default: "sample_a")
+        - label_b (str): Label for dataset B. (Default: "sample_b")
+        - export_svg (bool, optional): Flag indicating whether to export SVG plots (Default: False).
 
         Raises:
         - Exception: If an invalid error feature is provided.
         """
         self.in_paths_a = self.process_in(in_paths_a)
         self.in_paths_b = self.process_in(in_paths_b)
 
-        hs.check_create_dir(out_dir)
-        self.out_dir = out_dir
+        if out_dir:
+            out_dir = os.path.abspath(out_dir)
+            ext = os.path.splitext(out_dir)[1]
+            if ext:
+                hs.print_update(f"Warning: Extension {ext} was found. Make sure to provide a single output directory.")
+            hs.check_create_dir(out_dir)
+            self.out_dir = out_dir
+        else:
+            self.out_dir = os.path.dirname(self.in_paths_a[0])
 
         self.export_svg = export_svg
 
         self.label_a = label_a
         self.label_b = label_b
         
         try:
-            feature_idx = {"deletion_rate": 16,
-                           "insertion_rate": 17,
-                           "mismatch_rate": 19,
-                           "mismatch_rate_alt": 20}
+            feature_idx = {"deletion": 16,
+                           "insertion": 17,
+                           "mismatch": 19,
+                           "mismatch_alt": 20}
             self.error_feature_idx = feature_idx[error_feature]
         except KeyError:
-            raise Exception(f"Invalid error feature '{error_feature}'. Use one of: deletion_rate, insertion_rate, mismatch_rate, mismatch_rate_alt")
+            raise Exception(f"Invalid error feature '{error_feature}'. Use one of: mismatch, mismatch_alt, deletion, insertion")
 
         self.error_threshold = error_threshold
         self.coverage_threshold = coverage_threshold
 
-        self.ref_dict = hs.get_references(ref_path, give_update=False)
+        self.ref_path = ref_path
+        self.n_bins_seqmap = n_bins_seqmap
 
     ##############################################################################################################
     #                                           Initialization methods                                           #
     ##############################################################################################################
 
     def process_in(self, in_paths: str) -> List[str]:
         """
@@ -80,15 +109,15 @@
         Returns:
         - in_list (List[str]): A list of validated input file paths.
 
         Raises:
         - Exception: If any input file does not exist or has an unexpected file extension.
         - Exception: If input files are of different kinds (either .bam or .pileup). All files must be of the same kind.
         """
-        in_list = in_paths.split(",")
+        in_list = [os.path.abspath(p) for p in in_paths.split(",")]
         extensions = []
         for path in in_list:
             ext = os.path.splitext(path)[1]
             extensions.append(ext)
             hs.check_input_path(path, extensions=[".tsv"])
 
         if len(set(extensions)) > 1:
@@ -97,55 +126,55 @@
 
     ##############################################################################################################
     #                                             Processing methods                                             #
     ##############################################################################################################
 
     def extract_positions(self) -> None:
         """
-        Extract positions based on coverage and error thresholds, identify systematic positions,
-        and categorize them into overlapping and exclusive sets for datasets A and B.
+        Extract positions based on coverage and error thresholds, identify systematic positions 
+        (i.e. those that are found in all replicates), and categorize them into overlapping and 
+        exclusive sets for datasets A and B. Identified positions are stored in the a_and_b, 
+        a_excl and b_excl member variables.
         """
-        subsets_a = [self.extract_suffient_cvg_pos(path) for path in self.in_paths_a]
-        subsets_b = [self.extract_suffient_cvg_pos(path) for path in self.in_paths_b]
-
-        a_high_cvg = [pos[0] for pos in subsets_a]
-        a_high_err = [pos[1] for pos in subsets_a]
-        del(subsets_a)
-
-        b_high_cvg = [pos[0] for pos in subsets_b]
-        b_high_err = [pos[1] for pos in subsets_b]
-        del(subsets_b)
+        a_high_cvg, b_high_cvg, a_high_err, b_high_err = [], [], [], []
+        for paths, high_cvg, high_err in [(self.in_paths_a, a_high_cvg, a_high_err), (self.in_paths_b, b_high_cvg, b_high_err)]:
+            for path in paths:
+                hc, he = self.extract_suffient_cvg_pos(path)
+                high_cvg.append(hc)
+                high_err.append(he)
 
         a_high_cvg_syst = self.find_systematic_pos(a_high_cvg)
         del(a_high_cvg)
         a_high_err_syst = self.find_systematic_pos(a_high_err)
         del(a_high_err)
 
         b_high_cvg_syst = self.find_systematic_pos(b_high_cvg)
         del(b_high_cvg)
         b_high_err_syst = self.find_systematic_pos(b_high_err)
         del(b_high_err)
 
         a_and_b = set.intersection(a_high_err_syst, b_high_err_syst)
+        # filter out positions that are exclusive because of high error rates (not insufficient coverage)
         a_excl = set.intersection(a_high_err_syst, b_high_cvg_syst-a_and_b)
         b_excl = set.intersection(b_high_err_syst, a_high_cvg_syst-a_and_b)
 
         self.a_and_b = sorted(a_and_b)
         self.a_excl = sorted(a_excl)
         self.b_excl = sorted(b_excl)
 
-    def extract_suffient_cvg_pos(self, path: str) -> Tuple[List[Tuple[str, int]], List[Tuple[str, int]]]:
+    def extract_suffient_cvg_pos(self, path: str) -> Tuple[List[SITE], List[SITE]]:
         """
         Extract positions with sufficient coverage and error rate from the specified input file.
 
         Parameters:
         - path (str): Path to the input file.
 
         Returns:
-        - Tuple[List[Tuple[str, int]], List[Tuple[str, int]]]: Two lists of positions - one for high coverage and one for high error rate.
+        - List[Tuple[str, int]]: Sites with high coverage (>=coverage threshold)
+        - List[Tuple[str, int]]]: Sites with high coverage AND high error rate (>=error rate threshold)
 
         Note:
         - Uses the error feature index specified during object initialization.
         """
         hs.print_update(f"Processing {path} ... ", line_break=False)
         sys.stdout.flush()
         with open(path, "r") as file:
@@ -161,34 +190,35 @@
                     if error_rate >= self.error_threshold:
                         high_cvg_high_err_sites.append((chrom, site))
 
             hs.print_update("done", with_time=False)
 
             return high_cvg_sites, high_cvg_high_err_sites
 
-    def find_systematic_pos(self, replicate_pos: List[List[Tuple[str, int]]]) -> List[Tuple[str, int]]:
+    def find_systematic_pos(self, replicate_pos: List[List[SITE]]) -> Set[SITE]:
         """
         Identify systematic positions that are common across multiple replicates.
 
         Parameters:
-        - replicate_pos (List[List[Tuple[str, int]]]): List of positions from multiple replicates.
+        - replicate_pos (List[List[Tuple[str, int]]]): List of lists, where each sublist contains coordinates from a given replicate.
 
         Returns:
         - List[Tuple[str, int]]: List of systematic positions.
         """
-        replicate_pos = [set(pos) for pos in replicate_pos]
-        return set.intersection(*replicate_pos)
+        # https://stackoverflow.com/questions/2541752/best-way-to-find-the-intersection-of-multiple-sets
+        replicate_pos_set = [set(pos) for pos in replicate_pos]
+        return set.intersection(*replicate_pos_set) # type: ignore
 
     def write_bed_files(self) -> None:
         """Write BED files for overlapping and exclusive positions."""
         self.positions_to_bed(self.a_and_b, self.out_dir, f"{self.label_a}_{self.label_b}")
         self.positions_to_bed(self.a_excl, self.out_dir, f"{self.label_a}_excl")
         self.positions_to_bed(self.b_excl, self.out_dir, f"{self.label_b}_excl")
 
-    def positions_to_bed(self, positions: Set[Tuple[str, int]], out_dir: str, name: str) -> None:
+    def positions_to_bed(self, positions: List[SITE], out_dir: str, name: str) -> None:
         """
         Write positions to a BED file.
 
         Parameters:
         - positions (Set[Tuple[str, int]]): Set of positions to be written.
         - out_dir (str): Output directory.
         - name (str): Name for the output BED file.
@@ -202,15 +232,15 @@
 
     
 
     ##############################################################################################################
     #                                          Summary creation methods                                          #
     ##############################################################################################################
 
-    def custom_sort_key(self, item):
+    def custom_sort_key(self, item) -> Tuple[int] | Tuple[float, Any]:
         """
         Define a custom sorting key for sorting mixed alphanumeric items.
 
         This method defines a custom sorting key that can be used with the `sorted()` function or other sorting functions.
         It allows for sorting a list of mixed alphanumeric items in a way that numeric values are sorted numerically,
         and non-numeric values are placed at the end of the sorted list.
 
@@ -223,86 +253,192 @@
             - If the item is not numeric, it is placed last with a float('inf') value to ensure it comes after numeric values.
 
         Example:
             To sort a list of mixed alphanumeric items, you can use this custom sorting key as follows:
             ```
             sorted_list = sorted(my_list, key=obj.custom_sort_key)
             ```
-
         """
         if item.isdigit():  # Check if the item is a digit
             return (int(item),)  # Convert to integer and sort numerically
         else:
             return (float('inf'), item)  # Place non-digits at the end
 
-
-    def create_plot(self) -> go.Figure:
+    def update_plot(self, fig, title: str|None = None, xlab: str|None = None, ylab: str|None = None, height: int = 500, width: int = 800) -> go.Figure:
         """
-        Create a Plotly figure representing the chromosome-wise distribution of positions.
+        Updates the layout of a Plotly figure.
+
+        Parameters:
+        - fig (go.Figure): The Plotly figure to be updated.
+        - title (str | None): Title of the plot (optional).
+        - xlab (str | None): Label for the x-axis (optional).
+        - ylab (str | None): Label for the y-axis (optional).
+        - height (int): Height of the plot (default: 500).
+        - width (int): Width of the plot (default: 800).
 
         Returns:
-        - go.Figure: The Plotly figure.
+        - go.Figure: The updated Plotly figure.
         """
-        def update_plot(fig, title: str|None = None, xlab: str|None = None, ylab: str|None = None, height: int = 500, width: int = 800):
-            """
-            Updates the layout of a Plotly figure.
+        fig.update_layout(template="seaborn",
+                    title = title,
+                    xaxis_title = xlab,
+                    yaxis_title = ylab,
+                    font=dict(family="Open sans, sans-serif", size=20),
+                    plot_bgcolor="white",
+                    margin=dict(l=50, r=50, t=50, b=50),
+                    height=height,  # Set the height to a constant value
+                    width=width)
+        fig.update_xaxes(showline=True, linewidth=2, linecolor='black', mirror=True, showticklabels=True, ticks='outside', showgrid=False, tickwidth=2)
+        fig.update_yaxes(showline=True, linewidth=2, linecolor='black', mirror=True, showticklabels=True, ticks='outside', showgrid=False, tickwidth=2)
+        return fig
 
-            Parameters:
-            - fig (go.Figure): The Plotly figure to be updated.
-            - title (str | None): Title of the plot (optional).
-            - xlab (str | None): Label for the x-axis (optional).
-            - ylab (str | None): Label for the y-axis (optional).
-            - height (int): Height of the plot (default: 500).
-            - width (int): Width of the plot (default: 800).
+    def prepare_data_map(self) -> Tuple[List[float], Dict[str, Dict[str, List[int]]], Dict[str, Dict[str, List[int]]], Dict[str, List[int]]]:
+        """
+        Prepare data for generating a genomic sequence map.
 
-            Returns:
-            - go.Figure: The updated Plotly figure.
-            """
-            fig.update_layout(template="seaborn",
-                        title = title,
-                        xaxis_title = xlab,
-                        yaxis_title = ylab,
-                        font=dict(family="Open sans, sans-serif", size=20),
-                        plot_bgcolor="white",
-                        margin=dict(l=50, r=50, t=50, b=50),
-                        height=height,  # Set the height to a constant value
-                        width=width)
-            fig.update_xaxes(showline=True, linewidth=2, linecolor='black', mirror=True, showticklabels=True, ticks='outside', showgrid=False, tickwidth=2)
-            fig.update_yaxes(showline=True, linewidth=2, linecolor='black', mirror=True, showticklabels=True, ticks='outside', showgrid=False, tickwidth=2)
-            return fig
-        
-        chr_a_and_b = [pos[0] for pos in self.a_and_b]
-        sites_a_and_b = [pos[1] for pos in self.a_and_b]
+        Returns:
+        - List[float]: A list of y-values that function as the y-values between 0 and 1 for each bin.
+        - Dict[str, Dict[str, List[int]]]: Nested dictionary containing the counts scaled between 0 and 255 for each 
+                                            sequence (upper level) and group (lower level). Values for each group are 
+                                            combined to create a RGB color based on the counts
+        - Dict[str, Dict[str, List[int]]]: Nested dictionary containing the absolute counts for each sequence (upper 
+                                            level) and group (lower level)
+        - Dict[str, List[int]]: A dictionary mapping sequence names to lists of maximum values for bin boundaries.         
+        """
+        # transform the sets into dictionaries for easier data handling
+        a_and_b_dict = defaultdict(lambda: [])
+        a_excl_dict = defaultdict(lambda: [])
+        b_excl_dict = defaultdict(lambda: [])
+        for d, d_dict in [(self.a_and_b, a_and_b_dict), (self.a_excl, a_excl_dict), (self.b_excl, b_excl_dict)]:
+            for seq, coord in d:
+                d_dict[seq].append(coord)
+        a_and_b_dict = dict(a_and_b_dict)
+        a_excl_dict = dict(a_excl_dict)
+        b_excl_dict = dict(b_excl_dict)
+
+        # Calculate chromosome lengths
+        def get_ref_len(ref_path: str) -> Dict[str, int]:
+            """Reads reference file and extracts chromosome lengths."""
+            with open(ref_path, "r") as ref:
+                refs = {}
+                line = next(ref)
+                seq_name = line[1:].strip().split(" ")[0]
+                seq_len = 0
+
+                for line in ref:
+                    if line.startswith(">"):
+                        refs[seq_name] = seq_len
+                        seq_name = line[1:].strip().split(" ")[0]
+                        seq_len = 0
+                    else:
+                        seq_len += len(line.strip())
+                refs[seq_name] = seq_len # add the last dict entry
+            return refs
+        ref_lens = get_ref_len(self.ref_path)
+
+        # get sequences that are present (iterate over these only)
+        present_seq = set(a_and_b_dict.keys()) | set(a_excl_dict.keys()) | set(b_excl_dict.keys())
+        # initialize the counts for all three groups with zeroes
+        counts = defaultdict(lambda: {f"{self.label_a}+{self.label_b}": [0]*self.n_bins_seqmap, self.label_a: [0]*self.n_bins_seqmap, self.label_b: [0]*self.n_bins_seqmap})
+        bin_sizes = {} 
+        max_vals = {} # stores the values for labelling the bins
+        for seq in present_seq:
+            seq_len = ref_lens[seq]
+
+            bin_size = math.ceil(seq_len / self.n_bins_seqmap)
+            bin_sizes[seq] = bin_size
+            # initialize the maximum coordinates that a bin may contain (excluded)
+            max_vals[seq] = [bin_size*i for i in range(1,self.n_bins_seqmap)] + [seq_len+1] 
+
+            # fill the counts dictionary
+            for d_dict, key in [(a_and_b_dict, f"{self.label_a}+{self.label_b}"), (a_excl_dict, self.label_a), (b_excl_dict, self.label_b)]:
+                if seq in d_dict.keys():
+                    for coord in d_dict[seq]:
+                        bin_index = coord // bin_size
+                        counts[seq][key][bin_index] += 1    
+        counts = dict(counts)
+
+        # scale the values between 0 and 255 to use as RGB values for each bin of the map
+        counts_scaled = {}
+        max_val_ab = max([max(counts[seq][f"{self.label_a}+{self.label_b}"]) for seq in present_seq])
+        max_val_a = max([max(counts[seq][self.label_a]) for seq in present_seq])
+        max_val_b = max([max(counts[seq][self.label_b]) for seq in present_seq])
+        for seq in counts.keys():
+            counts_scaled[seq] = {}
+            for group, max_val in [(f"{self.label_a}+{self.label_b}", max_val_ab), (self.label_a, max_val_a), (self.label_b, max_val_b)]:
+                scaled = [round(i/max_val * 255) if max_val>0 else 0 for i in counts[seq][group]]
+                counts_scaled[seq][group] = scaled
 
-        chr_a_excl = [pos[0] for pos in self.a_excl]
-        sites_a_excl = [pos[1] for pos in self.a_excl]
+        # Generate y-values for bin positions along the chromosome
+        y_vals = [i/self.n_bins_seqmap for i in range(self.n_bins_seqmap)]
 
-        chr_b_excl =[pos[0] for pos in self.b_excl]
-        sites_b_excl =[pos[1] for pos in self.b_excl]
+        return y_vals, counts_scaled, counts, max_vals
 
-        all_keys = self.ref_dict.keys()
-        present_chr = set((all_keys & chr_a_and_b) | (all_keys & chr_a_excl) | (all_keys & chr_b_excl))
-        present_chr = list(sorted(present_chr, key=self.custom_sort_key))
-        chr_lens = [len(self.ref_dict[x]) for x in present_chr]
-
-        width = 1200
-        bargap = 0.9
-        bar_width = 1-bargap+0.15
-        n_bars = len(present_chr)
-        scatter_size = width/n_bars*bar_width
-
-        fig = update_plot(go.Figure(), height = 1000, width = width)
-        fig.add_trace(go.Bar(x=present_chr, y=chr_lens, marker=dict(color="lightgrey", line=dict(color="black", width=2)), name="Chromosomes", showlegend=False))
-        fig.update_layout(bargap=0.5, yaxis=dict(range=[0,max(chr_lens)+0.1*max(chr_lens)]))
-
-        fig.add_trace(go.Scatter(x=chr_a_and_b, y=sites_a_and_b, mode='markers', marker=dict(symbol='line-ew', color="#1f77b4", size=scatter_size, line=dict(width=1.1, color="#1f77b4")), name=f"{self.label_a}+{self.label_b}", hovertemplate="Chr%{x}:%{y}"))
-        fig.add_trace(go.Scatter(x=chr_a_excl, y=sites_a_excl, mode='markers', marker=dict(symbol='line-ew', color="#ff7f0e", size=scatter_size, line=dict(width=1.1, color="#ff7f0e")), name=f"{self.label_a}", hovertemplate="Chr%{x}:%{y}"))
-        fig.add_trace(go.Scatter(x=chr_b_excl, y=sites_b_excl, mode='markers', marker=dict(symbol='line-ew', color="#2ca02c", size=scatter_size, line=dict(width=1.1, color="#2ca02c")), name=f"{self.label_b}", hovertemplate="Chr%{x}:%{y}"))
-        fig.update_xaxes(fixedrange=True)
+    def create_map_plot(self) -> go.Figure:
+        """
+        Create a genomic sequence map plot using Plotly.
 
+        Returns:
+        - go.Figure: A Plotly figure object representing the genomic sequence map.
+        """
+        y_vals, counts_scaled, counts, max_vals = self.prepare_data_map()
+        fig = go.Figure()
+        fig = self.update_plot(fig, width=1200, height=1000)
+        tickvals = []
+        ticktext = []
+        bin_height = y_vals[1]
+        # set up a map for each sequence that is present
+        for x, seq in enumerate(counts.keys(), start = 1):
+            tickvals.append(x)
+            ticktext.append(seq)
+            bin_start = [1]+max_vals[seq] # first position of a bin (included)
+            bin_end = max_vals[seq] # last position of a bin (excluded)
+            bins = []
+            for y, r, g, b, count_ab, count_a, count_b, lab_start, lab_end in zip(y_vals, 
+                                                                                counts_scaled[seq][f"{self.label_a}+{self.label_b}"], 
+                                                                                counts_scaled[seq][self.label_a], 
+                                                                                counts_scaled[seq][self.label_b], 
+                                                                                counts[seq][f"{self.label_a}+{self.label_b}"], 
+                                                                                counts[seq][self.label_a], 
+                                                                                counts[seq][self.label_b], 
+                                                                                bin_start, bin_end):
+                # the fill color is determined by the number of shared and exclusive positions in a bin
+                # red portion corresponds to the number of shared positions, green and blue to A excl. and 
+                # b excl. respectively. I.e.: High red portion in the color of a bin -> more shared positions
+                # and so on
+                color = f"rgb({r},{g},{b})"
+                # create a rectangle for each bin
+                bin = go.Scatter(x=[x-0.3, x-0.3, x+0.3, x+0.3, x-0.3], 
+                                y=[y,y+bin_height,y+bin_height,y,y], 
+                                name=f"{lab_start}-{lab_end}<br>{self.label_a}+{self.label_b}: {count_ab}<br>{self.label_a}: {count_a}<br>{self.label_b}: {count_b}",
+                                fill="toself", 
+                                fillcolor=color,
+                                marker=dict(color=color),
+                                showlegend=False, mode='lines')
+                bins.append(bin)
+            # add rectangles of one sequence to figure
+            fig.add_traces(bins)
+            # surround rectangles by a shape as a border
+            fig.add_shape(type="rect",
+                        x0=x - 0.3, y0=0,
+                        x1=x + 0.3, y1=1,
+                        line=dict(color="#000000", width=3),
+                        fillcolor="rgba(0,0,0,0)",
+                        xref="x", yref="y")
+
+        fig.update_xaxes(tickmode = 'array',
+                        tickvals = tickvals,
+                        ticktext = ticktext)
+        fig.update_yaxes(tickmode = 'array',
+                        tickvals = [0,1],
+                        ticktext = ["5'", "3'"])
+        fig.update_xaxes(range=[0.5,tickvals[-1]+0.5])
+
+        # clean up hoverlabels
+        fig.update_layout(hoverlabel=dict(namelength=0)) 
         return fig
 
     def get_file_paths(self) -> Tuple[str, str]:
         """
         Get formatted HTML lists of input file paths for datasets A and B.
 
         Returns:
@@ -370,33 +506,30 @@
         """
         Create a summary HTML file containing an overview of shared and exclusive positions in samples A and B.
 
         This method generates a summary HTML file that includes information about the input files, a count table, and a genome map.
 
         If export_svg is True, the genome map is saved as an SVG file in the specified output directory.
 
-        The HTML file is saved with the format: "<out_dir>/<label_a>_<label_b>_summary.html".
-
-        Returns:
-        - None
+        The HTML file is saved with the format: "<out_dir>/<label_a>_<label_b>_diff.html".
         """
-        plot = self.create_plot()
+        plot = self.create_map_plot()
         if self.export_svg:
             self.write_svg(plot, "twosample_map")
         
         plot = to_html(plot, include_plotlyjs=False)
 
         paths_1, paths_2 = self.get_file_paths()
         count_table = self.create_count_table()
         time = datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
 
         css_string, plotly_js_string = hs.load_html_template_str()
 
-        outpath = os.path.join(self.out_dir, f"{self.label_a}_{self.label_b}_summary.html")
-
+        outpath = os.path.join(self.out_dir, f"{self.label_a}_{self.label_b}_diff.html")
+        hs.print_update(f"Writing summary to {outpath}")
         template = f"""
                     <!DOCTYPE html>
                     <html lang="en">
                     <head>
                         <meta charset="UTF-8">
                         <meta http-equiv="X-UA-Compatible" content="IE=edge">
                         <meta name="viewport" content="width=device-width, initial-scale=1.0">
@@ -438,24 +571,28 @@
                                 <div class="table-box">
                                     {count_table}
                                 </div>
                             </div>
                         </section>
 
                         <section>
-                            <button class="collapsible">Genome map</button>
+                            <button class="collapsible">Sequence map</button>
                             <div class="collapsible-content">
                                 <h2 class="hiddentitle" id="genome_map"></h2>
-                                <h3>Genome map displaying shared and exclusive positions between samples <i>{self.label_a}</i> and <i>{self.label_b}</i></h3>
+                                <h3>Sequence map displaying shared and exclusive positions between samples <i>{self.label_a}</i> and <i>{self.label_b}</i></h3>
                                 <div class="plot-container">
                                     {plot}
                                 </div>
                                 <p>
-                                    Genome map displaying the positions that are present in both samples, only in sample <i>{self.label_a}</i> and only in sample <i>{self.label_b}</i>.
-                                    Only chromosomes that contain extracted position(s) are shown.  
+                                    Sequence map displaying the positions that are present in both samples, only in sample <i>{self.label_a}</i> and only in sample <i>{self.label_b}</i>.
+                                    Sequences are split into {self.n_bins_seqmap} chunks of equal size. The color of a chunk is determined by the number of shared and exclusive positions,
+                                    where the count of <span style="color:red;">shared positions</span> influences the <span style="color:red;">red</span> portion of a given RGB color, the count of 
+                                    <span style="color:green;"><i>{self.label_a}</i>-exclusive positions</span> influence the <span style="color:green;">green</span> portion and 
+                                    <span style="color:blue;"><i>{self.label_b}</i>-exclusive positions</span> influence the <span style="color:blue;">blue</span> portion. Higher counts in a given 
+                                    category increases the intensity of the given color portion. Black indicates sequence segments where no high-coverage and high-error sites were indentified.
                                 </p>
                             </div>
                         </section>
 
                         <script>
                             var coll = document.getElementsByClassName("collapsible");
                             var i;
@@ -487,14 +624,19 @@
         """
         Execute the main workflow of the PositionExtractor class.
 
         This method performs the following tasks:
         1. Extract positions from input files.
         2. Write BED files for shared and exclusive positions.
         3. Create a summary HTML file containing an overview of shared and exclusive positions.
-
-        Returns:
-        - None
         """
         self.extract_positions()
         self.write_bed_files()
-        self.create_summary()
+        self.create_summary()
+        hs.print_update("Finished.")
+
+
+if __name__=="__main__":
+    e = PositionExtractor(in_paths_a="/home/vincent/projects/neet_project/testing/testing_pileup_extractor/data1/cyt1.tsv,/home/vincent/projects/neet_project/testing/testing_pileup_extractor/data1/cyt2.tsv,/home/vincent/projects/neet_project/testing/testing_pileup_extractor/data1/cyt3.tsv",
+                          in_paths_b="/home/vincent/projects/neet_project/testing/testing_pileup_extractor/data1/nuc1.tsv,/home/vincent/projects/neet_project/testing/testing_pileup_extractor/data1/nuc2.tsv,/home/vincent/projects/neet_project/testing/testing_pileup_extractor/data1/nuc3.tsv",
+                          ref_path="/home/vincent/projects/neet_project/testing/data1/ref/ref.fa")
+    e.main()
```

### Comparing `neet-nanopore-0.0.4/neet_nanopore.egg-info/PKG-INFO` & `neet_nanopore-1.0.0/neet_nanopore.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,51 +1,71 @@
 Metadata-Version: 2.1
 Name: neet-nanopore
-Version: 0.0.4
+Version: 1.0.0
 Home-page: https://github.com/dietvin/neet
 Author: Vincent Dietrich
 Author-email: dietricv@uni-mainz.de
 License: LICENSE
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Operating System :: OS Independent
 Requires-Python: >3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: plotly==5.18.0
+Requires-Dist: kaleido==0.2.1
+Requires-Dist: numpy==1.26.2
+Requires-Dist: pandas==2.1.4
 Requires-Dist: tqdm==4.66.1
 Requires-Dist: intervaltree==3.1.0
 Requires-Dist: scipy==1.11.4
+Requires-Dist: statsmodels==0.14.1
 Requires-Dist: pyfiglet==1.0.2
 Requires-Dist: setuptools==69.0.3
-Requires-Dist: pandas==2.1.4
 
 # NEET - Nanopore Error pattern Exploration Toolkit
 
 The Nanopore Error pattern Exploration Toolkit (`NEET`) provides a range of functionalities that provide an easily accessible and interactive analysis approach for (systematic) base-calling errors in direct RNA nanopore sequencing data. The implemented modules include options for condensing, visualizing and differentiating error features contained in direct RNA sequencing data - including mismatch, deletion and insertion rates, among others.
 
 ## Installation
+
 It is recommended to use Conda/Mamba and pip for installation:
+
 ```
 conda create -y -n neet python==3.10 && conda activate neet
 pip install neet-nanopore
 neet --version
 ```
+
 For more information and alternative installation approaches refer to the [Wiki](https://github.com/dietvin/neet/wiki/01-Installation).
 
 ## General usage
+
 Once installed `NEET` can be accessed via the terminal:
+
 ```
 neet --help
 ```
+
 Individual modules can be accessed as follows:
+
 ```
 neet [MODULE] --help
 ```
-Available modules are: Pileup Extractor (`extractor`), Summary (`summmary`), Position-of-Interest Analyzer (`analyzepoi`), Two-Sample Extractor (`twosample`), Position Summary (`possummary`), Filter (`filter`) and Bedops (`bedops`). 
-The modules are interconnected to provide different workflows for different scenarios. An overview of the main workflows is given below:
+
+Available modules are:
+
+- Pileup Extractor (`extractor`): Extract data from pileup files into feature tables
+- Summary (`summmary`): Summarize and visualize feature tables
+- Position-of-Interest Summary (`poisummary`): Summarize and visualize specific positions of interest
+- Position-of-Interest View (`poiview`): Visualize positions of interest
+- Position-of-Interest  (`poicompare`): Statistically compare positions of interest
+- Two-Sample Extractor (`extractdiff`): Identify and extract positions of increased error rates between two conditions
+- Filter (`filter`): Filter feature tables by given features
+- Bedops (`bedops`): Process and manipulate bed files
+  The modules are interconnected to provide different workflows for different scenarios. An overview of the main workflows is given below:
 
 ![Main workflow overview](https://github.com/dietvin/neet/blob/main/images/workflow_overview.jpg)
 
 A detailled description of all available modules is provided in the [Wiki](https://github.com/dietvin/neet/wiki/02-Modules). The Wiki also provides [walkthroughs](https://github.com/dietvin/neet/wiki/03-Example-Workflows) for some possible use cases.
```

### Comparing `neet-nanopore-0.0.4/neet_nanopore.egg-info/SOURCES.txt` & `neet_nanopore-1.0.0/neet_nanopore.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 neet/__init__.py
 neet/__main__.py
 neet/__version__.py
 neet/bed_ops.py
 neet/filter.py
 neet/helper_functions.py
 neet/pileup_extractor.py
-neet/poi_analyzer.py
-neet/position_summary.py
+neet/poi_sample_comparer.py
+neet/poi_summary.py
+neet/poi_view.py
 neet/summary.py
 neet/two_sample_extractor.py
 neet/summary_style/__init__.py
 neet/summary_style/plotly.js
 neet/summary_style/style.css
 neet_nanopore.egg-info/PKG-INFO
 neet_nanopore.egg-info/SOURCES.txt
```

### Comparing `neet-nanopore-0.0.4/setup.py` & `neet_nanopore-1.0.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 #!/usr/bin/env python
 
 from setuptools import setup
 
+exec(open("neet/__version__.py").read())
+
 setup(name="neet",
-      version="0.0.4",
+      version=__version__, # type: ignore (imported from __version__.py above)
       description="Nanopore error pattern exploration toolkit",
       author="Vincent Dietrich",
       author_email="dietricv@uni-mainz.de",
       url="https://github.com/dietvin/neet",
       license="LICENSE",
       packages=["neet", "neet.summary_style"],
       entry_points={"console_scripts": ["neet = neet.__main__:main",],},
       python_requires=">3.9",
-      install_requires=["plotly==5.18.0", 
+      install_requires=["plotly==5.18.0",
+                        "kaleido==0.2.1",
+                        "numpy==1.26.2",
+                        "pandas==2.1.4",
                         "tqdm==4.66.1", 
                         "intervaltree==3.1.0", 
                         "scipy==1.11.4", 
+                        "statsmodels==0.14.1",
                         "pyfiglet==1.0.2", 
-                        "setuptools==69.0.3",
-                        "pandas==2.1.4"],
+                        "setuptools==69.0.3"],
       long_description=open('README.md').read(),
       long_description_content_type='text/markdown',
       package_data = {"neet.summary_style": ["plotly.js", "style.css"]},
       classifiers=["Environment :: Console",
                    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
                    "Programming Language :: Python :: 3",
                    "Topic :: Scientific/Engineering :: Bio-Informatics",
```

