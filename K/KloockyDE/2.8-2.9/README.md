# Comparing `tmp/KloockyDE-2.8.tar.gz` & `tmp/KloockyDE-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KloockyDE-2.8.tar", last modified: Sat Feb 24 16:29:46 2024, max compression
+gzip compressed data, was "KloockyDE-2.9.tar", last modified: Wed Apr 24 10:56:26 2024, max compression
```

## Comparing `KloockyDE-2.8.tar` & `KloockyDE-2.9.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-02-24 16:29:46.420388 KloockyDE-2.8/
--rw-rw-rw-   0        0        0      221 2024-02-24 16:29:46.421388 KloockyDE-2.8/PKG-INFO
--rw-rw-rw-   0        0        0       78 2022-07-27 10:14:02.000000 KloockyDE-2.8/README.rst
--rw-rw-rw-   0        0        0      115 2024-02-24 16:29:46.421388 KloockyDE-2.8/setup.cfg
--rw-rw-rw-   0        0        0      404 2024-02-24 16:29:06.000000 KloockyDE-2.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-24 16:29:46.378388 KloockyDE-2.8/src/
-drwxrwxrwx   0        0        0        0 2024-02-24 16:29:46.395388 KloockyDE-2.8/src/KloockyDE/
-drwxrwxrwx   0        0        0        0 2024-02-24 16:29:46.401388 KloockyDE-2.8/src/KloockyDE/Algorithms/
-drwxrwxrwx   0        0        0        0 2024-02-24 16:29:46.408388 KloockyDE-2.8/src/KloockyDE/Algorithms/Search/
--rw-rw-rw-   0        0        0        0 2024-02-23 17:08:53.000000 KloockyDE-2.8/src/KloockyDE/Algorithms/Search/__init__.py
--rw-rw-rw-   0        0        0      995 2021-05-12 12:29:10.000000 KloockyDE-2.8/src/KloockyDE/Algorithms/Search/binarysearch.py
--rw-rw-rw-   0        0        0      604 2021-05-12 12:29:10.000000 KloockyDE-2.8/src/KloockyDE/Algorithms/Search/linearsearch.py
--rw-rw-rw-   0        0        0     1254 2021-05-12 12:29:10.000000 KloockyDE-2.8/src/KloockyDE/Algorithms/Search/min_max_search.py
-drwxrwxrwx   0        0        0        0 2024-02-24 16:29:46.416387 KloockyDE-2.8/src/KloockyDE/Algorithms/Sort/
--rw-rw-rw-   0        0        0        0 2024-02-23 17:08:46.000000 KloockyDE-2.8/src/KloockyDE/Algorithms/Sort/__init__.py
--rw-rw-rw-   0        0        0      953 2021-05-12 12:29:10.000000 KloockyDE-2.8/src/KloockyDE/Algorithms/Sort/bubblesort.py
--rw-rw-rw-   0        0        0     1370 2021-05-13 23:33:10.000000 KloockyDE-2.8/src/KloockyDE/Algorithms/Sort/heapsort.py
--rw-rw-rw-   0        0        0     1617 2021-05-12 12:29:10.000000 KloockyDE-2.8/src/KloockyDE/Algorithms/Sort/max_min_sort.py
--rw-rw-rw-   0        0        0     1340 2024-02-23 15:57:17.000000 KloockyDE-2.8/src/KloockyDE/Algorithms/Sort/quicksort.py
--rw-rw-rw-   0        0        0        0 2024-02-23 17:08:29.000000 KloockyDE-2.8/src/KloockyDE/Algorithms/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-24 16:29:46.419388 KloockyDE-2.8/src/KloockyDE/Extras/
--rw-rw-rw-   0        0        0        0 2024-02-23 17:09:02.000000 KloockyDE-2.8/src/KloockyDE/Extras/__init__.py
--rw-rw-rw-   0        0        0     9565 2024-02-23 15:49:00.000000 KloockyDE-2.8/src/KloockyDE/Extras/decode_ASCII.py
--rw-rw-rw-   0        0        0      557 2024-02-23 15:57:17.000000 KloockyDE-2.8/src/KloockyDE/ListsAndStrings.py
--rw-rw-rw-   0        0        0      743 2024-02-24 16:29:06.000000 KloockyDE-2.8/src/KloockyDE/__init__.py
--rw-rw-rw-   0        0        0    11189 2024-02-24 16:29:06.000000 KloockyDE-2.8/src/KloockyDE/filestuff.py
--rw-rw-rw-   0        0        0     2171 2024-02-24 16:29:06.000000 KloockyDE-2.8/src/KloockyDE/helpers.py
--rw-rw-rw-   0        0        0     1489 2024-02-23 15:57:17.000000 KloockyDE-2.8/src/KloockyDE/numberstuff.py
--rw-rw-rw-   0        0        0     2205 2024-02-23 16:56:22.000000 KloockyDE-2.8/src/KloockyDE/timestuff.py
-drwxrwxrwx   0        0        0        0 2024-02-24 16:29:46.400388 KloockyDE-2.8/src/KloockyDE.egg-info/
--rw-rw-rw-   0        0        0      221 2024-02-24 16:29:46.000000 KloockyDE-2.8/src/KloockyDE.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      894 2024-02-24 16:29:46.000000 KloockyDE-2.8/src/KloockyDE.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-24 16:29:46.000000 KloockyDE-2.8/src/KloockyDE.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-02-24 16:29:46.000000 KloockyDE-2.8/src/KloockyDE.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-02-24 16:29:46.000000 KloockyDE-2.8/src/KloockyDE.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 10:56:26.114933 KloockyDE-2.9/
+-rw-rw-rw-   0        0        0       93 2024-04-24 10:55:45.000000 KloockyDE-2.9/LICENSE.rst
+-rw-rw-rw-   0        0        0      248 2024-04-24 10:56:26.115898 KloockyDE-2.9/PKG-INFO
+-rw-rw-rw-   0        0        0      206 2024-04-24 10:55:10.000000 KloockyDE-2.9/README.rst
+-rw-rw-rw-   0        0        0      115 2024-04-24 10:56:26.115898 KloockyDE-2.9/setup.cfg
+-rw-rw-rw-   0        0        0      404 2024-04-24 10:50:35.000000 KloockyDE-2.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 10:56:26.072899 KloockyDE-2.9/src/
+drwxrwxrwx   0        0        0        0 2024-04-24 10:56:26.090899 KloockyDE-2.9/src/KloockyDE/
+drwxrwxrwx   0        0        0        0 2024-04-24 10:56:26.096923 KloockyDE-2.9/src/KloockyDE/Algorithms/
+drwxrwxrwx   0        0        0        0 2024-04-24 10:56:26.102928 KloockyDE-2.9/src/KloockyDE/Algorithms/Search/
+-rw-rw-rw-   0        0        0        0 2024-02-23 17:08:53.000000 KloockyDE-2.9/src/KloockyDE/Algorithms/Search/__init__.py
+-rw-rw-rw-   0        0        0      995 2021-05-12 12:29:10.000000 KloockyDE-2.9/src/KloockyDE/Algorithms/Search/binarysearch.py
+-rw-rw-rw-   0        0        0      604 2021-05-12 12:29:10.000000 KloockyDE-2.9/src/KloockyDE/Algorithms/Search/linearsearch.py
+-rw-rw-rw-   0        0        0     1254 2021-05-12 12:29:10.000000 KloockyDE-2.9/src/KloockyDE/Algorithms/Search/min_max_search.py
+drwxrwxrwx   0        0        0        0 2024-04-24 10:56:26.110930 KloockyDE-2.9/src/KloockyDE/Algorithms/Sort/
+-rw-rw-rw-   0        0        0        0 2024-02-23 17:08:46.000000 KloockyDE-2.9/src/KloockyDE/Algorithms/Sort/__init__.py
+-rw-rw-rw-   0        0        0      953 2021-05-12 12:29:10.000000 KloockyDE-2.9/src/KloockyDE/Algorithms/Sort/bubblesort.py
+-rw-rw-rw-   0        0        0     1370 2021-05-13 23:33:10.000000 KloockyDE-2.9/src/KloockyDE/Algorithms/Sort/heapsort.py
+-rw-rw-rw-   0        0        0     1617 2021-05-12 12:29:10.000000 KloockyDE-2.9/src/KloockyDE/Algorithms/Sort/max_min_sort.py
+-rw-rw-rw-   0        0        0     1340 2024-02-23 15:57:17.000000 KloockyDE-2.9/src/KloockyDE/Algorithms/Sort/quicksort.py
+-rw-rw-rw-   0        0        0        0 2024-02-23 17:08:29.000000 KloockyDE-2.9/src/KloockyDE/Algorithms/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 10:56:26.113896 KloockyDE-2.9/src/KloockyDE/Extras/
+-rw-rw-rw-   0        0        0        0 2024-02-23 17:09:02.000000 KloockyDE-2.9/src/KloockyDE/Extras/__init__.py
+-rw-rw-rw-   0        0        0     9565 2024-02-23 15:49:00.000000 KloockyDE-2.9/src/KloockyDE/Extras/decode_ASCII.py
+-rw-rw-rw-   0        0        0      557 2024-02-23 15:57:17.000000 KloockyDE-2.9/src/KloockyDE/ListsAndStrings.py
+-rw-rw-rw-   0        0        0      299 2024-04-24 10:50:35.000000 KloockyDE-2.9/src/KloockyDE/SafetySwitch.py
+-rw-rw-rw-   0        0        0      779 2024-04-24 10:50:35.000000 KloockyDE-2.9/src/KloockyDE/__init__.py
+-rw-rw-rw-   0        0        0    11189 2024-02-24 16:29:06.000000 KloockyDE-2.9/src/KloockyDE/filestuff.py
+-rw-rw-rw-   0        0        0     2171 2024-02-24 16:29:06.000000 KloockyDE-2.9/src/KloockyDE/helpers.py
+-rw-rw-rw-   0        0        0     1489 2024-02-23 15:57:17.000000 KloockyDE-2.9/src/KloockyDE/numberstuff.py
+-rw-rw-rw-   0        0        0     2205 2024-02-23 16:56:22.000000 KloockyDE-2.9/src/KloockyDE/timestuff.py
+drwxrwxrwx   0        0        0        0 2024-04-24 10:56:26.095929 KloockyDE-2.9/src/KloockyDE.egg-info/
+-rw-rw-rw-   0        0        0      248 2024-04-24 10:56:25.000000 KloockyDE-2.9/src/KloockyDE.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      936 2024-04-24 10:56:25.000000 KloockyDE-2.9/src/KloockyDE.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 10:56:25.000000 KloockyDE-2.9/src/KloockyDE.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-04-24 10:56:25.000000 KloockyDE-2.9/src/KloockyDE.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-24 10:56:25.000000 KloockyDE-2.9/src/KloockyDE.egg-info/top_level.txt
```

### Comparing `KloockyDE-2.8/src/KloockyDE/Algorithms/Search/binarysearch.py` & `KloockyDE-2.9/src/KloockyDE/Algorithms/Search/binarysearch.py`

 * *Files identical despite different names*

### Comparing `KloockyDE-2.8/src/KloockyDE/Algorithms/Search/linearsearch.py` & `KloockyDE-2.9/src/KloockyDE/Algorithms/Search/linearsearch.py`

 * *Files identical despite different names*

### Comparing `KloockyDE-2.8/src/KloockyDE/Algorithms/Search/min_max_search.py` & `KloockyDE-2.9/src/KloockyDE/Algorithms/Search/min_max_search.py`

 * *Files identical despite different names*

### Comparing `KloockyDE-2.8/src/KloockyDE/Algorithms/Sort/bubblesort.py` & `KloockyDE-2.9/src/KloockyDE/Algorithms/Sort/bubblesort.py`

 * *Files identical despite different names*

### Comparing `KloockyDE-2.8/src/KloockyDE/Algorithms/Sort/heapsort.py` & `KloockyDE-2.9/src/KloockyDE/Algorithms/Sort/heapsort.py`

 * *Files identical despite different names*

### Comparing `KloockyDE-2.8/src/KloockyDE/Algorithms/Sort/max_min_sort.py` & `KloockyDE-2.9/src/KloockyDE/Algorithms/Sort/max_min_sort.py`

 * *Files identical despite different names*

### Comparing `KloockyDE-2.8/src/KloockyDE/Algorithms/Sort/quicksort.py` & `KloockyDE-2.9/src/KloockyDE/Algorithms/Sort/quicksort.py`

 * *Files identical despite different names*

### Comparing `KloockyDE-2.8/src/KloockyDE/Extras/decode_ASCII.py` & `KloockyDE-2.9/src/KloockyDE/Extras/decode_ASCII.py`

 * *Files identical despite different names*

### Comparing `KloockyDE-2.8/src/KloockyDE/ListsAndStrings.py` & `KloockyDE-2.9/src/KloockyDE/ListsAndStrings.py`

 * *Files identical despite different names*

### Comparing `KloockyDE-2.8/src/KloockyDE/__init__.py` & `KloockyDE-2.9/src/KloockyDE/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,7 +9,9 @@
 # 2.5 fixed that
 # 2.6 - I forgot to put everything into packages for all previous 2.x versions. Fixed that
 # 2.7 Same as before, my fix did not work for some reason
 # 2.8
 #   Added some functions to filestuff for working with paths
 #   Added helpers file for small useful functions
 #   Added functions to helpers for replacing/removing multiple substrings in one command
+# 2.9
+#   Added SafetySwitch file
```

### Comparing `KloockyDE-2.8/src/KloockyDE/filestuff.py` & `KloockyDE-2.9/src/KloockyDE/filestuff.py`

 * *Files identical despite different names*

### Comparing `KloockyDE-2.8/src/KloockyDE/helpers.py` & `KloockyDE-2.9/src/KloockyDE/helpers.py`

 * *Files identical despite different names*

### Comparing `KloockyDE-2.8/src/KloockyDE/numberstuff.py` & `KloockyDE-2.9/src/KloockyDE/numberstuff.py`

 * *Files identical despite different names*

### Comparing `KloockyDE-2.8/src/KloockyDE/timestuff.py` & `KloockyDE-2.9/src/KloockyDE/timestuff.py`

 * *Files identical despite different names*

### Comparing `KloockyDE-2.8/src/KloockyDE.egg-info/SOURCES.txt` & `KloockyDE-2.9/src/KloockyDE.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+LICENSE.rst
 README.rst
 setup.cfg
 setup.py
 src/KloockyDE/ListsAndStrings.py
+src/KloockyDE/SafetySwitch.py
 src/KloockyDE/__init__.py
 src/KloockyDE/filestuff.py
 src/KloockyDE/helpers.py
 src/KloockyDE/numberstuff.py
 src/KloockyDE/timestuff.py
 src/KloockyDE.egg-info/PKG-INFO
 src/KloockyDE.egg-info/SOURCES.txt
```

