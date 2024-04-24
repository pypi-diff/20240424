# Comparing `tmp/FuzzyTM-2.0.8.tar.gz` & `tmp/FuzzyTM-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FuzzyTM-2.0.8.tar", last modified: Tue Apr 23 23:02:26 2024, max compression
+gzip compressed data, was "FuzzyTM-2.0.9.tar", last modified: Wed Apr 24 20:40:36 2024, max compression
```

## Comparing `FuzzyTM-2.0.8.tar` & `FuzzyTM-2.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 23:02:26.405471 FuzzyTM-2.0.8/
-drwxrwxrwx   0        0        0        0 2024-04-23 23:02:26.385524 FuzzyTM-2.0.8/FuzzyTM/
--rw-rw-rw-   0        0        0    63028 2022-11-23 10:50:28.000000 FuzzyTM-2.0.8/FuzzyTM/FuzzyTM.py
--rw-rw-rw-   0        0        0      155 2022-10-19 17:02:01.000000 FuzzyTM-2.0.8/FuzzyTM/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 23:02:26.402479 FuzzyTM-2.0.8/FuzzyTM/analysis/
--rw-rw-rw-   0        0        0        0 2024-04-23 21:00:12.000000 FuzzyTM-2.0.8/FuzzyTM/analysis/__init__.py
--rw-rw-rw-   0        0        0     8194 2024-04-23 22:51:33.000000 FuzzyTM-2.0.8/FuzzyTM/analysis/topic_specificity.py
-drwxrwxrwx   0        0        0        0 2024-04-23 23:02:26.398491 FuzzyTM-2.0.8/FuzzyTM.egg-info/
--rw-rw-rw-   0        0        0     7858 2024-04-23 23:02:26.000000 FuzzyTM-2.0.8/FuzzyTM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      286 2024-04-23 23:02:26.000000 FuzzyTM-2.0.8/FuzzyTM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 23:02:26.000000 FuzzyTM-2.0.8/FuzzyTM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-04-23 23:02:26.000000 FuzzyTM-2.0.8/FuzzyTM.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-23 23:02:26.000000 FuzzyTM-2.0.8/FuzzyTM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    18431 2021-11-01 14:27:46.000000 FuzzyTM-2.0.8/LICENSE
--rw-rw-rw-   0        0        0     7858 2024-04-23 23:02:26.404477 FuzzyTM-2.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     7517 2024-04-22 21:30:36.000000 FuzzyTM-2.0.8/README.md
--rw-rw-rw-   0        0        0       42 2024-04-23 23:02:26.405471 FuzzyTM-2.0.8/setup.cfg
--rw-rw-rw-   0        0        0      924 2024-04-23 22:54:04.000000 FuzzyTM-2.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 20:40:36.237928 FuzzyTM-2.0.9/
+drwxrwxrwx   0        0        0        0 2024-04-24 20:40:36.184843 FuzzyTM-2.0.9/FuzzyTM/
+-rw-rw-rw-   0        0        0    63026 2024-04-24 20:33:34.000000 FuzzyTM-2.0.9/FuzzyTM/FuzzyTM.py
+-rw-rw-rw-   0        0        0      155 2022-10-19 17:02:01.000000 FuzzyTM-2.0.9/FuzzyTM/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 20:40:36.234913 FuzzyTM-2.0.9/FuzzyTM/analysis/
+-rw-rw-rw-   0        0        0        0 2024-04-23 21:00:12.000000 FuzzyTM-2.0.9/FuzzyTM/analysis/__init__.py
+-rw-rw-rw-   0        0        0     8194 2024-04-23 22:51:33.000000 FuzzyTM-2.0.9/FuzzyTM/analysis/topic_specificity.py
+drwxrwxrwx   0        0        0        0 2024-04-24 20:40:36.217666 FuzzyTM-2.0.9/FuzzyTM.egg-info/
+-rw-rw-rw-   0        0        0     7858 2024-04-24 20:40:35.000000 FuzzyTM-2.0.9/FuzzyTM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      286 2024-04-24 20:40:35.000000 FuzzyTM-2.0.9/FuzzyTM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 20:40:35.000000 FuzzyTM-2.0.9/FuzzyTM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-04-24 20:40:35.000000 FuzzyTM-2.0.9/FuzzyTM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-24 20:40:35.000000 FuzzyTM-2.0.9/FuzzyTM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    18431 2021-11-01 14:27:46.000000 FuzzyTM-2.0.9/LICENSE
+-rw-rw-rw-   0        0        0     7858 2024-04-24 20:40:36.236934 FuzzyTM-2.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     7517 2024-04-22 21:30:36.000000 FuzzyTM-2.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-24 20:40:36.237928 FuzzyTM-2.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      924 2024-04-24 20:40:07.000000 FuzzyTM-2.0.9/setup.py
```

### Comparing `FuzzyTM-2.0.8/FuzzyTM/FuzzyTM.py` & `FuzzyTM-2.0.9/FuzzyTM/FuzzyTM.py`

 * *Files 1% similar despite different names*

```diff
@@ -632,14 +632,15 @@
                 The output from self._create_prob_word_i().
 
         Returns
         -------
             numpy.array : float
                 (shape: 1 x number of topics)
         """
+        
         return np.matmul(prob_topic_given_word_transpose.T,prob_word_i)
 
     @staticmethod
     def _check_passed_variables(
             algorithm,
             prob_topic_given_document_transpose,
             prob_topic_given_word_transpose,
@@ -744,43 +745,40 @@
                 prob_topic_given_word_transpose, self._prob_word_i,
                 )
         if algorithm in [
                 'flsa',
                 ]:
             prob_document_and_topic = (prob_topic_given_document_transpose.T * self._prob_document_j).T
             prob_document_given_topic = prob_document_and_topic / prob_document_and_topic.sum(axis=0)
-            self._prob_word_given_document = np.asarray(global_term_weights / global_term_weights.sum(1))
-            self._prob_word_given_topic = np.matmul(
-                self._prob_word_given_document.T,
-                prob_document_given_topic,
-                )
+            self._prob_word_given_document = global_term_weights / global_term_weights.sum(1)
+            self._prob_word_given_topic = self._prob_word_given_document.T.dot(
+                                        prob_document_given_topic
+                                    )
             prob_topic_given_document = prob_topic_given_document_transpose.T
             return self._prob_word_given_topic, prob_topic_given_document
 
         elif algorithm in [
                 'flsa-w',
                 'flsa-v',
                 'flsa-e'
                 ]:
             prob_word_and_topic = (prob_topic_given_word_transpose.T * self._prob_word_i).T
             self._prob_word_given_topic = prob_word_and_topic / prob_word_and_topic.sum(axis=0)
             if algorithm in [
                     'flsa-w',
                     ]:
-                self._prob_word_given_document = np.asarray(global_term_weights / global_term_weights.sum(1)).T
+                self._prob_word_given_document = (global_term_weights / global_term_weights.sum(1)).T
             elif algorithm in [
                     'flsa-v',
                     'flsa-e',
                     ]:
                 self._prob_word_given_document = np.asarray(local_term_weights / local_term_weights.sum(1)).T
-            prob_document_given_word = ((self._prob_word_given_document*self._prob_document_j).T /
-                                        np.array(self._prob_word_i))
-            prob_document_given_topic = np.matmul(
-                prob_document_given_word,
-                self._prob_word_given_topic,
+            prob_document_given_word = self._prob_word_given_document.T.multiply(np.reshape(self._prob_document_j, (-1, 1))).toarray() /np.reshape(np.array(self._prob_word_i), (1, -1))
+            prob_document_given_topic = prob_document_given_word.dot(
+                self._prob_word_given_topic
                 )
             prob_topic_given_document = ((prob_document_given_topic * self._prob_topic_k).T/
                                                self._prob_document_j)
             return self._prob_word_given_topic, prob_topic_given_document
         raise ValueError('"algorithm" is unknown.')
 
     def show_topics(
```

### Comparing `FuzzyTM-2.0.8/FuzzyTM/analysis/topic_specificity.py` & `FuzzyTM-2.0.9/FuzzyTM/analysis/topic_specificity.py`

 * *Files identical despite different names*

### Comparing `FuzzyTM-2.0.8/FuzzyTM.egg-info/PKG-INFO` & `FuzzyTM-2.0.9/FuzzyTM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuzzyTM
-Version: 2.0.8
+Version: 2.0.9
 Summary: A Python package for Fuzzy Topic Models
 Home-page: https://github.com/ERijck/FuzzyTM
 Author: Emil Rijcken
 Author-email: emil.rijcken@gmail.com
 License: GNU General Public License v3.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `FuzzyTM-2.0.8/LICENSE` & `FuzzyTM-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `FuzzyTM-2.0.8/PKG-INFO` & `FuzzyTM-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuzzyTM
-Version: 2.0.8
+Version: 2.0.9
 Summary: A Python package for Fuzzy Topic Models
 Home-page: https://github.com/ERijck/FuzzyTM
 Author: Emil Rijcken
 Author-email: emil.rijcken@gmail.com
 License: GNU General Public License v3.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `FuzzyTM-2.0.8/README.md` & `FuzzyTM-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `FuzzyTM-2.0.8/setup.py` & `FuzzyTM-2.0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 import pathlib
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '2.0.8'
+VERSION = '2.0.9'
 PACKAGE_NAME = 'FuzzyTM'
 AUTHOR = 'Emil Rijcken'
 AUTHOR_EMAIL = 'emil.rijcken@gmail.com'
 URL = 'https://github.com/ERijck/FuzzyTM'
 
 LICENSE = 'GNU General Public License v3.0'
 DESCRIPTION = 'A Python package for Fuzzy Topic Models'
```

