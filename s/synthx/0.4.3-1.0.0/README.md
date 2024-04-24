# Comparing `tmp/synthx-0.4.3.tar.gz` & `tmp/synthx-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synthx-0.4.3.tar", max compression
+gzip compressed data, was "synthx-1.0.0.tar", max compression
```

## Comparing `synthx-0.4.3.tar` & `synthx-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     7539 2024-04-22 16:29:44.049795 synthx-0.4.3/README.md
--rw-r--r--   0        0        0     1270 2024-04-23 01:39:44.139362 synthx-0.4.3/pyproject.toml
--rw-r--r--   0        0        0      415 2024-04-22 16:15:26.237522 synthx-0.4.3/synthx/__init__.py
--rw-r--r--   0        0        0        0 2024-03-24 06:28:58.858654 synthx-0.4.3/synthx/core/__init__.py
--rw-r--r--   0        0        0     7302 2024-04-18 01:31:14.755205 synthx-0.4.3/synthx/core/dataset.py
--rw-r--r--   0        0        0     4718 2024-03-25 05:07:58.244991 synthx-0.4.3/synthx/core/result.py
--rw-r--r--   0        0        0     7362 2024-04-22 16:14:41.909807 synthx-0.4.3/synthx/core/sample.py
--rw-r--r--   0        0        0      818 2024-04-18 01:31:14.755622 synthx-0.4.3/synthx/errors/__init__.py
--rw-r--r--   0        0        0    10394 2024-04-23 01:39:44.139643 synthx-0.4.3/synthx/method.py
--rw-r--r--   0        0        0       91 2024-03-25 05:14:52.967139 synthx-0.4.3/synthx/stats/__init__.py
--rw-r--r--   0        0        0     1802 2024-04-18 01:31:14.755779 synthx-0.4.3/synthx/stats/norm.py
--rw-r--r--   0        0        0     1026 2024-03-25 05:14:52.967319 synthx-0.4.3/synthx/stats/p.py
--rw-r--r--   0        0        0     8323 1970-01-01 00:00:00.000000 synthx-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     7541 2024-04-23 18:47:48.789276 synthx-1.0.0/README.md
+-rw-r--r--   0        0        0     1270 2024-04-23 18:47:48.799514 synthx-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      415 2024-04-22 16:15:26.237522 synthx-1.0.0/synthx/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-24 06:28:58.858654 synthx-1.0.0/synthx/core/__init__.py
+-rw-r--r--   0        0        0     8374 2024-04-23 18:47:48.799764 synthx-1.0.0/synthx/core/dataset.py
+-rw-r--r--   0        0        0     6772 2024-04-23 18:47:48.799976 synthx-1.0.0/synthx/core/result.py
+-rw-r--r--   0        0        0     7362 2024-04-22 16:14:41.909807 synthx-1.0.0/synthx/core/sample.py
+-rw-r--r--   0        0        0      818 2024-04-18 01:31:14.755622 synthx-1.0.0/synthx/errors/__init__.py
+-rw-r--r--   0        0        0    11233 2024-04-23 18:47:48.800205 synthx-1.0.0/synthx/method.py
+-rw-r--r--   0        0        0       91 2024-03-25 05:14:52.967139 synthx-1.0.0/synthx/stats/__init__.py
+-rw-r--r--   0        0        0     1802 2024-04-18 01:31:14.755779 synthx-1.0.0/synthx/stats/norm.py
+-rw-r--r--   0        0        0     1053 2024-04-23 18:47:48.800391 synthx-1.0.0/synthx/stats/p.py
+-rw-r--r--   0        0        0     8325 1970-01-01 00:00:00.000000 synthx-1.0.0/PKG-INFO
```

### Comparing `synthx-0.4.3/README.md` & `synthx-1.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 
 <img src="./docs/assets/imgs/synthetic_control.png" width="100%">
 
 You can estimate the causal effect of the intervention using the `estimate_effects()` method.
 
 ```python
 >>> sc.estimate_effects()
-0.8398940970771678
+[0.8398940970771678]
 ```
 
 ### Placebo Test
 
 Perform a Placebo Test to assess the statistical significance of the estimated treatment effect using the `placebo_test()` function.
 
 ```python
```

### Comparing `synthx-0.4.3/pyproject.toml` & `synthx-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "synthx"
-version = "0.4.3"
+version = "1.0.0"
 description = "A Python Library for Advanced Synthetic Control Analysis"
 authors = ["kenki931128 <kenki.nkmr@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `synthx-0.4.3/synthx/core/dataset.py` & `synthx-1.0.0/synthx/core/dataset.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,38 +26,41 @@
         *,
         unit_column: str,
         time_column: str,
         y_column: str,
         covariate_columns: Optional[list[str]],
         intervention_units: Union[Any, list[Any]],
         intervention_time: Union[int, date],
+        validation_time: Optional[Union[int, date]] = None,
         norm: Optional[str] = None,
     ) -> None:
         """Initialize the Dataset.
 
         Args:
             data (pl.DataFram): The input dataset as a Polars DataFrame.
             unit_column (str): The column representing the unit.
             time_column (str): The column representing the time period.
             y_column (str): The column representing the target variable.
             covariate_columns (Optional[list[str]]): The columns representing the covariates.
             intervention_units (Union[Any, list[Any]]): A list of intervented units
             intervention_time (Union[int, date]): When the intervention or event happens.
+            validation_time (Optional[Union[int, date]]): validation time if needed.
             norm (Optional[str]): If not None, will normalize the y_column.
                 it should be 'z_standardize'
         """
         self.data = data
         self.unit_column = unit_column
         self.time_column = time_column
         self.y_column = y_column
         self.covariate_columns = covariate_columns
         self.intervention_units = (
             intervention_units if isinstance(intervention_units, list) else [intervention_units]
         )
         self.intervention_time = intervention_time
+        self.validation_time = validation_time
         self.norm = norm
         self.__validate()
         self.__normalization()
 
     def plot(self, units: Optional[list[str]] = None, save: Optional[str] = None) -> None:
         """Plot the dataset and display its characteristics.
 
@@ -67,15 +70,20 @@
         """
         # Plot the target variable over time for each unit
         units = units if units is not None else self.data[self.unit_column].unique().to_list()
         plt.figure(figsize=(10, 6))
         for unit in units:
             unit_data = self.data.filter(pl.col(self.unit_column) == unit)
             plt.plot(unit_data[self.time_column], unit_data[self.y_column], label=f'Unit {unit}')
-        # Add vertical line for intervention time
+
+        # Add vertical line for validation time and intervention time
+        if self.validation_time is not None:
+            plt.axvline(
+                self.validation_time, color='orange', linestyle='--', label='Validation Time'  # type: ignore
+            )
         plt.axvline(
             self.intervention_time, color='red', linestyle='--', label='Intervention Time'  # type: ignore
         )
 
         plt.xlabel('Time')
         plt.ylabel('Target Variable')
         plt.title('Target Variable Over Time')
@@ -92,14 +100,16 @@
 
         Raises:
             ColumnNotFoundError if a required column is missing.
             InvalidColumnTypeError if a column has an invalid data type.
         """
         if self.unit_column not in self.data.columns:
             raise ColumnNotFoundError(self.unit_column)
+        if len(self.intervention_units) == 0:
+            raise InvalidInterventionUnitError(f'at least, need to specify one intervention unit.')
         for intervention_unit in self.intervention_units:
             if intervention_unit not in self.data[self.unit_column].unique():
                 raise InvalidInterventionUnitError(f'{intervention_unit} does not exist.')
 
         if self.time_column not in self.data.columns:
             raise ColumnNotFoundError(self.time_column)
         if self.data[self.time_column].dtype not in [pl.Int64, pl.Date]:
@@ -111,14 +121,24 @@
             and isinstance(self.intervention_time, date)
         ):
             raise InvalidColumnTypeError(
                 f'{self.time_column} and intervention_time should have the same type.'
             )
         if self.intervention_time > self.data[self.time_column].max():  # type: ignore
             raise InvalidInterventionTimeError(f'no date point at {self.intervention_time} time.')
+        if self.validation_time is not None and type(self.intervention_time) != type(
+            self.validation_time
+        ):
+            raise InvalidColumnTypeError(
+                f'intervention_time and validation_time should have the same type.'
+            )
+        if self.validation_time is not None and self.intervention_time <= self.validation_time:  # type: ignore
+            raise InvalidInterventionTimeError(
+                f'intervention_time should be later than validation_time.'
+            )
 
         if self.y_column not in self.data.columns:
             raise ColumnNotFoundError(self.y_column)
         if self.data[self.y_column].dtype != pl.Float64:
             raise InvalidColumnTypeError(f'{self.y_column} should be float.')
 
         units = self.data[self.unit_column].unique()
```

### Comparing `synthx-0.4.3/synthx/core/sample.py` & `synthx-1.0.0/synthx/core/sample.py`

 * *Files identical despite different names*

### Comparing `synthx-0.4.3/synthx/errors/__init__.py` & `synthx-1.0.0/synthx/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `synthx-0.4.3/synthx/method.py` & `synthx-1.0.0/synthx/method.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,70 +39,87 @@
         - Allow different weights for variables based on their importance or relevance.
         - Support multiple units that received the intervention. (also need to update result class)
     """
 
     df = dataset.data
 
     # condition
-    # TODO: add validation period
-    condition_pre_intervention_time = df[dataset.time_column] < dataset.intervention_time
-    condition_test_units = df[dataset.unit_column].is_in(dataset.intervention_units)
+    training_time = (
+        dataset.validation_time
+        if dataset.validation_time is not None
+        else dataset.intervention_time
+    )
+    condition_training_time = df[dataset.time_column] < training_time
     condition_control_units = ~df[dataset.unit_column].is_in(dataset.intervention_units)
 
-    # weights for variables
-    # TODO: use different weights for variables
+    # weights for variables and scale each variables
+    # weights of y_column : weights of others = 8 : 2.
+    # TODO: Update if there are better weights balance.
     variables = [dataset.y_column]
+    variable_weights: dict[str, float] = {}
     if dataset.covariate_columns is not None:
         variables += dataset.covariate_columns
-    variable_weights = {variable: 1 for variable in variables}
+        variable_weights = {
+            covariate: 2 / len(dataset.covariate_columns) for covariate in dataset.covariate_columns
+        }
+    variable_weights[dataset.y_column] = 8.0
+    for variable in variables:
+        df = df.with_columns(
+            ((pl.col(variable) - pl.col(variable).min()) / pl.col(variable).std()).alias(variable)
+        )
 
-    # TODO: multiple units intervention
-    if len(dataset.intervention_units) > 1:
-        raise NotImplementedError('multiple intervented units.')
-
-    # dataframe for test & control
-    df_test = df.filter(condition_pre_intervention_time & condition_test_units)
-    df_control = df.filter(condition_pre_intervention_time & condition_control_units)
-
-    # optimize unit weights
-    def objective(unit_weights: np.ndarray) -> float:
-        diff = 0
-        for variable in variables:
-            df_control_pivoted = df_control.pivot(
-                index=dataset.time_column, columns=dataset.unit_column, values=variable
-            ).drop(dataset.time_column)
-            arr_control_pivoted = df_control_pivoted.to_numpy()
-            arr_test = df_test[variable].to_numpy()
-            variable_weight = variable_weights[variable]
-            diff += np.sum(
-                variable_weight
-                * (arr_test - np.sum(arr_control_pivoted * unit_weights, axis=1)) ** 2
-            )
-        return diff
+    # dataframe for control
+    df_control = df.filter(condition_training_time & condition_control_units)
 
-    control_units = df_control[dataset.unit_column].unique().to_list()
-    initial_unit_weights = np.ones(len(control_units)) / len(control_units)
-    bounds = [(0, 1)] * len(control_units)
-    # The optimization of unit weights is performed using the 'minimize' function from scipy.
-    solution = scipy.optimize.minimize(
-        objective,
-        initial_unit_weights,
-        bounds=bounds,
-        constraints={'type': 'eq', 'fun': lambda w: np.sum(w) - 1},
-    )
+    control_unit_weights: list[np.ndarray] = []
+    for intervention_unit in dataset.intervention_units:
+        condition_test_unit = df[dataset.unit_column] == intervention_unit
+        df_test = df.filter(condition_training_time & condition_test_unit)
+
+        # optimize unit weights
+        def objective(unit_weights: np.ndarray) -> float:
+            diff = 0
+            for variable in variables:
+                df_control_pivoted = df_control.pivot(
+                    index=dataset.time_column, columns=dataset.unit_column, values=variable
+                ).drop(dataset.time_column)
+                arr_control_pivoted = df_control_pivoted.to_numpy()
+                arr_test = df_test[variable].to_numpy()
+                variable_weight = variable_weights[variable]
+                diff += np.sum(
+                    variable_weight
+                    * (arr_test - np.sum(arr_control_pivoted * unit_weights, axis=1)) ** 2
+                )
+            return diff
+
+        control_units = df_control[dataset.unit_column].unique().to_list()
+        initial_unit_weights = np.ones(len(control_units)) / len(control_units)
+        bounds = [(0, 1)] * len(control_units)
+        # The optimization of unit weights is performed using the 'minimize' function from scipy.
+        solution = scipy.optimize.minimize(
+            objective,
+            initial_unit_weights,
+            bounds=bounds,
+            constraints={'type': 'eq', 'fun': lambda w: np.sum(w) - 1},
+        )
 
-    if not solution.success:
-        raise NoFeasibleModelError('synthetic control optimization failed.')
+        if not solution.success:
+            raise NoFeasibleModelError(
+                f'synthetic control optimization failed: test unit {intervention_unit}'
+            )
+        control_unit_weights.append(solution.x)
 
-    return sx.SyntheticControlResult(dataset=dataset, control_unit_weights=solution.x)
+    return sx.SyntheticControlResult(
+        dataset=dataset, control_unit_weights=np.asarray(control_unit_weights)
+    )
 
 
 def placebo_test(
     dataset: sx.Dataset, n_jobs: int = -1
-) -> tuple[float, list[float], sx.SyntheticControlResult, list[sx.SyntheticControlResult]]:
+) -> tuple[list[float], list[float], sx.SyntheticControlResult, list[sx.SyntheticControlResult]]:
     """Perform a placebo test to assess the significance of the intervention effect.
 
     This function applies the synthetic control method to the test area and each control area
     in the given dataset, estimates the placebo effects, and returns the results.
 
     Args:
         dataset (sx.Dataset): The dataset containing the time series data for the test and control areas.
@@ -133,22 +150,22 @@
         .unique()
         .to_list()
     )
     df_placebo = dataset.data.filter(dataset.data[dataset.unit_column].is_in(control_units))
 
     def process_placebo(
         test_unit_placebo: sx.Dataset,
-    ) -> Optional[tuple[float, sx.SyntheticControlResult]]:
+    ) -> Optional[tuple[list[float], sx.SyntheticControlResult]]:
         """Apply synthetic control method to a single placebo unit and estimate the effect.
 
         Args:
             test_unit_placebo (sx.Dataset): The placebo unit to be used as the test unit.
 
         Returns:
-            tuple[float, sx.SyntheticControlResult] or None: If the synthetic control optimization
+            tuple[list[float], sx.SyntheticControlResult] or None: If the synthetic control optimization
                 is successful, returns a tuple containing the following elements:
                 - effect_placebo (float): The estimated placebo effect for the given control unit.
                 - sc_placebo (sx.SyntheticControlResult): The synthetic control result for placebo.
                 If the synthetic control optimization fails, returns None.
 
         Side Effects:
             Writes an error message to stderr using tqdm.write() if the synthetic control
@@ -165,36 +182,37 @@
             df_placebo,
             unit_column=dataset.unit_column,
             time_column=dataset.time_column,
             y_column=dataset.y_column,
             covariate_columns=dataset.covariate_columns,
             intervention_units=test_unit_placebo,
             intervention_time=dataset.intervention_time,
+            validation_time=dataset.validation_time,
         )
         try:
             sc_placebo = synthetic_control(dataset_placebo)
             effect_placebo = sc_placebo.estimate_effects()
             return effect_placebo, sc_placebo
         except NoFeasibleModelError:
             tqdm.write(
                 f'placebo synthetic control optimization failed: unit {test_unit_placebo}.',
                 file=sys.stderr,
             )
             return None
 
-    results = Parallel(n_jobs=-1)(
+    results = Parallel(n_jobs=n_jobs)(
         delayed(process_placebo)(test_unit_placebo) for test_unit_placebo in tqdm(control_units)
     )
 
     effects_placebo = []
     scs_placebo = []
     for result in results:
         if result is not None:
             effect_placebo, sc_placebo = result
-            effects_placebo.append(effect_placebo)
+            effects_placebo.append(effect_placebo[0])
             scs_placebo.append(sc_placebo)
 
     return effect_test, effects_placebo, sc_test, scs_placebo
 
 
 def sensitivity_check(
     dataset: sx.Dataset, effects_placebo: list[float], p_value_target: float = 0.03
@@ -218,25 +236,26 @@
         df_sensitivity = df.with_columns(
             pl.when(
                 pl.col(dataset.unit_column).is_in(dataset.intervention_units)
                 & (pl.col(dataset.time_column) >= dataset.intervention_time)
             )
             .then(pl.col(dataset.y_column) * uplift)
             .otherwise(pl.col(dataset.y_column))
-            .alias('y')
+            .alias(dataset.y_column)
         )
 
         dataset_sensitivity = sx.Dataset(
             df_sensitivity,
             unit_column=dataset.unit_column,
             time_column=dataset.time_column,
             y_column=dataset.y_column,
             covariate_columns=dataset.covariate_columns,
             intervention_units=dataset.intervention_units,
             intervention_time=dataset.intervention_time,
+            validation_time=dataset.validation_time,
         )
 
         try:
             sc = synthetic_control(dataset_sensitivity)
         except NoFeasibleModelError:
             r = uplift  # highly likely uplift was too big. TODO: think better algorithm.
             continue
```

### Comparing `synthx-0.4.3/synthx/stats/norm.py` & `synthx-1.0.0/synthx/stats/norm.py`

 * *Files identical despite different names*

### Comparing `synthx-0.4.3/synthx/stats/p.py` & `synthx-1.0.0/synthx/stats/p.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 def calc_p_value(
     effects_test: Union[float, list[float]],
     effects_control: Union[float, list[float]],
 ) -> float:
     """Calculate the p-value using the independent t-test.
 
     This function performs an independent t-test to compare the means of two groups
-    and returns the corresponding p-value.
+    and returns the corresponding p-value. This is two sample T Test.
 
     Args:
         effects_test (Union[float, list[float]]): The effect sizes of the test group.
             Can be a single float value or a list of float values.
         effects_control (Union[float, list[float]]): The effect sizes of the control group.
             Can be a single float value or a list of float values.
```

### Comparing `synthx-0.4.3/PKG-INFO` & `synthx-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthx
-Version: 0.4.3
+Version: 1.0.0
 Summary: A Python Library for Advanced Synthetic Control Analysis
 License: MIT
 Author: kenki931128
 Author-email: kenki.nkmr@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -143,15 +143,15 @@
 
 <img src="./docs/assets/imgs/synthetic_control.png" width="100%">
 
 You can estimate the causal effect of the intervention using the `estimate_effects()` method.
 
 ```python
 >>> sc.estimate_effects()
-0.8398940970771678
+[0.8398940970771678]
 ```
 
 ### Placebo Test
 
 Perform a Placebo Test to assess the statistical significance of the estimated treatment effect using the `placebo_test()` function.
 
 ```python
```

