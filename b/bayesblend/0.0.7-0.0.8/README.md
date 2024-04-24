# Comparing `tmp/bayesblend-0.0.7.tar.gz` & `tmp/bayesblend-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bayesblend-0.0.7.tar", max compression
+gzip compressed data, was "bayesblend-0.0.8.tar", max compression
```

## Comparing `bayesblend-0.0.7.tar` & `bayesblend-0.0.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1063 2024-04-19 21:12:34.085528 bayesblend-0.0.7/LICENSE
--rw-r--r--   0        0        0     1434 2024-04-19 21:12:34.085528 bayesblend-0.0.7/README.md
--rw-r--r--   0        0        0      305 2024-04-19 21:12:35.141530 bayesblend-0.0.7/bayesblend/__init__.py
--rw-r--r--   0        0        0     5460 2024-04-19 21:12:34.085528 bayesblend-0.0.7/bayesblend/io.py
--rw-r--r--   0        0        0    44104 2024-04-19 21:12:34.085528 bayesblend-0.0.7/bayesblend/models.py
--rw-r--r--   0        0        0     1822 2024-04-19 21:12:34.085528 bayesblend-0.0.7/bayesblend/stan_files/hierarchical_stacking.stan
--rw-r--r--   0        0        0     2889 2024-04-19 21:12:34.085528 bayesblend-0.0.7/bayesblend/stan_files/hierarchical_stacking_pooling.stan
--rw-r--r--   0        0        0      300 2024-04-19 21:12:34.085528 bayesblend-0.0.7/bayesblend/stan_files/stacking.stan
--rw-r--r--   0        0        0     2654 2024-04-19 21:12:35.141530 bayesblend-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     2156 1970-01-01 00:00:00.000000 bayesblend-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-24 13:39:04.678793 bayesblend-0.0.8/LICENSE
+-rw-r--r--   0        0        0     1434 2024-04-24 13:39:04.678793 bayesblend-0.0.8/README.md
+-rw-r--r--   0        0        0      305 2024-04-24 13:39:05.646791 bayesblend-0.0.8/bayesblend/__init__.py
+-rw-r--r--   0        0        0     5484 2024-04-24 13:39:04.678793 bayesblend-0.0.8/bayesblend/io.py
+-rw-r--r--   0        0        0    45289 2024-04-24 13:39:04.678793 bayesblend-0.0.8/bayesblend/models.py
+-rw-r--r--   0        0        0     1822 2024-04-24 13:39:04.678793 bayesblend-0.0.8/bayesblend/stan_files/hierarchical_stacking.stan
+-rw-r--r--   0        0        0     2889 2024-04-24 13:39:04.678793 bayesblend-0.0.8/bayesblend/stan_files/hierarchical_stacking_pooling.stan
+-rw-r--r--   0        0        0      300 2024-04-24 13:39:04.678793 bayesblend-0.0.8/bayesblend/stan_files/stacking.stan
+-rw-r--r--   0        0        0     2654 2024-04-24 13:39:05.646791 bayesblend-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2156 1970-01-01 00:00:00.000000 bayesblend-0.0.8/PKG-INFO
```

### Comparing `bayesblend-0.0.7/LICENSE` & `bayesblend-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bayesblend-0.0.7/README.md` & `bayesblend-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `bayesblend-0.0.7/bayesblend/io.py` & `bayesblend-0.0.8/bayesblend/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,17 @@
             return 0
 
     @property
     def shape(self) -> Tuple[int, ...]:
         return (
             self.log_lik.shape
             if self.log_lik is not None
-            else self.post_pred.shape if self.post_pred is not None else ()
+            else self.post_pred.shape
+            if self.post_pred is not None
+            else ()
         )
 
     @cached_property
     def log_lik_2d(self) -> np.ndarray[Any, Any] | None:
         if self.log_lik is None:
             return None
         if self.log_lik.ndim == 2:
```

### Comparing `bayesblend-0.0.7/bayesblend/models.py` & `bayesblend-0.0.8/bayesblend/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import typing
 import warnings
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from functools import cached_property
 from pathlib import Path
-from typing import Any, Dict, Hashable, List, Literal, Sequence, Set, Tuple, Union
+from typing import Any, Dict, Hashable, List, Literal, Sequence, Tuple, Union
 
 import arviz as az
 import numpy as np
 import pandas as pd
 from cmdstanpy import CmdStanMCMC, CmdStanModel
 from scipy.optimize import OptimizeResult, minimize
 from scipy.stats import dirichlet
@@ -37,15 +37,15 @@
 
 PointwiseDiagnostics = Dict[str, Sequence[float]]
 
 ContinuousTransforms = Literal["identity", "standardize", "relu"]
 
 CONTINUOUS_TRANSFORMS = list(typing.get_args(ContinuousTransforms))
 
-CovariateInfo = Dict[str, Union[Set[Any], Dict[str, float]]]
+CovariateInfo = Dict[str, Union[List[Any], Dict[str, float]]]
 
 Weights = Dict[str, np.ndarray]
 
 Priors = Dict[str, Union[List[Union[float, int]], float, int]]
 
 CMDSTAN_DEFAULTS = {
     "chains": 4,
@@ -702,15 +702,15 @@
                 minus = {
                     key + "_minus": _relu(values, key, plus=False)
                     for key, values in continuous_covariates.items()
                 }
                 continuous_covariates = plus | minus
 
         discrete_covariate_info = (
-            {key: v for key, v in covariate_info.items() if isinstance(v, set)}
+            {key: v for key, v in covariate_info.items() if isinstance(v, list)}
             if covariate_info is not None
             else None
         )
 
         discrete_covariates_padded = (
             _make_dummy_vars(
                 discrete_covariates,
@@ -730,15 +730,15 @@
 
     def _get_covariate_info(
         self,
         discrete_covariates: Dict[str, Sequence] | None = None,
         continuous_covariates: Dict[str, Sequence] | None = None,
     ) -> CovariateInfo:
         discrete_covariate_set = (
-            {k: set(v) for k, v in discrete_covariates.items()}
+            {k: _unique(v) for k, v in discrete_covariates.items()}
             if discrete_covariates is not None
             else {}
         )
         continuous_covariate_set = (
             {
                 k: {"mean": np.mean(v), "2sd": np.std(v) * 2, "median": np.median(v)}
                 for k, v in continuous_covariates.items()
@@ -1095,26 +1095,47 @@
     w = [np.exp(zz) / W for zz in z]
 
     return w
 
 
 def _make_dummy_vars(
     discrete_covariates: Dict[str, Sequence] | None = None,
-    discrete_covariate_info: Dict[str, Set[Any]] | None = None,
+    discrete_covariate_info: Dict[str, List[Any]] | None = None,
 ) -> Dict[Hashable, Sequence]:
     if discrete_covariates is None:
         return {}
 
     new_levels_df = pd.DataFrame()
+    levels_cache = [
+        level
+        for k, v in discrete_covariates.items()
+        for level in _unique([k + "_" + level for level in v])
+    ]
+    intercepts = [
+        k + "_" + v[0]
+        for k, v in (
+            discrete_covariates.items()
+            if discrete_covariate_info is None
+            else discrete_covariate_info.items()
+        )
+    ]
 
     if discrete_covariate_info is not None:
-        unique_levels_info = set().union(*list(discrete_covariate_info.values()))
-        unique_levels_data = set().union(*list(discrete_covariates.values()))
-        has_missing_levels = unique_levels_info - unique_levels_data
-        has_new_levels = unique_levels_data - unique_levels_info
+        unique_levels_info = {
+            k: set().union(v)
+            for k, v
+            in discrete_covariate_info.items()
+        }
+        unique_levels_data = {
+            k: set().union(v)
+            for k, v
+            in discrete_covariates.items()
+        }
+        has_missing_levels = {k: unique_levels_info[k] - unique_levels_data[k] for k in unique_levels_info}
+        has_new_levels = {k: unique_levels_data[k] - unique_levels_info[k] for k in unique_levels_data}
 
         # We create dummy coded columns here and append them to the end of the
         # dataframe so that we later know which columns did not originally
         # have the "new" covariates for prediction purposes
         if has_new_levels:
             new_levels_dict = {
                 covariate: list(
@@ -1129,46 +1150,52 @@
                 for level in new_levels:
                     new_covariate = covariate + "_" + level
                     dummy_codes = [
                         1 if v == level else 0 for v in discrete_covariates[covariate]
                     ]
                     new_level_dummys[new_covariate] = dummy_codes
 
-            new_levels_df = pd.DataFrame(new_level_dummys)
+            ordered_new_level_dummys = {
+                k: new_level_dummys[k]
+                for k in levels_cache
+                if k in new_level_dummys
+            }
+
+            new_levels_df = pd.DataFrame(ordered_new_level_dummys)
 
         # if levels are missing, append dummy df to end of data df, assign dummy
         # variables, and then remove appended dummy df from result. This way,
         # we get the necessary discrete covariate columns, even if all 0's
         if has_missing_levels:
             missing_level_df = pd.DataFrame(
                 {
                     k: pd.Series(list(v))
                     for k, v in (discrete_covariates | discrete_covariate_info).items()
                 }
             ).ffill()
 
+            concat_all_covariates = pd.concat(
+                [missing_level_df, pd.DataFrame(discrete_covariates)]
+            ).apply(lambda i: pd.Categorical(i, categories=i.unique(), ordered=True))  # type: ignore
+
             dummy_coded_df = pd.get_dummies(
-                pd.concat([pd.DataFrame(discrete_covariates), missing_level_df]),
-                drop_first=True,
-            ).iloc[: -len(missing_level_df)]
+                concat_all_covariates, dtype=int
+            ).drop(intercepts, axis=1).iloc[len(missing_level_df) :]
 
-            return pd.concat(
+            clean_dummies = pd.concat(
                 [dummy_coded_df.drop(new_levels_df.columns, axis=1), new_levels_df],
                 axis=1,
-            ).to_dict("list")
+            )
+            return clean_dummies.to_dict("list")
 
-    return pd.concat(
-        [
-            pd.get_dummies(
-                pd.DataFrame(discrete_covariates), drop_first=True, dtype=int
-            ),
-            new_levels_df,
-        ],
-        axis=1,
-    ).to_dict("list")
+    covariate_df = pd.DataFrame(discrete_covariates).apply(
+        lambda i: pd.Categorical(i, categories=i.unique(), ordered=True) # type: ignore
+    )
+    dummies = pd.get_dummies(covariate_df, dtype=int).drop(intercepts, axis=1)
+    return pd.concat([dummies, new_levels_df], axis=1).to_dict("list")
 
 
 def _concat_array_empty(arrays: List[np.ndarray], axis: int = 0) -> np.ndarray:
     return np.concatenate([array for array in arrays if len(array) > 0], axis=axis)
 
 
 def _running_weight_mean(
@@ -1178,7 +1205,12 @@
 
 
 def _normalize_weights(weights: np.ndarray):
     """Normalize weights due to rounding error, witch strict value check"""
     if not np.isclose(sum(weights), 1, atol=1e-7):
         raise ValueError(f"Weights do not sum to 1: {weights}.")
     return np.array([max(0, w) for w in weights / sum(weights)])
+
+
+def _unique(x: List[Any] | Sequence[Any]) -> List:
+    seen = set()
+    return [i for i in x if not (i in seen or seen.add(i))]  # type: ignore
```

### Comparing `bayesblend-0.0.7/bayesblend/stan_files/hierarchical_stacking.stan` & `bayesblend-0.0.8/bayesblend/stan_files/hierarchical_stacking.stan`

 * *Files identical despite different names*

### Comparing `bayesblend-0.0.7/bayesblend/stan_files/hierarchical_stacking_pooling.stan` & `bayesblend-0.0.8/bayesblend/stan_files/hierarchical_stacking_pooling.stan`

 * *Files identical despite different names*

### Comparing `bayesblend-0.0.7/pyproject.toml` & `bayesblend-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bayesblend"
-version = "0.0.7"
+version = "0.0.8"
 description = "Easily combine predictions from multiple Bayesian models using techniques including (pseudo) Bayesian model averaging, hierarchical stacking, and more!"
 authors = [
     "Nathaniel Haines <nathaniel.haines@ledgerinvesting.com>",
     "Conor Goold <conor@ledgerinvesting.com>",
 ]
 readme = "README.md"
```

### Comparing `bayesblend-0.0.7/PKG-INFO` & `bayesblend-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bayesblend
-Version: 0.0.7
+Version: 0.0.8
 Summary: Easily combine predictions from multiple Bayesian models using techniques including (pseudo) Bayesian model averaging, hierarchical stacking, and more!
 Author: Nathaniel Haines
 Author-email: nathaniel.haines@ledgerinvesting.com
 Requires-Python: >=3.10,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

