# Comparing `tmp/hep_ml_lab-0.4.0.tar.gz` & `tmp/hep_ml_lab-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hep_ml_lab-0.4.0.tar", max compression
+gzip compressed data, was "hep_ml_lab-0.4.1.tar", max compression
```

## Comparing `hep_ml_lab-0.4.0.tar` & `hep_ml_lab-0.4.1.tar`

### file list

```diff
@@ -1,54 +1,53 @@
--rw-r--r--   0        0        0     1064 2023-12-23 08:40:53.016508 hep_ml_lab-0.4.0/LICENSE
--rw-r--r--   0        0        0     2797 2024-04-22 13:39:00.894200 hep_ml_lab-0.4.0/README.md
--rw-r--r--   0        0        0      183 2024-03-15 06:20:36.741056 hep_ml_lab-0.4.0/hml/__init__.py
--rw-r--r--   0        0        0      530 2024-04-20 13:01:54.017209 hep_ml_lab-0.4.0/hml/approaches/__init__.py
--rw-r--r--   0        0        0       92 2024-04-03 03:17:21.104696 hep_ml_lab-0.4.0/hml/approaches/cuts/__init__.py
--rw-r--r--   0        0        0     2806 2024-04-22 11:27:56.102155 hep_ml_lab-0.4.0/hml/approaches/cuts/cut.py
--rw-r--r--   0        0        0     7380 2024-04-22 11:30:40.786156 hep_ml_lab-0.4.0/hml/approaches/cuts/cut_and_count.py
--rw-r--r--   0        0        0     4244 2024-04-22 11:27:53.158155 hep_ml_lab-0.4.0/hml/approaches/cuts/cut_layer.py
--rw-r--r--   0        0        0       84 2023-12-28 09:12:16.778964 hep_ml_lab-0.4.0/hml/approaches/networks/__init__.py
--rw-r--r--   0        0        0       34 2023-12-28 09:11:06.358963 hep_ml_lab-0.4.0/hml/approaches/networks/cnns/__init__.py
--rw-r--r--   0        0        0     1348 2024-04-22 11:28:02.730155 hep_ml_lab-0.4.0/hml/approaches/networks/cnns/simple_cnn.py
--rw-r--r--   0        0        0       34 2023-12-28 09:11:45.906964 hep_ml_lab-0.4.0/hml/approaches/networks/gnns/__init__.py
--rw-r--r--   0        0        0       25 2023-12-28 09:11:39.034964 hep_ml_lab-0.4.0/hml/approaches/networks/gnns/simple_gnn.py
--rw-r--r--   0        0        0       34 2023-12-28 09:10:31.910963 hep_ml_lab-0.4.0/hml/approaches/networks/mlps/__init__.py
--rw-r--r--   0        0        0      904 2024-04-22 11:28:09.858155 hep_ml_lab-0.4.0/hml/approaches/networks/mlps/simple_mlp.py
--rw-r--r--   0        0        0       72 2024-04-03 12:50:06.560890 hep_ml_lab-0.4.0/hml/approaches/trees/__init__.py
--rw-r--r--   0        0        0     8630 2024-03-26 06:39:43.028851 hep_ml_lab-0.4.0/hml/approaches/trees/gradient_boosted_decision_tree.py
--rw-r--r--   0        0        0      552 2024-04-22 11:28:34.846156 hep_ml_lab-0.4.0/hml/datasets/__init__.py
--rw-r--r--   0        0        0       25 2023-12-28 09:05:26.318961 hep_ml_lab-0.4.0/hml/datasets/demo_z_tagging.py
--rw-r--r--   0        0        0       28 2023-12-28 09:03:27.786961 hep_ml_lab-0.4.0/hml/datasets/graph_dataset.py
--rw-r--r--   0        0        0    10756 2024-04-22 11:30:26.266156 hep_ml_lab-0.4.0/hml/datasets/image_dataset.py
--rw-r--r--   0        0        0     8306 2024-04-22 11:28:42.814155 hep_ml_lab-0.4.0/hml/datasets/set_dataset.py
--rw-r--r--   0        0        0       47 2023-12-28 08:51:40.218957 hep_ml_lab-0.4.0/hml/generators/__init__.py
--rw-r--r--   0        0        0    17906 2024-04-22 11:32:50.546157 hep_ml_lab-0.4.0/hml/generators/madgraph5.py
--rw-r--r--   0        0        0      148 2023-12-28 09:16:14.950965 hep_ml_lab-0.4.0/hml/metrics/__init__.py
--rw-r--r--   0        0        0     1193 2024-04-22 11:30:20.342156 hep_ml_lab-0.4.0/hml/metrics/max_significance.py
--rw-r--r--   0        0        0     1205 2024-04-22 11:30:21.898156 hep_ml_lab-0.4.0/hml/metrics/rejection_at_efficiency.py
--rw-r--r--   0        0        0     2752 2024-04-22 11:27:06.542155 hep_ml_lab-0.4.0/hml/observables/__init__.py
--rw-r--r--   0        0        0     1699 2024-04-22 11:29:45.666156 hep_ml_lab-0.4.0/hml/observables/angular_distance.py
--rw-r--r--   0        0        0      399 2024-04-22 11:29:44.406156 hep_ml_lab-0.4.0/hml/observables/charge.py
--rw-r--r--   0        0        0     1052 2024-04-22 11:29:43.534156 hep_ml_lab-0.4.0/hml/observables/invariant_mass.py
--rw-r--r--   0        0        0     2435 2024-04-22 11:29:42.526156 hep_ml_lab-0.4.0/hml/observables/kinematics.py
--rw-r--r--   0        0        0     3647 2024-04-22 11:29:41.610156 hep_ml_lab-0.4.0/hml/observables/n_subjettiness.py
--rw-r--r--   0        0        0     6104 2024-04-22 11:29:38.586156 hep_ml_lab-0.4.0/hml/observables/observable.py
--rw-r--r--   0        0        0     3900 2024-04-22 11:29:39.950156 hep_ml_lab-0.4.0/hml/observables/observable_utils.py
--rw-r--r--   0        0        0      732 2024-04-22 11:29:36.046156 hep_ml_lab-0.4.0/hml/observables/size.py
--rw-r--r--   0        0        0      681 2024-04-22 11:29:34.206156 hep_ml_lab-0.4.0/hml/observables/tag.py
--rw-r--r--   0        0        0      235 2024-03-25 14:03:43.372513 hep_ml_lab-0.4.0/hml/operations/__init__.py
--rw-r--r--   0        0        0      637 2024-04-22 11:30:59.810156 hep_ml_lab-0.4.0/hml/operations/fastjet_ops.py
--rw-r--r--   0        0        0     1305 2024-04-22 11:31:06.614156 hep_ml_lab-0.4.0/hml/operations/keras_ops.py
--rw-r--r--   0        0        0        0 2024-03-12 07:03:43.891603 hep_ml_lab-0.4.0/hml/operations/repr_ops.py
--rw-r--r--   0        0        0     5529 2024-04-22 11:31:12.370156 hep_ml_lab-0.4.0/hml/operations/uproot_ops.py
--rw-r--r--   0        0        0     1041 2024-04-22 11:26:40.782155 hep_ml_lab-0.4.0/hml/physics_objects/__init__.py
--rw-r--r--   0        0        0     1969 2024-03-09 13:07:48.322260 hep_ml_lab-0.4.0/hml/physics_objects/collective.py
--rw-r--r--   0        0        0     2227 2024-03-09 13:26:26.446266 hep_ml_lab-0.4.0/hml/physics_objects/multiple.py
--rw-r--r--   0        0        0     1800 2024-03-09 13:08:41.262260 hep_ml_lab-0.4.0/hml/physics_objects/nested.py
--rw-r--r--   0        0        0     1228 2024-03-09 12:47:39.794252 hep_ml_lab-0.4.0/hml/physics_objects/physics_object.py
--rw-r--r--   0        0        0     1256 2024-03-09 13:14:59.278262 hep_ml_lab-0.4.0/hml/physics_objects/single.py
--rw-r--r--   0        0        0       71 2024-03-13 08:33:31.824123 hep_ml_lab-0.4.0/hml/representations/__init__.py
--rw-r--r--   0        0        0       21 2023-12-28 09:01:41.854960 hep_ml_lab-0.4.0/hml/representations/graph.py
--rw-r--r--   0        0        0    17453 2024-04-22 11:31:35.350156 hep_ml_lab-0.4.0/hml/representations/image.py
--rw-r--r--   0        0        0     2487 2024-04-22 11:31:38.206157 hep_ml_lab-0.4.0/hml/representations/set.py
--rw-r--r--   0        0        0     1897 2024-04-22 11:11:31.866150 hep_ml_lab-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4161 1970-01-01 00:00:00.000000 hep_ml_lab-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-12-23 08:40:53.016508 hep_ml_lab-0.4.1/LICENSE
+-rw-r--r--   0        0        0     3350 2024-04-24 09:31:52.071094 hep_ml_lab-0.4.1/README.md
+-rw-r--r--   0        0        0      193 2024-04-24 09:31:52.075094 hep_ml_lab-0.4.1/hml/__init__.py
+-rw-r--r--   0        0        0      530 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.1/hml/approaches/__init__.py
+-rw-r--r--   0        0        0       92 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.1/hml/approaches/cuts/__init__.py
+-rw-r--r--   0        0        0     2851 2024-04-24 08:39:13.795076 hep_ml_lab-0.4.1/hml/approaches/cuts/cut.py
+-rw-r--r--   0        0        0     7318 2024-04-24 08:39:13.799076 hep_ml_lab-0.4.1/hml/approaches/cuts/cut_and_count.py
+-rw-r--r--   0        0        0     4244 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.1/hml/approaches/cuts/cut_layer.py
+-rw-r--r--   0        0        0       84 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.1/hml/approaches/networks/__init__.py
+-rw-r--r--   0        0        0       34 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.1/hml/approaches/networks/cnns/__init__.py
+-rw-r--r--   0        0        0     1348 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.1/hml/approaches/networks/cnns/simple_cnn.py
+-rw-r--r--   0        0        0       34 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.1/hml/approaches/networks/gnns/__init__.py
+-rw-r--r--   0        0        0       25 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.1/hml/approaches/networks/gnns/simple_gnn.py
+-rw-r--r--   0        0        0       34 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.1/hml/approaches/networks/mlps/__init__.py
+-rw-r--r--   0        0        0      904 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.1/hml/approaches/networks/mlps/simple_mlp.py
+-rw-r--r--   0        0        0       72 2024-04-22 13:52:21.106204 hep_ml_lab-0.4.1/hml/approaches/trees/__init__.py
+-rw-r--r--   0        0        0     9251 2024-04-24 08:39:13.799076 hep_ml_lab-0.4.1/hml/approaches/trees/gradient_boosted_decision_tree.py
+-rw-r--r--   0        0        0      552 2024-04-22 13:52:21.106204 hep_ml_lab-0.4.1/hml/datasets/__init__.py
+-rw-r--r--   0        0        0       25 2024-04-22 13:52:21.106204 hep_ml_lab-0.4.1/hml/datasets/demo_z_tagging.py
+-rw-r--r--   0        0        0       28 2024-04-22 13:52:21.106204 hep_ml_lab-0.4.1/hml/datasets/graph_dataset.py
+-rw-r--r--   0        0        0    10756 2024-04-22 13:52:21.106204 hep_ml_lab-0.4.1/hml/datasets/image_dataset.py
+-rw-r--r--   0        0        0     8472 2024-04-24 08:39:13.799076 hep_ml_lab-0.4.1/hml/datasets/set_dataset.py
+-rw-r--r--   0        0        0       47 2024-04-22 13:52:21.106204 hep_ml_lab-0.4.1/hml/generators/__init__.py
+-rw-r--r--   0        0        0    17799 2024-04-24 08:39:13.799076 hep_ml_lab-0.4.1/hml/generators/madgraph5.py
+-rw-r--r--   0        0        0      148 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.1/hml/metrics/__init__.py
+-rw-r--r--   0        0        0     1193 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.1/hml/metrics/max_significance.py
+-rw-r--r--   0        0        0     1205 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.1/hml/metrics/rejection_at_efficiency.py
+-rw-r--r--   0        0        0     2774 2024-04-24 08:39:13.799076 hep_ml_lab-0.4.1/hml/observables/__init__.py
+-rw-r--r--   0        0        0     1699 2024-04-23 12:46:29.442671 hep_ml_lab-0.4.1/hml/observables/angular_distance.py
+-rw-r--r--   0        0        0      399 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.1/hml/observables/charge.py
+-rw-r--r--   0        0        0     1043 2024-04-24 08:39:13.803076 hep_ml_lab-0.4.1/hml/observables/invariant_mass.py
+-rw-r--r--   0        0        0     2435 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.1/hml/observables/kinematics.py
+-rw-r--r--   0        0        0     3647 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.1/hml/observables/n_subjettiness.py
+-rw-r--r--   0        0        0     6130 2024-04-24 08:39:13.803076 hep_ml_lab-0.4.1/hml/observables/observable.py
+-rw-r--r--   0        0        0      732 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.1/hml/observables/size.py
+-rw-r--r--   0        0        0      681 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.1/hml/observables/tag.py
+-rw-r--r--   0        0        0      235 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.1/hml/operations/__init__.py
+-rw-r--r--   0        0        0      637 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.1/hml/operations/fastjet_ops.py
+-rw-r--r--   0        0        0     1305 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.1/hml/operations/keras_ops.py
+-rw-r--r--   0        0        0        0 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.1/hml/operations/repr_ops.py
+-rw-r--r--   0        0        0     5529 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.1/hml/operations/uproot_ops.py
+-rw-r--r--   0        0        0     1056 2024-04-24 08:39:13.803076 hep_ml_lab-0.4.1/hml/physics_objects/__init__.py
+-rw-r--r--   0        0        0     1969 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.1/hml/physics_objects/collective.py
+-rw-r--r--   0        0        0     2227 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.1/hml/physics_objects/multiple.py
+-rw-r--r--   0        0        0     1800 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.1/hml/physics_objects/nested.py
+-rw-r--r--   0        0        0     1228 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.1/hml/physics_objects/physics_object.py
+-rw-r--r--   0        0        0     1256 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.1/hml/physics_objects/single.py
+-rw-r--r--   0        0        0       71 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.1/hml/representations/__init__.py
+-rw-r--r--   0        0        0       21 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.1/hml/representations/graph.py
+-rw-r--r--   0        0        0    17647 2024-04-24 08:39:13.803076 hep_ml_lab-0.4.1/hml/representations/image.py
+-rw-r--r--   0        0        0     2472 2024-04-24 08:39:13.803076 hep_ml_lab-0.4.1/hml/representations/set.py
+-rw-r--r--   0        0        0     1872 2024-04-24 09:31:52.075094 hep_ml_lab-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     4604 1970-01-01 00:00:00.000000 hep_ml_lab-0.4.1/PKG-INFO
```

### Comparing `hep_ml_lab-0.4.0/LICENSE` & `hep_ml_lab-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.0/README.md` & `hep_ml_lab-0.4.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -17,28 +17,37 @@
 To get started, please check out the [documents](https://star9daisy.github.io/hep-ml-lab/).
 
 ## Installation
 ```python
 pip install hep-ml-lab
 ```
 
+Check out the [install via pip](install/pip.md) for more details of prerequisites and post-installation steps or [install via Docker](install/docker.md) for a hassle-free experience.
+
 ## Module overview
 
-![module_overview](docs/images/module_overview.svg)
+![module_overview](docs/images/hml_modules.png)
 
 - `hml.generators`: API of Madgraph5 for simulating colliding events;
 - `hml.physics_objects`: Physics objects classfied by their counts;
 - `hml.observables`: General observables in jet physics;
 - `hml.representations`: Different data structure used to represent an event;
 - `hml.datasets`: Existing datasets and helper classes for creating new datasets;
 - `hml.approaches`: Cuts, trees and networks for classification;
 - `hml.metrics`: Metrics used in classical signal vs background analysis;
 
 ## Updates
 
+### v0.4.1
+- Fix module overview image in README.
+- Fix `GradientBoostedDecisionTree` to be compatible with different `sklearn` versions.
+- Fix `hml.datasets.SetDataset.show` to display the correct rows and columns.
+- Rename the `parse` and `register` functions to `parse_physics_object`, `parse_observable`, and `register_observable`.
+- Update the installation document.
+
 ### v0.4.0
 This version refactors most of the codebase to make it compatible with the array
 (from `awkward` and `uproot`) representation of the data.
 
 ### v0.3.0.1
 - Fix a bug that Madgraph5 may run into an infinite loop caused by HML keeping
   removing py.py file during initialization.
```

### Comparing `hep_ml_lab-0.4.0/hml/approaches/__init__.py` & `hep_ml_lab-0.4.1/hml/approaches/__init__.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.0/hml/approaches/cuts/cut.py` & `hep_ml_lab-0.4.1/hml/approaches/cuts/cut.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import re
 
 import awkward as ak
 
-from hml.observables import parse
+from hml.observables import parse_observable
 
 
 class Cut:
     def __init__(self, expression) -> None:
         self._expression = expression
         self._parse_expression(expression)
 
@@ -42,15 +42,17 @@
                 cuts_dict[new_cut[0]] = obs
                 cuts_dict[new_cut[1]] = obs
                 expr = expr.replace(cut, f"({new_cut[0]} & {new_cut[1]})")
             else:
                 cuts_dict[cut] = obs
 
         self._cuts_dict = cuts_dict
-        self._observables_dict = {obs: parse(obs) for obs in cuts_dict.values()}
+        self._observables_dict = {
+            obs: parse_observable(obs) for obs in cuts_dict.values()
+        }
         self._expr = expr
 
     def read(self, events):
         for obs in self._observables_dict.values():
             obs.read(events)
         observables_dict = self._observables_dict
 
@@ -62,15 +64,15 @@
         # Validate the type
         shapes = set([obs.shape for obs in observables_dict.values()])
         if len(shapes) != 1:
             raise ValueError
 
         expression = self._expr
         for cut in cuts_results:
-            cut_pattern = r"\b" + cut.replace(".", "\.") + r"\b"
+            cut_pattern = r"\b" + cut.replace(".", "\\.") + r"\b"
             expression = re.sub(cut_pattern, f"cuts_results['{cut}']", expression)
 
         self._value = ak.fill_none(eval(expression), False)
 
         if self._value.ndim > 1:
             if self._is_any:
                 self._value = ak.any(self._value, axis=1)
```

### Comparing `hep_ml_lab-0.4.0/hml/approaches/cuts/cut_and_count.py` & `hep_ml_lab-0.4.1/hml/approaches/cuts/cut_and_count.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
 import keras
 from keras import ops
 
-# from hml.utils import ops_histogram_fixed_width, ops_unique
 from hml.operations import ops_histogram_fixed_width, ops_unique
 
 from .cut_layer import CutLayer
 
 
 @keras.saving.register_keras_serializable()
 class CutAndCount(keras.Model):
```

### Comparing `hep_ml_lab-0.4.0/hml/approaches/cuts/cut_layer.py` & `hep_ml_lab-0.4.1/hml/approaches/cuts/cut_layer.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.0/hml/approaches/networks/cnns/simple_cnn.py` & `hep_ml_lab-0.4.1/hml/approaches/networks/cnns/simple_cnn.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.0/hml/approaches/networks/mlps/simple_mlp.py` & `hep_ml_lab-0.4.1/hml/approaches/networks/mlps/simple_mlp.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.0/hml/approaches/trees/gradient_boosted_decision_tree.py` & `hep_ml_lab-0.4.1/hml/approaches/trees/gradient_boosted_decision_tree.py`

 * *Files 8% similar despite different names*

```diff
@@ -133,15 +133,21 @@
                     )
             else:
                 raise ValueError(f"Unknown metric: {metric}")
 
         def _monitor(i, model, local_variables):
             y_true = local_variables["y"]
             raw_pred = local_variables["raw_predictions"]
-            y_prob = model._loss._raw_prediction_to_proba(raw_pred)
+
+            if hasattr(model._loss, "predict_proba"):
+                # This works in 1.4.2
+                y_prob = model._loss.predict_proba(raw_pred)
+            else:
+                # This works in 1.3.0
+                y_prob = model._loss._raw_prediction_to_proba(raw_pred)
             sample_weight = local_variables["sample_weight"]
 
             loss = model._loss(y_true, raw_pred, sample_weight)
 
             y_true = (
                 y_true if not is_categorical else keras.utils.to_categorical(y_true)
             )
@@ -154,21 +160,28 @@
                 i.update_state(y_true, y_prob, sample_weight=sample_weight)
                 train_values.append((name, i.result().numpy()))
                 history.history[name].append(i.result().numpy())
 
             # Validation metrics
             val_values = []
             if validation_split != 0.0 or validation_data is not None:
+                # Reshape y_val and change dtype to match the previous one
                 y_true = (
                     self.y_val if self.y_val.ndim == 1 else self.y_val.argmax(axis=1)
-                )  # (n_samples,)
+                ).astype(y_true.dtype)  # (n_samples,)
                 raw_pred = next(model._staged_raw_predict(self.x_val))  # (n_samples, 1)
-                y_prob = model._loss._raw_prediction_to_proba(
-                    raw_pred
-                )  # (n_samples, n_classes)
+                if hasattr(model._loss, "predict_proba"):
+                    # This works in 1.4.2
+                    y_prob = model._loss.predict_proba(raw_pred)
+                else:
+                    # This works in 1.3.0
+                    y_prob = model._loss._raw_prediction_to_proba(raw_pred)
+                # y_prob = model._loss._raw_prediction_to_proba(
+                #     raw_pred
+                # )  # (n_samples, n_classes)
 
                 # ! sample_weight: (n_samples x (1 - validation_fraction),)
                 # here the validation_fraction is a parameter of the parent class
                 # print(y_true.shape, raw_pred.shape, y_prob.shape, sample_weight.shape)
                 val_loss = model._loss(y_true, raw_pred)  # , sample_weight)
                 val_values.append(("val_loss", val_loss))
                 history.history["val_loss"].append(val_loss)
```

### Comparing `hep_ml_lab-0.4.0/hml/datasets/__init__.py` & `hep_ml_lab-0.4.1/hml/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.0/hml/datasets/image_dataset.py` & `hep_ml_lab-0.4.1/hml/datasets/image_dataset.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.0/hml/datasets/set_dataset.py` & `hep_ml_lab-0.4.1/hml/datasets/set_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -231,17 +231,22 @@
 
     def show(self, n_feature_per_line=3, n_samples=-1, target=None):
         if n_samples != -1:
             samples = self.samples[:n_samples]
         else:
             samples = self.samples
 
-        plt.figure(figsize=(4 * n_feature_per_line, 4))
+        n_features = len(self.feature_names)
+        plt.figure(figsize=(3 * n_feature_per_line, 3))
         for i, name in enumerate(self.feature_names):
-            ax = plt.subplot(1, n_feature_per_line, i + 1)
+            ax = plt.subplot(
+                (n_features + n_feature_per_line - 1) // n_feature_per_line,
+                n_feature_per_line,
+                i + 1,
+            )
 
             if target is None:
                 for i_target in np.unique(self.targets):
                     ax.hist(
                         samples[np.squeeze(self.targets == i_target)][:, i],
                         bins=50,
                         histtype="step",
```

### Comparing `hep_ml_lab-0.4.0/hml/generators/madgraph5.py` & `hep_ml_lab-0.4.1/hml/generators/madgraph5.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,19 @@
 import shutil
 import subprocess
 from pathlib import Path
 from tempfile import NamedTemporaryFile
 from typing import Union
 
 import pexpect
-
-# import ROOT
 from bs4 import BeautifulSoup
 from rich.console import Console
 from rich.table import Table
 
 PathLike = Union[str, Path]
-# from ..types import Path, PathLike
-
-# _ = ROOT.gSystem.Load("libDelphes")  # type: ignore
 
 
 class Madgraph5:
     def __init__(
         self,
         executable: PathLike,
         verbose: int = 1,
```

### Comparing `hep_ml_lab-0.4.0/hml/metrics/max_significance.py` & `hep_ml_lab-0.4.1/hml/metrics/max_significance.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.0/hml/metrics/rejection_at_efficiency.py` & `hep_ml_lab-0.4.1/hml/metrics/rejection_at_efficiency.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.0/hml/observables/__init__.py` & `hep_ml_lab-0.4.1/hml/observables/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,22 +76,22 @@
     if identifier is None or identifier == "None":
         return
 
     else:
         return ALL_OBJECTS_DICT.get(identifier)
 
 
-def register(obs: Observable, *alias: str) -> None:
+def register_observable(obs: Observable, *alias: str) -> None:
     ALL_OBJECTS.add(obs)
 
     for name in alias:
         ALL_OBJECTS_DICT[name] = obs
 
 
-def parse(name: str | None, **kwargs) -> Observable | None:
+def parse_observable(name: str | None, **kwargs) -> Observable | None:
     if name is None or (isinstance(name, str) and name == "None"):
         return
 
     if (class_name := name.split(".")[-1]) in ALL_OBJECTS_DICT:
         kwargs["class_name"] = class_name
         return ALL_OBJECTS_DICT[class_name].from_name(name, **kwargs)
```

### Comparing `hep_ml_lab-0.4.0/hml/observables/angular_distance.py` & `hep_ml_lab-0.4.1/hml/observables/angular_distance.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.0/hml/observables/invariant_mass.py` & `hep_ml_lab-0.4.1/hml/observables/invariant_mass.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from functools import reduce
 
 import awkward as ak
 import vector
 
 from hml.physics_objects.physics_object import PhysicsObject
 
+from ..operations import branch_to_momentum4d
 from .observable import Observable
-from .observable_utils import branches_to_momentum4d
 
 vector.register_awkward()
 
 
 class InvariantMass(Observable):
     def __init__(
         self,
@@ -23,15 +23,15 @@
         super().__init__(physics_object, class_name, supported_objects)
 
     def read(self, events):
         all_keys = {i.lower(): i for i in events.keys(full_paths=False)}
 
         momenta = []
         for obj in self.physics_object.all:
-            momentum4d = branches_to_momentum4d(events, all_keys[obj.branch.lower()])
+            momentum4d = branch_to_momentum4d(events, all_keys[obj.branch.lower()])
             padded_momentum4d = ak.pad_none(momentum4d[:, obj.slices[0]], 1)
             momenta.append(padded_momentum4d)
 
         total = reduce(lambda x, y: x + y, momenta)
         self._value = total.mass
 
         return self
```

### Comparing `hep_ml_lab-0.4.0/hml/observables/kinematics.py` & `hep_ml_lab-0.4.1/hml/observables/kinematics.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.0/hml/observables/n_subjettiness.py` & `hep_ml_lab-0.4.1/hml/observables/n_subjettiness.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.0/hml/observables/observable.py` & `hep_ml_lab-0.4.1/hml/observables/observable.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import awkward as ak
 
+from ..operations import branch_to_momentum4d, constituents_to_momentum4d
 from ..physics_objects import PhysicsObject, is_collective, is_multiple, is_single
-from ..physics_objects import parse as parse_object
-from .observable_utils import branches_to_momentum4d, get_constituents
+from ..physics_objects import parse_physics_object as parse_object
 
 
 class Observable:
     def __init__(
         self,
         physics_object: str | PhysicsObject | None = None,
         class_name: str | None = None,
@@ -126,19 +126,19 @@
 
         if is_single(self.physics_object) or is_collective(self.physics_object):
             if f"{branch}.{self.class_name.lower()}" in all_keys:
                 key = all_keys[f"{branch}.{self.class_name.lower()}"]
                 value = events[key].array()
 
             else:
-                array = branches_to_momentum4d(events, all_keys[branch])
+                array = branch_to_momentum4d(events, all_keys[branch])
                 value = getattr(array, self.class_name.lower())
 
         else:
-            array = get_constituents(events, all_keys[branch])
+            array = constituents_to_momentum4d(events, all_keys[branch])
             value = getattr(array, self.class_name.lower())
 
         if len(slices) == 1:
             value = value[:, slices[0]]
         else:
             value = value[:, slices[0], slices[1]]
```

### Comparing `hep_ml_lab-0.4.0/hml/observables/size.py` & `hep_ml_lab-0.4.1/hml/observables/size.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.0/hml/observables/tag.py` & `hep_ml_lab-0.4.1/hml/observables/tag.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.0/hml/operations/fastjet_ops.py` & `hep_ml_lab-0.4.1/hml/operations/fastjet_ops.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.0/hml/operations/keras_ops.py` & `hep_ml_lab-0.4.1/hml/operations/keras_ops.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.0/hml/operations/uproot_ops.py` & `hep_ml_lab-0.4.1/hml/operations/uproot_ops.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.0/hml/physics_objects/__init__.py` & `hep_ml_lab-0.4.1/hml/physics_objects/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 def get(identifier: str) -> PhysicsObject | None:
     """Retrieve a physics object class from its identifier"""
     return ALL_OBJECTS_DICT.get(identifier)
 
 
-def parse(name: str) -> PhysicsObject:
+def parse_physics_object(name: str) -> PhysicsObject:
     """Parse a name to create a physics object"""
     if is_single(name):
         return Single.from_name(name)
 
     elif is_collective(name):
         return Collective.from_name(name)
```

### Comparing `hep_ml_lab-0.4.0/hml/physics_objects/collective.py` & `hep_ml_lab-0.4.1/hml/physics_objects/collective.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.0/hml/physics_objects/multiple.py` & `hep_ml_lab-0.4.1/hml/physics_objects/multiple.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.0/hml/physics_objects/nested.py` & `hep_ml_lab-0.4.1/hml/physics_objects/nested.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.0/hml/physics_objects/physics_object.py` & `hep_ml_lab-0.4.1/hml/physics_objects/physics_object.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.0/hml/physics_objects/single.py` & `hep_ml_lab-0.4.1/hml/physics_objects/single.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.0/hml/representations/image.py` & `hep_ml_lab-0.4.1/hml/representations/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,27 +5,29 @@
 import awkward as ak
 import matplotlib.pyplot as plt
 import numba as nb
 import numpy as np
 import vector
 from fastjet import ClusterSequence, JetDefinition
 
-from hml.observables import parse
+from hml.observables import parse_observable
 from hml.operations import get_jet_algorithm
 
 vector.register_awkward()
 
 
 class Image:
     def __init__(self, height, width, channel=None):
-        self.height = parse(height) if isinstance(height, str) else height
-        self.width = parse(width) if isinstance(width, str) else width
+        self.height = parse_observable(height) if isinstance(height, str) else height
+        self.width = parse_observable(width) if isinstance(width, str) else width
 
         if channel is not None:
-            self.channel = parse(channel) if isinstance(channel, str) else channel
+            self.channel = (
+                parse_observable(channel) if isinstance(channel, str) else channel
+            )
         else:
             self.channel = None
 
         self.been_pixelated = None
         self.been_read = False
         self.registered_methods = []
         self.recorded_operations = []
@@ -50,18 +52,18 @@
         for method, kwargs in self.registered_methods:
             getattr(self, method)(**kwargs)
 
         return self
 
     def with_subjets(self, constituents, algorithm, r, min_pt):
         if self.been_read:
-            px = parse(f"{constituents}.Px").read(self.event).value
-            py = parse(f"{constituents}.Py").read(self.event).value
-            pz = parse(f"{constituents}.Pz").read(self.event).value
-            e = parse(f"{constituents}.E").read(self.event).value
+            px = parse_observable(f"{constituents}.Px").read(self.event).value
+            py = parse_observable(f"{constituents}.Py").read(self.event).value
+            pz = parse_observable(f"{constituents}.Pz").read(self.event).value
+            e = parse_observable(f"{constituents}.E").read(self.event).value
 
             px = ak.flatten(px, -1)
             py = ak.flatten(py, -1)
             pz = ak.flatten(pz, -1)
             e = ak.flatten(e, -1)
 
             particles = ak.zip(
@@ -95,16 +97,18 @@
                 )
             )
 
         return self
 
     def translate(self, origin="SubJet0"):
         if self.been_read:
-            origin_height = parse(f"{origin}.{self.height.__class__.__name__}")
-            origin_width = parse(f"{origin}.{self.width.__class__.__name__}")
+            origin_height = parse_observable(
+                f"{origin}.{self.height.__class__.__name__}"
+            )
+            origin_width = parse_observable(f"{origin}.{self.width.__class__.__name__}")
 
             obj = origin_height.physics_object.branch
             index = origin_height.physics_object.index
 
             if obj != "SubJet":
                 raise ValueError(f"{obj} is not supported yet!")
 
@@ -148,16 +152,16 @@
         else:
             self.registered_methods.append(("translate", {"origin": origin}))
 
         return self
 
     def rotate(self, axis="SubJet1", orientation=-90):
         if self.been_read:
-            axis_height = parse(f"{axis}.{self.height.__class__.__name__}")
-            axis_width = parse(f"{axis}.{self.width.__class__.__name__}")
+            axis_height = parse_observable(f"{axis}.{self.height.__class__.__name__}")
+            axis_width = parse_observable(f"{axis}.{self.width.__class__.__name__}")
 
             obj = axis_height.physics_object.branch
             index = axis_height.physics_object.index
 
             if obj != "SubJet":
                 raise ValueError(f"{obj} is not supported yet!")
```

### Comparing `hep_ml_lab-0.4.0/hml/representations/set.py` & `hep_ml_lab-0.4.1/hml/representations/set.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 from importlib import import_module
 
 import awkward as ak
-import numpy as np
 
-from hml.observables import ALL_OBJECTS_DICT, Observable, parse
+from hml.observables import Observable, parse_observable
 
 
 class Set:
     """A set of observables.
 
     Set is a 1D representation of an event. It contains a list of observables.
     It is usually used as input to approaches like CutAndCount and
@@ -25,15 +24,15 @@
         self.observables = self._init_observables(observables)
         self._values = None
 
     def _init_observables(self, observables: list[str | Observable]):
         output = []
         for obs in observables:
             if isinstance(obs, str):
-                output.append(parse(obs))
+                output.append(parse_observable(obs))
             else:
                 output.append(obs)
 
         return output
 
     def read(self, events):
         values = []
```

### Comparing `hep_ml_lab-0.4.0/pyproject.toml` & `hep_ml_lab-0.4.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 [tool.poetry]
 name = "hep-ml-lab"
-version = "0.4.0"
+version = "0.4.1"
 description = "An end-to-end framework used for research combining high-energy physics phenomenology with machine learning."
 license = "MIT"
 authors = ["Star9daisy <star9daisy@outlook.com>"]
 readme = "README.md"
-repository = "https://github.com/Star9daisy/hep-ml-lab"
+homepage = "https://github.com/Star9daisy/hep-ml-lab"
 documentation = "https://star9daisy.github.io/hep-ml-lab/"
 keywords = ["high energy physics", "machine learning", "framework"]
 
 packages = [{ include = "hml" }]
 
 [tool.poetry.dependencies]
 dill = "^0.3.7"
 numpy = "^1.22"
 pandas = "2.0.3"
 python = ">=3.9,<3.12"
 rich = "^13.4.2"
 scikit-learn = "^1.2.2"
-tensorflow = "^2.14.0"
 beautifulsoup4 = "^4.12.2"
 pexpect = "^4.9.0"
 awkward = "^2.5.1"
 fastjet = "^3.4.1.3"
 matplotlib = "^3.8.2"
 vector = "^1.3.0"
 numba = "^0.59.0"
-keras = ">=3.0.4"
+keras = ">=3.0.0"
 
 [tool.poetry.group.dev.dependencies]
 deptry = "^0.12.0"
 mkdocs = "^1.4.3"
 mkdocs-exclude = "^1.0.2"
 mkdocs-material = "^9.1.15"
 mkdocstrings = { extras = ["python"], version = "^0.22.0" }
```

### Comparing `hep_ml_lab-0.4.0/PKG-INFO` & `hep_ml_lab-0.4.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hep-ml-lab
-Version: 0.4.0
+Version: 0.4.1
 Summary: An end-to-end framework used for research combining high-energy physics phenomenology with machine learning.
 Home-page: https://github.com/Star9daisy/hep-ml-lab
 License: MIT
 Keywords: high energy physics,machine learning,framework
 Author: Star9daisy
 Author-email: star9daisy@outlook.com
 Requires-Python: >=3.9,<3.12
@@ -13,26 +13,24 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: awkward (>=2.5.1,<3.0.0)
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: dill (>=0.3.7,<0.4.0)
 Requires-Dist: fastjet (>=3.4.1.3,<4.0.0.0)
-Requires-Dist: keras (>=3.0.4)
+Requires-Dist: keras (>=3.0.0)
 Requires-Dist: matplotlib (>=3.8.2,<4.0.0)
 Requires-Dist: numba (>=0.59.0,<0.60.0)
 Requires-Dist: numpy (>=1.22,<2.0)
 Requires-Dist: pandas (==2.0.3)
 Requires-Dist: pexpect (>=4.9.0,<5.0.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
-Requires-Dist: tensorflow (>=2.14.0,<3.0.0)
 Requires-Dist: vector (>=1.3.0,<2.0.0)
 Project-URL: Documentation, https://star9daisy.github.io/hep-ml-lab/
-Project-URL: Repository, https://github.com/Star9daisy/hep-ml-lab
 Description-Content-Type: text/markdown
 
 # HEP ML Lab (HML)
 [![PyPI - Version](https://img.shields.io/pypi/v/hep-ml-lab)](https://pypi.org/project/hep-ml-lab/)
 [![Downloads](https://static.pepy.tech/badge/hep-ml-lab)](https://pepy.tech/project/hep-ml-lab)
 [![codecov](https://codecov.io/gh/Star9daisy/hep-ml-lab/branch/main/graph/badge.svg?token=6VWJi5ct6c)](https://app.codecov.io/gh/Star9daisy/hep-ml-lab)
 [![GitHub](https://img.shields.io/github/license/star9daisy/hep-ml-lab)](https://github.com/Star9daisy/hep-ml-lab/blob/main/LICENSE)
@@ -50,28 +48,37 @@
 To get started, please check out the [documents](https://star9daisy.github.io/hep-ml-lab/).
 
 ## Installation
 ```python
 pip install hep-ml-lab
 ```
 
+Check out the [install via pip](install/pip.md) for more details of prerequisites and post-installation steps or [install via Docker](install/docker.md) for a hassle-free experience.
+
 ## Module overview
 
-![module_overview](docs/images/module_overview.svg)
+![module_overview](docs/images/hml_modules.png)
 
 - `hml.generators`: API of Madgraph5 for simulating colliding events;
 - `hml.physics_objects`: Physics objects classfied by their counts;
 - `hml.observables`: General observables in jet physics;
 - `hml.representations`: Different data structure used to represent an event;
 - `hml.datasets`: Existing datasets and helper classes for creating new datasets;
 - `hml.approaches`: Cuts, trees and networks for classification;
 - `hml.metrics`: Metrics used in classical signal vs background analysis;
 
 ## Updates
 
+### v0.4.1
+- Fix module overview image in README.
+- Fix `GradientBoostedDecisionTree` to be compatible with different `sklearn` versions.
+- Fix `hml.datasets.SetDataset.show` to display the correct rows and columns.
+- Rename the `parse` and `register` functions to `parse_physics_object`, `parse_observable`, and `register_observable`.
+- Update the installation document.
+
 ### v0.4.0
 This version refactors most of the codebase to make it compatible with the array
 (from `awkward` and `uproot`) representation of the data.
 
 ### v0.3.0.1
 - Fix a bug that Madgraph5 may run into an infinite loop caused by HML keeping
   removing py.py file during initialization.
```

