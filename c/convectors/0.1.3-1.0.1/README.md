# Comparing `tmp/convectors-0.1.3.tar.gz` & `tmp/convectors-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "convectors-0.1.3.tar", last modified: Wed Oct 26 15:04:54 2022, max compression
+gzip compressed data, was "convectors-1.0.1.tar", last modified: Wed Apr 24 15:10:02 2024, max compression
```

## Comparing `convectors-0.1.3.tar` & `convectors-1.0.1.tar`

### file list

```diff
@@ -1,63 +1,51 @@
-drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2022-10-26 15:04:54.470956 convectors-0.1.3/
--rw-rw-r--   0 maixent   (1000) maixent   (1000)      117 2022-05-30 13:50:28.000000 convectors-0.1.3/MANIFEST.in
--rw-rw-r--   0 maixent   (1000) maixent   (1000)     3076 2022-10-26 15:04:54.466956 convectors-0.1.3/PKG-INFO
--rw-rw-r--   0 maixent   (1000) maixent   (1000)     2155 2022-06-14 17:22:11.000000 convectors-0.1.3/README.md
-drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2022-10-26 15:04:54.446956 convectors-0.1.3/convectors/
--rw-rw-r--   0 maixent   (1000) maixent   (1000)    11376 2022-04-12 11:48:44.000000 convectors-0.1.3/convectors/__init__.py
-drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2022-10-26 15:04:54.446956 convectors-0.1.3/convectors/classifier/
--rw-rw-r--   0 maixent   (1000) maixent   (1000)    27506 2022-06-17 09:16:26.000000 convectors-0.1.3/convectors/classifier/__init__.py
--rw-rw-r--   0 maixent   (1000) maixent   (1000)     6941 2022-06-16 16:36:38.000000 convectors-0.1.3/convectors/classifier/layers.py
--rw-rw-r--   0 maixent   (1000) maixent   (1000)      602 2022-03-18 14:50:26.000000 convectors-0.1.3/convectors/classifier/utils.py
--rw-rw-r--   0 maixent   (1000) maixent   (1000)     4136 2022-09-07 09:36:00.000000 convectors-0.1.3/convectors/collections.py
-drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2022-10-26 15:04:54.446956 convectors-0.1.3/convectors/embedding/
--rw-rw-r--   0 maixent   (1000) maixent   (1000)    21435 2022-10-26 13:45:38.000000 convectors-0.1.3/convectors/embedding/__init__.py
--rw-rw-r--   0 maixent   (1000) maixent   (1000)     4408 2022-06-14 17:12:11.000000 convectors-0.1.3/convectors/graph.py
-drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2022-10-26 15:04:54.446956 convectors-0.1.3/convectors/huggingface/
--rw-rw-r--   0 maixent   (1000) maixent   (1000)     5761 2022-05-11 12:12:41.000000 convectors-0.1.3/convectors/huggingface/__init__.py
-drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2022-10-26 15:04:54.446956 convectors-0.1.3/convectors/image/
--rw-r--r--   0 maixent   (1000) maixent   (1000)       56 2022-03-17 17:38:14.000000 convectors-0.1.3/convectors/image/__init__.py
-drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2022-10-26 15:04:54.450956 convectors-0.1.3/convectors/image/data/
--rw-r--r--   0 maixent   (1000) maixent   (1000)     3632 2022-03-17 17:37:50.000000 convectors-0.1.3/convectors/image/data/__init__.py
-drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2022-10-26 15:04:54.450956 convectors-0.1.3/convectors/image/features/
--rw-r--r--   0 maixent   (1000) maixent   (1000)     2350 2022-03-17 17:37:38.000000 convectors-0.1.3/convectors/image/features/__init__.py
-drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2022-10-26 15:04:54.450956 convectors-0.1.3/convectors/image/ml/
--rw-r--r--   0 maixent   (1000) maixent   (1000)     4011 2022-03-22 10:10:52.000000 convectors-0.1.3/convectors/image/ml/__init__.py
--rw-r--r--   0 maixent   (1000) maixent   (1000)     1083 2022-03-08 18:13:02.000000 convectors-0.1.3/convectors/image/utils.py
--rw-rw-r--   0 maixent   (1000) maixent   (1000)     1172 2022-10-04 09:40:23.000000 convectors-0.1.3/convectors/layers.py
-drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2022-10-26 15:04:54.450956 convectors-0.1.3/convectors/linguistics/
--rw-r--r--   0 maixent   (1000) maixent   (1000)    19813 2022-10-13 08:19:54.000000 convectors-0.1.3/convectors/linguistics/__init__.py
--rw-rw-r--   0 maixent   (1000) maixent   (1000)    39923 2022-07-29 12:43:25.000000 convectors-0.1.3/convectors/linguistics/stopwords.py
--rw-r--r--   0 maixent   (1000) maixent   (1000)      408 2022-10-04 09:39:35.000000 convectors-0.1.3/convectors/linguistics/utils.py
-drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2022-10-26 15:04:54.450956 convectors-0.1.3/convectors/multi/
--rw-rw-r--   0 maixent   (1000) maixent   (1000)     1283 2021-10-11 14:26:34.000000 convectors-0.1.3/convectors/multi/__init__.py
-drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2022-10-26 15:04:54.450956 convectors-0.1.3/convectors/preprocessing/
--rw-rw-r--   0 maixent   (1000) maixent   (1000)     2187 2021-10-15 09:26:19.000000 convectors-0.1.3/convectors/preprocessing/__init__.py
-drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2022-10-26 15:04:54.450956 convectors-0.1.3/convectors/reduction/
--rw-rw-r--   0 maixent   (1000) maixent   (1000)     3521 2022-06-09 09:15:08.000000 convectors-0.1.3/convectors/reduction/__init__.py
--rw-rw-r--   0 maixent   (1000) maixent   (1000)    10233 2021-08-25 08:40:15.000000 convectors-0.1.3/convectors/regressor.py
-drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2022-10-26 15:04:54.442956 convectors-0.1.3/convectors/ressources/
-drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2022-10-26 15:04:54.450956 convectors-0.1.3/convectors/ressources/cooc/
--rw-rw-r--   0 maixent   (1000) maixent   (1000)   164229 2022-05-30 13:45:11.000000 convectors-0.1.3/convectors/ressources/cooc/fr_cooc.p
--rw-rw-r--   0 maixent   (1000) maixent   (1000)   102516 2022-05-30 13:46:02.000000 convectors-0.1.3/convectors/ressources/cooc/fr_cooc_lower.p
-drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2022-10-26 15:04:54.458956 convectors-0.1.3/convectors/ressources/lemma/
--rw-rw-r--   0 maixent   (1000) maixent   (1000)   676982 2022-05-05 13:04:26.000000 convectors-0.1.3/convectors/ressources/lemma/de_lemma.p
--rw-rw-r--   0 maixent   (1000) maixent   (1000)   580932 2022-03-21 09:41:32.000000 convectors-0.1.3/convectors/ressources/lemma/en_lemma.p
--rw-rw-r--   0 maixent   (1000) maixent   (1000)  1991387 2021-12-16 10:19:26.000000 convectors-0.1.3/convectors/ressources/lemma/fr_lemma.p
--rw-rw-r--   0 maixent   (1000) maixent   (1000)   442222 2022-05-05 13:29:27.000000 convectors-0.1.3/convectors/ressources/lemma/it_lemma.p
--rw-rw-r--   0 maixent   (1000) maixent   (1000)   448070 2022-05-05 13:22:21.000000 convectors-0.1.3/convectors/ressources/lemma/pt_lemma.p
-drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2022-10-26 15:04:54.462956 convectors-0.1.3/convectors/ressources/ner/
--rw-rw-r--   0 maixent   (1000) maixent   (1000)  3416373 2022-05-13 09:16:42.000000 convectors-0.1.3/convectors/ressources/ner/en_ner.p
-drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2022-10-26 15:04:54.466956 convectors-0.1.3/convectors/spacy/
--rw-rw-r--   0 maixent   (1000) maixent   (1000)     1534 2021-11-29 10:13:07.000000 convectors-0.1.3/convectors/spacy/__init__.py
--rw-rw-r--   0 maixent   (1000) maixent   (1000)     2744 2022-07-11 08:43:04.000000 convectors-0.1.3/convectors/special.py
-drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2022-10-26 15:04:54.466956 convectors-0.1.3/convectors/task/
--rw-rw-r--   0 maixent   (1000) maixent   (1000)     1267 2022-09-26 12:45:29.000000 convectors-0.1.3/convectors/task/__init__.py
--rw-rw-r--   0 maixent   (1000) maixent   (1000)     3110 2022-10-26 13:44:15.000000 convectors-0.1.3/convectors/utils.py
-drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2022-10-26 15:04:54.446956 convectors-0.1.3/convectors.egg-info/
--rw-r--r--   0 maixent   (1000) maixent   (1000)     3076 2022-10-26 15:04:54.000000 convectors-0.1.3/convectors.egg-info/PKG-INFO
--rw-rw-r--   0 maixent   (1000) maixent   (1000)     1248 2022-10-26 15:04:54.000000 convectors-0.1.3/convectors.egg-info/SOURCES.txt
--rw-rw-r--   0 maixent   (1000) maixent   (1000)        1 2022-10-26 15:04:54.000000 convectors-0.1.3/convectors.egg-info/dependency_links.txt
--rw-rw-r--   0 maixent   (1000) maixent   (1000)       42 2022-10-26 15:04:54.000000 convectors-0.1.3/convectors.egg-info/requires.txt
--rw-rw-r--   0 maixent   (1000) maixent   (1000)       11 2022-10-26 15:04:54.000000 convectors-0.1.3/convectors.egg-info/top_level.txt
--rw-rw-r--   0 maixent   (1000) maixent   (1000)       38 2022-10-26 15:04:54.470956 convectors-0.1.3/setup.cfg
--rw-rw-r--   0 maixent   (1000) maixent   (1000)      850 2022-10-26 15:04:10.000000 convectors-0.1.3/setup.py
+drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2024-04-24 15:10:02.793300 convectors-1.0.1/
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)      333 2024-04-24 15:10:02.793300 convectors-1.0.1/PKG-INFO
+drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2024-04-24 15:10:02.789301 convectors-1.0.1/convectors/
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)        0 2023-06-27 09:51:21.000000 convectors-1.0.1/convectors/__init__.py
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)     8597 2024-04-24 10:13:33.000000 convectors-1.0.1/convectors/base_layer.py
+drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2024-04-24 15:10:02.789301 convectors-1.0.1/convectors/keras/
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)       45 2023-07-24 14:49:05.000000 convectors-1.0.1/convectors/keras/__init__.py
+-rw-r--r--   0 maixent   (1000) maixent   (1000)     4014 2023-09-14 15:24:24.000000 convectors-1.0.1/convectors/keras/base.py
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)      751 2023-07-25 08:21:37.000000 convectors-1.0.1/convectors/keras/callbacks.py
+drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2024-04-24 15:10:02.789301 convectors-1.0.1/convectors/knn/
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)      108 2023-12-04 13:09:02.000000 convectors-1.0.1/convectors/knn/__init__.py
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)     5700 2024-01-18 15:02:57.000000 convectors-1.0.1/convectors/knn/algorithms.py
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)      908 2023-12-04 13:25:15.000000 convectors-1.0.1/convectors/layers.py
+drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2024-04-24 15:10:02.789301 convectors-1.0.1/convectors/merging/
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)       65 2023-06-27 14:29:49.000000 convectors-1.0.1/convectors/merging/__init__.py
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)      888 2023-07-24 09:10:17.000000 convectors-1.0.1/convectors/merging/concatenate.py
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)     9304 2024-04-15 14:10:12.000000 convectors-1.0.1/convectors/models.py
+drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2024-04-24 15:10:02.789301 convectors-1.0.1/convectors/operations/
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)       47 2023-07-24 12:33:39.000000 convectors-1.0.1/convectors/operations/__init__.py
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)      386 2023-07-24 13:04:21.000000 convectors-1.0.1/convectors/operations/base.py
+drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2024-04-24 15:10:02.789301 convectors-1.0.1/convectors/preprocessing/
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)      261 2023-12-04 13:24:45.000000 convectors-1.0.1/convectors/preprocessing/__init__.py
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)     8555 2023-12-04 13:24:26.000000 convectors-1.0.1/convectors/preprocessing/base.py
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)      813 2023-10-02 17:17:47.000000 convectors-1.0.1/convectors/preprocessing/utils.py
+drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2024-04-24 15:10:02.789301 convectors-1.0.1/convectors/reduction/
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)       41 2023-07-24 11:42:33.000000 convectors-1.0.1/convectors/reduction/__init__.py
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)     1129 2023-12-04 13:14:15.000000 convectors-1.0.1/convectors/reduction/base.py
+drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2024-04-24 15:10:02.793300 convectors-1.0.1/convectors/tokenizers/
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)      179 2023-12-04 10:22:33.000000 convectors-1.0.1/convectors/tokenizers/__init__.py
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)     8573 2024-04-15 14:47:13.000000 convectors-1.0.1/convectors/tokenizers/base.py
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)    60084 2024-04-15 15:38:26.000000 convectors-1.0.1/convectors/tokenizers/stopwords.py
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)     2771 2023-07-24 09:11:03.000000 convectors-1.0.1/convectors/tokenizers/tiktoken.py
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)     2514 2024-04-15 14:50:17.000000 convectors-1.0.1/convectors/tokenizers/utils.py
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)      618 2023-09-12 14:04:16.000000 convectors-1.0.1/convectors/utils.py
+drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2024-04-24 15:10:02.793300 convectors-1.0.1/convectors/vectorizers/
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)      134 2024-04-15 10:31:31.000000 convectors-1.0.1/convectors/vectorizers/__init__.py
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)     2225 2024-04-15 10:32:32.000000 convectors-1.0.1/convectors/vectorizers/bm25.py
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)     3444 2024-04-15 09:30:57.000000 convectors-1.0.1/convectors/vectorizers/bow.py
+drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2024-04-24 15:10:02.789301 convectors-1.0.1/convectors.egg-info/
+-rw-r--r--   0 maixent   (1000) maixent   (1000)      333 2024-04-24 15:10:02.000000 convectors-1.0.1/convectors.egg-info/PKG-INFO
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)     1071 2024-04-24 15:10:02.000000 convectors-1.0.1/convectors.egg-info/SOURCES.txt
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)        1 2024-04-24 15:10:02.000000 convectors-1.0.1/convectors.egg-info/dependency_links.txt
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)       79 2024-04-24 15:10:02.000000 convectors-1.0.1/convectors.egg-info/requires.txt
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)       17 2024-04-24 15:10:02.000000 convectors-1.0.1/convectors.egg-info/top_level.txt
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)       38 2024-04-24 15:10:02.793300 convectors-1.0.1/setup.cfg
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)      658 2024-04-24 15:09:19.000000 convectors-1.0.1/setup.py
+drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2024-04-24 15:10:02.793300 convectors-1.0.1/tests/
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)        0 2023-06-27 09:14:38.000000 convectors-1.0.1/tests/__init__.py
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)     1139 2024-04-15 09:29:00.000000 convectors-1.0.1/tests/test_functional_api.py
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)     3548 2024-04-15 09:31:37.000000 convectors-1.0.1/tests/test_layers.py
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)      600 2024-04-15 16:01:11.000000 convectors-1.0.1/tests/test_topics.py
```

### Comparing `convectors-0.1.3/convectors.egg-info/SOURCES.txt` & `convectors-1.0.1/convectors.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,41 +1,37 @@
-MANIFEST.in
-README.md
 setup.py
 convectors/__init__.py
-convectors/collections.py
-convectors/graph.py
+convectors/base_layer.py
 convectors/layers.py
-convectors/regressor.py
-convectors/special.py
+convectors/models.py
 convectors/utils.py
 convectors.egg-info/PKG-INFO
 convectors.egg-info/SOURCES.txt
 convectors.egg-info/dependency_links.txt
 convectors.egg-info/requires.txt
 convectors.egg-info/top_level.txt
-convectors/classifier/__init__.py
-convectors/classifier/layers.py
-convectors/classifier/utils.py
-convectors/embedding/__init__.py
-convectors/huggingface/__init__.py
-convectors/image/__init__.py
-convectors/image/utils.py
-convectors/image/data/__init__.py
-convectors/image/features/__init__.py
-convectors/image/ml/__init__.py
-convectors/linguistics/__init__.py
-convectors/linguistics/stopwords.py
-convectors/linguistics/utils.py
-convectors/multi/__init__.py
+convectors/keras/__init__.py
+convectors/keras/base.py
+convectors/keras/callbacks.py
+convectors/knn/__init__.py
+convectors/knn/algorithms.py
+convectors/merging/__init__.py
+convectors/merging/concatenate.py
+convectors/operations/__init__.py
+convectors/operations/base.py
 convectors/preprocessing/__init__.py
+convectors/preprocessing/base.py
+convectors/preprocessing/utils.py
 convectors/reduction/__init__.py
-convectors/ressources/cooc/fr_cooc.p
-convectors/ressources/cooc/fr_cooc_lower.p
-convectors/ressources/lemma/de_lemma.p
-convectors/ressources/lemma/en_lemma.p
-convectors/ressources/lemma/fr_lemma.p
-convectors/ressources/lemma/it_lemma.p
-convectors/ressources/lemma/pt_lemma.p
-convectors/ressources/ner/en_ner.p
-convectors/spacy/__init__.py
-convectors/task/__init__.py
+convectors/reduction/base.py
+convectors/tokenizers/__init__.py
+convectors/tokenizers/base.py
+convectors/tokenizers/stopwords.py
+convectors/tokenizers/tiktoken.py
+convectors/tokenizers/utils.py
+convectors/vectorizers/__init__.py
+convectors/vectorizers/bm25.py
+convectors/vectorizers/bow.py
+tests/__init__.py
+tests/test_functional_api.py
+tests/test_layers.py
+tests/test_topics.py
```

