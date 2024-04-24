# Comparing `tmp/Project_DataPrepKit-0.3.tar.gz` & `tmp/Project_DataPrepKit-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Project_DataPrepKit-0.3.tar", last modified: Wed Apr 24 09:38:56 2024, max compression
+gzip compressed data, was "Project_DataPrepKit-0.4.tar", last modified: Wed Apr 24 09:46:02 2024, max compression
```

## Comparing `Project_DataPrepKit-0.3.tar` & `Project_DataPrepKit-0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 09:38:56.512514 Project_DataPrepKit-0.3/
--rw-rw-rw-   0        0        0      998 2024-04-24 09:38:56.509514 Project_DataPrepKit-0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-24 09:38:56.491514 Project_DataPrepKit-0.3/Project_DataPrepKit.egg-info/
--rw-rw-rw-   0        0        0      998 2024-04-24 09:38:55.000000 Project_DataPrepKit-0.3/Project_DataPrepKit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      333 2024-04-24 09:38:56.000000 Project_DataPrepKit-0.3/Project_DataPrepKit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 09:38:56.000000 Project_DataPrepKit-0.3/Project_DataPrepKit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-24 09:38:56.000000 Project_DataPrepKit-0.3/Project_DataPrepKit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      880 2024-04-24 09:37:17.000000 Project_DataPrepKit-0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 09:38:56.507514 Project_DataPrepKit-0.3/dataprepkit/
--rw-rw-rw-   0        0        0      544 2024-04-24 09:07:14.000000 Project_DataPrepKit-0.3/dataprepkit/DataEncoding.py
--rw-rw-rw-   0        0        0      293 2024-04-23 13:01:47.000000 Project_DataPrepKit-0.3/dataprepkit/DataReading.py
--rw-rw-rw-   0        0        0      684 2024-04-24 09:23:12.000000 Project_DataPrepKit-0.3/dataprepkit/DataSummaries.py
--rw-rw-rw-   0        0        0      629 2024-04-24 09:33:37.000000 Project_DataPrepKit-0.3/dataprepkit/HandleMissingValues.py
--rw-rw-rw-   0        0        0      546 2024-04-24 09:23:31.000000 Project_DataPrepKit-0.3/dataprepkit/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-24 09:38:56.512514 Project_DataPrepKit-0.3/setup.cfg
--rw-rw-rw-   0        0        0      343 2024-04-24 09:34:15.000000 Project_DataPrepKit-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:46:02.553087 Project_DataPrepKit-0.4/
+-rw-rw-rw-   0        0        0     1031 2024-04-24 09:46:02.550089 Project_DataPrepKit-0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-24 09:46:02.531086 Project_DataPrepKit-0.4/Project_DataPrepKit.egg-info/
+-rw-rw-rw-   0        0        0     1031 2024-04-24 09:46:01.000000 Project_DataPrepKit-0.4/Project_DataPrepKit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2024-04-24 09:46:02.000000 Project_DataPrepKit-0.4/Project_DataPrepKit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 09:46:01.000000 Project_DataPrepKit-0.4/Project_DataPrepKit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-24 09:46:01.000000 Project_DataPrepKit-0.4/Project_DataPrepKit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      913 2024-04-24 09:45:10.000000 Project_DataPrepKit-0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 09:46:02.547086 Project_DataPrepKit-0.4/dataprepkit/
+-rw-rw-rw-   0        0        0      544 2024-04-24 09:07:14.000000 Project_DataPrepKit-0.4/dataprepkit/DataEncoding.py
+-rw-rw-rw-   0        0        0      293 2024-04-23 13:01:47.000000 Project_DataPrepKit-0.4/dataprepkit/DataReading.py
+-rw-rw-rw-   0        0        0      684 2024-04-24 09:23:12.000000 Project_DataPrepKit-0.4/dataprepkit/DataSummaries.py
+-rw-rw-rw-   0        0        0      630 2024-04-24 09:45:31.000000 Project_DataPrepKit-0.4/dataprepkit/HandleMissingValues.py
+-rw-rw-rw-   0        0        0      546 2024-04-24 09:23:31.000000 Project_DataPrepKit-0.4/dataprepkit/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-24 09:46:02.554086 Project_DataPrepKit-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      343 2024-04-24 09:45:53.000000 Project_DataPrepKit-0.4/setup.py
```

### Comparing `Project_DataPrepKit-0.3/PKG-INFO` & `Project_DataPrepKit-0.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: Project_DataPrepKit
-Version: 0.3
+Version: 0.4
 Description-Content-Type: text/markdown
 
 # DataPrepKit
-**this project is made for the "Python Programming Foundation" course from [Electro PI](electropi.ai)**
+**this project is made for the "Python Programming Foundation" course from [Electro PI](https://electropi.ai/ "Go To Electro PI page")**
 
 ## Key Features:
 - Read files of type CSV, Excel, and JSON, using "DataReading" class.
 - Use "DataSummaries" class to create summaries for data frames, or get each individual summary value for mean, median, mode, standard deviation, number of values, minimum value, maximum value, and frequent values.
 - Clean up data bases with "HandleMissingValues"  class using one of these cleaning strategies: 'drop', 'mean', 'median', 'mode', 'ffill', 'bfill', or replace the missing values with a value of your choice using the "replace_missing_values" method.
 - Encode categorical data  using 'one-hot' strategy, or using 'label' from class "DataEncoding".
```

### Comparing `Project_DataPrepKit-0.3/Project_DataPrepKit.egg-info/PKG-INFO` & `Project_DataPrepKit-0.4/Project_DataPrepKit.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: Project-DataPrepKit
-Version: 0.3
+Version: 0.4
 Description-Content-Type: text/markdown
 
 # DataPrepKit
-**this project is made for the "Python Programming Foundation" course from [Electro PI](electropi.ai)**
+**this project is made for the "Python Programming Foundation" course from [Electro PI](https://electropi.ai/ "Go To Electro PI page")**
 
 ## Key Features:
 - Read files of type CSV, Excel, and JSON, using "DataReading" class.
 - Use "DataSummaries" class to create summaries for data frames, or get each individual summary value for mean, median, mode, standard deviation, number of values, minimum value, maximum value, and frequent values.
 - Clean up data bases with "HandleMissingValues"  class using one of these cleaning strategies: 'drop', 'mean', 'median', 'mode', 'ffill', 'bfill', or replace the missing values with a value of your choice using the "replace_missing_values" method.
 - Encode categorical data  using 'one-hot' strategy, or using 'label' from class "DataEncoding".
```

### Comparing `Project_DataPrepKit-0.3/README.md` & `Project_DataPrepKit-0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # DataPrepKit
-**this project is made for the "Python Programming Foundation" course from [Electro PI](electropi.ai)**
+**this project is made for the "Python Programming Foundation" course from [Electro PI](https://electropi.ai/ "Go To Electro PI page")**
 
 ## Key Features:
 - Read files of type CSV, Excel, and JSON, using "DataReading" class.
 - Use "DataSummaries" class to create summaries for data frames, or get each individual summary value for mean, median, mode, standard deviation, number of values, minimum value, maximum value, and frequent values.
 - Clean up data bases with "HandleMissingValues"  class using one of these cleaning strategies: 'drop', 'mean', 'median', 'mode', 'ffill', 'bfill', or replace the missing values with a value of your choice using the "replace_missing_values" method.
 - Encode categorical data  using 'one-hot' strategy, or using 'label' from class "DataEncoding".
```

### Comparing `Project_DataPrepKit-0.3/dataprepkit/DataEncoding.py` & `Project_DataPrepKit-0.4/dataprepkit/DataEncoding.py`

 * *Files identical despite different names*

### Comparing `Project_DataPrepKit-0.3/dataprepkit/DataSummaries.py` & `Project_DataPrepKit-0.4/dataprepkit/DataSummaries.py`

 * *Files identical despite different names*

### Comparing `Project_DataPrepKit-0.3/dataprepkit/HandleMissingValues.py` & `Project_DataPrepKit-0.4/dataprepkit/HandleMissingValues.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def handle_missing_values(data, strategy):
     if strategy == 'drop':
         clean_data = data.dropna()
     elif strategy in ['mean', 'median', 'mode']:
         clean_data = data.fillna(data.agg(strategy))
     elif strategy in ['ffill', 'bfill']:
         clean_data = data.fillna(method=strategy)
-    else
+    else:
         raise ValueError("Invalid strategy. Choose from 'drop', 'mean', 'median', 'mode', 'ffill', 'bfill'.")
     
     return clean_data
 
 def replace_missing_values(data, newValue):
     clean_data = data.replace(to_replace = np.nan, value = newValue)
```

### Comparing `Project_DataPrepKit-0.3/dataprepkit/__init__.py` & `Project_DataPrepKit-0.4/dataprepkit/__init__.py`

 * *Files identical despite different names*

