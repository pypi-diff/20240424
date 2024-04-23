# Comparing `tmp/troopwebhost_download-0.3.2.tar.gz` & `tmp/troopwebhost_download-0.3.3.tar.gz`

## Comparing `troopwebhost_download-0.3.2.tar` & `troopwebhost_download-0.3.3.tar`

### file list

```diff
@@ -1,12 +1,17 @@
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 troopwebhost_download-0.3.2/.env.example
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 troopwebhost_download-0.3.2/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 troopwebhost_download-0.3.2/twh_download/__init__.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 troopwebhost_download-0.3.2/twh_download/__main__.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 troopwebhost_download-0.3.2/twh_download/cli.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 troopwebhost_download-0.3.2/twh_download/config.toml
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 troopwebhost_download-0.3.2/twh_download/export.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 troopwebhost_download-0.3.2/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 troopwebhost_download-0.3.2/LICENSE
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 troopwebhost_download-0.3.2/README.md
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 troopwebhost_download-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 troopwebhost_download-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 troopwebhost_download-0.3.3/.env.example
+-rw-r--r--   0        0        0    21553 2020-02-02 00:00:00.000000 troopwebhost_download-0.3.3/104_adults.csv
+-rw-r--r--   0        0        0    53326 2020-02-02 00:00:00.000000 troopwebhost_download-0.3.3/104_merit_badges.csv
+-rw-r--r--   0        0        0  1551198 2020-02-02 00:00:00.000000 troopwebhost_download-0.3.3/104_rank_requirements_status.csv
+-rw-r--r--   0        0        0    16539 2020-02-02 00:00:00.000000 troopwebhost_download-0.3.3/104_scouts.csv
+-rw-r--r--   0        0        0  1199097 2020-02-02 00:00:00.000000 troopwebhost_download-0.3.3/104_uncompleted_merit_badge_requirements_by_scout.csv
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 troopwebhost_download-0.3.3/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 troopwebhost_download-0.3.3/twh_download/__init__.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 troopwebhost_download-0.3.3/twh_download/__main__.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 troopwebhost_download-0.3.3/twh_download/cli.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 troopwebhost_download-0.3.3/twh_download/config.toml
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 troopwebhost_download-0.3.3/twh_download/export.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 troopwebhost_download-0.3.3/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 troopwebhost_download-0.3.3/LICENSE
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 troopwebhost_download-0.3.3/README.md
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 troopwebhost_download-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 troopwebhost_download-0.3.3/PKG-INFO
```

### Comparing `troopwebhost_download-0.3.2/twh_download/cli.py` & `troopwebhost_download-0.3.3/twh_download/cli.py`

 * *Files identical despite different names*

### Comparing `troopwebhost_download-0.3.2/twh_download/export.py` & `troopwebhost_download-0.3.3/twh_download/export.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import requests
 from pathlib import Path
 import toml
 from dotenv import dotenv_values
 from getpass import getpass
 
-__version__ = "0.3.2"
+__version__ = "0.3.3"
 
 
 def login(session, username, password):
     payload = {
         "Selected_Action": "login",
         "Menu_Item_ID": 49792,
         "Form_ID": 7323,
```

### Comparing `troopwebhost_download-0.3.2/LICENSE` & `troopwebhost_download-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `troopwebhost_download-0.3.2/pyproject.toml` & `troopwebhost_download-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `troopwebhost_download-0.3.2/PKG-INFO` & `troopwebhost_download-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: troopwebhost-download
-Version: 0.3.2
+Version: 0.3.3
 Summary: Retrieve CSV files from Troopwebhost
 Author-email: Michael Perkins <perkinsms@gmail.com>
 Maintainer-email: Michael Perkins <perkinsms@gmail.com>
 License: MIT License
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

