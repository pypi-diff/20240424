# Comparing `tmp/synthx-1.0.0.tar.gz` & `tmp/synthx-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synthx-1.0.0.tar", max compression
+gzip compressed data, was "synthx-1.0.1.tar", max compression
```

## Comparing `synthx-1.0.0.tar` & `synthx-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     7541 2024-04-23 18:47:48.789276 synthx-1.0.0/README.md
--rw-r--r--   0        0        0     1270 2024-04-23 18:47:48.799514 synthx-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      415 2024-04-22 16:15:26.237522 synthx-1.0.0/synthx/__init__.py
--rw-r--r--   0        0        0        0 2024-03-24 06:28:58.858654 synthx-1.0.0/synthx/core/__init__.py
--rw-r--r--   0        0        0     8374 2024-04-23 18:47:48.799764 synthx-1.0.0/synthx/core/dataset.py
--rw-r--r--   0        0        0     6772 2024-04-23 18:47:48.799976 synthx-1.0.0/synthx/core/result.py
--rw-r--r--   0        0        0     7362 2024-04-22 16:14:41.909807 synthx-1.0.0/synthx/core/sample.py
--rw-r--r--   0        0        0      818 2024-04-18 01:31:14.755622 synthx-1.0.0/synthx/errors/__init__.py
--rw-r--r--   0        0        0    11233 2024-04-23 18:47:48.800205 synthx-1.0.0/synthx/method.py
--rw-r--r--   0        0        0       91 2024-03-25 05:14:52.967139 synthx-1.0.0/synthx/stats/__init__.py
--rw-r--r--   0        0        0     1802 2024-04-18 01:31:14.755779 synthx-1.0.0/synthx/stats/norm.py
--rw-r--r--   0        0        0     1053 2024-04-23 18:47:48.800391 synthx-1.0.0/synthx/stats/p.py
--rw-r--r--   0        0        0     8325 1970-01-01 00:00:00.000000 synthx-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     7544 2024-04-24 02:56:45.373477 synthx-1.0.1/README.md
+-rw-r--r--   0        0        0     1270 2024-04-24 02:56:45.381601 synthx-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      415 2024-04-22 16:15:26.237522 synthx-1.0.1/synthx/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-24 06:28:58.858654 synthx-1.0.1/synthx/core/__init__.py
+-rw-r--r--   0        0        0     8374 2024-04-23 18:48:20.102367 synthx-1.0.1/synthx/core/dataset.py
+-rw-r--r--   0        0        0     6772 2024-04-23 18:48:20.102583 synthx-1.0.1/synthx/core/result.py
+-rw-r--r--   0        0        0     7362 2024-04-22 16:14:41.909807 synthx-1.0.1/synthx/core/sample.py
+-rw-r--r--   0        0        0      818 2024-04-18 01:31:14.755622 synthx-1.0.1/synthx/errors/__init__.py
+-rw-r--r--   0        0        0    10880 2024-04-24 02:56:45.381859 synthx-1.0.1/synthx/method.py
+-rw-r--r--   0        0        0       91 2024-03-25 05:14:52.967139 synthx-1.0.1/synthx/stats/__init__.py
+-rw-r--r--   0        0        0     1802 2024-04-18 01:31:14.755779 synthx-1.0.1/synthx/stats/norm.py
+-rw-r--r--   0        0        0     1053 2024-04-23 18:47:48.800391 synthx-1.0.1/synthx/stats/p.py
+-rw-r--r--   0        0        0     8328 1970-01-01 00:00:00.000000 synthx-1.0.1/PKG-INFO
```

### Comparing `synthx-1.0.0/README.md` & `synthx-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -129,30 +129,30 @@
 ```
 
 ### Placebo Test
 
 Perform a Placebo Test to assess the statistical significance of the estimated treatment effect using the `placebo_test()` function.
 
 ```python
-effect_test, effects_placebo, sc_test, scs_placebo = sx.placebo_test(dataset)
+effects_test, effects_placebo, sc_test, scs_placebo = sx.placebo_test(dataset)
 ```
 
 Calculate the p-value of the estimated treatment effect using the `calc_p_value()` function from the `stats` module.
 
 ```python
->>> sx.stats.calc_p_value(effect_test, effects_placebo)
+>>> sx.stats.calc_p_value(effects_test, effects_placebo)
 0.03228841882463891
 ```
 
 ### Sensitivity Check
 
 Perform a sensitivity check on the synthetic control results using the `sensitivity_check()` function.
 
 ```python
->>> effect_test, effects_placebo, sc_test, scs_placebo = sx.placebo_test(dataset)
+>>> effects_test, effects_placebo, sc_test, scs_placebo = sx.placebo_test(dataset)
 >>> sensitivity_check(dataset, effects_placebo)
 1.05
 ```
 
 This means this set up can capture the effect of the intervention which has more than 5 % uplift.
 
 ## Contributing
```

### Comparing `synthx-1.0.0/pyproject.toml` & `synthx-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "synthx"
-version = "1.0.0"
+version = "1.0.1"
 description = "A Python Library for Advanced Synthetic Control Analysis"
 authors = ["kenki931128 <kenki.nkmr@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `synthx-1.0.0/synthx/core/dataset.py` & `synthx-1.0.1/synthx/core/dataset.py`

 * *Files identical despite different names*

### Comparing `synthx-1.0.0/synthx/core/result.py` & `synthx-1.0.1/synthx/core/result.py`

 * *Files identical despite different names*

### Comparing `synthx-1.0.0/synthx/core/sample.py` & `synthx-1.0.1/synthx/core/sample.py`

 * *Files identical despite different names*

### Comparing `synthx-1.0.0/synthx/errors/__init__.py` & `synthx-1.0.1/synthx/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `synthx-1.0.0/synthx/method.py` & `synthx-1.0.1/synthx/method.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,22 +26,16 @@
     Returns:
         sx.SyntheticControlResult: The result of synthetic control with optimized weights.
 
     Raises:
         NotImplementedError: If there are multiple units that received the intervention.
         NoFeasibleModelError: If the optimization of unit weights fails to find a feasible solution.
 
-    Note:
-        - The function currently supports only a single unit that received the intervention.
-        - The weights for variables (y and covariates) are currently set to 1 for all variables.
-
     TODO:
-        - Add validation period for evaluating the performance of the synthetic control.
         - Allow different weights for variables based on their importance or relevance.
-        - Support multiple units that received the intervention. (also need to update result class)
     """
 
     df = dataset.data
 
     # condition
     training_time = (
         dataset.validation_time
@@ -123,26 +117,26 @@
 
     Args:
         dataset (sx.Dataset): The dataset containing the time series data for the test and control areas.
         n_jobs (int): the number of cores used. -1 means using as many as possible.
 
     Returns:
         tuple: A tuple containing the following elements:
-            - effect_test (float): The estimated effect of the intervention in the test area.
-            - effects_placebo (List[float]): The estimated placebo effects for each control area.
+            - effects_test (list[float]): The estimated effect of the intervention in the test area.
+            - effects_placebo (list[float]): The estimated placebo effects for each control area.
             - sc_test (sx.SyntheticControlResult): The synthetic control result for the test area.
-            - scs_placebo (List[sx.SyntheticControlResult]): The synthetic control results
+            - scs_placebo (list[sx.SyntheticControlResult]): The synthetic control results
                 for each control area.
     """
     # placebo effect in test area
     try:
         sc_test = synthetic_control(dataset)
     except NoFeasibleModelError:
         raise NoFeasibleModelError('synthetic control optimization failed for test units.')
-    effect_test = sc_test.estimate_effects()
+    effects_test = sc_test.estimate_effects()
 
     # placebo effects in control areas
     effects_placebo: list[float] = []
     scs_placebo: list[sx.SyntheticControlResult] = []
     control_units = (
         dataset.data.filter(~dataset.data[dataset.unit_column].is_in(dataset.intervention_units))[
             dataset.unit_column
@@ -207,15 +201,15 @@
     scs_placebo = []
     for result in results:
         if result is not None:
             effect_placebo, sc_placebo = result
             effects_placebo.append(effect_placebo[0])
             scs_placebo.append(sc_placebo)
 
-    return effect_test, effects_placebo, sc_test, scs_placebo
+    return effects_test, effects_placebo, sc_test, scs_placebo
 
 
 def sensitivity_check(
     dataset: sx.Dataset, effects_placebo: list[float], p_value_target: float = 0.03
 ) -> Optional[float]:
     """Perform a sensitivity check on the synthetic control results.
 
@@ -226,15 +220,17 @@
 
     Returns:
         float or None: The uplift which becomes statistically significant.
     """
     df = dataset.data
 
     l, r = 1.0, 10.0
+    progress_bar = tqdm()
     while r - l > 0.001:
+        progress_bar.update(1)
         uplift = (l + r) / 2
 
         df_sensitivity = df.with_columns(
             pl.when(
                 pl.col(dataset.unit_column).is_in(dataset.intervention_units)
                 & (pl.col(dataset.time_column) >= dataset.intervention_time)
             )
@@ -263,14 +259,11 @@
         p_value = sx.stats.calc_p_value(sc.estimate_effects(), effects_placebo)
         if p_value <= p_value_target:
             r = uplift
         else:
             tqdm.write(f'uplift: {uplift:.4f}, p value: {p_value}.', file=sys.stderr)
             l = uplift
 
-    # even 1000% uplift cannot be captured.
-    if r == 10:
-        return None
-    # singnificant difference without actual uplift
-    if l == 1:
+    # even 1000% uplift cannot be captured / singnificant difference without actual uplift.
+    if r == 10 or l == 1:
         return None
     return r
```

### Comparing `synthx-1.0.0/synthx/stats/norm.py` & `synthx-1.0.1/synthx/stats/norm.py`

 * *Files identical despite different names*

### Comparing `synthx-1.0.0/synthx/stats/p.py` & `synthx-1.0.1/synthx/stats/p.py`

 * *Files identical despite different names*

### Comparing `synthx-1.0.0/PKG-INFO` & `synthx-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthx
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python Library for Advanced Synthetic Control Analysis
 License: MIT
 Author: kenki931128
 Author-email: kenki.nkmr@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -151,30 +151,30 @@
 ```
 
 ### Placebo Test
 
 Perform a Placebo Test to assess the statistical significance of the estimated treatment effect using the `placebo_test()` function.
 
 ```python
-effect_test, effects_placebo, sc_test, scs_placebo = sx.placebo_test(dataset)
+effects_test, effects_placebo, sc_test, scs_placebo = sx.placebo_test(dataset)
 ```
 
 Calculate the p-value of the estimated treatment effect using the `calc_p_value()` function from the `stats` module.
 
 ```python
->>> sx.stats.calc_p_value(effect_test, effects_placebo)
+>>> sx.stats.calc_p_value(effects_test, effects_placebo)
 0.03228841882463891
 ```
 
 ### Sensitivity Check
 
 Perform a sensitivity check on the synthetic control results using the `sensitivity_check()` function.
 
 ```python
->>> effect_test, effects_placebo, sc_test, scs_placebo = sx.placebo_test(dataset)
+>>> effects_test, effects_placebo, sc_test, scs_placebo = sx.placebo_test(dataset)
 >>> sensitivity_check(dataset, effects_placebo)
 1.05
 ```
 
 This means this set up can capture the effect of the intervention which has more than 5 % uplift.
 
 ## Contributing
```

