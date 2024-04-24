# Comparing `tmp/crnpy-0.5.1.tar.gz` & `tmp/crnpy-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crnpy-0.5.1.tar", last modified: Sun Jul 30 03:00:44 2023, max compression
+gzip compressed data, was "crnpy-0.6.0.tar", last modified: Wed Apr 24 02:02:23 2024, max compression
```

## Comparing `crnpy-0.5.1.tar` & `crnpy-0.6.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:00:44.367024 crnpy-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-30 03:00:33.000000 crnpy-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-30 03:00:44.367024 crnpy-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-07-30 03:00:33.000000 crnpy-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 03:00:44.367024 crnpy-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-30 03:00:33.000000 crnpy-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:00:44.367024 crnpy-0.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:00:44.367024 crnpy-0.5.1/src/crnpy/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-30 03:00:33.000000 crnpy-0.5.1/src/crnpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52969 2023-07-30 03:00:33.000000 crnpy-0.5.1/src/crnpy/crnpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9159 2023-07-30 03:00:33.000000 crnpy-0.5.1/src/crnpy/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:00:44.367024 crnpy-0.5.1/src/crnpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-30 03:00:44.000000 crnpy-0.5.1/src/crnpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-30 03:00:44.000000 crnpy-0.5.1/src/crnpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 03:00:44.000000 crnpy-0.5.1/src/crnpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-30 03:00:44.000000 crnpy-0.5.1/src/crnpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-30 03:00:44.000000 crnpy-0.5.1/src/crnpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:02:23.204850 crnpy-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-24 02:02:13.000000 crnpy-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-04-24 02:02:23.204850 crnpy-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-04-24 02:02:13.000000 crnpy-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 02:02:23.204850 crnpy-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-24 02:02:13.000000 crnpy-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:02:23.200850 crnpy-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:02:23.200850 crnpy-0.6.0/src/crnpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-24 02:02:13.000000 crnpy-0.6.0/src/crnpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68437 2024-04-24 02:02:13.000000 crnpy-0.6.0/src/crnpy/crnpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9159 2024-04-24 02:02:13.000000 crnpy-0.6.0/src/crnpy/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:02:23.204850 crnpy-0.6.0/src/crnpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-04-24 02:02:23.000000 crnpy-0.6.0/src/crnpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-24 02:02:23.000000 crnpy-0.6.0/src/crnpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 02:02:23.000000 crnpy-0.6.0/src/crnpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-24 02:02:23.000000 crnpy-0.6.0/src/crnpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 02:02:23.000000 crnpy-0.6.0/src/crnpy.egg-info/top_level.txt
```

### Comparing `crnpy-0.5.1/LICENSE` & `crnpy-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crnpy-0.5.1/PKG-INFO` & `crnpy-0.6.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,12 @@
-Metadata-Version: 2.1
-Name: crnpy
-Version: 0.5.1
-Summary: A Python package for the estimation and processing of soil moisture data from cosmic-ray neutron counts.
-Home-page: https://github.com/soilwater/crnpy
-Author: Joaquin Peraza, Andres Patrignani
-Author-email: jperaza@ksu.edu, andrespatrignani@ksu.edu
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![GitHub Workflow Status (building)](https://img.shields.io/github/actions/workflow/status/soilwater/crnpy/python-package.yml)](https://github.com/soilwater/crnpy/actions/workflows/python-package.yml)
 [![GitHub Workflow Status (publish)](https://img.shields.io/github/actions/workflow/status/soilwater/crnpy/python-publish.yml?label=publish)](https://github.com/soilwater/crnpy/actions/workflows/python-publish.yml)
 [![PyPI - Status](https://img.shields.io/pypi/v/crnpy)](https://pypi.org/project/crnpy/)
 [![GitHub commits since latest release (by SemVer including pre-releases)](https://img.shields.io/github/commits-since/soilwater/crnpy/latest/main)](https://github.com/soilwater/crnpy)
+![JOSS submission status](https://joss.theoj.org/papers/e65c1bb5fee58c39289efc4547d1fd10/status.svg)
 
 # Cosmic-Ray Neutron Python (CRNPy) Library
 
 <img src="https://raw.githubusercontent.com/soilwater/crnpy/main/docs/img/logo/crnpy-logo.png" alt="CRNPY logo" width="250"/>
 
 ## Overview
 Welcome to the homepage of the CRNPy (Cosmic-Ray Neutron Python) library, an open-source Python library designed for the processing and conversion of raw neutron counts from cosmic-ray neutron probes (CRNP) into soil moisture data.
@@ -28,15 +18,14 @@
 
 ## Key Features
 - Versatile and instrument agnostic: CRNPy can handle data from various CRNP manufacturers and models. It has been successfully tested on both roving and stationary CRNP.
 
 - Modular: The library is designed to be modular, allowing users to easily customize the processing workflow to their needs.
 
 
-
 ## Installation
 To install the CRNPy library, you can use Python's package manager. Open a terminal and type:
 
 ```pip install crnpy```
 
 from the Jupyter notebook, type:
 
@@ -45,14 +34,20 @@
 Ideally dependencies should be installed automatically. If not, you can install them manually by typing:
 
 ```pip install -r requirements.txt```
 
 The CRNPy library is compatible with Python 3.7 and above.
 See [requirements.txt](https://github.com/soilwater/crnpy/blob/main/requirements.txt) for a list of dependencies.
 
+## Examples
+
+- [https://soilwater.github.io/crnpy/examples/stationary/example_RDT_station/](Processing and analyzing data from a stationary detector)
+- [https://soilwater.github.io/crnpy/examples/rover/Hydroinnova_rover_example/](Processing and analyzing data from a roving detector)
+- [https://soilwater.github.io/crnpy/examples/calibration/calibration/](Device-specific field calibration)
+
 ## Authors
 The CRNPy library was developed at the Kansas State University Soil Water Processes Lab by:
 
 - Joaquin Peraza
 
 - Andres Patrignani
```

### Comparing `crnpy-0.5.1/README.md` & `crnpy-0.6.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,28 @@
+Metadata-Version: 2.1
+Name: crnpy
+Version: 0.6.0
+Summary: A Python package for the estimation and processing of soil moisture data from cosmic-ray neutron counts.
+Home-page: https://soilwater.github.io/crnpy/
+Author: Joaquin Peraza, Andres Patrignani
+Author-email: jperaza@ksu.edu, andrespatrignani@ksu.edu
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: scipy
+Requires-Dist: requests
+Requires-Dist: utm
+
 [![GitHub Workflow Status (building)](https://img.shields.io/github/actions/workflow/status/soilwater/crnpy/python-package.yml)](https://github.com/soilwater/crnpy/actions/workflows/python-package.yml)
 [![GitHub Workflow Status (publish)](https://img.shields.io/github/actions/workflow/status/soilwater/crnpy/python-publish.yml?label=publish)](https://github.com/soilwater/crnpy/actions/workflows/python-publish.yml)
 [![PyPI - Status](https://img.shields.io/pypi/v/crnpy)](https://pypi.org/project/crnpy/)
 [![GitHub commits since latest release (by SemVer including pre-releases)](https://img.shields.io/github/commits-since/soilwater/crnpy/latest/main)](https://github.com/soilwater/crnpy)
+![JOSS submission status](https://joss.theoj.org/papers/e65c1bb5fee58c39289efc4547d1fd10/status.svg)
 
 # Cosmic-Ray Neutron Python (CRNPy) Library
 
 <img src="https://raw.githubusercontent.com/soilwater/crnpy/main/docs/img/logo/crnpy-logo.png" alt="CRNPY logo" width="250"/>
 
 ## Overview
 Welcome to the homepage of the CRNPy (Cosmic-Ray Neutron Python) library, an open-source Python library designed for the processing and conversion of raw neutron counts from cosmic-ray neutron probes (CRNP) into soil moisture data.
@@ -17,15 +34,14 @@
 
 ## Key Features
 - Versatile and instrument agnostic: CRNPy can handle data from various CRNP manufacturers and models. It has been successfully tested on both roving and stationary CRNP.
 
 - Modular: The library is designed to be modular, allowing users to easily customize the processing workflow to their needs.
 
 
-
 ## Installation
 To install the CRNPy library, you can use Python's package manager. Open a terminal and type:
 
 ```pip install crnpy```
 
 from the Jupyter notebook, type:
 
@@ -34,14 +50,20 @@
 Ideally dependencies should be installed automatically. If not, you can install them manually by typing:
 
 ```pip install -r requirements.txt```
 
 The CRNPy library is compatible with Python 3.7 and above.
 See [requirements.txt](https://github.com/soilwater/crnpy/blob/main/requirements.txt) for a list of dependencies.
 
+## Examples
+
+- [https://soilwater.github.io/crnpy/examples/stationary/example_RDT_station/](Processing and analyzing data from a stationary detector)
+- [https://soilwater.github.io/crnpy/examples/rover/Hydroinnova_rover_example/](Processing and analyzing data from a roving detector)
+- [https://soilwater.github.io/crnpy/examples/calibration/calibration/](Device-specific field calibration)
+
 ## Authors
 The CRNPy library was developed at the Kansas State University Soil Water Processes Lab by:
 
 - Joaquin Peraza
 
 - Andres Patrignani
```

### Comparing `crnpy-0.5.1/setup.py` & `crnpy-0.6.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # contents of setup.py
 import setuptools
 
 setuptools.setup(
     name="crnpy",
-    version="0.5.1",
+    version="0.6.0",
     packages=['crnpy'],
     package_dir = {"": "src"},
     description="A Python package for the estimation and processing of soil moisture data from cosmic-ray neutron counts.",
     include_package_data=True,
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
-    url="https://github.com/soilwater/crnpy",
+    url="https://soilwater.github.io/crnpy/",
     author="Joaquin Peraza, Andres Patrignani",
     author_email="jperaza@ksu.edu, andrespatrignani@ksu.edu",
     license="MIT",
     license_files=["LICENSE"],
     install_requires=[
         "numpy",
         "pandas",
         "scipy",
-        "requests"
+        "requests",
+        "utm"
     ],
 )
```

### Comparing `crnpy-0.5.1/src/crnpy/__init__.py` & `crnpy-0.6.0/src/crnpy/__init__.py`

 * *Files identical despite different names*

### Comparing `crnpy-0.5.1/src/crnpy/crnpy.py` & `crnpy-0.6.0/src/crnpy/crnpy.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 # crnpy/crnpy.py
 """
 `crnpy` is a Python package for processing cosmic ray neutron data.
 
  Created by Joaquin Peraza and Andres Patrignani.
 """
 
-# Import modules
-import sys
-import warnings
+import crnpy.data as data
+import io
 import numbers
 import numpy as np
 import pandas as pd
 import requests
-import io
-
+import sys
+import utm
+import warnings
 
-from scipy.signal import savgol_filter
 from scipy.interpolate import griddata
+from scipy.signal import savgol_filter
 from scipy.special import erfcinv
-import crnpy.data as data
 
 # Define python version
 python_version = (3, 7)  # tuple of (major, minor) version requirement
 python_version_str = str(python_version[0]) + "." + str(python_version[1])
 
 # produce an error message if the python version is less than required
 if sys.version_info < python_version:
@@ -38,32 +37,32 @@
         timestamp_col (str): Name of the column with timestamps in datetime format.
         integration_time (int): Duration of the neutron counting interval in seconds. Typical values are 60 seconds and 3600 seconds.
         remove_first (bool, optional): Remove first row. Default is False.
         
     Returns:
         (pandas.DataFrame): 
     """
-    
+
     # Check format of timestamp column
     if df[timestamp_col].dtype != 'datetime64[ns]':
         raise TypeError('timestamp_col must be datetime64. Use `pd.to_datetime()` to fix this issue.')
 
     # Check if differences in timestamps are below or above the provided integration time
     idx_delta = df[timestamp_col].diff().dt.total_seconds() != integration_time
-    
+
     if remove_first:
         idx_delta[0] = True
-        
+
     # Select rows that meet the specified integration time
     df = df[~idx_delta]
     df.reset_index(drop=True, inplace=True)
 
     # Notify user about the number of rows that have been removed
     print(f"Removed a total of {sum(idx_delta)} rows.")
-    
+
     return df
 
 
 def fill_missing_timestamps(df, timestamp_col='timestamp', freq='H', round_timestamp=True, verbose=False):
     """Helper function to fill rows with missing timestamps in datetime record. Rows are filled with NaN values.
 
      Args:
@@ -90,68 +89,67 @@
     start_date = df[timestamp_col].iloc[0]
     end_date = df[timestamp_col].iloc[-1]
     date_range = pd.date_range(start_date, end_date, freq=freq)
     counter = 0
     for date in date_range:
         if date not in df[timestamp_col].values:
             if verbose:
-                print('Adding missing date:',date)
-            new_line = pd.DataFrame({timestamp_col:date}, index=[-1]) # By default fills columns with np.nan
-            df = pd.concat([df,new_line])
+                print('Adding missing date:', date)
+            new_line = pd.DataFrame({timestamp_col: date}, index=[-1])  # By default fills columns with np.nan
+            df = pd.concat([df, new_line])
             counter += 1
 
     df.sort_values(by=timestamp_col, inplace=True)
     df.reset_index(drop=True, inplace=True)
-    
+
     # Notify user about the number of rows that have been removed
     print(f"Added a total of {counter} missing timestamps.")
-    
+
     return df
 
 
-def total_raw_counts(counts, nan_strategy=None, timestamp_col=None):
+def total_raw_counts(counts):
     """Compute the sum of uncorrected neutron counts for all detectors.
 
     Args:
         counts (pandas.DataFrame): Dataframe containing only the columns with neutron counts.
-        nan_strategy (str): Strategy to use for NaN values. Options are 'interpolate', 'average', or None. Default is None.
 
     Returns:
         (pandas.DataFrame): Dataframe with the sum of uncorrected neutron counts for all detectors.
     """
 
     if counts.shape[0] > 1:
-        counts = counts.apply(lambda x: x.fillna(counts.mean(axis=1)),axis=0)
+        counts = counts.apply(lambda x: x.fillna(counts.mean(axis=1)), axis=0)
 
     # Compute sum of counts
     total_raw_counts = counts.sum(axis=1)
-    
+
     # Replace zeros with NaN
     total_raw_counts = total_raw_counts.replace(0, np.nan)
-    
+
     return total_raw_counts
 
 
 def is_outlier(x, method, window=11, min_val=None, max_val=None):
     """Function that tests whether values are outliers using a modified moving z-score based on the median absolute difference.
 
     Args:
-        x (pandas.DataFrame): Variable containing only the columns with neutron counts.
+        x (pd.DataFrame or pd.Series): Variable containing only the columns with neutron counts.
         method (str): Outlier detection method. One of: range, iqr, moviqr, zscore, movzscore, modified_zscore, and scaled_mad
         window (int, optional): Window size for the moving central tendency. Default is 11.
         min_val (int or float): Minimum value for a reading to be considered valid. Default is None.
         max_val(int or float): Maximum value for a reading to be considered valid. Default is None.
 
     Returns:
         (pandas.DataFrame): Boolean indicating outliers.
 
     References:
         Iglewicz, B. and Hoaglin, D.C., 1993. How to detect and handle outliers (Vol. 16). Asq Press.
     """
-        
+
     if not isinstance(x, pd.Series):
         raise TypeError('x must of type pandas.Series')
 
     # Separate this method to allow usage together with other methods below
     if isinstance(min_val, numbers.Number) and isinstance(max_val, numbers.Number):
         idx_range_outliers = (x < min_val) | (x > max_val)
     else:
@@ -160,50 +158,50 @@
     # Apply other methods in addition to a range check
     if method == 'iqr':
         q1 = x.quantile(0.25)
         q3 = x.quantile(0.75)
         iqr = q3 - q1
         high_fence = q3 + (1.5 * iqr)
         low_fence = q1 - (1.5 * iqr)
-        idx_outliers = (x<low_fence ) | (x>high_fence )
+        idx_outliers = (x < low_fence) | (x > high_fence)
 
     elif method == 'moviqr':
         q1 = x.rolling(window, center=True).quantile(0.25)
         q3 = x.rolling(window, center=True).quantile(0.75)
         iqr = q3 - q1
-        ub = q3 + (1.5 * iqr) # Upper boundary
-        lb = q1 - (1.5 * iqr) # Lower boundary
+        ub = q3 + (1.5 * iqr)  # Upper boundary
+        lb = q1 - (1.5 * iqr)  # Lower boundary
         idx_outliers = (x < lb) | (x > ub)
 
     elif method == 'zscore':
-        zscore = (x - x.mean())/x.std()
+        zscore = (x - x.mean()) / x.std()
         idx_outliers = (zscore < -3) | (zscore > 3)
 
     elif method == 'movzscore':
         movmean = x.rolling(window=window, center=True).mean()
         movstd = x.rolling(window=window, center=True).std()
-        movzscore = (x - movmean)/movstd
+        movzscore = (x - movmean) / movstd
         idx_outliers = (movzscore < -3) | (movzscore > 3)
 
     elif method == 'modified_zscore':
         # Compute median absolute difference
         movmedian = x.rolling(window, center=True).median()
         abs_diff = np.abs(x - movmedian)
         mad = abs_diff.rolling(window, center=True).median()
 
         # Compute modified z-score
         modified_z_score = 0.6745 * abs_diff / mad
         idx_outliers = (modified_z_score < -3.5) | (modified_z_score > 3.5)
 
     elif method == 'scaled_mad':
         # Returns true for elements more than three scaled MAD from the median. 
-        c = -1 / (np.sqrt(2)*erfcinv(3/2))
+        c = -1 / (np.sqrt(2) * erfcinv(3 / 2))
         median = np.nanmedian(x)
-        mad = c*np.nanmedian(np.abs(x - median))
-        idx_outliers = x > (median + 3*mad)
+        mad = c * np.nanmedian(np.abs(x - median))
+        idx_outliers = x > (median + 3 * mad)
 
     else:
         raise TypeError('Outlier detection method not found.')
 
     return idx_outliers | idx_range_outliers
 
 
@@ -231,27 +229,29 @@
 
     - P: atmospheric pressure
     - Pref: reference atmospheric pressure
     - L: Atmospheric attenuation coefficient.
 
 
     Args:
-        atm_pressure (list or array): Atmospheric pressure readings. Long-term average pressure is recommended.
+        pressure (list or array): Atmospheric pressure readings. Long-term average pressure is recommended.
         Pref (float): Reference atmospheric pressure.
         L (float): Atmospheric attenuation coefficient.
 
     Returns:
         (list): fp pressure correction factor.
 
     References:
+        Zreda, M., Shuttleworth, W. J., Zeng, X., Zweck, C., Desilets, D., Franz, T., and Rosolem, R.: COSMOS: the COsmic-ray Soil Moisture Observing System, Hydrol. Earth Syst. Sci., 16, 4079–4099, https://doi.org/10.5194/hess-16-4079-2012, 2012.
+
         M. Andreasen, K.H. Jensen, D. Desilets, T.E. Franz, M. Zreda, H.R. Bogena, and M.C. Looms. 2017. Status and perspectives on the cosmic-ray neutron method for soil moisture estimation and other environmental science applications. Vadose Zone J. 16(8). doi:10.2136/vzj2017.04.0086
     """
 
     # Compute pressure correction factor
-    fp = np.exp((Pref - pressure) / L) # Zreda et al. 2017 Eq 5.
+    fp = np.exp((Pref - pressure) / L)  # Zreda et al. 2017 Eq 5.
 
     return fp
 
 
 def correction_humidity(abs_humidity, Aref):
     r"""Correction factor for absolute humidity.
 
@@ -274,28 +274,32 @@
     where:
 
     - A: absolute humidity
     - Aref: reference absolute humidity
 
     Args:
         abs_humidity (list or array): Relative humidity readings.
-        temp (list or array): Temperature readings (Celsius).
         Aref (float): Reference absolute humidity (g/m^3). The day of the instrument calibration is recommended.
 
     Returns:
         (list): fw correction factor.
 
     References:
+        Rosolem, R., W. J. Shuttleworth, M. Zreda, T. E. Franz, X. Zeng, and S. A. Kurc, 2013: The Effect of Atmospheric Water Vapor on Neutron Count in the Cosmic-Ray Soil Moisture Observing System. J. Hydrometeor., 14, 1659–1671, https://doi.org/10.1175/JHM-D-12-0120.1.
+
         M. Andreasen, K.H. Jensen, D. Desilets, T.E. Franz, M. Zreda, H.R. Bogena, and M.C. Looms. 2017. Status and perspectives on the cosmic-ray neutron method for soil moisture estimation and other environmental science applications. Vadose Zone J. 16(8). doi:10.2136/vzj2017.04.0086
     """
     A = abs_humidity
-    fw = 1 + 0.0054*(A - Aref) # Zreda et al. 2017 Eq 6.
+    fw = 1 + 0.0054 * (A - Aref)  # Zreda et al. 2017 Eq 6.
     return fw
 
-def correction_incoming_flux(incoming_neutrons, incoming_Ref=None):
+
+def correction_incoming_flux(incoming_neutrons, incoming_Ref=None, fill_na=None, Rc_method=None, Rc_site=None,
+                             site_atmdepth=None, Rc_ref=None, ref_atmdepth=None):
+
     r"""Correction factor for incoming neutron flux.
 
     This function corrects neutron counts for incoming neutron flux using the method described in Anderson et al. (2017). The correction is performed using the following equation:
 
     $$
     C_{corrected} = \frac{C_{raw}}{f_i}
     $$
@@ -303,39 +307,67 @@
     where:
 
     - Ccorrected: corrected neutron counts
     - Craw: raw neutron counts
     - fi: incoming neutron flux correction factor
 
     $$
-    f_i = \frac{I_{ref}}{I}
+    f_i = \frac{I}{I_{ref}}
     $$
 
     where:
 
     - I: incoming neutron flux
     - Iref: reference incoming neutron flux
 
     Args:
         incoming_neutrons (list or array): Incoming neutron flux readings.
         incoming_Ref (float): Reference incoming neutron flux. Baseline incoming neutron flux.
+        fill_na (float): Value to fill missing data. If None, missing data remains as NaN.
+        Rc_method (str): Optional to correct for differences in cutoff rigidity between the site and the reference station. Possible values are 'McJannetandDesilets2023' or 'Hawdonetal2014'. If None, no correction is performed.
+        Rc_site (float): Cutoff rigidity at the monitoring site.
+        site_atmdepth (float): Atmospheric depth at the monitoring site.
+        Rc_ref (float): Cutoff rigidity at the reference station.
+        ref_atmdepth (float): Atmospheric depth at the reference station.
 
     Returns:
         (list): fi correction factor.
 
     References:
-        M. Andreasen, K.H. Jensen, D. Desilets, T.E. Franz, M. Zreda, H.R. Bogena, and M.C. Looms. 2017. Status and perspectives on the cosmic-ray neutron method for soil moisture estimation and other environmental science applications. Vadose Zone J. 16(8). doi:10.2136/vzj2017.04.0086
+        Hawdon, A., D. McJannet, and J. Wallace (2014), Calibration and correction procedures for cosmic-ray neutron soil moisture probes located across Australia, Water Resour. Res., 50, 5029–5043, doi:10.1002/2013WR015138.
 
+        M. Andreasen, K.H. Jensen, D. Desilets, T.E. Franz, M. Zreda, H.R. Bogena, and M.C. Looms. 2017. Status and perspectives on the cosmic-ray neutron method for soil moisture estimation and other environmental science applications. Vadose Zone J. 16(8). doi:10.2136/vzj2017.04.0086
 
+        McJannet, D. L., & Desilets, D. (2023). Incoming neutron flux corrections for cosmic-ray soil and snow sensors using the global neutron monitor network. Water Resources Research, 59, e2022WR033889. https://doi.org/10.1029/2022WR033889
     """
     if incoming_Ref is None and not isinstance(incoming_neutrons, type(None)):
         incoming_Ref = incoming_neutrons[0]
         warnings.warn('Reference incoming neutron flux not provided. Using first value of incoming neutron flux.')
     fi = incoming_neutrons / incoming_Ref
-    fi.fillna(1.0, inplace=True)  # Use a value of 1 for days without data
+
+    if Rc_method is not None:
+        if Rc_ref is None:
+            raise ValueError('Reference cutoff rigidity not provided.')
+        if Rc_site is None:
+            raise ValueError('Site cutoff rigidity not provided.')
+
+        if Rc_method == 'McJannetandDesilets2023':
+            tau = location_factor(site_atmdepth, Rc_site, ref_atmdepth, Rc_ref)
+            fi = 1 / (tau * fi + 1 - tau)
+
+        elif Rc_method == 'Hawdonetal2014':
+            Rc_corr = -0.075 * (Rc_site - Rc_ref) + 1.0
+            fi = (fi - 1.0) * Rc_corr + 1.0
+
+        else:
+            raise ValueError(
+                'Cutoff rigidity method not found. Valid options are: McJannetandDesilets2023, Hawdonetal2014.')
+
+    if fill_na is not None:
+        fi.fillna(fill_na, inplace=True)  # Use a value of 1 for days without data
 
     return fi
 
 
 def get_incoming_neutron_flux(start_date, end_date, station, utc_offset=0, expand_window=0, verbose=False):
     """Function to retrieve neutron flux from the Neutron Monitor Database.
 
@@ -350,61 +382,59 @@
     Returns:
         (pandas.DataFrame): Neutron flux in counts per hour and timestamps.
 
     References:
         Documentation available:https://www.nmdb.eu/nest/help.php#howto
     """
 
-    # Example: get_incoming_flux(station='IRKT',start_date='2020-04-10 11:00:00',end_date='2020-06-18 17:00:00')
+    # Example: get_incoming_neutron_flux(station='IRKT',start_date='2020-04-10 11:00:00',end_date='2020-06-18 17:00:00')
     # Template url = 'http://nest.nmdb.eu/draw_graph.php?formchk=1&stations[]=KERG&output=ascii&tabchoice=revori&dtype=corr_for_efficiency&date_choice=bydate&start_year=2009&start_month=09&start_day=01&start_hour=00&start_min=00&end_year=2009&end_month=09&end_day=05&end_hour=23&end_min=59&yunits=0'
 
-
     # Expand the time window by 1 hour to ensure an extra observation is included in the request.
     start_date -= pd.Timedelta(hours=expand_window)
     end_date += pd.Timedelta(hours=expand_window)
 
     # Convert local time to UTC
     start_date = start_date - pd.Timedelta(hours=utc_offset)
     end_date = end_date - pd.Timedelta(hours=utc_offset)
-    date_format = '%Y-%m-%d %H:%M:%S'
     root = 'http://www.nmdb.eu/nest/draw_graph.php?'
-    url_par = [ 'formchk=1',
-                'stations[]=' + station,
-                'output=ascii',
-                'tabchoice=revori',
-                'dtype=corr_for_efficiency',
-                'tresolution=' + str(60),
-                'date_choice=bydate',
-                'start_year=' + str(start_date.year),
-                'start_month=' + str(start_date.month),
-                'start_day=' + str(start_date.day),
-                'start_hour=' + str(start_date.hour),
-                'start_min=' + str(start_date.minute),
-                'end_year=' + str(end_date.year),
-                'end_month=' + str(end_date.month),
-                'end_day=' + str(end_date.day),
-                'end_hour=' + str(end_date.hour),
-                'end_min=' + str(end_date.minute),
-                'yunits=0']
+    url_par = ['formchk=1',
+               'stations[]=' + station,
+               'output=ascii',
+               'tabchoice=revori',
+               'dtype=corr_for_efficiency',
+               'tresolution=' + str(60),
+               'date_choice=bydate',
+               'start_year=' + str(start_date.year),
+               'start_month=' + str(start_date.month),
+               'start_day=' + str(start_date.day),
+               'start_hour=' + str(start_date.hour),
+               'start_min=' + str(start_date.minute),
+               'end_year=' + str(end_date.year),
+               'end_month=' + str(end_date.month),
+               'end_day=' + str(end_date.day),
+               'end_hour=' + str(end_date.hour),
+               'end_min=' + str(end_date.minute),
+               'yunits=0']
 
     url = root + '&'.join(url_par)
 
     if verbose:
         print(f"Retrieving data from {url}")
 
     r = requests.get(url).content.decode('utf-8')
 
     # Subtract 1 hour to restore the last date included in the request.
     end_date -= pd.Timedelta('1H')
     start = r.find("RCORR_E\n") + 8
     end = r.find('\n</code></pre><br>Total') - 1
     s = r[start:end]
-    s2 = ''.join([row.replace(';',',') for row in s])
+    s2 = ''.join([row.replace(';', ',') for row in s])
     try:
-        df_flux = pd.read_csv(io.StringIO(s2), names=['timestamp','counts'])
+        df_flux = pd.read_csv(io.StringIO(s2), names=['timestamp', 'counts'])
     except:
         if verbose:
             print(f"Error retrieving data from {url}")
         return None
 
     # Check if all values from selected detector are NaN. If yes, warn the user
     if df_flux['counts'].isna().all():
@@ -420,14 +450,40 @@
 the origin by a sentence like 'We acknowledge the NMDB database (www.nmdb.eu) founded under the European Union's FP7 programme 
 (contract no. 213007), and the PIs of individual neutron monitors at: IGY Jungfraujoch 
 (Physikalisches Institut, University of Bern, Switzerland)"""
 
     return df_flux
 
 
+def get_reference_neutron_flux(station, date=pd.to_datetime("2011-05-01")):
+    """Function to retrieve reference neutron flux from the Neutron Monitor Database. Default date is 2011-05-01, following previous studies (Zreda et a., 2012, Hawdon et al., 2014, Bogena et al., 2022).
+
+    Args:
+        station (str): Neutron Monitor station to retrieve data from.
+        date (datetime): Date of the reference neutron flux. Default is 2011-05-01.
+
+    Returns:
+        (float): Reference neutron flux in counts per hour.
+
+    References:
+        Zreda, M., Shuttleworth, W. J., Zeng, X., Zweck, C., Desilets, D., Franz, T., & Rosolem, R. (2012). COSMOS: The cosmic-ray soil moisture observing system. Hydrology and Earth System Sciences, 16(11), 4079-4099.
+
+        Hawdon, A., McJannet, D., & Wallace, J. (2014). Calibration and correction procedures for cosmic‐ray neutron soil moisture probes located across Australia. Water Resources Research, 50(6), 5029-5043.
+
+        Bogena, H. R., Schrön, M., Jakobi, J., Ney, P., Zacharias, S., Andreasen, M., ... & Vereecken, H. (2022). COSMOS-Europe: a European network of cosmic-ray neutron soil moisture sensors. Earth System Science Data, 14(3), 1125-1151.
+
+"""
+
+    # Get flux for 2011-05-01
+    df_flux = get_incoming_neutron_flux(date, date + pd.Timedelta(hours=24), station=station)
+    if df_flux is None:
+        warnings.warn(f"Reference neutron flux for {station} not available. Returning NaN.")
+    else:
+        return df_flux['counts'].median()
+
 
 def smooth_1d(values, window=5, order=3, method='moving_median'):
     """Use a Savitzky-Golay filter to smooth the signal of corrected neutron counts or another one-dimensional array (e.g. computed volumetric water content).
 
     Args:
         values (pd.DataFrame or pd.Serie): Dataframe containing the values to smooth.
         window (int): Window size for the Savitzky-Golay filter. Default is 5.
@@ -438,33 +494,40 @@
     Returns:
         (pd.DataFrame): DataFrame with smoothed values.
 
     References:
         Franz, T.E., Wahbi, A., Zhang, J., Vreugdenhil, M., Heng, L., Dercon, G., Strauss, P., Brocca, L. and Wagner, W., 2020.
         Practical data products from cosmic-ray neutron sensing for hydrological applications. Frontiers in Water, 2, p.9.
         doi.org/10.3389/frwa.2020.00009
+
+        Savitzky, A., & Golay, M. J. (1964). Smoothing and differentiation of data by simplified least squares procedures.
+        Analytical chemistry, 36(8), 1627-1639.
     """
 
+    if not isinstance(values, pd.Series) and not isinstance(values, pd.DataFrame):
+        raise ValueError('Input must be a pandas Series or DataFrame')
+
     if method == 'moving_average':
         corrected_counts = values.rolling(window=window, center=True, min_periods=1).mean()
     elif method == 'moving_median':
         corrected_counts = values.rolling(window=window, center=True, min_periods=1).median()
 
     elif method == 'savitzky_golay':
         if values.isna().any():
             print('Dataframe contains NaN values. Please remove NaN values before smoothing the data.')
 
         if type(values) == pd.core.series.Series:
-            filtered = savgol_filter(values,window,order)
-            corrected_counts = pd.DataFrame(filtered,columns=['smoothed'], index=values.index)
+            filtered = savgol_filter(values, window, order)
+            corrected_counts = pd.DataFrame(filtered, columns=['smoothed'], index=values.index)
         elif type(values) == pd.core.frame.DataFrame:
             for col in values.columns:
-                values[col] = savgol_filter(values[col],window,order)
+                values[col] = savgol_filter(values[col], window, order)
     else:
-        raise ValueError('Invalid method. Please select a valid filtering method., options are: moving_average, moving_median, savitzky_golay')
+        raise ValueError(
+            'Invalid method. Please select a valid filtering method., options are: moving_average, moving_median, savitzky_golay')
     corrected_counts = corrected_counts.ffill(limit=window).bfill(limit=window).copy()
     return corrected_counts
 
 
 def correction_bwe(counts, bwe, r2_N0=0.05):
     """Function to correct for biomass effects in neutron counts.
     following the approach described in Baatz et al., 2015.
@@ -479,15 +542,16 @@
 
     References:
         Baatz, R., H. R. Bogena, H.-J. Hendricks Franssen, J. A. Huisman, C. Montzka, and H. Vereecken (2015),
         An empiricalvegetation correction for soil water content quantification using cosmic ray probes,
         Water Resour. Res., 51, 2030–2046, doi:10.1002/ 2014WR016443.
     """
 
-    return counts/(1 - bwe*r2_N0)
+    return counts / (1 - bwe * r2_N0)
+
 
 def biomass_to_bwe(biomass_dry, biomass_fresh, fWE=0.494):
     """Function to convert biomass to biomass water equivalent.
 
     Args:
         biomass_dry (array or pd.Series or pd.DataFrame): Above ground dry biomass in kg m-2.
         biomass_fresh (array or pd.Series or pd.DataFrame): Above ground fresh biomass in kg m-2.
@@ -501,15 +565,16 @@
         Wahbi, A., Avery, W. (2018). In Situ Destructive Sampling. In:
         Cosmic Ray Neutron Sensing: Estimation of Agricultural Crop Biomass Water Equivalent.
         Springer, Cham. https://doi.org/10.1007/978-3-319-69539-6_2
     """
     return (biomass_fresh - biomass_dry) + fWE * biomass_dry
 
 
-def correction_road(counts, theta_N, road_width, road_distance=0.0, theta_road=0.12, p0=0.42, p1=0.5, p2=1.06, p3=4, p4=0.16, p6=0.94, p7=1.10, p8=2.70, p9=0.01):
+def correction_road(counts, theta_N, road_width, road_distance=0.0, theta_road=0.12, p0=0.42, p1=0.5, p2=1.06, p3=4,
+                    p4=0.16, p6=0.94, p7=1.10, p8=2.70, p9=0.01):
     """Function to correct for road effects in neutron counts.
     following the approach described in Schrön et al., 2018.
 
     Args:
         counts (array or pd.Series or pd.DataFrame): Array of ephithermal neutron counts.
         theta_N (float): Volumetric water content of the soil estimated from the uncorrected neutron counts.
         road_width (float): Width of the road in m.
@@ -521,25 +586,26 @@
         (array or pd.Series or pd.DataFrame): Array of corrected neutron counts for road effects.
 
     References:
         Schrön,M.,Rosolem,R.,Köhli,M., Piussi,L.,Schröter,I.,Iwema,J.,etal. (2018).Cosmic-ray neutron rover surveys
         of field soil moisture and the influence of roads.WaterResources Research,54,6441–6459.
         https://doi. org/10.1029/2017WR021719
     """
-    F1 = p0 * (1-np.exp(-p1*road_width))
+    F1 = p0 * (1 - np.exp(-p1 * road_width))
     F2 = -p2 - p3 * theta_road - ((p4 + theta_road) / (theta_N))
     F3 = p6 * np.exp(-p7 * (road_width ** -p8) * road_distance ** 4) + (1 - p6) * np.exp(-p9 * road_distance)
 
     C_roads = 1 + F1 * F2 * F3
 
     corrected_counts = counts / C_roads
 
     return corrected_counts
 
-def counts_to_vwc(counts, N0, Wlat, Wsoc ,bulk_density, a0=0.0808,a1=0.372,a2=0.115):
+
+def counts_to_vwc(counts, N0, Wlat, Wsoc, bulk_density, a0=0.0808, a1=0.372, a2=0.115):
     r"""Function to convert corrected and filtered neutron counts into volumetric water content.
 
     This method implements soil moisture estimation using the non-linear relationship between neutron count and soil volumetric water content following the approach described in Desilets et al., 2010.
 
     $\theta(N) =\frac{a_0}{(\frac{N}{N_0}) - a_1} - a_2 $
 
     Args:
@@ -558,21 +624,19 @@
     References:
         Desilets, D., M. Zreda, and T.P.A. Ferré. 2010. Nature’s neutron probe:
         Land surface hydrology at an elusive scale with cosmic rays. Water Resour. Res. 46:W11505.
         doi.org/10.1029/2009WR008726
     """
 
     # Convert neutron counts into vwc
-    vwc = (a0 / (counts/N0-a1) - a2 - Wlat - Wsoc) * bulk_density
+    vwc = (a0 / (counts / N0 - a1) - a2 - Wlat - Wsoc) * bulk_density
     return vwc
 
 
-
 def sensing_depth(vwc, pressure, p_ref, bulk_density, Wlat, dist=None, method='Schron_2017'):
-    # Convert docstring to google format
     """Function that computes the estimated sensing depth of the cosmic-ray neutron probe.
     The function offers several methods to compute the depth at which 86 % of the neutrons
     probe the soil profile.
 
     Args:
         vwc (array or pd.Series or pd.DataFrame): Estimated volumetric water content for each timestamp.
         pressure (array or pd.Series or pd.DataFrame): Atmospheric pressure in hPa for each timestamp.
@@ -594,32 +658,34 @@
         Improving calibration and validation of cosmic-ray neutron sensors in the light of spatial sensitivity.
         Hydrol. Earth Syst. Sci. 21, 5009–5030. doi.org/10.5194/hess-21-5009-2017
     """
 
     # Determine sensing depth (D86)
     if method == 'Schron_2017':
         # See Appendix A of Schrön et al. (2017)
-        Fp = 0.4922 / (0.86 - np.exp(-1 * pressure / p_ref));
+        Fp = 0.4922 / (0.86 - np.exp(-1 * pressure / p_ref))
         Fveg = 0
         results = []
         for d in dist:
             # Compute r_star
-            r_start = d/Fp
+            r_start = d / Fp
 
             # Compute soil depth that accounts for 86% of the neutron flux
-            D86 = 1/ bulk_density * (8.321+0.14249*(0.96655 + np.exp(-0.01*r_start))*(20+(Wlat+vwc)) / (0.0429+(Wlat+vwc)))
+            D86 = 1 / bulk_density * (8.321 + 0.14249 * (0.96655 + np.exp(-0.01 * r_start)) * (20 + (Wlat + vwc)) / (
+                    0.0429 + (Wlat + vwc)))
+
             results.append(D86)
 
     elif method == 'Franz_2012':
-        results = 5.8/(bulk_density*Wlat+vwc+0.0829)
+        results = 5.8 / (bulk_density * Wlat + vwc + 0.0829)
     else:
         raise ValueError('Method not recognized. Please select either "Schron_2017" or "Franz_2012".')
-
     return results
 
+
 def abs_humidity(relative_humidity, temp):
     """
     Compute the actual vapor pressure (e) in g m^-3 using RH (%) and current temperature (c) observations.
 
     Args:
         relative_humidity (float): relative humidity (%)
         temp (float): temperature (Celsius)
@@ -627,100 +693,324 @@
     Returns:
         float: actual vapor pressure (g m^-3)
     """
 
     ### Atmospheric water vapor factor
     # Saturation vapor pressure
     e_sat = 0.611 * np.exp(17.502 * temp / (
-                temp + 240.97)) * 1000  # in Pascals Eq. 3.8 p.41 Environmental Biophysics (Campbell and Norman)
+            temp + 240.97)) * 1000  # in Pascals Eq. 3.8 p.41 Environmental Biophysics (Campbell and Norman)
 
     # Vapor pressure Pascals
     Pw = e_sat * relative_humidity / 100
 
     # Absolute humidity (g/m^3)
     C = 2.16679  # g K/J;
     abs_h = C * Pw / (temp + 273.15)
     return abs_h
 
 
-def nrad_weight(h,theta,distances,depth,rhob=1.4):
+def nrad_weight(h, theta, distances, depth, profiles=None, rhob=1.4, method="Kohli_2015", p=None, Hveg=0, tol=0.01):
     """Function to compute distance weights corresponding to each soil sample.
 
     Args:
-        h (float): Air Humidity  from 0.1  to 50 in g/m^3. When h=0, the function will skip the distance weighting.
-        theta (array or pd.Series or pd.DataFrame): Soil Moisture for each sample (0.02 - 0.50 m^3/m^3)
-        distances (array or pd.Series or pd.DataFrame): Distances from the location of each sample to the origin (0.5 - 600 m)
-        depth (array or pd.Series or pd.DataFrame): Depths for each sample (m)
-        rhob (float): Bulk density in g/cm^3
+        h (np.array or pd.Series): Air Humidity  from 0.1  to 50 in g/m^3. When h=0, the function will skip the distance weighting.
+        theta (np.array or pd.Series): Soil Moisture for each sample (0.02 - 0.50 m^3/m^3)
+        distances (np.array or pd.Series): Distances from the location of each sample to the origin (0.5 - 600 m)
+        depth (np.array or pd.Series): Depths for each sample (m)
+        profiles (np.array or pd.Series): Soil profiles ID for each sample. Required for the 'Schron_2017' method.
+        rhob (np.array or pd.Series): Bulk density in g/cm^3
+        p (np.array or pd.Series): Atmospheric pressure in hPa. Required for the 'Schron_2017' method.
+        Hveg (np.array or pd.Series): Vegetation height in m. Required for the 'Schron_2017' method.
+        method (str): Method to compute the distance weights. Options are 'Kohli_2015' or 'Schron_2017'.
+        tol (float): Tolerance for the iterative solution. Default is 0.01. Required for the 'Schron_2017' method.
 
     Returns:
-        (array or pd.Series or pd.DataFrame): Distance weights for each sample.
+        theta_new (np.array or pd.Series): Weighted soil moisture values.
+        weights (np.array or pd.Series): Distance weights for each sample. For the 'Schron_2017' method, the weights are computed for each distance.
 
     References:
         Köhli, M., Schrön, M., Zreda, M., Schmidt, U., Dietrich, P., and Zacharias, S. (2015).
         Footprint characteristics revised for field-scale soil moisture monitoring with cosmic-ray
         neutrons. Water Resour. Res. 51, 5772–5790. doi:10.1002/2015WR017169
-    """
 
-    # Table A1. Parameters for Fi and D86
-    p10 = 8735;       p11 = 17.1758; p12 = 11720;      p13 = 0.00978;   p14 = 7045;      p15 = 0.003632;
-    p20 = 2.7925e-2;  p21 = 5.0399;  p22 = 2.8544e-2;  p23 = 0.002455;  p24 = 6.851e-5;  p25 = 9.2926;
-    p30 = 247970;     p31 = 17.63;   p32 = 374655;     p33 = 0.00191;   p34 = 195725;
-    p40 = 5.4818e-2;  p41 = 15.921;  p42 = 0.6373;     p43 = 5.99e-2;   p44 = 5.425e-4;
-    p50 = 1383702;    p51 = 4.156;   p52 = 5325;       p53 = 0.00238;   p54 = 0.0156;    p55 = 0.130;     p56 = 1521;
-    p60 = 6.031e-5;   p61 = 98.5;    p62 = 1.0466e-3;
-    p70 = 11747;      p71 = 41.66;   p72 = 4521;       p73 = 0.01998;   p74 = 0.00604;   p75 = 2534;      p76 = 0.00475;
-    p80 = 1.543e-2;   p81 = 10.06;   p82 = 1.807e-2;   p83 = 0.0011;    p84 = 8.81e-5;   p85 = 0.0405;    p86 = 20.24;
-    p90 = 8.321;      p91 = 0.14249; p92 = 0.96655;    p93 = 26.42;     p94 = 0.0567;
-
-
-    # Numerical determination of the penetration depth (86%) (Eq. 8)
-    D86 = 1/rhob*(p90+p91*(p92+np.exp(-1*distances/100))*(p93+theta)/(p94+theta))
-
-    # Depth weights (Eq. 7)
-    Wd = np.exp(-2*depth/D86)
-
-    if h == 0:
-        W = 1 # skip distance weighting
-
-    elif (h >= 0.1) and (h<= 50):
-        # Functions for Fi (Appendix A in Köhli et al., 2015)
-        F1 = p10*(1+p13*h)*np.exp(-p11*theta)+p12*(1+p15*h)-p14*theta
-        F2 = ((-p20+p24*h)*np.exp(-p21*theta/(1+p25*theta))+p22)*(1+h*p23)
-        F3 = (p30*(1+p33*h)*np.exp(-p31*theta)+p32-p34*theta)
-        F4 = p40*np.exp(-p41*theta)+p42-p43*theta+p44*h
-        F5 = p50*(0.02-1/p55/(h-p55+p56*theta))*(p54-theta)*np.exp(-p51*(theta-p54))+p52*(0.7-h*theta*p53)
-        F6 = p60*(h+p61)+p62*theta
-        F7 = (p70*(1-p76*h)*np.exp(-p71*theta*(1-h*p74))+p72-p75*theta)*(2+h*p73)
-        F8 = ((-p80+p84*h)*np.exp(-p81*theta/(1+p85*h+p86*theta))+p82)*(2+h*p83)
-
-        # Distance weights (Eq. 3)
-        W = np.ones_like(distances)*np.nan
-        for i in range(len(distances)):
-            if (distances[i]<=50) and (distances[i]>0.5):
-                W[i]=F1[i]*(np.exp(-F2[i]*distances[i]))+F3[i]*np.exp(-F4[i]*distances[i])
+        Schrön, M., Köhli, M., Scheiffele, L., Iwema, J., Bogena, H. R., Lv, L.,
+        Martini, E., Baroni, G., Rosolem, R., Weimar, J., Mai, J., Cuntz, M., Rebmann, C.,
+        Oswald, S. E., Dietrich, P., Schmidt, U., and Zacharias, S.: Improving calibration and
+        validation of cosmic-ray neutron sensors in the light of spatial sensitivity,
+        Hydrol. Earth Syst. Sci., 21, 5009–5030, https://doi.org/10.5194/hess-21-5009-2017, 2017.
+    """
+
+    if method == 'Kohli_2015':
+        # Table A1. Parameters for Fi and D86
+        p10 = 8735;
+        p11 = 17.1758;
+        p12 = 11720;
+        p13 = 0.00978;
+        p14 = 7045;
+        p15 = 0.003632;
+        p20 = 2.7925e-2;
+        p21 = 5.0399;
+        p22 = 2.8544e-2;
+        p23 = 0.002455;
+        p24 = 6.851e-5;
+        p25 = 9.2926;
+        p30 = 247970;
+        p31 = 17.63;
+        p32 = 374655;
+        p33 = 0.00191;
+        p34 = 195725;
+        p40 = 5.4818e-2;
+        p41 = 15.921;
+        p42 = 0.6373;
+        p43 = 5.99e-2;
+        p44 = 5.425e-4;
+        p50 = 1383702;
+        p51 = 4.156;
+        p52 = 5325;
+        p53 = 0.00238;
+        p54 = 0.0156;
+        p55 = 0.130;
+        p56 = 1521;
+        p60 = 6.031e-5;
+        p61 = 98.5;
+        p62 = 1.0466e-3;
+        p70 = 11747;
+        p71 = 41.66;
+        p72 = 4521;
+        p73 = 0.01998;
+        p74 = 0.00604;
+        p75 = 2534;
+        p76 = 0.00475;
+        p80 = 1.543e-2;
+        p81 = 10.06;
+        p82 = 1.807e-2;
+        p83 = 0.0011;
+        p84 = 8.81e-5;
+        p85 = 0.0405;
+        p86 = 20.24;
+        p90 = 8.321;
+        p91 = 0.14249;
+        p92 = 0.96655;
+        p93 = 26.42;
+        p94 = 0.0567;
+
+        # Numerical determination of the penetration depth (86%) (Eq. 8)
+        D86 = 1 / rhob * (p90 + p91 * (p92 + np.exp(-1 * distances / 100)) * (p93 + theta) / (p94 + theta))
+
+        # Depth weights (Eq. 7)
+        Wd = np.exp(-2 * depth / D86)
+
+        if h == 0:
+            W = 1  # skip distance weighting
+
+        elif (h >= 0.1) and (h <= 50):
+            # Functions for Fi (Appendix A in Köhli et al., 2015)
+            F1 = p10 * (1 + p13 * h) * np.exp(-p11 * theta) + p12 * (1 + p15 * h) - p14 * theta
+            F2 = ((-p20 + p24 * h) * np.exp(-p21 * theta / (1 + p25 * theta)) + p22) * (1 + h * p23)
+            F3 = (p30 * (1 + p33 * h) * np.exp(-p31 * theta) + p32 - p34 * theta)
+            F4 = p40 * np.exp(-p41 * theta) + p42 - p43 * theta + p44 * h
+            F5 = p50 * (0.02 - 1 / p55 / (h - p55 + p56 * theta)) * (p54 - theta) * np.exp(
+                -p51 * (theta - p54)) + p52 * (0.7 - h * theta * p53)
+            F6 = p60 * (h + p61) + p62 * theta
+            F7 = (p70 * (1 - p76 * h) * np.exp(-p71 * theta * (1 - h * p74)) + p72 - p75 * theta) * (2 + h * p73)
+            F8 = ((-p80 + p84 * h) * np.exp(-p81 * theta / (1 + p85 * h + p86 * theta)) + p82) * (2 + h * p83)
+
+            # Distance weights (Eq. 3)
+            W = np.ones_like(distances) * np.nan
+            for i in range(len(distances)):
+                if (distances[i] <= 50) and (distances[i] > 0.5):
+                    W[i] = F1[i] * (np.exp(-F2[i] * distances[i])) + F3[i] * np.exp(-F4[i] * distances[i])
 
-            elif (distances[i]>50) and (distances[i]<600):
-                W[i]=F5[i]*(np.exp(-F6[i]*distances[i]))+F7[i]*np.exp(-F8[i]*distances[i])
+                elif (distances[i] > 50) and (distances[i] < 600):
+                    W[i] = F5[i] * (np.exp(-F6[i] * distances[i])) + F7[i] * np.exp(-F8[i] * distances[i])
 
-            else:
-                raise ValueError('Input distances are not valid.')
+                else:
+                    raise ValueError('Input distances are not valid.')
 
-    else:
-        raise ValueError('Air humidity values are out of range.')
+        else:
+            raise ValueError('Air humidity values are out of range.')
+
+        # Combined and normalized weights
+        weights = Wd * W / np.nansum(Wd * W)
 
+        theta_new = np.sum(theta * weights)
 
-    # Combined and normalized weights
-    weights = Wd*W/np.nansum(Wd*W)
+        return theta_new, weights
+    elif method == 'Schron_2017':
+        # Horizontal distance weights According to Eq. 6 and Table A1 in Schrön et al. (2017)
+        # Method for calculating the horizontal distance weights from 0 to 1m
+        def WrX(r, x, y):
+            x00 = 3.7
+            a00 = 8735;
+            a01 = 22.689;
+            a02 = 11720;
+            a03 = 0.00978;
+            a04 = 9306;
+            a05 = 0.003632
+            a10 = 2.7925e-2;
+            a11 = 6.6577;
+            a12 = 0.028544;
+            a13 = 0.002455;
+            a14 = 6.851e-5;
+            a15 = 12.2755
+            a20 = 247970;
+            a21 = 23.289;
+            a22 = 374655;
+            a23 = 0.00191;
+            a24 = 258552
+            a30 = 5.4818e-2;
+            a31 = 21.032;
+            a32 = 0.6373;
+            a33 = 0.0791;
+            a34 = 5.425e-4
+
+            x0 = x00
+            A0 = (a00 * (1 + a03 * x) * np.exp(-a01 * y) + a02 * (1 + a05 * x) - a04 * y)
+            A1 = ((-a10 + a14 * x) * np.exp(-a11 * y / (1 + a15 * y)) + a12) * (1 + x * a13)
+            A2 = (a20 * (1 + a23 * x) * np.exp(-a21 * y) + a22 - a24 * y)
+            A3 = a30 * np.exp(-a31 * y) + a32 - a33 * y + a34 * x
+
+            return ((A0 * (np.exp(-A1 * r)) + A2 * np.exp(-A3 * r)) * (1 - np.exp(-x0 * r)))
+
+        # Method for calculating the horizontal distance weights from 1 to 50m
+        def WrA(r, x, y):
+            a00 = 8735;
+            a01 = 22.689;
+            a02 = 11720;
+            a03 = 0.00978;
+            a04 = 9306;
+            a05 = 0.003632
+            a10 = 2.7925e-2;
+            a11 = 6.6577;
+            a12 = 0.028544;
+            a13 = 0.002455;
+            a14 = 6.851e-5;
+            a15 = 12.2755
+            a20 = 247970;
+            a21 = 23.289;
+            a22 = 374655;
+            a23 = 0.00191;
+            a24 = 258552
+            a30 = 5.4818e-2;
+            a31 = 21.032;
+            a32 = 0.6373;
+            a33 = 0.0791;
+            a34 = 5.425e-4
+
+            A0 = (a00 * (1 + a03 * x) * np.exp(-a01 * y) + a02 * (1 + a05 * x) - a04 * y)
+            A1 = ((-a10 + a14 * x) * np.exp(-a11 * y / (1 + a15 * y)) + a12) * (1 + x * a13)
+            A2 = (a20 * (1 + a23 * x) * np.exp(-a21 * y) + a22 - a24 * y)
+            A3 = a30 * np.exp(-a31 * y) + a32 - a33 * y + a34 * x
+
+            return A0 * np.exp(-A1 * r) + A2 * np.exp(-A3 * r)
+
+        # Method for calculating the horizontal distance weights from 50 to 600m
+        def WrB(r, x, y):
+            b00 = 39006;
+            b01 = 15002337;
+            b02 = 2009.24;
+            b03 = 0.01181;
+            b04 = 3.146;
+            b05 = 16.7417;
+            b06 = 3727
+            b10 = 6.031e-5;
+            b11 = 98.5;
+            b12 = 0.0013826
+            b20 = 11747;
+            b21 = 55.033;
+            b22 = 4521;
+            b23 = 0.01998;
+            b24 = 0.00604;
+            b25 = 3347.4;
+            b26 = 0.00475
+            b30 = 1.543e-2;
+            b31 = 13.29;
+            b32 = 1.807e-2;
+            b33 = 0.0011;
+            b34 = 8.81e-5;
+            b35 = 0.0405;
+            b36 = 26.74
+
+            B0 = (b00 - b01 / (b02 * y + x - 0.13)) * (b03 - y) * np.exp(-b04 * y) - b05 * x * y + b06
+            B1 = b10 * (x + b11) + b12 * y
+            B2 = (b20 * (1 - b26 * x) * np.exp(-b21 * y * (1 - x * b24)) + b22 - b25 * y) * (2 + x * b23)
+            B3 = ((-b30 + b34 * x) * np.exp(-b31 * y / (1 + b35 * x + b36 * y)) + b32) * (2 + x * b33)
+
+            return B0 * np.exp(-B1 * r) + B2 * np.exp(-B3 * r)
+
+        # Wrapper method for calculating the horizontal distance weights
+        def Wr(r, x, y):
+            if r <= 1:
+                return WrX(r, x, y)
+            elif r <= 50:
+                return WrA(r, x, y)
+            elif r <= 600:
+                return WrB(r, x, y)
+            else:
+                raise ValueError("r must be between 1 and 600m when using 'Schron_2017' method")
+
+        def rscaled(r, p, y, Hveg = 0):
+            Fp = 0.4922 / (0.86 - np.exp(-p / 1013.25))
+            Fveg = 1 - 0.17 * (1 - np.exp(-0.41 * Hveg)) * (1 + np.exp(-9.25 * y))
+            return r / Fp / Fveg
+
+        if profiles is None:
+            raise ValueError("Profile ID's must be provided when using 'Schron_2017' method")
+
+        # Rename variables to be consistent with the revised paper
+        r = distances
+        theta_ = np.mean(theta) # Start with the mean value of theta as initial guess
+        bd = np.mean(rhob) # Neutrons are impacted by the bulk density across the whole area and not just the sample area. https://github.com/soilwater/crnpy/issues/9#issuecomment-2003813777
+
+        # Vertical distance weights functions
+        def D86(r, bd, y):
+            return 1 / bd * (8.321 + 0.14249 * (0.96655 + np.exp(-0.01 * r)) * (20 + y) / (0.0429 + y))
+
+        def Wd(d, r, bd, y):
+            return np.exp(-2 * d / D86(r, bd, y))
+
+        step = 0
+        diff = 1
+        while diff > tol:
+            step += 1
+            print(f"Step {step}, diff = {diff}", end="\r")
+            # Calculate the scaled distance and D86
+            r = rscaled(distances, p, theta_, Hveg)
+
+            # Calculate the vertical average for each profile
+            P = np.unique(profiles)
+            theta_P = []
+            r_stars = []
+            for i in range(len(P)):
+                profile = P[i]
+                idx = profiles == profile
+                depths_P = depth[idx]
+                r_P = r[idx]
+                theta_Pi = theta[idx]
+                # Calculate the vertical distance weights
+                Wd_P = Wd(depths_P, r_P, bd, theta_Pi)
+                # Calculate the vertical average of theta
+                theta_P_i = np.sum(Wd_P * theta_Pi) / np.sum(Wd_P)
+                theta_P.append(theta_P_i)
+                r_stars.append(np.mean(r_P))
+
+            # Calculate the horizontal distance weights
+            Wrs = np.array([Wr(r_star, theta_p, Hveg) for r_star, theta_p in zip(r_stars, theta_P)])
+            theta_new = np.sum(Wrs * theta_P) / np.sum(Wrs)
+            diff = np.abs(theta_new - theta_)
+            theta_ = theta_new
 
-    return weights
+        print(f"Solution converged after {step} steps, the average soil moisture is {theta_new}")
 
+        return theta_new, [theta_P, r_stars, Wrs]
+    else:
+        raise ValueError(f"Method {method} not recognized. Please use one of the following methods: 'Kohli_2015' or 'Schron_2017'")
 
 
-def exp_filter(sm,T=1):
+def exp_filter(sm, T=1):
     """Exponential filter to estimate soil moisture in the rootzone from surface observtions.
 
     Args:
         sm (list or array): Soil moisture in mm of water for the top layer of the soil profile.
         T (float): Characteristic time length in the same units as the measurement interval.
 
     Returns:
@@ -734,44 +1024,43 @@
         Franz, T.E., Wahbi, A., Zhang, J., Vreugdenhil, M., Heng, L., Dercon, G., Strauss, P., Brocca, L. and Wagner, W., 2020.
         Practical data products from cosmic-ray neutron sensing for hydrological applications. Frontiers in Water, 2, p.9.
 
         Rossini, P. and Patrignani, A., 2021. Predicting rootzone soil moisture from surface observations in cropland using an exponential filter.
         Soil Science Society of America Journal.
     """
 
-
     # Parameters
     t_delta = 1
     sm_min = np.min(sm)
     sm_max = np.max(sm)
     ms = (sm - sm_min) / (sm_max - sm_min)
 
     # Pre-allocate soil water index array and recursive constant K
-    SWI = np.ones_like(ms)*np.nan
-    K = np.ones_like(ms)*np.nan
+    SWI = np.ones_like(ms) * np.nan
+    K = np.ones_like(ms) * np.nan
 
     # Initial conditions
     SWI[0] = ms[0]
     K[0] = 1
 
     # Values from 2 to N
-    for n in range(1,len(SWI)):
-        if ~np.isnan(ms[n]) & ~np.isnan(ms[n-1]):
-            K[n] = K[n-1] / (K[n-1] + np.exp(-t_delta/T))
-            SWI[n] = SWI[n-1] + K[n]*(ms[n] - SWI[n-1])
+    for n in range(1, len(SWI)):
+        if ~np.isnan(ms[n]) & ~np.isnan(ms[n - 1]):
+            K[n] = K[n - 1] / (K[n - 1] + np.exp(-t_delta / T))
+            SWI[n] = SWI[n - 1] + K[n] * (ms[n] - SWI[n - 1])
         else:
             continue
 
     # Rootzone storage
     sm_subsurface = SWI * (sm_max - sm_min) + sm_min
 
     return sm_subsurface
 
 
-def cutoff_rigidity(lat,lon):
+def cutoff_rigidity(lat, lon):
     """Function to estimate the approximate cutoff rigidity for any point on Earth according to the
     tabulated data of Smart and Shea, 2019. The returned value can be used to select the appropriate
     neutron monitor station to estimate the cosmic-ray neutron intensity at the location of interest.
 
     Args:
         lat (float): Geographic latitude in decimal degrees. Value in range -90 to 90
         lon (float): Geographic longitude in decimal degrees. Values in range from 0 to 360.
@@ -784,43 +1073,134 @@
         Estimate the cutoff rigidity for Newark, NJ, US
 
         >>> zq = cutoff_rigidity(39.68, -75.75)
         >>> print(zq)
         2.52 GV (Value from NMD is 2.40 GV)
 
     References:
+        Hawdon, A., McJannet, D., & Wallace, J. (2014). Calibration and correction procedures
+        for cosmic‐ray neutron soil moisture probes located across Australia. Water Resources Research,
+        50(6), 5029-5043.
+
         Smart, D. & Shea, Matthew. (2001). Geomagnetic Cutoff Rigidity Computer Program:
         Theory, Software Description and Example. NASA STI/Recon Technical Report N.
 
         Shea, M. A., & Smart, D. F. (2019, July). Re-examination of the First Five Ground-Level Events.
         In International Cosmic Ray Conference (ICRC2019) (Vol. 36, p. 1149).
     """
     xq = lon
     yq = lat
 
     if xq < 0:
-        xq = xq*-1 + 180
+        xq = xq * -1 + 180
     Z = np.array(data.cutoff_rigidity)
     x = np.linspace(0, 360, Z.shape[1])
     y = np.linspace(90, -90, Z.shape[0])
     X, Y = np.meshgrid(x, y)
-    points = np.array( (X.flatten(), Y.flatten()) ).T
+    points = np.array((X.flatten(), Y.flatten())).T
     values = Z.flatten()
-    zq = griddata(points, values, (xq,yq))
+    zq = griddata(points, values, (xq, yq))
+
+    return np.round(zq, 2)
+
+def atmospheric_depth(elevation, latitude):
+    """Function to estimate the atmospheric depth for any point on Earth according to McJannet and Desilets, 2023
+
+    This function is required in the calculation of the location-dependent reference correction proposed by McJannet and Desilets, 2023.
+
+    Args:
+        elevation (float): Elevation in meters above sea level.
+        latitude (float): Geographic latitude in decimal degrees. Value in range -90 to 90
+
+    Returns:
+        (float): Atmospheric depth in g/cm2
+
+    References:
+        Atmosphere, U. S. (1976). US standard atmosphere. National Oceanic and Atmospheric Administration.
+
+        McJannet, D. L., & Desilets, D. (2023). Incoming Neutron Flux Corrections for Cosmic‐Ray Soil and Snow Sensors Using the Global Neutron Monitor Network. Water Resources Research, 59(4), e2022WR033889.
+    """
+
+    density_of_rock = 2670  # Density of rock in kg/m3
+    air_pressure_sea_level = 1013.25  # Air pressure at sea level in hPa
+    air_molar_mass = 0.0289644  # Air molar mass in kg/mol
+    universal_gas_constant = 8.31432  # Universal gas constant in J/(mol*K)
+    reference_temperature = 288.15  # Reference temperature Kelvin
+    temperature_lapse_rate = -0.0065  # Temperature lapse rate in K/m
+
+    # Gravity at sea-level calculation
+    gravity_sea_level = 9.780327 * (
+            1 + 0.0053024 * np.sin(np.radians(latitude)) ** 2 - 0.0000058 * np.sin(2 * np.radians(latitude)) ** 2)
+    # Free air correction
+    free_air = -3.086 * 10 ** -6 * elevation
+    # Bouguer correction
+    bouguer_corr = 4.193 * 10 ** -10 * density_of_rock * elevation
+    # Total gravity
+    gravity = gravity_sea_level + free_air + bouguer_corr
+
+    # Air pressure calculation
+    reference_air_pressure = air_pressure_sea_level * (
+            1 + temperature_lapse_rate / reference_temperature * elevation) ** ((-gravity * air_molar_mass) / (
+            universal_gas_constant * temperature_lapse_rate))
+
+    # Atmospheric depth calculation
+    atmospheric_depth = (10 * reference_air_pressure) / gravity
+    return atmospheric_depth
+
+
+def location_factor(site_atmospheric_depth, site_Rc, reference_atmospheric_depth, reference_Rc):
+    """
+    Function to estimate the location factor between two sites according to McJannet and Desilets, 2023.
+
+
+    Args:
+        site_atmospheric_depth (float): Atmospheric depth at the site in g/cm2. Can be estimated using the function `atmospheric_depth()`
+        site_Rc (float): Cutoff rigidity at the site in GV. Can be estimated using the function `cutoff_rigidity()`
+        reference_atmospheric_depth (float): Atmospheric depth at the reference location in g/cm2.
+        reference_Rc (float): Cutoff rigidity at the reference location in GV.
+
+    Returns:
+        (float): Location-dependent correction factor.
+
+    References:
+        McJannet, D. L., & Desilets, D. (2023). Incoming Neutron Flux Corrections for Cosmic‐Ray Soil and Snow Sensors Using the Global Neutron Monitor Network. Water Resources Research, 59(4), e2022WR033889.
+
+    """
+
+    # Renamed variables based on the provided table
+    c0 = -0.0009  # from C39
+    c1 = 1.7699  # from C40
+    c2 = 0.0064  # from C41
+    c3 = 1.8855  # from C42
+    c4 = 0.000013  # from C43
+    c5 = -1.2237  # from C44
+    epsilon = 1  # from C45
+
+    # Translated formula with renamed variables from McJannet and Desilets, 2023
+    tau_new = epsilon * (c0 * reference_atmospheric_depth + c1) * (
+            1 - np.exp(
+        -(c2 * reference_atmospheric_depth + c3) * reference_Rc ** (c4 * reference_atmospheric_depth + c5)))
+
+    norm_factor = 1 / tau_new
+
+    # Calculate the result using the provided parameters
+    tau = epsilon * norm_factor * (c0 * site_atmospheric_depth + c1) * (
+            1 - np.exp(-(c2 * site_atmospheric_depth + c3) * site_Rc ** (c4 * site_atmospheric_depth + c5)))
+    return tau
 
-    return np.round(zq,2)
 
 
 def find_neutron_monitor(Rc, start_date=None, end_date=None, verbose=False):
     """Search for potential reference neutron monitoring stations based on cutoff rigidity.
 
     Args:
         Rc (float): Cutoff rigidity in GV. Values in range 1.0 to 3.0 GV.
         start_date (datetime): Start date for the period of interest.
         end_date (datetime): End date for the period of interest.
+        verbose (bool): If True, print a expanded output of the incoming neutron flux data.
 
     Returns:
         (list): List of top five stations with closes cutoff rigidity.
             User needs to select station according to site altitude.
 
     Examples:
         >>> from crnpy import crnpy
@@ -842,70 +1222,77 @@
         57   YKTK                       Yakutsk  1.65         105
 
     References:
         https://www.nmdb.eu/nest/help.php#helpstations
     """
 
     # Load file with list of neutron monitoring stations
-    stations = pd.DataFrame(data.neutron_detectors, columns=["STID","NAME","R","Altitude_m"])
+    stations = pd.DataFrame(data.neutron_detectors, columns=["STID", "NAME", "R", "Altitude_m"])
 
     # Sort stations by closest cutoff rigidity
     idx_R = (stations['R'] - Rc).abs().argsort()
 
     if start_date is not None and end_date is not None:
         stations["Period available"] = False
         for i in range(10):
             station = stations.iloc[idx_R[i]]["STID"]
             try:
                 if get_incoming_neutron_flux(start_date, end_date, station, verbose=verbose) is not None:
-                    stations.iloc[idx_R[i],-1] = True
+                    stations.iloc[idx_R[i], -1] = True
             except:
                 pass
+
         if sum(stations["Period available"] == True) == 0:
             print("No stations available for the selected period!")
         else:
             stations = stations[stations["Period available"] == True]
             idx_R = (stations['R'] - Rc).abs().argsort()
             result = stations.iloc[idx_R.iloc[:10]]
     else:
         result = stations.reindex(idx_R).head(10).rename_axis(None)
 
     # Print results
     print('')
-    print("""Select a station with an altitude similar to that of your location. For more information go to: 'https://www.nmdb.eu/nest/help.php#helpstations""")
+    print(
+        """Select a station with an altitude similar to that of your location. For more information go to: 'https://www.nmdb.eu/nest/help.php#helpstations""")
     print('')
     print(f"Your cutoff rigidity is {Rc} GV")
     print(result)
     return result
 
 
 def interpolate_incoming_flux(nmdb_timestamps, nmdb_counts, crnp_timestamps):
     """Function to interpolate incoming neutron flux to match the timestamps of the observations.
 
     Args:
-        nmdb_timestamps (pd.Series): Series of timestamps in datetime format from the NMDB.
-        nmdb_counts (pd.Series): Series of neutron counts from the NMDB
-        crnp_timestamps (pd.Series): Series of timestamps in datetime format from the station or device.
+        nmdb_timestamps (pd.Series or np.array): Series or array of timestamps in datetime format from the NMDB
+        nmdb_counts (pd.Series or np.array): Series or array of incoming neutron flux counts from the NMDB
+        crnp_timestamps (pd.Series or np.array): Series or array of timestamps in datetime format from the CRNP device
 
     Returns:
         (pd.Series): Series containing interpolated incoming neutron flux. Length of Series is the same as crnp_timestamps
     """
-    incoming_flux = np.array([])
-    for k,timestamp in enumerate(crnp_timestamps):
-        if timestamp in nmdb_timestamps.values:
-            idx = timestamp == nmdb_timestamps
-            incoming_flux = np.append(incoming_flux, nmdb_counts.loc[idx])
-        else:
-            incoming_flux = np.append(incoming_flux, np.nan)
+    # Create a DataFrame from nmdb timestamps and counts
+    df_nmdb = pd.DataFrame({'timestamp': nmdb_timestamps, 'counts': nmdb_counts})
+
 
-    # Interpolate nan values
-    incoming_flux = pd.Series(incoming_flux).interpolate(method='nearest', limit_direction='both')
+    # Set the Timestamp column as the index
+    df_nmdb.set_index('timestamp', inplace=True)
 
-    # Return only the values for the selected timestamps
-    return incoming_flux
+    # Reindex the DataFrame to the timestamps from the CRNP device using the nearest method
+    # This will match each CRNP timestamp with the nearest NMDB timestamp
+    interpolated_flux = df_nmdb.reindex(crnp_timestamps, method='nearest')['counts'].values
+
+    # drop NaN values
+    interpolated_flux = interpolated_flux[~np.isnan(interpolated_flux)]
+
+    assert len(interpolated_flux) == len(
+        crnp_timestamps), "Length of interpolated flux does not match length of CRNP timestamps"
+
+    return interpolated_flux
 
 
 def lattice_water(clay_content, total_carbon=None):
     r"""Estimate the amount of water in the lattice of clay minerals.
 
     ![img1](img/lattice_water_simple.png) | ![img2](img/lattice_water_multiple.png)
     :-------------------------:|:-------------------------:
@@ -923,100 +1310,52 @@
     if total_carbon is None:
         lattice_water = 0.097 * clay_content
     else:
         lattice_water = -0.028 + 0.077 * clay_content + 0.459 * total_carbon
     return lattice_water
 
 
-def latlon_to_utm(lat, lon, utm_zone_number, missing_values=None):
+def latlon_to_utm(lat, lon, utm_zone_number=None, utm_zone_letter=None):
     """Convert geographic coordinates (lat, lon) to projected coordinates (utm) using the Military Grid Reference System.
 
     Function only applies to non-polar coordinates.
     If further functionality is required, consider using the utm module. See references for more information.
 
     ![UTM zones](https://upload.wikimedia.org/wikipedia/commons/thumb/b/b7/Universal_Transverse_Mercator_zones.svg/1920px-Universal_Transverse_Mercator_zones.svg.png)
     UTM zones on an equirectangular world map with irregular zones in red and New York City's zone highlighted. See [UTM zones](https://en.wikipedia.org/wiki/Universal_Transverse_Mercator_coordinate_system#UTM_zones) for a full description.
 
 
     Args:
         lat (float, array): Latitude in decimal degrees.
         lon (float, array): Longitude in decimal degrees.
-        utm_zone_number (int): Universal Transverse Mercator (UTM) zone.
+        utm_zone_number (int): UTM zone number. If None, the zone number is automatically calculated.
+        utm_zone_letter (str): UTM zone letter. If None, the zone letter is automatically calculated.
 
     Returns:
-        (float, float): Tuple of easting and northing coordinates in meters. First element is easting, second is northing.
+        (float, float, int, str): Tuple of easting, northing, zone number and zone letter. First element is easting, second is northing, third is zone number and fourth is zone letter.
 
     References:
          Code adapted from utm module created by Tobias Bieniek (Github username: Turbo87)
          [https://github.com/Turbo87/utm](https://github.com/Turbo87/utm)
 
          [https://www.maptools.com/tutorials/grid_zone_details#](https://www.maptools.com/tutorials/grid_zone_details#)
     """
+    # utm module requires numpy arrays
+    if not isinstance(lat, np.ndarray):
+        lat = np.array(lat)
+    if not isinstance(lon, np.ndarray):
+        lon = np.array(lon)
 
+    if utm_zone_number is None or utm_zone_letter is None:
+        easting, northing, zone_number, zone_letter = utm.from_latlon(lat, lon)
+    else:
+        easting, northing, zone_number, zone_letter = utm.from_latlon(lat, lon, utm_zone_number, utm_zone_letter)
 
-    # Define constants
-    R = 6_378_137  # Earth's radius at the Equator in meters
-
-    # Convert input data to Numpy arrays
-    if (type(lat) is not np.ndarray) or (type(lon) is not np.ndarray):
-        try:
-            lat = np.array(lat)
-            lon = np.array(lon)
-        except:
-            raise "Input values cannot be converted to Numpy arrays."
-
-    # Check latitude range
-    if np.any(lat < -80) | np.any(lat > 84):
-        raise "One or more latitude values exceed the range -80 to 84"
-
-    # Check longitude range
-    if np.any(lon < -180) | np.any(lon > 180):
-        raise "One or more longitude values exceed the range -180 to 180"
-
-    # Constants
-    K0 = 0.9996
-    E = 0.00669438
-    E_P2 = E / (1 - E)
-
-    M1 = (1 - E / 4 - 3 * E ** 2 / 64 - 5 * E ** 3 / 256)
-    M2 = (3 * E / 8 + 3 * E ** 2 / 32 + 45 * E ** 3 / 1024)
-    M3 = (15 * E ** 2 / 256 + 45 * E ** 3 / 1024)
-    M4 = (35 * E ** 3 / 3072)
-
-    # Trigonometric operations
-    lat_rad = np.radians(lat)
-    lon_rad = np.radians(lon)
-
-    lat_sin = np.sin(lat_rad)
-    lat_cos = np.cos(lat_rad)
-    lat_tan = lat_sin / lat_cos
-    lat_tan2 = lat_tan * lat_tan
-    lat_tan4 = lat_tan2 * lat_tan2
-
-    # Find central meridian.
-    central_lon = (utm_zone_number * 6 - 180) - 3  # Zones are every 6 degrees.
-    central_lon_rad = np.radians(central_lon)
-
-    n = R / np.sqrt(1 - E * lat_sin ** 2)
-    c = E_P2 * lat_cos ** 2
-
-    with np.errstate(divide='ignore', invalid='ignore'):
-        a = lat_cos * (np.remainder(((lon_rad - central_lon_rad) + np.pi), (2 * np.pi)) - np.pi)
-    m = R * (M1 * lat_rad - M2 * np.sin(2 * lat_rad) + M3 * np.sin(4 * lat_rad) - M4 * np.sin(6 * lat_rad))
-
-    easting = K0 * n * (a + a ** 3 / 6 * (1 - lat_tan2 + c) + a ** 5 / 120 * (
-                5 - 18 * lat_tan2 + lat_tan4 + 72 * c - 58 * E_P2)) + 500_000
-    northing = K0 * (m + n * lat_tan * (
-                a ** 2 / 2 + a ** 4 / 24 * (5 - lat_tan2 + 9 * c + 4 * c ** 2) + a ** 6 / 720 * (
-                    61 - 58 * lat_tan2 + lat_tan4 + 600 * c - 330 * E_P2)))
-
-    if np.any(lat < 0):
-        northing += 10_000_000
+    return easting, northing, zone_number, zone_letter
 
-    return easting, northing
 
 def euclidean_distance(px, py, x, y):
     """Function that computes the Euclidean distance between one point
     in space and one or more points.
 
     Args:
         px (float): x projected coordinate of the point.
@@ -1064,26 +1403,25 @@
     for k in range(N):
         px = x[k]
         py = y[k]
 
         distances = euclidean_distance(px, py, x, y)
         idx_within_buffer = distances <= buffer
 
-
         if np.isnan(z[k]):
             z_new_val = np.nan
         elif len(distances[idx_within_buffer]) > min_neighbours:
             if method == 'mean':
                 z_new_val = np.nanmean(z[idx_within_buffer])
             elif method == 'median':
                 z_new_val = np.nanmedian(z[idx_within_buffer])
             else:
                 raise f"Method {method} does not exist. Provide either 'mean' or 'median'."
         else:
-            z_new_val = z[k] # If there are not enough neighbours, keep the original value
+            z_new_val = z[k]  # If there are not enough neighbours, keep the original value
 
         # Append smoothed value to array
         z_smooth = np.append(z_smooth, z_new_val)
 
     if rnd:
         z_smooth = np.round(z_smooth, 0)
 
@@ -1156,15 +1494,16 @@
     # Drop NaN values in x y and z
     idx_nan = np.isnan(x) | np.isnan(y) | np.isnan(z)
     x = x[~idx_nan]
     y = y[~idx_nan]
     z = z[~idx_nan]
 
     if idx_nan.any():
-        print(f"WARNING: {np.isnan(x).sum()}, {np.isnan(y).sum()}, and {np.isnan(z).sum()} NaN values were dropped from x, y, and z.")
+        print(
+            f"WARNING: {np.isnan(x).sum()}, {np.isnan(y).sum()}, and {np.isnan(z).sum()} NaN values were dropped from x, y, and z.")
 
     # Create 2D grid for interpolation
     Nx = round((np.max(x) - np.min(x)) / dx) + 1
     Ny = round((np.max(y) - np.min(y)) / dy) + 1
     X_vec = np.linspace(np.min(x), np.max(x), Nx)
     Y_vec = np.linspace(np.min(y), np.max(y), Ny)
     X_pred, Y_pred = np.meshgrid(X_vec, Y_vec)
@@ -1191,28 +1530,27 @@
 
     Returns:
         x_est (array): Estimated x coordinates.
         y_est (array): Estimated y coordinates.
     """
 
     # Make it datatype agnostic
-    if(isinstance(x, pd.Series)):
+    if (isinstance(x, pd.Series)):
         x = x.values
-    if(isinstance(y, pd.Series)):
+    if (isinstance(y, pd.Series)):
         y = y.values
 
     # Do the average of the two points
     x_est = (x[1:] + x[:-1]) / 2
     y_est = (y[1:] + y[:-1]) / 2
 
     # Add the first point to match the length of the original array
     x_est = np.insert(x_est, 0, x[0])
     y_est = np.insert(y_est, 0, y[0])
 
-
     return x_est, y_est
 
 
 def uncertainty_counts(raw_counts, metric="std", fp=1, fw=1, fi=1):
     """Function to estimate the uncertainty of raw counts.
 
     Measurements of proportional neutron detector systems are governed by counting statistics that follow a Poissonian probability distribution (Zreda et al., 2012).
@@ -1238,21 +1576,21 @@
 
     """
 
     s = fw / (fp * fi)
     if metric == "std":
         uncertainty = np.sqrt(raw_counts) * s
     elif metric == "cv":
-        uncertainty = 1 /  np.sqrt(raw_counts) * s
+        uncertainty = 1 / np.sqrt(raw_counts) * s
     else:
         raise f"Metric {metric} does not exist. Provide either 'std' or 'cv' for standard deviation or coefficient of variation."
     return uncertainty
 
 
-def uncertainty_vwc(raw_counts, N0, bulk_density, fp=1, fw=1, fi=1, a0=0.0808,a1=0.372,a2=0.115):
+def uncertainty_vwc(raw_counts, N0, bulk_density, fp=1, fw=1, fi=1, a0=0.0808, a1=0.372, a2=0.115):
     r"""Function to estimate the uncertainty propagated to volumetric water content.
 
     The uncertainty of the volumetric water content is estimated by propagating the uncertainty of the raw counts.
     Following Eq. 10 in Jakobi et al. (2020), the uncertainty of the volumetric water content can be expressed as:
     $$
     \sigma_{\theta_g}(N) = \sigma_N \frac{a_0 N_0}{(N_{cor} - a_1 N_0)^4} \sqrt{(N_{cor} - a_1 N_0)^4 + 8 \sigma_N^2 (N_{cor} - a_1 N_0)^2 + 15 \sigma_N^4}
     $$
@@ -1271,21 +1609,12 @@
     References:
         Jakobi J, Huisman JA, Schrön M, Fiedler J, Brogi C, Vereecken H and Bogena HR (2020) Error Estimation for Soil Moisture Measurements With
         Cosmic Ray Neutron Sensing and Implications for Rover Surveys. Front. Water 2:10. doi: 10.3389/frwa.2020.00010
     """
 
     Ncorr = raw_counts * fw / (fp * fi)
     sigma_N = uncertainty_counts(raw_counts, metric="std", fp=fp, fw=fw, fi=fi)
-    sigma_GWC = sigma_N * ((a0*N0) / ((Ncorr - a1*N0)**4)) * np.sqrt((Ncorr - a1 * N0)**4 + 8 * sigma_N**2 * (Ncorr - a1 * N0)**2 + 15 * sigma_N**4)
+    sigma_GWC = sigma_N * ((a0 * N0) / ((Ncorr - a1 * N0) ** 4)) * np.sqrt(
+        (Ncorr - a1 * N0) ** 4 + 8 * sigma_N ** 2 * (Ncorr - a1 * N0) ** 2 + 15 * sigma_N ** 4)
     sigma_VWC = sigma_GWC * bulk_density
 
     return sigma_VWC
-
-
-
-
-
-
-
-
-
-
```

### Comparing `crnpy-0.5.1/src/crnpy/data.py` & `crnpy-0.6.0/src/crnpy/data.py`

 * *Files identical despite different names*

### Comparing `crnpy-0.5.1/src/crnpy.egg-info/PKG-INFO` & `crnpy-0.6.0/src/crnpy.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 Metadata-Version: 2.1
 Name: crnpy
-Version: 0.5.1
+Version: 0.6.0
 Summary: A Python package for the estimation and processing of soil moisture data from cosmic-ray neutron counts.
-Home-page: https://github.com/soilwater/crnpy
+Home-page: https://soilwater.github.io/crnpy/
 Author: Joaquin Peraza, Andres Patrignani
 Author-email: jperaza@ksu.edu, andrespatrignani@ksu.edu
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: scipy
+Requires-Dist: requests
+Requires-Dist: utm
 
 [![GitHub Workflow Status (building)](https://img.shields.io/github/actions/workflow/status/soilwater/crnpy/python-package.yml)](https://github.com/soilwater/crnpy/actions/workflows/python-package.yml)
 [![GitHub Workflow Status (publish)](https://img.shields.io/github/actions/workflow/status/soilwater/crnpy/python-publish.yml?label=publish)](https://github.com/soilwater/crnpy/actions/workflows/python-publish.yml)
 [![PyPI - Status](https://img.shields.io/pypi/v/crnpy)](https://pypi.org/project/crnpy/)
 [![GitHub commits since latest release (by SemVer including pre-releases)](https://img.shields.io/github/commits-since/soilwater/crnpy/latest/main)](https://github.com/soilwater/crnpy)
+![JOSS submission status](https://joss.theoj.org/papers/e65c1bb5fee58c39289efc4547d1fd10/status.svg)
 
 # Cosmic-Ray Neutron Python (CRNPy) Library
 
 <img src="https://raw.githubusercontent.com/soilwater/crnpy/main/docs/img/logo/crnpy-logo.png" alt="CRNPY logo" width="250"/>
 
 ## Overview
 Welcome to the homepage of the CRNPy (Cosmic-Ray Neutron Python) library, an open-source Python library designed for the processing and conversion of raw neutron counts from cosmic-ray neutron probes (CRNP) into soil moisture data.
@@ -28,15 +34,14 @@
 
 ## Key Features
 - Versatile and instrument agnostic: CRNPy can handle data from various CRNP manufacturers and models. It has been successfully tested on both roving and stationary CRNP.
 
 - Modular: The library is designed to be modular, allowing users to easily customize the processing workflow to their needs.
 
 
-
 ## Installation
 To install the CRNPy library, you can use Python's package manager. Open a terminal and type:
 
 ```pip install crnpy```
 
 from the Jupyter notebook, type:
 
@@ -45,14 +50,20 @@
 Ideally dependencies should be installed automatically. If not, you can install them manually by typing:
 
 ```pip install -r requirements.txt```
 
 The CRNPy library is compatible with Python 3.7 and above.
 See [requirements.txt](https://github.com/soilwater/crnpy/blob/main/requirements.txt) for a list of dependencies.
 
+## Examples
+
+- [https://soilwater.github.io/crnpy/examples/stationary/example_RDT_station/](Processing and analyzing data from a stationary detector)
+- [https://soilwater.github.io/crnpy/examples/rover/Hydroinnova_rover_example/](Processing and analyzing data from a roving detector)
+- [https://soilwater.github.io/crnpy/examples/calibration/calibration/](Device-specific field calibration)
+
 ## Authors
 The CRNPy library was developed at the Kansas State University Soil Water Processes Lab by:
 
 - Joaquin Peraza
 
 - Andres Patrignani
```

