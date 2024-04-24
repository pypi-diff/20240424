# Comparing `tmp/cimat-0.1.0.tar.gz` & `tmp/cimat-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cimat-0.1.0.tar", max compression
+gzip compressed data, was "cimat-0.1.1.tar", max compression
```

## Comparing `cimat-0.1.0.tar` & `cimat-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    10142 2024-04-19 23:11:01.812000 cimat-0.1.0/LICENSE
--rw-r--r--   0        0        0       89 2024-04-19 23:11:01.823000 cimat-0.1.0/NOTICE
--rw-r--r--   0        0        0     4200 2024-04-23 18:49:28.571000 cimat-0.1.0/README.md
--rw-r--r--   0        0        0       84 2024-04-23 18:42:53.305000 cimat-0.1.0/cimat/__init__.py
--rw-r--r--   0        0        0     1440 2024-04-23 18:42:53.324000 cimat-0.1.0/cimat/mtdata.py
--rw-r--r--   0        0        0     9930 2024-04-23 18:42:53.342000 cimat-0.1.0/cimat/uncertainty_estimator.py
--rw-r--r--   0        0        0      403 2024-04-23 18:49:05.868000 cimat-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4745 1970-01-01 00:00:00.000000 cimat-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    10142 2024-04-19 23:11:01.812000 cimat-0.1.1/LICENSE
+-rw-r--r--   0        0        0       89 2024-04-19 23:11:01.823000 cimat-0.1.1/NOTICE
+-rw-r--r--   0        0        0     4191 2024-04-23 18:51:31.064000 cimat-0.1.1/README.md
+-rw-r--r--   0        0        0       84 2024-04-23 18:42:53.305000 cimat-0.1.1/cimat/__init__.py
+-rw-r--r--   0        0        0     1440 2024-04-23 18:42:53.324000 cimat-0.1.1/cimat/mtdata.py
+-rw-r--r--   0        0        0     9930 2024-04-23 18:42:53.342000 cimat-0.1.1/cimat/uncertainty_estimator.py
+-rw-r--r--   0        0        0      403 2024-04-23 20:34:48.650000 cimat-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4736 1970-01-01 00:00:00.000000 cimat-0.1.1/PKG-INFO
```

### Comparing `cimat-0.1.0/LICENSE` & `cimat-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cimat-0.1.0/README.md` & `cimat-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -18,18 +18,18 @@
 
 such that $\mathbb{P}(\theta^*\in C_{\alpha})\geq 1-\alpha$. Check out [our
 paper](https://arxiv.org/abs/2306.01198) for a description of the methods.
 
 ## :rocket: Getting started
 
 In order to intall the cimat package, run 
-<!-- ```
+```
 pip install cimat
 ```
-or  -->
+or 
 ```
 pip install git+https://github.com/awslabs/cis-matching-tasks.git
 ```
 for the latest version of the package. 
 
 Test your setup using this example that derives confidence intervals for FNMR
 and FMR obtained by binarizing the similarity scores at a given threshold:
```

#### html2text {}

```diff
@@ -5,20 +5,20 @@
 1 matching tasks like face and speaker verification. With cimat, you can
 generate confidence intervals ($C_{\alpha}$) with a confidence level of $1-
 \alpha$ for metrics ($\theta^*$) such as: - False Positive Rate (FPR, aka FMR
 or FAR) and False Negative Rate (FNR, aka FNMR or FRR) estimates - ROC
 coordinate estimates such as FNR@FPR (aka FNMR@FMR or FRR@FAR) such that
 $\mathbb{P}(\theta^*\in C_{\alpha})\geq 1-\alpha$. Check out [our paper](https:
 //arxiv.org/abs/2306.01198) for a description of the methods. ## :rocket:
-Getting started In order to intall the cimat package, run ``` pip install
-git+https://github.com/awslabs/cis-matching-tasks.git ``` for the latest
-version of the package. Test your setup using this example that derives
-confidence intervals for FNMR and FMR obtained by binarizing the similarity
-scores at a given threshold: ``` import json from cimat import MTData,
-UncertaintyEstimator # Load embeddings from JSON file into a dictionary
+Getting started In order to intall the cimat package, run ``` pip install cimat
+``` or ``` pip install git+https://github.com/awslabs/cis-matching-tasks.git
+``` for the latest version of the package. Test your setup using this example
+that derives confidence intervals for FNMR and FMR obtained by binarizing the
+similarity scores at a given threshold: ``` import json from cimat import
+MTData, UncertaintyEstimator # Load embeddings from JSON file into a dictionary
 structure df = json.load(open('data/embeddings.json', 'r')) # Example
 structure: dictionary[id][image] = embedding mt = MTData(df)
 mt.generate_similarity_scores() # Generate cosine similarity scores between
 images # Set a threshold for determining matches versus non-matches threshold =
 0.9 # Instantiate the class to estimate error rates using similarity scores #
 Example structure: dictionary[id1][id2] = [score between image from id1 and
 id2] uq = UncertaintyEstimator(scores=mt.similarity_scores) # Compute False
```

### Comparing `cimat-0.1.0/cimat/mtdata.py` & `cimat-0.1.1/cimat/mtdata.py`

 * *Files identical despite different names*

### Comparing `cimat-0.1.0/cimat/uncertainty_estimator.py` & `cimat-0.1.1/cimat/uncertainty_estimator.py`

 * *Files identical despite different names*

### Comparing `cimat-0.1.0/PKG-INFO` & `cimat-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cimat
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for uncertainty quantification of error rates in 1:1 matching tasks.
 Author: Riccardo Fogliato
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: numpy (>=1.25.2,<2.0.0)
@@ -33,18 +33,18 @@
 
 such that $\mathbb{P}(\theta^*\in C_{\alpha})\geq 1-\alpha$. Check out [our
 paper](https://arxiv.org/abs/2306.01198) for a description of the methods.
 
 ## :rocket: Getting started
 
 In order to intall the cimat package, run 
-<!-- ```
+```
 pip install cimat
 ```
-or  -->
+or 
 ```
 pip install git+https://github.com/awslabs/cis-matching-tasks.git
 ```
 for the latest version of the package. 
 
 Test your setup using this example that derives confidence intervals for FNMR
 and FMR obtained by binarizing the similarity scores at a given threshold:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cimat Version: 0.1.0 Summary: A package for
+Metadata-Version: 2.1 Name: cimat Version: 0.1.1 Summary: A package for
 uncertainty quantification of error rates in 1:1 matching tasks. Author:
 Riccardo Fogliato Requires-Python: >=3.11,<4.0 Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: numpy (>=1.25.2,<2.0.0)
 Requires-Dist: scikit-learn (>=1.4.2,<2.0.0) Requires-Dist: scipy
 (>=1.13.0,<2.0.0) Requires-Dist: tqdm (>=4.66.2,<5.0.0) Description-Content-
 Type: text/markdown
@@ -13,20 +13,20 @@
 1 matching tasks like face and speaker verification. With cimat, you can
 generate confidence intervals ($C_{\alpha}$) with a confidence level of $1-
 \alpha$ for metrics ($\theta^*$) such as: - False Positive Rate (FPR, aka FMR
 or FAR) and False Negative Rate (FNR, aka FNMR or FRR) estimates - ROC
 coordinate estimates such as FNR@FPR (aka FNMR@FMR or FRR@FAR) such that
 $\mathbb{P}(\theta^*\in C_{\alpha})\geq 1-\alpha$. Check out [our paper](https:
 //arxiv.org/abs/2306.01198) for a description of the methods. ## :rocket:
-Getting started In order to intall the cimat package, run ``` pip install
-git+https://github.com/awslabs/cis-matching-tasks.git ``` for the latest
-version of the package. Test your setup using this example that derives
-confidence intervals for FNMR and FMR obtained by binarizing the similarity
-scores at a given threshold: ``` import json from cimat import MTData,
-UncertaintyEstimator # Load embeddings from JSON file into a dictionary
+Getting started In order to intall the cimat package, run ``` pip install cimat
+``` or ``` pip install git+https://github.com/awslabs/cis-matching-tasks.git
+``` for the latest version of the package. Test your setup using this example
+that derives confidence intervals for FNMR and FMR obtained by binarizing the
+similarity scores at a given threshold: ``` import json from cimat import
+MTData, UncertaintyEstimator # Load embeddings from JSON file into a dictionary
 structure df = json.load(open('data/embeddings.json', 'r')) # Example
 structure: dictionary[id][image] = embedding mt = MTData(df)
 mt.generate_similarity_scores() # Generate cosine similarity scores between
 images # Set a threshold for determining matches versus non-matches threshold =
 0.9 # Instantiate the class to estimate error rates using similarity scores #
 Example structure: dictionary[id1][id2] = [score between image from id1 and
 id2] uq = UncertaintyEstimator(scores=mt.similarity_scores) # Compute False
```

