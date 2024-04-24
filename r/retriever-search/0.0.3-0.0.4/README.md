# Comparing `tmp/retriever_search-0.0.3.tar.gz` & `tmp/retriever_search-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retriever_search-0.0.3.tar", last modified: Wed Apr 24 08:37:46 2024, max compression
+gzip compressed data, was "retriever_search-0.0.4.tar", last modified: Wed Apr 24 08:58:45 2024, max compression
```

## Comparing `retriever_search-0.0.3.tar` & `retriever_search-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-04-24 08:37:46.593261 retriever_search-0.0.3/
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1062 2024-04-23 05:51:14.000000 retriever_search-0.0.3/LICENSE
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      549 2024-04-24 08:37:46.592550 retriever_search-0.0.3/PKG-INFO
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      389 2024-04-24 08:17:21.000000 retriever_search-0.0.3/README.md
-drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-04-24 08:37:46.591863 retriever_search-0.0.3/retriever_search.egg-info/
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      549 2024-04-24 08:37:46.000000 retriever_search-0.0.3/retriever_search.egg-info/PKG-INFO
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      225 2024-04-24 08:37:46.000000 retriever_search-0.0.3/retriever_search.egg-info/SOURCES.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)        1 2024-04-24 08:37:46.000000 retriever_search-0.0.3/retriever_search.egg-info/dependency_links.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      191 2024-04-24 08:37:46.000000 retriever_search-0.0.3/retriever_search.egg-info/requires.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)       17 2024-04-24 08:37:46.000000 retriever_search-0.0.3/retriever_search.egg-info/top_level.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)       38 2024-04-24 08:37:46.593477 retriever_search-0.0.3/setup.cfg
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      641 2024-04-24 08:32:32.000000 retriever_search-0.0.3/setup.py
+drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-04-24 08:58:45.012519 retriever_search-0.0.4/
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1062 2024-04-23 05:51:14.000000 retriever_search-0.0.4/LICENSE
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      549 2024-04-24 08:58:45.012148 retriever_search-0.0.4/PKG-INFO
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      409 2024-04-24 08:54:46.000000 retriever_search-0.0.4/README.md
+drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-04-24 08:58:45.011700 retriever_search-0.0.4/retriever_search.egg-info/
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      549 2024-04-24 08:58:44.000000 retriever_search-0.0.4/retriever_search.egg-info/PKG-INFO
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      225 2024-04-24 08:58:44.000000 retriever_search-0.0.4/retriever_search.egg-info/SOURCES.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)        1 2024-04-24 08:58:44.000000 retriever_search-0.0.4/retriever_search.egg-info/dependency_links.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      191 2024-04-24 08:58:44.000000 retriever_search-0.0.4/retriever_search.egg-info/requires.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)       17 2024-04-24 08:58:44.000000 retriever_search-0.0.4/retriever_search.egg-info/top_level.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)       38 2024-04-24 08:58:45.012602 retriever_search-0.0.4/setup.cfg
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      641 2024-04-24 08:32:32.000000 retriever_search-0.0.4/setup.py
```

### Comparing `retriever_search-0.0.3/LICENSE` & `retriever_search-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `retriever_search-0.0.3/PKG-INFO` & `retriever_search-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retriever_search
-Version: 0.0.3
+Version: 0.0.4
 Home-page: https://github.com/GovML/retriever.git
 Author: Sidharth Kathpal
 Author-email: kathpal.sid@gmail.com
 License-File: LICENSE
 Requires-Dist: haystack-ai==2.0.0
 Requires-Dist: pymupdf==1.22.5
 Requires-Dist: sentence-transformers==2.5.1
```

### Comparing `retriever_search-0.0.3/retriever_search.egg-info/PKG-INFO` & `retriever_search-0.0.4/retriever_search.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retriever_search
-Version: 0.0.3
+Version: 0.0.4
 Home-page: https://github.com/GovML/retriever.git
 Author: Sidharth Kathpal
 Author-email: kathpal.sid@gmail.com
 License-File: LICENSE
 Requires-Dist: haystack-ai==2.0.0
 Requires-Dist: pymupdf==1.22.5
 Requires-Dist: sentence-transformers==2.5.1
```

### Comparing `retriever_search-0.0.3/setup.py` & `retriever_search-0.0.4/setup.py`

 * *Files identical despite different names*

