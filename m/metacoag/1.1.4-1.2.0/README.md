# Comparing `tmp/metacoag-1.1.4.tar.gz` & `tmp/metacoag-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metacoag-1.1.4.tar", last modified: Mon Jul 24 23:59:38 2023, max compression
+gzip compressed data, was "metacoag-1.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `metacoag-1.1.4.tar` & `metacoag-1.2.0.tar`

### file list

```diff
@@ -1,31 +1,28 @@
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-07-24 23:59:38.311308 metacoag-1.1.4/
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     5232 2022-08-05 12:06:27.000000 metacoag-1.1.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)    35149 2022-08-05 12:06:27.000000 metacoag-1.1.4/LICENSE
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      343 2023-02-14 12:08:36.000000 metacoag-1.1.4/MANIFEST.in
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)    10606 2023-07-24 23:59:38.311012 metacoag-1.1.4/PKG-INFO
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     9888 2023-06-01 00:40:34.000000 metacoag-1.1.4/README.md
--rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)    39668 2023-07-24 06:31:05.000000 metacoag-1.1.4/metacoag
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-07-24 23:59:38.149155 metacoag-1.1.4/metacoag.egg-info/
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)    10606 2023-07-24 23:59:38.000000 metacoag-1.1.4/metacoag.egg-info/PKG-INFO
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      647 2023-07-24 23:59:38.000000 metacoag-1.1.4/metacoag.egg-info/SOURCES.txt
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)        1 2023-07-24 23:59:38.000000 metacoag-1.1.4/metacoag.egg-info/dependency_links.txt
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       72 2023-07-24 23:59:38.000000 metacoag-1.1.4/metacoag.egg-info/entry_points.txt
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       62 2023-07-24 23:59:38.000000 metacoag-1.1.4/metacoag.egg-info/requires.txt
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       15 2023-07-24 23:59:38.000000 metacoag-1.1.4/metacoag.egg-info/top_level.txt
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)        1 2022-11-25 05:01:14.000000 metacoag-1.1.4/metacoag.egg-info/zip-safe
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-07-24 23:59:38.153861 metacoag-1.1.4/metacoag_utils/
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     6148 2023-06-01 01:29:39.000000 metacoag-1.1.4/metacoag_utils/.DS_Store
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)        0 2022-08-05 12:06:27.000000 metacoag-1.1.4/metacoag_utils/__init__.py
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-07-24 23:59:38.154501 metacoag-1.1.4/metacoag_utils/auxiliary/
--rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20) 15929643 2022-08-05 12:06:27.000000 metacoag-1.1.4/metacoag_utils/auxiliary/marker.hmm
--rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)     1099 2022-08-05 12:06:27.000000 metacoag-1.1.4/metacoag_utils/bidirectionalmap.py
--rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)     6522 2023-07-24 06:31:05.000000 metacoag-1.1.4/metacoag_utils/feature_utils.py
--rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)    12073 2023-05-15 05:51:35.000000 metacoag-1.1.4/metacoag_utils/graph_utils.py
--rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)    15011 2023-07-24 06:31:05.000000 metacoag-1.1.4/metacoag_utils/label_prop_utils.py
--rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)     8923 2023-07-24 06:31:05.000000 metacoag-1.1.4/metacoag_utils/marker_gene_utils.py
--rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)    15606 2023-07-24 06:31:05.000000 metacoag-1.1.4/metacoag_utils/matching_utils.py
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-07-24 23:59:38.309336 metacoag-1.1.4/metacoag_utils/support/
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     6148 2023-06-01 01:29:39.000000 metacoag-1.1.4/metacoag_utils/support/.DS_Store
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1745 2023-06-13 02:12:10.000000 metacoag-1.1.4/metacoag_utils/support/combine_cov.py
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       38 2023-07-24 23:59:38.311398 metacoag-1.1.4/setup.cfg
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1574 2023-07-24 06:32:51.000000 metacoag-1.1.4/setup.py
+-rw-r--r--   0        0        0    35149 2024-04-24 05:53:58.299179 metacoag-1.2.0/LICENSE
+-rw-r--r--   0        0        0    10234 2024-04-24 05:53:58.299179 metacoag-1.2.0/README.md
+-rw-r--r--   0        0        0     4010 2024-04-24 05:53:58.299179 metacoag-1.2.0/docs/citation.md
+-rw-r--r--   0        0        0   139640 2024-04-24 05:53:58.299179 metacoag-1.2.0/docs/images/MetaCoAG_Logo.png
+-rw-r--r--   0        0        0   127240 2024-04-24 05:53:58.299179 metacoag-1.2.0/docs/images/MetaCoAG_Logo_dark.png
+-rw-r--r--   0        0        0   119215 2024-04-24 05:53:58.299179 metacoag-1.2.0/docs/images/MetaCoAG_Logo_light.png
+-rwxr-xr-x   0        0        0   877577 2024-04-24 05:53:58.307179 metacoag-1.2.0/docs/images/MetaCoAG_workflow.png
+-rw-r--r--   0        0        0      747 2024-04-24 05:53:58.307179 metacoag-1.2.0/docs/index.md
+-rw-r--r--   0        0        0     1066 2024-04-24 05:53:58.307179 metacoag-1.2.0/docs/install.md
+-rw-r--r--   0        0        0     2416 2024-04-24 05:53:58.307179 metacoag-1.2.0/docs/preprocess.md
+-rw-r--r--   0        0        0      300 2024-04-24 05:53:58.307179 metacoag-1.2.0/docs/requirements.txt
+-rw-r--r--   0        0        0     5491 2024-04-24 05:53:58.307179 metacoag-1.2.0/docs/usage.md
+-rw-r--r--   0        0        0      766 2024-04-24 05:53:58.307179 metacoag-1.2.0/docs/workflow.md
+-rw-r--r--   0        0        0     2000 2024-04-24 05:53:58.307179 metacoag-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       50 2024-04-24 05:53:58.307179 metacoag-1.2.0/requirements.txt
+-rw-r--r--   0        0        0      357 2024-04-24 05:53:58.307179 metacoag-1.2.0/src/metacoag/__init__.py
+-rwxr-xr-x   0        0        0    39864 2024-04-24 05:53:58.307179 metacoag-1.2.0/src/metacoag/cli.py
+-rw-r--r--   0        0        0      357 2024-04-24 05:53:58.307179 metacoag-1.2.0/src/metacoag/metacoag_utils/__init__.py
+-rwxr-xr-x   0        0        0 15929643 2024-04-24 05:53:58.359179 metacoag-1.2.0/src/metacoag/metacoag_utils/auxiliary/marker.hmm
+-rwxr-xr-x   0        0        0     1099 2024-04-24 05:53:58.359179 metacoag-1.2.0/src/metacoag/metacoag_utils/bidirectionalmap.py
+-rwxr-xr-x   0        0        0     6594 2024-04-24 05:53:58.359179 metacoag-1.2.0/src/metacoag/metacoag_utils/feature_utils.py
+-rwxr-xr-x   0        0        0    13080 2024-04-24 05:53:58.359179 metacoag-1.2.0/src/metacoag/metacoag_utils/graph_utils.py
+-rwxr-xr-x   0        0        0    15020 2024-04-24 05:53:58.359179 metacoag-1.2.0/src/metacoag/metacoag_utils/label_prop_utils.py
+-rwxr-xr-x   0        0        0     8923 2024-04-24 05:53:58.359179 metacoag-1.2.0/src/metacoag/metacoag_utils/marker_gene_utils.py
+-rwxr-xr-x   0        0        0    15606 2024-04-24 05:53:58.359179 metacoag-1.2.0/src/metacoag/metacoag_utils/matching_utils.py
+-rw-r--r--   0        0        0     1745 2024-04-24 05:53:58.359179 metacoag-1.2.0/src/metacoag/metacoag_utils/support/combine_cov.py
+-rw-r--r--   0        0        0     3784 2024-04-24 05:53:58.359179 metacoag-1.2.0/src/metacoag/metacoag_utils/support/gfa2fasta.py
+-rw-r--r--   0        0        0    11699 1970-01-01 00:00:00.000000 metacoag-1.2.0/PKG-INFO
```

### Comparing `metacoag-1.1.4/LICENSE` & `metacoag-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metacoag-1.1.4/PKG-INFO` & `metacoag-1.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,21 @@
-Metadata-Version: 2.1
-Name: metacoag
-Version: 1.1.4
-Summary: MetaCoAG: Binning Metagenomic Contigs via Composition, Coverage and Assembly Graphs
-Home-page: https://github.com/metagentools/MetaCoAG
-Author: Vijini Mallawaarachchi and Yu Lin
-Author-email: viji.mallawaarachchi@gmail.com
-License: GPL-3.0
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Natural Language :: English
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <p align="center">
-  <img src="https://raw.githubusercontent.com/metagentools/MetaCoAG/master/MetaCoAG_Logo.png" width="500" title="MetaCoAG logo" alt="MetaCoAG logo">
+  <img src="https://raw.githubusercontent.com/metagentools/MetaCoAG/develop/MetaCoAG_Logo.png" width="500" title="MetaCoAG logo" alt="MetaCoAG logo">
 </p>
 
 # MetaCoAG: Binning Metagenomic Contigs via Composition, Coverage and Assembly Graphs
 
 [![DOI](https://img.shields.io/badge/DOI-10.1007/978--3--031--04749--7__5-informational)](https://doi.org/10.1007/978-3-031-04749-7_5)
 [![DOI](https://img.shields.io/badge/DOI-10.1089/cmb.2022.0262-green)](https://doi.org/10.1089/cmb.2022.0262)
 [![Anaconda-Server Badge](https://anaconda.org/bioconda/metacoag/badges/version.svg)](https://anaconda.org/bioconda/metacoag)
 [![PyPI version](https://badge.fury.io/py/metacoag.svg)](https://badge.fury.io/py/metacoag)
 [![Anaconda-Server Badge](https://anaconda.org/bioconda/metacoag/badges/downloads.svg)](https://anaconda.org/bioconda/metacoag)
 
-[![CI](https://github.com/metagentools/MetaCoAG/actions/workflows/testing.yml/badge.svg)](https://github.com/metagentools/MetaCoAG/actions/workflows/testing.yml)
+[![CI](https://github.com/metagentools/MetaCoAG/actions/workflows/testing_python.yml/badge.svg)](https://github.com/metagentools/MetaCoAG/actions/workflows/testing_python.yml)
+[![Coverage Status](https://coveralls.io/repos/github/metagentools/MetaCoAG/badge.svg?branch=develop)](https://coveralls.io/github/metagentools/MetaCoAG?branch=develop)
 ![GitHub](https://img.shields.io/github/license/Vini2/MetaCoAG)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![CodeQL](https://github.com/metagentools/MetaCoAG/actions/workflows/codeql.yml/badge.svg)](https://github.com/metagentools/MetaCoAG/actions/workflows/codeql.yml)
 [![Documentation Status](https://readthedocs.org/projects/metacoag/badge/?version=latest)](https://metacoag.readthedocs.io/en/latest/?badge=latest)
 
 MetaCoAG is a metagenomic contig binning tool that makes use of the connectivity information found in assembly graphs, apart from the composition and coverage information. MetaCoAG makes use of single-copy marker genes along with a graph matching technique and a label propagation technique to bin contigs. MetaCoAG is tested on contigs obtained from next-generation sequencing (NGS) data. Currently, MetaCoAG supports contigs assembled using metaSPAdes and MEGAHIT, and recently we have added support for Flye assemblies (has not been tested extensively).
 
@@ -106,22 +89,29 @@
 ### Using `pip`
 You can run the following command to install MetaCoAG using `pip`. Make sure you are in the MetaCoAG folder.
 
 ```
 pip install .
 ```
 
-**Note:** If you use pip to setup MetaCoAG for development, you will have to install [FragGeneScan](https://sourceforge.net/projects/fraggenescan/) and [HMMER](http://hmmer.org/) manually and add them to your system path.
+### Using `flit`
+You can run the following command to install MetaCoAG using `flit`. Make sure you are in the MetaCoAG folder.
+
+```
+flit install
+```
+
+**Note:** If you use pip or flit to setup MetaCoAG for development, you will have to install [FragGeneScan](https://sourceforge.net/projects/fraggenescan/) and [HMMER](http://hmmer.org/) manually and add them to your system path.
 
 ### Test the setup
 
 After setting up, run the following command to ensure that metacoag is working.
 
 ```
-metacoag -h
+metacoag --help
 ```
 
 ## Example Usage
 
 ```
 metacoag --assembler spades --graph /path/to/graph_file.gfa --contigs /path/to/contigs.fasta --paths /path/to/paths_file.paths --abundance /path/to/abundance.tsv --output /path/to/output_folder
 ```
```

### Comparing `metacoag-1.1.4/README.md` & `metacoag-1.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,60 @@
+Metadata-Version: 2.1
+Name: metacoag
+Version: 1.2.0
+Summary: MetaCoAG: Binning Metagenomic Contigs via Composition, Coverage and Assembly Graphs
+Keywords: metagenomics,binning,contigs,bioinformatics
+Author-email: Vijini Mallawaarachchi <viji.mallawaarachchi@gmail.com>
+Requires-Python: >=3.9,<3.13
+Description-Content-Type: text/markdown
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Classifier: Operating System :: OS Independent
+Requires-Dist: biopython
+Requires-Dist: igraph
+Requires-Dist: networkx
+Requires-Dist: scipy
+Requires-Dist: numpy
+Requires-Dist: tqdm
+Requires-Dist: pandas
+Requires-Dist: click
+Requires-Dist: black ; extra == "dev"
+Requires-Dist: click ; extra == "dev"
+Requires-Dist: docformatter ; extra == "dev"
+Requires-Dist: flit ; extra == "dev"
+Requires-Dist: nox ; extra == "dev"
+Requires-Dist: isort ; extra == "dev"
+Requires-Dist: pytest ; extra == "dev"
+Requires-Dist: pytest-cov ; extra == "dev"
+Requires-Dist: pytest-xdist ; extra == "dev"
+Requires-Dist: nox ; extra == "test"
+Requires-Dist: pytest ; extra == "test"
+Requires-Dist: pytest-cov ; extra == "test"
+Requires-Dist: pytest-xdist ; extra == "test"
+Project-URL: Home, https://metacoag.readthedocs.io
+Provides-Extra: dev
+Provides-Extra: test
+
 <p align="center">
-  <img src="https://raw.githubusercontent.com/metagentools/MetaCoAG/master/MetaCoAG_Logo.png" width="500" title="MetaCoAG logo" alt="MetaCoAG logo">
+  <img src="https://raw.githubusercontent.com/metagentools/MetaCoAG/develop/MetaCoAG_Logo.png" width="500" title="MetaCoAG logo" alt="MetaCoAG logo">
 </p>
 
 # MetaCoAG: Binning Metagenomic Contigs via Composition, Coverage and Assembly Graphs
 
 [![DOI](https://img.shields.io/badge/DOI-10.1007/978--3--031--04749--7__5-informational)](https://doi.org/10.1007/978-3-031-04749-7_5)
 [![DOI](https://img.shields.io/badge/DOI-10.1089/cmb.2022.0262-green)](https://doi.org/10.1089/cmb.2022.0262)
 [![Anaconda-Server Badge](https://anaconda.org/bioconda/metacoag/badges/version.svg)](https://anaconda.org/bioconda/metacoag)
 [![PyPI version](https://badge.fury.io/py/metacoag.svg)](https://badge.fury.io/py/metacoag)
 [![Anaconda-Server Badge](https://anaconda.org/bioconda/metacoag/badges/downloads.svg)](https://anaconda.org/bioconda/metacoag)
 
-[![CI](https://github.com/metagentools/MetaCoAG/actions/workflows/testing.yml/badge.svg)](https://github.com/metagentools/MetaCoAG/actions/workflows/testing.yml)
+[![CI](https://github.com/metagentools/MetaCoAG/actions/workflows/testing_python.yml/badge.svg)](https://github.com/metagentools/MetaCoAG/actions/workflows/testing_python.yml)
+[![Coverage Status](https://coveralls.io/repos/github/metagentools/MetaCoAG/badge.svg?branch=develop)](https://coveralls.io/github/metagentools/MetaCoAG?branch=develop)
 ![GitHub](https://img.shields.io/github/license/Vini2/MetaCoAG)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![CodeQL](https://github.com/metagentools/MetaCoAG/actions/workflows/codeql.yml/badge.svg)](https://github.com/metagentools/MetaCoAG/actions/workflows/codeql.yml)
 [![Documentation Status](https://readthedocs.org/projects/metacoag/badge/?version=latest)](https://metacoag.readthedocs.io/en/latest/?badge=latest)
 
 MetaCoAG is a metagenomic contig binning tool that makes use of the connectivity information found in assembly graphs, apart from the composition and coverage information. MetaCoAG makes use of single-copy marker genes along with a graph matching technique and a label propagation technique to bin contigs. MetaCoAG is tested on contigs obtained from next-generation sequencing (NGS) data. Currently, MetaCoAG supports contigs assembled using metaSPAdes and MEGAHIT, and recently we have added support for Flye assemblies (has not been tested extensively).
 
@@ -88,22 +128,29 @@
 ### Using `pip`
 You can run the following command to install MetaCoAG using `pip`. Make sure you are in the MetaCoAG folder.
 
 ```
 pip install .
 ```
 
-**Note:** If you use pip to setup MetaCoAG for development, you will have to install [FragGeneScan](https://sourceforge.net/projects/fraggenescan/) and [HMMER](http://hmmer.org/) manually and add them to your system path.
+### Using `flit`
+You can run the following command to install MetaCoAG using `flit`. Make sure you are in the MetaCoAG folder.
+
+```
+flit install
+```
+
+**Note:** If you use pip or flit to setup MetaCoAG for development, you will have to install [FragGeneScan](https://sourceforge.net/projects/fraggenescan/) and [HMMER](http://hmmer.org/) manually and add them to your system path.
 
 ### Test the setup
 
 After setting up, run the following command to ensure that metacoag is working.
 
 ```
-metacoag -h
+metacoag --help
 ```
 
 ## Example Usage
 
 ```
 metacoag --assembler spades --graph /path/to/graph_file.gfa --contigs /path/to/contigs.fasta --paths /path/to/paths_file.paths --abundance /path/to/abundance.tsv --output /path/to/output_folder
 ```
@@ -156,7 +203,8 @@
 ## Funding
 
 MetaCoAG is funded by an [Essential Open Source Software for Science Grant](https://chanzuckerberg.com/eoss/proposals/cogent3-python-apis-for-iq-tree-and-graphbin-via-a-plug-in-architecture/) from the Chan Zuckerberg Initiative.
 
 <p align="left">
   <img src="https://chanzuckerberg.com/wp-content/themes/czi/img/logo.svg" width="300">
 </p>
+
```

### Comparing `metacoag-1.1.4/metacoag` & `metacoag-1.2.0/src/metacoag/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 import time
 
 import click
 from Bio import SeqIO
 from igraph import *
 from tqdm import tqdm
 
-from metacoag_utils import (feature_utils, graph_utils, label_prop_utils,
+from metacoag.metacoag_utils import (feature_utils, graph_utils, label_prop_utils,
                             marker_gene_utils, matching_utils)
-from metacoag_utils.bidirectionalmap import BidirectionalMap
+from metacoag.metacoag_utils.bidirectionalmap import BidirectionalMap
 
 __author__ = "Vijini Mallawaarachchi and Yu Lin"
 __copyright__ = "Copyright 2020, MetaCoAG Project"
 __license__ = "GPL-3.0"
-__version__ = "1.1.4"
+__version__ = "1.2.0"
 __maintainer__ = "Vijini Mallawaarachchi"
 __email__ = "vijini.mallawaarachchi@anu.edu.au"
 __status__ = "Stable Release"
 
 
 # Set global paramters
 # ---------------------------------------------------
@@ -39,15 +39,15 @@
 # Setup argument parser
 # ---------------------------------------------------
 
 @click.command()
 @click.option(
     "--assembler",
     help="name of the assembler used. (Supports SPAdes, MEGAHIT and Flye)",
-    type=click.Choice(["spades", "megahit", "megahitc", "flye"], case_sensitive=False),
+    type=click.Choice(["spades", "megahit", "megahitc", "flye", "custom"], case_sensitive=False),
     required=True,
 )
 @click.option(
     "--graph",
     help="path to the assembly graph file",
     type=click.Path(exists=True),
     required=True,
@@ -233,15 +233,15 @@
         if not prefix.endswith("_"):
             prefix = f"{prefix}_"
 
 
     # Setup logger
     # ------------------------------------------------------------------------
 
-    logger = logging.getLogger("MetaCoaAG 1.1.4")
+    logger = logging.getLogger("MetaCoaAG 1.2.0")
     logger.setLevel(logging.DEBUG)
     logging.captureWarnings(True)
     formatter = logging.Formatter("%(asctime)s - %(levelname)s - %(message)s")
     consoleHeader = logging.StreamHandler()
     consoleHeader.setFormatter(formatter)
     consoleHeader.setLevel(logging.INFO)
     logger.addHandler(consoleHeader)
@@ -329,87 +329,99 @@
     logger.info("MetaCoAG started")
     start_time = time.time()
 
 
     # Get links of the assembly graph
     # ------------------------------------------------------------------------
 
-    try:
-        if assembler == "spades":
-            # Get paths, segments, links and contigs of the assembly graph
-            (
-                paths,
-                segment_contigs,
-                node_count,
-                contigs_map,
-                contig_names,
-            ) = graph_utils.get_segment_paths_spades(contig_paths_file)
-
-            # Get reverse mapping of contig map
-            contigs_map_rev = contigs_map.inverse
-
-            # Get reverse mapping of contig identifiers
-            contig_names_rev = contig_names.inverse
-
-        if assembler == "megahit":
-            original_contigs = {}
-            contig_descriptions = {}
-
-            # Get mapping of original contig identifiers with descriptions
-            for index, record in enumerate(SeqIO.parse(contigs_file, "fasta")):
-                original_contigs[record.id] = str(record.seq)
-                contig_descriptions[record.id] = record.description
-
-            # Get links and contigs of the assembly graph
-            (
-                node_count,
-                graph_contigs,
-                links,
-                contig_names,
-            ) = graph_utils.get_links_megahit(assembly_graph_file)
-
-            # Get reverse mapping of contig identifiers
-            contig_names_rev = contig_names.inverse
-
-        if assembler == "flye":
-            # Get contigs map
-            contig_names = graph_utils.get_flye_contig_map(contigs_file)
-
-            # Get reverse mapping of contig identifiers
-            contig_names_rev = contig_names.inverse
-
-            # Get links and contigs of the assembly graph
-            (
-                paths,
-                segment_contigs,
-                node_count,
-                contigs_map,
-            ) = graph_utils.get_links_flye(contig_paths_file, contig_names_rev)
-
-            # Get reverse mapping of contig map
-            contigs_map_rev = contigs_map.inverse
-
-        if assembler == "megahitc":
-
-            # Get links and contigs of the assembly graph
-            (
-                node_count,
-                links,
-                contig_names,
-            ) = graph_utils.get_links_megahit_custom(assembly_graph_file)
-
-            # Get reverse mapping of contig identifiers
-            contig_names_rev = contig_names.inverse
-
-    except:
-        logger.error(
-            "Please make sure that the correct path to the contig paths file is provided."
-        )
-        logger.info("Exiting MetaCoAG... Bye...!")
-        sys.exit(1)
+    # try:
+    if assembler == "spades":
+        # Get paths, segments, links and contigs of the assembly graph
+        (
+            paths,
+            segment_contigs,
+            node_count,
+            contigs_map,
+            contig_names,
+        ) = graph_utils.get_segment_paths_spades(contig_paths_file)
+
+        # Get reverse mapping of contig map
+        contigs_map_rev = contigs_map.inverse
+
+        # Get reverse mapping of contig identifiers
+        contig_names_rev = contig_names.inverse
+
+    if assembler == "megahit":
+        original_contigs = {}
+        contig_descriptions = {}
+
+        # Get mapping of original contig identifiers with descriptions
+        for index, record in enumerate(SeqIO.parse(contigs_file, "fasta")):
+            original_contigs[record.id] = str(record.seq)
+            contig_descriptions[record.id] = record.description
+
+        # Get links and contigs of the assembly graph
+        (
+            node_count,
+            graph_contigs,
+            links,
+            contig_names,
+        ) = graph_utils.get_links_megahit(assembly_graph_file)
+
+        # Get reverse mapping of contig identifiers
+        contig_names_rev = contig_names.inverse
+
+    if assembler == "flye":
+        # Get contigs map
+        contig_names = graph_utils.get_flye_contig_map(contigs_file)
+
+        # Get reverse mapping of contig identifiers
+        contig_names_rev = contig_names.inverse
+
+        # Get links and contigs of the assembly graph
+        (
+            paths,
+            segment_contigs,
+            node_count,
+            contigs_map,
+        ) = graph_utils.get_links_flye(contig_paths_file, contig_names_rev)
+
+        # Get reverse mapping of contig map
+        contigs_map_rev = contigs_map.inverse
+
+    if assembler == "megahitc":
+
+        # Get links and contigs of the assembly graph
+        (
+            node_count,
+            links,
+            contig_names,
+        ) = graph_utils.get_links_megahit_custom(assembly_graph_file)
+
+        # Get reverse mapping of contig identifiers
+        contig_names_rev = contig_names.inverse
+
+    if assembler == "custom":
+
+        # Get links and contigs of the assembly graph
+        (
+            node_count,
+            links,
+            contig_names,
+        ) = graph_utils.get_links_custom(assembly_graph_file)
+
+        # Get reverse mapping of contig identifiers
+        contig_names_rev = contig_names.inverse
+
+    # except:
+    #     logger.error(
+    #         "Please make sure that the correct path to the contig paths file is provided."
+    #     )
+    #     logger.info("Exiting MetaCoAG... Bye...!")
+    #     sys.exit(1)
 
     # Construct the assembly graph
     # -------------------------------
 
     all_contigs = [x for x in range(node_count)]
 
     try:
@@ -440,18 +452,19 @@
                 assembly_graph_file=assembly_graph_file,
                 contigs_map=contigs_map,
                 contigs_map_rev=contigs_map_rev,
                 paths=paths,
                 segment_contigs=segment_contigs,
             )
 
-        if assembler == "megahit" or assembler == "megahitc":
+        if assembler == "megahit" or assembler == "megahitc" or assembler == "custom":
             edge_list = graph_utils.get_graph_edges_megahit(
                 links=links, contig_names_rev=contig_names_rev
             )
+        
 
         # Add edges to the graph
         assembly_graph.add_edges(edge_list)
 
         # Simplify the graph
         assembly_graph.simplify(multiple=True, loops=False, combine_edges=None)
```

### Comparing `metacoag-1.1.4/metacoag_utils/auxiliary/marker.hmm` & `metacoag-1.2.0/src/metacoag/metacoag_utils/auxiliary/marker.hmm`

 * *Files identical despite different names*

### Comparing `metacoag-1.1.4/metacoag_utils/bidirectionalmap.py` & `metacoag-1.2.0/src/metacoag/metacoag_utils/bidirectionalmap.py`

 * *Files identical despite different names*

### Comparing `metacoag-1.1.4/metacoag_utils/feature_utils.py` & `metacoag-1.2.0/src/metacoag/metacoag_utils/feature_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 #!/usr/bin/env python3
 
 import itertools
 import logging
 import os
 import pickle
 import sys
+from collections import defaultdict
 from multiprocessing import Pool
 
 import numpy as np
 from Bio import SeqIO
 
 # Create logger
-logger = logging.getLogger("MetaCoaAG 1.1.4")
+logger = logging.getLogger("MetaCoaAG 1.2.0")
 
 # Set complements of each nucleotide
 complements = {"A": "T", "C": "G", "G": "C", "T": "A"}
 
 # Set bits for each nucleotide
 nt_bits = {"A": 0, "C": 1, "G": 2, "T": 3}
 
@@ -115,17 +116,17 @@
         if contig_lengths[i] >= min_length:
             tetramer_profiles[i] = normalized_tetramer_profiles[i]
 
     return tetramer_profiles
 
 
 def get_cov_len(contigs_file, contig_names_rev, min_length, abundance_file):
-    coverages = {}
+    coverages = defaultdict(lambda: [0])
 
-    contig_lengths = {}
+    contig_lengths = defaultdict(int)
 
     i = 0
 
     sequences = []
 
     for index, record in enumerate(SeqIO.parse(contigs_file, "fasta")):
         contig_num = contig_names_rev[record.id]
```

### Comparing `metacoag-1.1.4/metacoag_utils/graph_utils.py` & `metacoag-1.2.0/src/metacoag/metacoag_utils/graph_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import multiprocessing as mp
 import re
 from collections import defaultdict
 
 from Bio import SeqIO
 
-from metacoag_utils.bidirectionalmap import BidirectionalMap
+from metacoag.metacoag_utils.bidirectionalmap import BidirectionalMap
 
 
 def get_segment_paths_spades(contig_paths):
     paths = {}
     segment_contigs = {}
     node_count = 0
 
@@ -325,14 +325,51 @@
                 my_map[node_count] = my_node
                 nodes.append(my_node)
                 node_count += 1
 
             # Identify lines with link information
             elif line.startswith("L"):
                 link = []
+                strings = line.split("\t")
+
+                if strings[1] != strings[3]:
+                    start = strings[1]
+                    end = strings[3]
+                    link.append(start)
+                    link.append(end)
+                    links.append(link)
+
+    return node_count, links, my_map
+
+
+def get_links_custom(assembly_graph_file):
+    my_map = BidirectionalMap()
+
+    node_count = 0
+
+    nodes = []
+
+    links = []
+
+    # Get contig connections from .gfa file
+    with open(assembly_graph_file) as file:
+        for line in file.readlines():
+            line = line.strip()
+
+            # Count the number of contigs
+            if line.startswith("S"):
+                strings = line.split("\t")
+                my_node = strings[1]
+                my_map[node_count] = my_node
+                nodes.append(my_node)
+                node_count += 1
+
+            # Identify lines with link information
+            elif line.startswith("L"):
+                link = []
                 strings = line.split("\t")
 
                 if strings[1] != strings[3]:
                     start = strings[1]
                     end = strings[3]
                     link.append(start)
                     link.append(end)
```

### Comparing `metacoag-1.1.4/metacoag_utils/label_prop_utils.py` & `metacoag-1.2.0/src/metacoag/metacoag_utils/label_prop_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #!/usr/bin/env python3
 
 import heapq
 import logging
 import math
 import sys
 
-from metacoag_utils import matching_utils
+from metacoag.metacoag_utils import matching_utils
 
 MAX_WEIGHT = sys.float_info.max
 
 # create logger
-logger = logging.getLogger("MetaCoaAG 1.1.4")
+logger = logging.getLogger("MetaCoaAG 1.2.0")
 
 
 class DataWrap:
     def __init__(self, data):
         self.data = data
 
     def __lt__(self, other):
```

### Comparing `metacoag-1.1.4/metacoag_utils/marker_gene_utils.py` & `metacoag-1.2.0/src/metacoag/metacoag_utils/marker_gene_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 
 import logging
 import os
 import pathlib
 
 # create logger
-logger = logging.getLogger("MetaCoaAG 1.1.4")
+logger = logging.getLogger("MetaCoaAG 1.2.0")
 
 
 # Modified from SolidBin
 def scan_for_marker_genes(contigs_file, nthreads, markerURL, no_cut_tc, hard=0):
 
     fragScanURL = "run_FragGeneScan.pl"
     hmmExeURL = "hmmsearch"
```

### Comparing `metacoag-1.1.4/metacoag_utils/matching_utils.py` & `metacoag-1.2.0/src/metacoag/metacoag_utils/matching_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Constants set from MaxBin 2.0
 MU_INTRA, SIGMA_INTRA = 0, 0.01037897 / 2
 MU_INTER, SIGMA_INTER = 0.0676654, 0.03419337
 VERY_SMALL_DOUBLE = 1e-10
 MAX_WEIGHT = sys.float_info.max
 
 # create logger
-logger = logging.getLogger("MetaCoaAG 1.1.4")
+logger = logging.getLogger("MetaCoaAG 1.2.0")
 
 
 def normpdf(x, mean, sd):
     var = float(sd) ** 2
     denom = sd * (2 * math.pi) ** 0.5
     num = math.exp(-((float(x) - float(mean)) ** 2) / (2 * var))
     return num / denom
```

### Comparing `metacoag-1.1.4/metacoag_utils/support/combine_cov.py` & `metacoag-1.2.0/src/metacoag/metacoag_utils/support/combine_cov.py`

 * *Files identical despite different names*

