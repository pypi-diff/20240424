# Comparing `tmp/lingualigner-0.8.tar.gz` & `tmp/lingualigner-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lingualigner-0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lingualigner-0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lingualigner-0.8.tar` & `lingualigner-0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       27 2024-04-13 00:41:40.164099 lingualigner-0.8/.gitignore
--rw-r--r--   0        0        0     1091 2024-04-12 15:55:09.589586 lingualigner-0.8/LICENSE
--rw-r--r--   0        0        0     2507 2024-04-13 00:44:21.306976 lingualigner-0.8/LinguAligner/__init__.py
--rw-r--r--   0        0        0     6324 2024-04-13 00:17:53.246358 lingualigner-0.8/LinguAligner/aligners.py
--rw-r--r--   0        0        0     1359 2024-04-12 19:03:23.712783 lingualigner-0.8/LinguAligner/multiple_translations.py
--rw-r--r--   0        0        0     4529 2024-04-12 18:55:33.013673 lingualigner-0.8/LinguAligner/translation.py
--rw-r--r--   0        0        0     2398 2023-07-05 13:10:41.000000 lingualigner-0.8/LinguAligner/utils.py
--rw-r--r--   0        0        0     4950 2024-04-13 00:44:12.394497 lingualigner-0.8/README.md
--rw-r--r--   0        0        0   101207 2024-02-08 00:36:31.515866 lingualigner-0.8/img/eval_EE.png
--rw-r--r--   0        0        0    88477 2024-02-08 00:35:58.477683 lingualigner-0.8/img/eval_by_comp.png
--rw-r--r--   0        0        0      454 2024-04-13 00:39:51.431876 lingualigner-0.8/pyproject.toml
--rw-r--r--   0        0        0      133 2024-04-12 13:43:59.759184 lingualigner-0.8/resources/resource.json
--rw-r--r--   0        0        0     4782 2024-04-13 00:29:23.803830 lingualigner-0.8/teste.ipynb
--rw-r--r--   0        0        0     5432 1970-01-01 00:00:00.000000 lingualigner-0.8/PKG-INFO
+-rw-r--r--   0        0        0       27 2024-04-13 00:41:40.164099 lingualigner-0.9/.gitignore
+-rw-r--r--   0        0        0     1091 2024-04-12 15:55:09.589586 lingualigner-0.9/LICENSE
+-rw-r--r--   0        0        0     2507 2024-04-13 00:45:44.613283 lingualigner-0.9/LinguAligner/__init__.py
+-rw-r--r--   0        0        0     6324 2024-04-13 00:17:53.246358 lingualigner-0.9/LinguAligner/aligners.py
+-rw-r--r--   0        0        0     1359 2024-04-12 19:03:23.712783 lingualigner-0.9/LinguAligner/multiple_translations.py
+-rw-r--r--   0        0        0     4529 2024-04-12 18:55:33.013673 lingualigner-0.9/LinguAligner/translation.py
+-rw-r--r--   0        0        0     2398 2023-07-05 13:10:41.000000 lingualigner-0.9/LinguAligner/utils.py
+-rw-r--r--   0        0        0     4959 2024-04-13 00:45:38.314507 lingualigner-0.9/README.md
+-rw-r--r--   0        0        0   101207 2024-02-08 00:36:31.515866 lingualigner-0.9/img/eval_EE.png
+-rw-r--r--   0        0        0    88477 2024-02-08 00:35:58.477683 lingualigner-0.9/img/eval_by_comp.png
+-rw-r--r--   0        0        0      454 2024-04-13 00:39:51.431876 lingualigner-0.9/pyproject.toml
+-rw-r--r--   0        0        0      133 2024-04-12 13:43:59.759184 lingualigner-0.9/resources/resource.json
+-rw-r--r--   0        0        0     4782 2024-04-13 00:29:23.803830 lingualigner-0.9/teste.ipynb
+-rw-r--r--   0        0        0     5441 1970-01-01 00:00:00.000000 lingualigner-0.9/PKG-INFO
```

### Comparing `lingualigner-0.8/LICENSE` & `lingualigner-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lingualigner-0.8/LinguAligner/__init__.py` & `lingualigner-0.9/LinguAligner/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """LinguAligner is a Python library for aligning annotations in parallel corpora. It is designed to be used in the context of parallel corpora annotation alignment, where the goal is to align annotations in the source language with annotations in the target language. """
-__version__ = "0.8"
+__version__ = "0.9"
 
 
 from . import aligners
 import spacy
 from . import translation
 from transformers import BertTokenizer, BertModel, logging
 logging.set_verbosity_error()
```

### Comparing `lingualigner-0.8/LinguAligner/aligners.py` & `lingualigner-0.9/LinguAligner/aligners.py`

 * *Files identical despite different names*

### Comparing `lingualigner-0.8/LinguAligner/multiple_translations.py` & `lingualigner-0.9/LinguAligner/multiple_translations.py`

 * *Files identical despite different names*

### Comparing `lingualigner-0.8/LinguAligner/translation.py` & `lingualigner-0.9/LinguAligner/translation.py`

 * *Files identical despite different names*

### Comparing `lingualigner-0.8/LinguAligner/utils.py` & `lingualigner-0.9/LinguAligner/utils.py`

 * *Files identical despite different names*

### Comparing `lingualigner-0.8/README.md` & `lingualigner-0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
 ## Evaluation
 To measure the effectiveness of the alignment pipeline we tested it on ACE-2005 corpus. Manual alignments were conducted on the entire ACE-2005-PT test set, which includes 1,310 annotations. These alignments were performed by a linguist expert to ensure high-quality annotations, following the same annotation [guidelines](https://www.ldc.upenn.edu/sites/www.ldc.upenn.edu/files/english-events-guidelines-v5.4.3.pdf) of the original ACE-2005 corpus.
 
 The evaluation results are presented in Table 1:
 
 <p>
-    <img src="https://github.com/lfcc1/LinguAligner/blob/main/img/eval_by_comp.png" alt="Results" width="500"/>
+    <img src="https://github.com/lfcc1/LinguAligner/blob/main/img/eval_by_comp.png?raw=true" alt="Results" width="500"/>
     <br>
     <em>Table 1: Evaluation Results by pipeline component</em>
 </p>
 
 
 
 ## License
```

### Comparing `lingualigner-0.8/img/eval_EE.png` & `lingualigner-0.9/img/eval_EE.png`

 * *Files identical despite different names*

### Comparing `lingualigner-0.8/img/eval_by_comp.png` & `lingualigner-0.9/img/eval_by_comp.png`

 * *Files identical despite different names*

### Comparing `lingualigner-0.8/teste.ipynb` & `lingualigner-0.9/teste.ipynb`

 * *Files identical despite different names*

### Comparing `lingualigner-0.8/PKG-INFO` & `lingualigner-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LinguAligner
-Version: 0.8
+Version: 0.9
 Summary: LinguAligner is a Python library for aligning annotations in parallel corpora. It is designed to be used in the context of parallel corpora annotation alignment, where the goal is to align annotations in the source language with annotations in the target language. 
 Author-email: lfc <lfc@di.uminho.pt>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Homepage, https://github.com/lfcc1/LinguAligner
 Project-URL: Issues, https://github.com/lfcc1/LinguAligner/issues
 
@@ -92,15 +92,15 @@
 
 ## Evaluation
 To measure the effectiveness of the alignment pipeline we tested it on ACE-2005 corpus. Manual alignments were conducted on the entire ACE-2005-PT test set, which includes 1,310 annotations. These alignments were performed by a linguist expert to ensure high-quality annotations, following the same annotation [guidelines](https://www.ldc.upenn.edu/sites/www.ldc.upenn.edu/files/english-events-guidelines-v5.4.3.pdf) of the original ACE-2005 corpus.
 
 The evaluation results are presented in Table 1:
 
 <p>
-    <img src="https://github.com/lfcc1/LinguAligner/blob/main/img/eval_by_comp.png" alt="Results" width="500"/>
+    <img src="https://github.com/lfcc1/LinguAligner/blob/main/img/eval_by_comp.png?raw=true" alt="Results" width="500"/>
     <br>
     <em>Table 1: Evaluation Results by pipeline component</em>
 </p>
 
 
 
 ## License
```

