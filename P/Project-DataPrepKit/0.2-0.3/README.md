# Comparing `tmp/Project_DataPrepKit-0.2.tar.gz` & `tmp/Project_DataPrepKit-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Project_DataPrepKit-0.2.tar", last modified: Wed Apr 24 09:25:00 2024, max compression
+gzip compressed data, was "Project_DataPrepKit-0.3.tar", last modified: Wed Apr 24 09:38:56 2024, max compression
```

## Comparing `Project_DataPrepKit-0.2.tar` & `Project_DataPrepKit-0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 09:25:00.936401 Project_DataPrepKit-0.2/
--rw-rw-rw-   0        0        0      984 2024-04-24 09:25:00.932401 Project_DataPrepKit-0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-24 09:25:00.913402 Project_DataPrepKit-0.2/Project_DataPrepKit/
--rw-rw-rw-   0        0        0      544 2024-04-24 09:07:14.000000 Project_DataPrepKit-0.2/Project_DataPrepKit/DataEncoding.py
--rw-rw-rw-   0        0        0      293 2024-04-23 13:01:47.000000 Project_DataPrepKit-0.2/Project_DataPrepKit/DataReading.py
--rw-rw-rw-   0        0        0      684 2024-04-24 09:23:12.000000 Project_DataPrepKit-0.2/Project_DataPrepKit/DataSummaries.py
--rw-rw-rw-   0        0        0      625 2024-04-24 09:17:27.000000 Project_DataPrepKit-0.2/Project_DataPrepKit/HandleMissingValues.py
--rw-rw-rw-   0        0        0      546 2024-04-24 09:23:31.000000 Project_DataPrepKit-0.2/Project_DataPrepKit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 09:25:00.928401 Project_DataPrepKit-0.2/Project_DataPrepKit.egg-info/
--rw-rw-rw-   0        0        0      984 2024-04-24 09:24:59.000000 Project_DataPrepKit-0.2/Project_DataPrepKit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      373 2024-04-24 09:25:00.000000 Project_DataPrepKit-0.2/Project_DataPrepKit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 09:24:59.000000 Project_DataPrepKit-0.2/Project_DataPrepKit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-04-24 09:24:59.000000 Project_DataPrepKit-0.2/Project_DataPrepKit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      866 2024-04-24 09:22:17.000000 Project_DataPrepKit-0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-24 09:25:00.937401 Project_DataPrepKit-0.2/setup.cfg
--rw-rw-rw-   0        0        0      343 2024-04-23 14:18:27.000000 Project_DataPrepKit-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:38:56.512514 Project_DataPrepKit-0.3/
+-rw-rw-rw-   0        0        0      998 2024-04-24 09:38:56.509514 Project_DataPrepKit-0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-24 09:38:56.491514 Project_DataPrepKit-0.3/Project_DataPrepKit.egg-info/
+-rw-rw-rw-   0        0        0      998 2024-04-24 09:38:55.000000 Project_DataPrepKit-0.3/Project_DataPrepKit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2024-04-24 09:38:56.000000 Project_DataPrepKit-0.3/Project_DataPrepKit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 09:38:56.000000 Project_DataPrepKit-0.3/Project_DataPrepKit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-24 09:38:56.000000 Project_DataPrepKit-0.3/Project_DataPrepKit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      880 2024-04-24 09:37:17.000000 Project_DataPrepKit-0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 09:38:56.507514 Project_DataPrepKit-0.3/dataprepkit/
+-rw-rw-rw-   0        0        0      544 2024-04-24 09:07:14.000000 Project_DataPrepKit-0.3/dataprepkit/DataEncoding.py
+-rw-rw-rw-   0        0        0      293 2024-04-23 13:01:47.000000 Project_DataPrepKit-0.3/dataprepkit/DataReading.py
+-rw-rw-rw-   0        0        0      684 2024-04-24 09:23:12.000000 Project_DataPrepKit-0.3/dataprepkit/DataSummaries.py
+-rw-rw-rw-   0        0        0      629 2024-04-24 09:33:37.000000 Project_DataPrepKit-0.3/dataprepkit/HandleMissingValues.py
+-rw-rw-rw-   0        0        0      546 2024-04-24 09:23:31.000000 Project_DataPrepKit-0.3/dataprepkit/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-24 09:38:56.512514 Project_DataPrepKit-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      343 2024-04-24 09:34:15.000000 Project_DataPrepKit-0.3/setup.py
```

### Comparing `Project_DataPrepKit-0.2/PKG-INFO` & `Project_DataPrepKit-0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: Project_DataPrepKit
-Version: 0.2
+Version: 0.3
 Description-Content-Type: text/markdown
 
 # DataPrepKit
-**this project is made for the "Python Programming Foundation" course from electropi.ai**
+**this project is made for the "Python Programming Foundation" course from [Electro PI](electropi.ai)**
 
 ## Key Features:
 - Read files of type CSV, Excel, and JSON, using "DataReading" class.
 - Use "DataSummaries" class to create summaries for data frames, or get each individual summary value for mean, median, mode, standard deviation, number of values, minimum value, maximum value, and frequent values.
 - Clean up data bases with "HandleMissingValues"  class using one of these cleaning strategies: 'drop', 'mean', 'median', 'mode', 'ffill', 'bfill', or replace the missing values with a value of your choice using the "replace_missing_values" method.
 - Encode categorical data  using 'one-hot' strategy, or using 'label' from class "DataEncoding".
 
-All classes are methods are imported in the initial files, so there is no need to import each method seperately!
+All classes and methods are imported in the initial files, so there is no need to import each method seperately!
```

### Comparing `Project_DataPrepKit-0.2/Project_DataPrepKit/DataEncoding.py` & `Project_DataPrepKit-0.3/dataprepkit/DataEncoding.py`

 * *Files identical despite different names*

### Comparing `Project_DataPrepKit-0.2/Project_DataPrepKit/DataSummaries.py` & `Project_DataPrepKit-0.3/dataprepkit/DataSummaries.py`

 * *Files identical despite different names*

### Comparing `Project_DataPrepKit-0.2/Project_DataPrepKit/HandleMissingValues.py` & `Project_DataPrepKit-0.3/dataprepkit/HandleMissingValues.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 
 #Handling Missing Values
 def handle_missing_values(data, strategy):
-if strategy == 'drop':
+    if strategy == 'drop':
         clean_data = data.dropna()
     elif strategy in ['mean', 'median', 'mode']:
         clean_data = data.fillna(data.agg(strategy))
     elif strategy in ['ffill', 'bfill']:
         clean_data = data.fillna(method=strategy)
     else
         raise ValueError("Invalid strategy. Choose from 'drop', 'mean', 'median', 'mode', 'ffill', 'bfill'.")
```

### Comparing `Project_DataPrepKit-0.2/Project_DataPrepKit/__init__.py` & `Project_DataPrepKit-0.3/dataprepkit/__init__.py`

 * *Files identical despite different names*

### Comparing `Project_DataPrepKit-0.2/Project_DataPrepKit.egg-info/PKG-INFO` & `Project_DataPrepKit-0.3/Project_DataPrepKit.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: Project-DataPrepKit
-Version: 0.2
+Version: 0.3
 Description-Content-Type: text/markdown
 
 # DataPrepKit
-**this project is made for the "Python Programming Foundation" course from electropi.ai**
+**this project is made for the "Python Programming Foundation" course from [Electro PI](electropi.ai)**
 
 ## Key Features:
 - Read files of type CSV, Excel, and JSON, using "DataReading" class.
 - Use "DataSummaries" class to create summaries for data frames, or get each individual summary value for mean, median, mode, standard deviation, number of values, minimum value, maximum value, and frequent values.
 - Clean up data bases with "HandleMissingValues"  class using one of these cleaning strategies: 'drop', 'mean', 'median', 'mode', 'ffill', 'bfill', or replace the missing values with a value of your choice using the "replace_missing_values" method.
 - Encode categorical data  using 'one-hot' strategy, or using 'label' from class "DataEncoding".
 
-All classes are methods are imported in the initial files, so there is no need to import each method seperately!
+All classes and methods are imported in the initial files, so there is no need to import each method seperately!
```

### Comparing `Project_DataPrepKit-0.2/README.md` & `Project_DataPrepKit-0.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DataPrepKit
-**this project is made for the "Python Programming Foundation" course from electropi.ai**
+**this project is made for the "Python Programming Foundation" course from [Electro PI](electropi.ai)**
 
 ## Key Features:
 - Read files of type CSV, Excel, and JSON, using "DataReading" class.
 - Use "DataSummaries" class to create summaries for data frames, or get each individual summary value for mean, median, mode, standard deviation, number of values, minimum value, maximum value, and frequent values.
 - Clean up data bases with "HandleMissingValues"  class using one of these cleaning strategies: 'drop', 'mean', 'median', 'mode', 'ffill', 'bfill', or replace the missing values with a value of your choice using the "replace_missing_values" method.
 - Encode categorical data  using 'one-hot' strategy, or using 'label' from class "DataEncoding".
 
-All classes are methods are imported in the initial files, so there is no need to import each method seperately!
+All classes and methods are imported in the initial files, so there is no need to import each method seperately!
```

