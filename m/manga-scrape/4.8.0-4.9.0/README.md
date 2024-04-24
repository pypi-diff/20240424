# Comparing `tmp/manga_scrape-4.8.0.tar.gz` & `tmp/manga_scrape-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manga_scrape-4.8.0.tar", last modified: Thu Apr  4 03:21:13 2024, max compression
+gzip compressed data, was "manga_scrape-4.9.0.tar", last modified: Thu Apr  4 03:39:03 2024, max compression
```

## Comparing `manga_scrape-4.8.0.tar` & `manga_scrape-4.9.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:21:13.824872 manga_scrape-4.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-04 03:21:08.000000 manga_scrape-4.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-04 03:21:13.824872 manga_scrape-4.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-04 03:21:08.000000 manga_scrape-4.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:21:13.820872 manga_scrape-4.8.0/manga/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 03:21:08.000000 manga_scrape-4.8.0/manga/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 03:21:08.000000 manga_scrape-4.8.0/manga/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:21:13.820872 manga_scrape-4.8.0/manga/sites/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-04 03:21:08.000000 manga_scrape-4.8.0/manga/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-04 03:21:08.000000 manga_scrape-4.8.0/manga/sites/domains.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-04 03:21:08.000000 manga_scrape-4.8.0/manga/sites/test.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-04 03:21:08.000000 manga_scrape-4.8.0/manga/sites/unknown_domain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:21:13.824872 manga_scrape-4.8.0/manga/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-04 03:21:08.000000 manga_scrape-4.8.0/manga/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11821 2024-04-04 03:21:08.000000 manga_scrape-4.8.0/manga/tools/guess.py
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-04 03:21:08.000000 manga_scrape-4.8.0/manga/tools/inc_chapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-04 03:21:08.000000 manga_scrape-4.8.0/manga/tools/no_unicode.py
--rw-r--r--   0 runner    (1001) docker     (127)     5603 2024-04-04 03:21:08.000000 manga_scrape-4.8.0/manga/tools/open_new.py
--rw-r--r--   0 runner    (1001) docker     (127)     9457 2024-04-04 03:21:08.000000 manga_scrape-4.8.0/manga/tools/test_sites.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-04 03:21:08.000000 manga_scrape-4.8.0/manga/tools/unnumbered_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-04 03:21:08.000000 manga_scrape-4.8.0/manga/tools/up_number.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:21:13.824872 manga_scrape-4.8.0/manga/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-04 03:21:08.000000 manga_scrape-4.8.0/manga/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-04 03:21:08.000000 manga_scrape-4.8.0/manga/utils/extract_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-04 03:21:08.000000 manga_scrape-4.8.0/manga/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-04 03:21:08.000000 manga_scrape-4.8.0/manga/utils/split_on_num.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:21:13.824872 manga_scrape-4.8.0/manga_scrape.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-04 03:21:13.000000 manga_scrape-4.8.0/manga_scrape.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-04 03:21:13.000000 manga_scrape-4.8.0/manga_scrape.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 03:21:13.000000 manga_scrape-4.8.0/manga_scrape.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-04 03:21:13.000000 manga_scrape-4.8.0/manga_scrape.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-04 03:21:13.000000 manga_scrape-4.8.0/manga_scrape.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-04 03:21:13.000000 manga_scrape-4.8.0/manga_scrape.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-04 03:21:08.000000 manga_scrape-4.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 03:21:13.824872 manga_scrape-4.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:39:03.713518 manga_scrape-4.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-04 03:39:00.000000 manga_scrape-4.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-04 03:39:03.713518 manga_scrape-4.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-04 03:39:00.000000 manga_scrape-4.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:39:03.709519 manga_scrape-4.9.0/manga/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 03:39:00.000000 manga_scrape-4.9.0/manga/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 03:39:00.000000 manga_scrape-4.9.0/manga/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:39:03.709519 manga_scrape-4.9.0/manga/sites/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-04 03:39:00.000000 manga_scrape-4.9.0/manga/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-04-04 03:39:00.000000 manga_scrape-4.9.0/manga/sites/domains.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-04 03:39:00.000000 manga_scrape-4.9.0/manga/sites/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-04 03:39:00.000000 manga_scrape-4.9.0/manga/sites/unknown_domain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:39:03.709519 manga_scrape-4.9.0/manga/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-04 03:39:00.000000 manga_scrape-4.9.0/manga/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11821 2024-04-04 03:39:00.000000 manga_scrape-4.9.0/manga/tools/guess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-04 03:39:00.000000 manga_scrape-4.9.0/manga/tools/inc_chapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-04 03:39:00.000000 manga_scrape-4.9.0/manga/tools/no_unicode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5603 2024-04-04 03:39:00.000000 manga_scrape-4.9.0/manga/tools/open_new.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9457 2024-04-04 03:39:00.000000 manga_scrape-4.9.0/manga/tools/test_sites.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-04 03:39:00.000000 manga_scrape-4.9.0/manga/tools/unnumbered_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-04 03:39:00.000000 manga_scrape-4.9.0/manga/tools/up_number.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:39:03.713518 manga_scrape-4.9.0/manga/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-04 03:39:00.000000 manga_scrape-4.9.0/manga/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-04 03:39:00.000000 manga_scrape-4.9.0/manga/utils/extract_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-04 03:39:00.000000 manga_scrape-4.9.0/manga/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-04 03:39:00.000000 manga_scrape-4.9.0/manga/utils/split_on_num.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:39:03.713518 manga_scrape-4.9.0/manga_scrape.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-04 03:39:03.000000 manga_scrape-4.9.0/manga_scrape.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-04 03:39:03.000000 manga_scrape-4.9.0/manga_scrape.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 03:39:03.000000 manga_scrape-4.9.0/manga_scrape.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-04 03:39:03.000000 manga_scrape-4.9.0/manga_scrape.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-04 03:39:03.000000 manga_scrape-4.9.0/manga_scrape.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-04 03:39:03.000000 manga_scrape-4.9.0/manga_scrape.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-04 03:39:00.000000 manga_scrape-4.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 03:39:03.713518 manga_scrape-4.9.0/setup.cfg
```

### Comparing `manga_scrape-4.8.0/LICENSE` & `manga_scrape-4.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `manga_scrape-4.8.0/PKG-INFO` & `manga_scrape-4.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manga_scrape
-Version: 4.8.0
+Version: 4.9.0
 Summary: A python package used for automating finding manga chapters
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/zwimer/manga
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
```

### Comparing `manga_scrape-4.8.0/manga/sites/domains.py` & `manga_scrape-4.9.0/manga/sites/domains.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,14 +82,22 @@
     return "cursorNext" in data and "Alternative" not in data
 
 
 def manhuascan_com(data: str) -> bool:
     return "loadchapter" in data and "chapterNumber = null" not in data
 
 
+def manhuafast_com(data: str) -> bool:
+    return "backInfoPage" in data and "Read Last" not in data
+
+
+def manhuafast_net(data: str) -> bool:
+    return "prev_page" in data and "Read Last" not in data
+
+
 def manhuaus_org(data: str) -> bool:
     return "prev_page" in data and "main-menu" not in data
 
 
 def manhwatop_com(data: str) -> bool:
     return "loader.svg" in data and "Show more" not in data
 
@@ -123,11 +131,13 @@
     "mangakakalots.net": mangakakalots_com,
     #
     "readmanganato.com": chapmanganato_com,
     "chapmanganato.com": chapmanganato_com,
     "chapmanganato.to": chapmanganato_to,
     #
     "manhuascan.com": manhuascan_com,
+    "manhuafast.com": manhuafast_com,
+    "manhuafast.net": manhuafast_net,
     "manhuaus.org": manhuaus_org,
     "manhwatop.com": manhwatop_com,
     "zinmanga.com": zinmanga_com,
 }
```

### Comparing `manga_scrape-4.8.0/manga/sites/test.py` & `manga_scrape-4.9.0/manga/sites/test.py`

 * *Files identical despite different names*

### Comparing `manga_scrape-4.8.0/manga/tools/guess.py` & `manga_scrape-4.9.0/manga/tools/guess.py`

 * *Files identical despite different names*

### Comparing `manga_scrape-4.8.0/manga/tools/inc_chapter.py` & `manga_scrape-4.9.0/manga/tools/inc_chapter.py`

 * *Files identical despite different names*

### Comparing `manga_scrape-4.8.0/manga/tools/no_unicode.py` & `manga_scrape-4.9.0/manga/tools/no_unicode.py`

 * *Files identical despite different names*

### Comparing `manga_scrape-4.8.0/manga/tools/open_new.py` & `manga_scrape-4.9.0/manga/tools/open_new.py`

 * *Files identical despite different names*

### Comparing `manga_scrape-4.8.0/manga/tools/test_sites.py` & `manga_scrape-4.9.0/manga/tools/test_sites.py`

 * *Files identical despite different names*

### Comparing `manga_scrape-4.8.0/manga/tools/unnumbered_helper.py` & `manga_scrape-4.9.0/manga/tools/unnumbered_helper.py`

 * *Files identical despite different names*

### Comparing `manga_scrape-4.8.0/manga/tools/up_number.py` & `manga_scrape-4.9.0/manga/tools/up_number.py`

 * *Files identical despite different names*

### Comparing `manga_scrape-4.8.0/manga/utils/extract_url.py` & `manga_scrape-4.9.0/manga/utils/extract_url.py`

 * *Files identical despite different names*

### Comparing `manga_scrape-4.8.0/manga/utils/files.py` & `manga_scrape-4.9.0/manga/utils/files.py`

 * *Files identical despite different names*

### Comparing `manga_scrape-4.8.0/manga/utils/split_on_num.py` & `manga_scrape-4.9.0/manga/utils/split_on_num.py`

 * *Files identical despite different names*

### Comparing `manga_scrape-4.8.0/manga_scrape.egg-info/PKG-INFO` & `manga_scrape-4.9.0/manga_scrape.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manga_scrape
-Version: 4.8.0
+Version: 4.9.0
 Summary: A python package used for automating finding manga chapters
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/zwimer/manga
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
```

### Comparing `manga_scrape-4.8.0/manga_scrape.egg-info/SOURCES.txt` & `manga_scrape-4.9.0/manga_scrape.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `manga_scrape-4.8.0/pyproject.toml` & `manga_scrape-4.9.0/pyproject.toml`

 * *Files identical despite different names*

