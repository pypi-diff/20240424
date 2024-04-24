# Comparing `tmp/cnspy_csv2dataframe-0.1.1.tar.gz` & `tmp/cnspy_csv2dataframe-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/jungr/workspace/CNS/VIO_Evaluation_Framework/py3_pkgs/cnspy_eco_system_test/pkgs/d_csv2dataframe/dist/tmpk6bcirm3/cnspy_c", last modified: Sat Mar 20 14:23:48 2021, max compression
+gzip compressed data, was "cnspy_csv2dataframe-0.2.0.tar", last modified: Wed Apr 24 12:16:54 2024, max compression
```

## Comparing `cnspy_csv2dataframe-0.1.1.tar` & `cnspy_csv2dataframe-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,33 @@
-drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2021-03-20 14:23:48.330450 cnspy_csv2dataframe-0.1.1/
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     2677 2021-03-20 14:23:48.330450 cnspy_csv2dataframe-0.1.1/PKG-INFO
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     1704 2021-03-20 14:21:27.000000 cnspy_csv2dataframe-0.1.1/README.md
-drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2021-03-20 14:23:48.326450 cnspy_csv2dataframe-0.1.1/cnspy_csv2dataframe/
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     4209 2021-03-20 12:20:48.000000 cnspy_csv2dataframe-0.1.1/cnspy_csv2dataframe/CSV2DataFrame.py
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     1244 2021-03-20 12:20:48.000000 cnspy_csv2dataframe-0.1.1/cnspy_csv2dataframe/PoseCovCSV2DataFrame.py
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     4512 2021-03-20 12:20:48.000000 cnspy_csv2dataframe-0.1.1/cnspy_csv2dataframe/PoseWithCov2DataFrame.py
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     3017 2021-03-20 12:20:48.000000 cnspy_csv2dataframe-0.1.1/cnspy_csv2dataframe/TUMCSV2DataFrame.py
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     1551 2021-03-20 12:20:48.000000 cnspy_csv2dataframe-0.1.1/cnspy_csv2dataframe/TimestampCSV2DataFrame.py
--rw-rw-r--   0 jungr     (1000) jungr     (1000)        0 2021-03-20 12:20:48.000000 cnspy_csv2dataframe-0.1.1/cnspy_csv2dataframe/__init__.py
-drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2021-03-20 14:23:48.330450 cnspy_csv2dataframe-0.1.1/cnspy_csv2dataframe.egg-info/
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     2677 2021-03-20 14:23:48.000000 cnspy_csv2dataframe-0.1.1/cnspy_csv2dataframe.egg-info/PKG-INFO
--rw-rw-r--   0 jungr     (1000) jungr     (1000)      621 2021-03-20 14:23:48.000000 cnspy_csv2dataframe-0.1.1/cnspy_csv2dataframe.egg-info/SOURCES.txt
--rw-rw-r--   0 jungr     (1000) jungr     (1000)        1 2021-03-20 14:23:48.000000 cnspy_csv2dataframe-0.1.1/cnspy_csv2dataframe.egg-info/dependency_links.txt
--rw-rw-r--   0 jungr     (1000) jungr     (1000)       57 2021-03-20 14:23:48.000000 cnspy_csv2dataframe-0.1.1/cnspy_csv2dataframe.egg-info/requires.txt
--rw-rw-r--   0 jungr     (1000) jungr     (1000)       25 2021-03-20 14:23:48.000000 cnspy_csv2dataframe-0.1.1/cnspy_csv2dataframe.egg-info/top_level.txt
--rw-rw-r--   0 jungr     (1000) jungr     (1000)       38 2021-03-20 14:23:48.330450 cnspy_csv2dataframe-0.1.1/setup.cfg
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     1302 2021-03-20 14:21:27.000000 cnspy_csv2dataframe-0.1.1/setup.py
-drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2021-03-20 14:23:48.330450 cnspy_csv2dataframe-0.1.1/test/
--rw-rw-r--   0 jungr     (1000) jungr     (1000)        0 2021-03-20 12:20:48.000000 cnspy_csv2dataframe-0.1.1/test/__init__.py
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     1869 2021-03-20 12:20:48.000000 cnspy_csv2dataframe-0.1.1/test/test_CSV2DataFrame.py
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     2059 2021-03-20 12:20:48.000000 cnspy_csv2dataframe-0.1.1/test/test_PoseWithCov2DataFrame.py
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     3251 2021-03-20 12:20:48.000000 cnspy_csv2dataframe-0.1.1/test/test_TUMCSV2DataFrame.py
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     1582 2021-03-20 12:20:48.000000 cnspy_csv2dataframe-0.1.1/test/test_TimestampCSV2DataFrame.py
+drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2024-04-24 12:16:54.113237 cnspy_csv2dataframe-0.2.0/
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)    35149 2022-05-30 14:10:28.000000 cnspy_csv2dataframe-0.2.0/LICENCE
+-rw-r--r--   0 jungr     (1000) jungr     (1000)     2614 2024-04-24 12:16:54.113237 cnspy_csv2dataframe-0.2.0/PKG-INFO
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     1854 2024-04-24 11:46:06.000000 cnspy_csv2dataframe-0.2.0/README.md
+drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2024-04-24 12:16:54.113237 cnspy_csv2dataframe-0.2.0/cnspy_csv2dataframe/
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     5769 2024-04-24 11:46:06.000000 cnspy_csv2dataframe-0.2.0/cnspy_csv2dataframe/CSV2DataFrame.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     1295 2024-04-24 11:46:06.000000 cnspy_csv2dataframe-0.2.0/cnspy_csv2dataframe/PosOrientCovCSV2DataFrame.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     4099 2024-04-24 11:46:06.000000 cnspy_csv2dataframe-0.2.0/cnspy_csv2dataframe/PosOrientWithCov2DataFrame.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     2843 2024-04-24 11:46:06.000000 cnspy_csv2dataframe-0.2.0/cnspy_csv2dataframe/PosOrientWithCovTyped2DataFrame.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     3398 2024-04-24 11:46:06.000000 cnspy_csv2dataframe-0.2.0/cnspy_csv2dataframe/PoseErrorStamped2DataFrame.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     2849 2024-04-24 11:46:06.000000 cnspy_csv2dataframe-0.2.0/cnspy_csv2dataframe/PoseTypedStamped2DataFrame.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     4127 2024-04-24 11:46:06.000000 cnspy_csv2dataframe-0.2.0/cnspy_csv2dataframe/PoseWithCov2DataFrame.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     2705 2024-04-24 11:46:06.000000 cnspy_csv2dataframe-0.2.0/cnspy_csv2dataframe/PoseWithCovTyped2DataFrame.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     3045 2024-04-24 11:46:06.000000 cnspy_csv2dataframe-0.2.0/cnspy_csv2dataframe/TUMCSV2DataFrame.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     1566 2024-04-24 11:46:06.000000 cnspy_csv2dataframe-0.2.0/cnspy_csv2dataframe/TimestampCSV2DataFrame.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)        0 2022-05-30 14:10:28.000000 cnspy_csv2dataframe-0.2.0/cnspy_csv2dataframe/__init__.py
+drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2024-04-24 12:16:54.113237 cnspy_csv2dataframe-0.2.0/cnspy_csv2dataframe.egg-info/
+-rw-r--r--   0 jungr     (1000) jungr     (1000)     2614 2024-04-24 12:16:54.000000 cnspy_csv2dataframe-0.2.0/cnspy_csv2dataframe.egg-info/PKG-INFO
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     1014 2024-04-24 12:16:54.000000 cnspy_csv2dataframe-0.2.0/cnspy_csv2dataframe.egg-info/SOURCES.txt
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)        1 2024-04-24 12:16:54.000000 cnspy_csv2dataframe-0.2.0/cnspy_csv2dataframe.egg-info/dependency_links.txt
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)       57 2024-04-24 12:16:54.000000 cnspy_csv2dataframe-0.2.0/cnspy_csv2dataframe.egg-info/requires.txt
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)       25 2024-04-24 12:16:54.000000 cnspy_csv2dataframe-0.2.0/cnspy_csv2dataframe.egg-info/top_level.txt
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)       38 2024-04-24 12:16:54.113237 cnspy_csv2dataframe-0.2.0/setup.cfg
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     1302 2022-05-30 14:10:28.000000 cnspy_csv2dataframe-0.2.0/setup.py
+drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2024-04-24 12:16:54.113237 cnspy_csv2dataframe-0.2.0/test/
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)        0 2022-05-30 14:10:28.000000 cnspy_csv2dataframe-0.2.0/test/__init__.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     3652 2024-04-24 11:46:06.000000 cnspy_csv2dataframe-0.2.0/test/test_CSV2DataFrame.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     3188 2024-04-24 11:46:06.000000 cnspy_csv2dataframe-0.2.0/test/test_PosOrientWithCov2DataFrame.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     2747 2024-04-24 11:46:06.000000 cnspy_csv2dataframe-0.2.0/test/test_PosOrientWithCovTyped2DataFrame.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     2280 2024-04-24 11:46:06.000000 cnspy_csv2dataframe-0.2.0/test/test_PoseWithCov2DataFrame.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     2461 2024-04-24 11:46:06.000000 cnspy_csv2dataframe-0.2.0/test/test_PoseWithCovTyped2DataFrame.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     3273 2024-04-24 11:46:06.000000 cnspy_csv2dataframe-0.2.0/test/test_TUMCSV2DataFrame.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     1582 2022-05-30 14:10:28.000000 cnspy_csv2dataframe-0.2.0/test/test_TimestampCSV2DataFrame.py
```

### Comparing `cnspy_csv2dataframe-0.1.1/PKG-INFO` & `cnspy_csv2dataframe-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,63 @@
 Metadata-Version: 2.1
 Name: cnspy_csv2dataframe
-Version: 0.1.1
+Version: 0.2.0
 Summary: CSV to pandas.Dataframe converter
 Home-page: https://github.com/aau-cns/cnspy_csv2dataframe/
 Author: Roland Jung
 Author-email: roland.jung@aau.at
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/aau-cns/cnspy_csv2dataframe/issues
-Description: # cnspy_csv2dataframe
-        
-        
-        The class [CSV2DataFrame](./cnspy_csv2dataframe/CSV2DataFrame.py) is intended to load [CSV-files](https://en.wikipedia.org/wiki/Comma-separated_values) into a `pandas.DataFrame`. The CSV files need to match known formats (defined by their header in the first line) according to those defined in the package [spatial_csv_formats]().
-          
-        In case no format is specified, it tries to match the first line of the CSV-File with known headers from [cnspy_spatial_csv_formats](https://github.com/aau-cns/cnspy_spatial_csv_formats) and loads the data in that format. 
-        
-        There a some specialization of  [CSV2DataFrame](./cnspy_csv2dataframe/CSV2DataFrame.py) that support different operations on the data:
-        * [PoseCovCSV2DataFrame](./cnspy_csv2dataframe/PoseCovCSV2DataFrame.py)
-        * [PoseWithCov2DataFrame](./cnspy_csv2dataframe/PoseWithCov2DataFrame.py)
-        * [TimestampCSV2DataFrame](./cnspy_csv2dataframe/TimestampCSV2DataFrame.py)
-        * [TUMCSV2DataFrame](./cnspy_csv2dataframe/TUMCSV2DataFrame.py)
-        
-        ## Installation
-        
-        Install the current code base from GitHub and pip install a link to that cloned copy
-        ```
-        git clone https://github.com/aau-cns/csv2dataframe.git
-        cd csv2dataframe
-        pip install -e .
-        ```
-        
-        ## Dependencies
-        
-        It is part of the [cnspy eco-system](hhttps://github.com/aau-cns/cnspy_eco_system_test) of the [cns-github](https://github.com/aau-cns) group.  
-        
-        * [numpy]()
-        * [pandas]()
-        * [cnspy_spatial_csv_formats](https://github.com/aau-cns/cnspy_spatial_csv_formats)
-        * [cnspy_numpy_utils](https://github.com/aau-cns/cnspy_numpy_utils)
-        
-        
-        ## License
-        
-        
-        Software License Agreement (GNU GPLv3  License), refer to the LICENSE file.
-        
-        *Sharing is caring!* - [Roland Jung](https://github.com/jungr-ait)
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENCE
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: cnspy_numpy_utils
+Requires-Dist: cnspy_spatial_csv_formats
+
+# cnspy_csv2dataframe
+
+
+The class [CSV2DataFrame](./cnspy_csv2dataframe/CSV2DataFrame.py) is intended to load [CSV-files](https://en.wikipedia.org/wiki/Comma-separated_values) into a `pandas.DataFrame`. The CSV files need to match known formats (defined by their header in the first line) according to those defined in the package [spatial_csv_formats]().
+  
+In case no format is specified, it tries to match the first line of the CSV-File with known headers from [cnspy_spatial_csv_formats](https://github.com/aau-cns/cnspy_spatial_csv_formats) and loads the data in that format. 
+
+There a some specialization of  [CSV2DataFrame](./cnspy_csv2dataframe/CSV2DataFrame.py) that support different operations on the data:
+* [PoseCovCSV2DataFrame](./cnspy_csv2dataframe/PosOrientCovCSV2DataFrame.py)
+* [PoseWithCov2DataFrame](./cnspy_csv2dataframe/PosOrientWithCov2DataFrame.py)
+* [TimestampCSV2DataFrame](./cnspy_csv2dataframe/TimestampCSV2DataFrame.py)
+* [TUMCSV2DataFrame](./cnspy_csv2dataframe/TUMCSV2DataFrame.py)
+
+## Installation
+
+Install the current code base from GitHub and pip install a link to that cloned copy
+```
+git clone https://github.com/aau-cns/cnspy_csv2dataframe.git
+cd cnspy_csv2dataframe
+pip install -e .
+```
+or the [official package](https://pypi.org/project/cnspy-csv2dataframe/) via
+```commandline
+pip install cnspy-csv2dataframe
+```
+
+## Dependencies
+
+It is part of the [cnspy eco-system](hhttps://github.com/aau-cns/cnspy_eco_system_test) of the [cns-github](https://github.com/aau-cns) group.  
+
+* [numpy]()
+* [pandas]()
+* [cnspy_spatial_csv_formats](https://github.com/aau-cns/cnspy_spatial_csv_formats)
+* [cnspy_numpy_utils](https://github.com/aau-cns/cnspy_numpy_utils)
+
+
+## License
+
+
+Software License Agreement (GNU GPLv3  License), refer to the LICENSE file.
+
+*Sharing is caring!* - [Roland Jung](https://github.com/jungr-ait)
```

### Comparing `cnspy_csv2dataframe-0.1.1/README.md` & `cnspy_csv2dataframe-0.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -2,27 +2,31 @@
 
 
 The class [CSV2DataFrame](./cnspy_csv2dataframe/CSV2DataFrame.py) is intended to load [CSV-files](https://en.wikipedia.org/wiki/Comma-separated_values) into a `pandas.DataFrame`. The CSV files need to match known formats (defined by their header in the first line) according to those defined in the package [spatial_csv_formats]().
   
 In case no format is specified, it tries to match the first line of the CSV-File with known headers from [cnspy_spatial_csv_formats](https://github.com/aau-cns/cnspy_spatial_csv_formats) and loads the data in that format. 
 
 There a some specialization of  [CSV2DataFrame](./cnspy_csv2dataframe/CSV2DataFrame.py) that support different operations on the data:
-* [PoseCovCSV2DataFrame](./cnspy_csv2dataframe/PoseCovCSV2DataFrame.py)
-* [PoseWithCov2DataFrame](./cnspy_csv2dataframe/PoseWithCov2DataFrame.py)
+* [PoseCovCSV2DataFrame](./cnspy_csv2dataframe/PosOrientCovCSV2DataFrame.py)
+* [PoseWithCov2DataFrame](./cnspy_csv2dataframe/PosOrientWithCov2DataFrame.py)
 * [TimestampCSV2DataFrame](./cnspy_csv2dataframe/TimestampCSV2DataFrame.py)
 * [TUMCSV2DataFrame](./cnspy_csv2dataframe/TUMCSV2DataFrame.py)
 
 ## Installation
 
 Install the current code base from GitHub and pip install a link to that cloned copy
 ```
-git clone https://github.com/aau-cns/csv2dataframe.git
-cd csv2dataframe
+git clone https://github.com/aau-cns/cnspy_csv2dataframe.git
+cd cnspy_csv2dataframe
 pip install -e .
 ```
+or the [official package](https://pypi.org/project/cnspy-csv2dataframe/) via
+```commandline
+pip install cnspy-csv2dataframe
+```
 
 ## Dependencies
 
 It is part of the [cnspy eco-system](hhttps://github.com/aau-cns/cnspy_eco_system_test) of the [cns-github](https://github.com/aau-cns) group.  
 
 * [numpy]()
 * [pandas]()
```

### Comparing `cnspy_csv2dataframe-0.1.1/cnspy_csv2dataframe/CSV2DataFrame.py` & `cnspy_csv2dataframe-0.2.0/cnspy_csv2dataframe/CSV2DataFrame.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,99 +19,118 @@
 # Requirements:
 # sudo pip install numpy pandas
 ########################################################################################################################
 import os
 import math
 import pandas as pandas
 import numpy as np
-from cnspy_spatial_csv_formats.CSVFormatPose import CSVFormatPose
+from cnspy_spatial_csv_formats.CSVSpatialFormatType import CSVSpatialFormatType
 
 
 class CSV2DataFrame:
-    format = CSVFormatPose.none
+    format = CSVSpatialFormatType.none
     data_frame = None
     data_loaded = False
     fn = None
 
-    def __init__(self, filename=None, fmt=None):
-        if filename is None:
-            pass  # Do nothing.. data can be loaded later on!
-        else:
-            self.load_from_CSV(fn=filename, fmt=fmt)
+    def __init__(self, fn=None, fmt=None):
+        # fmt allows manually overwrite expected format to be parsed into dataframe
+        if fn is not None:
+            self.load_from_CSV(fn=fn, fmt_type=fmt)
 
-    def subsample(self, step=None, num_max_points=None):
+    def subsample(self, step=None, num_max_points=None, verbose=False):
         if self.data_loaded:
             self.data_frame = CSV2DataFrame.subsample_DataFrame(self.data_frame, step=step,
-                                                                num_max_points=num_max_points)
+                                                                num_max_points=num_max_points,
+                                                                verbose=verbose)
         else:
             print("CSV2DataFrame: data was not loaded!")
 
-    def load_from_CSV(self, fn, fmt=None):
+    def load_from_CSV(self, fn, fmt_type=None):
         if os.path.exists(fn):
-            if fmt is not None:
-                fmt_ = fmt
-            elif fmt is None and self.format is not CSVFormatPose.none:
-                fmt_ = self.format
-            else:
-                fmt_ = CSVFormatPose.identify_format(fn)
-
-            if fmt_ is not CSVFormatPose.none:
-                self.data_frame = CSV2DataFrame.load_CSV(filename=fn, fmt=fmt_)
-                self.fn = fn
-                self.data_loaded = True
-                self.format = fmt_
-                return True
+            # if the format is still not known it cannot be loaded, if it is None than it will be identified
+            self.data_frame, self.format = CSV2DataFrame.load_CSV(filename=fn, fmt=fmt_type)
+            self.fn = fn
+            self.data_loaded = True
+            return True
         else:
             print("CSV2DataFrame.load_from_CSV(): file does not exist: {0}".format(fn))
+
+        # default assignment
+        self.data_frame = None
+        self.fn = None
+        self.data_loaded = False
+        self.format = CSVSpatialFormatType.none
         return False
 
     def save_to_CSV(self, fn, fmt=None):
-        if fmt is None:
-            fmt_ = self.format
-
         if self.data_loaded:
-            CSV2DataFrame.save_CSV(data_frame=self.data_frame, filename=fn, fmt=fmt_)
+            CSV2DataFrame.save_CSV(data_frame=self.data_frame, filename=fn, fmt=fmt)
         else:
             print("CSV2DataFrame: data was not loaded!")
 
     @staticmethod
-    def load_CSV(filename, fmt):
-        data = pandas.read_csv(filename, sep='\s+|\,', comment='#', header=None, names=CSVFormatPose.get_format(fmt),
-                               engine='python')
-        return data
+    def identify_format(dataframe):
+        if isinstance(dataframe, pandas.DataFrame):
+            return CSVSpatialFormatType.header_to_format_type(','.join(dataframe.keys().values))
+        return CSVSpatialFormatType.none
+
+    @staticmethod
+    def load_CSV(filename, fmt=None):
+        if isinstance(fmt, CSVSpatialFormatType) and fmt is not CSVSpatialFormatType.none:
+            data = pandas.read_csv(filename, sep='\s+|\,', comment='#', header=None,
+                                   names=CSVSpatialFormatType.get_format(fmt),
+                                   engine='python')
+        else:
+            data = pandas.read_csv(filename, sep='\s+|\,', comment='#',
+                                   engine='python')
+            fmt = CSV2DataFrame.identify_format(data)
+        return data, fmt
 
     @staticmethod
-    def save_CSV(data_frame, filename, fmt, save_index=False):
+    def save_CSV(data_frame, filename, fmt=None, save_index=False):
         head = os.path.dirname(os.path.abspath(filename))
         if not os.path.exists(head):
             os.makedirs(head)
 
-        data_frame.to_csv(filename, sep=',', index=save_index,
-                          header=CSVFormatPose.get_header(fmt),
-                          columns=CSVFormatPose.get_format(fmt))
+        if isinstance(fmt, CSVSpatialFormatType) and fmt is not CSVSpatialFormatType.none:
+            data_frame.to_csv(filename, sep=',', index=save_index,
+                              header=CSVSpatialFormatType.get_header(fmt),
+                              columns=CSVSpatialFormatType.get_format(fmt))
+        else:
+            data_frame.to_csv(filename, sep=',', index=save_index)
 
     @staticmethod
     def subsample_DataFrame(df, step=None, num_max_points=None, verbose=False):
 
         num_elems = len(df.index)
 
         if num_max_points:
             step = 1
             if (int(num_max_points) > 0) and (int(num_max_points) < num_elems):
                 step = int(math.ceil(num_elems / float(num_max_points)))
 
         sparse_indices = np.arange(start=0, stop=num_elems, step=step)
 
-        if (num_max_points or step):
+        if num_max_points or step:
             if verbose:
                 print("CSV2DataFrame.subsample_DataFrame():")
                 print("* len: " + str(num_elems) + ", max_num_points: " + str(
                     num_max_points) + ", subsample by: " + str(step))
 
-            df_sub = df.loc[sparse_indices]
-            df_sub.reset_index(inplace=True)
-
-            return df_sub
-
+            return CSV2DataFrame.sample_DataFrame(df, sparse_indices)
         else:
             return df
 
+    @staticmethod
+    def sample_DataFrame(df, indices_arr):
+        num_elems = len(df.index)
+        assert (len(indices_arr) <= num_elems), "CSV2DataFrame.sample_DataFrame():\n\t index array must be smaller " \
+                                                    "equal the dataframe."
+        assert (max(indices_arr) <= num_elems), "CSV2DataFrame.sample_DataFrame():\n\t elements in the index array " \
+                                                    "must be smaller equal the dataframe."
+        assert (min(indices_arr) >= 0), "CSV2DataFrame.sample_DataFrame():\n\t elemts in the index array " \
+                                                    "must be greater equal zero."
+
+        df_sub = df.iloc[indices_arr]
+        df_sub.reset_index(inplace=True, drop=True)
+        return df_sub
```

### Comparing `cnspy_csv2dataframe-0.1.1/cnspy_csv2dataframe/PoseCovCSV2DataFrame.py` & `cnspy_csv2dataframe-0.2.0/cnspy_csv2dataframe/PosOrientCovCSV2DataFrame.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
 # Requirements:
 # sudo pip install numpy pandas
 ########################################################################################################################
 import os
-from cnspy_spatial_csv_formats.CSVFormatPose import CSVFormatPose
+from cnspy_spatial_csv_formats.CSVSpatialFormatType import CSVSpatialFormatType
 from cnspy_csv2dataframe.CSV2DataFrame import CSV2DataFrame
 
 
-class PoseCovCSV2DataFrame(CSV2DataFrame):
+class PosOrientCovCSV2DataFrame(CSV2DataFrame):
     def __init__(self, fn=None):
-        CSV2DataFrame.__init__(self, filename=fn, fmt=CSVFormatPose.PoseCov)
+        # identify the covariance format via fmt=None!
+        CSV2DataFrame.__init__(self, fn=fn, fmt=None)
```

### Comparing `cnspy_csv2dataframe-0.1.1/cnspy_csv2dataframe/PoseWithCov2DataFrame.py` & `cnspy_csv2dataframe-0.2.0/cnspy_csv2dataframe/PosOrientWithCov2DataFrame.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,37 +19,38 @@
 # Requirements:
 # sudo pip install numpy pandas
 ########################################################################################################################
 import os
 from sys import version_info
 import pandas as pandas
 import numpy as np
-from cnspy_spatial_csv_formats.CSVFormatPose import CSVFormatPose
+
+from cnspy_csv2dataframe.TUMCSV2DataFrame import TUMCSV2DataFrame
+from cnspy_spatial_csv_formats.CSVSpatialFormatType import CSVSpatialFormatType
 from cnspy_csv2dataframe.CSV2DataFrame import CSV2DataFrame
 import cnspy_numpy_utils.matrix_conversions as matrix_conversions
 
 
-class PoseWithCov2DataFrame(CSV2DataFrame):
+class PosOrientWithCov2DataFrame(CSV2DataFrame):
     def __init__(self, fn=None):
-        CSV2DataFrame.__init__(self, filename=fn, fmt=CSVFormatPose.PoseWithCov)
+        # identify the covariance format via fmt=None!
+        CSV2DataFrame.__init__(self, fn=fn, fmt=None)
 
     @staticmethod
-    def DataFrame_to_TPQCov(data_frame):
+    def from_DataFrame(data_frame):
+        assert (isinstance(data_frame, pandas.DataFrame))
+
+        t_vec, p_vec, q_vec = TUMCSV2DataFrame.from_DataFrame(data_frame)
+
         if version_info[0] < 3:
-            t_vec = data_frame.as_matrix(['t'])
-            p_vec = data_frame.as_matrix(['tx', 'ty', 'tz'])
-            q_vec = data_frame.as_matrix(['qx', 'qy', 'qz', 'qw'])
             cov_vec_p = data_frame.as_matrix(['pxx', 'pxy', 'pxz', 'pyy', 'pyz', 'pzz'])
             cov_vec_q = data_frame.as_matrix(['qrr', 'qrp', 'qry', 'qpp', 'qpy', 'qyy'])
         else:
             # FIX(scm): for newer versions as_matrix is deprecated, using to_numpy instead
             # from https://stackoverflow.com/questions/60164560/attributeerror-series-object-has-no-attribute-as-matrix-why-is-it-error
-            t_vec = data_frame[['t']].to_numpy()
-            p_vec = data_frame[['tx', 'ty', 'tz']].to_numpy()
-            q_vec = data_frame[['qx', 'qy', 'qz', 'qw']].to_numpy()
             cov_vec_p = data_frame[['pxx', 'pxy', 'pxz', 'pyy', 'pyz', 'pzz']].to_numpy()
             cov_vec_q = data_frame[['qrr', 'qrp', 'qry', 'qpp', 'qpy', 'qyy']].to_numpy()
 
         l = t_vec.shape[0]
 
         P_vec_p = np.zeros((l, 3, 3))
         P_vec_q = np.zeros((l, 3, 3))
@@ -58,39 +59,34 @@
         for i in range(0, l):
             P_vec_p[i] = matrix_conversions.tri_vec_to_mat(cov_vec_p[i,], n=3)
             P_vec_q[i] = matrix_conversions.tri_vec_to_mat(cov_vec_q[i,], n=3)
 
         return t_vec, p_vec, q_vec, P_vec_p, P_vec_q
 
     @staticmethod
-    def TPQCov_to_DataFrame(t_vec, p_vec, q_vec, P_vec_p, P_vec_q):
+    def to_DataFrame(t_vec, p_vec, q_vec, P_vec_p, P_vec_q):
         t_rows, t_cols = t_vec.shape  # does not work in Python 3
-        p_rows, p_cols = p_vec.shape
-        q_rows, q_cols = q_vec.shape
         P_p_len, P_p_rows, P_p_cols = P_vec_p.shape
-        assert (t_rows == p_rows)
-        assert (t_rows == q_rows)
-        assert (p_cols == 3)
-        assert (q_cols == 4)
         assert (P_p_len == t_rows)
         assert (P_p_rows == 3 and P_p_cols == 3)
         assert (P_vec_p.shape == P_vec_q.shape)
 
+        df1 = TUMCSV2DataFrame.to_DataFrame(t_vec, p_vec, q_vec)
+
         l = t_rows
         cov_vec_p = np.zeros((l, 6))
         cov_vec_q = np.zeros((l, 6))
         for i in range(0, l):
             # https://stackoverflow.com/questions/17527693/transform-the-upper-lower-triangular-part-of-a-symmetric-matrix-2d-array-into/58806626#58806626
             # https://stackoverflow.com/questions/8905501/extract-upper-or-lower-triangular-part-of-a-numpy-matrix
             cov_vec_p[i] = matrix_conversions.mat_to_tri_vec(P_vec_p[i])
             cov_vec_q[i] = matrix_conversions.mat_to_tri_vec(P_vec_q[i])
 
-        data_frame = pandas.DataFrame(
-            {'t': t_vec[:, 0], 'tx': p_vec[:, 0], 'ty': p_vec[:, 1], 'tz': p_vec[:, 2],
-             'qx': q_vec[:, 0], 'qy': q_vec[:, 1], 'qz': q_vec[:, 2], 'qw': q_vec[:, 3],
-             'pxx': cov_vec_p[:, 0], 'pxy': cov_vec_p[:, 1], 'pxz': cov_vec_p[:, 2], 'pyy': cov_vec_p[:, 3],
+        df2 = pandas.DataFrame(
+            {'pxx': cov_vec_p[:, 0], 'pxy': cov_vec_p[:, 1], 'pxz': cov_vec_p[:, 2], 'pyy': cov_vec_p[:, 3],
              'pyz': cov_vec_p[:, 4], 'pzz': cov_vec_p[:, 5],
              'qrr': cov_vec_q[:, 0], 'qrp': cov_vec_q[:, 1], 'qry': cov_vec_q[:, 2], 'qpp': cov_vec_q[:, 3],
              'qpy': cov_vec_q[:, 4], 'qyy': cov_vec_q[:, 5]})
-        return data_frame
+
+        return pandas.concat([df1, df2], axis=1)
```

### Comparing `cnspy_csv2dataframe-0.1.1/cnspy_csv2dataframe/TUMCSV2DataFrame.py` & `cnspy_csv2dataframe-0.2.0/cnspy_csv2dataframe/TUMCSV2DataFrame.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,21 +19,22 @@
 # Requirements:
 # sudo pip install numpy pandas
 ########################################################################################################################
 import os
 from sys import version_info
 import math
 import pandas as pandas
-from cnspy_spatial_csv_formats.CSVFormatPose import CSVFormatPose
+import numpy as np
+from cnspy_spatial_csv_formats.CSVSpatialFormatType import CSVSpatialFormatType
 from cnspy_csv2dataframe.CSV2DataFrame import CSV2DataFrame
 
 
 class TUMCSV2DataFrame(CSV2DataFrame):
     def __init__(self, fn=''):
-        CSV2DataFrame.__init__(self, filename=fn, fmt=CSVFormatPose.TUM)
+        CSV2DataFrame.__init__(self, fn=fn, fmt=CSVSpatialFormatType.TUM)
 
     @staticmethod
     def DataFrame_to_numpy_dict(df):
         np_dict = {
             't': df[['t']].values.transpose()[0],
             'tx': df[['tx']].values.transpose()[0],
             'ty': df[['ty']].values.transpose()[0],
@@ -42,28 +43,28 @@
             'qy': df[['qy']].values.transpose()[0],
             'qz': df[['qz']].values.transpose()[0],
             'qw': df[['qw']].values.transpose()[0]
         }
         return np_dict
 
     @staticmethod
-    def DataFrame_to_TPQ(data_frame):
+    def from_DataFrame(data_frame):
         if version_info[0] < 3:
             t_vec = data_frame.as_matrix(['t'])
             p_vec = data_frame.as_matrix(['tx', 'ty', 'tz'])
             q_vec = data_frame.as_matrix(['qx', 'qy', 'qz', 'qw'])
         else:
             t_vec = data_frame[['t']].to_numpy()
             p_vec = data_frame[['tx', 'ty', 'tz']].to_numpy()
             q_vec = data_frame[['qx', 'qy', 'qz', 'qw']].to_numpy()
 
         return t_vec, p_vec, q_vec
 
     @staticmethod
-    def TPQ_to_DataFrame(t_vec, p_vec, q_vec):
+    def to_DataFrame(t_vec, p_vec, q_vec):
         if t_vec.ndim == 2:
             t_rows, t_cols = t_vec.shape
         else:
             t_vec = np.array([t_vec])
             t_rows, t_cols = t_vec.shape
 
         p_rows, p_cols = p_vec.shape
```

### Comparing `cnspy_csv2dataframe-0.1.1/cnspy_csv2dataframe/TimestampCSV2DataFrame.py` & `cnspy_csv2dataframe-0.2.0/cnspy_csv2dataframe/TimestampCSV2DataFrame.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
 # Requirements:
 # sudo pip install numpy pandas
 ########################################################################################################################
 from sys import version_info
 import pandas as pandas
-from cnspy_spatial_csv_formats.CSVFormatPose import CSVFormatPose
+from cnspy_spatial_csv_formats.CSVSpatialFormatType import CSVSpatialFormatType
 from cnspy_csv2dataframe.CSV2DataFrame import CSV2DataFrame
 
 
 class TimestampCSV2DataFrame(CSV2DataFrame):
     def __init__(self, fn=''):
-        CSV2DataFrame.__init__(self, filename=fn, fmt=CSVFormatPose.Timestamp)
+        CSV2DataFrame.__init__(self, fn=fn, fmt=CSVSpatialFormatType.Timestamp)
 
     def get_t_vec(self):
         if self.data_loaded:
             if version_info[0] < 3:
                 return self.data_frame.as_matrix(['t'])
             else:
                 return self.data_frame[['t']].to_numpy()
```

### Comparing `cnspy_csv2dataframe-0.1.1/cnspy_csv2dataframe.egg-info/PKG-INFO` & `cnspy_csv2dataframe-0.2.0/cnspy_csv2dataframe.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,63 @@
 Metadata-Version: 2.1
-Name: cnspy-csv2dataframe
-Version: 0.1.1
+Name: cnspy_csv2dataframe
+Version: 0.2.0
 Summary: CSV to pandas.Dataframe converter
 Home-page: https://github.com/aau-cns/cnspy_csv2dataframe/
 Author: Roland Jung
 Author-email: roland.jung@aau.at
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/aau-cns/cnspy_csv2dataframe/issues
-Description: # cnspy_csv2dataframe
-        
-        
-        The class [CSV2DataFrame](./cnspy_csv2dataframe/CSV2DataFrame.py) is intended to load [CSV-files](https://en.wikipedia.org/wiki/Comma-separated_values) into a `pandas.DataFrame`. The CSV files need to match known formats (defined by their header in the first line) according to those defined in the package [spatial_csv_formats]().
-          
-        In case no format is specified, it tries to match the first line of the CSV-File with known headers from [cnspy_spatial_csv_formats](https://github.com/aau-cns/cnspy_spatial_csv_formats) and loads the data in that format. 
-        
-        There a some specialization of  [CSV2DataFrame](./cnspy_csv2dataframe/CSV2DataFrame.py) that support different operations on the data:
-        * [PoseCovCSV2DataFrame](./cnspy_csv2dataframe/PoseCovCSV2DataFrame.py)
-        * [PoseWithCov2DataFrame](./cnspy_csv2dataframe/PoseWithCov2DataFrame.py)
-        * [TimestampCSV2DataFrame](./cnspy_csv2dataframe/TimestampCSV2DataFrame.py)
-        * [TUMCSV2DataFrame](./cnspy_csv2dataframe/TUMCSV2DataFrame.py)
-        
-        ## Installation
-        
-        Install the current code base from GitHub and pip install a link to that cloned copy
-        ```
-        git clone https://github.com/aau-cns/csv2dataframe.git
-        cd csv2dataframe
-        pip install -e .
-        ```
-        
-        ## Dependencies
-        
-        It is part of the [cnspy eco-system](hhttps://github.com/aau-cns/cnspy_eco_system_test) of the [cns-github](https://github.com/aau-cns) group.  
-        
-        * [numpy]()
-        * [pandas]()
-        * [cnspy_spatial_csv_formats](https://github.com/aau-cns/cnspy_spatial_csv_formats)
-        * [cnspy_numpy_utils](https://github.com/aau-cns/cnspy_numpy_utils)
-        
-        
-        ## License
-        
-        
-        Software License Agreement (GNU GPLv3  License), refer to the LICENSE file.
-        
-        *Sharing is caring!* - [Roland Jung](https://github.com/jungr-ait)
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENCE
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: cnspy_numpy_utils
+Requires-Dist: cnspy_spatial_csv_formats
+
+# cnspy_csv2dataframe
+
+
+The class [CSV2DataFrame](./cnspy_csv2dataframe/CSV2DataFrame.py) is intended to load [CSV-files](https://en.wikipedia.org/wiki/Comma-separated_values) into a `pandas.DataFrame`. The CSV files need to match known formats (defined by their header in the first line) according to those defined in the package [spatial_csv_formats]().
+  
+In case no format is specified, it tries to match the first line of the CSV-File with known headers from [cnspy_spatial_csv_formats](https://github.com/aau-cns/cnspy_spatial_csv_formats) and loads the data in that format. 
+
+There a some specialization of  [CSV2DataFrame](./cnspy_csv2dataframe/CSV2DataFrame.py) that support different operations on the data:
+* [PoseCovCSV2DataFrame](./cnspy_csv2dataframe/PosOrientCovCSV2DataFrame.py)
+* [PoseWithCov2DataFrame](./cnspy_csv2dataframe/PosOrientWithCov2DataFrame.py)
+* [TimestampCSV2DataFrame](./cnspy_csv2dataframe/TimestampCSV2DataFrame.py)
+* [TUMCSV2DataFrame](./cnspy_csv2dataframe/TUMCSV2DataFrame.py)
+
+## Installation
+
+Install the current code base from GitHub and pip install a link to that cloned copy
+```
+git clone https://github.com/aau-cns/cnspy_csv2dataframe.git
+cd cnspy_csv2dataframe
+pip install -e .
+```
+or the [official package](https://pypi.org/project/cnspy-csv2dataframe/) via
+```commandline
+pip install cnspy-csv2dataframe
+```
+
+## Dependencies
+
+It is part of the [cnspy eco-system](hhttps://github.com/aau-cns/cnspy_eco_system_test) of the [cns-github](https://github.com/aau-cns) group.  
+
+* [numpy]()
+* [pandas]()
+* [cnspy_spatial_csv_formats](https://github.com/aau-cns/cnspy_spatial_csv_formats)
+* [cnspy_numpy_utils](https://github.com/aau-cns/cnspy_numpy_utils)
+
+
+## License
+
+
+Software License Agreement (GNU GPLv3  License), refer to the LICENSE file.
+
+*Sharing is caring!* - [Roland Jung](https://github.com/jungr-ait)
```

### Comparing `cnspy_csv2dataframe-0.1.1/cnspy_csv2dataframe.egg-info/SOURCES.txt` & `cnspy_csv2dataframe-0.2.0/cnspy_csv2dataframe.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,27 @@
+LICENCE
 README.md
 setup.py
 cnspy_csv2dataframe/CSV2DataFrame.py
-cnspy_csv2dataframe/PoseCovCSV2DataFrame.py
+cnspy_csv2dataframe/PosOrientCovCSV2DataFrame.py
+cnspy_csv2dataframe/PosOrientWithCov2DataFrame.py
+cnspy_csv2dataframe/PosOrientWithCovTyped2DataFrame.py
+cnspy_csv2dataframe/PoseErrorStamped2DataFrame.py
+cnspy_csv2dataframe/PoseTypedStamped2DataFrame.py
 cnspy_csv2dataframe/PoseWithCov2DataFrame.py
+cnspy_csv2dataframe/PoseWithCovTyped2DataFrame.py
 cnspy_csv2dataframe/TUMCSV2DataFrame.py
 cnspy_csv2dataframe/TimestampCSV2DataFrame.py
 cnspy_csv2dataframe/__init__.py
 cnspy_csv2dataframe.egg-info/PKG-INFO
 cnspy_csv2dataframe.egg-info/SOURCES.txt
 cnspy_csv2dataframe.egg-info/dependency_links.txt
 cnspy_csv2dataframe.egg-info/requires.txt
 cnspy_csv2dataframe.egg-info/top_level.txt
 test/__init__.py
 test/test_CSV2DataFrame.py
+test/test_PosOrientWithCov2DataFrame.py
+test/test_PosOrientWithCovTyped2DataFrame.py
 test/test_PoseWithCov2DataFrame.py
+test/test_PoseWithCovTyped2DataFrame.py
 test/test_TUMCSV2DataFrame.py
 test/test_TimestampCSV2DataFrame.py
```

### Comparing `cnspy_csv2dataframe-0.1.1/setup.py` & `cnspy_csv2dataframe-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `cnspy_csv2dataframe-0.1.1/test/test_PoseWithCov2DataFrame.py` & `cnspy_csv2dataframe-0.2.0/test/test_PoseWithCov2DataFrame.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,43 +16,48 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
 ########################################################################################################################
 import os
 import unittest
 import time
-from cnspy_spatial_csv_formats.CSVFormatPose import CSVFormatPose
+from cnspy_spatial_csv_formats.CSVSpatialFormatType import CSVSpatialFormatType
 from cnspy_csv2dataframe.CSV2DataFrame import CSV2DataFrame
 from cnspy_csv2dataframe.PoseWithCov2DataFrame import PoseWithCov2DataFrame
 
+
 SAMPLE_DATA_DIR = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'sample_data')
 
 class PoseWithCov2DataFrame_Test(unittest.TestCase):
     start_time = None
 
     def start(self):
         self.start_time = time.time()
 
     def stop(self):
         print("Process time: " + str((time.time() - self.start_time)))
 
     def load_(self):
         print('loading...')
-        fn = str(SAMPLE_DATA_DIR + '/ID1-pose-est-cov.csv')
+        fn = str(SAMPLE_DATA_DIR + '/ID1-pose-est-pose-cov.csv')
         obj = PoseWithCov2DataFrame(fn=fn)
         return obj
 
     def test_load_trajectory_from_CSV(self):
         obj = self.load_()
         self.assertTrue(obj.data_loaded)
+        self.assertTrue(obj.format == CSVSpatialFormatType.PoseWithCovTyped)
+
         self.start()
-        t_vec, p_vec, q_vec, P_vec_p, P_vec_q = PoseWithCov2DataFrame.DataFrame_to_TPQCov(obj.data_frame)
+        t_vec, p_vec, q_vec, P_vec_T = PoseWithCov2DataFrame.from_DataFrame(obj.data_frame)
         self.stop()
 
-        print(P_vec_p[1000])
-        print(P_vec_q[1000])
-        print(p_vec[1000])
-        print(q_vec[1000])
+        print('P: ' + str(P_vec_T[1000]))
+        print('p: ' + str(p_vec[1000]))
+        print('q: ' + str(q_vec[1000]))
+
+        df = PoseWithCov2DataFrame.to_DataFrame(t_vec, p_vec, q_vec, P_vec_T)
+        print('keys: ' + str(df.keys().values))
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `cnspy_csv2dataframe-0.1.1/test/test_TUMCSV2DataFrame.py` & `cnspy_csv2dataframe-0.2.0/test/test_TUMCSV2DataFrame.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #
 ########################################################################################################################
 import os
 import unittest
 import numpy as np
 from cnspy_csv2dataframe.TUMCSV2DataFrame import TUMCSV2DataFrame
 from cnspy_csv2dataframe.CSV2DataFrame import CSV2DataFrame
-from cnspy_spatial_csv_formats.CSVFormatPose import CSVFormatPose
+from cnspy_spatial_csv_formats.CSVSpatialFormatType import CSVSpatialFormatType
 
 SAMPLE_DATA_DIR = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'sample_data')
 
 class TUMCSVdata_Test(unittest.TestCase):
     def load_sample_data_frame(self):
         return TUMCSV2DataFrame(fn=str(SAMPLE_DATA_DIR + '/ID1-pose-gt.csv'))
 
@@ -42,15 +42,15 @@
         d = self.load_sample_data_frame()
         np_dict = TUMCSV2DataFrame.DataFrame_to_numpy_dict(d.data_frame)
 
         self.assertTrue(len(np_dict['t']) > 100)
 
     def test_data_to_tqp(self):
         d = self.load_sample_data_frame()
-        t_vec, p_vec, q_vec = TUMCSV2DataFrame.DataFrame_to_TPQ(d.data_frame)
+        t_vec, p_vec, q_vec = TUMCSV2DataFrame.from_DataFrame(d.data_frame)
 
         self.assertTrue(len(t_vec) > 0)
         self.assertTrue(len(t_vec) == len(p_vec))
 
     def test_tpq_to_data_frame(self):
         p_vec = np.array([[21, 72, 67],
                           [23, 78, 69],
@@ -60,25 +60,25 @@
                           [0, 0, 0, 1],
                           [0, 0, 0, 1],
                           [0, 0, 0, 1]])
         t_vec = np.array([[0],
                           [1],
                           [2],
                           [3]])
-        df = TUMCSV2DataFrame.TPQ_to_DataFrame(t_vec, p_vec, q_vec)
+        df = TUMCSV2DataFrame.to_DataFrame(t_vec, p_vec, q_vec)
         print(str(df))
-        CSV2DataFrame.save_CSV(data_frame=df, filename=str(SAMPLE_DATA_DIR + '/results/any.csv'), fmt=CSVFormatPose.TUM)
+        CSV2DataFrame.save_CSV(data_frame=df, filename=str(SAMPLE_DATA_DIR + '/results/any.csv'), fmt=CSVSpatialFormatType.TUM)
 
     def test_subsample_DataFrame(self):
         d = self.load_sample_data_frame()
 
         num_samples = 200
         df_sub = TUMCSV2DataFrame.subsample_DataFrame(d.data_frame, num_max_points=200, verbose=True)
 
         self.assertTrue(len(df_sub.index) <= num_samples)
 
         CSV2DataFrame.save_CSV(data_frame=df_sub, filename=str(SAMPLE_DATA_DIR + '/results/gt_sub_200.csv'),
-                               fmt=CSVFormatPose.TUM)
+                               fmt=CSVSpatialFormatType.TUM)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `cnspy_csv2dataframe-0.1.1/test/test_TimestampCSV2DataFrame.py` & `cnspy_csv2dataframe-0.2.0/test/test_TimestampCSV2DataFrame.py`

 * *Files identical despite different names*

