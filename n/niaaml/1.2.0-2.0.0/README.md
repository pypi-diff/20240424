# Comparing `tmp/niaaml-1.2.0.tar.gz` & `tmp/niaaml-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niaaml-1.2.0.tar", max compression
+gzip compressed data, was "niaaml-2.0.0.tar", max compression
```

## Comparing `niaaml-1.2.0.tar` & `niaaml-2.0.0.tar`

### file list

```diff
@@ -1,68 +1,76 @@
--rw-r--r--   0        0        0    14048 2024-02-16 13:06:58.000634 niaaml-1.2.0/CHANGELOG.md
--rw-r--r--   0        0        0      395 2024-02-16 13:06:58.000634 niaaml-1.2.0/CITATION.md
--rw-r--r--   0        0        0     1368 2024-02-16 13:06:58.000634 niaaml-1.2.0/COMPONENTS.md
--rw-r--r--   0        0        0     1069 2024-02-16 13:06:58.001634 niaaml-1.2.0/LICENSE
--rw-r--r--   0        0        0     5268 2024-02-16 13:06:58.001634 niaaml-1.2.0/README.rst
--rw-r--r--   0        0        0      819 2024-02-16 13:06:58.004634 niaaml-1.2.0/niaaml/__init__.py
--rw-r--r--   0        0        0     1119 2024-02-16 13:06:58.004634 niaaml-1.2.0/niaaml/classifiers/__init__.py
--rw-r--r--   0        0        0     2835 2024-02-16 13:06:58.004634 niaaml-1.2.0/niaaml/classifiers/ada_boost.py
--rw-r--r--   0        0        0     2914 2024-02-16 13:06:58.004634 niaaml-1.2.0/niaaml/classifiers/bagging.py
--rw-r--r--   0        0        0      894 2024-02-16 13:06:58.004634 niaaml-1.2.0/niaaml/classifiers/classifier.py
--rw-r--r--   0        0        0     2959 2024-02-16 13:06:58.004634 niaaml-1.2.0/niaaml/classifiers/decision_tree.py
--rw-r--r--   0        0        0     2955 2024-02-16 13:06:58.004634 niaaml-1.2.0/niaaml/classifiers/extremely_randomized_trees.py
--rw-r--r--   0        0        0     2609 2024-02-16 13:06:58.004634 niaaml-1.2.0/niaaml/classifiers/gaussian_naive_bayes.py
--rw-r--r--   0        0        0     3084 2024-02-16 13:06:58.004634 niaaml-1.2.0/niaaml/classifiers/gaussian_process.py
--rw-r--r--   0        0        0     2914 2024-02-16 13:06:58.005634 niaaml-1.2.0/niaaml/classifiers/k_neighbors.py
--rw-r--r--   0        0        0     2915 2024-02-16 13:06:58.005634 niaaml-1.2.0/niaaml/classifiers/linear_svc.py
--rw-r--r--   0        0        0     3107 2024-02-16 13:06:58.005634 niaaml-1.2.0/niaaml/classifiers/multi_layer_perceptron.py
--rw-r--r--   0        0        0     2814 2024-02-16 13:06:58.005634 niaaml-1.2.0/niaaml/classifiers/quadratic_driscriminant_analysis.py
--rw-r--r--   0        0        0     2902 2024-02-16 13:06:58.005634 niaaml-1.2.0/niaaml/classifiers/random_forest.py
--rw-r--r--   0        0        0     1761 2024-02-16 13:06:58.005634 niaaml-1.2.0/niaaml/classifiers/utility.py
--rw-r--r--   0        0        0      221 2024-02-16 13:06:58.005634 niaaml-1.2.0/niaaml/data/__init__.py
--rw-r--r--   0        0        0      743 2024-02-16 13:06:58.005634 niaaml-1.2.0/niaaml/data/basic_data_reader.py
--rw-r--r--   0        0        0     1460 2024-02-16 13:06:58.005634 niaaml-1.2.0/niaaml/data/csv_data_reader.py
--rw-r--r--   0        0        0     1391 2024-02-16 13:06:58.005634 niaaml-1.2.0/niaaml/data/data_reader.py
--rw-r--r--   0        0        0      406 2024-02-16 13:06:58.005634 niaaml-1.2.0/niaaml/fitness/__init__.py
--rw-r--r--   0        0        0      977 2024-02-16 13:06:58.005634 niaaml-1.2.0/niaaml/fitness/accuracy.py
--rw-r--r--   0        0        0     1000 2024-02-16 13:06:58.005634 niaaml-1.2.0/niaaml/fitness/cohen_kappa.py
--rw-r--r--   0        0        0      966 2024-02-16 13:06:58.005634 niaaml-1.2.0/niaaml/fitness/f1.py
--rw-r--r--   0        0        0      952 2024-02-16 13:06:58.005634 niaaml-1.2.0/niaaml/fitness/fitness_function.py
--rw-r--r--   0        0        0     1004 2024-02-16 13:06:58.005634 niaaml-1.2.0/niaaml/fitness/precision.py
--rw-r--r--   0        0        0      762 2024-02-16 13:06:58.005634 niaaml-1.2.0/niaaml/fitness/utility.py
--rw-r--r--   0        0        0     1451 2024-02-16 13:06:58.005634 niaaml-1.2.0/niaaml/logger.py
--rw-r--r--   0        0        0    21985 2024-02-16 13:06:58.005634 niaaml-1.2.0/niaaml/pipeline.py
--rw-r--r--   0        0        0     1903 2024-02-16 13:06:58.005634 niaaml-1.2.0/niaaml/pipeline_component.py
--rw-r--r--   0        0        0    21156 2024-02-16 13:06:58.006634 niaaml-1.2.0/niaaml/pipeline_optimizer.py
--rw-r--r--   0        0        0      397 2024-02-16 13:06:58.006634 niaaml-1.2.0/niaaml/preprocessing/__init__.py
--rw-r--r--   0        0        0      403 2024-02-16 13:06:58.006634 niaaml-1.2.0/niaaml/preprocessing/encoding/__init__.py
--rw-r--r--   0        0        0     1097 2024-02-16 13:06:58.006634 niaaml-1.2.0/niaaml/preprocessing/encoding/feature_encoder.py
--rw-r--r--   0        0        0     1745 2024-02-16 13:06:58.006634 niaaml-1.2.0/niaaml/preprocessing/encoding/one_hot_encoder.py
--rw-r--r--   0        0        0     1667 2024-02-16 13:06:58.006634 niaaml-1.2.0/niaaml/preprocessing/encoding/utility.py
--rw-r--r--   0        0        0     1369 2024-02-16 13:06:58.006634 niaaml-1.2.0/niaaml/preprocessing/feature_selection/__init__.py
--rw-r--r--   0        0        0     2022 2024-02-16 13:06:58.006634 niaaml-1.2.0/niaaml/preprocessing/feature_selection/_feature_selection_threshold_problem.py
--rw-r--r--   0        0        0     3345 2024-02-16 13:06:58.006634 niaaml-1.2.0/niaaml/preprocessing/feature_selection/bat_algorithm.py
--rw-r--r--   0        0        0     3229 2024-02-16 13:06:58.006634 niaaml-1.2.0/niaaml/preprocessing/feature_selection/differential_evolution.py
--rw-r--r--   0        0        0      805 2024-02-16 13:06:58.006634 niaaml-1.2.0/niaaml/preprocessing/feature_selection/feature_selection_algorithm.py
--rw-r--r--   0        0        0     2787 2024-02-16 13:06:58.006634 niaaml-1.2.0/niaaml/preprocessing/feature_selection/grey_wolf_optimizer.py
--rw-r--r--   0        0        0     2963 2024-02-16 13:06:58.006634 niaaml-1.2.0/niaaml/preprocessing/feature_selection/jDEFSTH.py
--rw-r--r--   0        0        0     3219 2024-02-16 13:06:58.006634 niaaml-1.2.0/niaaml/preprocessing/feature_selection/particle_swarm_optimization.py
--rw-r--r--   0        0        0     2608 2024-02-16 13:06:58.006634 niaaml-1.2.0/niaaml/preprocessing/feature_selection/select_k_best.py
--rw-r--r--   0        0        0     2216 2024-02-16 13:06:58.006634 niaaml-1.2.0/niaaml/preprocessing/feature_selection/select_percentile.py
--rw-r--r--   0        0        0     1639 2024-02-16 13:06:58.006634 niaaml-1.2.0/niaaml/preprocessing/feature_selection/utility.py
--rw-r--r--   0        0        0     1994 2024-02-16 13:06:58.006634 niaaml-1.2.0/niaaml/preprocessing/feature_selection/variance_threshold.py
--rw-r--r--   0        0        0      823 2024-02-16 13:06:58.007634 niaaml-1.2.0/niaaml/preprocessing/feature_transform/__init__.py
--rw-r--r--   0        0        0      930 2024-02-16 13:06:58.007634 niaaml-1.2.0/niaaml/preprocessing/feature_transform/feature_transform_algorithm.py
--rw-r--r--   0        0        0     1762 2024-02-16 13:06:58.007634 niaaml-1.2.0/niaaml/preprocessing/feature_transform/max_abs_scaler.py
--rw-r--r--   0        0        0     1944 2024-02-16 13:06:58.007634 niaaml-1.2.0/niaaml/preprocessing/feature_transform/normalizer.py
--rw-r--r--   0        0        0     1957 2024-02-16 13:06:58.007634 niaaml-1.2.0/niaaml/preprocessing/feature_transform/quantile_transformer.py
--rw-r--r--   0        0        0     1885 2024-02-16 13:06:58.007634 niaaml-1.2.0/niaaml/preprocessing/feature_transform/robust_scaler.py
--rw-r--r--   0        0        0     1716 2024-02-16 13:06:58.007634 niaaml-1.2.0/niaaml/preprocessing/feature_transform/standard_scaler.py
--rw-r--r--   0        0        0     1117 2024-02-16 13:06:58.007634 niaaml-1.2.0/niaaml/preprocessing/feature_transform/utility.py
--rw-r--r--   0        0        0      345 2024-02-16 13:06:58.007634 niaaml-1.2.0/niaaml/preprocessing/imputation/__init__.py
--rw-r--r--   0        0        0     1023 2024-02-16 13:06:58.007634 niaaml-1.2.0/niaaml/preprocessing/imputation/imputer.py
--rw-r--r--   0        0        0     1788 2024-02-16 13:06:58.007634 niaaml-1.2.0/niaaml/preprocessing/imputation/simple_imputer.py
--rw-r--r--   0        0        0     1342 2024-02-16 13:06:58.007634 niaaml-1.2.0/niaaml/preprocessing/imputation/utility.py
--rw-r--r--   0        0        0      372 2024-02-16 13:06:58.007634 niaaml-1.2.0/niaaml/preprocessing/preprocessing_algorithm.py
--rw-r--r--   0        0        0     4808 2024-02-16 13:06:58.008634 niaaml-1.2.0/niaaml/utilities.py
--rw-r--r--   0        0        0     1063 2024-02-16 13:06:58.009634 niaaml-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     6134 1970-01-01 00:00:00.000000 niaaml-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    14048 2024-04-24 07:16:54.422507 niaaml-2.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0      395 2024-04-24 07:16:54.422507 niaaml-2.0.0/CITATION.md
+-rw-r--r--   0        0        0     1368 2024-04-24 07:16:54.422507 niaaml-2.0.0/COMPONENTS.md
+-rw-r--r--   0        0        0     1069 2024-04-24 07:16:54.422507 niaaml-2.0.0/LICENSE
+-rw-r--r--   0        0        0    22558 2024-04-24 07:16:54.422507 niaaml-2.0.0/README.md
+-rw-r--r--   0        0        0      819 2024-04-24 07:16:54.426507 niaaml-2.0.0/niaaml/__init__.py
+-rw-r--r--   0        0        0     1616 2024-04-24 07:16:54.426507 niaaml-2.0.0/niaaml/classifiers/__init__.py
+-rw-r--r--   0        0        0     2835 2024-04-24 07:16:54.426507 niaaml-2.0.0/niaaml/classifiers/ada_boost.py
+-rw-r--r--   0        0        0     2914 2024-04-24 07:16:54.426507 niaaml-2.0.0/niaaml/classifiers/bagging.py
+-rw-r--r--   0        0        0      894 2024-04-24 07:16:54.426507 niaaml-2.0.0/niaaml/classifiers/classifier.py
+-rw-r--r--   0        0        0     2959 2024-04-24 07:16:54.426507 niaaml-2.0.0/niaaml/classifiers/decision_tree.py
+-rw-r--r--   0        0        0     2955 2024-04-24 07:16:54.426507 niaaml-2.0.0/niaaml/classifiers/extremely_randomized_trees.py
+-rw-r--r--   0        0        0     2609 2024-04-24 07:16:54.426507 niaaml-2.0.0/niaaml/classifiers/gaussian_naive_bayes.py
+-rw-r--r--   0        0        0     3084 2024-04-24 07:16:54.427507 niaaml-2.0.0/niaaml/classifiers/gaussian_process.py
+-rw-r--r--   0        0        0     2914 2024-04-24 07:16:54.427507 niaaml-2.0.0/niaaml/classifiers/k_neighbors.py
+-rw-r--r--   0        0        0     2915 2024-04-24 07:16:54.427507 niaaml-2.0.0/niaaml/classifiers/linear_svc.py
+-rw-r--r--   0        0        0     3107 2024-04-24 07:16:54.427507 niaaml-2.0.0/niaaml/classifiers/multi_layer_perceptron.py
+-rw-r--r--   0        0        0     2814 2024-04-24 07:16:54.427507 niaaml-2.0.0/niaaml/classifiers/quadratic_driscriminant_analysis.py
+-rw-r--r--   0        0        0     2902 2024-04-24 07:16:54.427507 niaaml-2.0.0/niaaml/classifiers/random_forest.py
+-rw-r--r--   0        0        0     2813 2024-04-24 07:16:54.427507 niaaml-2.0.0/niaaml/classifiers/regression_decision_tree.py
+-rw-r--r--   0        0        0     2747 2024-04-24 07:16:54.427507 niaaml-2.0.0/niaaml/classifiers/regression_gaussian_process.py
+-rw-r--r--   0        0        0     2819 2024-04-24 07:16:54.427507 niaaml-2.0.0/niaaml/classifiers/regression_lasso.py
+-rw-r--r--   0        0        0     2666 2024-04-24 07:16:54.427507 niaaml-2.0.0/niaaml/classifiers/regression_linear_model.py
+-rw-r--r--   0        0        0     2823 2024-04-24 07:16:54.427507 niaaml-2.0.0/niaaml/classifiers/regression_ridge.py
+-rw-r--r--   0        0        0     2401 2024-04-24 07:16:54.427507 niaaml-2.0.0/niaaml/classifiers/utility.py
+-rw-r--r--   0        0        0      221 2024-04-24 07:16:54.427507 niaaml-2.0.0/niaaml/data/__init__.py
+-rw-r--r--   0        0        0      743 2024-04-24 07:16:54.427507 niaaml-2.0.0/niaaml/data/basic_data_reader.py
+-rw-r--r--   0        0        0     1727 2024-04-24 07:16:54.427507 niaaml-2.0.0/niaaml/data/csv_data_reader.py
+-rw-r--r--   0        0        0     1391 2024-04-24 07:16:54.427507 niaaml-2.0.0/niaaml/data/data_reader.py
+-rw-r--r--   0        0        0      495 2024-04-24 07:16:54.427507 niaaml-2.0.0/niaaml/fitness/__init__.py
+-rw-r--r--   0        0        0      977 2024-04-24 07:16:54.427507 niaaml-2.0.0/niaaml/fitness/accuracy.py
+-rw-r--r--   0        0        0     1000 2024-04-24 07:16:54.427507 niaaml-2.0.0/niaaml/fitness/cohen_kappa.py
+-rw-r--r--   0        0        0      966 2024-04-24 07:16:54.427507 niaaml-2.0.0/niaaml/fitness/f1.py
+-rw-r--r--   0        0        0     1261 2024-04-24 07:16:54.427507 niaaml-2.0.0/niaaml/fitness/fitness_function.py
+-rw-r--r--   0        0        0     1218 2024-04-24 07:16:54.427507 niaaml-2.0.0/niaaml/fitness/mse.py
+-rw-r--r--   0        0        0     1004 2024-04-24 07:16:54.427507 niaaml-2.0.0/niaaml/fitness/precision.py
+-rw-r--r--   0        0        0     1140 2024-04-24 07:16:54.427507 niaaml-2.0.0/niaaml/fitness/r2.py
+-rw-r--r--   0        0        0      876 2024-04-24 07:16:54.427507 niaaml-2.0.0/niaaml/fitness/utility.py
+-rw-r--r--   0        0        0     1451 2024-04-24 07:16:54.428507 niaaml-2.0.0/niaaml/logger.py
+-rw-r--r--   0        0        0    22867 2024-04-24 07:16:54.428507 niaaml-2.0.0/niaaml/pipeline.py
+-rw-r--r--   0        0        0     1903 2024-04-24 07:16:54.428507 niaaml-2.0.0/niaaml/pipeline_component.py
+-rw-r--r--   0        0        0    21156 2024-04-24 07:16:54.428507 niaaml-2.0.0/niaaml/pipeline_optimizer.py
+-rw-r--r--   0        0        0      397 2024-04-24 07:16:54.428507 niaaml-2.0.0/niaaml/preprocessing/__init__.py
+-rw-r--r--   0        0        0      403 2024-04-24 07:16:54.428507 niaaml-2.0.0/niaaml/preprocessing/encoding/__init__.py
+-rw-r--r--   0        0        0     1097 2024-04-24 07:16:54.428507 niaaml-2.0.0/niaaml/preprocessing/encoding/feature_encoder.py
+-rw-r--r--   0        0        0     1745 2024-04-24 07:16:54.428507 niaaml-2.0.0/niaaml/preprocessing/encoding/one_hot_encoder.py
+-rw-r--r--   0        0        0     1667 2024-04-24 07:16:54.428507 niaaml-2.0.0/niaaml/preprocessing/encoding/utility.py
+-rw-r--r--   0        0        0     1511 2024-04-24 07:16:54.428507 niaaml-2.0.0/niaaml/preprocessing/feature_selection/__init__.py
+-rw-r--r--   0        0        0     2022 2024-04-24 07:16:54.428507 niaaml-2.0.0/niaaml/preprocessing/feature_selection/_feature_selection_threshold_problem.py
+-rw-r--r--   0        0        0     3345 2024-04-24 07:16:54.428507 niaaml-2.0.0/niaaml/preprocessing/feature_selection/bat_algorithm.py
+-rw-r--r--   0        0        0     3229 2024-04-24 07:16:54.428507 niaaml-2.0.0/niaaml/preprocessing/feature_selection/differential_evolution.py
+-rw-r--r--   0        0        0      805 2024-04-24 07:16:54.428507 niaaml-2.0.0/niaaml/preprocessing/feature_selection/feature_selection_algorithm.py
+-rw-r--r--   0        0        0     2787 2024-04-24 07:16:54.428507 niaaml-2.0.0/niaaml/preprocessing/feature_selection/grey_wolf_optimizer.py
+-rw-r--r--   0        0        0     2963 2024-04-24 07:16:54.428507 niaaml-2.0.0/niaaml/preprocessing/feature_selection/jDEFSTH.py
+-rw-r--r--   0        0        0     3219 2024-04-24 07:16:54.428507 niaaml-2.0.0/niaaml/preprocessing/feature_selection/particle_swarm_optimization.py
+-rw-r--r--   0        0        0     2608 2024-04-24 07:16:54.429507 niaaml-2.0.0/niaaml/preprocessing/feature_selection/select_k_best.py
+-rw-r--r--   0        0        0     2216 2024-04-24 07:16:54.429507 niaaml-2.0.0/niaaml/preprocessing/feature_selection/select_percentile.py
+-rw-r--r--   0        0        0     2086 2024-04-24 07:16:54.429507 niaaml-2.0.0/niaaml/preprocessing/feature_selection/select_univariate_regression.py
+-rw-r--r--   0        0        0     1816 2024-04-24 07:16:54.429507 niaaml-2.0.0/niaaml/preprocessing/feature_selection/utility.py
+-rw-r--r--   0        0        0     1994 2024-04-24 07:16:54.429507 niaaml-2.0.0/niaaml/preprocessing/feature_selection/variance_threshold.py
+-rw-r--r--   0        0        0      823 2024-04-24 07:16:54.429507 niaaml-2.0.0/niaaml/preprocessing/feature_transform/__init__.py
+-rw-r--r--   0        0        0      930 2024-04-24 07:16:54.429507 niaaml-2.0.0/niaaml/preprocessing/feature_transform/feature_transform_algorithm.py
+-rw-r--r--   0        0        0     1762 2024-04-24 07:16:54.429507 niaaml-2.0.0/niaaml/preprocessing/feature_transform/max_abs_scaler.py
+-rw-r--r--   0        0        0     1944 2024-04-24 07:16:54.429507 niaaml-2.0.0/niaaml/preprocessing/feature_transform/normalizer.py
+-rw-r--r--   0        0        0     1957 2024-04-24 07:16:54.429507 niaaml-2.0.0/niaaml/preprocessing/feature_transform/quantile_transformer.py
+-rw-r--r--   0        0        0     1885 2024-04-24 07:16:54.429507 niaaml-2.0.0/niaaml/preprocessing/feature_transform/robust_scaler.py
+-rw-r--r--   0        0        0     1716 2024-04-24 07:16:54.429507 niaaml-2.0.0/niaaml/preprocessing/feature_transform/standard_scaler.py
+-rw-r--r--   0        0        0     1117 2024-04-24 07:16:54.429507 niaaml-2.0.0/niaaml/preprocessing/feature_transform/utility.py
+-rw-r--r--   0        0        0      345 2024-04-24 07:16:54.429507 niaaml-2.0.0/niaaml/preprocessing/imputation/__init__.py
+-rw-r--r--   0        0        0     1023 2024-04-24 07:16:54.429507 niaaml-2.0.0/niaaml/preprocessing/imputation/imputer.py
+-rw-r--r--   0        0        0     1788 2024-04-24 07:16:54.429507 niaaml-2.0.0/niaaml/preprocessing/imputation/simple_imputer.py
+-rw-r--r--   0        0        0     1342 2024-04-24 07:16:54.429507 niaaml-2.0.0/niaaml/preprocessing/imputation/utility.py
+-rw-r--r--   0        0        0      372 2024-04-24 07:16:54.429507 niaaml-2.0.0/niaaml/preprocessing/preprocessing_algorithm.py
+-rw-r--r--   0        0        0     5937 2024-04-24 07:16:54.429507 niaaml-2.0.0/niaaml/utilities.py
+-rw-r--r--   0        0        0     1161 2024-04-24 07:16:54.430507 niaaml-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0    23498 1970-01-01 00:00:00.000000 niaaml-2.0.0/PKG-INFO
```

### Comparing `niaaml-1.2.0/CHANGELOG.md` & `niaaml-2.0.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/COMPONENTS.md` & `niaaml-2.0.0/COMPONENTS.md`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/LICENSE` & `niaaml-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/niaaml/__init__.py` & `niaaml-2.0.0/niaaml/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,8 +25,8 @@
     "PipelineOptimizer",
     "Pipeline",
     "PipelineComponent",
     "Logger",
 ]
 
 __project__ = "niaaml"
-__version__ = "1.2.0"
+__version__ = "2.0.0"
```

### Comparing `niaaml-1.2.0/niaaml/classifiers/__init__.py` & `niaaml-2.0.0/niaaml/classifiers/utility.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,62 @@
-from niaaml.classifiers.classifier import Classifier
-from niaaml.classifiers.random_forest import RandomForest
-from niaaml.classifiers.multi_layer_perceptron import MultiLayerPerceptron
-from niaaml.classifiers.linear_svc import LinearSVC
+from niaaml.classifiers.regression_decision_tree import DecisionTreeRegression
+from niaaml.classifiers.regression_gaussian_process import GaussianProcessRegression
+from niaaml.utilities import Factory
 from niaaml.classifiers.ada_boost import AdaBoost
-from niaaml.classifiers.extremely_randomized_trees import ExtremelyRandomizedTrees
 from niaaml.classifiers.bagging import Bagging
+from niaaml.classifiers.extremely_randomized_trees import ExtremelyRandomizedTrees
+from niaaml.classifiers.linear_svc import LinearSVC
+from niaaml.classifiers.multi_layer_perceptron import MultiLayerPerceptron
+from niaaml.classifiers.random_forest import RandomForest
 from niaaml.classifiers.decision_tree import DecisionTree
 from niaaml.classifiers.k_neighbors import KNeighbors
 from niaaml.classifiers.gaussian_process import GaussianProcess
 from niaaml.classifiers.gaussian_naive_bayes import GaussianNB
 from niaaml.classifiers.quadratic_driscriminant_analysis import (
     QuadraticDiscriminantAnalysis,
 )
-from niaaml.classifiers.utility import ClassifierFactory
+from niaaml.classifiers.regression_linear_model import LinearRegression
+from niaaml.classifiers.regression_ridge import RidgeRegression
+from niaaml.classifiers.regression_lasso import LassoRegression
+
+__all__ = ["ClassifierFactory"]
+
+
+class ClassifierFactory(Factory):
+    r"""Class with string mappings to classifiers.
+
+    Date:
+        2020
+
+    Author:
+        Luka Pečnik
+
+    License:
+        MIT
+
+    Attributes:
+        _entities (Dict[str, Classifier]): Mapping from strings to classifiers.
+
+    See Also:
+        * :class:`niaaml.utilities.Factory`
+    """
 
-__all__ = [
-    "Classifier",
-    "RandomForest",
-    "MultiLayerPerceptron",
-    "LinearSVC",
-    "AdaBoost",
-    "Bagging",
-    "ExtremelyRandomizedTrees",
-    "DecisionTree",
-    "KNeighbors",
-    "GaussianProcess",
-    "GaussianNB",
-    "QuadraticDiscriminantAnalysis",
-    "ClassifierFactory",
-]
+    def _set_parameters(self, **kwargs):
+        r"""Set the parameters/arguments of the factory."""
+        self._entities = {
+            "AdaBoost": AdaBoost,
+            "Bagging": Bagging,
+            "ExtremelyRandomizedTrees": ExtremelyRandomizedTrees,
+            "LinearSVC": LinearSVC,
+            "MultiLayerPerceptron": MultiLayerPerceptron,
+            "RandomForest": RandomForest,
+            "DecisionTree": DecisionTree,
+            "DecisionTreeRegression": DecisionTreeRegression,
+            "KNeighbors": KNeighbors,
+            "GaussianProcess": GaussianProcess,
+            "GaussianProcessRegression": GaussianProcessRegression,
+            "GaussianNB": GaussianNB,
+            "QuadraticDiscriminantAnalysis": QuadraticDiscriminantAnalysis,
+            "LinearRegression": LinearRegression,
+            "RidgeRegression": RidgeRegression,
+            "LassoRegression": LassoRegression,
+        }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `niaaml-1.2.0/niaaml/classifiers/ada_boost.py` & `niaaml-2.0.0/niaaml/classifiers/ada_boost.py`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/niaaml/classifiers/bagging.py` & `niaaml-2.0.0/niaaml/classifiers/bagging.py`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/niaaml/classifiers/classifier.py` & `niaaml-2.0.0/niaaml/classifiers/classifier.py`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/niaaml/classifiers/decision_tree.py` & `niaaml-2.0.0/niaaml/classifiers/decision_tree.py`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/niaaml/classifiers/extremely_randomized_trees.py` & `niaaml-2.0.0/niaaml/classifiers/extremely_randomized_trees.py`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/niaaml/classifiers/gaussian_naive_bayes.py` & `niaaml-2.0.0/niaaml/classifiers/gaussian_naive_bayes.py`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/niaaml/classifiers/gaussian_process.py` & `niaaml-2.0.0/niaaml/classifiers/gaussian_process.py`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/niaaml/classifiers/k_neighbors.py` & `niaaml-2.0.0/niaaml/classifiers/k_neighbors.py`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/niaaml/classifiers/linear_svc.py` & `niaaml-2.0.0/niaaml/classifiers/linear_svc.py`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/niaaml/classifiers/multi_layer_perceptron.py` & `niaaml-2.0.0/niaaml/classifiers/multi_layer_perceptron.py`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/niaaml/classifiers/quadratic_driscriminant_analysis.py` & `niaaml-2.0.0/niaaml/classifiers/quadratic_driscriminant_analysis.py`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/niaaml/classifiers/random_forest.py` & `niaaml-2.0.0/niaaml/classifiers/random_forest.py`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/niaaml/data/basic_data_reader.py` & `niaaml-2.0.0/niaaml/data/basic_data_reader.py`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/niaaml/data/csv_data_reader.py` & `niaaml-2.0.0/niaaml/data/csv_data_reader.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,31 +21,36 @@
         __contains_classes (bool): Tells if src contains expected classification results or only features.
         __has_header (bool): Tells if src contains header row.
 
     See Also:
         * :class:`niaaml.data.DataReader`
     """
 
-    def _set_parameters(self, src, contains_classes=True, has_header=False, **kwargs):
+    def _set_parameters(self, src, contains_classes=True, has_header=False, ignore_columns=[], **kwargs):
         r"""Set the parameters of the algorithm.
 
         Arguments:
             src (string): Path to a CSV dataset file.
             contains_classes (Optional[bool]): Tells if src contains expected classification results or only features.
             has_header (Optional[bool]): Tells if src contains header row.
+            ignore_columns (Optional[List[int]]): Column indices to drop.
         """
         self.__src = src
         self.__contains_classes = contains_classes
         self.__has_header = has_header
+        self.__ignore_columns = ignore_columns
         self._read_data()
 
     def _read_data(self, **kwargs):
         r"""Read data from expected source."""
         data = pd.read_csv(
             self.__src, header=None if self.__has_header is False else "infer"
         )
         header = data.columns
 
         if self.__contains_classes:
             self._y = data.pop(header[len(header) - 1])
+        
+        if len(self.__ignore_columns) > 0:
+            data.drop(header[self.__ignore_columns], axis=1, inplace=True)
 
         self._x = data
```

### Comparing `niaaml-1.2.0/niaaml/data/data_reader.py` & `niaaml-2.0.0/niaaml/data/data_reader.py`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/niaaml/fitness/accuracy.py` & `niaaml-2.0.0/niaaml/fitness/accuracy.py`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/niaaml/fitness/cohen_kappa.py` & `niaaml-2.0.0/niaaml/fitness/cohen_kappa.py`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/niaaml/fitness/f1.py` & `niaaml-2.0.0/niaaml/fitness/f1.py`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/niaaml/fitness/fitness_function.py` & `niaaml-2.0.0/niaaml/fitness/precision.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,37 @@
-__all__ = ["FitnessFunction"]
+from sklearn.metrics import precision_score
+from niaaml.fitness.fitness_function import FitnessFunction
 
+__all__ = ["Precision"]
 
-class FitnessFunction:
-    r"""Class for implementing fitness functions.
+
+class Precision(FitnessFunction):
+    r"""Class representing the precision as a fitness function.
 
     Date:
         2020
 
     Author:
         Luka Pečnik
 
     License:
         MIT
 
-    Attributes:
-        Name (str): Name of the fitness function.
-    """
-    Name = None
+    Documentation:
+        https://scikit-learn.org/stable/modules/generated/sklearn.metrics.precision_score.html
 
-    def __init__(self, **kwargs):
-        r"""Initialize fitness function."""
-        self.set_parameters(**kwargs)
-
-    def set_parameters(self, **kwargs):
-        r"""Set the parameters/arguments of the pipeline component."""
-        return
+    See Also:
+        * :class:`niaaml.fitness.FitnessFunction`
+    """
+    Name = "Precision"
 
     def get_fitness(self, predicted, expected):
         r"""Return fitness value. The larger return value should represent a better fitness for the framework to work properly.
 
         Arguments:
             predicted (pandas.core.series.Series): Predicted values.
             expected (pandas.core.series.Series): Expected values.
 
         Returns:
             float: Calculated fitness value.
         """
-        return None
+        return precision_score(expected, predicted, average="weighted")
```

### Comparing `niaaml-1.2.0/niaaml/fitness/precision.py` & `niaaml-2.0.0/niaaml/fitness/utility.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,31 @@
-from sklearn.metrics import precision_score
-from niaaml.fitness.fitness_function import FitnessFunction
+from niaaml.utilities import Factory
+from niaaml.fitness.accuracy import Accuracy
+from niaaml.fitness.cohen_kappa import CohenKappa
+from niaaml.fitness.precision import Precision
+from niaaml.fitness.f1 import F1
+from niaaml.fitness.r2 import R2
+from niaaml.fitness.mse import MSE
 
-__all__ = ["Precision"]
+__all__ = ["FitnessFactory"]
 
 
-class Precision(FitnessFunction):
-    r"""Class representing the precision as a fitness function.
+class FitnessFactory(Factory):
+    r"""Class with string mappings to fitness class.
 
-    Date:
-        2020
-
-    Author:
-        Luka Pečnik
-
-    License:
-        MIT
-
-    Documentation:
-        https://scikit-learn.org/stable/modules/generated/sklearn.metrics.precision_score.html
+    Attributes:
+        _entities (Dict[str, Fitness]): Mapping from strings to fitness classes.
 
     See Also:
-        * :class:`niaaml.fitness.FitnessFunction`
+        * :class:`niaaml.utilities.Factory`
     """
-    Name = "Precision"
-
-    def get_fitness(self, predicted, expected):
-        r"""Return fitness value. The larger return value should represent a better fitness for the framework to work properly.
 
-        Arguments:
-            predicted (pandas.core.series.Series): Predicted values.
-            expected (pandas.core.series.Series): Expected values.
-
-        Returns:
-            float: Calculated fitness value.
-        """
-        return precision_score(expected, predicted, average="weighted")
+    def _set_parameters(self, **kwargs):
+        r"""Set the parameters/arguments of the factory."""
+        self._entities = {
+            "Accuracy": Accuracy,
+            "Precision": Precision,
+            "CohenKappa": CohenKappa,
+            "F1": F1,
+            "R2": R2,
+            "MSE": MSE,
+        }
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `niaaml-1.2.0/niaaml/logger.py` & `niaaml-2.0.0/niaaml/logger.py`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/niaaml/pipeline.py` & `niaaml-2.0.0/niaaml/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from sklearn.model_selection import train_test_split
-from niaaml.utilities import MinMax, get_bin_index, OptimizationStats
+from niaaml.utilities import MinMax, RegressionOptimizationStats, get_bin_index, OptimizationStats
 from niaaml.fitness import FitnessFactory
 from niapy.problems import Problem
 from niapy.util.factory import get_algorithm
 from niapy.task import Task
 import pandas as pd
 import numpy as np
 import copy
@@ -151,16 +151,16 @@
         number_of_evaluations,
         optimization_algorithm,
         fitness_function,
     ):
         r"""Optimize pipeline's hyperparameters.
 
         Arguments:
-            x (pandas.core.frame.DataFrame): n samples to classify.
-            y (pandas.core.series.Series): n classes of the samples in the x array.
+            x (pandas.core.frame.DataFrame): n input samples.
+            y (pandas.core.series.Series): n classes/targets of the samples in the x array.
             population_size (uint): Number of individuals in the optimization process.
             number_of_evaluations (uint): Number of maximum evaluations.
             optimization_algorithm (str): Name of the optimization algorithm to use.
             fitness_function (str): Name of the fitness function to use.
 
         Returns:
             float: Best fitness value found in optimization process.
@@ -407,17 +407,18 @@
         """
         self.__parent = parent
         self.__x = x
         self.__y = y
         self.__population_size = population_size
         self.__current_best_fitness = np.inf
         self.__fitness_function = FitnessFactory().get_result(fitness_function)
+        self.__lower_bound, self.__upper_bound = self.__fitness_function.get_bounds()
         self.__evals = 0
         self.__logger = self.__parent.get_logger()
-        super().__init__(dimension, 0.0, 1.0)
+        super().__init__(dimension, lower=self.__lower_bound, upper=self.__upper_bound)
 
     @staticmethod
     def evaluate_pipeline(
         solution_vector,
         feature_selection_algorithm,
         feature_transform_algorithm,
         classifier,
@@ -457,42 +458,48 @@
         params_all = [
             (feature_selection_algorithm_params, feature_selection_algorithm),
             (feature_transform_algorithm_params, feature_transform_algorithm),
             (classifier_params, classifier),
         ]
         solution_index = 0
 
-        for i in params_all:
+        # iterate over parameters and components and pass the prepared parameters to `set_parameters`
+        for params, component in params_all:
             args = dict()
-            for key in i[0]:
-                if i[0][key] is not None:
-                    if isinstance(i[0][key].value, MinMax):
+            for key in params:
+                if params[key] is not None:
+                    if isinstance(params[key].value, MinMax):
                         val = (
-                            solution_vector[solution_index] * i[0][key].value.max
-                            + i[0][key].value.min
+                            solution_vector[solution_index] * params[key].value.max
+                            + params[key].value.min
                         )
                         if (
-                            i[0][key].param_type is np.intc
-                            or i[0][key].param_type is int
-                            or i[0][key].param_type is np.uintc
-                            or i[0][key].param_type is np.uint
+                            params[key].param_type is np.intc
+                            or params[key].param_type is int
+                            or params[key].param_type is np.uintc
+                            or params[key].param_type is np.uint
                         ):
-                            val = i[0][key].param_type(np.floor(val))
-                            if val >= i[0][key].value.max:
-                                val = i[0][key].value.max - 1
+                            val = params[key].param_type(np.floor(val))
+                            if val >= params[key].value.max:
+                                val = params[key].value.max - 1
                         args[key] = val
                     else:
-                        args[key] = i[0][key].value[
+                        # normalize solution vector
+                        # this needs to be done since the binning logic expect them to be in a range between 0 and 1
+                        lower, upper = fitness_function.get_bounds()
+                        solution_vector = (solution_vector - lower) / (upper - lower)
+
+                        args[key] = params[key].value[
                             get_bin_index(
-                                solution_vector[solution_index], len(i[0][key].value)
+                                solution_vector[solution_index], len(params[key].value)
                             )
                         ]
                 solution_index += 1
-            if i[1] is not None:
-                i[1].set_parameters(**args)
+            if component:
+                component.set_parameters(**args)
 
         x_train, x_test, y_train, y_test = train_test_split(x, y, test_size=0.2)
 
         if feature_selection_algorithm is None:
             selected_features_mask = np.ones(x.shape[1], dtype=bool)
         else:
             selected_features_mask = feature_selection_algorithm.select_features(
@@ -505,18 +512,23 @@
         if feature_transform_algorithm is not None:
             feature_transform_algorithm.fit(x_train)
             x_train = feature_transform_algorithm.transform(x_train)
             x_test = feature_transform_algorithm.transform(x_test)
 
         classifier.fit(x_train, y_train)
         predictions = classifier.predict(x_test)
+
+        # infer task for the selection of the OptimizationStats
+        # only regression models have the "Task" attribute
+        classification = not hasattr(classifier, 'Task')
+
         return (
             fitness_function.get_fitness(predictions, y_test) * -1,
             selected_features_mask,
-            OptimizationStats(predictions, y_test),
+            OptimizationStats(predictions, y_test) if classification else RegressionOptimizationStats(predictions, y_test),
         )
 
     def _evaluate(self, x):
         r"""Override fitness function.
 
         Args:
             x (numpy.ndarray): Solution:
```

### Comparing `niaaml-1.2.0/niaaml/pipeline_component.py` & `niaaml-2.0.0/niaaml/pipeline_component.py`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/niaaml/pipeline_optimizer.py` & `niaaml-2.0.0/niaaml/pipeline_optimizer.py`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/niaaml/preprocessing/encoding/feature_encoder.py` & `niaaml-2.0.0/niaaml/preprocessing/encoding/feature_encoder.py`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/niaaml/preprocessing/encoding/one_hot_encoder.py` & `niaaml-2.0.0/niaaml/preprocessing/encoding/one_hot_encoder.py`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/niaaml/preprocessing/encoding/utility.py` & `niaaml-2.0.0/niaaml/preprocessing/encoding/utility.py`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/niaaml/preprocessing/feature_selection/__init__.py` & `niaaml-2.0.0/niaaml/preprocessing/feature_selection/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,21 +15,24 @@
 from niaaml.preprocessing.feature_selection.grey_wolf_optimizer import GreyWolfOptimizer
 from niaaml.preprocessing.feature_selection.utility import (
     FeatureSelectionAlgorithmFactory,
 )
 from niaaml.preprocessing.feature_selection._feature_selection_threshold_problem import (
     _FeatureSelectionThresholdProblem,
 )
+from niaaml.preprocessing.feature_selection.select_univariate_regression import SelectUnivariateRegression
+
 
 __all__ = [
     "FeatureSelectionAlgorithm",
     "VarianceThreshold",
     "jDEFSTH",
     "SelectPercentile",
     "ParticleSwarmOptimization",
     "BatAlgorithm",
     "DifferentialEvolution",
     "GreyWolfOptimizer",
     "SelectKBest",
+    "SelectUnivariateRegression",
     "FeatureSelectionAlgorithmFactory",
     "_FeatureSelectionThresholdProblem",
 ]
```

### Comparing `niaaml-1.2.0/niaaml/preprocessing/feature_selection/_feature_selection_threshold_problem.py` & `niaaml-2.0.0/niaaml/preprocessing/feature_selection/_feature_selection_threshold_problem.py`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/niaaml/preprocessing/feature_selection/bat_algorithm.py` & `niaaml-2.0.0/niaaml/preprocessing/feature_selection/bat_algorithm.py`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/niaaml/preprocessing/feature_selection/differential_evolution.py` & `niaaml-2.0.0/niaaml/preprocessing/feature_selection/differential_evolution.py`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/niaaml/preprocessing/feature_selection/feature_selection_algorithm.py` & `niaaml-2.0.0/niaaml/preprocessing/feature_selection/feature_selection_algorithm.py`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/niaaml/preprocessing/feature_selection/grey_wolf_optimizer.py` & `niaaml-2.0.0/niaaml/preprocessing/feature_selection/grey_wolf_optimizer.py`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/niaaml/preprocessing/feature_selection/jDEFSTH.py` & `niaaml-2.0.0/niaaml/preprocessing/feature_selection/jDEFSTH.py`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/niaaml/preprocessing/feature_selection/particle_swarm_optimization.py` & `niaaml-2.0.0/niaaml/preprocessing/feature_selection/particle_swarm_optimization.py`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/niaaml/preprocessing/feature_selection/select_k_best.py` & `niaaml-2.0.0/niaaml/preprocessing/feature_selection/select_k_best.py`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/niaaml/preprocessing/feature_selection/select_percentile.py` & `niaaml-2.0.0/niaaml/preprocessing/feature_selection/select_percentile.py`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/niaaml/preprocessing/feature_selection/utility.py` & `niaaml-2.0.0/niaaml/preprocessing/feature_selection/utility.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from niaaml.preprocessing.feature_selection.select_univariate_regression import SelectUnivariateRegression
 from niaaml.utilities import Factory
 from niaaml.preprocessing.feature_selection.bat_algorithm import BatAlgorithm
 from niaaml.preprocessing.feature_selection.differential_evolution import (
     DifferentialEvolution,
 )
 from niaaml.preprocessing.feature_selection.grey_wolf_optimizer import GreyWolfOptimizer
 from niaaml.preprocessing.feature_selection.jDEFSTH import jDEFSTH
@@ -32,8 +33,9 @@
             "SelectKBest": SelectKBest,
             "SelectPercentile": SelectPercentile,
             "VarianceThreshold": VarianceThreshold,
             "BatAlgorithm": BatAlgorithm,
             "DifferentialEvolution": DifferentialEvolution,
             "GreyWolfOptimizer": GreyWolfOptimizer,
             "ParticleSwarmOptimization": ParticleSwarmOptimization,
+            "SelectUnivariateRegression": SelectUnivariateRegression,
         }
```

### Comparing `niaaml-1.2.0/niaaml/preprocessing/feature_selection/variance_threshold.py` & `niaaml-2.0.0/niaaml/preprocessing/feature_selection/variance_threshold.py`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/niaaml/preprocessing/feature_transform/__init__.py` & `niaaml-2.0.0/niaaml/preprocessing/feature_transform/__init__.py`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/niaaml/preprocessing/feature_transform/feature_transform_algorithm.py` & `niaaml-2.0.0/niaaml/preprocessing/feature_transform/feature_transform_algorithm.py`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/niaaml/preprocessing/feature_transform/max_abs_scaler.py` & `niaaml-2.0.0/niaaml/preprocessing/feature_transform/max_abs_scaler.py`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/niaaml/preprocessing/feature_transform/normalizer.py` & `niaaml-2.0.0/niaaml/preprocessing/feature_transform/normalizer.py`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/niaaml/preprocessing/feature_transform/quantile_transformer.py` & `niaaml-2.0.0/niaaml/preprocessing/feature_transform/quantile_transformer.py`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/niaaml/preprocessing/feature_transform/robust_scaler.py` & `niaaml-2.0.0/niaaml/preprocessing/feature_transform/robust_scaler.py`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/niaaml/preprocessing/feature_transform/standard_scaler.py` & `niaaml-2.0.0/niaaml/preprocessing/feature_transform/standard_scaler.py`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/niaaml/preprocessing/feature_transform/utility.py` & `niaaml-2.0.0/niaaml/preprocessing/feature_transform/utility.py`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/niaaml/preprocessing/imputation/imputer.py` & `niaaml-2.0.0/niaaml/preprocessing/imputation/imputer.py`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/niaaml/preprocessing/imputation/simple_imputer.py` & `niaaml-2.0.0/niaaml/preprocessing/imputation/simple_imputer.py`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/niaaml/preprocessing/imputation/utility.py` & `niaaml-2.0.0/niaaml/preprocessing/imputation/utility.py`

 * *Files identical despite different names*

### Comparing `niaaml-1.2.0/niaaml/utilities.py` & `niaaml-2.0.0/niaaml/utilities.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-from sklearn.metrics import accuracy_score, precision_score, cohen_kappa_score, f1_score
+from sklearn.metrics import accuracy_score, precision_score, cohen_kappa_score, f1_score, r2_score, mean_absolute_error, mean_squared_error
 import numpy as np
 
 __all__ = [
     "MinMax",
     "ParameterDefinition",
     "OptimizationStats",
+    "RegressionOptimizationStats",
     "Factory",
     "get_bin_index",
 ]
 
 
 def get_bin_index(value, number_of_bins):
     """Gets index of value's bin. Value must be between 0.0 and 1.0.
@@ -180,7 +181,45 @@
         """
         return "Accuracy: {acc},\nPrecision: {prc},\nCohen's kappa: {ck},\nF1-score: {f1}".format(
             acc=self._accuracy,
             prc=self._precision,
             ck=self._cohen_kappa,
             f1=self._f1_score,
         )
+
+
+class RegressionOptimizationStats:
+    r"""Class that holds pipeline optimization result's statistics. Includes R2, MAE and MSE.
+
+    Date:
+        2024
+
+    Author:
+        Laurenz Farthofer
+
+    License:
+        MIT
+
+    Attributes:
+        _r2 (float): Calculated R2.
+        _mae (float): Calculated mean absolute error.
+        _mse (float): Calculated mean squared error.
+    """
+
+    def __init__(self, predicted, expected, **kwargs):
+        r"""Initialize the factory.
+
+        Arguments:
+            predicted (Iterable[any]): Array of predictions.
+            expected (Iterable[any]): Array of targets.
+        """
+        self._r2 = r2_score(expected, predicted)
+        self._mae = mean_absolute_error(expected, predicted)
+        self._mse = mean_squared_error(expected, predicted)
+
+    def to_string(self):
+        r"""User friendly representation of the object.
+
+        Returns:
+            str: User friendly representation of the object.
+        """
+        return f"R2: {self._r2},\nMAE: {self._mae},\nMSE: {self._mse}"
```

### Comparing `niaaml-1.2.0/pyproject.toml` & `niaaml-2.0.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [tool.poetry]
 name = "NiaAML"
-version = "1.2.0"
+version = "2.0.0"
 description = "Python automated machine learning framework"
 license = "MIT"
-authors = ["Luka Pečnik <lukapecnik96@gmail.com>", "Iztok Fister Jr. <iztok@iztok-jr-fister.eu>"]
+authors = ["Luka Pečnik <lukapecnik96@gmail.com>", "Iztok Fister Jr. <iztok@iztok-jr-fister.eu>", "Laurenz Farthofer <laurenz@hey.com>"]
 keywords = ['classification', 'NiaPy', 'scikit-learn', 'nature-inspired algorithms', 'feature selection', 'preprocessing']
-homepage = "https://github.com/lukapecnik/NiaAML"
-repository = "https://github.com/lukapecnik/NiaAML"
-readme = "README.rst"
+homepage = "https://github.com/firefly-cpp/NiaAML"
+repository = "https://github.com/firefly-cpp/NiaAML"
+documentation= "https://niaaml.readthedocs.io/en/latest/"
+readme = "README.md"
 include = [
     { path="LICENSE", format="sdist" },
     { path="CHANGELOG.md", format="sdist" },
     { path="CITATION.md", format="sdist" },
     { path="COMPONENTS.md", format="sdist" }
 ]
```

