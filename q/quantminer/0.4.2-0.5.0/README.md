# Comparing `tmp/quantminer-0.4.2.tar.gz` & `tmp/quantminer-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantminer-0.4.2.tar", last modified: Thu Apr 11 21:17:29 2024, max compression
+gzip compressed data, was "quantminer-0.5.0.tar", last modified: Wed Apr 24 02:41:11 2024, max compression
```

## Comparing `quantminer-0.4.2.tar` & `quantminer-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-11 21:17:29.705021 quantminer-0.4.2/
--rw-r--r--   0 jerryinyang   (501) staff       (20)      167 2024-04-11 21:17:29.704897 quantminer-0.4.2/PKG-INFO
--rw-r--r--   0 jerryinyang   (501) staff       (20)      258 2024-04-10 10:17:30.000000 quantminer-0.4.2/pyproject.toml
-drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-11 21:17:29.703446 quantminer-0.4.2/quantminer/
--rw-r--r--   0 jerryinyang   (501) staff       (20)       34 2024-04-10 11:41:22.000000 quantminer-0.4.2/quantminer/__init__.py
-drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-11 21:17:29.704580 quantminer-0.4.2/quantminer/classes/
--rw-r--r--   0 jerryinyang   (501) staff       (20)       73 2024-04-10 11:38:53.000000 quantminer-0.4.2/quantminer/classes/__init__.py
--rw-r--r--   0 jerryinyang   (501) staff       (20)     2718 2024-04-10 11:32:09.000000 quantminer-0.4.2/quantminer/classes/pivot_pip.py
--rw-r--r--   0 jerryinyang   (501) staff       (20)    13017 2024-04-10 04:48:20.000000 quantminer-0.4.2/quantminer/classes/seqkmeans.py
--rw-r--r--   0 jerryinyang   (501) staff       (20)    22367 2024-04-11 21:16:37.000000 quantminer-0.4.2/quantminer/pipminer.py
-drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-11 21:17:29.704024 quantminer-0.4.2/quantminer.egg-info/
--rw-r--r--   0 jerryinyang   (501) staff       (20)      167 2024-04-11 21:17:29.000000 quantminer-0.4.2/quantminer.egg-info/PKG-INFO
--rw-r--r--   0 jerryinyang   (501) staff       (20)      333 2024-04-11 21:17:29.000000 quantminer-0.4.2/quantminer.egg-info/SOURCES.txt
--rw-r--r--   0 jerryinyang   (501) staff       (20)        1 2024-04-11 21:17:29.000000 quantminer-0.4.2/quantminer.egg-info/dependency_links.txt
--rw-r--r--   0 jerryinyang   (501) staff       (20)       89 2024-04-11 21:17:29.000000 quantminer-0.4.2/quantminer.egg-info/requires.txt
--rw-r--r--   0 jerryinyang   (501) staff       (20)       11 2024-04-11 21:17:29.000000 quantminer-0.4.2/quantminer.egg-info/top_level.txt
--rw-r--r--   0 jerryinyang   (501) staff       (20)       38 2024-04-11 21:17:29.705155 quantminer-0.4.2/setup.cfg
--rw-r--r--   0 jerryinyang   (501) staff       (20)      600 2024-04-11 21:16:43.000000 quantminer-0.4.2/setup.py
+drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-24 02:41:11.717281 quantminer-0.5.0/
+-rw-r--r--   0 jerryinyang   (501) staff       (20)     3868 2024-04-24 02:41:11.717065 quantminer-0.5.0/PKG-INFO
+-rw-r--r--   0 jerryinyang   (501) staff       (20)      258 2024-04-10 10:17:30.000000 quantminer-0.5.0/pyproject.toml
+drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-24 02:41:11.715557 quantminer-0.5.0/quantminer/
+-rw-r--r--   0 jerryinyang   (501) staff       (20)       34 2024-04-10 11:41:22.000000 quantminer-0.5.0/quantminer/__init__.py
+-rw-r--r--   0 jerryinyang   (501) staff       (20)     6014 2024-04-24 01:58:38.000000 quantminer-0.5.0/quantminer/_test_transform.py
+drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-24 02:41:11.716467 quantminer-0.5.0/quantminer/classes/
+-rw-r--r--   0 jerryinyang   (501) staff       (20)      126 2024-04-24 01:07:11.000000 quantminer-0.5.0/quantminer/classes/__init__.py
+-rw-r--r--   0 jerryinyang   (501) staff       (20)    11263 2024-04-24 02:32:15.000000 quantminer-0.5.0/quantminer/classes/reducers.py
+-rw-r--r--   0 jerryinyang   (501) staff       (20)    13017 2024-04-10 04:48:20.000000 quantminer-0.5.0/quantminer/classes/seqkmeans.py
+-rw-r--r--   0 jerryinyang   (501) staff       (20)    24480 2024-04-24 02:36:57.000000 quantminer-0.5.0/quantminer/pipminer.py
+drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-24 02:41:11.716664 quantminer-0.5.0/quantminer.egg-info/
+-rw-r--r--   0 jerryinyang   (501) staff       (20)     3868 2024-04-24 02:41:11.000000 quantminer-0.5.0/quantminer.egg-info/PKG-INFO
+-rw-r--r--   0 jerryinyang   (501) staff       (20)      362 2024-04-24 02:41:11.000000 quantminer-0.5.0/quantminer.egg-info/SOURCES.txt
+-rw-r--r--   0 jerryinyang   (501) staff       (20)        1 2024-04-24 02:41:11.000000 quantminer-0.5.0/quantminer.egg-info/dependency_links.txt
+-rw-r--r--   0 jerryinyang   (501) staff       (20)     1976 2024-04-24 02:41:11.000000 quantminer-0.5.0/quantminer.egg-info/requires.txt
+-rw-r--r--   0 jerryinyang   (501) staff       (20)       11 2024-04-24 02:41:11.000000 quantminer-0.5.0/quantminer.egg-info/top_level.txt
+-rw-r--r--   0 jerryinyang   (501) staff       (20)       38 2024-04-24 02:41:11.717321 quantminer-0.5.0/setup.cfg
+-rw-r--r--   0 jerryinyang   (501) staff       (20)      594 2024-04-24 02:40:58.000000 quantminer-0.5.0/setup.py
```

### Comparing `quantminer-0.4.2/quantminer/classes/seqkmeans.py` & `quantminer-0.5.0/quantminer/classes/seqkmeans.py`

 * *Files identical despite different names*

### Comparing `quantminer-0.4.2/quantminer/pipminer.py` & `quantminer-0.5.0/quantminer/pipminer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,67 +1,84 @@
 import pickle  # noqa
 import warnings
 
+from copy import copy
 from pathlib import Path
 from typing import List, Literal, Optional, Union
 
 import matplotlib.pyplot as plt 
 import numpy as np
 import pandas as pd
 import quantstats as qt
 from kneed import KneeLocator
 from sklearn.cluster import Birch, KMeans
 from sklearn.metrics import silhouette_score
 from sktime.clustering.k_means import TimeSeriesKMeansTslearn 
 
-from .classes import PIP, SeqKMeans
+from .classes import ReducerFFT, ReducerFFTWavelet, ReducerPIP, ReducerWavelet, SeqKMeans
 
 warnings.filterwarnings("ignore", category=RuntimeWarning)
 
 
 class Miner:
     def __init__(self, 
                  n_lookback: int, 
                  n_pivots: int, 
                  n_clusters: int = 8,
                  hold_period: int = 6,
                  model_type:Literal['standard', 'ts', 'sequential']='standard',
-                 verbose = False) -> None:
+                 reducer:Literal['FFT', 'PIP', 'Wavelet', 'FFTWavelet']='PIP',
+                 verbose = False,
+                 wavelet:Literal['db1', 'db2', 'db3', 'db4', 'coif1', 'haar', 'sym5', 'bior3.5']='coif2',
+                 ) -> None:
+            
         self.n_lookback = n_lookback
         self.n_pivots = n_pivots
         self.hold_period = hold_period
         self.n_cluster = n_clusters
 
         self._model_type = model_type
 
         # Store Training Data
         self._data: List = []
+        self._price_data = []
         self._data_train_X: Union[List, np.ndarray] = []
         self._data_train_y: Union[List, np.ndarray] = []
 
         # Store Clusters Assignments
         self._unique_pip_indices : Union[List, np.ndarray]= []
         self._cluster_labels = []
 
         # Store Selected Cluster Labels
         self._cluster_labels_long = []
         self._cluster_labels_short = []
 
         # Store the dimensionality reduction agent
-        self._agent_reduce: PIP = None
+        self._agent_reduce: ReducerPIP = self.__init_reducer(reducer, wavelet=wavelet)
 
         # Store the clustering agent
         self._agent_cluster = None
 
         # Preset attributes
         self._verbose = verbose
         self._random_state = 0
 
 
-    def fit(self, data: np.ndarray):
+    def fit(self, data: np.ndarray, price_data: np.ndarray=None):
+        
+        # Save raw price data for returns computation
+        if price_data is None:
+            price_data = copy(data)
+            
+        if len(price_data) != len(data):
+            raise ValueError(f"Length mismatch: `price_data` is {len(price_data)}, `data` is {len(data)}")
+        
+        # Assign self._price_data
+        self._price_data = self._preprocess_data(price_data, test_mode=True)
+        
         # Set the random state
         np.random.seed(self._random_state)
 
         # Preprocess the training data
         self._preprocess_data(data)
 
         # Create training dataset
@@ -85,21 +102,30 @@
         martins = self._compute_performance()
 
         self.verbose_output("Training Complete : ", martins)
 
         # Clean up stored data
         self._cleanup()
 
-        return martins
+        print(martins)
+
 
+    def test(self, data:np.ndarray, price_data:np.ndarray=None, plot_equity=False):
+        # Save raw price data for returns computation
+        if price_data is None:
+            price_data = copy(data)
+
+        if len(price_data) != len(data):
+            raise ValueError(f"Length mismatch: `price_data` is {len(price_data)}, `data` is {len(data)}")
 
-    def test(self, data: List[np.ndarray], plot_equity=False):
         # Preprocess Data
         data = self._preprocess_data(data, test_mode=True)
-        _returns = np.diff(data, prepend=data[0])
+        price_data = self._preprocess_data(price_data, test_mode=True)
+
+        _returns = np.diff(price_data, prepend=data[0])
 
         # Generate data windows
         windows = self._generate_training_set(data)
 
         # Transform the Data
         _pivots, _unique_indices = self._transform_data(windows)
 
@@ -189,26 +215,26 @@
 
         return signal, list(np.squeeze(_pivots))
 
 
     def save_model(self, path:Union[Path, str]):
         # Convert path to Path object, and check if it exists
         if not isinstance(path, Path):
-            path = Path(str)
+            path = Path(path)
             
             if not path.exists():
                 raise FileNotFoundError(f"File not found: {path}")
             
         # Save model
         with open(path, 'wb') as f:
             try:
                 pickle.dump(self, f)
                 self.verbose_output(f'Model saved at {path}')
-            except Exception as e:
-                raise e
+            except Exception:
+                raise
     
     @staticmethod
     def load_model(path:Union[Path, str]):
         # Convert path to Path object, and check if it exists
         if not isinstance(path, Path):
             path = Path(str)
             
@@ -216,16 +242,16 @@
                 raise FileNotFoundError(f"File not found. Model does not exist at : {path}")
             
         # Save model
         with open(path, 'rb') as f:
             try:
                 miner = pickle.load(f)
                 print(f'OUTPUT : Model Loaded from : {path}')
-            except Exception as e:
-                raise e
+            except Exception:
+                raise
         
         return miner 
 
 
     def apply_holding_period(self, labels, hold_period:Optional[int]=-1, selected_labels:Optional[List]=None):
         """
         Applies a holding period to selected cluster labels, ensuring that consecutive occurrences of the same label are separated by the specified time.
@@ -277,17 +303,19 @@
     def _preprocess_data(self, data, **kwargs):
         """
         Perform series-level data transformations. These can include detrending, denoising/filtering, domain transformations.
         The parameters of these transformations are saved, to be used for new data.
         """
 
         if kwargs.get("test_mode", False):
-            return np.log(data)
+            # return np.sign(data) * np.log1p(np.abs(data))
+            return np.arcsinh(data)
 
-        self._data = np.log(data)
+        # self._data = np.sign(data) * np.log1p(np.abs(data))
+        self._data = np.arcsinh(data)
 
 
     def _generate_training_set(self, data: np.ndarray = None):
         """
         Generate the trainging input (X) and target (y) datasets. When running a test, the `data` parameter is to be processed.
         """
         # Clear stores for training data
@@ -346,19 +374,15 @@
         
         # Ensure the training set has been generated
         if len(data) < 0:
             raise ValueError("No training data to transform")
 
         # Dimensionality Reduction
         if (self._agent_reduce is None):
-            if not test_mode:
-                self._agent_reduce = PIP(n_pivots=self.n_pivots, dist_measure=1)
-            
-            else:
-                raise ValueError("Model has not been training. self._agent_reduce is missing.")
+            raise ValueError("Model has not been training. self._agent_reduce has not been initialized.")
 
         pivots = self._agent_reduce.transform(data)
 
         # Only keep unique patterns
         null_pivots = [-1] * self.n_pivots
 
         # Compare each group with the previous one, excluding the first and last items
@@ -467,21 +491,22 @@
         self._cluster_labels_long.clear()
         self._cluster_labels_short.clear()
 
         # Store the cluster scores from each data
         cluster_scores = []
 
         # Compute the returns
-        _returns = np.diff(self._data, prepend=self._data[0])
+        _returns = np.diff(self._price_data, prepend=self._price_data[0])
 
         # Get the cluster labels
         _labels = self._cluster_labels
 
         # Iterate through each cluster label
         for _label in range(self.n_cluster):
+
             # Create a mask for the label in the labels; everything else should be zero
             mask_label: np.ndarray = _labels == _label
 
             # Filter the labels
             _signals = mask_label.astype(int)
 
             # Implement Holding Period
@@ -497,15 +522,15 @@
 
 
     def _compute_performance(self):
         """
         Test the performance of the selected clusters
         """
 
-        _returns = np.diff(self._data, prepend=self._data[0])
+        _returns = np.diff(self._price_data, prepend=self._price_data[0])
 
         # Get the full labels
         _labels = self._cluster_labels
 
         # Filter for only selected labels
         mask_long = np.isin(_labels, self._cluster_labels_long)
         mask_short = np.isin(_labels, self._cluster_labels_short)
@@ -527,14 +552,15 @@
     def _cleanup(self):
         """
         Clear up memory used to store training data
         """
 
         # Clear Training Data
         self._data = []
+        self._price_data = []
         self._data_train_X = []
         self._data_train_y = []
 
         # Clear Clusters Assignments
         self._unique_pip_indices = []
         self._cluster_labels = []
 
@@ -577,30 +603,30 @@
         return new_signals
 
 
     def __compute_martin(self, rets: np.array):
     
         return qt.stats.ulcer_performance_index(pd.Series(rets))
     
-        rsum = np.sum(rets)
-        short = False
-        if rsum < 0.0:
-            rets *= -1
-            rsum *= -1
-            short = True
-
-        csum = np.cumsum(rets)
-        eq = pd.Series(np.exp(csum))
-        sumsq = np.sum(((eq / eq.cummax()) - 1) ** 2.0)
-        ulcer_index = (sumsq / len(rets)) ** 0.5
-        martin = rsum / (ulcer_index + 1.0e-10)
-        if short:
-            martin = -martin
+        # rsum = np.sum(rets)
+        # short = False
+        # if rsum < 0.0:
+        #     rets *= -1
+        #     rsum *= -1
+        #     short = True
+
+        # csum = np.cumsum(rets)
+        # eq = pd.Series(np.exp(csum))
+        # sumsq = np.sum(((eq / eq.cummax()) - 1) ** 2.0)
+        # ulcer_index = (sumsq / len(rets)) ** 0.5
+        # martin = rsum / (ulcer_index + 1.0e-10)
+        # if short:
+        #     martin = -martin
 
-        return martin
+        # return martin
 
 
     def __find_n_clusters(self):
         # Assuming X is your time series data
         n_clusters = range(2, 50)  # change this range according to your needs
         silhouette_scores = []
         X = self._data_train_X
@@ -671,48 +697,71 @@
             ),
         )
 
         # Show the plot
         fig.show()
 
 
+    def __init_reducer(self, reducer:str, wavelet:str):
+
+        if reducer == 'FFT':
+            return ReducerFFT(n_components=self.n_pivots)
+            
+        elif reducer == 'Wavelet':
+            return ReducerWavelet(n_coefficients=self.n_pivots,
+                                  wavelet=wavelet)
+        
+        elif reducer == 'FFTWavelet':
+            return ReducerFFTWavelet(n_components=self.n_pivots)
+
+        else:
+            return ReducerPIP(n_pivots=self.n_pivots, dist_measure=1)
+
+
     def verbose_output(self, *args):
         if not self._verbose:
             return
         
         for _ in args:
-            print(args)
+            print(_)
 
 
 if __name__ == "__main__":
     parent_path = Path(__file__).parent
     btc_path = parent_path / 'data/BTCUSDT_FULL.parquet'
     
     # Define your date range
     start_date = "2017-12-01"
-    end_date = "2022-12-31"
+    end_date = "2021-12-31"
 
     raw_data = pd.read_parquet(btc_path)
 
     # Filter the DataFrame
     train_data = raw_data[(raw_data.index >= start_date) & (raw_data.index <= end_date)]
     test_data = raw_data[
-        (raw_data.index >= "2023-01-01") & (raw_data.index <= "2023-12-31")
+        (raw_data.index >= "2022-01-01") & (raw_data.index <= "2023-12-31")
     ]
 
     train_data = train_data["close"].dropna(axis=0)
     train_data = train_data.to_numpy()
 
     test_data = test_data["close"].dropna(axis=0)
     test_data = test_data.to_numpy()
 
-    # miner = Miner(25, 5)
+
+    miner = Miner(25, 10, reducer="Wavelet", wavelet='haar')
+
+    # print('Successful')
+    # miner.fit(np.diff(train_data, prepend=train_data[0]-1), train_data)
+    # print(miner.test(np.diff(test_data, prepend=test_data[0]-1), test_data))
+
     # miner.fit(train_data)
+    miner.fit(np.diff(train_data, prepend=train_data[0]-1), train_data)
 
     # miner.save_model(parent_path / 'pipminer.pkl')
 
-    miner : Miner = Miner.load_model(parent_path / 'pipminer.pkl')
+    # miner : Miner = Miner.load_model(parent_path / 'pipminer.pkl')
 
     # print(miner.transform(test_data))
 
-    miner.test(test_data)
-    print('Successful')
+    # print(miner.test(test_data))
+    print(miner.test(np.diff(test_data, prepend=test_data[0]-1), test_data))
```

