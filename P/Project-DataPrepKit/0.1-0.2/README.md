# Comparing `tmp/Project_DataPrepKit-0.1.tar.gz` & `tmp/Project_DataPrepKit-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Project_DataPrepKit-0.1.tar", last modified: Tue Apr 23 13:21:07 2024, max compression
+gzip compressed data, was "Project_DataPrepKit-0.2.tar", last modified: Wed Apr 24 09:25:00 2024, max compression
```

## Comparing `Project_DataPrepKit-0.1.tar` & `Project_DataPrepKit-0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 13:21:07.207535 Project_DataPrepKit-0.1/
--rw-rw-rw-   0        0        0       64 2024-04-23 13:21:07.204538 Project_DataPrepKit-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-23 13:21:07.190534 Project_DataPrepKit-0.1/Project_DataPrepKit/
--rw-rw-rw-   0        0        0      285 2024-04-23 13:01:49.000000 Project_DataPrepKit-0.1/Project_DataPrepKit/DataEncoding.py
--rw-rw-rw-   0        0        0      293 2024-04-23 13:01:47.000000 Project_DataPrepKit-0.1/Project_DataPrepKit/DataReading.py
--rw-rw-rw-   0        0        0      303 2024-04-23 13:01:44.000000 Project_DataPrepKit-0.1/Project_DataPrepKit/DataSummaries.py
--rw-rw-rw-   0        0        0      955 2024-04-23 13:09:22.000000 Project_DataPrepKit-0.1/Project_DataPrepKit/HandleMissingValues.py
--rw-rw-rw-   0        0        0      596 2024-04-23 13:09:21.000000 Project_DataPrepKit-0.1/Project_DataPrepKit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 13:21:07.201535 Project_DataPrepKit-0.1/Project_DataPrepKit.egg-info/
--rw-rw-rw-   0        0        0       64 2024-04-23 13:21:02.000000 Project_DataPrepKit-0.1/Project_DataPrepKit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      363 2024-04-23 13:21:03.000000 Project_DataPrepKit-0.1/Project_DataPrepKit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 13:21:02.000000 Project_DataPrepKit-0.1/Project_DataPrepKit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-04-23 13:21:02.000000 Project_DataPrepKit-0.1/Project_DataPrepKit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 13:21:07.208534 Project_DataPrepKit-0.1/setup.cfg
--rw-rw-rw-   0        0        0      196 2024-04-23 13:15:37.000000 Project_DataPrepKit-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:25:00.936401 Project_DataPrepKit-0.2/
+-rw-rw-rw-   0        0        0      984 2024-04-24 09:25:00.932401 Project_DataPrepKit-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-24 09:25:00.913402 Project_DataPrepKit-0.2/Project_DataPrepKit/
+-rw-rw-rw-   0        0        0      544 2024-04-24 09:07:14.000000 Project_DataPrepKit-0.2/Project_DataPrepKit/DataEncoding.py
+-rw-rw-rw-   0        0        0      293 2024-04-23 13:01:47.000000 Project_DataPrepKit-0.2/Project_DataPrepKit/DataReading.py
+-rw-rw-rw-   0        0        0      684 2024-04-24 09:23:12.000000 Project_DataPrepKit-0.2/Project_DataPrepKit/DataSummaries.py
+-rw-rw-rw-   0        0        0      625 2024-04-24 09:17:27.000000 Project_DataPrepKit-0.2/Project_DataPrepKit/HandleMissingValues.py
+-rw-rw-rw-   0        0        0      546 2024-04-24 09:23:31.000000 Project_DataPrepKit-0.2/Project_DataPrepKit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:25:00.928401 Project_DataPrepKit-0.2/Project_DataPrepKit.egg-info/
+-rw-rw-rw-   0        0        0      984 2024-04-24 09:24:59.000000 Project_DataPrepKit-0.2/Project_DataPrepKit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      373 2024-04-24 09:25:00.000000 Project_DataPrepKit-0.2/Project_DataPrepKit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 09:24:59.000000 Project_DataPrepKit-0.2/Project_DataPrepKit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-24 09:24:59.000000 Project_DataPrepKit-0.2/Project_DataPrepKit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      866 2024-04-24 09:22:17.000000 Project_DataPrepKit-0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-24 09:25:00.937401 Project_DataPrepKit-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      343 2024-04-23 14:18:27.000000 Project_DataPrepKit-0.2/setup.py
```

### Comparing `Project_DataPrepKit-0.1/Project_DataPrepKit/HandleMissingValues.py` & `Project_DataPrepKit-0.2/Project_DataPrepKit/HandleMissingValues.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,19 @@
 import numpy as np
 
 #Handling Missing Values
-def handle_missing_values(df, strategy):
-    if strategy == 'drop':
-        clean_df = df.dropna()
-    elif strategy in ['pad', 'bfill']:
-        clean_df = df.fillna(method=strategy)
-    else:
-        raise ValueError("Invalid strategy. Choose from 'drop', 'pad', 'bfill'.")
+def handle_missing_values(data, strategy):
+if strategy == 'drop':
+        clean_data = data.dropna()
+    elif strategy in ['mean', 'median', 'mode']:
+        clean_data = data.fillna(data.agg(strategy))
+    elif strategy in ['ffill', 'bfill']:
+        clean_data = data.fillna(method=strategy)
+    else
+        raise ValueError("Invalid strategy. Choose from 'drop', 'mean', 'median', 'mode', 'ffill', 'bfill'.")
     
-    return clean_df
+    return clean_data
 
-def handle_missing_values(df, strategy, column):
-    if strategy == 'mean':
-        clean_df = df.fillna(value = df[column].mean())
-    elif strategy == 'max':
-        clean_df = df.fillna(value = df[column].max())
-    elif strategy == 'min':
-        clean_df = df.fillna(value = df[column].min())
-    else:
-        raise ValueError("Invalid strategy. Choose from 'mean', 'max', 'min'.")
+def replace_missing_values(data, newValue):
+    clean_data = data.replace(to_replace = np.nan, value = newValue)
     
-    return clean_df
-
-def replace_missing_values(df, value):
-    df2 = df.replace(to_replace = np.nan, value = value)
-    
-    return df2
-
-def interpolate_missing_values(df):
-    df2 = df.interpolate(method='linear')
+    return clean_data
```

