# Comparing `tmp/PyGRF-0.0.6.tar.gz` & `tmp/PyGRF-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyGRF-0.0.6.tar", last modified: Sat Apr 20 22:22:18 2024, max compression
+gzip compressed data, was "PyGRF-0.0.7.tar", last modified: Tue Apr 23 23:03:12 2024, max compression
```

## Comparing `PyGRF-0.0.6.tar` & `PyGRF-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 22:22:18.164745 PyGRF-0.0.6/
--rw-rw-rw-   0        0        0     1088 2024-03-16 20:45:00.000000 PyGRF-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     2389 2024-04-20 22:22:18.164745 PyGRF-0.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-20 22:22:18.148730 PyGRF-0.0.6/PyGRF/
--rw-rw-rw-   0        0        0    22877 2024-04-16 22:16:45.000000 PyGRF-0.0.6/PyGRF/PyGRF.py
--rw-rw-rw-   0        0        0      105 2024-03-17 01:02:06.000000 PyGRF-0.0.6/PyGRF/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-20 22:22:18.164745 PyGRF-0.0.6/PyGRF.egg-info/
--rw-rw-rw-   0        0        0     2389 2024-04-20 22:22:18.000000 PyGRF-0.0.6/PyGRF.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2024-04-20 22:22:18.000000 PyGRF-0.0.6/PyGRF.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 22:22:18.000000 PyGRF-0.0.6/PyGRF.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-04-20 22:22:18.000000 PyGRF-0.0.6/PyGRF.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-20 22:22:18.000000 PyGRF-0.0.6/PyGRF.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1491 2024-04-20 22:11:20.000000 PyGRF-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2024-04-20 22:22:18.164745 PyGRF-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     2993 2024-04-20 22:22:07.000000 PyGRF-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 23:03:12.208246 PyGRF-0.0.7/
+-rw-rw-rw-   0        0        0     1088 2024-03-16 20:45:00.000000 PyGRF-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     2389 2024-04-23 23:03:12.208246 PyGRF-0.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-23 23:03:12.192627 PyGRF-0.0.7/PyGRF/
+-rw-rw-rw-   0        0        0    22891 2024-04-23 22:57:30.000000 PyGRF-0.0.7/PyGRF/PyGRF.py
+-rw-rw-rw-   0        0        0      105 2024-03-17 01:02:06.000000 PyGRF-0.0.7/PyGRF/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 23:03:12.208246 PyGRF-0.0.7/PyGRF.egg-info/
+-rw-rw-rw-   0        0        0     2389 2024-04-23 23:03:12.000000 PyGRF-0.0.7/PyGRF.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2024-04-23 23:03:12.000000 PyGRF-0.0.7/PyGRF.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 23:03:12.000000 PyGRF-0.0.7/PyGRF.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-04-23 23:03:12.000000 PyGRF-0.0.7/PyGRF.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-23 23:03:12.000000 PyGRF-0.0.7/PyGRF.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1491 2024-04-20 22:11:20.000000 PyGRF-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-23 23:03:12.208246 PyGRF-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     2993 2024-04-23 23:02:09.000000 PyGRF-0.0.7/setup.py
```

### Comparing `PyGRF-0.0.6/LICENSE` & `PyGRF-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `PyGRF-0.0.6/PKG-INFO` & `PyGRF-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyGRF
-Version: 0.0.6
+Version: 0.0.7
 Summary: PyGRF: An improved Python Geographical Random Forest model.
 Home-page: https://github.com/geoai-lab/PyGRF
 Author: Kai Sun, Ryan Zhenqi Zhou, Jiyeon Kim, and Yingjie Hu
 Author-email: ksun4@buffalo.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `PyGRF-0.0.6/PyGRF/PyGRF.py` & `PyGRF-0.0.7/PyGRF/PyGRF.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,31 +35,31 @@
     n_jobs: int, default=None
         The number of jobs to execute in parallel.
         More details please refer to the documentation of scikit-learn at the link: https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestRegressor.html
     bootstrap: bool, default = True
         Whether each tree is built using bootstrap sampling (with replacement) from the original dataset. If False, each tree is built using the entire dataset.
         Note that this parameter should be true if out of bag (OOB) predictions are needed.
         More details please refer to the documentation of scikit-learn at the link: https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestRegressor.html.
-    random_seed: int, instance of Numpy RandomState or None, default=None
+    random_state: int, instance of Numpy RandomState or None, default=None
         Determine the randomness within the model fitting. This parameter has to be fixed in order to achieve reproducibility in the model fitting process.
         More details please refer to the documentation of scikit-learn at the link: https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestRegressor.html.
     """
 
     def __init__(self, band_width, n_estimators=100, max_features=1.0, kernel="adaptive", train_weighted=True, predict_weighted=True,
-                 resampled=True, n_jobs=None, bootstrap=True, random_seed=None):
+                 resampled=True, n_jobs=None, bootstrap=True, random_state=None):
         self.n_estimators = n_estimators
         self.max_features = max_features
         self.band_width = band_width
         self.kernel = kernel
         self.train_weighted = train_weighted
         self.predict_weighted = predict_weighted
         self.n_jobs = n_jobs
         self.bootstrap = bootstrap
         self.resampled = resampled
-        self.random_seed = random_seed
+        self.random_state = random_state
         self.global_model = None
         self.local_models = None
         self.train_data_coords = None
         self.distance_matrix = None
         self.train_data_columns = None
 
     def fit(self, X_train, y_train, coords):
@@ -86,19 +86,19 @@
         # save the columns of the training data
         self.train_data_columns = X_train.columns.tolist()
 
         # fit and save the global model, and get the OOB predictions from the global model if bootstrap is True
         if self.bootstrap:
             rf_global = RandomForestRegressor(bootstrap=self.bootstrap, oob_score=True, n_estimators=self.n_estimators,
                                               max_features=self.max_features, n_jobs=self.n_jobs,
-                                              random_state=self.random_seed)
+                                              random_state=self.random_state)
         else:
             rf_global = RandomForestRegressor(bootstrap=self.bootstrap, n_estimators=self.n_estimators,
                                               max_features=self.max_features, n_jobs=self.n_jobs,
-                                              random_state=self.random_seed)
+                                              random_state=self.random_state)
         rf_global.fit(X_train, y_train)
         self.global_model = rf_global
         if self.bootstrap:
             global_oob_prediction = rf_global.oob_prediction_
 
         # create an empty list for saving local models
         self.local_models = []
@@ -141,45 +141,45 @@
             # the independent and dependent variables of samples for training local models
             local_X_train = X_train.iloc[idx]
             local_y_train = y_train.iloc[idx]
 
             # build a local model
             if self.bootstrap:
                 rf_local = RandomForestRegressor(bootstrap=self.bootstrap, oob_score=True, n_estimators=self.n_estimators,
-                                                 max_features=self.max_features, n_jobs=self.n_jobs, random_state=self.random_seed)
+                                                 max_features=self.max_features, n_jobs=self.n_jobs, random_state=self.random_state)
             else:
                 rf_local = RandomForestRegressor(bootstrap=self.bootstrap,
                                                  n_estimators=self.n_estimators,
-                                                 max_features=self.max_features, n_jobs=self.n_jobs, random_state=self.random_seed)
+                                                 max_features=self.max_features, n_jobs=self.n_jobs, random_state=self.random_state)
 
             # fit a local model using local trianing data, which may be expanded with replacement
             if self.train_weighted:
                 if self.resampled and len(local_X_train) < 2 * self.n_estimators:
                     resampled_length = min(2 * self.n_estimators, 2*len(local_X_train)) - len(local_X_train)
                     more_X_train_resampled, more_y_train_resampled, more_sample_weights_resampled = resample(
                         local_X_train,
                         local_y_train,
                         sample_weights,
                         replace=True,
                         n_samples=resampled_length,
-                        random_state=self.random_seed)
+                        random_state=self.random_state)
                     local_X_train_resampled = pd.concat([local_X_train, more_X_train_resampled], ignore_index=True)
                     local_y_train_resampled = pd.concat([local_y_train, more_y_train_resampled], ignore_index=True)
                     sample_weights_resampled = np.concatenate((sample_weights, more_sample_weights_resampled))
                     rf_local.fit(local_X_train_resampled, local_y_train_resampled, sample_weights_resampled)
                 else:
                     rf_local.fit(local_X_train, local_y_train, sample_weights)
             else:
                 if self.resampled and len(local_X_train) < 2 * self.n_estimators:
                     resampled_length = min(2 * self.n_estimators, 2*len(local_X_train)) - len(local_X_train)
                     more_X_train_resampled, more_y_train_resampled = resample(local_X_train,
                                                                               local_y_train,
                                                                               replace=True,
                                                                               n_samples=resampled_length,
-                                                                              random_state=self.random_seed)
+                                                                              random_state=self.random_state)
                     local_X_train_resampled = pd.concat([local_X_train, more_X_train_resampled], ignore_index=True)
                     local_y_train_resampled = pd.concat([local_y_train, more_y_train_resampled], ignore_index=True)
                     rf_local.fit(local_X_train_resampled, local_y_train_resampled)
                 else:
                     rf_local.fit(local_X_train, local_y_train)
 
             # get the local OOB prediction for the current sample
@@ -366,15 +366,15 @@
     found_bandwidth, found_moran_I, found_p_value = bandwidth_list[max_index], moran_I_list[max_index], p_value_list[max_index]
     print("bandwidth: {}, moran's I: {}, p-value: {}".format(found_bandwidth, found_moran_I, found_p_value))
 
     return found_bandwidth, found_moran_I, found_p_value
 
 
 def search_bandwidth(X, y, coords, n_estimators, max_features, bw_min=None, bw_max=None, step=1, train_weighted=True, resampled=True, n_jobs=None,
-                     random_seed=None):
+                     random_state=None):
     """
     Optimize the bandwidth using OOB score
 
     Parameters
     ----------
     X: data frame
         A data frame of independent variables of samples in the data used for searching the optimal bandwidth.
@@ -394,15 +394,15 @@
         The step for iterating the band_width between minimum and maximum values.
     train_weighted: bool, default = True
         Whether samples are weighted based on distances in the PyGRF model.
     resampled: bool, default = True
         Whether local samples are expanded in the PyGRF model.
     n_jobs: int, default=None
         The number of jobs to execute in parallel.
-    random_seed: int, instance of Numpy RandomState or None, default=None
+    random_state: int, instance of Numpy RandomState or None, default=None
         Determine the randomness within the PyGRF model fitting.
 
     Returns
     -------
     search_result: dictionary
         The result of searching the optimal band_width
     """
@@ -423,15 +423,15 @@
     df_search_bw = pd.DataFrame(columns=['bandwidth', 'mixed'])
 
     # iterate each band_width between minimum and maximum values
     for current_bw in range(bw_min, bw_max + 1, step):
         band_width_list.append(current_bw)
 
         # fit PyGRF model using the test bandwidth and get the OOB predictions
-        grf = PyGRFBuilder(n_estimators=n_estimators, max_features=max_features, band_width=current_bw, random_seed=random_seed,
+        grf = PyGRFBuilder(n_estimators=n_estimators, max_features=max_features, band_width=current_bw, random_state=random_state,
                     train_weighted=train_weighted)
         y_oob_local, y_oob_global = grf.fit(X, y, coords)
 
         # compute R-squred scores using local OOB predictions and global OOB predictions
         # r_oob_local = r2_score(y, y_oob_local)
         # local_list.append(r_oob_local)
         y_oob_mixed = (np.array(y_oob_local) + np.array(y_oob_global)) / 2
```

### Comparing `PyGRF-0.0.6/PyGRF.egg-info/PKG-INFO` & `PyGRF-0.0.7/PyGRF.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyGRF
-Version: 0.0.6
+Version: 0.0.7
 Summary: PyGRF: An improved Python Geographical Random Forest model.
 Home-page: https://github.com/geoai-lab/PyGRF
 Author: Kai Sun, Ryan Zhenqi Zhou, Jiyeon Kim, and Yingjie Hu
 Author-email: ksun4@buffalo.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `PyGRF-0.0.6/README.md` & `PyGRF-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `PyGRF-0.0.6/setup.py` & `PyGRF-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Package meta-data.
 NAME = 'PyGRF'
 DESCRIPTION = 'PyGRF: An improved Python Geographical Random Forest model.'
 URL = 'https://github.com/geoai-lab/PyGRF'
 EMAIL = 'ksun4@buffalo.edu'
 AUTHOR = 'Kai Sun, Ryan Zhenqi Zhou, Jiyeon Kim, and Yingjie Hu'
 REQUIRES_PYTHON = '>=3.8.0'
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 
 # Packages are required for this module to be executed.
 REQUIRED = [
     'pandas', 'numpy', 'scikit-learn', 'scipy', 'libpysal', 'esda'
 ]
 
 here = os.path.abspath(os.path.dirname(__file__))
```

