# Comparing `tmp/topsearch-0.0.2.tar.gz` & `tmp/topsearch-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "topsearch-0.0.2.tar", max compression
+gzip compressed data, was "topsearch-0.0.3.tar", max compression
```

## Comparing `topsearch-0.0.2.tar` & `topsearch-0.0.3.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0        0        0     1088 2024-02-07 09:18:36.918600 topsearch-0.0.2/LICENSE
--rw-r--r--   0        0        0     7577 2024-03-22 16:52:51.899726 topsearch-0.0.2/README.md
--rw-r--r--   0        0        0      889 2024-03-22 18:06:56.260125 topsearch-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-05 17:05:09.155000 topsearch-0.0.2/src/topsearch/__init__.py
--rw-r--r--   0        0        0        0 2024-03-04 16:45:12.286369 topsearch-0.0.2/src/topsearch/analysis/__init__.py
--rw-r--r--   0        0        0      163 2024-02-05 17:05:09.173833 topsearch-0.0.2/src/topsearch/analysis/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     7556 2024-02-05 17:05:09.171151 topsearch-0.0.2/src/topsearch/analysis/__pycache__/batch_selection.cpython-310.pyc
--rw-r--r--   0        0        0     2480 2024-02-05 17:05:09.173097 topsearch-0.0.2/src/topsearch/analysis/__pycache__/graph_properties.cpython-310.pyc
--rw-r--r--   0        0        0     3525 2024-02-05 17:05:09.172099 topsearch-0.0.2/src/topsearch/analysis/__pycache__/minima_properties.cpython-310.pyc
--rw-r--r--   0        0        0     3336 2024-02-05 17:05:09.174389 topsearch-0.0.2/src/topsearch/analysis/__pycache__/pair_selection.cpython-310.pyc
--rw-r--r--   0        0        0     1511 2024-02-05 17:05:09.171671 topsearch-0.0.2/src/topsearch/analysis/__pycache__/roughness.cpython-310.pyc
--rw-r--r--   0        0        0    11321 2024-03-22 16:52:51.987550 topsearch-0.0.2/src/topsearch/analysis/batch_selection.py
--rw-r--r--   0        0        0     2496 2024-03-04 16:45:12.291963 topsearch-0.0.2/src/topsearch/analysis/graph_properties.py
--rw-r--r--   0        0        0     4013 2024-03-04 16:45:12.292403 topsearch-0.0.2/src/topsearch/analysis/minima_properties.py
--rw-r--r--   0        0        0     3288 2024-03-22 16:52:51.987977 topsearch-0.0.2/src/topsearch/analysis/pair_selection.py
--rw-r--r--   0        0        0     1711 2024-03-04 16:45:12.293254 topsearch-0.0.2/src/topsearch/analysis/roughness.py
--rw-r--r--   0        0        0        1 2024-03-04 16:46:31.350761 topsearch-0.0.2/src/topsearch/data/__init__.py
--rw-r--r--   0        0        0      159 2024-02-05 17:05:09.323335 topsearch-0.0.2/src/topsearch/data/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    20073 2024-02-05 17:05:09.322705 topsearch-0.0.2/src/topsearch/data/__pycache__/coordinates.cpython-310.pyc
--rw-r--r--   0        0        0     8346 2024-02-05 17:05:09.323056 topsearch-0.0.2/src/topsearch/data/__pycache__/kinetic_transition_network.cpython-310.pyc
--rw-r--r--   0        0        0     6369 2024-02-05 17:05:09.323622 topsearch-0.0.2/src/topsearch/data/__pycache__/model_data.cpython-310.pyc
--rw-r--r--   0        0        0    27183 2024-03-22 16:52:51.988461 topsearch-0.0.2/src/topsearch/data/coordinates.py
--rw-r--r--   0        0        0     8982 2024-03-22 16:52:51.988976 topsearch-0.0.2/src/topsearch/data/kinetic_transition_network.py
--rw-r--r--   0        0        0     6700 2024-03-22 16:52:51.989481 topsearch-0.0.2/src/topsearch/data/model_data.py
--rw-r--r--   0        0        0        0 2024-03-04 16:47:36.356007 topsearch-0.0.2/src/topsearch/global_optimisation/__init__.py
--rw-r--r--   0        0        0      174 2024-02-05 17:05:09.590930 topsearch-0.0.2/src/topsearch/global_optimisation/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4800 2024-02-05 17:05:09.591439 topsearch-0.0.2/src/topsearch/global_optimisation/__pycache__/basin_hopping.cpython-310.pyc
--rw-r--r--   0        0        0     4416 2024-02-05 17:05:09.590611 topsearch-0.0.2/src/topsearch/global_optimisation/__pycache__/perturbations.cpython-310.pyc
--rw-r--r--   0        0        0     6741 2024-03-22 16:54:23.940695 topsearch-0.0.2/src/topsearch/global_optimisation/basin_hopping.py
--rw-r--r--   0        0        0     4511 2024-03-04 16:47:36.357373 topsearch-0.0.2/src/topsearch/global_optimisation/perturbations.py
--rw-r--r--   0        0        0        0 2024-03-04 16:48:26.111698 topsearch-0.0.2/src/topsearch/minimisation/__init__.py
--rw-r--r--   0        0        0      167 2024-02-05 17:05:09.593951 topsearch-0.0.2/src/topsearch/minimisation/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1125 2024-02-05 17:05:09.593616 topsearch-0.0.2/src/topsearch/minimisation/__pycache__/lbfgs.cpython-310.pyc
--rw-r--r--   0        0        0     1240 2024-03-22 16:52:51.990390 topsearch-0.0.2/src/topsearch/minimisation/lbfgs.py
--rw-r--r--   0        0        0        0 2024-03-04 16:48:57.642361 topsearch-0.0.2/src/topsearch/plotting/__init__.py
--rw-r--r--   0        0        0      163 2024-02-05 17:05:09.596607 topsearch-0.0.2/src/topsearch/plotting/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     5820 2024-02-05 17:05:09.595879 topsearch-0.0.2/src/topsearch/plotting/__pycache__/disconnectivity.cpython-310.pyc
--rw-r--r--   0        0        0     2214 2024-02-05 17:05:09.596255 topsearch-0.0.2/src/topsearch/plotting/__pycache__/network.cpython-310.pyc
--rw-r--r--   0        0        0     4070 2024-02-05 17:05:09.595579 topsearch-0.0.2/src/topsearch/plotting/__pycache__/stationary_points.cpython-310.pyc
--rw-r--r--   0        0        0     8152 2024-03-22 16:52:51.990841 topsearch-0.0.2/src/topsearch/plotting/disconnectivity.py
--rw-r--r--   0        0        0     2090 2024-03-04 16:48:57.643958 topsearch-0.0.2/src/topsearch/plotting/network.py
--rw-r--r--   0        0        0     5795 2024-03-22 16:52:51.991295 topsearch-0.0.2/src/topsearch/plotting/stationary_points.py
--rw-r--r--   0        0        0        0 2024-03-04 16:50:21.938464 topsearch-0.0.2/src/topsearch/potentials/__init__.py
--rw-r--r--   0        0        0      165 2024-02-05 17:05:09.603497 topsearch-0.0.2/src/topsearch/potentials/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     5911 2024-02-05 17:05:09.600165 topsearch-0.0.2/src/topsearch/potentials/__pycache__/atomic.cpython-310.pyc
--rw-r--r--   0        0        0     2962 2024-02-05 17:05:09.601118 topsearch-0.0.2/src/topsearch/potentials/__pycache__/bayesian_optimisation.cpython-310.pyc
--rw-r--r--   0        0        0     4494 2024-02-05 17:05:09.601561 topsearch-0.0.2/src/topsearch/potentials/__pycache__/dataset_fitting.cpython-310.pyc
--rw-r--r--   0        0        0     3582 2024-02-05 17:05:09.600467 topsearch-0.0.2/src/topsearch/potentials/__pycache__/dataset_regression.cpython-310.pyc
--rw-r--r--   0        0        0     3650 2024-02-05 17:05:09.602584 topsearch-0.0.2/src/topsearch/potentials/__pycache__/dft.cpython-310.pyc
--rw-r--r--   0        0        0     2576 2024-02-05 17:05:09.599845 topsearch-0.0.2/src/topsearch/potentials/__pycache__/force_fields.cpython-310.pyc
--rw-r--r--   0        0        0     5451 2024-02-05 17:05:09.602918 topsearch-0.0.2/src/topsearch/potentials/__pycache__/gaussian_process.cpython-310.pyc
--rw-r--r--   0        0        0     3680 2024-02-05 17:05:09.602255 topsearch-0.0.2/src/topsearch/potentials/__pycache__/ml_potentials.cpython-310.pyc
--rw-r--r--   0        0        0     6000 2024-02-05 17:05:09.603237 topsearch-0.0.2/src/topsearch/potentials/__pycache__/molecular.cpython-310.pyc
--rw-r--r--   0        0        0     3510 2024-02-05 17:05:09.600771 topsearch-0.0.2/src/topsearch/potentials/__pycache__/potential.cpython-310.pyc
--rw-r--r--   0        0        0     3596 2024-02-05 17:05:09.603902 topsearch-0.0.2/src/topsearch/potentials/__pycache__/test_functions.cpython-310-pytest-7.4.3.pyc
--rw-r--r--   0        0        0     3487 2024-02-05 17:05:09.601937 topsearch-0.0.2/src/topsearch/potentials/__pycache__/test_functions.cpython-310.pyc
--rw-r--r--   0        0        0     6419 2024-03-22 16:52:51.991707 topsearch-0.0.2/src/topsearch/potentials/atomic.py
--rw-r--r--   0        0        0     2538 2024-03-22 16:52:51.992126 topsearch-0.0.2/src/topsearch/potentials/bayesian_optimisation.py
--rw-r--r--   0        0        0     4610 2024-03-22 16:52:51.992545 topsearch-0.0.2/src/topsearch/potentials/dataset_fitting.py
--rw-r--r--   0        0        0     3946 2024-03-22 16:52:51.993106 topsearch-0.0.2/src/topsearch/potentials/dft.py
--rw-r--r--   0        0        0     2792 2024-03-22 16:52:51.993531 topsearch-0.0.2/src/topsearch/potentials/force_fields.py
--rw-r--r--   0        0        0     6658 2024-03-22 16:52:51.993874 topsearch-0.0.2/src/topsearch/potentials/gaussian_process.py
--rw-r--r--   0        0        0     4745 2024-03-22 16:52:51.994211 topsearch-0.0.2/src/topsearch/potentials/ml_potentials.py
--rw-r--r--   0        0        0     3928 2024-03-22 17:54:26.549618 topsearch-0.0.2/src/topsearch/potentials/potential.py
--rw-r--r--   0        0        0     2538 2024-03-22 16:52:51.995096 topsearch-0.0.2/src/topsearch/potentials/test_functions.py
--rw-r--r--   0        0        0        0 2024-02-05 17:05:09.605742 topsearch-0.0.2/src/topsearch/sampling/__init__.py
--rw-r--r--   0        0        0      163 2024-02-05 17:05:09.606895 topsearch-0.0.2/src/topsearch/sampling/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    13538 2024-02-05 17:05:09.606553 topsearch-0.0.2/src/topsearch/sampling/__pycache__/exploration.cpython-310.pyc
--rw-r--r--   0        0        0    19382 2024-03-04 16:51:13.107032 topsearch-0.0.2/src/topsearch/sampling/exploration.py
--rw-r--r--   0        0        0        0 2024-02-05 17:05:09.607530 topsearch-0.0.2/src/topsearch/similarity/__init__.py
--rw-r--r--   0        0        0      165 2024-02-05 17:05:09.609535 topsearch-0.0.2/src/topsearch/similarity/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     9129 2024-02-05 17:05:09.608729 topsearch-0.0.2/src/topsearch/similarity/__pycache__/molecular_similarity.cpython-310.pyc
--rw-r--r--   0        0        0     5861 2024-02-05 17:05:09.609184 topsearch-0.0.2/src/topsearch/similarity/__pycache__/similarity.cpython-310.pyc
--rw-r--r--   0        0        0    14441 2024-03-22 17:54:26.549946 topsearch-0.0.2/src/topsearch/similarity/molecular_similarity.py
--rw-r--r--   0        0        0     7273 2024-03-22 16:52:51.996182 topsearch-0.0.2/src/topsearch/similarity/similarity.py
--rw-r--r--   0        0        0        0 2024-02-05 17:05:09.612518 topsearch-0.0.2/src/topsearch/transition_states/__init__.py
--rw-r--r--   0        0        0      172 2024-02-05 17:05:09.613615 topsearch-0.0.2/src/topsearch/transition_states/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    16885 2024-02-05 17:05:09.613978 topsearch-0.0.2/src/topsearch/transition_states/__pycache__/hybrid_eigenvector_following.cpython-310.pyc
--rw-r--r--   0        0        0    11193 2024-02-05 17:05:09.613349 topsearch-0.0.2/src/topsearch/transition_states/__pycache__/nudged_elastic_band.cpython-310.pyc
--rw-r--r--   0        0        0    28595 2024-03-22 17:54:26.550264 topsearch-0.0.2/src/topsearch/transition_states/hybrid_eigenvector_following.py
--rw-r--r--   0        0        0    16707 2024-03-22 16:52:51.997350 topsearch-0.0.2/src/topsearch/transition_states/nudged_elastic_band.py
--rw-r--r--   0        0        0     8647 1970-01-01 00:00:00.000000 topsearch-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1088 2024-02-07 09:18:36.918600 topsearch-0.0.3/LICENSE
+-rw-r--r--   0        0        0     7445 2024-04-03 12:18:36.422772 topsearch-0.0.3/README.md
+-rw-r--r--   0        0        0      889 2024-04-24 10:13:35.557216 topsearch-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-05 17:05:09.155000 topsearch-0.0.3/src/topsearch/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-04 16:45:12.286369 topsearch-0.0.3/src/topsearch/analysis/__init__.py
+-rw-r--r--   0        0        0      163 2024-02-05 17:05:09.173833 topsearch-0.0.3/src/topsearch/analysis/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     7556 2024-02-05 17:05:09.171151 topsearch-0.0.3/src/topsearch/analysis/__pycache__/batch_selection.cpython-310.pyc
+-rw-r--r--   0        0        0     2480 2024-02-05 17:05:09.173097 topsearch-0.0.3/src/topsearch/analysis/__pycache__/graph_properties.cpython-310.pyc
+-rw-r--r--   0        0        0     3525 2024-02-05 17:05:09.172099 topsearch-0.0.3/src/topsearch/analysis/__pycache__/minima_properties.cpython-310.pyc
+-rw-r--r--   0        0        0     3336 2024-02-05 17:05:09.174389 topsearch-0.0.3/src/topsearch/analysis/__pycache__/pair_selection.cpython-310.pyc
+-rw-r--r--   0        0        0     1511 2024-02-05 17:05:09.171671 topsearch-0.0.3/src/topsearch/analysis/__pycache__/roughness.cpython-310.pyc
+-rw-r--r--   0        0        0    11321 2024-04-03 12:15:46.559253 topsearch-0.0.3/src/topsearch/analysis/batch_selection.py
+-rw-r--r--   0        0        0     2496 2024-03-04 16:45:12.291963 topsearch-0.0.3/src/topsearch/analysis/graph_properties.py
+-rw-r--r--   0        0        0     4013 2024-03-04 16:45:12.292403 topsearch-0.0.3/src/topsearch/analysis/minima_properties.py
+-rw-r--r--   0        0        0     3288 2024-04-03 12:15:46.562303 topsearch-0.0.3/src/topsearch/analysis/pair_selection.py
+-rw-r--r--   0        0        0     1711 2024-03-04 16:45:12.293254 topsearch-0.0.3/src/topsearch/analysis/roughness.py
+-rw-r--r--   0        0        0        1 2024-03-04 16:46:31.350761 topsearch-0.0.3/src/topsearch/data/__init__.py
+-rw-r--r--   0        0        0      159 2024-02-05 17:05:09.323335 topsearch-0.0.3/src/topsearch/data/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    20073 2024-02-05 17:05:09.322705 topsearch-0.0.3/src/topsearch/data/__pycache__/coordinates.cpython-310.pyc
+-rw-r--r--   0        0        0     8346 2024-02-05 17:05:09.323056 topsearch-0.0.3/src/topsearch/data/__pycache__/kinetic_transition_network.cpython-310.pyc
+-rw-r--r--   0        0        0     6369 2024-02-05 17:05:09.323622 topsearch-0.0.3/src/topsearch/data/__pycache__/model_data.cpython-310.pyc
+-rw-r--r--   0        0        0    27908 2024-04-24 09:39:46.932950 topsearch-0.0.3/src/topsearch/data/coordinates.py
+-rw-r--r--   0        0        0     8982 2024-04-03 12:15:46.568337 topsearch-0.0.3/src/topsearch/data/kinetic_transition_network.py
+-rw-r--r--   0        0        0     6700 2024-04-03 12:15:46.572307 topsearch-0.0.3/src/topsearch/data/model_data.py
+-rw-r--r--   0        0        0        0 2024-03-04 16:47:36.356007 topsearch-0.0.3/src/topsearch/global_optimisation/__init__.py
+-rw-r--r--   0        0        0      174 2024-02-05 17:05:09.590930 topsearch-0.0.3/src/topsearch/global_optimisation/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4800 2024-02-05 17:05:09.591439 topsearch-0.0.3/src/topsearch/global_optimisation/__pycache__/basin_hopping.cpython-310.pyc
+-rw-r--r--   0        0        0     4416 2024-02-05 17:05:09.590611 topsearch-0.0.3/src/topsearch/global_optimisation/__pycache__/perturbations.cpython-310.pyc
+-rw-r--r--   0        0        0     6741 2024-03-22 16:54:23.940695 topsearch-0.0.3/src/topsearch/global_optimisation/basin_hopping.py
+-rw-r--r--   0        0        0     4511 2024-03-04 16:47:36.357373 topsearch-0.0.3/src/topsearch/global_optimisation/perturbations.py
+-rw-r--r--   0        0        0        0 2024-03-04 16:48:26.111698 topsearch-0.0.3/src/topsearch/minimisation/__init__.py
+-rw-r--r--   0        0        0      167 2024-02-05 17:05:09.593951 topsearch-0.0.3/src/topsearch/minimisation/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1125 2024-02-05 17:05:09.593616 topsearch-0.0.3/src/topsearch/minimisation/__pycache__/lbfgs.cpython-310.pyc
+-rw-r--r--   0        0        0     1240 2024-04-03 12:15:46.577680 topsearch-0.0.3/src/topsearch/minimisation/lbfgs.py
+-rw-r--r--   0        0        0        0 2024-03-04 16:48:57.642361 topsearch-0.0.3/src/topsearch/plotting/__init__.py
+-rw-r--r--   0        0        0      163 2024-02-05 17:05:09.596607 topsearch-0.0.3/src/topsearch/plotting/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     5820 2024-02-05 17:05:09.595879 topsearch-0.0.3/src/topsearch/plotting/__pycache__/disconnectivity.cpython-310.pyc
+-rw-r--r--   0        0        0     2214 2024-02-05 17:05:09.596255 topsearch-0.0.3/src/topsearch/plotting/__pycache__/network.cpython-310.pyc
+-rw-r--r--   0        0        0     4070 2024-02-05 17:05:09.595579 topsearch-0.0.3/src/topsearch/plotting/__pycache__/stationary_points.cpython-310.pyc
+-rw-r--r--   0        0        0     8152 2024-04-03 12:15:46.579373 topsearch-0.0.3/src/topsearch/plotting/disconnectivity.py
+-rw-r--r--   0        0        0     2090 2024-03-04 16:48:57.643958 topsearch-0.0.3/src/topsearch/plotting/network.py
+-rw-r--r--   0        0        0     5795 2024-04-03 12:15:46.582630 topsearch-0.0.3/src/topsearch/plotting/stationary_points.py
+-rw-r--r--   0        0        0        0 2024-03-04 16:50:21.938464 topsearch-0.0.3/src/topsearch/potentials/__init__.py
+-rw-r--r--   0        0        0      165 2024-02-05 17:05:09.603497 topsearch-0.0.3/src/topsearch/potentials/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     5911 2024-02-05 17:05:09.600165 topsearch-0.0.3/src/topsearch/potentials/__pycache__/atomic.cpython-310.pyc
+-rw-r--r--   0        0        0     2962 2024-02-05 17:05:09.601118 topsearch-0.0.3/src/topsearch/potentials/__pycache__/bayesian_optimisation.cpython-310.pyc
+-rw-r--r--   0        0        0     4494 2024-02-05 17:05:09.601561 topsearch-0.0.3/src/topsearch/potentials/__pycache__/dataset_fitting.cpython-310.pyc
+-rw-r--r--   0        0        0     3582 2024-02-05 17:05:09.600467 topsearch-0.0.3/src/topsearch/potentials/__pycache__/dataset_regression.cpython-310.pyc
+-rw-r--r--   0        0        0     3650 2024-02-05 17:05:09.602584 topsearch-0.0.3/src/topsearch/potentials/__pycache__/dft.cpython-310.pyc
+-rw-r--r--   0        0        0     2576 2024-02-05 17:05:09.599845 topsearch-0.0.3/src/topsearch/potentials/__pycache__/force_fields.cpython-310.pyc
+-rw-r--r--   0        0        0     5451 2024-02-05 17:05:09.602918 topsearch-0.0.3/src/topsearch/potentials/__pycache__/gaussian_process.cpython-310.pyc
+-rw-r--r--   0        0        0     3680 2024-02-05 17:05:09.602255 topsearch-0.0.3/src/topsearch/potentials/__pycache__/ml_potentials.cpython-310.pyc
+-rw-r--r--   0        0        0     6000 2024-02-05 17:05:09.603237 topsearch-0.0.3/src/topsearch/potentials/__pycache__/molecular.cpython-310.pyc
+-rw-r--r--   0        0        0     3510 2024-02-05 17:05:09.600771 topsearch-0.0.3/src/topsearch/potentials/__pycache__/potential.cpython-310.pyc
+-rw-r--r--   0        0        0     3596 2024-02-05 17:05:09.603902 topsearch-0.0.3/src/topsearch/potentials/__pycache__/test_functions.cpython-310-pytest-7.4.3.pyc
+-rw-r--r--   0        0        0     3487 2024-02-05 17:05:09.601937 topsearch-0.0.3/src/topsearch/potentials/__pycache__/test_functions.cpython-310.pyc
+-rw-r--r--   0        0        0     6419 2024-04-03 12:15:46.586499 topsearch-0.0.3/src/topsearch/potentials/atomic.py
+-rw-r--r--   0        0        0     2538 2024-04-03 12:15:46.588759 topsearch-0.0.3/src/topsearch/potentials/bayesian_optimisation.py
+-rw-r--r--   0        0        0     4610 2024-04-03 12:15:46.590322 topsearch-0.0.3/src/topsearch/potentials/dataset_fitting.py
+-rw-r--r--   0        0        0     3946 2024-04-03 12:15:46.591594 topsearch-0.0.3/src/topsearch/potentials/dft.py
+-rw-r--r--   0        0        0     2792 2024-04-03 12:15:46.595412 topsearch-0.0.3/src/topsearch/potentials/force_fields.py
+-rw-r--r--   0        0        0     6658 2024-04-03 12:15:46.596768 topsearch-0.0.3/src/topsearch/potentials/gaussian_process.py
+-rw-r--r--   0        0        0     4745 2024-04-03 12:15:46.599963 topsearch-0.0.3/src/topsearch/potentials/ml_potentials.py
+-rw-r--r--   0        0        0     3928 2024-03-22 17:54:26.549618 topsearch-0.0.3/src/topsearch/potentials/potential.py
+-rw-r--r--   0        0        0     2538 2024-04-03 12:15:46.602995 topsearch-0.0.3/src/topsearch/potentials/test_functions.py
+-rw-r--r--   0        0        0        0 2024-02-05 17:05:09.605742 topsearch-0.0.3/src/topsearch/sampling/__init__.py
+-rw-r--r--   0        0        0      163 2024-02-05 17:05:09.606895 topsearch-0.0.3/src/topsearch/sampling/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    13538 2024-02-05 17:05:09.606553 topsearch-0.0.3/src/topsearch/sampling/__pycache__/exploration.cpython-310.pyc
+-rw-r--r--   0        0        0    19382 2024-03-04 16:51:13.107032 topsearch-0.0.3/src/topsearch/sampling/exploration.py
+-rw-r--r--   0        0        0        0 2024-02-05 17:05:09.607530 topsearch-0.0.3/src/topsearch/similarity/__init__.py
+-rw-r--r--   0        0        0      165 2024-02-05 17:05:09.609535 topsearch-0.0.3/src/topsearch/similarity/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     9129 2024-02-05 17:05:09.608729 topsearch-0.0.3/src/topsearch/similarity/__pycache__/molecular_similarity.cpython-310.pyc
+-rw-r--r--   0        0        0     5861 2024-02-05 17:05:09.609184 topsearch-0.0.3/src/topsearch/similarity/__pycache__/similarity.cpython-310.pyc
+-rw-r--r--   0        0        0    16788 2024-04-24 09:39:31.700522 topsearch-0.0.3/src/topsearch/similarity/molecular_similarity.py
+-rw-r--r--   0        0        0     7273 2024-04-03 12:15:46.607204 topsearch-0.0.3/src/topsearch/similarity/similarity.py
+-rw-r--r--   0        0        0        0 2024-02-05 17:05:09.612518 topsearch-0.0.3/src/topsearch/transition_states/__init__.py
+-rw-r--r--   0        0        0      172 2024-02-05 17:05:09.613615 topsearch-0.0.3/src/topsearch/transition_states/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    16885 2024-02-05 17:05:09.613978 topsearch-0.0.3/src/topsearch/transition_states/__pycache__/hybrid_eigenvector_following.cpython-310.pyc
+-rw-r--r--   0        0        0    11193 2024-02-05 17:05:09.613349 topsearch-0.0.3/src/topsearch/transition_states/__pycache__/nudged_elastic_band.cpython-310.pyc
+-rw-r--r--   0        0        0    28595 2024-03-22 17:54:26.550264 topsearch-0.0.3/src/topsearch/transition_states/hybrid_eigenvector_following.py
+-rw-r--r--   0        0        0    16750 2024-04-24 09:40:03.403782 topsearch-0.0.3/src/topsearch/transition_states/nudged_elastic_band.py
+-rw-r--r--   0        0        0     8515 1970-01-01 00:00:00.000000 topsearch-0.0.3/PKG-INFO
```

### Comparing `topsearch-0.0.2/LICENSE` & `topsearch-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/README.md` & `topsearch-0.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 <p align="center">
     <img src="./images/TopSearchLogo.png" height="390" width="390">
 </p>
 
 # TopSearch
 
-_This project is currently migrating to open source. Please check back regularly as more functionality is being added and updated_
-
 ## Introduction
 
 The TopSearch package provides functionality to map the topography of surfaces, and can be used to map the solution space of machine learning algorithms. Many machine learning algorithms have non-convex loss (or cost) functions, and the aim of fitting is usually to locate low-valued or diverse solutions. An understanding of the solution space organisation provides key understanding about the reproducibility, explainability and performance of ML methods. 
 
 The methodology derives from the field of chemical physics, and is agnostic to the given surface, allowing application to a wide range of machine learning algorithms. Leveraging ideas from chemical physics we can assess the performance and reliability of [neural networks](https://doi.org/10.1088/2632-2153/ac49a9), [Gaussian processes](https://arxiv.org/abs/2305.10748), Bayesian optimisation, [clustering algorithms](https://doi.org/10.1063/5.0078793) and understand the effect of [dataset roughness](https://doi.org/10.1039/D3ME00189J) on model performance. Application of the same framework to many different machine learning paradigms provides a route for transferable understanding, and its application to machine learning is reviewed in [this paper](https://doi.org/10.1039/D3DD00204G).
 
 ## Overview
@@ -30,20 +28,20 @@
 
 For more details of the methodology please refer to [`common_citations.md`](./common_citations.md).
 
 ## Installation
 
 Instructions are for installation into a conda environment. First create the conda environment
 ```
-conda create -n topsearch_env python=3.10
+conda create -n topsearch_env python=3.11
 conda activate topsearch_env
 ```
 The package is available on PyPI and can be installed using pip
 ```
-pip install topsearch==0.0.1
+pip install topsearch==0.0.2
 ```
 
 For the source code you can clone the git repository locally using
 ```
 git clone https://github.com/IBM/topography-searcher.git
 ```
 and then install the dependencies using either
```

### Comparing `topsearch-0.0.2/pyproject.toml` & `topsearch-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "topsearch"
-version = "0.0.2"
+version = "0.0.3"
 description = "A Python package for topographical analysis of machine learning models and physical systems"
 license = "MIT"
 authors = ["Luke Dicks <luke.dicks@ibm.com>"]
 readme = "README.md"
 keywords = ["machine-learning", "chemistry", "topography", "landscapes", "explainable-ai"]
 repository = "https://github.com/IBM/topography-searcher/"
```

### Comparing `topsearch-0.0.2/src/topsearch/analysis/__pycache__/batch_selection.cpython-310.pyc` & `topsearch-0.0.3/src/topsearch/analysis/__pycache__/batch_selection.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/analysis/__pycache__/graph_properties.cpython-310.pyc` & `topsearch-0.0.3/src/topsearch/analysis/__pycache__/graph_properties.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/analysis/__pycache__/minima_properties.cpython-310.pyc` & `topsearch-0.0.3/src/topsearch/analysis/__pycache__/minima_properties.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/analysis/__pycache__/pair_selection.cpython-310.pyc` & `topsearch-0.0.3/src/topsearch/analysis/__pycache__/pair_selection.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/analysis/__pycache__/roughness.cpython-310.pyc` & `topsearch-0.0.3/src/topsearch/analysis/__pycache__/roughness.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/analysis/batch_selection.py` & `topsearch-0.0.3/src/topsearch/analysis/batch_selection.py`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/analysis/graph_properties.py` & `topsearch-0.0.3/src/topsearch/analysis/graph_properties.py`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/analysis/minima_properties.py` & `topsearch-0.0.3/src/topsearch/analysis/minima_properties.py`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/analysis/pair_selection.py` & `topsearch-0.0.3/src/topsearch/analysis/pair_selection.py`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/analysis/roughness.py` & `topsearch-0.0.3/src/topsearch/analysis/roughness.py`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/data/__pycache__/coordinates.cpython-310.pyc` & `topsearch-0.0.3/src/topsearch/data/__pycache__/coordinates.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/data/__pycache__/kinetic_transition_network.cpython-310.pyc` & `topsearch-0.0.3/src/topsearch/data/__pycache__/kinetic_transition_network.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/data/__pycache__/model_data.cpython-310.pyc` & `topsearch-0.0.3/src/topsearch/data/__pycache__/model_data.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/data/coordinates.py` & `topsearch-0.0.3/src/topsearch/data/coordinates.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,14 +141,18 @@
                     adj_matrix[i][j] = 1
                     adj_matrix[j][i] = 1
         # Turns adjacency matrix into graph
         adj_graph = nx.from_numpy_array(adj_matrix)
         # Test if all nodes are connected
         return nx.is_connected(adj_graph)
 
+    def get_connected_atoms(self) -> list:
+        """ Get the connected atom labels of each atom in molecule """
+        return [['H']]*self.n_atoms
+
     def remove_atom_clashes(self):
         """ Routine to remove clashes between atoms that result in
             very large gradient and explosion of the cluster.
             Unused default parameter is for matching with other classes """
         centre_of_mass = np.array([np.average(self.position[0::3]),
                                    np.average(self.position[1::3]),
                                    np.average(self.position[2::3])])
@@ -237,14 +241,28 @@
             ref_bond_labels.append(sorted([self.atom_labels[u],
                                            self.atom_labels[v]]))
         # Compare the sorted lists of bonds to test similarity
         if sorted(current_bond_labels) == sorted(ref_bond_labels):
             return True
         return False
 
+    def get_connected_atoms(self) -> list:
+        """ Get the connected atom labels of each atom in molecule """
+        current_bonds = self.get_bonds()
+        bond_labels = []
+        # Loop over all atoms
+        for i in range(self.n_atoms):
+            labels_i = []
+            # Add the atom label for all connections out of node i
+            for j in current_bonds.edges(i):
+                labels_i.append(self.atom_labels[j[1]])
+            # Append to the list for each atom in turn
+            bond_labels.append(sorted(labels_i))
+        return bond_labels
+
     def get_planar_rings(self) -> list:
         """ Find the atoms that belong to a planar ring in the molecule """
         # Find closed loops in the system, which are rings
         loop_nodes = nx.cycle_basis(self.reference_bonds)
         ring_atoms = []
         # Check if each loop is planar
         for i in loop_nodes:
```

### Comparing `topsearch-0.0.2/src/topsearch/data/kinetic_transition_network.py` & `topsearch-0.0.3/src/topsearch/data/kinetic_transition_network.py`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/data/model_data.py` & `topsearch-0.0.3/src/topsearch/data/model_data.py`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/global_optimisation/__pycache__/basin_hopping.cpython-310.pyc` & `topsearch-0.0.3/src/topsearch/global_optimisation/__pycache__/basin_hopping.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/global_optimisation/__pycache__/perturbations.cpython-310.pyc` & `topsearch-0.0.3/src/topsearch/global_optimisation/__pycache__/perturbations.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/global_optimisation/basin_hopping.py` & `topsearch-0.0.3/src/topsearch/global_optimisation/basin_hopping.py`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/global_optimisation/perturbations.py` & `topsearch-0.0.3/src/topsearch/global_optimisation/perturbations.py`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/minimisation/__pycache__/lbfgs.cpython-310.pyc` & `topsearch-0.0.3/src/topsearch/minimisation/__pycache__/lbfgs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/minimisation/lbfgs.py` & `topsearch-0.0.3/src/topsearch/minimisation/lbfgs.py`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/plotting/__pycache__/disconnectivity.cpython-310.pyc` & `topsearch-0.0.3/src/topsearch/plotting/__pycache__/disconnectivity.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/plotting/__pycache__/network.cpython-310.pyc` & `topsearch-0.0.3/src/topsearch/plotting/__pycache__/network.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/plotting/__pycache__/stationary_points.cpython-310.pyc` & `topsearch-0.0.3/src/topsearch/plotting/__pycache__/stationary_points.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/plotting/disconnectivity.py` & `topsearch-0.0.3/src/topsearch/plotting/disconnectivity.py`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/plotting/network.py` & `topsearch-0.0.3/src/topsearch/plotting/network.py`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/plotting/stationary_points.py` & `topsearch-0.0.3/src/topsearch/plotting/stationary_points.py`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/potentials/__pycache__/atomic.cpython-310.pyc` & `topsearch-0.0.3/src/topsearch/potentials/__pycache__/atomic.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/potentials/__pycache__/bayesian_optimisation.cpython-310.pyc` & `topsearch-0.0.3/src/topsearch/potentials/__pycache__/bayesian_optimisation.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/potentials/__pycache__/dataset_fitting.cpython-310.pyc` & `topsearch-0.0.3/src/topsearch/potentials/__pycache__/dataset_fitting.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/potentials/__pycache__/dataset_regression.cpython-310.pyc` & `topsearch-0.0.3/src/topsearch/potentials/__pycache__/dataset_regression.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/potentials/__pycache__/dft.cpython-310.pyc` & `topsearch-0.0.3/src/topsearch/potentials/__pycache__/dft.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/potentials/__pycache__/force_fields.cpython-310.pyc` & `topsearch-0.0.3/src/topsearch/potentials/__pycache__/force_fields.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/potentials/__pycache__/gaussian_process.cpython-310.pyc` & `topsearch-0.0.3/src/topsearch/potentials/__pycache__/gaussian_process.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/potentials/__pycache__/ml_potentials.cpython-310.pyc` & `topsearch-0.0.3/src/topsearch/potentials/__pycache__/ml_potentials.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/potentials/__pycache__/molecular.cpython-310.pyc` & `topsearch-0.0.3/src/topsearch/potentials/__pycache__/molecular.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/potentials/__pycache__/potential.cpython-310.pyc` & `topsearch-0.0.3/src/topsearch/potentials/__pycache__/potential.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/potentials/__pycache__/test_functions.cpython-310-pytest-7.4.3.pyc` & `topsearch-0.0.3/src/topsearch/potentials/__pycache__/test_functions.cpython-310-pytest-7.4.3.pyc`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/potentials/__pycache__/test_functions.cpython-310.pyc` & `topsearch-0.0.3/src/topsearch/potentials/__pycache__/test_functions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/potentials/atomic.py` & `topsearch-0.0.3/src/topsearch/potentials/atomic.py`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/potentials/bayesian_optimisation.py` & `topsearch-0.0.3/src/topsearch/potentials/bayesian_optimisation.py`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/potentials/dataset_fitting.py` & `topsearch-0.0.3/src/topsearch/potentials/dataset_fitting.py`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/potentials/dft.py` & `topsearch-0.0.3/src/topsearch/potentials/dft.py`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/potentials/force_fields.py` & `topsearch-0.0.3/src/topsearch/potentials/force_fields.py`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/potentials/gaussian_process.py` & `topsearch-0.0.3/src/topsearch/potentials/gaussian_process.py`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/potentials/ml_potentials.py` & `topsearch-0.0.3/src/topsearch/potentials/ml_potentials.py`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/potentials/potential.py` & `topsearch-0.0.3/src/topsearch/potentials/potential.py`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/potentials/test_functions.py` & `topsearch-0.0.3/src/topsearch/potentials/test_functions.py`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/sampling/__pycache__/exploration.cpython-310.pyc` & `topsearch-0.0.3/src/topsearch/sampling/__pycache__/exploration.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/sampling/exploration.py` & `topsearch-0.0.3/src/topsearch/sampling/exploration.py`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/similarity/__pycache__/molecular_similarity.cpython-310.pyc` & `topsearch-0.0.3/src/topsearch/similarity/__pycache__/molecular_similarity.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/similarity/__pycache__/similarity.cpython-310.pyc` & `topsearch-0.0.3/src/topsearch/similarity/__pycache__/similarity.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/similarity/molecular_similarity.py` & `topsearch-0.0.3/src/topsearch/similarity/molecular_similarity.py`

 * *Files 18% similar despite different names*

```diff
@@ -43,42 +43,88 @@
         """ Hungarian algorithm adapted to solve the linear assignment problem
             for each atom of each distinct element. Finds the optimal
             permutation of all atoms respecting the atomic species """
         # Initialise permutation vector to track atom swaps
         permutation = np.zeros((coords1.n_atoms), dtype=int)
         # Copy second coordinates to leave unchanged
         permuted_coords = coords2.copy()
-        # Loop over each element to perform alignment w.r.t each in turn
-        elements = list(set(coords1.atom_labels))
-        for element in elements:
+        perm_group1, perm_group2 = self.get_permutable_groups(coords1, coords2)
+        # Loop over each perm group to perform alignment w.r.t each in turn
+        for i in range(len(perm_group1)):
             # Get atoms of the given element
-            element_atoms = \
-                [i for i, x in enumerate(coords1.atom_labels) if x == element]
-            if len(element_atoms) > 1:
+            perm_atoms1 = perm_group1[i]
+            perm_atoms2 = perm_group2[i]
+            if len(perm_atoms1) > 1:
                 # Get coordinates of just atoms of this element
                 coords1_element = np.take(coords1.position.reshape(-1, 3),
-                                          element_atoms, axis=0)
+                                          perm_atoms1, axis=0)
                 coords2_element = np.take(coords2.reshape(-1, 3),
-                                          element_atoms, axis=0)
+                                          perm_atoms2, axis=0)
                 # Calculate distance matrix for these subset of atoms
                 dist_matrix = distance_matrix(coords1_element,
                                               coords2_element)
                 # Optimal permutational alignment
                 col_ind = linear_sum_assignment(dist_matrix**2)[1]
                 # Update coordinates and permutation vector
-                for idx, atom in enumerate(element_atoms):
-                    permutation[atom] = element_atoms[col_ind[idx]]
+                for idx, atom in enumerate(perm_atoms1):
+                    permutation[atom] = perm_atoms1[col_ind[idx]]
                     permuted_coords[atom*3:(atom*3)+3] = \
-                        coords2[element_atoms[col_ind[idx]]*3:
-                                (element_atoms[col_ind[idx]]*3)+3]
+                        coords2[perm_atoms2[col_ind[idx]]*3:
+                                (perm_atoms2[col_ind[idx]]*3)+3]
             # Only one atom so no need for permutational alignment
             else:
-                permutation[element_atoms[0]] = element_atoms[0]
+                permutation[perm_atoms1[0]] = perm_atoms1[0]
         return permuted_coords, permutation
 
+    def get_permutable_groups(self, coords1: type, coords2: NDArray) -> list:
+        """ Determine the subsets of atoms that are allowed to be permuted
+            when minimising the distance between conformations. Must be
+            of the same element and have the same bonds """
+        # Initialise the sets of permutable atoms from coords1 and 2
+        permutable_groups1 = []
+        permutable_groups2 = []
+        # Get the connected species for each atom as we
+        # only want to allow permutation of atoms with same bonding
+        original_coords = coords1.position.copy()
+        bond_labels1 = coords1.get_connected_atoms()
+        coords1.position = coords2
+        bond_labels2 = coords1.get_connected_atoms()
+        coords1.position = original_coords
+        # Find the set of different elements in the molecule
+        elements = list(set(coords1.atom_labels))
+        # Loop over each species separately
+        for element in elements:
+            # Get each atom of a given element
+            element_atoms = \
+                [i for i, x in enumerate(coords1.atom_labels) if x == element]
+            # Initialise the arrays to store the connected atoms of each in set
+            elements_bonds1 = []
+            elements_bonds2 = []
+            # Loop over all atoms of element, adding their connections
+            for i in element_atoms:
+                elements_bonds1.append(bond_labels1[i])
+                elements_bonds2.append(bond_labels2[i])
+            # Find the unique set of environments for these atoms
+            unique_envs1 = \
+                list(set(tuple(sorted(row)) for row in elements_bonds1))
+            # Loop over each unique environment finding the atoms with it
+            for i in unique_envs1:
+                perm_atoms1 = []
+                perm_atoms2 = []
+                # Loop over all the atoms of this element checking which
+                # match the current environment
+                for j in element_atoms:
+                    if bond_labels1[j] == list(i):
+                        perm_atoms1.append(j)
+                    if bond_labels2[j] == list(i):
+                        perm_atoms2.append(j)
+                permutable_groups1.append(perm_atoms1)
+                permutable_groups2.append(perm_atoms2)
+        return permutable_groups1, permutable_groups2
+
     def rotational_alignment(self, coords1: type, coords2: NDArray) -> tuple:
         """ Find the rotation that minimises the distance between
             two sets of vectors using the Kabsch algorithm and apply it """
         if self.weighted:
             best_rotation, dist = \
                 rotations.align_vectors(coords1.position.reshape(-1, 3),
                                         coords2.reshape(-1, 3),
@@ -221,15 +267,15 @@
         if dist < self.distance_criterion:
             return dist, coords1, coords2_aligned, permutation
         # Not identical so try to find best permutation and rotation
         best_dist = dist
         best_coords2 = coords2_aligned
         best_perm = permutation
         # Iterate 50 times from different overall rotations
-        for i in range(50):
+        for i in range(150):
             coords2_rotated = self.random_rotation(coords2)
             dist, coords_opt, permutation = \
                 self.align(coords1, coords2_rotated)
             # If sufficiently close to be a match leave the loop early
             if dist < self.distance_criterion:
                 return dist, coords1, coords_opt, permutation
             # If an improvement on previous closest alignment then update
@@ -249,15 +295,15 @@
                 return dist, coords1, coords2_aligned, permutation
             # Not identical so try to find best permutation and rotation
             if dist < best_dist:
                 best_dist = dist
                 best_coords2 = coords2_aligned
                 best_perm = permutation
             # Iterate 50 times from different overall rotations
-            for i in range(50):
+            for i in range(150):
                 coords2_rotated = self.random_rotation(coords2)
                 dist, coords_opt, permutation = \
                     self.align(coords1, coords2_rotated)
                 # If sufficiently close to be a match leave the loop early
                 if dist < self.distance_criterion:
                     return dist, coords1, coords_opt, permutation
                 # If an improvement on previous closest alignment then update
```

### Comparing `topsearch-0.0.2/src/topsearch/similarity/similarity.py` & `topsearch-0.0.3/src/topsearch/similarity/similarity.py`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/transition_states/__pycache__/hybrid_eigenvector_following.cpython-310.pyc` & `topsearch-0.0.3/src/topsearch/transition_states/__pycache__/hybrid_eigenvector_following.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/transition_states/__pycache__/nudged_elastic_band.cpython-310.pyc` & `topsearch-0.0.3/src/topsearch/transition_states/__pycache__/nudged_elastic_band.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/transition_states/hybrid_eigenvector_following.py` & `topsearch-0.0.3/src/topsearch/transition_states/hybrid_eigenvector_following.py`

 * *Files identical despite different names*

### Comparing `topsearch-0.0.2/src/topsearch/transition_states/nudged_elastic_band.py` & `topsearch-0.0.3/src/topsearch/transition_states/nudged_elastic_band.py`

 * *Files 6% similar despite different names*

```diff
@@ -172,21 +172,23 @@
         bond_differences = (np.asarray(represent2[0]) -
                             np.asarray(represent1[1]))/(self.n_images-1)
         angle_differences = (np.asarray(represent2[1]) -
                              np.asarray(represent1[3]))/(self.n_images-1)
         dihedral_differences = []
         # Accounting for periodicity in dihedrals
         for i in range(len(represent1[5])):
-            plus_dist = np.abs(represent2[2][i] - represent1[5][i])
-            minus_dist = np.abs(represent2[2][i] + 360.0 - represent1[5][i])
-            if plus_dist < minus_dist:
-                dihedral_differences.append(represent2[2][i]-represent1[5][i])
+            dist1 = represent2[2][i] - represent1[5][i]
+            dist2 = dist1 + 360.0
+            dist3 = dist1 - 360.0
+            if np.abs(dist1) < np.abs(dist2) and np.abs(dist1) < np.abs(dist3):
+                dihedral_differences.append(dist1)
+            elif np.abs(dist2) < np.abs(dist1) and np.abs(dist2) < np.abs(dist3):
+                dihedral_differences.append(dist2)
             else:
-                dihedral_differences.append(represent2[2][i] + 360.0
-                                            - represent1[5][i])
+                dihedral_differences.append(dist3)
         dihedral_differences = \
             np.asarray(dihedral_differences)/(self.n_images-1)
         # Make the linear interpolation
         band = np.zeros((self.n_images, coords1.ndim), dtype=float)
         band[0, :] = coords1.position
         for i in range(1, self.n_images):
             coords1.change_bond_lengths(represent1[0],
```

### Comparing `topsearch-0.0.2/PKG-INFO` & `topsearch-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: topsearch
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python package for topographical analysis of machine learning models and physical systems
 Home-page: https://github.com/IBM/topography-searcher/
 License: MIT
 Keywords: machine-learning,chemistry,topography,landscapes,explainable-ai
 Author: Luke Dicks
 Author-email: luke.dicks@ibm.com
 Requires-Python: >=3.10,<3.13
@@ -26,16 +26,14 @@
 
 <p align="center">
     <img src="./images/TopSearchLogo.png" height="390" width="390">
 </p>
 
 # TopSearch
 
-_This project is currently migrating to open source. Please check back regularly as more functionality is being added and updated_
-
 ## Introduction
 
 The TopSearch package provides functionality to map the topography of surfaces, and can be used to map the solution space of machine learning algorithms. Many machine learning algorithms have non-convex loss (or cost) functions, and the aim of fitting is usually to locate low-valued or diverse solutions. An understanding of the solution space organisation provides key understanding about the reproducibility, explainability and performance of ML methods. 
 
 The methodology derives from the field of chemical physics, and is agnostic to the given surface, allowing application to a wide range of machine learning algorithms. Leveraging ideas from chemical physics we can assess the performance and reliability of [neural networks](https://doi.org/10.1088/2632-2153/ac49a9), [Gaussian processes](https://arxiv.org/abs/2305.10748), Bayesian optimisation, [clustering algorithms](https://doi.org/10.1063/5.0078793) and understand the effect of [dataset roughness](https://doi.org/10.1039/D3ME00189J) on model performance. Application of the same framework to many different machine learning paradigms provides a route for transferable understanding, and its application to machine learning is reviewed in [this paper](https://doi.org/10.1039/D3DD00204G).
 
 ## Overview
@@ -56,20 +54,20 @@
 
 For more details of the methodology please refer to [`common_citations.md`](./common_citations.md).
 
 ## Installation
 
 Instructions are for installation into a conda environment. First create the conda environment
 ```
-conda create -n topsearch_env python=3.10
+conda create -n topsearch_env python=3.11
 conda activate topsearch_env
 ```
 The package is available on PyPI and can be installed using pip
 ```
-pip install topsearch==0.0.1
+pip install topsearch==0.0.2
 ```
 
 For the source code you can clone the git repository locally using
 ```
 git clone https://github.com/IBM/topography-searcher.git
 ```
 and then install the dependencies using either
```

