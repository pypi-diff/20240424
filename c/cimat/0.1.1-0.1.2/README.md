# Comparing `tmp/cimat-0.1.1.tar.gz` & `tmp/cimat-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cimat-0.1.1.tar", max compression
+gzip compressed data, was "cimat-0.1.2.tar", max compression
```

## Comparing `cimat-0.1.1.tar` & `cimat-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    10142 2024-04-19 23:11:01.812000 cimat-0.1.1/LICENSE
--rw-r--r--   0        0        0       89 2024-04-19 23:11:01.823000 cimat-0.1.1/NOTICE
--rw-r--r--   0        0        0     4191 2024-04-23 18:51:31.064000 cimat-0.1.1/README.md
--rw-r--r--   0        0        0       84 2024-04-23 18:42:53.305000 cimat-0.1.1/cimat/__init__.py
--rw-r--r--   0        0        0     1440 2024-04-23 18:42:53.324000 cimat-0.1.1/cimat/mtdata.py
--rw-r--r--   0        0        0     9930 2024-04-23 18:42:53.342000 cimat-0.1.1/cimat/uncertainty_estimator.py
--rw-r--r--   0        0        0      403 2024-04-23 20:34:48.650000 cimat-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4736 1970-01-01 00:00:00.000000 cimat-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    10142 2024-04-19 23:11:01.812000 cimat-0.1.2/LICENSE
+-rw-r--r--   0        0        0       89 2024-04-19 23:11:01.823000 cimat-0.1.2/NOTICE
+-rw-r--r--   0        0        0     4191 2024-04-23 18:51:31.064000 cimat-0.1.2/README.md
+-rw-r--r--   0        0        0       84 2024-04-23 18:42:53.305000 cimat-0.1.2/cimat/__init__.py
+-rw-r--r--   0        0        0     1440 2024-04-23 18:42:53.324000 cimat-0.1.2/cimat/mtdata.py
+-rw-r--r--   0        0        0     9930 2024-04-23 18:42:53.342000 cimat-0.1.2/cimat/uncertainty_estimator.py
+-rw-r--r--   0        0        0      402 2024-04-24 01:13:16.129000 cimat-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4836 1970-01-01 00:00:00.000000 cimat-0.1.2/PKG-INFO
```

### Comparing `cimat-0.1.1/LICENSE` & `cimat-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cimat-0.1.1/README.md` & `cimat-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `cimat-0.1.1/cimat/mtdata.py` & `cimat-0.1.2/cimat/mtdata.py`

 * *Files identical despite different names*

### Comparing `cimat-0.1.1/cimat/uncertainty_estimator.py` & `cimat-0.1.2/cimat/uncertainty_estimator.py`

 * *Files identical despite different names*

### Comparing `cimat-0.1.1/PKG-INFO` & `cimat-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: cimat
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package for uncertainty quantification of error rates in 1:1 matching tasks.
 Author: Riccardo Fogliato
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: numpy (>=1.25.2,<2.0.0)
 Requires-Dist: scikit-learn (>=1.4.2,<2.0.0)
 Requires-Dist: scipy (>=1.13.0,<2.0.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
-Metadata-Version: 2.1 Name: cimat Version: 0.1.1 Summary: A package for
+Metadata-Version: 2.1 Name: cimat Version: 0.1.2 Summary: A package for
 uncertainty quantification of error rates in 1:1 matching tasks. Author:
-Riccardo Fogliato Requires-Python: >=3.11,<4.0 Classifier: Programming Language
-:: Python :: 3 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3.12 Requires-Dist: numpy (>=1.25.2,<2.0.0)
-Requires-Dist: scikit-learn (>=1.4.2,<2.0.0) Requires-Dist: scipy
-(>=1.13.0,<2.0.0) Requires-Dist: tqdm (>=4.66.2,<5.0.0) Description-Content-
-Type: text/markdown
+Riccardo Fogliato Requires-Python: >=3.9,<4.0 Classifier: Programming Language
+:: Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
+Dist: numpy (>=1.25.2,<2.0.0) Requires-Dist: scikit-learn (>=1.4.2,<2.0.0)
+Requires-Dist: scipy (>=1.13.0,<2.0.0) Requires-Dist: tqdm (>=4.66.2,<5.0.0)
+Description-Content-Type: text/markdown
  ************ CCoonnffiiddeennccee IInntteerrvvaallss ffoorr EErrrroorr RRaatteess iinn ::jjiiggssaaww:: MMaattcchhiinngg TTaasskkss ************
                               _[_P_a_p_e_r_][Apache-2.0]
 This repository hosts the cimat (Confidence Intervals for MAtching Tasks)
 package, designed to create confidence intervals for performance metrics in 1:
 1 matching tasks like face and speaker verification. With cimat, you can
 generate confidence intervals ($C_{\alpha}$) with a confidence level of $1-
 \alpha$ for metrics ($\theta^*$) such as: - False Positive Rate (FPR, aka FMR
```

