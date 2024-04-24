# Comparing `tmp/svinsight-0.2.8.tar.gz` & `tmp/svinsight-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svinsight-0.2.8.tar", last modified: Wed Apr 17 20:29:12 2024, max compression
+gzip compressed data, was "svinsight-0.3.0.tar", last modified: Wed Apr 24 16:03:35 2024, max compression
```

## Comparing `svinsight-0.2.8.tar` & `svinsight-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 matthewpreisser   (501) staff       (20)        0 2024-04-17 20:29:12.527010 svinsight-0.2.8/
--rw-r--r--   0 matthewpreisser   (501) staff       (20)     1073 2024-04-12 14:13:08.000000 svinsight-0.2.8/LICENSE
--rw-r--r--   0 matthewpreisser   (501) staff       (20)      783 2024-04-17 20:29:12.526720 svinsight-0.2.8/PKG-INFO
--rw-r--r--   0 matthewpreisser   (501) staff       (20)      208 2024-04-15 14:32:42.000000 svinsight-0.2.8/README.md
-drwxr-xr-x   0 matthewpreisser   (501) staff       (20)        0 2024-04-17 20:29:12.524908 svinsight-0.2.8/SVInsight/
--rw-r--r--   0 matthewpreisser   (501) staff       (20)       57 2024-04-17 20:16:27.000000 svinsight-0.2.8/SVInsight/__init__.py
--rw-r--r--   0 matthewpreisser   (501) staff       (20)    17061 2024-04-15 15:22:19.000000 svinsight-0.2.8/SVInsight/census_variables.py
--rw-r--r--   0 matthewpreisser   (501) staff       (20)    59348 2024-04-17 19:36:33.000000 svinsight-0.2.8/SVInsight/svi.py
-drwxr-xr-x   0 matthewpreisser   (501) staff       (20)        0 2024-04-17 20:29:12.526498 svinsight-0.2.8/SVInsight.egg-info/
--rw-r--r--   0 matthewpreisser   (501) staff       (20)      783 2024-04-17 20:29:12.000000 svinsight-0.2.8/SVInsight.egg-info/PKG-INFO
--rw-r--r--   0 matthewpreisser   (501) staff       (20)      462 2024-04-17 20:29:12.000000 svinsight-0.2.8/SVInsight.egg-info/SOURCES.txt
--rw-r--r--   0 matthewpreisser   (501) staff       (20)        1 2024-04-17 20:29:12.000000 svinsight-0.2.8/SVInsight.egg-info/dependency_links.txt
--rw-r--r--   0 matthewpreisser   (501) staff       (20)      135 2024-04-17 20:29:12.000000 svinsight-0.2.8/SVInsight.egg-info/requires.txt
--rw-r--r--   0 matthewpreisser   (501) staff       (20)       10 2024-04-17 20:29:12.000000 svinsight-0.2.8/SVInsight.egg-info/top_level.txt
--rw-r--r--   0 matthewpreisser   (501) staff       (20)      757 2024-04-17 20:29:09.000000 svinsight-0.2.8/pyproject.toml
--rw-r--r--   0 matthewpreisser   (501) staff       (20)       38 2024-04-17 20:29:12.527068 svinsight-0.2.8/setup.cfg
--rw-r--r--   0 matthewpreisser   (501) staff       (20)      828 2024-04-17 20:28:31.000000 svinsight-0.2.8/setup.py
-drwxr-xr-x   0 matthewpreisser   (501) staff       (20)        0 2024-04-17 20:29:12.526371 svinsight-0.2.8/tests/
--rw-r--r--   0 matthewpreisser   (501) staff       (20)     6769 2024-04-17 19:36:33.000000 svinsight-0.2.8/tests/test_svinsight.py
+drwxr-xr-x   0 matthewpreisser   (501) staff       (20)        0 2024-04-24 16:03:35.993900 svinsight-0.3.0/
+-rw-r--r--   0 matthewpreisser   (501) staff       (20)     1073 2024-04-12 14:13:08.000000 svinsight-0.3.0/LICENSE
+-rw-r--r--   0 matthewpreisser   (501) staff       (20)      982 2024-04-24 16:03:35.993697 svinsight-0.3.0/PKG-INFO
+-rw-r--r--   0 matthewpreisser   (501) staff       (20)     3082 2024-04-24 15:50:56.000000 svinsight-0.3.0/README.md
+drwxr-xr-x   0 matthewpreisser   (501) staff       (20)        0 2024-04-24 16:03:35.991435 svinsight-0.3.0/SVInsight/
+-rw-r--r--   0 matthewpreisser   (501) staff       (20)       57 2024-04-24 15:57:57.000000 svinsight-0.3.0/SVInsight/__init__.py
+-rw-r--r--   0 matthewpreisser   (501) staff       (20)    17061 2024-04-15 15:22:19.000000 svinsight-0.3.0/SVInsight/census_variables.py
+-rw-r--r--   0 matthewpreisser   (501) staff       (20)    76938 2024-04-23 20:46:50.000000 svinsight-0.3.0/SVInsight/svi.py
+drwxr-xr-x   0 matthewpreisser   (501) staff       (20)        0 2024-04-24 16:03:35.993473 svinsight-0.3.0/SVInsight.egg-info/
+-rw-r--r--   0 matthewpreisser   (501) staff       (20)      982 2024-04-24 16:03:35.000000 svinsight-0.3.0/SVInsight.egg-info/PKG-INFO
+-rw-r--r--   0 matthewpreisser   (501) staff       (20)      462 2024-04-24 16:03:35.000000 svinsight-0.3.0/SVInsight.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewpreisser   (501) staff       (20)        1 2024-04-24 16:03:35.000000 svinsight-0.3.0/SVInsight.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewpreisser   (501) staff       (20)       86 2024-04-24 16:03:35.000000 svinsight-0.3.0/SVInsight.egg-info/requires.txt
+-rw-r--r--   0 matthewpreisser   (501) staff       (20)       10 2024-04-24 16:03:35.000000 svinsight-0.3.0/SVInsight.egg-info/top_level.txt
+-rw-r--r--   0 matthewpreisser   (501) staff       (20)     1057 2024-04-24 15:58:08.000000 svinsight-0.3.0/pyproject.toml
+-rw-r--r--   0 matthewpreisser   (501) staff       (20)       38 2024-04-24 16:03:35.993939 svinsight-0.3.0/setup.cfg
+-rw-r--r--   0 matthewpreisser   (501) staff       (20)      828 2024-04-24 15:58:01.000000 svinsight-0.3.0/setup.py
+drwxr-xr-x   0 matthewpreisser   (501) staff       (20)        0 2024-04-24 16:03:35.993265 svinsight-0.3.0/tests/
+-rw-r--r--   0 matthewpreisser   (501) staff       (20)     7918 2024-04-18 18:30:46.000000 svinsight-0.3.0/tests/test_svinsight.py
```

### Comparing `svinsight-0.2.8/LICENSE` & `svinsight-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `svinsight-0.2.8/PKG-INFO` & `svinsight-0.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.1
 Name: SVInsight
-Version: 0.2.8
+Version: 0.3.0
 Summary: Create social vulnerabilty index
 Home-page: https://github.com/mdp0023/SVInsight/
-Author: M. Preisser, P. Passalacqua, R. P. Bixler
+Author: Paola Passalacqua, R. Patrick Bixler
 Author-email: Matthew Preisser <mattpreisser@gmail.com>
-Project-URL: Homepage, https://example.com
-Project-URL: Documentation, https://readthedocs.org
-Keywords: SVI
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python
-Requires-Python: >=3.8
+Project-URL: Homepage, https://github.com/mdp0023/SVInsight
+Project-URL: Documentation, https://mdp0023.github.io/SVInsight/
+Keywords: SVI,Social-Vulnerability,Hazards,Census,Demographics
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: census>=0.8.21
-Requires-Dist: factor_analyzer>=0.5.1
-Requires-Dist: geopandas>=0.14.2
-Requires-Dist: numpy>=1.26.4
-Requires-Dist: pandas>=2.2.2
-Requires-Dist: PyYAML>=6.0.1
-Requires-Dist: scikit_learn>=1.3.0
-Requires-Dist: openpyxl>=3.0.10
+Requires-Dist: census
+Requires-Dist: factor_analyzer
+Requires-Dist: geopandas
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: PyYAML
+Requires-Dist: scikit_learn
+Requires-Dist: openpyxl
+Requires-Dist: matplotlib
```

### Comparing `svinsight-0.2.8/SVInsight/census_variables.py` & `svinsight-0.3.0/SVInsight/census_variables.py`

 * *Files identical despite different names*

### Comparing `svinsight-0.2.8/SVInsight/svi.py` & `svinsight-0.3.0/SVInsight/svi.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 
 import os 
 import csv
 import copy
 import shutil
-import zipfile
+# import zipfile
 import numpy as np
 import requests
 import pandas as pd
-from ftplib import FTP
-import ftputil
+# from ftplib import FTP
 import geopandas as gpd
 from census import Census
 import concurrent.futures
+import matplotlib.pyplot as plt
+from matplotlib.patches import Patch
+import matplotlib as mpl
 from concurrent.futures import ThreadPoolExecutor
 from sklearn.preprocessing import MinMaxScaler
 from factor_analyzer import FactorAnalyzer
 import yaml
+from scipy.stats import pearsonr
+import scipy.stats as stats
 
 from .census_variables import setup_census_variables
 
 # current structure:
     # Each instance of class is a standalone project for a given study area.
     # A user can run different boundaries (tract or bg) and years within a single project
     # Will have a method to generate a .yaml file to save the variables (configuration) of a run 
@@ -158,20 +162,20 @@
         :type year: int
         :param overwrite: whether or not to overwrite an existing geopackage if it exists. Default is False
         :type overwrite: bool
 
         :return: The boundary data as a GeoDataFrame.
         :rtype: gpd.GeoDataFrame
 
-        :raises ValueError: If the boundary type is invalid, the year is not between 2010 and 2022, or geoids not properly formatted.
+        :raises ValueError: If the boundary type is invalid, the year is not between 2013 and 2021, or geoids not properly formatted.
         """
         
         # Validate Variables
         self._validate_value(boundary, ['bg', 'tract'], 'boundary')
-        self._validate_value(year, [2010, 2012, 2013, 2014, 2015, 2016, 2017, 2018, 2019, 2020, 2021, 2022], 'year')
+        self._validate_value(year, [2013, 2014, 2015, 2016, 2017, 2018, 2019, 2020, 2021], 'year')
         self._validate_format(boundary, str, 'boundary')
         self._validate_format(year, int, 'year')
 
 
         # If shapefile already exists, pass 
         if os.path.exists(os.path.join(self.boundaries, f"{self.project_name}_{year}_{boundary}.gpkg")) and overwrite is False:
             
@@ -183,15 +187,15 @@
 
             # helper functions
             def _download(year, state, boundary):
                 """
                 Downloads a shapefile from a remote FTP server, extracts it, and returns the boundary shapefile as a GeoDataFrame.
 
                 Args:
-                    year (int): The year of the shapefile.
+                    year (int): The year of the shapefile. Valid options are from 2011 to 2021.
                     state (str): The state abbreviation.
                     boundary (str): The boundary type. Must be 'bg' or 'tract'
 
                 Returns:
                     geopandas.GeoDataFrame: The boundary shapefile as a GeoDataFrame.
                 """
                
@@ -211,29 +215,31 @@
                 # # Open the file locally and write it to folder
                 # print('opening binary')
                 # with open(zipped_dir, "wb") as file:
                 #     ftp.retrbinary(f"RETR {zipped_filename}", file.write)
                 # print('opened binary')
 
                 # Specify the URL of the file you want to download
-                url = f"https://www2.census.gov/geo/tiger/GENZ{year}/shp/{zipped_filename}"
-
+                if year >= 2014:
+                    url = f"https://www2.census.gov/geo/tiger/GENZ{year}/shp/{zipped_filename}"
+                elif year == 2013:
+                    url = f"https://www2.census.gov/geo/tiger/GENZ{year}/{zipped_filename}"
+               
                 # Send a GET request to the URL
                 response = requests.get(url, stream=True)
 
                 # Check if the request was successful
                 if response.status_code == 200:
                     # Open a local file with the same name as the remote file
                     with open(zipped_dir, 'wb') as file:
                         # Write the contents of the remote file to the local file
                         for chunk in response.iter_content(chunk_size=1024):
                             if chunk:
                                 file.write(chunk)
 
-
                 # Unzip the file
                 shutil.unpack_archive(zipped_dir, filename_dir)
                 # with zipfile.ZipFile(f"{zipped_dir}", 'r') as zip_ref:
                 #     zip_ref.extractall(filename_dir)
 
                 # Read the shapefile with geopandas
                 boundary_shp = gpd.read_file(f"{filename_dir}/{filename}.shp")
@@ -293,32 +299,32 @@
     # Method to pull census data and fill holes
     def census_data(self, boundary: str = 'bg', year: int = 2019, interpolate: bool = True, verbose: bool = False, overwrite: bool = False):
         """
         Pulls Census data for a specific boundary and year.
 
         :param boundary: The boundary type to retrieve data for. Valid options are 'bg' (block group) and 'tract' (census tract).
         :type boundary: str
-        :param year: The year of the Census data to retrieve. Valid options are from 2010 to 2022.
+        :param year: The year of the Census data to retrieve. Valid options are from 2011 to 2021.
         :type year: int
-        :param interpolate: Whether to interpolate missing data. Defaults to True.
+        :param interpolate: Whether to interpolate missing data. Defaults to True. If year is before 2014, ignored and not-interpolated.
         :type interpolate: bool, optional
         :param verbose: Whether to display verbose output. Defaults to False.
         :type verbose: bool, optional
         :param overwrite: Whether to overwrite existing data. Defaults to False.
         :type overwrite: bool, optional
 
-        :raises ValueError: If the boundary type is invalid or the year is not between 2010 and 2022.
+        :raises ValueError: If the boundary type is invalid or the year is not between 2013 and 2021.
         :raises FileNotFoundError: If the shapefile for the specified boundary and year does not exist.
 
         :return: None
         :rtype: None
         """
         # Validate Variables
         self._validate_value(boundary, ['bg', 'tract'], 'boundary')
-        self._validate_value(year, [2010, 2012, 2013, 2014, 2015, 2016, 2017, 2018, 2019, 2020, 2021, 2022], 'year')
+        self._validate_value(year, [2013, 2014, 2015, 2016, 2017, 2018, 2019, 2020, 2021], 'year')
         self._validate_format(boundary, str, 'boundary')
         self._validate_format(year, int, 'year')
 
         # If data already exists and overwrite is False, don't pull data 
         if os.path.exists(os.path.join(self.data, f"{self.project_name}_{year}_{boundary}_rawdata.gpkg")) and overwrite is False:
             pass
         else:
@@ -399,24 +405,24 @@
         :type num: list
         :param den: The list of denominator variables used to calculate the variable. Default is [1].
         :type den: list, optional
         :param description: Optional description of the variable. Default is None.
         :type description: str, optional
         
         :raises ValueError: If the variable name already exists.
-        :raises ValueError: If the boundary type is invalid or the year is not between 2010 and 2022.
+        :raises ValueError: If the boundary type is invalid or the year is not between 2013 and 2021.
         :raises FileNotFoundError: If the raw data file doesn't exist. Run the census_data method first.
         
         :return: None
         :rtype: None
         """
         
         # Validate Variables
         self._validate_value(boundary, ['bg', 'tract'], 'boundary')
-        self._validate_value(year, [2010, 2012, 2013, 2014, 2015, 2016, 2017, 2018, 2019, 2020, 2021, 2022], 'year')
+        self._validate_value(year, [2013, 2014, 2015, 2016, 2017, 2018, 2019, 2020, 2021], 'year')
         
         # if name of variable already exists, raise error
         if name in self.all_vars_eqs:
             raise ValueError(f"Variable '{name}' already exists.")
 
         # open the raw data file as a df 
         if not os.path.exists(os.path.join(self.data, f"{self.project_name}_{year}_{boundary}_rawdata.gpkg")):
@@ -436,15 +442,15 @@
         # create list of raw data names that needs to be added
         vars = [var for var in num + den if isinstance(var, str)]
         missing_vars = [var for var in vars if var not in shapefile.keys()]
         if not missing_vars:
             pass
         else:
             # Pull Census data
-            data_df = self._census_pull(self.geoids, boundary, missing_vars, self.api_key, year,pop_filter=None)
+            data_df = self._census_pull(self.geoids, boundary, missing_vars, self.api_key, year, pop_filter=self.low_pop_filter)
             # Fill missing columns
             data_df = self._fill_empty(data_df, boundary, self.geoids, self.api_key, year, verbose=False)  
 
             # create a new column with a shared 'key' to relate dataframes to
             if boundary == 'bg':
                 shapefile['bg_fips'] = shapefile['GEOID']
                 # merge geopandas shapefile with data_df shapefile
@@ -520,15 +526,15 @@
         :type config_file: str
         :param boundary: The boundary type for the SVI calculation. Default is 'bg'.
         :type boundary: str
         :param year: The year for which the SVI is calculated. Default is 2019.
         :type year: int
 
         :returns: None
-        :raises ValueError: If the boundary type is invalid or the year is not between 2010 and 2022,
+        :raises ValueError: If the boundary type is invalid or the year is not between 2013 and 2021,
 
         This method reads a configuration file in YAML format, loads the raw data as a dataframe,
         calculates the SVI using two different methods, and saves the results to output files.
 
         **Method 1: Iterative Factor Analysis**
         
         - Conducts factor analysis on the input variables to identify significant components.
@@ -546,15 +552,15 @@
 
         The output dataframe is saved as a GeoPackage file and a CSV file.
         Additionally, intermediate results from Method 1 such as significant components, loading factors, and variances
         are saved in an Excel file for documentation purposes.
         """
         # validate inputs
         self._validate_value(boundary, ['bg', 'tract'], 'boundary')
-        self._validate_value(year, [2010, 2012, 2013, 2014, 2015, 2016, 2017, 2018, 2019, 2020, 2021, 2022], 'year')
+        self._validate_value(year, [2013, 2014, 2015, 2016, 2017, 2018, 2019, 2020, 2021], 'year')
 
         # open the configuration file
         with open(os.path.join(self.variables, f"{config_file}.yaml")) as stream:
             try:
                 docs = list(yaml.safe_load_all(stream))
             except yaml.YAMLError as exc:
                 print(exc)
@@ -647,21 +653,22 @@
 
             return sig_components, include, df_ratio_var, df_variances
 
 
         # 1. Scale data
         scaler = MinMaxScaler()
         fa_df = pd.DataFrame(data=scaler.fit_transform(fa_df), columns=fa_df.columns, index=fa_df.index)
-        
         # 2. Conduct Factor Analysis and calculate initial loading factors
         fa, n_factors, loading_factors, facs = _initalize_fa(fa_df)
         # 3. Calculate initial variances
         sig_components, include, df_ratio_var, df_variances = _calc_variance(fa, n_factors, loading_factors, facs, df_variances)
 
         num_refactors+=1
+
+        fa_refactor_df = fa_df[include].copy()
         # 4. Begin refactor loop with initial 'include' array
         while len(include) != len(fa_df.columns):
             fa_refactor_df = fa_df[include].copy()
             fa, n_factors, loading_factors, facs = _initalize_fa(fa_refactor_df)
             sig_components, include, df_ratio_var, df_variances = _calc_variance(fa, n_factors, loading_factors, facs, df_variances)
 
             # Determine if length of new dataset is equal to significant variables
@@ -730,19 +737,316 @@
         for col in rank_df.columns:
             rank_df[col] = rank_df[col].rank(ascending=False)
         rank_df['sum_rank'] = rank_df.sum(axis=1)
         output_df['RM_SVI_Rank'] = rank_df['sum_rank'].rank()
         output_df['RM_SVI_Percentile'] = rank_df['sum_rank'].rank(ascending=False, pct=True)
         
 
+        # Order check
+        # Determine if the slopes of the two ranks have opposite signs
+        output_df = output_df.sort_values('FA_SVI_Rank')
+        list1 = output_df['FA_SVI_Rank'].tolist()
+        list2 = output_df['RM_SVI_Rank'].tolist()
+        slope1, _ = np.polyfit(range(len(list1)), list1, 1)
+        slope2, _ = np.polyfit(range(len(list2)), list2, 1)
+        # Check if the slopes have different signs
+        if np.sign(slope1) != np.sign(slope2):
+            output_df['FA_SVI_Scaled'] = output_df['FA_SVI_Scaled'].max() - output_df['FA_SVI_Scaled']
+            output_df['FA_SVI_Rank'] = output_df['FA_SVI_Rank'].max() - output_df['FA_SVI_Rank']
+            output_df['FA_SVI_Percentile'] = output_df['FA_SVI_Percentile'].max() - output_df['FA_SVI_Percentile']
+        else:
+            pass
+
         # save geopackage and csv output
         output_df.to_file(os.path.join(self.svis, f"{self.project_name}_{year}_{boundary}_{config_file}_svi.gpkg"))
         output_df.to_csv(os.path.join(self.svis, f"{self.project_name}_{year}_{boundary}_{config_file}_svi.csv"))
          
 
+    # Method to create various plots
+    def plot_svi(self, plot_option: int, geopackages: list):
+        """
+        Simple plotting method to quickly map an SVI variable or compare two SVIs.
+
+        :param plot_option: Which plot method to use: Either 1 (single SVI map), 2 (two side by side maps), or 3 (full comparison figure).
+        :type plot_option: int
+        :param geopackages: The required information for plotting, must be format: [year, boundary, config, variable]. Nested list if plot_option 2.
+        :type geopackages: list
+
+
+        :returns: matplotlib figure object
+        :raises ValueError: If the boundary type is invalid or the year is not between 2013 and 2021,
+
+        
+        This method quickly creates an example SVI plot either by itself or in a comparative format. The plot options and their required information can be found below.
+
+        **Plot Option 1: Single Plot**
+
+        A single figure of a single SVI estimate. The geopackage parameter must be in the format [year, boundary, config, variable] where:
+
+        - Year: SVI estimate year (int)
+        - Boundary: Boundary of interest ('bg' or 'tract', str)
+        - Config: Which config file was used to create the SVI estimate (str)
+        - Variable: Which SVI variable to plot (i.e., the attributes of the SVI geopackages created, str). 
+
+        **Plot Option 2: Simple Comparative Plot**
+
+        A simple two by one figure to visually compare two differnet SVI estimates. These estimates can be from the same or different geopackages. The geopackages parameter should be a nested list of the same variables as described in plot option 1: [[year, boundary, config, variable],[year, boundary, config, variable]].
+
+        **Plot Option 3: Complete Comparative Plot**
+
+        A more detailed plotting option, that will produce a difference plot and calculate a linear regression. Because the difference map and linear regression require the same set of input geoids (i.e., the same locations in the geopackage), it is currently required that the variables come from the same geopackage, and its intended purpose is to therefore compare the differences between the Factor Analysis and Rank Method methodologies that have the same configuration. The geopackages input should be formated as follows: [year, boundary, config]. The additional plots show the following information:
+
+        - Difference plot: Shows the The FA_SVI_Rank minus the RM_SVI_Rank to highlight areas where the factor analysis method is under (negative) and over (positive) predicting SVI rank when compared to the rank method. 
+        - Linear Regression: Shows linear correlation betweeen factor analysis and rank method SVI estimates and automatically computes an r-squared value with p-value, 95% confidence interval, and 95% prediction interval.
+        
+        """
+        # Special Use Boundaries Legened Element
+        legend_elements = [Patch(facecolor='black', edgecolor='black',
+                                label='No Data Available')]
+        
+        # Single geopackage plot
+        if plot_option == 1:
+            if len(geopackages) != 4:
+                raise ValueError("geopackages must have length 4 for plot_option 1")
+            fig, (ax1, ax2) = plt.subplots(2, 1, 
+                            figsize=(6, 6), 
+                            gridspec_kw={'height_ratios': [9, 1]})
+            
+            # extract variables
+            year=geopackages[0]
+            boundary=geopackages[1]
+            config_file=geopackages[2]
+            var = geopackages[3]
+
+            # set titles
+            ax1.set_title(f'{self.project_name}_{year}_{boundary}_{config_file}:\n{var}')
+            ax1.legend(handles=legend_elements, loc='lower left')
+
+            # read geopackage of data
+            gdf=gpd.read_file(f"{self.svis}/{self.project_name}_{year}_{boundary}_{config_file}_svi.gpkg")
+            # read geopackage of background
+            background = gpd.read_file(f"{self.boundaries}/{self.project_name}_{year}_{boundary}.gpkg")
+
+            # plot the figure
+            self._plot_single(ax1, background, gdf, var)
+            
+            # plot cbar
+            self._plot_cmap(fig,ax2,plot_option)
+  
+            
+        # Double geopackage plot    
+        elif plot_option == 2:
+            if len(geopackages) != 2:
+                raise ValueError("For plot option 2, geopackages must have exactly 2 elements.")
+            for gp in geopackages:
+                if len(gp) != 4:
+                    raise ValueError("Each element in geopackages must have a length of 4.")
+            # Create Figure
+            fig, (ax1, ax2, ax3) = plt.subplots(1,3, 
+                                    figsize=(12,6),
+                                    gridspec_kw={'width_ratios':[9,1,9]})
+            axes = [ax1, ax3]
+            
+            # shift center axis over, move y labels to right
+            pos = ax2.get_position()
+            pos.x0 -= 0.01875  
+            pos.x1 -= 0.01875  
+            ax2.set_position(pos)
+            ax3.yaxis.tick_right()
+            ax3.yaxis.set_label_position("right")
+            
+            for idx, geopackage in enumerate(geopackages):
+                # extract variables
+                year=geopackage[0]
+                boundary=geopackage[1]
+                config_file=geopackage[2]
+                var = geopackage[3]
+
+                #set titles
+                axes[idx].set_title(f'{self.project_name}_{year}_{boundary}_{config_file}:\n{var}')
+                axes[idx].legend(handles=legend_elements, loc='lower left')
+
+                # read geopackage of data
+                gdf=gpd.read_file(f"{self.svis}/{self.project_name}_{year}_{boundary}_{config_file}_svi.gpkg")
+                # read geopackage of background
+                background = gpd.read_file(f"{self.boundaries}/{self.project_name}_{year}_{boundary}.gpkg")
+            
+                # plot the figure
+                self._plot_single(axes[idx], background, gdf, var)
+                
+            # plot cbar
+            self._plot_cmap(fig,ax2,plot_option)
+            
+                   
+        elif plot_option == 3:
+            if len(geopackages) != 3:
+                raise ValueError("For plot option 3, geopackages must have exactly 3 elements.")
+           # Create Figure
+            fig, axes = plt.subplots(2,3, 
+                                    figsize=(10,8),
+                                    gridspec_kw={'width_ratios':[9,1,9]})
+            ax1, ax2, ax3, ax4, ax5, ax6 = axes.flatten()
+
+            # shift center axis over, move y labels to right
+            pos = ax2.get_position()
+            pos.x0 -= 0.03
+            pos.x1 -= 0.03  
+            ax2.set_position(pos)
+            ax3.yaxis.tick_right()
+            ax3.yaxis.set_label_position("right")
+
+            pos = ax5.get_position()
+            pos.x0 -= 0.03  
+            pos.x1 -= 0.03 
+            ax5.set_position(pos)
+            ax6.yaxis.tick_right()
+            ax6.yaxis.set_label_position("right")
+            
+            axes = [ax1, ax3]
+
+            gdfs = []
+            vars=[]
+            f_names=[]
+
+            variables = ['FA_SVI_Rank', 'RM_SVI_Rank']
+            for idx, var in enumerate(variables):
+                # extract variables
+                year=geopackages[0]
+                boundary=geopackages[1]
+                config_file=geopackages[2]
+
+                #set titles
+                axes[idx].set_title(f'{self.project_name}_{year}_{boundary}_{config_file}:\n{var}')
+                axes[idx].legend(handles=legend_elements, loc='lower left')
+
+                # read geopackage of data
+                gdf=gpd.read_file(f"{self.svis}/{self.project_name}_{year}_{boundary}_{config_file}_svi.gpkg")
+                # read geopackage of background
+                background = gpd.read_file(f"{self.boundaries}/{self.project_name}_{year}_{boundary}.gpkg")
+                gdfs.append(gdf)
+                vars.append(var)
+                f_names.append(f'{self.project_name}_{year}_{boundary}_{config_file}')
+                # plot the figure
+                self._plot_single(axes[idx], background, gdf, var)
+                
+            # plot cbar for SVI
+            self._plot_cmap(fig,ax2,plot_option)
+
+            # merge to remove any different locations
+            merged_gdf = gdfs[0].merge(gdfs[1], left_index=True, right_index=True,suffixes=('_left', '_right'))
+            # Create difference
+            merged_gdf['difference'] = merged_gdf[f"{vars[0]}_left"] - merged_gdf[f"{vars[1]}_right"]
+
+            # # Custom color ramp for map of differences
+            cmap = mpl.cm.Spectral_r
+            bounds = np.linspace(0, 1, 10+1)
+            np.delete(bounds, 0)
+            bins = []
+            for bound in bounds:
+                bins.append(merged_gdf['difference'].quantile(bound))
+            norm = mpl.colors.BoundaryNorm(bounds, cmap.N)
+
+            # # plot difference
+            ax4.set_title('Difference (L - R)')
+            merged_gdf = gpd.GeoDataFrame(merged_gdf, geometry='geometry_left')
+            self._plot_single(ax4, background, merged_gdf, 'difference', cmap='Spectral_r')
+            ax4.legend(handles=legend_elements, loc='lower left')
+
+            cbar = fig.colorbar(mpl.cm.ScalarMappable(norm=norm, cmap=cmap),
+                                cax=ax5, orientation='vertical',
+                                label="Under/Over Prediction")
+            yticklabels = [str(round(float(label), 2)) for label in bins]
+            cbar.ax.set_yticklabels(yticklabels)
+
+
+            # determine correlation
+            pearson_r, p_value = pearsonr(merged_gdf[f"{vars[0]}_left"], merged_gdf[f"{vars[1]}_right"])
+
+            # calculate regression
+            x = merged_gdf[f"{vars[0]}_left"].values
+            y = merged_gdf[f"{vars[1]}_right"].values
+
+            slope, intercept = np.polyfit(x, y, 1)  # linear model adjustment
+
+            y_model = np.polyval([slope, intercept], x)   # modeling...
+
+            x_mean = np.mean(x)
+            y_mean = np.mean(y)
+            n = x.size                        # number of samples
+            m = 2                             # number of parameters
+            dof = n - m                       # degrees of freedom
+            t = stats.t.ppf(0.975, dof)       # Students statistic of interval confidence
+            residual = y - y_model
+            std_error = (np.sum(residual**2) / dof)**.5   # Standard deviation of the error
+
+            # calculating the r2
+            numerator = np.sum((x - x_mean)*(y - y_mean))
+            denominator = (np.sum((x - x_mean)**2) * np.sum((y - y_mean)**2))**.5
+            correlation_coef = numerator / denominator
+            r2 = correlation_coef**2
+
+            # mean squared error
+            MSE = 1/n * np.sum((y - y_model)**2)
+
+            # to plot the adjusted model
+            x_line = np.linspace(np.min(x), np.max(x), 100)
+            y_line = np.polyval([slope, intercept], x_line)
+
+            # confidence interval
+            ci = t * std_error * (1/n + (x_line - x_mean)**2 / np.sum((x - x_mean)**2))**.5
+            # predicting interval
+            pi = t * std_error * (1 + 1/n + (x_line - x_mean) **2 / np.sum((x - x_mean)**2))**.5
+
+            # plot scatter points
+            ax6.plot(x, y, 'o', color='royalblue')
+            # plot regression line
+            ax6.plot(x_line, y_line, color='royalblue')
+            # prediction interval
+            ax6.fill_between(x_line, 
+                            y_line + pi, 
+                            y_line - pi,
+                            color='lightcyan', 
+                            label='95% prediction interval')
+            # confidence interval
+            ax6.fill_between(x_line, 
+                            y_line + ci, 
+                            y_line - ci,
+                            color='skyblue', 
+                            label='95% confidence interval')
+                # set axis labels and limits
+            ax6.set_xlabel('Left plot')
+            ax6.set_ylabel('Right plot')
+            ax6.set_xlim([0, max(x)])
+            ax6.set_ylim([0, max(y)])
+
+            # rounding round appropriate values
+            a = str(np.round(intercept))
+            b = str(np.round(slope, 2))
+            r2s = str(np.round(r2, 2))
+            # p = str(np.round(p_value,2))
+            MSEs = str(np.round(MSE))
+
+            # plot text
+            textstr = '\n'.join((f'y = {a} + {b}x',
+                                f'$r^2$ = {r2s}',
+                                f'p-value = {p_value:.03g}'))
+            # patch properties
+            props = dict(boxstyle='square', facecolor='lightgray', alpha=0.80)
+            # text box in upper left in axes coords
+            ax6.text(0.025, 0.975,
+                    textstr,
+                    transform=ax6.transAxes,
+                    fontsize=8,
+                    verticalalignment='top',
+                    bbox=props)
+            legend = ax6.legend(fontsize=8, loc=4, facecolor='lightgray')
+            legend.get_frame().set_alpha(0.90)
+            legend.get_frame().set_edgecolor("black")
+
+        return fig
 
 
 
     ###################################################
     # PRIVATE METHODS (helper functions)
     ###################################################
 
@@ -901,21 +1205,33 @@
             high_range (list): A list of high range values for calculating the median.
             interpolated_output (list): A list to store information about interpolated data.
 
         Returns:
             pandas.DataFrame: The updated data_df with interpolated values.
 
         """
-        # Filter out the data that we want
+        # Select rows we are interested in 
         neighbor_data = holes_df.filter(items=neighbors, axis=0)
+        # select columns we are interested in 
         neighbor_data = neighbor_data.filter(like=filter_like, axis=1)
+        
+        # order from decreasing to increasing
+        # Extract the numeric part of the column names and convert to int
+        def extract_number(col_name):
+            return int(col_name.split('_')[1][:-1])
+        # Sort the columns based on the numeric part
+        sorted_columns = sorted(neighbor_data.columns, key=extract_number)
+        # Reorder the DataFrame
+        neighbor_data = neighbor_data[sorted_columns]
+
         # sum data
         sum_neighbor_data = neighbor_data.sum()
         # determine total number of sample points
         N = sum_neighbor_data[drop]
+        
         # can now drop this value from dataframe
         sum_neighbor_data.drop(drop, inplace=True)
         
         if var == 'B01002_001E':
             # have to combine like female and male categories
             pairs = [['B01001_003E', 'B01001_027E'], ['B01001_004E', 'B01001_028E'], ['B01001_005E', 'B01001_029E'], 
                      ['B01001_006E', 'B01001_030E'], ['B01001_007E', 'B01001_031E'], ['B01001_008E', 'B01001_032E'], 
@@ -949,38 +1265,60 @@
             # create median calculation dictionary
             calc = pd.DataFrame.from_dict({'low_range':low_range,
                                             'high_range':high_range,
                                             'freq': sum_neighbor_data,
                                             'cumsum_perc': cumsum_perc})
 
             # determine lower limit of the median interval
-            index = abs(calc['freq'].cumsum() - N/2).idxmin()
-            L1 = calc['low_range'][index+1]
+            index = (calc['freq'].cumsum() >= N/2).idxmax()
+            #L1 = calc['low_range'][index+1]
+            
 
             if index == 0:
-                # not enough info, don't interpolate
+                # not enough info, median is in lowest bound, don't interpolate
                 pass
             else:
-                # determine the number of data points below the median interval
-                cumsum_before = calc['freq'].cumsum()[index-1]
-                # determine the width of the median interval
-                width = calc['high_range'][index + 1] - calc['low_range'][index + 1] + 1
-                # determine the number of data points in the median interval
-                freq_medain = calc['freq'][index + 1]
-                # rare case if new median falls in range of values with zero frequency
-                if freq_medain == 0:
-                    median = L1 + (N/2 - cumsum_before)
-                else:
-                    # calculate median
-                    median = L1 + (N/2 - cumsum_before) / freq_medain * width
+                # determine median count 
+                median_count = np.round(N/2,0)
+                # Determine number of points in range needed to get to median
+                points_needed =  median_count - calc['freq'].cumsum()[index-1]
+
+                # determine proportion (returns 0 if divide by 0)
+                p = np.divide(points_needed, calc['freq'][index], out=np.zeros_like(points_needed), where=calc['freq'].cumsum()[index]!=0)
+               
+                # # determine the width of the median interval
+                width = calc['high_range'][index] - calc['low_range'][index]
+                
+                # calculate the new value 
+                interpolated_value = p*width+calc['low_range'][index]
+
                 # fill in values of data frame
-                data_df.loc[fips, var] = median
+                data_df.loc[fips, var] = interpolated_value
+                    
                 interpolated_output.append([f'{fips}', var, 'Interpolated'])
 
 
+                # # determine the number of data points below the median interval
+                # cumsum_before = calc['freq'].cumsum()[index-1]
+                # # determine the width of the median interval
+                # width = calc['high_range'][index + 1] - calc['low_range'][index + 1] + 1
+                # # determine the number of data points in the median interval
+                # freq_medain = calc['freq'][index + 1]
+                # # rare case if new median falls in range of values with zero frequency
+                # if freq_medain == 0:
+                #     median = L1 + (N/2 - cumsum_before)
+                # else:
+                #     # calculate median
+                #     median = L1 + (N/2 - cumsum_before) / freq_medain * width
+                # print(L1, N, cumsum_before, freq_medain, width, median)
+                # # fill in values of data frame
+                # data_df.loc[fips, var] = median
+                # interpolated_output.append([f'{fips}', var, 'Interpolated'])
+
+
         return data_df
   
     # helper function, find holes
     def __find_holes(self, data_df):
         """
         Finds missing holes in the given data DataFrame.
 
@@ -1192,14 +1530,16 @@
             interpolate (bool): If True, interpolate missing values. If False, fill missing values without interpolation.
             verbose (bool, optional): If True, save the interpolated info output as a CSV file. Defaults to False.
 
         Returns:
             pandas.DataFrame: The DataFrame with missing values filled.
 
         """
+        if year <= 2014:
+            interpolate = False
         # create output data file to save interpolated results
         interpolated_output=[]
 
         # find holes
         miss_vals, unique_missing_vals = self.__find_holes(data_df)       
 
         if interpolate is True:
@@ -1218,9 +1558,54 @@
                 writer = csv.writer(file)
                 # Write rows to the CSV file
                 writer.writerows(interpolated_output)
 
             
         return data_df
     
+    def _plot_single(self,ax,background,gdf, var, cmap=None):
+        "Produce single SVI plot"
+        # plot background
+        background.plot(ax=ax, color='black')
+        
+        # Add gridlines
+        ax.grid(True, which='major', color='grey', linewidth=0.25)
+
+        if cmap is None:
+            # select proper color ramp
+            if gdf[var].max() > 1:
+                cmap = 'coolwarm_r'
+            else:
+                cmap = 'coolwarm'
+
+        else:
+            cmap=cmap
+
+        # plot the figure
+        gdf.plot(ax=ax,
+                    column=var,
+                    cmap=cmap,
+                    scheme='quantiles',
+                    k=10,
+                    edgecolor='black',
+                    linewidth=0.5)
+        
+    def _plot_cmap(self, fig, ax, plot_option):
+        """Plot SVI cmap"""
+        cmap = mpl.cm.coolwarm
+        bounds = np.linspace(0, 1, 10+1)
+        norm = mpl.colors.BoundaryNorm(bounds, cmap.N)
+        labels = ['0','10','20','30','40','50','60','70','80','90','100']
+        if plot_option == 1:
+            cbar = fig.colorbar(mpl.cm.ScalarMappable(norm=norm, cmap=cmap),
+                            cax=ax, orientation='horizontal',
+                            label="Percentile")
+            cbar.ax.set_xticklabels(labels)
+        else:
+            cbar = fig.colorbar(mpl.cm.ScalarMappable(norm=norm, cmap=cmap),
+                            cax=ax, orientation='vertical',
+                            label="Percentile")
+            cbar.ax.set_yticklabels(labels)
+
+
```

### Comparing `svinsight-0.2.8/SVInsight.egg-info/PKG-INFO` & `svinsight-0.3.0/SVInsight.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.1
 Name: SVInsight
-Version: 0.2.8
+Version: 0.3.0
 Summary: Create social vulnerabilty index
 Home-page: https://github.com/mdp0023/SVInsight/
-Author: M. Preisser, P. Passalacqua, R. P. Bixler
+Author: Paola Passalacqua, R. Patrick Bixler
 Author-email: Matthew Preisser <mattpreisser@gmail.com>
-Project-URL: Homepage, https://example.com
-Project-URL: Documentation, https://readthedocs.org
-Keywords: SVI
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python
-Requires-Python: >=3.8
+Project-URL: Homepage, https://github.com/mdp0023/SVInsight
+Project-URL: Documentation, https://mdp0023.github.io/SVInsight/
+Keywords: SVI,Social-Vulnerability,Hazards,Census,Demographics
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: census>=0.8.21
-Requires-Dist: factor_analyzer>=0.5.1
-Requires-Dist: geopandas>=0.14.2
-Requires-Dist: numpy>=1.26.4
-Requires-Dist: pandas>=2.2.2
-Requires-Dist: PyYAML>=6.0.1
-Requires-Dist: scikit_learn>=1.3.0
-Requires-Dist: openpyxl>=3.0.10
+Requires-Dist: census
+Requires-Dist: factor_analyzer
+Requires-Dist: geopandas
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: PyYAML
+Requires-Dist: scikit_learn
+Requires-Dist: openpyxl
+Requires-Dist: matplotlib
```

### Comparing `svinsight-0.2.8/pyproject.toml` & `svinsight-0.3.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,47 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "SVInsight"
-version = "0.2.8"
+version = "0.3.0"
 dependencies = [
-    "census>=0.8.21",
-    "factor_analyzer>=0.5.1",
-    "geopandas>=0.14.2",
-    "numpy>=1.26.4",
-    "pandas>=2.2.2",
-    "PyYAML>=6.0.1",
-    "scikit_learn>=1.3.0",
-    "openpyxl>=3.0.10"
+    "census",
+    "factor_analyzer",
+    "geopandas",
+    "numpy",
+    "pandas",
+    "PyYAML",
+    "scikit_learn",
+    "openpyxl",
+    "matplotlib"
 ]
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 authors = [
   {name = "Matthew Preisser", email = "mattpreisser@gmail.com"},
+  {name = "Paola Passalacqua"},
+  {name = "R. Patrick Bixler"}
+
 ]
 description = "Create social vulnerabilty index"
 readme = "README.rst"
 license = {file = "LICENSE.txt"}
-keywords = ["SVI"]
+keywords = ["SVI",
+            "Social-Vulnerability",
+            "Hazards",
+            "Census",
+            "Demographics"]
 classifiers = [
-  "Development Status :: 3 - Alpha",
-  "Programming Language :: Python"
+  "Development Status :: 4 - Beta",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12"
+
 ]
 
 [project.urls]
-Homepage = "https://example.com"
-Documentation = "https://readthedocs.org"
+Homepage = "https://github.com/mdp0023/SVInsight"
+Documentation = "https://mdp0023.github.io/SVInsight/"
```

### Comparing `svinsight-0.2.8/setup.py` & `svinsight-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from setuptools import setup, find_packages
 #from SVInsight import __version__ as version
 
 setup(
     name='SVInsight',
-    version='0.2.8',
+    version='0.3.0',
     license='MIT',
     description='SVInsight - A python package for calculating an exploratory social vulnerability index',
     author='M. Preisser, P. Passalacqua, R. P. Bixler',
     author_email='mattpreisser@gmail.com',
     url='https://github.com/mdp0023/SVInsight/',
     packages= find_packages(exclude=['*.tests']),
     package_data = {'' : ['*.txt', '*.npz']},
```

### Comparing `svinsight-0.2.8/tests/test_svinsight.py` & `svinsight-0.3.0/tests/test_svinsight.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import sys
-sys.path.append('/Users/matthewpreisser/Documents/Research/Codes/SVInsight')
+sys.path.insert(0, '/Users/matthewpreisser/Documents/Research/Codes/SVInsight')
 
 # import package
 from SVInsight import SVInsight as svi 
 import os
 import pytest
 import geopandas as gpd
 
@@ -45,15 +45,15 @@
             ['12345','48256']]
     for geo in geos:
        assert svi(project_name, file_path, api_key, geo)
 
 
 
 # create a generic test architecture
-def run_svi_workflow(project, boundary, year, overwrite=True):
+def run_svi_workflow(project, boundary, year, overwrite=True, varchange=False):
     # test project instance
     assert project
     # test folder instances
     for loc in ['Boundaries','Variables', 'Data', 'Documentation', 'SVIs']:
         assert os.path.exists(os.path.join(project.file_path, loc))
     
     # Call the function with the test inputs
@@ -74,19 +74,28 @@
 
     # check that the output files exists
     output_file1 = os.path.join(project.data, f"{project.project_name}_{year}_{boundary}_rawdata.csv")
     output_file2 = os.path.join(project.data, f"{project.project_name}_{year}_{boundary}_rawdata.gpkg")
     assert os.path.isfile(output_file1)
     assert os.path.isfile(output_file2)
 
-    # check configure
-    try:
-        project.configure_variables(f"{config}_{year}_{boundary}")
-    except Exception:
-        assert False, "configure_variables execution failed"
+    if varchange is True:
+        # change variables to calculate an economic index
+         # check configure
+        try:
+            project.configure_variables(f"{config}_{year}_{boundary}", include=['MDHSEVAL','PERCAP','QRICH'])
+        except Exception:
+            assert False, "configure_variables execution failed"
+
+    else:
+        # check configure
+        try:
+            project.configure_variables(f"{config}_{year}_{boundary}")
+        except Exception:
+            assert False, "configure_variables execution failed"
 
     # check if output files exist
     output_file3 = os.path.join(project.variables, f"{config}_{year}_{boundary}.yaml")
     assert os.path.isfile(output_file3)
     
     # check svi creation
     try:
@@ -114,55 +123,68 @@
         assert not (svi_test[column] == 0).all(), f"All values in column {column} are 0"
 
 # create fixture of project
 @pytest.fixture
 def project():
     return svi(project_name, file_path, api_key, geoids)
 
+api_key = os.environ.get('API_KEY')
 
-##############################################################################################
-# develop a test project for single county
-project_name = 'test_project_single_county' 
-file_path = os.path.dirname(os.path.realpath(__file__))
-api_key = os.getenv('CENSUS_API_KEY')
-geoids = ['48453']
-boundaries = ['bg', 'tract']
-years = [2015, 2020]
-config='config'
-
-@pytest.mark.parametrize("boundary, year", [(b, y) for b in boundaries for y in years])
-def test_single_county_project(project, boundary, year, overwrite=False):
-    """test creating and running a single county project for different years and boundaries"""
-    run_svi_workflow(project, boundary, year, overwrite=overwrite)
-##############################################################################################
+# ##############################################################################################
+# # develop a test project for single county
+# project_name = 'test_project_single_county' 
+# file_path = os.path.dirname(os.path.realpath(__file__))
+# geoids = ['48453']
+# boundaries = ['bg', 'tract']
+# years = [2015, 2020]
+# config='config'
+
+# @pytest.mark.parametrize("boundary, year", [(b, y) for b in boundaries for y in years])
+# def test_single_county_project(project, boundary, year, overwrite=False):
+#     """test creating and running a single county project for different years and boundaries"""
+#     run_svi_workflow(project, boundary, year, overwrite=overwrite)
+# ##############################################################################################
  
-##############################################################################################
-# develop a test project for multiple counties
-project_name = 'test_project_multiple_counties' 
-file_path = os.path.dirname(os.path.realpath(__file__))
-api_key = os.getenv('CENSUS_API_KEY')
-geoids = ['48453','21117']
-boundaries = ['bg', 'tract']
-years = [2015, 2020]
-config='config'
-
-@pytest.mark.parametrize("boundary, year", [(b, y) for b in boundaries for y in years])
-def test_multiple_county_project(project, boundary, year, overwrite=False):
-    """test creating and running a multiple counties project for different years and boundaries"""
-    run_svi_workflow(project, boundary, year, overwrite=overwrite)
-##############################################################################################
+# ##############################################################################################
+# # develop a test project for multiple counties
+# project_name = 'test_project_multiple_counties' 
+# file_path = os.path.dirname(os.path.realpath(__file__))
+# geoids = ['48453','21117']
+# boundaries = ['bg', 'tract']
+# years = [2015, 2020]
+# config='config'
+
+# @pytest.mark.parametrize("boundary, year", [(b, y) for b in boundaries for y in years])
+# def test_multiple_county_project(project, boundary, year, overwrite=False):
+#     """test creating and running a multiple counties project for different years and boundaries"""
+#     run_svi_workflow(project, boundary, year, overwrite=overwrite)
+# ##############################################################################################
+
+# ##############################################################################################
+# # develop a test project for multiple states
+# project_name = 'test_project_multiple_states' 
+# file_path = os.path.dirname(os.path.realpath(__file__))
+# geoids = ['25','44']
+# boundaries = ['bg', 'tract']
+# years = [2015]
+# config='config'
+
+# @pytest.mark.parametrize("boundary, year", [(b, y) for b in boundaries for y in years])
+# def test_multiple_states_project(project, boundary, year, overwrite=False):
+#     """test creating and running a multiple states project for different years and boundaries"""
+#     run_svi_workflow(project, boundary, year, overwrite=overwrite)
+# ##############################################################################################
 
 ##############################################################################################
-# develop a test project for multiple states
-project_name = 'test_project_multiple_states' 
+# develop a test project for single county, economic index
+project_name = 'test_project_economic_index' 
 file_path = os.path.dirname(os.path.realpath(__file__))
-api_key = os.getenv('CENSUS_API_KEY')
-geoids = ['25','44']
-boundaries = ['bg', 'tract']
-years = [2015]
+geoids = ['48453']
+boundaries = ['bg']
+years = [2017]
 config='config'
 
 @pytest.mark.parametrize("boundary, year", [(b, y) for b in boundaries for y in years])
-def test_multiple_states_project(project, boundary, year, overwrite=False):
+def test_single_county_economic_project(project, boundary, year, overwrite=True):
     """test creating and running a multiple states project for different years and boundaries"""
-    run_svi_workflow(project, boundary, year, overwrite=overwrite)
+    run_svi_workflow(project, boundary, year, overwrite=overwrite, varchange=True)
 ##############################################################################################
```

