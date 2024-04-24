# Comparing `tmp/pyhgvsv-0.1.tar.gz` & `tmp/pyhgvsv-0.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhgvsv-0.1.tar", last modified: Wed Apr 24 15:25:43 2024, max compression
+gzip compressed data, was "pyhgvsv-0.1.post1.tar", last modified: Wed Apr 24 15:49:39 2024, max compression
```

## Comparing `pyhgvsv-0.1.tar` & `pyhgvsv-0.1.post1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 i9a5000   (1000) i9a5000   (1000)        0 2024-04-24 15:25:43.569952 pyhgvsv-0.1/
--rw-rw-r--   0 i9a5000   (1000) i9a5000   (1000)     1100 2024-04-24 14:01:21.000000 pyhgvsv-0.1/LICENSE
--rw-r--r--   0 i9a5000   (1000) i9a5000   (1000)     8640 2024-04-24 15:25:43.569952 pyhgvsv-0.1/PKG-INFO
--rw-rw-r--   0 i9a5000   (1000) i9a5000   (1000)     8162 2024-04-24 14:18:23.000000 pyhgvsv-0.1/README.md
--rw-rw-r--   0 i9a5000   (1000) i9a5000   (1000)      580 2024-04-24 14:36:23.000000 pyhgvsv-0.1/pyproject.toml
--rw-rw-r--   0 i9a5000   (1000) i9a5000   (1000)       38 2024-04-24 15:25:43.569952 pyhgvsv-0.1/setup.cfg
-drwxrwxr-x   0 i9a5000   (1000) i9a5000   (1000)        0 2024-04-24 15:25:43.565951 pyhgvsv-0.1/src/
-drwxrwxr-x   0 i9a5000   (1000) i9a5000   (1000)        0 2024-04-24 15:25:43.569952 pyhgvsv-0.1/src/pyhgvsv/
--rw-rw-r--   0 i9a5000   (1000) i9a5000   (1000)    50833 2024-04-24 15:15:07.000000 pyhgvsv-0.1/src/pyhgvsv/__init__.py
--rw-rw-r--   0 i9a5000   (1000) i9a5000   (1000)     4354 2024-04-24 14:01:21.000000 pyhgvsv-0.1/src/pyhgvsv/models.py
--rw-rw-r--   0 i9a5000   (1000) i9a5000   (1000)     3970 2024-04-24 14:01:21.000000 pyhgvsv-0.1/src/pyhgvsv/utils.py
--rw-rw-r--   0 i9a5000   (1000) i9a5000   (1000)    11661 2024-04-24 14:01:21.000000 pyhgvsv-0.1/src/pyhgvsv/variants.py
-drwxrwxr-x   0 i9a5000   (1000) i9a5000   (1000)        0 2024-04-24 15:25:43.569952 pyhgvsv-0.1/src/pyhgvsv.egg-info/
--rw-r--r--   0 i9a5000   (1000) i9a5000   (1000)     8640 2024-04-24 15:25:43.000000 pyhgvsv-0.1/src/pyhgvsv.egg-info/PKG-INFO
--rw-rw-r--   0 i9a5000   (1000) i9a5000   (1000)      263 2024-04-24 15:25:43.000000 pyhgvsv-0.1/src/pyhgvsv.egg-info/SOURCES.txt
--rw-rw-r--   0 i9a5000   (1000) i9a5000   (1000)        1 2024-04-24 15:25:43.000000 pyhgvsv-0.1/src/pyhgvsv.egg-info/dependency_links.txt
--rw-rw-r--   0 i9a5000   (1000) i9a5000   (1000)        8 2024-04-24 15:25:43.000000 pyhgvsv-0.1/src/pyhgvsv.egg-info/top_level.txt
+drwxrwxr-x   0 i9a5000   (1000) i9a5000   (1000)        0 2024-04-24 15:49:39.629853 pyhgvsv-0.1.post1/
+-rw-rw-r--   0 i9a5000   (1000) i9a5000   (1000)     1100 2024-04-24 14:01:21.000000 pyhgvsv-0.1.post1/LICENSE
+-rw-r--r--   0 i9a5000   (1000) i9a5000   (1000)     8864 2024-04-24 15:49:39.629853 pyhgvsv-0.1.post1/PKG-INFO
+-rw-rw-r--   0 i9a5000   (1000) i9a5000   (1000)     8380 2024-04-24 15:43:44.000000 pyhgvsv-0.1.post1/README.md
+-rw-rw-r--   0 i9a5000   (1000) i9a5000   (1000)      586 2024-04-24 15:48:18.000000 pyhgvsv-0.1.post1/pyproject.toml
+-rw-rw-r--   0 i9a5000   (1000) i9a5000   (1000)       38 2024-04-24 15:49:39.629853 pyhgvsv-0.1.post1/setup.cfg
+drwxrwxr-x   0 i9a5000   (1000) i9a5000   (1000)        0 2024-04-24 15:49:39.621853 pyhgvsv-0.1.post1/src/
+drwxrwxr-x   0 i9a5000   (1000) i9a5000   (1000)        0 2024-04-24 15:49:39.629853 pyhgvsv-0.1.post1/src/pyhgvsv/
+-rw-rw-r--   0 i9a5000   (1000) i9a5000   (1000)    50833 2024-04-24 15:15:07.000000 pyhgvsv-0.1.post1/src/pyhgvsv/__init__.py
+-rw-rw-r--   0 i9a5000   (1000) i9a5000   (1000)     4354 2024-04-24 14:01:21.000000 pyhgvsv-0.1.post1/src/pyhgvsv/models.py
+-rw-rw-r--   0 i9a5000   (1000) i9a5000   (1000)     3970 2024-04-24 14:01:21.000000 pyhgvsv-0.1.post1/src/pyhgvsv/utils.py
+-rw-rw-r--   0 i9a5000   (1000) i9a5000   (1000)    11661 2024-04-24 14:01:21.000000 pyhgvsv-0.1.post1/src/pyhgvsv/variants.py
+drwxrwxr-x   0 i9a5000   (1000) i9a5000   (1000)        0 2024-04-24 15:49:39.629853 pyhgvsv-0.1.post1/src/pyhgvsv.egg-info/
+-rw-r--r--   0 i9a5000   (1000) i9a5000   (1000)     8864 2024-04-24 15:49:39.000000 pyhgvsv-0.1.post1/src/pyhgvsv.egg-info/PKG-INFO
+-rw-rw-r--   0 i9a5000   (1000) i9a5000   (1000)      263 2024-04-24 15:49:39.000000 pyhgvsv-0.1.post1/src/pyhgvsv.egg-info/SOURCES.txt
+-rw-rw-r--   0 i9a5000   (1000) i9a5000   (1000)        1 2024-04-24 15:49:39.000000 pyhgvsv-0.1.post1/src/pyhgvsv.egg-info/dependency_links.txt
+-rw-rw-r--   0 i9a5000   (1000) i9a5000   (1000)        8 2024-04-24 15:49:39.000000 pyhgvsv-0.1.post1/src/pyhgvsv.egg-info/top_level.txt
```

### Comparing `pyhgvsv-0.1/LICENSE` & `pyhgvsv-0.1.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhgvsv-0.1/PKG-INFO` & `pyhgvsv-0.1.post1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhgvsv
-Version: 0.1
+Version: 0.1.post1
 Summary: HGVS variant name parsing and generation with SV (structural variant) support
 Author-email: Parker Payne <parker.payne@bcm.edu>
 Project-URL: Homepage, https://github.com/parkerpayne/hgvsv
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=2.6
@@ -136,22 +136,22 @@
     chrom, offset, ref, alt, genome, transcript)
 # Returns 'NM_000352.3(ABCC8):c.215A>G'
 
 # Format an HGVS name for a structural variant (deletion).
 chrom, offset, ref, alt, sv_length = ('chrY', 24861625, '', '', -4780)
 transcript = get_transcript('NM_001388484.1')
 hgvs_name = hgvsv.format_hgvs_name(
-    chrom, offset, ref, alt, genome, transcript)
+    chrom, offset, ref, alt, genome, transcript, sv_length)
 # Returns 'NM_001388484.1(DAZ4):c.1210-436_1354-437del4780'
 
 # Format an HGVS name for a structural variant (insertion).
 chrom, offset, ref, alt, sv_length = ('chr17', 8141778, '', 'TTCTCCCCCCTTGAACTTGAGCTCAATTC', 29)
 transcript = get_transcript('NM_002616.3')
 hgvs_name = hgvsv.format_hgvs_name(
-    chrom, offset, ref, alt, genome, transcript)
+    chrom, offset, ref, alt, genome, transcript, sv_length)
 # Returns 'NM_002616.3(PER1):c.3600+26_3600+27ins29'
 ```
 
 The `hgvsv` library can also perform just the parsing step and provide
 a parse tree of the HGVS name.
 
 ```python
@@ -168,15 +168,21 @@
 # hgvs_name.cdna_end = hgvs.CDNACoord(215, -10)
 # hgvs_name.ref_allele = 'A'
 # hgvs_name.alt_allele = 'G'
 ```
 
 ## Install
 
-This library can be installed using the `setup.py` file as follows:
+`hgvsv` can be installed via pip:
+
+```sh
+pip install pyhgvsv
+```
+
+Or the library can be installed using the `setup.py` file as follows:
 
 ```sh
 python setup.py install
 ```
 
 ## Tests
 
@@ -187,11 +193,13 @@
 ```
 
 ## Requirements
 
 This library requires at least Python 2.6, but otherwise has no
 external dependencies.
 
+The library's use often requires refSeq data, which can be found at [genome.ucsc.edu](http://genome.ucsc.edu/cgi-bin/hgTables)
+
 The library does assume that genome sequence is available through a `pyfaidx`
 compatible `Fasta` object. For an example of writing a wrapper for
 a different genome sequence back-end, see
 [hgvs.tests.genome.MockGenome](pyhgvs/tests/genome.py).
```

### Comparing `pyhgvsv-0.1/README.md` & `pyhgvsv-0.1.post1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -123,22 +123,22 @@
     chrom, offset, ref, alt, genome, transcript)
 # Returns 'NM_000352.3(ABCC8):c.215A>G'
 
 # Format an HGVS name for a structural variant (deletion).
 chrom, offset, ref, alt, sv_length = ('chrY', 24861625, '', '', -4780)
 transcript = get_transcript('NM_001388484.1')
 hgvs_name = hgvsv.format_hgvs_name(
-    chrom, offset, ref, alt, genome, transcript)
+    chrom, offset, ref, alt, genome, transcript, sv_length)
 # Returns 'NM_001388484.1(DAZ4):c.1210-436_1354-437del4780'
 
 # Format an HGVS name for a structural variant (insertion).
 chrom, offset, ref, alt, sv_length = ('chr17', 8141778, '', 'TTCTCCCCCCTTGAACTTGAGCTCAATTC', 29)
 transcript = get_transcript('NM_002616.3')
 hgvs_name = hgvsv.format_hgvs_name(
-    chrom, offset, ref, alt, genome, transcript)
+    chrom, offset, ref, alt, genome, transcript, sv_length)
 # Returns 'NM_002616.3(PER1):c.3600+26_3600+27ins29'
 ```
 
 The `hgvsv` library can also perform just the parsing step and provide
 a parse tree of the HGVS name.
 
 ```python
@@ -155,15 +155,21 @@
 # hgvs_name.cdna_end = hgvs.CDNACoord(215, -10)
 # hgvs_name.ref_allele = 'A'
 # hgvs_name.alt_allele = 'G'
 ```
 
 ## Install
 
-This library can be installed using the `setup.py` file as follows:
+`hgvsv` can be installed via pip:
+
+```sh
+pip install pyhgvsv
+```
+
+Or the library can be installed using the `setup.py` file as follows:
 
 ```sh
 python setup.py install
 ```
 
 ## Tests
 
@@ -174,11 +180,13 @@
 ```
 
 ## Requirements
 
 This library requires at least Python 2.6, but otherwise has no
 external dependencies.
 
+The library's use often requires refSeq data, which can be found at [genome.ucsc.edu](http://genome.ucsc.edu/cgi-bin/hgTables)
+
 The library does assume that genome sequence is available through a `pyfaidx`
 compatible `Fasta` object. For an example of writing a wrapper for
 a different genome sequence back-end, see
 [hgvs.tests.genome.MockGenome](pyhgvs/tests/genome.py).
```

### Comparing `pyhgvsv-0.1/pyproject.toml` & `pyhgvsv-0.1.post1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyhgvsv"
-version = "0.1"
+version = "0.1.post1"
 authors = [
   { name="Parker Payne", email="parker.payne@bcm.edu" },
 ]
 description = "HGVS variant name parsing and generation with SV (structural variant) support"
 readme = "README.md"
 requires-python = ">=2.6"
 classifiers = [
```

### Comparing `pyhgvsv-0.1/src/pyhgvsv/__init__.py` & `pyhgvsv-0.1.post1/src/pyhgvsv/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhgvsv-0.1/src/pyhgvsv/models.py` & `pyhgvsv-0.1.post1/src/pyhgvsv/models.py`

 * *Files identical despite different names*

### Comparing `pyhgvsv-0.1/src/pyhgvsv/utils.py` & `pyhgvsv-0.1.post1/src/pyhgvsv/utils.py`

 * *Files identical despite different names*

### Comparing `pyhgvsv-0.1/src/pyhgvsv/variants.py` & `pyhgvsv-0.1.post1/src/pyhgvsv/variants.py`

 * *Files identical despite different names*

### Comparing `pyhgvsv-0.1/src/pyhgvsv.egg-info/PKG-INFO` & `pyhgvsv-0.1.post1/src/pyhgvsv.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhgvsv
-Version: 0.1
+Version: 0.1.post1
 Summary: HGVS variant name parsing and generation with SV (structural variant) support
 Author-email: Parker Payne <parker.payne@bcm.edu>
 Project-URL: Homepage, https://github.com/parkerpayne/hgvsv
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=2.6
@@ -136,22 +136,22 @@
     chrom, offset, ref, alt, genome, transcript)
 # Returns 'NM_000352.3(ABCC8):c.215A>G'
 
 # Format an HGVS name for a structural variant (deletion).
 chrom, offset, ref, alt, sv_length = ('chrY', 24861625, '', '', -4780)
 transcript = get_transcript('NM_001388484.1')
 hgvs_name = hgvsv.format_hgvs_name(
-    chrom, offset, ref, alt, genome, transcript)
+    chrom, offset, ref, alt, genome, transcript, sv_length)
 # Returns 'NM_001388484.1(DAZ4):c.1210-436_1354-437del4780'
 
 # Format an HGVS name for a structural variant (insertion).
 chrom, offset, ref, alt, sv_length = ('chr17', 8141778, '', 'TTCTCCCCCCTTGAACTTGAGCTCAATTC', 29)
 transcript = get_transcript('NM_002616.3')
 hgvs_name = hgvsv.format_hgvs_name(
-    chrom, offset, ref, alt, genome, transcript)
+    chrom, offset, ref, alt, genome, transcript, sv_length)
 # Returns 'NM_002616.3(PER1):c.3600+26_3600+27ins29'
 ```
 
 The `hgvsv` library can also perform just the parsing step and provide
 a parse tree of the HGVS name.
 
 ```python
@@ -168,15 +168,21 @@
 # hgvs_name.cdna_end = hgvs.CDNACoord(215, -10)
 # hgvs_name.ref_allele = 'A'
 # hgvs_name.alt_allele = 'G'
 ```
 
 ## Install
 
-This library can be installed using the `setup.py` file as follows:
+`hgvsv` can be installed via pip:
+
+```sh
+pip install pyhgvsv
+```
+
+Or the library can be installed using the `setup.py` file as follows:
 
 ```sh
 python setup.py install
 ```
 
 ## Tests
 
@@ -187,11 +193,13 @@
 ```
 
 ## Requirements
 
 This library requires at least Python 2.6, but otherwise has no
 external dependencies.
 
+The library's use often requires refSeq data, which can be found at [genome.ucsc.edu](http://genome.ucsc.edu/cgi-bin/hgTables)
+
 The library does assume that genome sequence is available through a `pyfaidx`
 compatible `Fasta` object. For an example of writing a wrapper for
 a different genome sequence back-end, see
 [hgvs.tests.genome.MockGenome](pyhgvs/tests/genome.py).
```

