# Comparing `tmp/survival_data_handler-2024.1.1.tar.gz` & `tmp/survival_data_handler-2024.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "survival_data_handler-2024.1.1.tar", last modified: Tue Apr 16 09:21:21 2024, max compression
+gzip compressed data, was "survival_data_handler-2024.1.2.tar", last modified: Wed Apr 24 07:09:56 2024, max compression
```

## Comparing `survival_data_handler-2024.1.1.tar` & `survival_data_handler-2024.1.2.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:21:21.476953 survival_data_handler-2024.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-16 09:21:15.000000 survival_data_handler-2024.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-16 09:21:21.476953 survival_data_handler-2024.1.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     1892 2024-04-16 09:21:15.000000 survival_data_handler-2024.1.1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      363 2024-04-16 09:21:15.000000 survival_data_handler-2024.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-16 09:21:15.000000 survival_data_handler-2024.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 09:21:21.476953 survival_data_handler-2024.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:21:21.472953 survival_data_handler-2024.1.1/survival_data_handler/
--rwxr-xr-x   0 runner    (1001) docker     (127)      835 2024-04-16 09:21:15.000000 survival_data_handler-2024.1.1/survival_data_handler/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7236 2024-04-16 09:21:15.000000 survival_data_handler-2024.1.1/survival_data_handler/analysis.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23493 2024-04-16 09:21:15.000000 survival_data_handler-2024.1.1/survival_data_handler/main.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5569 2024-04-16 09:21:15.000000 survival_data_handler-2024.1.1/survival_data_handler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:21:21.476953 survival_data_handler-2024.1.1/survival_data_handler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-16 09:21:21.000000 survival_data_handler-2024.1.1/survival_data_handler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-16 09:21:21.000000 survival_data_handler-2024.1.1/survival_data_handler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 09:21:21.000000 survival_data_handler-2024.1.1/survival_data_handler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-16 09:21:21.000000 survival_data_handler-2024.1.1/survival_data_handler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 09:21:21.000000 survival_data_handler-2024.1.1/survival_data_handler.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:21:21.476953 survival_data_handler-2024.1.1/test/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1946 2024-04-16 09:21:15.000000 survival_data_handler-2024.1.1/test/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:09:56.259169 survival_data_handler-2024.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-24 07:09:49.000000 survival_data_handler-2024.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-24 07:09:56.259169 survival_data_handler-2024.1.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2108 2024-04-24 07:09:49.000000 survival_data_handler-2024.1.2/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-04-24 07:09:49.000000 survival_data_handler-2024.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-24 07:09:49.000000 survival_data_handler-2024.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 07:09:56.259169 survival_data_handler-2024.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:09:56.259169 survival_data_handler-2024.1.2/survival_data_handler/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      835 2024-04-24 07:09:49.000000 survival_data_handler-2024.1.2/survival_data_handler/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7236 2024-04-24 07:09:49.000000 survival_data_handler-2024.1.2/survival_data_handler/analysis.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21703 2024-04-24 07:09:49.000000 survival_data_handler-2024.1.2/survival_data_handler/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-04-24 07:09:49.000000 survival_data_handler-2024.1.2/survival_data_handler/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8297 2024-04-24 07:09:49.000000 survival_data_handler-2024.1.2/survival_data_handler/plotting.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5586 2024-04-24 07:09:49.000000 survival_data_handler-2024.1.2/survival_data_handler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:09:56.259169 survival_data_handler-2024.1.2/survival_data_handler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-24 07:09:56.000000 survival_data_handler-2024.1.2/survival_data_handler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-24 07:09:56.000000 survival_data_handler-2024.1.2/survival_data_handler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 07:09:56.000000 survival_data_handler-2024.1.2/survival_data_handler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-24 07:09:56.000000 survival_data_handler-2024.1.2/survival_data_handler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 07:09:56.000000 survival_data_handler-2024.1.2/survival_data_handler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:09:56.259169 survival_data_handler-2024.1.2/test/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2868 2024-04-24 07:09:49.000000 survival_data_handler-2024.1.2/test/test_main.py
```

### Comparing `survival_data_handler-2024.1.1/LICENSE` & `survival_data_handler-2024.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `survival_data_handler-2024.1.1/PKG-INFO` & `survival_data_handler-2024.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: survival_data_handler
-Version: 2024.1.1
+Version: 2024.1.2
 Author-email: Vincent Laurent <vlaurent@eurobios.com>
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib>=3
 Requires-Dist: seaborn
 Requires-Dist: numba
 Requires-Dist: scipy
 Requires-Dist: scikit-learn
-Requires-Dist: pandas
+Requires-Dist: pandas>2
 Requires-Dist: lifelines
 
 # Survival data handler
+![code coverage](https://raw.githubusercontent.com/eurobios-mews-labs/survival-data-handler/coverage-badge/coverage.svg?raw=true)
+[![PyPI version](https://badge.fury.io/py/palma.svg)](https://badge.fury.io/py/palma)
 
 ```python
 import pandas as pd
 
 from lifelines import CoxPHFitter
 from lifelines.datasets import load_rossi
```

### Comparing `survival_data_handler-2024.1.1/README.md` & `survival_data_handler-2024.1.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # Survival data handler
+![code coverage](https://raw.githubusercontent.com/eurobios-mews-labs/survival-data-handler/coverage-badge/coverage.svg?raw=true)
+[![PyPI version](https://badge.fury.io/py/palma.svg)](https://badge.fury.io/py/palma)
 
 ```python
 import pandas as pd
 
 from lifelines import CoxPHFitter
 from lifelines.datasets import load_rossi
```

### Comparing `survival_data_handler-2024.1.1/survival_data_handler/__init__.py` & `survival_data_handler-2024.1.2/survival_data_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `survival_data_handler-2024.1.1/survival_data_handler/analysis.py` & `survival_data_handler-2024.1.2/survival_data_handler/analysis.py`

 * *Files identical despite different names*

### Comparing `survival_data_handler-2024.1.1/survival_data_handler/main.py` & `survival_data_handler-2024.1.2/survival_data_handler/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,64 +6,76 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import typing
-from typing import Callable, Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sns
-from numba import njit
 from scipy.interpolate import interp1d
 from sklearn import metrics
 
 from survival_data_handler.utils import process_survival_function, \
     compute_derivative, residual_life, shift_from_interp
+from survival_data_handler import plotting
+
+
+class TimeCurve:
+    def __init__(self, df, name):
+        self.__data = df
+        self.__name = name
+
+    @property
+    def data(self) -> pd.DataFrame:
+        return self.__data
+
 
 # ======================================================================================================================
 # AESTHETICS
 cmap = sns.color_palette('rainbow', as_cmap=True)
 event_censored_color = cmap(0.1)
 event_observed_color = cmap(0.95)
 
 
 class Lifespan:
+    __index = "origin_index"
 
     # ==============================================
     #           CLASS METHOD
     # ==============================================
 
     def __init__(self,
                  ageing_curves: pd.DataFrame,
                  index: iter,
                  age: iter,
                  birth: iter,
                  window: tuple,
                  risks: tuple = (0.96, 0.98),
                  default_precision="float"):
 
-        self.df_curves = ageing_curves
+        self.__curves = ageing_curves.__deepcopy__()
         self.df_idx = pd.DataFrame(
             dict(age=age,
                  birth=birth,
                  index=index))
-        self._index = "origin_index"
-        self.df_idx.index.name = self._index
+
+        self.df_idx.index.name = self.__index
         self.index = index
         self.age = age
         self.window = window
         self.__p = default_precision
 
-        df_curves = self.df_curves.T
+        self.__check_args()
+
         self.survival_estimation = SurvivalEstimation(
-            df_curves, unit='D',
+            self.curves, unit='D',
             n_unit=365.25)
 
         self._df_idx_unique = self.df_idx.drop_duplicates(
             subset=["index", "birth"])
         self.starting_dates = self._df_idx_unique["birth"]
 
         self.risk_level = risks
@@ -75,14 +87,19 @@
             suffixes=("_u", ""))
 
         self._corresp = self._corresp.drop(columns=c)
         self.confusion_matrix_threshold = np.nan
         self.__computed = []
         self.__supervised = False
 
+    def __check_args(self):
+
+        if hasattr(self.curves.columns, "dt"):
+            ValueError("curves index must have dt property")
+
     @property
     def computed_historical_data(self):
         return self.__computed
 
     @property
     def supervised(self):
         return self.__supervised
@@ -106,44 +123,49 @@
             return ret.loc[index], self.event.loc[index], self.durations.loc[
                 index], entry
 
     def _shift_helper(self, data: typing.Union[pd.DataFrame, pd.Series]):
         data = pd.merge(self._df_idx_unique["index"].reset_index(), data,
                         right_index=True,
                         left_on='index')
-        data = data.set_index(self._index).drop("index", axis=1)
+        data = data.set_index(self.__index).drop("index", axis=1)
         ret = shift_from_interp(
             data=data,
             starting_dates=self.starting_dates,
             period=pd.to_timedelta(30, unit="d"),
             date_initial=self.window[0], date_final=self.window[1],
             dtypes=self.__p
         )
         return ret
 
     # ==============================================
     #           ENRICH REPRESENTATION
     # ==============================================
+    @property
+    def survival_function(self) -> pd.DataFrame:
+        if "survival_function" not in self.__computed:
+            self.compute_survival()
+        return self.__survival_function
 
     def compute_expected_residual_life(self) -> None:
         data = pd.Series(self.survival_estimation.residual_life_interp)
         data.name = "interp"
         data = self._shift_helper(data)
         self.residual_lifespan = self._decompose_unique(data)[0].astype(
             self.__p)
         self.__computed.append("residual_lifespan")
 
     def compute_survival(self):
         data = pd.Series(self.survival_estimation.survival_interp)
         data.name = "interp"
         data = self._shift_helper(data)
-        self.survival_function = self._decompose_unique(data)[0].astype(
+        self.__survival_function = self._decompose_unique(data)[0].astype(
             self.__p)
-        self.survival_function[self.survival_function > 1] = np.nan
-        self.survival_function[self.survival_function < 0] = 0
+        self.__survival_function[self.__survival_function > 1] = np.nan
+        self.__survival_function[self.__survival_function < 0] = 0
         self.__computed.append("survival_function")
 
     def compute_residual_survival(self, t0) -> None:
         assert "survival_function" in self.computed_historical_data
 
         t0 = max(t0, self.survival_function.columns[0])
         s0 = get(self.survival_function, t0).astype("float16").values
@@ -250,15 +272,15 @@
         return df_matrix
 
     # ==============================================
     #           PLOTS CURVES
     # ==============================================
     def plot_curves(self):
         plt.figure(dpi=200, figsize=(7, 5))
-        self.df_curves.T.plot(legend=False)
+        self.curves.plot(legend=False)
 
     def plot_curves_residual_life(self, **kwargs):
         self.survival_estimation.plot_residual_life(**kwargs)
         plt.ylabel("Expected residual lifespan")
         plt.xlabel("Time [Y]")
 
     def plot_cumulated_times(self):
@@ -365,15 +387,15 @@
               )
         plt.legend()
 
     def plot_tagged_sample(
             self, data: pd.DataFrame, n_sample=None,
             n_sample_pos=None, n_sample_neg=None,
     ):
-        from survival_trees import plotting
+
         assert self.__supervised, "No supervision provided"
         corresp, event, duration, entry = self._decompose_unique(data,
                                                                  get_supervision=True)
         if n_sample is None and n_sample_neg is None and n_sample_pos is None:
             sample = corresp
         elif n_sample_pos is None and n_sample_neg is None:
             sample = corresp.sample(n_sample)
@@ -393,15 +415,14 @@
             event_observed_color=event_observed_color,
             add_marker=True,
         )
         return index
 
     def plotly_auc_vs_score(self, temporal_scores: pd.DataFrame,
                             temporal_metric: pd.Series, **kwargs):
-        from survival_trees import plotting
         corresp, event, duration, entry = self._decompose_unique(
             temporal_scores, get_supervision=True)
         time_start, time_stop = duration.min(), duration.max()
         corresp = corresp[
             [c for c in corresp.columns if time_start <= c <= time_stop]]
         return plotting.auc_vs_score_plotly(temporal_scores=corresp,
                                             event_observed=event,
@@ -409,38 +430,44 @@
                                             entry_time=entry,
                                             temporal_metric=temporal_metric,
                                             **kwargs)
 
     @staticmethod
     def plotly_roc_curve(roc: dict, colormap="magma_r", template="plotly_white",
                          **kwargs):
-        from survival_trees import plotting
         return plotting.plot_roc_curve_plotly(roc, colormap=colormap,
                                               template=template, **kwargs)
 
     # ==============================================
     #           METRIC ASSESSMENT
     # ==============================================
     def assess_metric(self, data, method="roc-cd",
                       metric=metrics.roc_auc_score):
-        from survival_trees import metric as m
+
         corresp, event, duration, _ = self._decompose_unique(data,
                                                              get_supervision=True)
 
         time_start, time_stop = duration.min(), duration.max()
         corresp = corresp[
             [c for c in corresp.columns if time_start <= c <= time_stop]]
-        return m.time_dependent_helper(
+        return metric.time_dependent_helper(
             corresp,
             event_observed=event,
             censoring_time=duration,
             method=method,
             function=metric
         )
 
+    # ==============================================
+    #           Properties
+    # ==============================================
+    @property
+    def curves(self) -> pd.DataFrame:
+        return self.__curves
+
 
 def get(data: pd.DataFrame, date):
     search = np.searchsorted(data.columns.to_list(), date)
     return data.iloc[:, search]
 
 
 class SurvivalEstimation:
@@ -452,17 +479,19 @@
                  survival_curves: pd.DataFrame,
                  unit='D', n_unit=1.,
                  process_input_data=True):
 
         survival_curves = survival_curves.__deepcopy__()
         if process_input_data:
             survival_curves = process_survival_function(survival_curves)
+
         self.survival = survival_curves
+        self.__check_args()
 
-        self.times = self.survival.index.to_numpy()
+        self.times = self.survival.columns.to_numpy()
         self.unit = pd.to_timedelta(n_unit, unit=unit).total_seconds()
 
         self.derivative = compute_derivative(self.survival, self.unit)
         self.hazard = - self.derivative / self.survival
         self.cumulative_hazard = - np.log(self.survival)
 
         self.__survival = self.survival.__deepcopy__()
@@ -471,32 +500,32 @@
         self.residual_life = residual_life(self.__survival)
         self.residual_life.columns = self.survival.columns
         self.residual_life[
             self.residual_life > 1e5] = self.residual_life.columns.max()
         self.residual_survival = None
         # CREATE INTERPOLATION
         self.hazard_interp = {
-            c: interp1d(self.hazard.index.astype(int),
-                        self.hazard[c], fill_value="extrapolate") for c in
-            self.hazard.columns
+            c: interp1d(self.hazard.columns.astype(int),
+                        self.hazard.loc[c], fill_value="extrapolate") for c in
+            self.hazard.index
         }
         self.survival_interp = {
-            c: interp1d(self.survival.index.astype(int),
-                        self.survival[c], fill_value="extrapolate") for c in
-            self.survival.columns
+            c: interp1d(self.survival.columns.astype(int),
+                        self.survival.loc[c], fill_value="extrapolate") for c in
+            self.survival.index
         }
         self.cumulative_hazard_interp = {
-            c: interp1d(self.cumulative_hazard.index.astype(int),
-                        self.cumulative_hazard[c], fill_value="extrapolate") for
-            c in self.cumulative_hazard.columns
+            c: interp1d(self.cumulative_hazard.columns.astype(int),
+                        self.cumulative_hazard.loc[c], fill_value="extrapolate") for
+            c in self.cumulative_hazard.index
         }
         self.residual_life_interp = {
-            c: interp1d(self.residual_life.T.index.astype(int),
-                        self.residual_life.T[c], fill_value="extrapolate") for
-            c in self.residual_life.T.columns
+            c: interp1d(self.residual_life.columns.astype(int),
+                        self.residual_life.loc[c], fill_value="extrapolate") for
+            c in self.residual_life.index
         }
 
     def plot_residual_life(self, sample=None, mean_behaviour=True):
         if not mean_behaviour:
             if sample is not None:
                 residual_life_ = self.residual_life.sample(sample)
             else:
@@ -526,93 +555,10 @@
                                      des.iloc[i - 1], alpha=0.2, facecolor=c)
 
             plt.grid()
             plt.legend()
             plt.ylabel("Expected residual lifespan")
             plt.xlabel("Time")
 
-
-@njit
-def find_date(s: np.array, s_dates: np.array, columns: np.array,
-              datetime: np.array, values: np.array):
-    ret = {}
-    for d in s:
-        loc = s_dates == d
-        idx_start = np.argmin(np.abs((columns - d)))
-        t0 = (columns - d)[0]
-        select_column_input = np.array(datetime > t0)
-        idx_stop = idx_start + sum(select_column_input) - 1
-        if idx_start == -1:
-            continue
-
-        select_col = columns[idx_start:idx_stop]
-        n_cols = len(select_col)
-        v = values[loc][:, select_column_input][:, :n_cols]
-
-        ret[t0] = loc, select_col, v
-    return ret
-
-
-def score(t_true: iter, t_pred: iter, observed: iter, score_function: callable):
-    times = np.sort(np.unique(t_true))
-    assert t_true.__len__() == t_pred.__len__(), TypeError(
-        "The number of observation in prediction "
-        "and ground truth does not correspond")
-    ret = pd.Series(index=times)
-    for t in times:
-        y_true = (t_true > t) & observed
-        y_pred = t_pred.loc[t]
-        ret.loc[t] = score_function(y_true, y_pred)
-    return ret
-
-
-class Search:
-
-    def __init__(self, fun):
-        self.fun = fun
-
-    @njit
-    def __call__(self, support):
-        fun = self.fun
-        if len(support) == 1:
-            return support[0]
-        m = len(support) // 2
-        left = fun(support[0])
-        right = fun(support[-1])
-        middle = fun(support[m])
-        if left >= middle >= right:
-            return self(support[:m])
-        elif left <= middle <= right:
-            return self(support[m:])
-        else:
-            return max(self(fun, support[m:]), self(support[:m]))
-
-
-def find_threshold(y_true: np.ndarray, y_pred: np.ndarray,
-                   target_metric: Union[Callable, str],
-                   score: bool):
-    """
-    Given true and predicted values, compute decision rule's threshold which
-    optimizes the target metric
-    """
-    n = 100000
-    if isinstance(target_metric, str):
-        target_metric = getattr(metrics, target_metric)
-    threshold = np.sort(np.unique(y_pred))
-
-    if len(y_pred) > n:
-        choice = np.random.choice(range(0, len(y_pred)), size=n)
-    else:
-        choice = range(len(y_pred))
-
-    sign = 1 if score else -1
-
-    def compute_metric(th):
-        return sign * target_metric(
-            np.array(y_true)[choice],
-            np.array(y_pred)[choice] > th)
-
-    return Search(compute_metric)(threshold)
-
-
-def date_to_year(date):
-    return date.value / 1e9 / 60 / 60 / 24 / 365.25 + 1970
+    def __check_args(self):
+        if hasattr(self.survival.columns, "dt"):
+            ValueError("curves index must have dt property")
```

### Comparing `survival_data_handler-2024.1.1/survival_data_handler/utils.py` & `survival_data_handler-2024.1.2/survival_data_handler/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,29 +96,28 @@
 
        References:
        - doi:10.1016/j.jspi.2004.06.012
     """
     deltas = np.diff(survival_estimate.columns.values)
 
     # days = deltas.astype('timedelta64[D]').astype(int) / 365.25
-    dt = np.ones((len(survival_estimate), 1), dtype=precision) * deltas.reshape(
+    dt = 1.*np.ones((len(survival_estimate), 1), dtype=precision) * deltas.reshape(
         1, -1)
 
-    surv_int = survival_estimate.__deepcopy__()
+    surv_int = survival_estimate.__deepcopy__().astype(float)
 
-    s_left = survival_estimate.iloc[:, 1:].values
-    s_right = survival_estimate.iloc[:, :-1].values
+    s_left = survival_estimate.iloc[:, 1:].values.astype(float)
+    s_right = survival_estimate.iloc[:, :-1].values.astype(float)
 
-    surv_int.iloc[:, :-1] = (s_left + s_right) / 2
+    surv_int.iloc[:, :-1] = (s_left + s_right) / 2.
     surv_int.iloc[:, :-1] *= dt
 
     surv_int = surv_int[np.sort(surv_int.columns)[::-1]].cumsum(axis=1)
     ret = (surv_int / survival_estimate).astype(precision)
     ret[survival_estimate == 0] = 0
-    del surv_int, dt, deltas
     return ret - survival_estimate.columns[0]
 
 
 class _PoolShift:
     def __init__(self, dates, starting_dates, data):
         self.dates = dates
         self.starting_dates = starting_dates.values
```

### Comparing `survival_data_handler-2024.1.1/survival_data_handler.egg-info/PKG-INFO` & `survival_data_handler-2024.1.2/survival_data_handler.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: survival_data_handler
-Version: 2024.1.1
+Version: 2024.1.2
 Author-email: Vincent Laurent <vlaurent@eurobios.com>
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib>=3
 Requires-Dist: seaborn
 Requires-Dist: numba
 Requires-Dist: scipy
 Requires-Dist: scikit-learn
-Requires-Dist: pandas
+Requires-Dist: pandas>2
 Requires-Dist: lifelines
 
 # Survival data handler
+![code coverage](https://raw.githubusercontent.com/eurobios-mews-labs/survival-data-handler/coverage-badge/coverage.svg?raw=true)
+[![PyPI version](https://badge.fury.io/py/palma.svg)](https://badge.fury.io/py/palma)
 
 ```python
 import pandas as pd
 
 from lifelines import CoxPHFitter
 from lifelines.datasets import load_rossi
```

### Comparing `survival_data_handler-2024.1.1/test/test_main.py` & `survival_data_handler-2024.1.2/test/test_main.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 import pandas as pd
 import pytest
 from lifelines import CoxPHFitter
 from lifelines.datasets import load_rossi
 
-from survival_data_handler.main import SurvivalEstimation
+from survival_data_handler.main import SurvivalEstimation, Lifespan
 from survival_data_handler.utils import smooth, process_survival_function, \
     compute_derivative
 
 
 @pytest.fixture()
 def data():
     rossi = load_rossi()
@@ -54,11 +54,43 @@
 
 def test_survival_estimation(data):
     _, curves = data
     se = SurvivalEstimation(
         curves.drop_duplicates(), unit='D',
         n_unit=365.25)
     se.plot_residual_life()
+    # se.plot_residual_life(mean_behaviour=False)
+
+
+def test_survival_estimation_attributes(data):
+    rossi, curves = data
+
+    rossi["index"] = rossi.index
+    se = SurvivalEstimation(survival_curves=curves)
+    assert hasattr(se, "hazard_interp")
+
+
+def test_lifespan(data):
+    rossi, curves = data
+
+    age = pd.to_timedelta(rossi["age"] * 365.25, unit="D")
+    birth = pd.to_datetime('2000')
+    rossi["index"] = rossi.index
+    lifespan = Lifespan(
+        curves,
+        index=rossi["index"],
+        birth=birth,
+        age=age,
+        window=(pd.to_datetime("2000"), pd.to_datetime("2100"))
+    )
+
+    # test plot function
+    lifespan.plot_curves_residual_life()
+    lifespan.plot_curves()
+    lifespan.add_supervision(event=rossi["arrest"],
+                             durations=pd.to_timedelta(rossi["week"] * 7, unit="D"))
+
+    lifespan.compute_survival()
+    lifespan.compute_expected_residual_life()
+    lifespan.compute_percentile_life()
 
 
-def test_lifespan():
-    rossi = load_rossi()
```

