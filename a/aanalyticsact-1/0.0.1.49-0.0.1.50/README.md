# Comparing `tmp/aanalyticsact_1-0.0.1.49.tar.gz` & `tmp/aanalyticsact_1-0.0.1.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aanalyticsact_1-0.0.1.49.tar", last modified: Thu Apr 18 07:19:37 2024, max compression
+gzip compressed data, was "aanalyticsact_1-0.0.1.50.tar", last modified: Wed Apr 24 05:08:48 2024, max compression
```

## Comparing `aanalyticsact_1-0.0.1.49.tar` & `aanalyticsact_1-0.0.1.50.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 07:19:37.583301 aanalyticsact_1-0.0.1.49/
--rw-rw-rw-   0        0        0      191 2024-04-18 07:19:37.583301 aanalyticsact_1-0.0.1.49/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-18 07:19:37.567687 aanalyticsact_1-0.0.1.49/aanalyticsact_1/
--rw-rw-rw-   0        0        0      151 2023-12-20 04:59:52.000000 aanalyticsact_1-0.0.1.49/aanalyticsact_1/__init__.py
--rw-rw-rw-   0        0        0       24 2024-04-18 07:01:48.000000 aanalyticsact_1-0.0.1.49/aanalyticsact_1/__version__.py
--rw-rw-rw-   0        0        0     7109 2023-12-20 04:59:52.000000 aanalyticsact_1-0.0.1.49/aanalyticsact_1/actExecute.py
--rw-rw-rw-   0        0        0    18010 2024-03-22 05:30:19.000000 aanalyticsact_1-0.0.1.49/aanalyticsact_1/actModuler.py
--rw-rw-rw-   0        0        0     9139 2024-04-18 06:51:22.000000 aanalyticsact_1-0.0.1.49/aanalyticsact_1/actRunner.py
-drwxrwxrwx   0        0        0        0 2024-04-18 07:19:37.567687 aanalyticsact_1-0.0.1.49/aanalyticsact_1.egg-info/
--rw-rw-rw-   0        0        0      191 2024-04-18 07:19:37.000000 aanalyticsact_1-0.0.1.49/aanalyticsact_1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2024-04-18 07:19:37.000000 aanalyticsact_1-0.0.1.49/aanalyticsact_1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 07:19:37.000000 aanalyticsact_1-0.0.1.49/aanalyticsact_1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-18 07:19:37.000000 aanalyticsact_1-0.0.1.49/aanalyticsact_1.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 07:19:37.583301 aanalyticsact_1-0.0.1.49/setup.cfg
--rw-rw-rw-   0        0        0      732 2024-04-18 07:19:16.000000 aanalyticsact_1-0.0.1.49/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 05:08:48.716898 aanalyticsact_1-0.0.1.50/
+-rw-rw-rw-   0        0        0      191 2024-04-24 05:08:48.715936 aanalyticsact_1-0.0.1.50/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-24 05:08:48.710581 aanalyticsact_1-0.0.1.50/aanalyticsact_1/
+-rw-rw-rw-   0        0        0      151 2023-12-20 04:59:52.000000 aanalyticsact_1-0.0.1.50/aanalyticsact_1/__init__.py
+-rw-rw-rw-   0        0        0       24 2024-04-24 05:06:20.000000 aanalyticsact_1-0.0.1.50/aanalyticsact_1/__version__.py
+-rw-rw-rw-   0        0        0     7109 2023-12-20 04:59:52.000000 aanalyticsact_1-0.0.1.50/aanalyticsact_1/actExecute.py
+-rw-rw-rw-   0        0        0    18036 2024-04-24 05:03:50.000000 aanalyticsact_1-0.0.1.50/aanalyticsact_1/actModuler.py
+-rw-rw-rw-   0        0        0     9139 2024-04-18 06:51:22.000000 aanalyticsact_1-0.0.1.50/aanalyticsact_1/actRunner.py
+drwxrwxrwx   0        0        0        0 2024-04-24 05:08:48.714903 aanalyticsact_1-0.0.1.50/aanalyticsact_1.egg-info/
+-rw-rw-rw-   0        0        0      191 2024-04-24 05:08:48.000000 aanalyticsact_1-0.0.1.50/aanalyticsact_1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2024-04-24 05:08:48.000000 aanalyticsact_1-0.0.1.50/aanalyticsact_1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 05:08:48.000000 aanalyticsact_1-0.0.1.50/aanalyticsact_1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-24 05:08:48.000000 aanalyticsact_1-0.0.1.50/aanalyticsact_1.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 05:08:48.716898 aanalyticsact_1-0.0.1.50/setup.cfg
+-rw-rw-rw-   0        0        0      732 2024-04-24 05:08:44.000000 aanalyticsact_1-0.0.1.50/setup.py
```

### Comparing `aanalyticsact_1-0.0.1.49/aanalyticsact_1/actExecute.py` & `aanalyticsact_1-0.0.1.50/aanalyticsact_1/actExecute.py`

 * *Files identical despite different names*

### Comparing `aanalyticsact_1-0.0.1.49/aanalyticsact_1/actModuler.py` & `aanalyticsact_1-0.0.1.50/aanalyticsact_1/actModuler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Created by Sunkyeong Lee
 # Inquiry : sunkyeong.lee@concentrix.com / sunkyong9768@gmail.com
 # Updated by Youngkwang Cho 
 # Inquiry : youngkwang.Cho@concentrix.com 
+# encoding, create_engine()
+
 
 import aanalytics2 as api2
 import aanalyticsactauth as auth
 import json
 from datetime import datetime, timedelta
 from copy import deepcopy
 from sqlalchemy import create_engine
@@ -192,18 +194,18 @@
     if if_site_code == True:
         if returnRsID(jsonLocation) == "sssamsung4mstglobal":
             df = filterSiteCode(df, site_code)
  
     stackTodb(df, dbTableName)
 
 def create_connection_pool():   ###YK
-    db_connection_str = 'mysql+pymysql://root:12345@127.0.0.1:3307/act'
+    db_connection_str = 'mysql+pymysql://root:12345@127.0.0.1:3307/act?charset=utf8mb4'
     pool_size = 20  
     max_overflow = 10  
-    return create_engine(db_connection_str, encoding='utf-8', poolclass=pool.QueuePool, pool_size=pool_size, max_overflow=max_overflow)
+    return create_engine(db_connection_str, poolclass=pool.QueuePool, pool_size=pool_size, max_overflow=max_overflow)
 
 def stackTodb(dataFrame, dbTableName):  ###YK
     print(dataFrame)
     db_connection = create_connection_pool()
     with db_connection.connect() as conn:
     	dataFrame = unicodeCompile_df(dataFrame)
     	dataFrame.to_sql(name=dbTableName, con=conn, if_exists='append', index=False)
@@ -284,15 +286,15 @@
 
     def remove_non_bmp(text):
         if isinstance(text, str):
             return only_BMP_pattern.sub(r'', text) # only BMP characters
         else:
             return text  # 문자열이 아닌 경우 그대로 반환
 
-    return df.applymap(remove_non_bmp)
+    return df.apply(remove_non_bmp)
 
 # Save as dictionary format return in tuple
 def ReturnJsonchanged(startDate, endDate, jsonFile, jsonFilebreakdown, start_hour, end_hour, site_code):
     itemIDList = returnItemID(startDate, endDate, jsonFile, start_hour, end_hour, site_code)
 
     itemIDdict = {}
     for i in range(len(itemIDList)):
```

### Comparing `aanalyticsact_1-0.0.1.49/aanalyticsact_1/actRunner.py` & `aanalyticsact_1-0.0.1.50/aanalyticsact_1/actRunner.py`

 * *Files identical despite different names*

### Comparing `aanalyticsact_1-0.0.1.49/setup.py` & `aanalyticsact_1-0.0.1.50/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import sys
 
 from setuptools import find_packages, setup
 
 # Package meta-data.
 NAME = 'aanalyticsact_1'
-Version= '0.0.1.49'
+Version= '0.0.1.50'
 URL = 'https://github.com/Glory-Cho/aanalyticsact)1'
 Summary= 'adobe analytics library for Team ACT'
 EMAIL = 'youngkwang.cho@concentrix.com'
 AUTHOR = 'Youngkwang Cho'
 
 here = os.path.abspath(os.path.dirname(__file__))
```

