# Comparing `tmp/risklabai-0.0.80.tar.gz` & `tmp/RiskLabAI-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "risklabai-0.0.80.tar", last modified: Wed Apr 24 08:28:12 2024, max compression
+gzip compressed data, was "RiskLabAI-0.0.9.tar", last modified: Mon Jul 31 10:59:47 2023, max compression
```

## Comparing `risklabai-0.0.80.tar` & `RiskLabAI-0.0.9.tar`

### file list

```diff
@@ -1,133 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:28:12.089154 risklabai-0.0.80/
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-24 08:28:02.000000 risklabai-0.0.80/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-24 08:28:12.089154 risklabai-0.0.80/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-24 08:28:02.000000 risklabai-0.0.80/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:28:12.069154 risklabai-0.0.80/RiskLabAI/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:28:12.073154 risklabai-0.0.80/RiskLabAI/backtest/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/backtest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/backtest/backtest_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/backtest/backtest_synthetic_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    12167 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/backtest/backtset_overfitting_in_the_machine_learning_era_simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/backtest/bet_sizing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/backtest/probabilistic_sharpe_ratio.py
--rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/backtest/probability_of_backtest_overfitting.py
--rw-r--r--   0 runner    (1001) docker     (127)     8053 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/backtest/strategy_risk.py
--rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/backtest/test_set_overfitting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:28:12.073154 risklabai-0.0.80/RiskLabAI/backtest/validation/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/backtest/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13793 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/backtest/validation/combinatorial_purged.py
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/backtest/validation/cross_validator_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/backtest/validation/cross_validator_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8753 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/backtest/validation/cross_validator_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    12915 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/backtest/validation/kfold.py
--rw-r--r--   0 runner    (1001) docker     (127)    20004 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/backtest/validation/purged_kfold.py
--rw-r--r--   0 runner    (1001) docker     (127)     7058 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/backtest/validation/walk_forward.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:28:12.073154 risklabai-0.0.80/RiskLabAI/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/cluster/clustering.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:28:12.073154 risklabai-0.0.80/RiskLabAI/controller/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14344 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/controller/bars_initializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5680 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/controller/data_structure_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:28:12.077154 risklabai-0.0.80/RiskLabAI/data/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:28:12.077154 risklabai-0.0.80/RiskLabAI/data/denoise/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/data/denoise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12235 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/data/denoise/denoising.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:28:12.077154 risklabai-0.0.80/RiskLabAI/data/differentiation/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/data/differentiation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11236 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/data/differentiation/differentiation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:28:12.077154 risklabai-0.0.80/RiskLabAI/data/distance/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/data/distance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/data/distance/distance_metric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:28:12.077154 risklabai-0.0.80/RiskLabAI/data/labeling/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/data/labeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/data/labeling/financial_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)    20754 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/data/labeling/labeling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:28:12.077154 risklabai-0.0.80/RiskLabAI/data/structures/
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/data/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6744 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/data/structures/abstract_bars.py
--rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/data/structures/abstract_imbalance_bars.py
--rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/data/structures/abstract_information_driven_bars.py
--rw-r--r--   0 runner    (1001) docker     (127)     9475 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/data/structures/abstract_run_bars.py
--rw-r--r--   0 runner    (1001) docker     (127)    12377 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/data/structures/data_structures_lopez.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/data/structures/filtering_lopez.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/data/structures/hedging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/data/structures/imbalance_bars.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/data/structures/infomation_driven_bars.py
--rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/data/structures/run_bars.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/data/structures/standard_bars.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/data/structures/standard_bars_lopez.py
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/data/structures/time_bars.py
--rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/data/structures/utilities_lopez.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:28:12.081154 risklabai-0.0.80/RiskLabAI/data/synthetic_data/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/data/synthetic_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/data/synthetic_data/drift_burst_hypothesis.py
--rw-r--r--   0 runner    (1001) docker     (127)     9402 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/data/synthetic_data/synthetic_controlled_environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:28:12.081154 risklabai-0.0.80/RiskLabAI/data/weights/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/data/weights/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/data/weights/sample_weights.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:28:12.081154 risklabai-0.0.80/RiskLabAI/ensemble/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/ensemble/bagging_classifier_accuracy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:28:12.081154 risklabai-0.0.80/RiskLabAI/features/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:28:12.081154 risklabai-0.0.80/RiskLabAI/features/entropy_features/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/features/entropy_features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/features/entropy_features/entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/features/entropy_features/kontoyiannis.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/features/entropy_features/lempel_ziv.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/features/entropy_features/plug_in.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/features/entropy_features/pmf.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/features/entropy_features/shannon.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:28:12.085154 risklabai-0.0.80/RiskLabAI/features/feature_importance/
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/features/feature_importance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/features/feature_importance/clustered_feature_importance_mda.py
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/features/feature_importance/clustered_feature_importance_mdi.py
--rw-r--r--   0 runner    (1001) docker     (127)    12272 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/features/feature_importance/clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/features/feature_importance/feature_importance_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/features/feature_importance/feature_importance_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/features/feature_importance/feature_importance_mda.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/features/feature_importance/feature_importance_mdi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/features/feature_importance/feature_importance_sfi.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/features/feature_importance/feature_importance_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/features/feature_importance/generate_synthetic_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/features/feature_importance/orthogonal_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/features/feature_importance/weighted_tau.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:28:12.085154 risklabai-0.0.80/RiskLabAI/features/microstructural_features/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/features/microstructural_features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/features/microstructural_features/bekker_parkinson_volatility_estimator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/features/microstructural_features/corwin_schultz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:28:12.085154 risklabai-0.0.80/RiskLabAI/features/structural_breaks/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/features/structural_breaks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/features/structural_breaks/structural_breaks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:28:12.085154 risklabai-0.0.80/RiskLabAI/hpc/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/hpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/hpc/hpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:28:12.085154 risklabai-0.0.80/RiskLabAI/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14483 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/optimization/hrp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/optimization/hyper_parameter_tuning.py
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/optimization/nco.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:28:12.085154 risklabai-0.0.80/RiskLabAI/pde/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/pde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14678 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/pde/equation.py
--rw-r--r--   0 runner    (1001) docker     (127)    18512 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/pde/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14124 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/pde/solver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:28:12.089154 risklabai-0.0.80/RiskLabAI/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/utils/ewma.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/utils/momentum_mean_reverting_strategy_sides.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/utils/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-24 08:28:02.000000 risklabai-0.0.80/RiskLabAI/utils/smoothing_average.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:28:12.089154 risklabai-0.0.80/RiskLabAI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-24 08:28:12.000000 risklabai-0.0.80/RiskLabAI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-04-24 08:28:12.000000 risklabai-0.0.80/RiskLabAI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 08:28:12.000000 risklabai-0.0.80/RiskLabAI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-24 08:28:12.000000 risklabai-0.0.80/RiskLabAI.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-24 08:28:12.000000 risklabai-0.0.80/RiskLabAI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-24 08:28:12.000000 risklabai-0.0.80/RiskLabAI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-24 08:28:02.000000 risklabai-0.0.80/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-24 08:28:12.089154 risklabai-0.0.80/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:59:47.919233 RiskLabAI-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-31 10:59:33.000000 RiskLabAI-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-31 10:59:47.919233 RiskLabAI-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-31 10:59:33.000000 RiskLabAI-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:59:47.919233 RiskLabAI-0.0.9/RiskLabAI/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:59:47.919233 RiskLabAI-0.0.9/RiskLabAI/RiskLabAI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-31 10:59:47.000000 RiskLabAI-0.0.9/RiskLabAI/RiskLabAI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-31 10:59:47.000000 RiskLabAI-0.0.9/RiskLabAI/RiskLabAI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 10:59:47.000000 RiskLabAI-0.0.9/RiskLabAI/RiskLabAI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-31 10:59:47.000000 RiskLabAI-0.0.9/RiskLabAI/RiskLabAI.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-31 10:59:47.000000 RiskLabAI-0.0.9/RiskLabAI/RiskLabAI.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:59:47.919233 RiskLabAI-0.0.9/RiskLabAI/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-31 10:59:33.000000 RiskLabAI-0.0.9/RiskLabAI/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:59:47.919233 RiskLabAI-0.0.9/RiskLabAI/data/structures/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-31 10:59:33.000000 RiskLabAI-0.0.9/RiskLabAI/data/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-31 10:59:33.000000 RiskLabAI-0.0.9/RiskLabAI/data/structures/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-31 10:59:33.000000 RiskLabAI-0.0.9/RiskLabAI/data/structures/hedging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-31 10:59:33.000000 RiskLabAI-0.0.9/RiskLabAI/data/structures/infomation_driven_bars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-07-31 10:59:33.000000 RiskLabAI-0.0.9/RiskLabAI/data/structures/standard_bars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-07-31 10:59:33.000000 RiskLabAI-0.0.9/RiskLabAI/data/structures/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:59:47.919233 RiskLabAI-0.0.9/RiskLabAI/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-31 10:59:33.000000 RiskLabAI-0.0.9/RiskLabAI/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-31 10:59:33.000000 RiskLabAI-0.0.9/RiskLabAI/utils/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-31 10:59:33.000000 RiskLabAI-0.0.9/RiskLabAI/utils/smoothing_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-31 10:59:33.000000 RiskLabAI-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-31 10:59:47.919233 RiskLabAI-0.0.9/setup.cfg
```

### Comparing `risklabai-0.0.80/LICENSE` & `RiskLabAI-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `risklabai-0.0.80/RiskLabAI/data/structures/infomation_driven_bars.py` & `RiskLabAI-0.0.9/RiskLabAI/data/structures/infomation_driven_bars.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,62 +1,53 @@
 from typing import Tuple
 import numpy as np
 import pandas as pd
 
-from RiskLabAI.data.structures.utilities_lopez import compute_thresholds, create_ohlcv_dataframe
+from .utilities import *
 
 def generate_information_driven_bars(
     tick_data: pd.DataFrame,
     bar_type: str = "volume",
     initial_expected_ticks: int = 2000
 ) -> Tuple[pd.DataFrame, np.ndarray, np.ndarray]:
     """
     Implements Information-Driven Bars.
 
+    Reference: De Prado, M. (2018) Advances in Financial Machine Learning. John Wiley & Sons.
+
     This function computes the Information-Driven Bars based on tick data and the chosen bar type.
+    The following formulas are used in this function:
 
-    :param tick_data: DataFrame of tick data.
-    :type tick_data: pd.DataFrame
-    :param bar_type: Type of the bar. Can be "tick", "volume", or "dollar".
-    :type bar_type: str, default "volume"
-    :param initial_expected_ticks: The initial value of expected ticks.
-    :type initial_expected_ticks: int, default 2000
-
-    :return: Tuple containing the OHLCV DataFrame, absolute thetas, and thresholds.
-    :rtype: Tuple[pd.DataFrame, np.ndarray, np.ndarray]
-
-    .. note:: 
-       Reference:
-       De Prado, M. (2018) Advances in Financial Machine Learning. John Wiley & Sons.
-
-    .. math::
-       E_b = |\bar{x}|
-
-       where:
-       - :math:`E_b` is the expected value of the bars.
-       - :math:`\bar{x}` is the mean of the input data.
+    - The absolute value of the mean of the input data:
+
+      .. math:: E_b = |\bar{x}|
 
-    The compute_thresholds function is called to compute times_delta, thetas_absolute, thresholds,
-    times, thetas, and grouping_id.
+    - The compute_thresholds function is called to compute times_delta, thetas_absolute, thresholds,
+      times, thetas, and grouping_id.
+
+    :param tick_data: DataFrame of tick data.
+    :param bar_type: User can choose between "tick", "volume", or "dollar" imbalanced bars. Default is "volume".
+    :param initial_expected_ticks: The initial value of expected ticks. Default is 2000.
+    :return: Tuple containing the OHLCV DataFrame, thetas_absolute, and thresholds.
     """
 
     if bar_type == "volume":
-        input_data = tick_data['volume_labeled']
+        input_data = tick_data['volumelabeled']
     elif bar_type == "tick":
         input_data = tick_data['label']
     elif bar_type == "dollar":
-        input_data = tick_data['dollar_labeled']
+        input_data = tick_data['dollarslabeled']
     else:
         raise ValueError("Invalid bar type. Choose 'tick', 'volume', or 'dollar'.")
 
     bar_expected_value = np.abs(input_data.mean())
-    times_delta, thetas_absolute, thresholds, times, thetas, grouping_id = compute_thresholds(
-        input_data, initial_expected_ticks, bar_expected_value)
 
-    tick_grouped = tick_data.reset_index().assign(grouping_id=grouping_id)
-    dates = tick_grouped.groupby('grouping_id', as_index=False).first()['dates']
-    tick_data_grouped = tick_grouped.groupby('grouping_id')
+    times_delta, thetas_absolute, thresholds, times, thetas, grouping_id = compute_thresholds(input_data, initial_expected_ticks, bar_expected_value)
+
+    tick_grouped = tick_data.reset_index().assign(groupingID=grouping_id)
+    dates = tick_grouped.groupby('groupingID', as_index=False).first()['dates']
+    tick_data_grouped = tick_grouped.groupby('groupingID')
 
     ohlcv_dataframe = create_ohlcv_dataframe(tick_data_grouped)
     ohlcv_dataframe.set_index(dates, drop=True, inplace=True)
 
-    return ohlcv_dataframe, thetas_absolute, thresholds
+    return ohlcv_dataframe, thetas_absolute, thresholds
```

### Comparing `risklabai-0.0.80/RiskLabAI/data/structures/utilities_lopez.py` & `RiskLabAI-0.0.9/RiskLabAI/data/structures/utilities.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,60 +1,61 @@
 import numpy as np
 import pandas as pd
 import time
 from typing import List, Tuple
-from RiskLabAI.utils.smoothing_average import compute_exponential_weighted_moving_average
-from RiskLabAI.utils.progress import  progress_bar
-
+from RiskLabAI.utils import exponential_weighted_moving_average, progress_bar
 
 def compute_thresholds(
     target_column: np.ndarray,
     initial_expected_ticks: int,
     initial_bar_size: float
 ) -> Tuple[List[float], np.ndarray, np.ndarray, List[int], np.ndarray, np.ndarray]:
     """
-    Groups the target_column DataFrame based on a feature and calculates thresholds.
+    Group the DataFrame based on a feature and calculate thresholds.
 
     This function groups the target_column DataFrame based on a feature
     and calculates the thresholds, which can be used in financial machine learning
     applications such as dynamic time warping.
 
-    :param target_column: Target column of the DataFrame.
-    :type target_column: np.ndarray
-    :param initial_expected_ticks: Initial expected number of ticks.
-    :type initial_expected_ticks: int
-    :param initial_bar_size: Initial expected size of each tick.
-    :type initial_bar_size: float
-    :return: A tuple containing the time deltas, absolute theta values, thresholds,
-        times, theta values, and grouping IDs.
-    :rtype: Tuple[List[float], np.ndarray, np.ndarray, List[int], np.ndarray, np.ndarray]
+    Reference:
+        De Prado, M. (2018). Advances in financial machine learning. John Wiley & Sons.
+
+    Args:
+        target_column (np.ndarray): Target column of the DataFrame.
+        initial_expected_ticks (int): Initial expected number of ticks.
+        initial_bar_size (float): Initial expected size of each tick.
+
+    Returns:
+        Tuple[List[float], np.ndarray, np.ndarray, List[int], np.ndarray, np.ndarray]:
+        A tuple containing the time deltas, absolute theta values, thresholds, times,
+        theta values, and grouping IDs.
     """
     num_values = target_column.shape[0]
-    target_column_values = target_column.astype(np.float64)
+    target_column = target_column.values.astype(np.float64)
     absolute_thetas = np.zeros(num_values)
     thresholds = np.zeros(num_values)
     thetas = np.zeros(num_values)
     grouping_ids = np.zeros(num_values)
 
-    current_theta = target_column_values[0]
+    current_theta = target_column[0]
     thetas[0] = current_theta
     absolute_thetas[0] = np.abs(current_theta)
     current_grouping_id = 0
     grouping_ids[0] = current_grouping_id
 
     time_deltas = []
     times = []
     previous_time = 0
     expected_ticks = initial_expected_ticks
     expected_bar_value = initial_bar_size
 
     start_time = time.time()
 
     for i in range(1, num_values):
-        current_theta += target_column_values[i]
+        current_theta += target_column[i]
         thetas[i] = current_theta
         absolute_theta = np.abs(current_theta)
         absolute_thetas[i] = absolute_theta
 
         threshold = expected_ticks * expected_bar_value
         thresholds[i] = threshold
         grouping_ids[i] = current_grouping_id
@@ -62,45 +63,44 @@
         if absolute_theta >= threshold:
             current_grouping_id += 1
             current_theta = 0
             time_delta = np.float64(i - previous_time)
             time_deltas.append(time_delta)
             times.append(i)
             previous_time = i
-            expected_ticks = compute_exponential_weighted_moving_average(
+            expected_ticks = exponential_weighted_moving_average(
                 np.array(time_deltas), window_length=np.int64(len(time_deltas))
             )[-1]
             expected_bar_value = np.abs(
-                compute_exponential_weighted_moving_average(
-                    target_column_values[:i], window_length=np.int64(initial_expected_ticks)
+                exponential_weighted_moving_average(
+                    target_column[:i], window_length=np.int64(initial_expected_ticks)
                 )[-1]
             )
 
+        # Replace 'progress_bar' with your actual progress bar function
         progress_bar(i, num_values, start_time)
 
     return time_deltas, absolute_thetas, thresholds, times, thetas, grouping_ids
 
-
 def create_ohlcv_dataframe(
     tick_data_grouped: pd.core.groupby.DataFrameGroupBy
 ) -> pd.DataFrame:
     """
-    Takes a grouped DataFrame and creates a new one with OHLCV data and other relevant information.
+    Takes a grouped dataframe, combining and creating a new one with information about
+    prices and volume.
 
-    :param tick_data_grouped: Grouped DataFrame based on some criteria (e.g., time).
+    :param tick_data_grouped: Grouped dataframes based on some criteria (e.g., time)
     :type tick_data_grouped: pd.core.groupby.DataFrameGroupBy
-    :return: A DataFrame containing OHLCV data and other relevant information.
+    :return: A dataframe containing OHLCV data and other relevant information
     :rtype: pd.DataFrame
     """
-    ohlc = tick_data_grouped['price'].ohlc()
-    ohlc['volume'] = tick_data_grouped['size'].sum()
+    ohlc = tick_data_grouped['price'].ohlc()  # find price in each tick
+    ohlc['volume'] = tick_data_grouped['size'].sum()  # find volume traded
     ohlc['value_of_trades'] = tick_data_grouped.apply(
         lambda x: (x['price'] * x['size']).sum() / x['size'].sum()
-    )
-    ohlc['price_mean'] = tick_data_grouped['price'].mean()
-    ohlc['tick_count'] = tick_data_grouped['price'].count()
-    ohlc['price_mean_log_return'] = np.log(ohlc['price_mean']) - np.log(ohlc['price_mean'].shift(1))
-
+    )  # find value of trades
+    ohlc['price_mean'] = tick_data_grouped['price'].mean()  # mean of price
+    ohlc['tick_count'] = tick_data_grouped['price'].count()  # number of ticks
+    ohlc['price_mean_log_return'] = (
+        np.log(ohlc['price_mean']) - np.log(ohlc['price_mean'].shift(1))
+    )  # find log return
     return ohlc
-
-
-
```

### Comparing `risklabai-0.0.80/RiskLabAI/utils/progress.py` & `RiskLabAI-0.0.9/RiskLabAI/utils/progress.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,29 @@
 import sys
 import time
 from typing import NoReturn
 
-
 def progress_bar(
-    current_progress: int, 
-    total_progress: int, 
-    start_time: float, 
+    current_progress: int,
+    total_progress: int,
+    start_time: float,
     bar_length: int = 20
 ) -> NoReturn:
     """
-    Display a terminal-style progress bar with completion percentage and estimated remaining time.
-
-    :param current_progress: Current value indicating the progress made.
-    :param total_progress: Total value representing the completion of the task.
-    :param start_time: The time at which the task started, typically acquired via time.time().
-    :param bar_length: Length of the progress bar in terminal characters, default is 20.
-    
-    The displayed progress bar uses the formula:
-
-    .. math::
-        \text{percentage} = \frac{\text{current\_progress}}{\text{total\_progress}}
+    Display a progress bar for a task with a given completion percentage and remaining time.
 
-    The estimated remaining time is calculated based on elapsed time and progress made:
-
-    .. math::
-        \text{remaining\_time} = \frac{\text{elapsed\_time} \times (\text{total\_progress} - \text{current\_progress})}{\text{current\_progress}}
-
-    :return: None
+    Args:
+        current_progress (int): Current progress value of the task.
+        total_progress (int): Total value of the task, representing 100% completion.
+        start_time (float): Start time of the task (typically from time.time()).
+        bar_length (int, optional): Length of the progress bar. Default is 20.
     """
-
-    percentage = current_progress / total_progress
+    percentage = float(current_progress) / total_progress
     arrow = '-' * int(round(percentage * bar_length) - 1) + '>'
     spaces = ' ' * (bar_length - len(arrow))
 
     elapsed_time = time.time() - start_time
-    
-    if current_progress == 0:
-        remaining_time = "Calculating..."
-    else:
-        remaining_time = int(
-            (elapsed_time / current_progress) * (total_progress - current_progress) / 60
-        )
+    remaining_time = int(((elapsed_time / current_progress) * (total_progress - current_progress)) / 60)
 
-    if current_progress == total_progress:
-        sys.stdout.write("\rCompleted: [{0}] 100% - Task completed!\n".format('-' * bar_length))
-    
-    else:
-        sys.stdout.write("\rCompleted: [{0}] {1}% - {2} minutes remaining.".format(
-            arrow + spaces, int(round(percentage * 100)), remaining_time))
-    
+    sys.stdout.write("\rCompleted: [{0}] {1}% - {2} minutes remaining.".format(
+                     arrow + spaces, int(round(percentage * 100)), remaining_time))
     sys.stdout.flush()
```

### Comparing `risklabai-0.0.80/RiskLabAI/utils/smoothing_average.py` & `RiskLabAI-0.0.9/RiskLabAI/utils/smoothing_average.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,39 @@
 import numpy as np
-from typing import List
+from typing import List, Tuple
 
-
-def compute_exponential_weighted_moving_average(
-    input_series: np.ndarray, 
+def exponential_weighted_moving_average(
+    input_series: np.ndarray,
     window_length: int
 ) -> np.ndarray:
     """
     Compute the exponential weighted moving average (EWMA) of a time series array.
 
     The EWMA is calculated using the formula:
 
     .. math::
-        EWMA_t = \\frac{x_t + (1 - \\alpha) x_{t-1} + (1 - \\alpha)^2 x_{t-2} + \\ldots}{\\omega_t}
 
-    where:
+        EWMA_t = \\frac{x_t + (1 - \\alpha) * x_{t-1} + (1 - \\alpha)^2 * x_{t-2} + \\cdots}{\\omega_t}
 
-    .. math::
-        \\omega_t = 1 + (1 - \\alpha) + (1 - \\alpha)^2 + \\ldots + (1 - \\alpha)^t,
-        \\alpha = \\frac{2}{{window\_length + 1}}
+    where :math:`\\omega_t = 1 + (1 - \\alpha) + (1 - \\alpha)^2 + \\cdots + (1 - \\alpha)^t`,
+    and :math:`\\alpha = \\frac{2}{\\text{window_length} + 1}`
 
-    :param input_series: Input time series array.
-    :type input_series: np.ndarray
-    :param window_length: Window length for the exponential weighted moving average.
-    :type window_length: int
-    :return: An array containing the computed EWMA values.
-    :rtype: np.ndarray
-    """
+    Args:
+        input_series (np.ndarray): Input time series array.
+        window_length (int): Window length for the exponential weighted moving average.
 
+    Returns:
+        np.ndarray: An array containing the computed EWMA values.
+    """
     num_values = input_series.shape[0]
     ewma_output = np.empty(num_values, dtype='float64')
+    omega = 1
     alpha = 2 / float(window_length + 1)
-    multiplier = 1 - alpha
-    current_weighted_sum = input_series[0]
-    ewma_output[0] = current_weighted_sum
+    current_input_value = input_series[0]
+    ewma_output[0] = current_input_value
 
     for i in range(1, num_values):
-        current_weighted_sum = current_weighted_sum * multiplier + input_series[i]
-        ewma_output[i] = current_weighted_sum / (1 - multiplier ** (i+1))
+        omega += (1 - alpha) ** i
+        current_input_value = current_input_value * (1 - alpha) + input_series[i]
+        ewma_output[i] = current_input_value / omega
 
     return ewma_output
```

### Comparing `risklabai-0.0.80/setup.cfg` & `RiskLabAI-0.0.9/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 [metadata]
 name = RiskLabAI
-version = 0.0.80
+version = 0.0.9
 author = RiskLab
-author_email = arian@risklab.ai
+author_email = research@risklab.ai
 description = Financial AI using Python.
 long_description_content_type = text/markdown
 url = https://github.com/RiskLabAI/RiskLabAI.py
 project_urls = 
 	Bug Tracker = https://github.com/RiskLabAI/RiskLabAI.py/issues
 	Changelog = https://github.com/RiskLabAI/RiskLabAI.py/releases
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: BSD License
 	Intended Audience :: Developers
 
 [options]
+package_dir = 
+	= RiskLabAI
 packages = find:
-install_requires = 
-	scipy
-	ta
-	quantecon
+python_requires = >=3.6
+
+[options.packages.find]
+where = RiskLabAI
 
 [options.entry_points]
 console_scripts = 
 	RiskLabAI = RiskLabAI.app:entry_point
 
 [egg_info]
 tag_build =
```

