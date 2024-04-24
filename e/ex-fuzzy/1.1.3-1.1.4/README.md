# Comparing `tmp/ex_fuzzy-1.1.3.tar.gz` & `tmp/ex_fuzzy-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ex_fuzzy-1.1.3.tar", last modified: Thu Apr 11 15:42:48 2024, max compression
+gzip compressed data, was "ex_fuzzy-1.1.4.tar", last modified: Wed Apr 24 13:51:01 2024, max compression
```

## Comparing `ex_fuzzy-1.1.3.tar` & `ex_fuzzy-1.1.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 15:42:48.265662 ex_fuzzy-1.1.3/
--rw-rw-rw-   0        0        0    35184 2024-04-10 13:18:52.000000 ex_fuzzy-1.1.3/LICENSE
--rw-rw-rw-   0        0        0     5785 2024-04-11 15:42:48.263661 ex_fuzzy-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     4736 2024-04-10 16:32:46.000000 ex_fuzzy-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 15:42:48.164651 ex_fuzzy-1.1.3/ex_fuzzy/
-drwxrwxrwx   0        0        0        0 2024-04-11 15:42:48.240659 ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/
--rw-rw-rw-   0        0        0      282 2024-04-05 15:43:34.000000 ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/__init__.py
--rw-rw-rw-   0        0        0     6197 2024-01-31 12:48:36.000000 ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/centroid.py
--rw-rw-rw-   0        0        0    11027 2024-04-11 15:17:33.000000 ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/classifiers.py
--rw-rw-rw-   0        0        0     7433 2024-01-30 16:48:50.000000 ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/cognitive_maps.py
--rw-rw-rw-   0        0        0    15674 2024-04-05 10:32:51.000000 ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/eval_rules.py
--rw-rw-rw-   0        0        0     2640 2024-04-05 14:46:18.000000 ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/eval_tools.py
--rw-rw-rw-   0        0        0    42810 2024-04-11 15:37:23.000000 ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/evolutionary_fit.py
--rw-rw-rw-   0        0        0    17306 2024-04-05 15:07:12.000000 ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/fuzzy_sets.py
--rw-rw-rw-   0        0        0     6160 2024-04-03 14:16:49.000000 ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/maintenance.py
--rw-rw-rw-   0        0        0     3677 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/persistence.py
--rw-rw-rw-   0        0        0    11420 2024-04-05 16:05:24.000000 ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/rule_mining.py
--rw-rw-rw-   0        0        0    39296 2024-04-11 15:35:59.000000 ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/rules.py
--rw-rw-rw-   0        0        0    27001 2024-01-31 15:05:05.000000 ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/temporal.py
--rw-rw-rw-   0        0        0    25751 2024-04-05 15:33:36.000000 ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/utils.py
--rw-rw-rw-   0        0        0    15945 2024-04-04 16:52:41.000000 ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/vis_rules.py
-drwxrwxrwx   0        0        0        0 2024-04-11 15:42:48.188652 ex_fuzzy-1.1.3/ex_fuzzy.egg-info/
--rw-rw-rw-   0        0        0     5785 2024-04-11 15:42:47.000000 ex_fuzzy-1.1.3/ex_fuzzy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      785 2024-04-11 15:42:48.000000 ex_fuzzy-1.1.3/ex_fuzzy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 15:42:47.000000 ex_fuzzy-1.1.3/ex_fuzzy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-04-11 15:42:47.000000 ex_fuzzy-1.1.3/ex_fuzzy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-11 15:42:47.000000 ex_fuzzy-1.1.3/ex_fuzzy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 15:42:48.266663 ex_fuzzy-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1773 2024-04-11 15:42:39.000000 ex_fuzzy-1.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-11 15:42:48.258661 ex_fuzzy-1.1.3/tests/
--rw-rw-rw-   0        0        0     1261 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.3/tests/test_centroids.py
--rw-rw-rw-   0        0        0     1963 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.3/tests/test_classification.py
--rw-rw-rw-   0        0        0      797 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.3/tests/test_eval_tools.py
--rw-rw-rw-   0        0        0     1821 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.3/tests/test_fuzzy_sets.py
--rw-rw-rw-   0        0        0     4189 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.3/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-24 13:51:01.501254 ex_fuzzy-1.1.4/
+-rw-rw-rw-   0        0        0    35184 2024-04-10 13:18:52.000000 ex_fuzzy-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0     4333 2024-04-24 13:51:01.494273 ex_fuzzy-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3284 2024-04-22 14:14:00.000000 ex_fuzzy-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 13:51:01.369252 ex_fuzzy-1.1.4/ex_fuzzy/
+drwxrwxrwx   0        0        0        0 2024-04-24 13:51:01.469252 ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/
+-rw-rw-rw-   0        0        0      282 2024-04-05 15:43:34.000000 ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/__init__.py
+-rw-rw-rw-   0        0        0     6197 2024-01-31 12:48:36.000000 ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/centroid.py
+-rw-rw-rw-   0        0        0    11027 2024-04-11 15:17:33.000000 ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/classifiers.py
+-rw-rw-rw-   0        0        0     7433 2024-01-30 16:48:50.000000 ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/cognitive_maps.py
+-rw-rw-rw-   0        0        0    15878 2024-04-18 15:39:28.000000 ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/eval_rules.py
+-rw-rw-rw-   0        0        0     2693 2024-04-24 13:08:01.000000 ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/eval_tools.py
+-rw-rw-rw-   0        0        0    43114 2024-04-24 13:36:10.000000 ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/evolutionary_fit.py
+-rw-rw-rw-   0        0        0    17306 2024-04-05 15:07:12.000000 ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/fuzzy_sets.py
+-rw-rw-rw-   0        0        0     6160 2024-04-03 14:16:49.000000 ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/maintenance.py
+-rw-rw-rw-   0        0        0     3677 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/persistence.py
+-rw-rw-rw-   0        0        0    11420 2024-04-05 16:05:24.000000 ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/rule_mining.py
+-rw-rw-rw-   0        0        0    41199 2024-04-23 15:06:45.000000 ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/rules.py
+-rw-rw-rw-   0        0        0    27001 2024-01-31 15:05:05.000000 ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/temporal.py
+-rw-rw-rw-   0        0        0    25751 2024-04-05 15:33:36.000000 ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/utils.py
+-rw-rw-rw-   0        0        0    16166 2024-04-24 13:41:44.000000 ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/vis_rules.py
+drwxrwxrwx   0        0        0        0 2024-04-24 13:51:01.400254 ex_fuzzy-1.1.4/ex_fuzzy.egg-info/
+-rw-rw-rw-   0        0        0     4333 2024-04-24 13:51:01.000000 ex_fuzzy-1.1.4/ex_fuzzy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      785 2024-04-24 13:51:01.000000 ex_fuzzy-1.1.4/ex_fuzzy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 13:51:01.000000 ex_fuzzy-1.1.4/ex_fuzzy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-04-24 13:51:01.000000 ex_fuzzy-1.1.4/ex_fuzzy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-24 13:51:01.000000 ex_fuzzy-1.1.4/ex_fuzzy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 13:51:01.502251 ex_fuzzy-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1773 2024-04-24 13:50:10.000000 ex_fuzzy-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 13:51:01.491252 ex_fuzzy-1.1.4/tests/
+-rw-rw-rw-   0        0        0     1261 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.4/tests/test_centroids.py
+-rw-rw-rw-   0        0        0     1963 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.4/tests/test_classification.py
+-rw-rw-rw-   0        0        0      797 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.4/tests/test_eval_tools.py
+-rw-rw-rw-   0        0        0     1821 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.4/tests/test_fuzzy_sets.py
+-rw-rw-rw-   0        0        0     4189 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.4/tests/test_utils.py
```

### Comparing `ex_fuzzy-1.1.3/LICENSE` & `ex_fuzzy-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.3/PKG-INFO` & `ex_fuzzy-1.1.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ex_fuzzy
-Version: 1.1.3
+Version: 1.1.4
 Summary: Library to perform explainable AI using fuzzy logic.
 Home-page: https://github.com/Fuminides/ex-fuzzy
 Download-URL: https://pypi.org/project/ex-fuzzy/
 Maintainer: Javier Fumanal Idocin
 Maintainer-email: javierfumanalidocin@gmail.com
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
@@ -51,18 +51,18 @@
 
 ### Visualization
 
 Use plots to visualize any kind of fuzzy sets, and use graphs to visualize rules or print them on screen.
 
 
 <p align="center">
-  <img src="https://user-images.githubusercontent.com/12574757/210235257-17b22ede-762b-406c-880a-497e06964f17.png" width="350" title="Fuzzy graph">
-  <img src="https://user-images.githubusercontent.com/12574757/210235264-be98fff9-d1b6-4f3b-8b93-b11e0466a48c.png" width="350" title="Type 1 example">
-  <img src="https://private-user-images.githubusercontent.com/12574757/310877934-89b7184e-5dcc-445f-8b5f-7d4e9388c56f.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTI3NTk5NTAsIm5iZiI6MTcxMjc1OTY1MCwicGF0aCI6Ii8xMjU3NDc1Ny8zMTA4Nzc5MzQtODliNzE4NGUtNWRjYy00NDVmLThiNWYtN2Q0ZTkzODhjNTZmLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA0MTAlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNDEwVDE0MzQxMFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWU0MzQ2YzhjMmQyM2M2MDlhMzc2MGUwMzUxYzFlNDgyNjk1OTU4NTY3ZGQ1Y2RhZDM2N2MzZDY2MTU2ZGVmMTImWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.bnJll8XpKV6o7R6MXmjNB7wJQY8eYyBMANpwkPQjRo0" width="350" title="Type 2 example">
-  <img src="https://private-user-images.githubusercontent.com/12574757/310877940-cf4453fe-6f82-4f49-b418-c774729022f7.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTI3NTk5NTAsIm5iZiI6MTcxMjc1OTY1MCwicGF0aCI6Ii8xMjU3NDc1Ny8zMTA4Nzc5NDAtY2Y0NDUzZmUtNmY4Mi00ZjQ5LWI0MTgtYzc3NDcyOTAyMmY3LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA0MTAlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNDEwVDE0MzQxMFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTcyNmQwNTFiNzNmYTljN2ZjZjcyYjY2ZTg3NWRjZDMxNmMyNGFmZTBlMGNkOTg4YTdlN2RkODNhYzc0OGE1NmUmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.Q_LcDf9RsPHi_QKuqMxkaIQ0dKvx8-dSv0u-KcyRNIA" width="350" title="General Type 2 example">
+  <img src="https://user-images.githubusercontent.com/12574757/210235257-17b22ede-762b-406c-880a-497e06964f17.png" height="320" title="Fuzzy graph">
+  <img src="https://user-images.githubusercontent.com/12574757/210235264-be98fff9-d1b6-4f3b-8b93-b11e0466a48c.png" height="320" title="Type 1 example">
+  <img src="https://github.com/Fuminides/ex-fuzzy/assets/12574757/0a3f4508-6ab8-40b5-938b-d89b619c53a3" height="350" title="Type 2 example">
+  <img src="https://github.com/Fuminides/ex-fuzzy/assets/12574757/b356a09f-4c66-45c9-8362-ebdbda684669" height="350" title="General Type 2 example">
   
 </p>
 
 ## Dependencies
 
 - Numpy
 - Pandas
```

### Comparing `ex_fuzzy-1.1.3/README.md` & `ex_fuzzy-1.1.4/ex_fuzzy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,34 @@
+Metadata-Version: 2.1
+Name: ex-fuzzy
+Version: 1.1.4
+Summary: Library to perform explainable AI using fuzzy logic.
+Home-page: https://github.com/Fuminides/ex-fuzzy
+Download-URL: https://pypi.org/project/ex-fuzzy/
+Maintainer: Javier Fumanal Idocin
+Maintainer-email: javierfumanalidocin@gmail.com
+License: GPL-3.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: networkx
+Requires-Dist: matplotlib
+Requires-Dist: pymoo
+Requires-Dist: pandas
+Requires-Dist: scikit-learn
+
 # Ex-Fuzzy
 ex-Fuzzy is a fuzzy toolbox library for Python with special focus in its accesibility to use and visualization of results. In this way, we focus on the ex(-Fuzzy)plainable capacities of approximate reasoning.
 
 Some of the tools available in this library include:
 
 - Support for approximate reasoning using fuzzy association rules, for both classification and regression problems. This includes rule base optimization using genetic algorithms and rule visualization.
 - Precomputed and optimized fuzzy variables and their correspondent linguistic variables (i.e low, medium, high).
@@ -24,18 +51,18 @@
 
 ### Visualization
 
 Use plots to visualize any kind of fuzzy sets, and use graphs to visualize rules or print them on screen.
 
 
 <p align="center">
-  <img src="https://user-images.githubusercontent.com/12574757/210235257-17b22ede-762b-406c-880a-497e06964f17.png" width="350" title="Fuzzy graph">
-  <img src="https://user-images.githubusercontent.com/12574757/210235264-be98fff9-d1b6-4f3b-8b93-b11e0466a48c.png" width="350" title="Type 1 example">
-  <img src="https://private-user-images.githubusercontent.com/12574757/310877934-89b7184e-5dcc-445f-8b5f-7d4e9388c56f.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTI3NTk5NTAsIm5iZiI6MTcxMjc1OTY1MCwicGF0aCI6Ii8xMjU3NDc1Ny8zMTA4Nzc5MzQtODliNzE4NGUtNWRjYy00NDVmLThiNWYtN2Q0ZTkzODhjNTZmLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA0MTAlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNDEwVDE0MzQxMFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWU0MzQ2YzhjMmQyM2M2MDlhMzc2MGUwMzUxYzFlNDgyNjk1OTU4NTY3ZGQ1Y2RhZDM2N2MzZDY2MTU2ZGVmMTImWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.bnJll8XpKV6o7R6MXmjNB7wJQY8eYyBMANpwkPQjRo0" width="350" title="Type 2 example">
-  <img src="https://private-user-images.githubusercontent.com/12574757/310877940-cf4453fe-6f82-4f49-b418-c774729022f7.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTI3NTk5NTAsIm5iZiI6MTcxMjc1OTY1MCwicGF0aCI6Ii8xMjU3NDc1Ny8zMTA4Nzc5NDAtY2Y0NDUzZmUtNmY4Mi00ZjQ5LWI0MTgtYzc3NDcyOTAyMmY3LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA0MTAlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNDEwVDE0MzQxMFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTcyNmQwNTFiNzNmYTljN2ZjZjcyYjY2ZTg3NWRjZDMxNmMyNGFmZTBlMGNkOTg4YTdlN2RkODNhYzc0OGE1NmUmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.Q_LcDf9RsPHi_QKuqMxkaIQ0dKvx8-dSv0u-KcyRNIA" width="350" title="General Type 2 example">
+  <img src="https://user-images.githubusercontent.com/12574757/210235257-17b22ede-762b-406c-880a-497e06964f17.png" height="320" title="Fuzzy graph">
+  <img src="https://user-images.githubusercontent.com/12574757/210235264-be98fff9-d1b6-4f3b-8b93-b11e0466a48c.png" height="320" title="Type 1 example">
+  <img src="https://github.com/Fuminides/ex-fuzzy/assets/12574757/0a3f4508-6ab8-40b5-938b-d89b619c53a3" height="350" title="Type 2 example">
+  <img src="https://github.com/Fuminides/ex-fuzzy/assets/12574757/b356a09f-4c66-45c9-8362-ebdbda684669" height="350" title="General Type 2 example">
   
 </p>
 
 ## Dependencies
 
 - Numpy
 - Pandas
```

### Comparing `ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/centroid.py` & `ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/centroid.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/classifiers.py` & `ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/classifiers.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/cognitive_maps.py` & `ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/cognitive_maps.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/eval_rules.py` & `ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/eval_rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,21 @@
         '''
         self.mrule_base = mrule_base
         self.X = X
         self.y = y
         self.time_moments = time_moments
 
         self.consequents = mrule_base.get_consequents()
+        self.consequents_names = mrule_base.get_consequents_names()
         self.precomputed_truth = precomputed_truth
 
+        if isinstance(y[0], str):
+            self.y = np.array([list(self.consequents_names).index(str(y)) for y in y])
+
+
 
     def compute_pattern_support(self) -> np.array:
         '''
         Computes the pattern support for each of the rules for the given X.
         Each pattern support firing strength is the result of the tnorm for all the antecedent memeberships,
         dvided by their number.
 
@@ -144,15 +149,15 @@
             res = np.zeros((len(patterns), ))
         elif self.mrule_base.fuzzy_type() == fs.FUZZY_SETS.t2:
             res = np.zeros((len(patterns), 2))
         elif self.mrule_base.fuzzy_type() == fs.FUZZY_SETS.gt2:
             res = np.zeros((len(patterns), 2))
 
         for ix, pattern in enumerate(patterns):
-            antecedent_consequent_match = self.y == self.consequents[ix]
+            antecedent_consequent_match = np.equal(self.y, self.consequents[ix])
             pattern_firing_strength = antecedent_memberships[:, ix]
             dem = np.sum(pattern_firing_strength)
             if dem == 0:
                 res[ix] = 0
             else:
                 res[ix] = np.sum(
                     pattern_firing_strength[antecedent_consequent_match]) / dem
```

### Comparing `ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/eval_tools.py` & `ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/eval_tools.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,18 +27,20 @@
     :param y_test: Test labels.
     :param plot_rules: If True, it plots the rules.
     :param print_rules: If True, it prints the rules.
     :param plot_partitions: If True, it plots the fuzzy partitions.
     :return: None
     '''
     # Get the unique classes from the classifier
-    unique_classes = fl_classifier.classes_
-    # Convert the names from the labels to the corresponding class
-    y_train = np.array([list(unique_classes).index(str(y)) for y in y_train])
-    y_test = np.array([list(unique_classes).index(str(y)) for y in y_test])
+    unique_classes = fl_classifier.classes_names
+
+    # Convert the names from the labels to the corresponding class if necessary
+    if isinstance(y_train[0], str):
+      y_train = np.array([list(unique_classes).index(str(y)) for y in y_train])
+      y_test = np.array([list(unique_classes).index(str(y)) for y in y_test])
     
     if print_accuracy:
       print('------------')
       print('ACCURACY')
       print('Train performance: ' +
             str(np.mean(np.equal(y_train, fl_classifier.predict(X_train)))))
       print('Test performance: ' +
@@ -50,15 +52,15 @@
             str(matthews_corrcoef(y_train, fl_classifier.predict(X_train))))
       print('Test performance: ' +
             str(matthews_corrcoef(y_test, fl_classifier.predict(X_test))))
       print('------------')
 
 
     if print_rules or return_rules:
-        res = fl_classifier.print_rules(return_rules)
+        res = fl_classifier.print_rules(True)
 
         if print_rules:
             print(res)
 
     if plot_partitions:
         fl_classifier.plot_fuzzy_variables()
```

### Comparing `ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/evolutionary_fit.py` & `ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/evolutionary_fit.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 
 class BaseFuzzyRulesClassifier(ClassifierMixin):
     '''
     Class that is used as a classifier for a fuzzy rule based system. Supports precomputed and optimization of the linguistic variables.
     '''
 
-    def __init__(self,  nRules: int = 30, nAnts: int = 4, fuzzy_type: fs.FUZZY_SETS = fs.FUZZY_SETS.t1, tolerance: float = 0.0,
+    def __init__(self,  nRules: int = 30, nAnts: int = 4, fuzzy_type: fs.FUZZY_SETS = fs.FUZZY_SETS.t1, tolerance: float = 0.0, class_names: list[str] = None,
                  n_linguist_variables: int = 3, verbose=False, linguistic_variables: list[fs.fuzzyVariable] = None,
                  domain: list[float] = None, n_class: int=None, precomputed_rules: rules.MasterRuleBase=None, runner: int=1) -> None:
         '''
         Inits the optimizer with the corresponding parameters.
 
         :param nRules: number of rules to optimize.
         :param nAnts: max number of antecedents to use.
@@ -59,20 +59,28 @@
         if mnt.save_usage_flag:
             mnt.usage_data[mnt.usage_categories.Funcs]['fit'] += 1
 
         if precomputed_rules is not None:
             self.nRules = len(precomputed_rules.get_rules())
             self.nAnts = len(precomputed_rules.get_rules()[0].antecedents)
             self.n_class = len(precomputed_rules)
-            self.classes_ = precomputed_rules.consequent_names
+            self.nclasses_ = len(precomputed_rules.consequent_names)
+            self.classes_names = precomputed_rules.consequent_names
             self.rule_base = precomputed_rules
         else:
             self.nRules = nRules
             self.nAnts = nAnts
-            self.classes_ = n_class
+            self.nclasses_ = n_class
+            if not (class_names is None):
+                if isinstance(class_names, np.ndarray):
+                    self.classes_names = list(class_names)
+                else:
+                    self.classes_names = class_names
+            else:
+                self.classes_names = class_names
 
         self.custom_loss = None
         self.verbose = verbose
         self.tolerance = tolerance
         
 
         if runner > 1:
@@ -125,21 +133,19 @@
         :param checkpoints: integer. Number of checkpoints to save the best rulebase found so far.
         :param candidate_rules: if these rules exist, the optimization process will choose the best rules from this set. If None (default) the rules will be generated from scratch.
         :return: None. The classifier is fitted to the data.
         '''
         if mnt.save_usage_flag:
             mnt.usage_data[mnt.usage_categories.Funcs]['fit'] += 1
             
-        if self.classes_ is None:
-            if isinstance(y, pd.Series):
-                self.classes_ = [str(aux) for aux in y.unique()]
-                # Convert the names in the label vector to integer classes
-                y = np.array(y.replace(self.classes_, np.arange(len(self.classes_))))
-            else:
-                self.classes_ = [str(aux) for aux in np.unique(y)]
+        if self.classes_names is None:
+            self.classes_names = [aux for aux in np.unique(y)]
+        
+        if isinstance(y[0], str):
+            y = np.array([self.classes_names.index(str(aux)) for aux in y])
             
         if candidate_rules is None:
             if initial_rules is not None:
                 self.fuzzy_type = initial_rules.fuzzy_type()
                 self.n_linguist_variables = initial_rules.n_linguist_variables()
                 self.domain = [fv.domain for fv in initial_rules[0].antecedents]
                 self.nRules = len(initial_rules.get_rules())
@@ -199,15 +205,15 @@
                             best_individual, self.fuzzy_type)
                         eval_performance = evr.evalRuleBase(
                             rule_base, np.array(X), y)
                         
                         eval_performance.add_full_evaluation()  
                         # self.rename_fuzzy_variables() This wont work on checkpoints!
                         rule_base.purge_rules(self.tolerance)
-                        rule_base.rename_cons(self.classes_)
+                        rule_base.rename_cons(self.nclasses_)
                         checkpoint_rules = rule_base.print_rules(True)
                         f.write(checkpoint_rules)     
 
         else:
             res = minimize(problem,
                         algorithm,
                         # termination,
@@ -230,14 +236,15 @@
             self.X = X.values
         except AttributeError:
             self.X = X
             self.var_names = [str(ix) for ix in range(X.shape[1])]
 
         self.rule_base = problem._construct_ruleBase(
         best_individual, self.fuzzy_type)
+        self.rule_base.rename_cons(self.classes_names)
 
         self.eval_performance = evr.evalRuleBase(
         self.rule_base, np.array(X), y)
 
         self.eval_performance.add_full_evaluation()  
         if self.lvs is None:
             self.rename_fuzzy_variables()
@@ -252,15 +259,15 @@
         :param rule_base: ruleBase object.
         :return: None
         '''
         self.rule_base = rule_base
         self.nRules = len(rule_base.get_rules())
         self.nAnts = len(rule_base.get_rules()[0].antecedents)
         self.n_class = len(rule_base)
-        self.classes_ = rule_base.consequent_names
+        self.nclasses_ = rule_base.consequent_names
         
 
     def forward(self, X: np.array) -> np.array:
         '''
         Returns the predicted class for each sample.
 
         :param X: np array samples x features.
```

### Comparing `ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/fuzzy_sets.py` & `ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/fuzzy_sets.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/maintenance.py` & `ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/maintenance.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/persistence.py` & `ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/persistence.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/rule_mining.py` & `ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/rule_mining.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/rules.py` & `ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/rules.py`

 * *Files 0% similar despite different names*

```diff
@@ -337,14 +337,17 @@
         for jx, rule in enumerate(self.rules):
             rule_antecedents = rule.antecedents
 
             if self.fuzzy_type() == fs.FUZZY_SETS.t1:
                 membership = np.zeros((x.shape[0], len(rule_antecedents)))
             elif self.fuzzy_type() == fs.FUZZY_SETS.t2:
                 membership = np.zeros((x.shape[0], len(rule_antecedents), 2))
+            elif self.fuzzy_type() == fs.FUZZY_SETS.gt2:
+                membership = np.zeros(
+                    (x.shape[0], len(rule_antecedents), len(self.alpha_cuts), 2))
 
             
             for ix, vl in enumerate(rule_antecedents):
                 n_nonvl = 0
                 if vl >= 0:
                     membership_antecedent = list(antecedents_memberships[ix])[vl]
                     membership[:, ix] = membership_antecedent
@@ -733,36 +736,40 @@
         Returns the correspoing type of the RuleBase using the enum type in the fuzzy_sets module.
 
         :return: the corresponding fuzzy set type of the RuleBase.
         '''
         return fs.FUZZY_SETS.gt2
 
 
-    def compute_rule_antecedent_memberships(self, x: np.array, scaled=True) -> np.array:
+    def compute_rule_antecedent_memberships(self, x: np.array, scaled=True, antecedents_memberships=None) -> np.array:
         '''
         Computes the membership for the antecedents performing the alpha_cut reduction.
 
         :param x: array with the values of the inputs.
         :param scaled: if True, the memberships are scaled to sum 1 in each sample.
+        :param antecedents_memberships: precomputed antecedent memberships. Not supported for GT2.
+        :return: array with the memberships of the antecedents for each sample.
         '''
         antecedent_membership = super().compute_rule_antecedent_memberships(x, scaled)
         return self._alpha_reduction(antecedent_membership)
 
 
-    def alpha_compute_rule_antecedent_memberships(self, x: np.array, scaled=True) -> np.array:
+    def alpha_compute_rule_antecedent_memberships(self, x: np.array, scaled=True, antecedents_memberships=None) -> np.array:
         '''
         Computes the membership for the antecedents for all the alpha cuts.
 
         :param x: array with the values of the inputs.
         :param scaled: if True, the memberships are scaled to sum 1 in each sample.
+        :param antecedents_memberships: precomputed antecedent memberships. Not supported for GT2.
         :return: array with the memberships of the antecedents for each sample.
         '''
         return super().compute_rule_antecedent_memberships(x, scaled)
 
 
+
 class RuleBaseT1(RuleBase):
     '''
     Class optimized to work with multiple rules at the same time. Supports only one consequent.
     (Use one rulebase per consequent to study classification problems. Check MasterRuleBase class for more documentation)
 
     This class supports t1 fs.
     '''
@@ -838,14 +845,15 @@
         Returns the correspoing type of the RuleBase using the enum type in the fuzzy_sets module.
 
         :return: the corresponding fuzzy set type of the RuleBase.
         '''
         return fs.FUZZY_SETS.t1
 
 
+
 class MasterRuleBase():
     '''
     This Class encompasses a list of rule bases where each one corresponds to a different class.
     '''
 
     def __init__(self, rule_base: list[RuleBase], consequent_names: list[str]=None) -> None:
         '''
@@ -884,16 +892,25 @@
 
     def get_consequents(self) -> list[int]:
         '''
         Returns a list with the consequents of each rule base.
 
         :return: list with the consequents of each rule base.
         '''
-        return sum([[self.consequent_names[ix]]*len(x) for ix, x in enumerate(self.rule_bases)], [])
+        return sum([[ix]*len(x) for ix, x in enumerate(self.rule_bases)], [])
+
+
+    def get_consequents_names(self) -> list[str]:
+        '''
+        Returns a list with the names of the consequents.
 
+        :return: list with the names of the consequents.
+        '''
+        return self.consequent_names
+    
 
     def get_rulebase_matrix(self) -> list[np.array]:
         '''
         Returns a list with the rulebases for each antecedent in matrix format.
 
         :return: list with the rulebases for each antecedent in matrix format.
         '''
@@ -961,15 +978,15 @@
         :param precomputed_truth: if not None, the antecedent memberships are already computed. (Used for sped up in genetic algorithms)
         :return: array with the winning rule for each sample.
         '''
         # Raise an error if there no rules
         if len(self.get_rules()) == 0:
             raise RuleError('No rules to predict!')
         
-        consequents = sum([[self.consequent_names[ix]]*len(self[ix].rules)
+        consequents = sum([[ix]*len(self[ix].rules)
                           for ix in range(len(self.rule_bases))], [])  # The sum is for flatenning the list
         winning_rules = self._winning_rules(X, precomputed_truth=precomputed_truth)
 
         return np.array([consequents[ix] for ix in winning_rules])
 
 
     def add_rule_base(self, rule_base: RuleBase) -> None:
@@ -1099,14 +1116,45 @@
     def get_antecedents(self) -> list[fs.fuzzyVariable]:
         '''
         Returns the antecedents of the rule base.
         '''
         return self.antecedents
     
 
+def construct_rule_base(rule_matrix: np.array, consequents: np.array, antecedents: list[fs.fuzzyVariable], rule_weights: np.array, class_names: list=None) -> MasterRuleBase:
+    '''
+    Constructs a rule base from a matrix of rules.
+
+    :param rule_matrix: matrix with the rules.
+    :param consequents: array with the consequents per rule.
+    :param antecedents: list of fuzzy variables.
+    :param class_names: list with the names of the classes.
+    '''
+    rule_lists = {ix:[] for ix in range(len(np.unique(consequents)))}
+
+    for ix, consequent in enumerate(consequents):
+        if not np.equal(rule_matrix, -1).all():
+            rule_object = RuleSimple(rule_matrix[ix])
+            rule_object.score = rule_weights[ix]
+            rule_lists[consequent].append(rule_object)
+
+    for ix, consequent in enumerate(np.unique(consequents)):
+        rule_base = RuleBaseT1(antecedents, rule_lists[ix])
+        
+        if ix == 0:
+            res = MasterRuleBase([rule_base], np.unique(consequents))
+        else:
+            res.add_rule_base(rule_base)
+
+    if class_names is not None:
+        res.rename_cons(class_names)
+
+    return res
+
+
 def list_rules_to_matrix(rule_list: list[RuleSimple]) -> np.array:
     '''
     Returns a matrix out of the rule list.
 
     :param rule_list: list of rules.
     :return: matrix with the antecedents of the rules.
     '''
```

### Comparing `ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/temporal.py` & `ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/temporal.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/utils.py` & `ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/utils.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/vis_rules.py` & `ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/vis_rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,16 +146,19 @@
     '''
     Connects antecedents connected by checking if both are in the same rule.
 
     :param mrule_base: Master rule base to connect.
     :return: List of list of pandas dataframes with the connections in adjacency matrix format.
     '''
     res = []
-    for rule_base in mrule_base.rule_bases:
-        res.append(connect_rulebase(rule_base))
+    for ix, rule_base in enumerate(mrule_base.rule_bases):
+        try:
+            res.append(connect_rulebase(rule_base))
+        except:
+            print('Error in the visualization of the rule base: "' + mrule_base.get_consequents_names()[ix] + '", probably because there are no rules in the rule base.')
 
     return res
 
 
 def visualize_rulebase(mrule_base: rules.MasterRuleBase, export_path: str=None) -> None:
     '''
     Visualize a rule base using low, medium and high partitions with 1 rule in common -> 1 edge connections.
```

### Comparing `ex_fuzzy-1.1.3/ex_fuzzy.egg-info/SOURCES.txt` & `ex_fuzzy-1.1.4/ex_fuzzy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.3/setup.py` & `ex_fuzzy-1.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 DISTNAME = "ex_fuzzy"
 DESCRIPTION = "Library to perform explainable AI using fuzzy logic."
 MAINTAINER = "Javier Fumanal Idocin"
 MAINTAINER_EMAIL = "javierfumanalidocin@gmail.com"
 URL = "https://github.com/Fuminides/ex-fuzzy"
 LICENSE = "GPL-3.0"
 DOWNLOAD_URL = "https://pypi.org/project/ex-fuzzy/"
-VERSION = "1.1.3"
+VERSION = "1.1.4"
 INSTALL_REQUIRES = ["numpy", "networkx", "matplotlib", "pymoo", "pandas", "scikit-learn"]
 CLASSIFIERS = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.7",
```

### Comparing `ex_fuzzy-1.1.3/tests/test_centroids.py` & `ex_fuzzy-1.1.4/tests/test_centroids.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.3/tests/test_classification.py` & `ex_fuzzy-1.1.4/tests/test_classification.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.3/tests/test_eval_tools.py` & `ex_fuzzy-1.1.4/tests/test_eval_tools.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.3/tests/test_fuzzy_sets.py` & `ex_fuzzy-1.1.4/tests/test_fuzzy_sets.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.3/tests/test_utils.py` & `ex_fuzzy-1.1.4/tests/test_utils.py`

 * *Files identical despite different names*

