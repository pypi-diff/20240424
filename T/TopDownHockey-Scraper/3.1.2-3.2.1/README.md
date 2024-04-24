# Comparing `tmp/TopDownHockey_Scraper-3.1.2.tar.gz` & `tmp/topdownhockey_scraper-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TopDownHockey_Scraper-3.1.2.tar", last modified: Thu Jan  4 04:05:14 2024, max compression
+gzip compressed data, was "topdownhockey_scraper-3.2.1.tar", last modified: Wed Apr 24 03:40:03 2024, max compression
```

## Comparing `TopDownHockey_Scraper-3.1.2.tar` & `topdownhockey_scraper-3.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 patrickbacon   (501) staff       (20)        0 2024-01-04 04:05:14.887509 TopDownHockey_Scraper-3.1.2/
--rw-rw-r--   0 patrickbacon   (501) staff       (20)     1073 2021-10-23 01:32:32.000000 TopDownHockey_Scraper-3.1.2/LICENSE
--rw-r--r--   0 patrickbacon   (501) staff       (20)     5462 2024-01-04 04:05:14.887444 TopDownHockey_Scraper-3.1.2/PKG-INFO
--rw-rw-r--   0 patrickbacon   (501) staff       (20)     4697 2023-11-09 21:19:28.000000 TopDownHockey_Scraper-3.1.2/README.md
--rw-rw-r--   0 patrickbacon   (501) staff       (20)      103 2021-10-23 01:32:32.000000 TopDownHockey_Scraper-3.1.2/pyproject.toml
--rw-rw-r--   0 patrickbacon   (501) staff       (20)      892 2024-01-04 04:05:14.887786 TopDownHockey_Scraper-3.1.2/setup.cfg
--rw-rw-r--   0 patrickbacon   (501) staff       (20)     1191 2024-01-04 04:05:00.000000 TopDownHockey_Scraper-3.1.2/setup.py
-drwxr-xr-x   0 patrickbacon   (501) staff       (20)        0 2024-01-04 04:05:14.885755 TopDownHockey_Scraper-3.1.2/src/
-drwxr-xr-x   0 patrickbacon   (501) staff       (20)        0 2024-01-04 04:05:14.886455 TopDownHockey_Scraper-3.1.2/src/TopDownHockey_Scraper/
--rw-rw-r--   0 patrickbacon   (501) staff       (20)    45380 2023-10-04 05:55:32.000000 TopDownHockey_Scraper-3.1.2/src/TopDownHockey_Scraper/TopDownHockey_EliteProspects_Scraper.py
--rw-rw-r--   0 patrickbacon   (501) staff       (20)   148401 2024-01-04 04:04:34.000000 TopDownHockey_Scraper-3.1.2/src/TopDownHockey_Scraper/TopDownHockey_NHL_Scraper.py
-drwxr-xr-x   0 patrickbacon   (501) staff       (20)        0 2024-01-04 04:05:14.887260 TopDownHockey_Scraper-3.1.2/src/TopDownHockey_Scraper.egg-info/
--rw-r--r--   0 patrickbacon   (501) staff       (20)     5462 2024-01-04 04:05:14.000000 TopDownHockey_Scraper-3.1.2/src/TopDownHockey_Scraper.egg-info/PKG-INFO
--rw-r--r--   0 patrickbacon   (501) staff       (20)      416 2024-01-04 04:05:14.000000 TopDownHockey_Scraper-3.1.2/src/TopDownHockey_Scraper.egg-info/SOURCES.txt
--rw-r--r--   0 patrickbacon   (501) staff       (20)        1 2024-01-04 04:05:14.000000 TopDownHockey_Scraper-3.1.2/src/TopDownHockey_Scraper.egg-info/dependency_links.txt
--rw-r--r--   0 patrickbacon   (501) staff       (20)       68 2024-01-04 04:05:14.000000 TopDownHockey_Scraper-3.1.2/src/TopDownHockey_Scraper.egg-info/requires.txt
--rw-r--r--   0 patrickbacon   (501) staff       (20)       22 2024-01-04 04:05:14.000000 TopDownHockey_Scraper-3.1.2/src/TopDownHockey_Scraper.egg-info/top_level.txt
+drwxr-xr-x   0 patrickbacon   (501) staff       (20)        0 2024-04-24 03:40:03.500409 topdownhockey_scraper-3.2.1/
+-rw-rw-r--   0 patrickbacon   (501) staff       (20)     1073 2021-10-23 01:32:32.000000 topdownhockey_scraper-3.2.1/LICENSE
+-rw-r--r--   0 patrickbacon   (501) staff       (20)     5462 2024-04-24 03:40:03.500352 topdownhockey_scraper-3.2.1/PKG-INFO
+-rw-rw-r--   0 patrickbacon   (501) staff       (20)     4697 2023-11-09 21:19:28.000000 topdownhockey_scraper-3.2.1/README.md
+-rw-rw-r--   0 patrickbacon   (501) staff       (20)      103 2021-10-23 01:32:32.000000 topdownhockey_scraper-3.2.1/pyproject.toml
+-rw-rw-r--   0 patrickbacon   (501) staff       (20)      892 2024-04-24 03:40:03.500675 topdownhockey_scraper-3.2.1/setup.cfg
+-rw-rw-r--   0 patrickbacon   (501) staff       (20)     1191 2024-04-24 03:39:43.000000 topdownhockey_scraper-3.2.1/setup.py
+drwxr-xr-x   0 patrickbacon   (501) staff       (20)        0 2024-04-24 03:40:03.497179 topdownhockey_scraper-3.2.1/src/
+drwxr-xr-x   0 patrickbacon   (501) staff       (20)        0 2024-04-24 03:40:03.498578 topdownhockey_scraper-3.2.1/src/TopDownHockey_Scraper/
+-rw-rw-r--   0 patrickbacon   (501) staff       (20)    45380 2023-10-04 05:55:32.000000 topdownhockey_scraper-3.2.1/src/TopDownHockey_Scraper/TopDownHockey_EliteProspects_Scraper.py
+-rw-rw-r--   0 patrickbacon   (501) staff       (20)   148401 2024-01-04 04:04:34.000000 topdownhockey_scraper-3.2.1/src/TopDownHockey_Scraper/TopDownHockey_NHL_Scraper.py
+drwxr-xr-x   0 patrickbacon   (501) staff       (20)        0 2024-04-24 03:40:03.499966 topdownhockey_scraper-3.2.1/src/TopDownHockey_Scraper.egg-info/
+-rw-r--r--   0 patrickbacon   (501) staff       (20)     5462 2024-04-24 03:40:03.000000 topdownhockey_scraper-3.2.1/src/TopDownHockey_Scraper.egg-info/PKG-INFO
+-rw-r--r--   0 patrickbacon   (501) staff       (20)      416 2024-04-24 03:40:03.000000 topdownhockey_scraper-3.2.1/src/TopDownHockey_Scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 patrickbacon   (501) staff       (20)        1 2024-04-24 03:40:03.000000 topdownhockey_scraper-3.2.1/src/TopDownHockey_Scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 patrickbacon   (501) staff       (20)       68 2024-04-24 03:40:03.000000 topdownhockey_scraper-3.2.1/src/TopDownHockey_Scraper.egg-info/requires.txt
+-rw-r--r--   0 patrickbacon   (501) staff       (20)       22 2024-04-24 03:40:03.000000 topdownhockey_scraper-3.2.1/src/TopDownHockey_Scraper.egg-info/top_level.txt
```

### Comparing `TopDownHockey_Scraper-3.1.2/LICENSE` & `topdownhockey_scraper-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `TopDownHockey_Scraper-3.1.2/PKG-INFO` & `topdownhockey_scraper-3.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TopDownHockey_Scraper
-Version: 3.1.2
+Version: 3.2.1
 Summary: The TopDownHockey Scraper
 Home-page: https://github.com/TopDownHockey/TopDownHockey_Scraper
 Author: Patrick Bacon
 Author-email: patrick.s.bacon@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/TopDownHockey/TopDownHockey_Scraper/issues
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: TopDownHockey_Scraper Version: 3.1.2 Summary: The
+Metadata-Version: 2.1 Name: TopDownHockey_Scraper Version: 3.2.1 Summary: The
 TopDownHockey Scraper Home-page: https://github.com/TopDownHockey/
 TopDownHockey_Scraper Author: Patrick Bacon Author-email:
 patrick.s.bacon@gmail.com License: MIT Project-URL: Bug Tracker, https://
 github.com/TopDownHockey/TopDownHockey_Scraper/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
```

### Comparing `TopDownHockey_Scraper-3.1.2/README.md` & `topdownhockey_scraper-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `TopDownHockey_Scraper-3.1.2/setup.cfg` & `topdownhockey_scraper-3.2.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = TopDownHockey_Scraper
-version = 3.1.2
+version = 3.2.1
 author = Patrick Bacon
 author_email = patrick.s.bacon@gmail.com
 description = A package built for scraping hockey data from EliteProspects, the NHL's HTML/API reports, and ESPN's XML reports.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/TopDownHockey/TopDownHockeyScraper
 project_urls =
```

### Comparing `TopDownHockey_Scraper-3.1.2/setup.py` & `topdownhockey_scraper-3.2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="TopDownHockey_Scraper", # Replace with your own username
-    version="3.1.2",
+    version="3.2.1",
     author="Patrick Bacon",
     author_email="patrick.s.bacon@gmail.com",
     description="The TopDownHockey Scraper",
     long_description=long_description,
     license = 'MIT',
     long_description_content_type="text/markdown",
     url="https://github.com/TopDownHockey/TopDownHockey_Scraper",
```

### Comparing `TopDownHockey_Scraper-3.1.2/src/TopDownHockey_Scraper/TopDownHockey_EliteProspects_Scraper.py` & `topdownhockey_scraper-3.2.1/src/TopDownHockey_Scraper/TopDownHockey_EliteProspects_Scraper.py`

 * *Files identical despite different names*

### Comparing `TopDownHockey_Scraper-3.1.2/src/TopDownHockey_Scraper/TopDownHockey_NHL_Scraper.py` & `topdownhockey_scraper-3.2.1/src/TopDownHockey_Scraper/TopDownHockey_NHL_Scraper.py`

 * *Files identical despite different names*

### Comparing `TopDownHockey_Scraper-3.1.2/src/TopDownHockey_Scraper.egg-info/PKG-INFO` & `topdownhockey_scraper-3.2.1/src/TopDownHockey_Scraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TopDownHockey_Scraper
-Version: 3.1.2
+Version: 3.2.1
 Summary: The TopDownHockey Scraper
 Home-page: https://github.com/TopDownHockey/TopDownHockey_Scraper
 Author: Patrick Bacon
 Author-email: patrick.s.bacon@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/TopDownHockey/TopDownHockey_Scraper/issues
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: TopDownHockey_Scraper Version: 3.1.2 Summary: The
+Metadata-Version: 2.1 Name: TopDownHockey_Scraper Version: 3.2.1 Summary: The
 TopDownHockey Scraper Home-page: https://github.com/TopDownHockey/
 TopDownHockey_Scraper Author: Patrick Bacon Author-email:
 patrick.s.bacon@gmail.com License: MIT Project-URL: Bug Tracker, https://
 github.com/TopDownHockey/TopDownHockey_Scraper/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
```

