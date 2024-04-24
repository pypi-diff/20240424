# Comparing `tmp/sts_lib-0.27.3.tar.gz` & `tmp/sts_lib-0.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sts_lib-0.27.3.tar", last modified: Tue Apr 23 12:41:23 2024, max compression
+gzip compressed data, was "sts_lib-0.28.0.tar", last modified: Wed Apr 24 14:48:24 2024, max compression
```

## Comparing `sts_lib-0.27.3.tar` & `sts_lib-0.28.0.tar`

### file list

```diff
@@ -1,55 +1,80 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 12:41:23.200500 sts_lib-0.27.3/
--rw-rw-rw-   0        0        0    11358 2024-04-19 09:05:26.000000 sts_lib-0.27.3/LICENSE
--rw-rw-rw-   0        0        0       13 2024-04-19 09:05:26.000000 sts_lib-0.27.3/MANIFEST.in
--rw-rw-rw-   0        0        0    11030 2024-04-23 12:41:23.199501 sts_lib-0.27.3/PKG-INFO
--rw-rw-rw-   0        0        0     9577 2024-04-23 09:54:22.000000 sts_lib-0.27.3/README.md
--rw-rw-rw-   0        0        0     1728 2024-04-23 12:41:23.202486 sts_lib-0.27.3/setup.cfg
--rw-rw-rw-   0        0        0       65 2024-04-19 09:05:26.000000 sts_lib-0.27.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 12:41:23.159628 sts_lib-0.27.3/sts/
--rw-rw-rw-   0        0        0    52156 2024-04-23 12:35:24.000000 sts_lib-0.27.3/sts/__init__.py
--rw-rw-rw-   0        0        0       89 2024-04-19 09:05:26.000000 sts_lib-0.27.3/sts/__main__.py
--rw-rw-rw-   0        0        0     7551 2024-04-23 09:39:28.000000 sts_lib-0.27.3/sts/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-23 12:41:23.160622 sts_lib-0.27.3/sts/data/
-drwxrwxrwx   0        0        0        0 2024-04-23 12:41:23.173752 sts_lib-0.27.3/sts/data/config/
--rw-rw-rw-   0        0        0      915 2024-04-23 09:39:28.000000 sts_lib-0.27.3/sts/data/config/_default.json
--rw-rw-rw-   0        0        0      608 2024-04-23 09:37:27.000000 sts_lib-0.27.3/sts/data/config/hk2s.json
--rw-rw-rw-   0        0        0      346 2024-04-23 09:37:27.000000 sts_lib-0.27.3/sts/data/config/hk2t.json
--rw-rw-rw-   0        0        0      410 2024-04-23 09:39:28.000000 sts_lib-0.27.3/sts/data/config/jp2t.json
--rw-rw-rw-   0        0        0      419 2024-04-23 09:39:28.000000 sts_lib-0.27.3/sts/data/config/s2hk.json
--rw-rw-rw-   0        0        0      267 2024-04-23 09:39:28.000000 sts_lib-0.27.3/sts/data/config/s2t.json
--rw-rw-rw-   0        0        0      417 2024-04-23 09:39:28.000000 sts_lib-0.27.3/sts/data/config/s2tw.json
--rw-rw-rw-   0        0        0      608 2024-04-23 09:39:28.000000 sts_lib-0.27.3/sts/data/config/s2twp.json
--rw-rw-rw-   0        0        0      247 2024-04-23 09:37:27.000000 sts_lib-0.27.3/sts/data/config/t2hk.json
--rw-rw-rw-   0        0        0      261 2024-04-23 09:39:28.000000 sts_lib-0.27.3/sts/data/config/t2jp.json
--rw-rw-rw-   0        0        0      267 2024-04-23 09:37:27.000000 sts_lib-0.27.3/sts/data/config/t2s.json
--rw-rw-rw-   0        0        0      245 2024-04-23 09:37:27.000000 sts_lib-0.27.3/sts/data/config/t2tw.json
--rw-rw-rw-   0        0        0      606 2024-04-23 09:37:27.000000 sts_lib-0.27.3/sts/data/config/tw2s.json
--rw-rw-rw-   0        0        0      670 2024-04-23 09:39:28.000000 sts_lib-0.27.3/sts/data/config/tw2sp.json
--rw-rw-rw-   0        0        0      344 2024-04-23 09:37:27.000000 sts_lib-0.27.3/sts/data/config/tw2t.json
-drwxrwxrwx   0        0        0        0 2024-04-23 12:41:23.189297 sts_lib-0.27.3/sts/data/dictionary/
--rw-rw-rw-   0        0        0      595 2024-04-23 09:39:28.000000 sts_lib-0.27.3/sts/data/dictionary/HKVariants.txt
--rw-rw-rw-   0        0        0     2865 2024-04-23 09:37:27.000000 sts_lib-0.27.3/sts/data/dictionary/HKVariantsRevPhrases.txt
--rw-rw-rw-   0        0        0      103 2024-04-23 09:39:28.000000 sts_lib-0.27.3/sts/data/dictionary/JPShinjitaiCharacters.txt
--rw-rw-rw-   0        0        0     2720 2024-04-23 09:37:27.000000 sts_lib-0.27.3/sts/data/dictionary/JPShinjitaiPhrases.txt
--rw-rw-rw-   0        0        0     3307 2024-04-23 09:39:28.000000 sts_lib-0.27.3/sts/data/dictionary/JPVariants.txt
--rw-rw-rw-   0        0        0    38333 2024-04-23 09:39:28.000000 sts_lib-0.27.3/sts/data/dictionary/STCharacters.txt
--rw-rw-rw-   0        0        0  1053351 2024-04-23 09:39:28.000000 sts_lib-0.27.3/sts/data/dictionary/STPhrases.txt
--rw-rw-rw-   0        0        0    38740 2024-04-23 09:39:28.000000 sts_lib-0.27.3/sts/data/dictionary/TSCharacters.txt
--rw-rw-rw-   0        0        0     5438 2024-04-23 09:39:28.000000 sts_lib-0.27.3/sts/data/dictionary/TSPhrases.txt
--rw-rw-rw-   0        0        0     8014 2024-04-23 09:37:55.000000 sts_lib-0.27.3/sts/data/dictionary/TWPhrasesIT.txt
--rw-rw-rw-   0        0        0     2205 2024-04-23 09:37:27.000000 sts_lib-0.27.3/sts/data/dictionary/TWPhrasesName.txt
--rw-rw-rw-   0        0        0      608 2024-04-23 09:39:28.000000 sts_lib-0.27.3/sts/data/dictionary/TWPhrasesOther.txt
--rw-rw-rw-   0        0        0      351 2024-04-23 09:39:28.000000 sts_lib-0.27.3/sts/data/dictionary/TWVariants.txt
--rw-rw-rw-   0        0        0     1143 2024-04-23 09:37:27.000000 sts_lib-0.27.3/sts/data/dictionary/TWVariantsRevPhrases.txt
--rw-rw-rw-   0        0        0    22760 2024-04-23 08:00:20.000000 sts_lib-0.27.3/sts/data/htmlpage.tpl.html
-drwxrwxrwx   0        0        0        0 2024-04-23 12:41:23.191297 sts_lib-0.27.3/sts/data/scheme/
--rw-rw-rw-   0        0        0    21633 2024-04-23 09:39:28.000000 sts_lib-0.27.3/sts/data/scheme/st_multi.txt
--rw-rw-rw-   0        0        0      436 2024-04-23 09:39:28.000000 sts_lib-0.27.3/sts/data/scheme/ts_multi.txt
--rw-rw-rw-   0        0        0     2108 2024-04-23 09:18:42.000000 sts_lib-0.27.3/sts/data/scheme/variant.txt
-drwxrwxrwx   0        0        0        0 2024-04-23 12:41:23.197500 sts_lib-0.27.3/sts_lib.egg-info/
--rw-rw-rw-   0        0        0    11030 2024-04-23 12:41:23.000000 sts_lib-0.27.3/sts_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1325 2024-04-23 12:41:23.000000 sts_lib-0.27.3/sts_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 12:41:23.000000 sts_lib-0.27.3/sts_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-04-23 12:41:23.000000 sts_lib-0.27.3/sts_lib.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      202 2024-04-23 12:41:23.000000 sts_lib-0.27.3/sts_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-23 12:41:23.000000 sts_lib-0.27.3/sts_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 14:48:24.049973 sts_lib-0.28.0/
+-rw-rw-rw-   0        0        0    11358 2024-04-19 09:05:26.000000 sts_lib-0.28.0/LICENSE
+-rw-rw-rw-   0        0        0       13 2024-04-19 09:05:26.000000 sts_lib-0.28.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    11150 2024-04-24 14:48:24.049973 sts_lib-0.28.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9697 2024-04-24 14:00:06.000000 sts_lib-0.28.0/README.md
+-rw-rw-rw-   0        0        0     1814 2024-04-24 14:48:24.051687 sts_lib-0.28.0/setup.cfg
+-rw-rw-rw-   0        0        0       65 2024-04-19 09:05:26.000000 sts_lib-0.28.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:48:23.941627 sts_lib-0.28.0/sts/
+-rw-rw-rw-   0        0        0    52162 2024-04-24 14:46:21.000000 sts_lib-0.28.0/sts/__init__.py
+-rw-rw-rw-   0        0        0       89 2024-04-19 09:05:26.000000 sts_lib-0.28.0/sts/__main__.py
+-rw-rw-rw-   0        0        0     7551 2024-04-23 13:05:20.000000 sts_lib-0.28.0/sts/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:48:23.943403 sts_lib-0.28.0/sts/data/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:48:23.914548 sts_lib-0.28.0/sts/data/OpenCC/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:48:23.978875 sts_lib-0.28.0/sts/data/OpenCC/config/
+-rw-rw-rw-   0        0        0      915 2024-04-24 14:46:21.000000 sts_lib-0.28.0/sts/data/OpenCC/config/_default.json
+-rw-rw-rw-   0        0        0      608 2024-04-24 14:46:21.000000 sts_lib-0.28.0/sts/data/OpenCC/config/hk2s.json
+-rw-rw-rw-   0        0        0      346 2024-04-24 14:46:21.000000 sts_lib-0.28.0/sts/data/OpenCC/config/hk2t.json
+-rw-rw-rw-   0        0        0      410 2024-04-24 14:46:21.000000 sts_lib-0.28.0/sts/data/OpenCC/config/jp2t.json
+-rw-rw-rw-   0        0        0      419 2024-04-24 14:46:21.000000 sts_lib-0.28.0/sts/data/OpenCC/config/s2hk.json
+-rw-rw-rw-   0        0        0      267 2024-04-24 14:46:21.000000 sts_lib-0.28.0/sts/data/OpenCC/config/s2t.json
+-rw-rw-rw-   0        0        0      417 2024-04-24 14:46:21.000000 sts_lib-0.28.0/sts/data/OpenCC/config/s2tw.json
+-rw-rw-rw-   0        0        0      608 2024-04-24 14:46:21.000000 sts_lib-0.28.0/sts/data/OpenCC/config/s2twp.json
+-rw-rw-rw-   0        0        0      247 2024-04-24 14:46:21.000000 sts_lib-0.28.0/sts/data/OpenCC/config/t2hk.json
+-rw-rw-rw-   0        0        0      261 2024-04-24 14:46:21.000000 sts_lib-0.28.0/sts/data/OpenCC/config/t2jp.json
+-rw-rw-rw-   0        0        0      267 2024-04-24 14:46:21.000000 sts_lib-0.28.0/sts/data/OpenCC/config/t2s.json
+-rw-rw-rw-   0        0        0      245 2024-04-24 14:46:21.000000 sts_lib-0.28.0/sts/data/OpenCC/config/t2tw.json
+-rw-rw-rw-   0        0        0      606 2024-04-24 14:46:21.000000 sts_lib-0.28.0/sts/data/OpenCC/config/tw2s.json
+-rw-rw-rw-   0        0        0      670 2024-04-24 14:46:21.000000 sts_lib-0.28.0/sts/data/OpenCC/config/tw2sp.json
+-rw-rw-rw-   0        0        0      344 2024-04-24 14:46:21.000000 sts_lib-0.28.0/sts/data/OpenCC/config/tw2t.json
+drwxrwxrwx   0        0        0        0 2024-04-24 14:48:24.013328 sts_lib-0.28.0/sts/data/OpenCC/dictionary/
+-rw-rw-rw-   0        0        0      595 2024-04-24 14:46:21.000000 sts_lib-0.28.0/sts/data/OpenCC/dictionary/HKVariants.txt
+-rw-rw-rw-   0        0        0     2865 2024-04-24 14:46:21.000000 sts_lib-0.28.0/sts/data/OpenCC/dictionary/HKVariantsRevPhrases.txt
+-rw-rw-rw-   0        0        0      103 2024-04-24 14:46:21.000000 sts_lib-0.28.0/sts/data/OpenCC/dictionary/JPShinjitaiCharacters.txt
+-rw-rw-rw-   0        0        0     2720 2024-04-24 14:46:21.000000 sts_lib-0.28.0/sts/data/OpenCC/dictionary/JPShinjitaiPhrases.txt
+-rw-rw-rw-   0        0        0     3307 2024-04-24 14:46:21.000000 sts_lib-0.28.0/sts/data/OpenCC/dictionary/JPVariants.txt
+-rw-rw-rw-   0        0        0    38333 2024-04-24 14:46:21.000000 sts_lib-0.28.0/sts/data/OpenCC/dictionary/STCharacters.txt
+-rw-rw-rw-   0        0        0  1053351 2024-04-24 14:46:21.000000 sts_lib-0.28.0/sts/data/OpenCC/dictionary/STPhrases.txt
+-rw-rw-rw-   0        0        0    38740 2024-04-24 14:46:21.000000 sts_lib-0.28.0/sts/data/OpenCC/dictionary/TSCharacters.txt
+-rw-rw-rw-   0        0        0     5438 2024-04-24 14:46:21.000000 sts_lib-0.28.0/sts/data/OpenCC/dictionary/TSPhrases.txt
+-rw-rw-rw-   0        0        0     8014 2024-04-24 14:46:21.000000 sts_lib-0.28.0/sts/data/OpenCC/dictionary/TWPhrasesIT.txt
+-rw-rw-rw-   0        0        0     2205 2024-04-24 14:46:21.000000 sts_lib-0.28.0/sts/data/OpenCC/dictionary/TWPhrasesName.txt
+-rw-rw-rw-   0        0        0      608 2024-04-24 14:46:21.000000 sts_lib-0.28.0/sts/data/OpenCC/dictionary/TWPhrasesOther.txt
+-rw-rw-rw-   0        0        0      351 2024-04-24 14:46:21.000000 sts_lib-0.28.0/sts/data/OpenCC/dictionary/TWVariants.txt
+-rw-rw-rw-   0        0        0     1143 2024-04-24 14:46:21.000000 sts_lib-0.28.0/sts/data/OpenCC/dictionary/TWVariantsRevPhrases.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 14:48:24.016325 sts_lib-0.28.0/sts/data/OpenCC/scheme/
+-rw-rw-rw-   0        0        0    21633 2024-04-24 14:46:21.000000 sts_lib-0.28.0/sts/data/OpenCC/scheme/st_multi.txt
+-rw-rw-rw-   0        0        0      436 2024-04-24 14:46:21.000000 sts_lib-0.28.0/sts/data/OpenCC/scheme/ts_multi.txt
+-rw-rw-rw-   0        0        0     2108 2024-04-24 14:46:21.000000 sts_lib-0.28.0/sts/data/OpenCC/scheme/variant.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 14:48:24.034317 sts_lib-0.28.0/sts/data/config/
+-rw-rw-rw-   0        0        0      701 2024-04-24 14:46:22.000000 sts_lib-0.28.0/sts/data/config/hk2s.json
+-rw-rw-rw-   0        0        0      421 2024-04-24 14:46:22.000000 sts_lib-0.28.0/sts/data/config/hk2t.json
+-rw-rw-rw-   0        0        0      448 2024-04-24 14:46:21.000000 sts_lib-0.28.0/sts/data/config/jp2t.json
+-rw-rw-rw-   0        0        0     1059 2024-04-24 14:46:22.000000 sts_lib-0.28.0/sts/data/config/s2hk.json
+-rw-rw-rw-   0        0        0      820 2024-04-24 14:46:22.000000 sts_lib-0.28.0/sts/data/config/s2t.json
+-rw-rw-rw-   0        0        0     1057 2024-04-24 14:46:22.000000 sts_lib-0.28.0/sts/data/config/s2tw.json
+-rw-rw-rw-   0        0        0     1315 2024-04-24 14:46:23.000000 sts_lib-0.28.0/sts/data/config/s2twp.json
+-rw-rw-rw-   0        0        0      254 2024-04-24 14:46:21.000000 sts_lib-0.28.0/sts/data/config/t2hk.json
+-rw-rw-rw-   0        0        0      268 2024-04-24 14:46:21.000000 sts_lib-0.28.0/sts/data/config/t2jp.json
+-rw-rw-rw-   0        0        0      281 2024-04-24 14:46:21.000000 sts_lib-0.28.0/sts/data/config/t2s.json
+-rw-rw-rw-   0        0        0      252 2024-04-24 14:46:21.000000 sts_lib-0.28.0/sts/data/config/t2tw.json
+-rw-rw-rw-   0        0        0      699 2024-04-24 14:46:22.000000 sts_lib-0.28.0/sts/data/config/tw2s.json
+-rw-rw-rw-   0        0        0     1114 2024-04-24 14:46:22.000000 sts_lib-0.28.0/sts/data/config/tw2sp.json
+-rw-rw-rw-   0        0        0      419 2024-04-24 14:46:22.000000 sts_lib-0.28.0/sts/data/config/tw2t.json
+drwxrwxrwx   0        0        0        0 2024-04-24 14:48:24.042394 sts_lib-0.28.0/sts/data/dictionary/
+-rw-rw-rw-   0        0        0       78 2024-04-24 14:46:22.000000 sts_lib-0.28.0/sts/data/dictionary/HKVariantsRev.txt
+-rw-rw-rw-   0        0        0      175 2024-04-24 14:46:22.000000 sts_lib-0.28.0/sts/data/dictionary/STPhrases.txt
+-rw-rw-rw-   0        0        0      622 2024-04-24 14:46:22.000000 sts_lib-0.28.0/sts/data/dictionary/STPhrasesExpNum.txt
+-rw-rw-rw-   0        0        0       12 2024-04-24 14:46:22.000000 sts_lib-0.28.0/sts/data/dictionary/STPhrasesExpNumPost.txt
+-rw-rw-rw-   0        0        0       63 2024-04-24 14:46:23.000000 sts_lib-0.28.0/sts/data/dictionary/TWPhrases.txt
+-rw-rw-rw-   0        0        0      117 2024-04-24 14:46:22.000000 sts_lib-0.28.0/sts/data/dictionary/TWPhrasesRev.txt
+-rw-rw-rw-   0        0        0      489 2024-04-24 14:46:22.000000 sts_lib-0.28.0/sts/data/dictionary/TWPhrasesRevExpLang.txt
+-rw-rw-rw-   0        0        0       91 2024-04-24 14:46:22.000000 sts_lib-0.28.0/sts/data/dictionary/TWVariantsRev.txt
+-rw-rw-rw-   0        0        0    22760 2024-04-24 14:46:49.000000 sts_lib-0.28.0/sts/data/htmlpage.tpl.html
+drwxrwxrwx   0        0        0        0 2024-04-24 14:48:24.047975 sts_lib-0.28.0/sts_lib.egg-info/
+-rw-rw-rw-   0        0        0    11150 2024-04-24 14:48:23.000000 sts_lib-0.28.0/sts_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2222 2024-04-24 14:48:23.000000 sts_lib-0.28.0/sts_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 14:48:23.000000 sts_lib-0.28.0/sts_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-04-24 14:48:23.000000 sts_lib-0.28.0/sts_lib.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      202 2024-04-24 14:48:23.000000 sts_lib-0.28.0/sts_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-24 14:48:23.000000 sts_lib-0.28.0/sts_lib.egg-info/top_level.txt
```

### Comparing `sts_lib-0.27.3/LICENSE` & `sts_lib-0.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.3/PKG-INFO` & `sts_lib-0.28.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sts-lib
-Version: 0.27.3
+Version: 0.28.0
 Summary: An open library for flexible simplified-traditional Chinese text conversion.
 Home-page: https://github.com/danny0838/sts-lib
 Author: Danny Lin
 Author-email: danny0838@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
@@ -149,37 +149,39 @@
  * @property {string} [mode=load] - the mode to handle the loaded dicts.
  *     - "load" to simply merge the loaded keys and values;
  *     - "swap" to reverse the dict (i.e. use the values as keys and the keys
  *       as values);
  *     - "join" to chain dicts (a conversion using a dict joining dict1 and
  *       dict2 works like a conversion using dict1 and then dict2, but takes
  *       care of word segmentation);
- *     - "filter" to filter the output values in the loaded dicts with extra
- *       "include" and "exclude" properties
  *     - "expand" to expand the placeholders (defined in the extra
  *       "placeholders" property) in the first dict with the matching key and
  *        values in other dicts;
- *     - "remove_keys" to remove keys from the first dict if it appears in any
- *       other one;
- *     - "remove_values" to remove key-value pairs from the first dict if it
- *       appears in any other one.
+ *     - "filter" to filter the output keys and values in the loaded dicts
+ *       using extra "method", "include", and "exclude" properties.
  * @property {srcDictScheme[]} [src] - the source dicts. `file` must exist when
  *     omitted.
  * @property {boolean} [sort] - true to sort the keys of the output dictionary.
  * @property {boolean} [check] - true to raise an exception if the output
  *     contains an invalid char which will be loaded incorrectly. Set this
  *     when the output is a plain text table file and the source files contain
  *     untrusted JSON or YAML data that may include a char like " ", "\t",
  *     "\n", etc. in the dictionary.
+ * @property {string[]} [placeholders] - strings to be expanded using other
+ *     dicts. (for "expand" mode)
+ * @property {string} [method=remove_key_values] - how to filter (for "filter"
+ *     mode)
+ *     - "remove_keys" to remove keys from the first dict if it appears in any
+ *       other one;
+ *     - "remove_key_values" to remove key-value pairs from the first dict if it
+ *       appears in any other one.
  * @property {string} [include] - a regex filter that discards non-matched
  *     conversion values. (for "filter" mode)
  * @property {string} [exclude] - a regex filter that discards matched
  *     conversion values. (for "filter" mode)
- * @property {string[]} [placeholders] - strings to be expanded using other
- *     dicts. (for "expand" mode)
  */
 ```
 
 ### Dictionary 詞典檔
 
 原始詞典檔可為純文字、JSON、或 YAML。編譯產生的詞典檔有純文字（`.list`）、JSON列表（`.jlist`）、JSON樹（`.tlist`）三種格式，其中前二者可再作為原始檔輸入，後者則只能用於轉換。
```

### Comparing `sts_lib-0.27.3/README.md` & `sts_lib-0.28.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -114,37 +114,39 @@
  * @property {string} [mode=load] - the mode to handle the loaded dicts.
  *     - "load" to simply merge the loaded keys and values;
  *     - "swap" to reverse the dict (i.e. use the values as keys and the keys
  *       as values);
  *     - "join" to chain dicts (a conversion using a dict joining dict1 and
  *       dict2 works like a conversion using dict1 and then dict2, but takes
  *       care of word segmentation);
- *     - "filter" to filter the output values in the loaded dicts with extra
- *       "include" and "exclude" properties
  *     - "expand" to expand the placeholders (defined in the extra
  *       "placeholders" property) in the first dict with the matching key and
  *        values in other dicts;
- *     - "remove_keys" to remove keys from the first dict if it appears in any
- *       other one;
- *     - "remove_values" to remove key-value pairs from the first dict if it
- *       appears in any other one.
+ *     - "filter" to filter the output keys and values in the loaded dicts
+ *       using extra "method", "include", and "exclude" properties.
  * @property {srcDictScheme[]} [src] - the source dicts. `file` must exist when
  *     omitted.
  * @property {boolean} [sort] - true to sort the keys of the output dictionary.
  * @property {boolean} [check] - true to raise an exception if the output
  *     contains an invalid char which will be loaded incorrectly. Set this
  *     when the output is a plain text table file and the source files contain
  *     untrusted JSON or YAML data that may include a char like " ", "\t",
  *     "\n", etc. in the dictionary.
+ * @property {string[]} [placeholders] - strings to be expanded using other
+ *     dicts. (for "expand" mode)
+ * @property {string} [method=remove_key_values] - how to filter (for "filter"
+ *     mode)
+ *     - "remove_keys" to remove keys from the first dict if it appears in any
+ *       other one;
+ *     - "remove_key_values" to remove key-value pairs from the first dict if it
+ *       appears in any other one.
  * @property {string} [include] - a regex filter that discards non-matched
  *     conversion values. (for "filter" mode)
  * @property {string} [exclude] - a regex filter that discards matched
  *     conversion values. (for "filter" mode)
- * @property {string[]} [placeholders] - strings to be expanded using other
- *     dicts. (for "expand" mode)
  */
 ```
 
 ### Dictionary 詞典檔
 
 原始詞典檔可為純文字、JSON、或 YAML。編譯產生的詞典檔有純文字（`.list`）、JSON列表（`.jlist`）、JSON樹（`.tlist`）三種格式，其中前二者可再作為原始檔輸入，後者則只能用於轉換。
```

### Comparing `sts_lib-0.27.3/setup.cfg` & `sts_lib-0.28.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -73,36 +73,42 @@
 00000480: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
 00000490: 6b61 6765 5f64 6174 615d 0d0a 7374 7320  kage_data]..sts 
 000004a0: 3d20 0d0a 0964 6174 612f 2a2e 6874 6d6c  = ...data/*.html
 000004b0: 0d0a 0964 6174 612f 636f 6e66 6967 2f2a  ...data/config/*
 000004c0: 2e6a 736f 6e0d 0a09 6461 7461 2f64 6963  .json...data/dic
 000004d0: 7469 6f6e 6172 792f 2a2e 7478 740d 0a09  tionary/*.txt...
 000004e0: 6461 7461 2f73 6368 656d 652f 2a2e 7478  data/scheme/*.tx
-000004f0: 740d 0a0d 0a5b 6f70 7469 6f6e 732e 656e  t....[options.en
-00000500: 7472 795f 706f 696e 7473 5d0d 0a63 6f6e  try_points]..con
-00000510: 736f 6c65 5f73 6372 6970 7473 203d 200d  sole_scripts = .
-00000520: 0a09 7374 7320 3d20 7374 732e 636c 693a  ..sts = sts.cli:
-00000530: 6d61 696e 0d0a 0d0a 5b66 6c61 6b65 385d  main....[flake8]
-00000540: 0d0a 6578 636c 7564 6520 3d20 6275 696c  ..exclude = buil
-00000550: 642c 202e 6769 740d 0a6d 6178 2d6c 696e  d, .git..max-lin
-00000560: 652d 6c65 6e67 7468 203d 2031 3630 0d0a  e-length = 160..
-00000570: 6578 7465 6e64 2d73 656c 6563 7420 3d20  extend-select = 
-00000580: 0d0a 0945 3132 330d 0a69 676e 6f72 6520  ...E123..ignore 
-00000590: 3d20 0d0a 0957 3530 330d 0a69 676e 6f72  = ...W503..ignor
-000005a0: 652d 6e61 6d65 7320 3d20 0d0a 0973 6574  e-names = ...set
-000005b0: 5570 0d0a 0974 6561 7244 6f77 6e0d 0a09  Up...tearDown...
-000005c0: 7365 7455 7043 6c61 7373 0d0a 0974 6561  setUpClass...tea
-000005d0: 7244 6f77 6e43 6c61 7373 0d0a 0973 6574  rDownClass...set
-000005e0: 5570 4d6f 6475 6c65 0d0a 0974 6561 7244  UpModule...tearD
-000005f0: 6f77 6e4d 6f64 756c 650d 0a09 6173 796e  ownModule...asyn
-00000600: 6353 6574 5570 0d0a 0961 7379 6e63 5465  cSetUp...asyncTe
-00000610: 6172 446f 776e 0d0a 0973 6574 5570 5465  arDown...setUpTe
-00000620: 7374 4461 7461 0d0a 0966 6169 6c75 7265  stData...failure
-00000630: 4578 6365 7074 696f 6e0d 0a09 6c6f 6e67  Exception...long
-00000640: 4d65 7373 6167 650d 0a09 6d61 7844 6966  Message...maxDif
-00000650: 660d 0a0d 0a5b 6973 6f72 745d 0d0a 6d75  f....[isort]..mu
-00000660: 6c74 695f 6c69 6e65 5f6f 7574 7075 7420  lti_line_output 
-00000670: 3d20 330d 0a69 6e63 6c75 6465 5f74 7261  = 3..include_tra
-00000680: 696c 696e 675f 636f 6d6d 6120 3d20 7472  iling_comma = tr
-00000690: 7565 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  ue....[egg_info]
-000006a0: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
-000006b0: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
+000004f0: 740d 0a09 6461 7461 2f4f 7065 6e43 432f  t...data/OpenCC/
+00000500: 636f 6e66 6967 2f2a 2e6a 736f 6e0d 0a09  config/*.json...
+00000510: 6461 7461 2f4f 7065 6e43 432f 6469 6374  data/OpenCC/dict
+00000520: 696f 6e61 7279 2f2a 2e74 7874 0d0a 0964  ionary/*.txt...d
+00000530: 6174 612f 4f70 656e 4343 2f73 6368 656d  ata/OpenCC/schem
+00000540: 652f 2a2e 7478 740d 0a0d 0a5b 6f70 7469  e/*.txt....[opti
+00000550: 6f6e 732e 656e 7472 795f 706f 696e 7473  ons.entry_points
+00000560: 5d0d 0a63 6f6e 736f 6c65 5f73 6372 6970  ]..console_scrip
+00000570: 7473 203d 200d 0a09 7374 7320 3d20 7374  ts = ...sts = st
+00000580: 732e 636c 693a 6d61 696e 0d0a 0d0a 5b66  s.cli:main....[f
+00000590: 6c61 6b65 385d 0d0a 6578 636c 7564 6520  lake8]..exclude 
+000005a0: 3d20 6275 696c 642c 202e 6769 740d 0a6d  = build, .git..m
+000005b0: 6178 2d6c 696e 652d 6c65 6e67 7468 203d  ax-line-length =
+000005c0: 2031 3630 0d0a 6578 7465 6e64 2d73 656c   160..extend-sel
+000005d0: 6563 7420 3d20 0d0a 0945 3132 330d 0a69  ect = ...E123..i
+000005e0: 676e 6f72 6520 3d20 0d0a 0957 3530 330d  gnore = ...W503.
+000005f0: 0a69 676e 6f72 652d 6e61 6d65 7320 3d20  .ignore-names = 
+00000600: 0d0a 0973 6574 5570 0d0a 0974 6561 7244  ...setUp...tearD
+00000610: 6f77 6e0d 0a09 7365 7455 7043 6c61 7373  own...setUpClass
+00000620: 0d0a 0974 6561 7244 6f77 6e43 6c61 7373  ...tearDownClass
+00000630: 0d0a 0973 6574 5570 4d6f 6475 6c65 0d0a  ...setUpModule..
+00000640: 0974 6561 7244 6f77 6e4d 6f64 756c 650d  .tearDownModule.
+00000650: 0a09 6173 796e 6353 6574 5570 0d0a 0961  ..asyncSetUp...a
+00000660: 7379 6e63 5465 6172 446f 776e 0d0a 0973  syncTearDown...s
+00000670: 6574 5570 5465 7374 4461 7461 0d0a 0966  etUpTestData...f
+00000680: 6169 6c75 7265 4578 6365 7074 696f 6e0d  ailureException.
+00000690: 0a09 6c6f 6e67 4d65 7373 6167 650d 0a09  ..longMessage...
+000006a0: 6d61 7844 6966 660d 0a0d 0a5b 6973 6f72  maxDiff....[isor
+000006b0: 745d 0d0a 6d75 6c74 695f 6c69 6e65 5f6f  t]..multi_line_o
+000006c0: 7574 7075 7420 3d20 330d 0a69 6e63 6c75  utput = 3..inclu
+000006d0: 6465 5f74 7261 696c 696e 675f 636f 6d6d  de_trailing_comm
+000006e0: 6120 3d20 7472 7565 0d0a 0d0a 5b65 6767  a = true....[egg
+000006f0: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
+00000700: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
+00000710: 2030 0d0a 0d0a                            0....
```

### Comparing `sts_lib-0.27.3/sts/__init__.py` & `sts_lib-0.28.0/sts/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         @_lazyprop.setter
         def _lazyprop(self, value):
             setattr(self, attr_name, value)
 
         return _lazyprop
 
 
-__version__ = '0.27.3'
+__version__ = '0.28.0'
 
 StsDictMatch = namedtuple('StsDictMatch', ['conv', 'start', 'end'])
 StsDictConv = namedtuple('StsDictConv', ['key', 'values'])
 
 
 class StreamList(list):
     """Convert an iterable into a serializable "list".
@@ -1054,14 +1054,18 @@
                 srcs[i] = self.normalize_dict_scheme(src, config_dir)
 
         mode = dict_scheme.setdefault('mode', 'load')
         dict_scheme['sort'] = bool(dict_scheme.get('sort'))
         dict_scheme['check'] = bool(dict_scheme.get('check'))
 
         if mode == 'filter':
+            method = dict_scheme.setdefault('method', 'remove_key_values')
+            if method not in ('remove_keys', 'remove_key_values'):
+                raise ValueError(f'unknown method for filter: {method}')
+
             try:
                 dict_scheme['include'] = re.compile(dict_scheme['include'])
             except KeyError:
                 dict_scheme['include'] = None
             except re.error as exc:
                 raise ValueError(f'regex syntax error of the "include" filter: {exc}')
 
@@ -1135,31 +1139,14 @@
         for src in dict_scheme['src']:
             if isinstance(src, str):
                 table.load(src)
             else:
                 table.update(src)
         return table
 
-    def _make_dict_mode_filter(self, dict_scheme):
-        table = self._make_dict_mode_load(dict_scheme)
-
-        include = dict_scheme['include']
-        exclude = dict_scheme['exclude']
-        if include or exclude:
-            _table = table
-            table = Table()
-            for key, values in _table.items():
-                values = [v for v in values
-                          if (include is None or include.search(v))
-                          and (exclude is None or not exclude.search(v))]
-                if values:
-                    table.add(key, values)
-
-        return table
-
     def _make_dict_mode_swap(self, dict_scheme):
         table = self._make_dict_mode_load(dict_scheme)
         table = table.swap()
         return table
 
     def _make_dict_mode_join(self, dict_scheme):
         table = Table()
@@ -1245,46 +1232,60 @@
             for value in dicts[dict_idx][comb[comb_idx]]:
                 newparts = parts[:idx] + [value] + parts[idx + 1:]
                 substack.append((newparts, idx + 1))
             while substack:
                 stack.append(substack.pop())
         return rv
 
-    def _make_dict_mode_remove_keys(self, dict_scheme):
+    def _make_dict_mode_filter(self, dict_scheme):
+        method = getattr(self, f'_make_dict_mode_filter_method_{dict_scheme["method"]}')
+
         srcs = dict_scheme['src']
         src = srcs.pop(0)
         table = Table().load(src) if isinstance(src, str) else src
         for src in srcs:
             dict_ = Table().load(src) if isinstance(src, str) else src
-            for k in dict_:
-                try:
-                    del table[k]
-                except KeyError:
-                    continue
+            method(table, dict_)
+
+        include = dict_scheme['include']
+        exclude = dict_scheme['exclude']
+        if include or exclude:
+            _table = table
+            table = Table()
+            for key, values in _table.items():
+                values = [v for v in values
+                          if (include is None or include.search(v))
+                          and (exclude is None or not exclude.search(v))]
+                if values:
+                    table.add(key, values)
+
         return table
 
-    def _make_dict_mode_remove_values(self, dict_scheme):
-        srcs = dict_scheme['src']
-        src = srcs.pop(0)
-        table = Table().load(src) if isinstance(src, str) else src
-        for src in srcs:
-            dict_ = Table().load(src) if isinstance(src, str) else src
-            for k, vv in dict_.items():
+    @staticmethod
+    def _make_dict_mode_filter_method_remove_keys(table, dict):
+        for k in dict:
+            try:
+                del table[k]
+            except KeyError:
+                continue
+
+    @staticmethod
+    def _make_dict_mode_filter_method_remove_key_values(table, dict):
+        for k, vv in dict.items():
+            try:
+                t = table[k]
+            except KeyError:
+                continue
+            for v in vv:
                 try:
-                    t = table[k]
-                except KeyError:
-                    continue
-                for v in vv:
-                    try:
-                        t.remove(v)
-                    except ValueError:
-                        pass
-                if not t:
-                    del table[k]
-        return table
+                    t.remove(v)
+                except ValueError:
+                    pass
+            if not t:
+                del table[k]
 
     def get_config_file(self, config, base_dir=None):
         """Calculate the path of a config file.
 
         1. Use it if it's an absolute path.
         2. Assume relative to base_dir or CWD.
         3. Assume relative to default config directory. (basename only; .json omissible)
```

### Comparing `sts_lib-0.27.3/sts/cli.py` & `sts_lib-0.28.0/sts/cli.py`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.3/sts/data/config/_default.json` & `sts_lib-0.28.0/sts/data/OpenCC/config/_default.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.3/sts/data/config/hk2s.json` & `sts_lib-0.28.0/sts/data/OpenCC/config/hk2s.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.3/sts/data/config/s2twp.json` & `sts_lib-0.28.0/sts/data/OpenCC/config/s2twp.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.3/sts/data/config/tw2s.json` & `sts_lib-0.28.0/sts/data/OpenCC/config/tw2s.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.3/sts/data/config/tw2sp.json` & `sts_lib-0.28.0/sts/data/OpenCC/config/tw2sp.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.3/sts/data/dictionary/HKVariants.txt` & `sts_lib-0.28.0/sts/data/OpenCC/dictionary/HKVariants.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.3/sts/data/dictionary/HKVariantsRevPhrases.txt` & `sts_lib-0.28.0/sts/data/OpenCC/dictionary/HKVariantsRevPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.3/sts/data/dictionary/JPShinjitaiPhrases.txt` & `sts_lib-0.28.0/sts/data/OpenCC/dictionary/JPShinjitaiPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.3/sts/data/dictionary/JPVariants.txt` & `sts_lib-0.28.0/sts/data/OpenCC/dictionary/JPVariants.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.3/sts/data/dictionary/STCharacters.txt` & `sts_lib-0.28.0/sts/data/OpenCC/dictionary/STCharacters.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.3/sts/data/dictionary/STPhrases.txt` & `sts_lib-0.28.0/sts/data/OpenCC/dictionary/STPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.3/sts/data/dictionary/TSCharacters.txt` & `sts_lib-0.28.0/sts/data/OpenCC/dictionary/TSCharacters.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.3/sts/data/dictionary/TSPhrases.txt` & `sts_lib-0.28.0/sts/data/OpenCC/dictionary/TSPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.3/sts/data/dictionary/TWPhrasesIT.txt` & `sts_lib-0.28.0/sts/data/OpenCC/dictionary/TWPhrasesIT.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.3/sts/data/dictionary/TWPhrasesName.txt` & `sts_lib-0.28.0/sts/data/OpenCC/dictionary/TWPhrasesName.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.3/sts/data/dictionary/TWPhrasesOther.txt` & `sts_lib-0.28.0/sts/data/OpenCC/dictionary/TWPhrasesOther.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.3/sts/data/dictionary/TWVariantsRevPhrases.txt` & `sts_lib-0.28.0/sts/data/OpenCC/dictionary/TWVariantsRevPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.3/sts/data/htmlpage.tpl.html` & `sts_lib-0.28.0/sts/data/htmlpage.tpl.html`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.3/sts/data/scheme/st_multi.txt` & `sts_lib-0.28.0/sts/data/OpenCC/scheme/st_multi.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.3/sts/data/scheme/variant.txt` & `sts_lib-0.28.0/sts/data/OpenCC/scheme/variant.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.3/sts_lib.egg-info/PKG-INFO` & `sts_lib-0.28.0/sts_lib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sts-lib
-Version: 0.27.3
+Version: 0.28.0
 Summary: An open library for flexible simplified-traditional Chinese text conversion.
 Home-page: https://github.com/danny0838/sts-lib
 Author: Danny Lin
 Author-email: danny0838@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
@@ -149,37 +149,39 @@
  * @property {string} [mode=load] - the mode to handle the loaded dicts.
  *     - "load" to simply merge the loaded keys and values;
  *     - "swap" to reverse the dict (i.e. use the values as keys and the keys
  *       as values);
  *     - "join" to chain dicts (a conversion using a dict joining dict1 and
  *       dict2 works like a conversion using dict1 and then dict2, but takes
  *       care of word segmentation);
- *     - "filter" to filter the output values in the loaded dicts with extra
- *       "include" and "exclude" properties
  *     - "expand" to expand the placeholders (defined in the extra
  *       "placeholders" property) in the first dict with the matching key and
  *        values in other dicts;
- *     - "remove_keys" to remove keys from the first dict if it appears in any
- *       other one;
- *     - "remove_values" to remove key-value pairs from the first dict if it
- *       appears in any other one.
+ *     - "filter" to filter the output keys and values in the loaded dicts
+ *       using extra "method", "include", and "exclude" properties.
  * @property {srcDictScheme[]} [src] - the source dicts. `file` must exist when
  *     omitted.
  * @property {boolean} [sort] - true to sort the keys of the output dictionary.
  * @property {boolean} [check] - true to raise an exception if the output
  *     contains an invalid char which will be loaded incorrectly. Set this
  *     when the output is a plain text table file and the source files contain
  *     untrusted JSON or YAML data that may include a char like " ", "\t",
  *     "\n", etc. in the dictionary.
+ * @property {string[]} [placeholders] - strings to be expanded using other
+ *     dicts. (for "expand" mode)
+ * @property {string} [method=remove_key_values] - how to filter (for "filter"
+ *     mode)
+ *     - "remove_keys" to remove keys from the first dict if it appears in any
+ *       other one;
+ *     - "remove_key_values" to remove key-value pairs from the first dict if it
+ *       appears in any other one.
  * @property {string} [include] - a regex filter that discards non-matched
  *     conversion values. (for "filter" mode)
  * @property {string} [exclude] - a regex filter that discards matched
  *     conversion values. (for "filter" mode)
- * @property {string[]} [placeholders] - strings to be expanded using other
- *     dicts. (for "expand" mode)
  */
 ```
 
 ### Dictionary 詞典檔
 
 原始詞典檔可為純文字、JSON、或 YAML。編譯產生的詞典檔有純文字（`.list`）、JSON列表（`.jlist`）、JSON樹（`.tlist`）三種格式，其中前二者可再作為原始檔輸入，後者則只能用於轉換。
```

