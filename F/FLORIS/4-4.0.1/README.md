# Comparing `tmp/FLORIS-4.tar.gz` & `tmp/floris-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FLORIS-4.tar", last modified: Tue Apr  9 20:24:44 2024, max compression
+gzip compressed data, was "floris-4.0.1.tar", last modified: Wed Apr 24 20:44:03 2024, max compression
```

## Comparing `FLORIS-4.tar` & `floris-4.0.1.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:24:44.785059 FLORIS-4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:24:44.781059 FLORIS-4/FLORIS.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-09 20:24:44.000000 FLORIS-4/FLORIS.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-09 20:24:44.000000 FLORIS-4/FLORIS.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 20:24:44.000000 FLORIS-4/FLORIS.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-09 20:24:44.000000 FLORIS-4/FLORIS.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 20:24:44.000000 FLORIS-4/FLORIS.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-09 20:24:34.000000 FLORIS-4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-09 20:24:44.785059 FLORIS-4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7682 2024-04-09 20:24:34.000000 FLORIS-4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:24:44.761059 FLORIS-4/floris/
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-09 20:24:34.000000 FLORIS-4/floris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-09 20:24:34.000000 FLORIS-4/floris/convert_floris_input_v3_to_v4.py
--rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-04-09 20:24:34.000000 FLORIS-4/floris/convert_turbine_v3_to_v4.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:24:44.765059 FLORIS-4/floris/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    15986 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    20841 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/farm.py
--rw-r--r--   0 runner    (1001) docker     (127)    13505 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/flow_field.py
--rw-r--r--   0 runner    (1001) docker     (127)    35084 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     9070 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/rotor_velocity.py
--rw-r--r--   0 runner    (1001) docker     (127)    62372 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/solver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:24:44.765059 FLORIS-4/floris/core/turbine/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/turbine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22052 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/turbine/operation_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    28768 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/turbine/turbine.py
--rw-r--r--   0 runner    (1001) docker     (127)     5807 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/wake.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:24:44.765059 FLORIS-4/floris/core/wake_combination/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/wake_combination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/wake_combination/fls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/wake_combination/max.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/wake_combination/sosfs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:24:44.765059 FLORIS-4/floris/core/wake_deflection/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/wake_deflection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/wake_deflection/empirical_gauss.py
--rw-r--r--   0 runner    (1001) docker     (127)    17284 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/wake_deflection/gauss.py
--rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/wake_deflection/jimenez.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/wake_deflection/none.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:24:44.765059 FLORIS-4/floris/core/wake_turbulence/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/wake_turbulence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/wake_turbulence/crespo_hernandez.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/wake_turbulence/none.py
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/wake_turbulence/wake_induced_mixing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:24:44.769059 FLORIS-4/floris/core/wake_velocity/
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/wake_velocity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6965 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/wake_velocity/cumulative_gauss_curl.py
--rw-r--r--   0 runner    (1001) docker     (127)    10851 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/wake_velocity/empirical_gauss.py
--rw-r--r--   0 runner    (1001) docker     (127)     8254 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/wake_velocity/gauss.py
--rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/wake_velocity/jensen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/wake_velocity/none.py
--rw-r--r--   0 runner    (1001) docker     (127)     6389 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/wake_velocity/turbopark.py
--rw-r--r--   0 runner    (1001) docker     (127)  9163212 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/wake_velocity/turbopark_lookup_table.mat
--rw-r--r--   0 runner    (1001) docker     (127)    13916 2024-04-09 20:24:34.000000 FLORIS-4/floris/cut_plane.py
--rw-r--r--   0 runner    (1001) docker     (127)    71608 2024-04-09 20:24:34.000000 FLORIS-4/floris/floris_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    29230 2024-04-09 20:24:34.000000 FLORIS-4/floris/flow_visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)    21418 2024-04-09 20:24:34.000000 FLORIS-4/floris/layout_visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-04-09 20:24:34.000000 FLORIS-4/floris/logging_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:24:44.777059 FLORIS-4/floris/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-09 20:24:34.000000 FLORIS-4/floris/optimization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:24:44.781059 FLORIS-4/floris/optimization/layout_optimization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 20:24:34.000000 FLORIS-4/floris/optimization/layout_optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-04-09 20:24:34.000000 FLORIS-4/floris/optimization/layout_optimization/layout_optimization_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    23715 2024-04-09 20:24:34.000000 FLORIS-4/floris/optimization/layout_optimization/layout_optimization_boundary_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     8786 2024-04-09 20:24:34.000000 FLORIS-4/floris/optimization/layout_optimization/layout_optimization_pyoptsparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     7230 2024-04-09 20:24:34.000000 FLORIS-4/floris/optimization/layout_optimization/layout_optimization_pyoptsparse_spread.py
--rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-04-09 20:24:34.000000 FLORIS-4/floris/optimization/layout_optimization/layout_optimization_scipy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:24:44.781059 FLORIS-4/floris/optimization/other/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-09 20:24:34.000000 FLORIS-4/floris/optimization/other/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12797 2024-04-09 20:24:34.000000 FLORIS-4/floris/optimization/other/boundary_grid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:24:44.781059 FLORIS-4/floris/optimization/yaw_optimization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 20:24:34.000000 FLORIS-4/floris/optimization/yaw_optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28535 2024-04-09 20:24:34.000000 FLORIS-4/floris/optimization/yaw_optimization/yaw_optimization_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-04-09 20:24:34.000000 FLORIS-4/floris/optimization/yaw_optimization/yaw_optimization_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     9205 2024-04-09 20:24:34.000000 FLORIS-4/floris/optimization/yaw_optimization/yaw_optimizer_geometric.py
--rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-04-09 20:24:34.000000 FLORIS-4/floris/optimization/yaw_optimization/yaw_optimizer_scipy.py
--rw-r--r--   0 runner    (1001) docker     (127)    13219 2024-04-09 20:24:34.000000 FLORIS-4/floris/optimization/yaw_optimization/yaw_optimizer_sr.py
--rw-r--r--   0 runner    (1001) docker     (127)    22700 2024-04-09 20:24:34.000000 FLORIS-4/floris/parallel_floris_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:24:44.781059 FLORIS-4/floris/turbine_library/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-09 20:24:34.000000 FLORIS-4/floris/turbine_library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-09 20:24:34.000000 FLORIS-4/floris/turbine_library/iea_10MW.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-09 20:24:34.000000 FLORIS-4/floris/turbine_library/iea_15MW.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-09 20:24:34.000000 FLORIS-4/floris/turbine_library/iea_15MW_floating_multi_dim_cp_ct.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-09 20:24:34.000000 FLORIS-4/floris/turbine_library/iea_15MW_multi_dim_cp_ct.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-04-09 20:24:34.000000 FLORIS-4/floris/turbine_library/nrel_5MW.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    34909 2024-04-09 20:24:34.000000 FLORIS-4/floris/turbine_library/turbine_previewer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-04-09 20:24:34.000000 FLORIS-4/floris/turbine_library/turbine_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-04-09 20:24:34.000000 FLORIS-4/floris/type_dec.py
--rw-r--r--   0 runner    (1001) docker     (127)    36981 2024-04-09 20:24:34.000000 FLORIS-4/floris/uncertain_floris_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10222 2024-04-09 20:24:34.000000 FLORIS-4/floris/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-09 20:24:34.000000 FLORIS-4/floris/version.py
--rw-r--r--   0 runner    (1001) docker     (127)   104097 2024-04-09 20:24:34.000000 FLORIS-4/floris/wind_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-04-09 20:24:34.000000 FLORIS-4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 20:24:44.785059 FLORIS-4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-09 20:24:34.000000 FLORIS-4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:44:03.651120 floris-4.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:44:03.651120 floris-4.0.1/FLORIS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-24 20:44:03.000000 floris-4.0.1/FLORIS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-24 20:44:03.000000 floris-4.0.1/FLORIS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 20:44:03.000000 floris-4.0.1/FLORIS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-24 20:44:03.000000 floris-4.0.1/FLORIS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 20:44:03.000000 floris-4.0.1/FLORIS.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-24 20:43:55.000000 floris-4.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-24 20:44:03.651120 floris-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7634 2024-04-24 20:43:55.000000 floris-4.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:44:03.631120 floris-4.0.1/floris/
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-24 20:43:55.000000 floris-4.0.1/floris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-04-24 20:43:55.000000 floris-4.0.1/floris/convert_floris_input_v3_to_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-04-24 20:43:55.000000 floris-4.0.1/floris/convert_turbine_v3_to_v4.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:44:03.631120 floris-4.0.1/floris/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-24 20:43:55.000000 floris-4.0.1/floris/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-24 20:43:55.000000 floris-4.0.1/floris/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15986 2024-04-24 20:43:55.000000 floris-4.0.1/floris/core/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20839 2024-04-24 20:43:55.000000 floris-4.0.1/floris/core/farm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13505 2024-04-24 20:43:55.000000 floris-4.0.1/floris/core/flow_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35077 2024-04-24 20:43:55.000000 floris-4.0.1/floris/core/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9070 2024-04-24 20:43:55.000000 floris-4.0.1/floris/core/rotor_velocity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62372 2024-04-24 20:43:55.000000 floris-4.0.1/floris/core/solver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:44:03.631120 floris-4.0.1/floris/core/turbine/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-24 20:43:55.000000 floris-4.0.1/floris/core/turbine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22052 2024-04-24 20:43:55.000000 floris-4.0.1/floris/core/turbine/operation_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28768 2024-04-24 20:43:55.000000 floris-4.0.1/floris/core/turbine/turbine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5807 2024-04-24 20:43:55.000000 floris-4.0.1/floris/core/wake.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:44:03.635120 floris-4.0.1/floris/core/wake_combination/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-24 20:43:55.000000 floris-4.0.1/floris/core/wake_combination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-24 20:43:55.000000 floris-4.0.1/floris/core/wake_combination/fls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-24 20:43:55.000000 floris-4.0.1/floris/core/wake_combination/max.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-24 20:43:55.000000 floris-4.0.1/floris/core/wake_combination/sosfs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:44:03.635120 floris-4.0.1/floris/core/wake_deflection/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-24 20:43:55.000000 floris-4.0.1/floris/core/wake_deflection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-04-24 20:43:55.000000 floris-4.0.1/floris/core/wake_deflection/empirical_gauss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17284 2024-04-24 20:43:55.000000 floris-4.0.1/floris/core/wake_deflection/gauss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-04-24 20:43:55.000000 floris-4.0.1/floris/core/wake_deflection/jimenez.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-24 20:43:55.000000 floris-4.0.1/floris/core/wake_deflection/none.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:44:03.635120 floris-4.0.1/floris/core/wake_turbulence/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-24 20:43:55.000000 floris-4.0.1/floris/core/wake_turbulence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-24 20:43:55.000000 floris-4.0.1/floris/core/wake_turbulence/crespo_hernandez.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-24 20:43:55.000000 floris-4.0.1/floris/core/wake_turbulence/none.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-24 20:43:55.000000 floris-4.0.1/floris/core/wake_turbulence/wake_induced_mixing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:44:03.635120 floris-4.0.1/floris/core/wake_velocity/
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-24 20:43:55.000000 floris-4.0.1/floris/core/wake_velocity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6965 2024-04-24 20:43:55.000000 floris-4.0.1/floris/core/wake_velocity/cumulative_gauss_curl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10851 2024-04-24 20:43:55.000000 floris-4.0.1/floris/core/wake_velocity/empirical_gauss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8254 2024-04-24 20:43:55.000000 floris-4.0.1/floris/core/wake_velocity/gauss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-04-24 20:43:55.000000 floris-4.0.1/floris/core/wake_velocity/jensen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-24 20:43:55.000000 floris-4.0.1/floris/core/wake_velocity/none.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6389 2024-04-24 20:43:55.000000 floris-4.0.1/floris/core/wake_velocity/turbopark.py
+-rw-r--r--   0 runner    (1001) docker     (127)  9163212 2024-04-24 20:43:55.000000 floris-4.0.1/floris/core/wake_velocity/turbopark_lookup_table.mat
+-rw-r--r--   0 runner    (1001) docker     (127)    13916 2024-04-24 20:43:55.000000 floris-4.0.1/floris/cut_plane.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71608 2024-04-24 20:43:55.000000 floris-4.0.1/floris/floris_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29230 2024-04-24 20:43:55.000000 floris-4.0.1/floris/flow_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21418 2024-04-24 20:43:55.000000 floris-4.0.1/floris/layout_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-04-24 20:43:55.000000 floris-4.0.1/floris/logging_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:44:03.647120 floris-4.0.1/floris/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-24 20:43:55.000000 floris-4.0.1/floris/optimization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:44:03.647120 floris-4.0.1/floris/optimization/layout_optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:43:55.000000 floris-4.0.1/floris/optimization/layout_optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-04-24 20:43:55.000000 floris-4.0.1/floris/optimization/layout_optimization/layout_optimization_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23715 2024-04-24 20:43:55.000000 floris-4.0.1/floris/optimization/layout_optimization/layout_optimization_boundary_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8786 2024-04-24 20:43:55.000000 floris-4.0.1/floris/optimization/layout_optimization/layout_optimization_pyoptsparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7230 2024-04-24 20:43:55.000000 floris-4.0.1/floris/optimization/layout_optimization/layout_optimization_pyoptsparse_spread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-04-24 20:43:55.000000 floris-4.0.1/floris/optimization/layout_optimization/layout_optimization_scipy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:44:03.647120 floris-4.0.1/floris/optimization/other/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-24 20:43:55.000000 floris-4.0.1/floris/optimization/other/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12797 2024-04-24 20:43:55.000000 floris-4.0.1/floris/optimization/other/boundary_grid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:44:03.651120 floris-4.0.1/floris/optimization/yaw_optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:43:55.000000 floris-4.0.1/floris/optimization/yaw_optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28535 2024-04-24 20:43:55.000000 floris-4.0.1/floris/optimization/yaw_optimization/yaw_optimization_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-04-24 20:43:55.000000 floris-4.0.1/floris/optimization/yaw_optimization/yaw_optimization_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9205 2024-04-24 20:43:55.000000 floris-4.0.1/floris/optimization/yaw_optimization/yaw_optimizer_geometric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-04-24 20:43:55.000000 floris-4.0.1/floris/optimization/yaw_optimization/yaw_optimizer_scipy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13219 2024-04-24 20:43:55.000000 floris-4.0.1/floris/optimization/yaw_optimization/yaw_optimizer_sr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22700 2024-04-24 20:43:55.000000 floris-4.0.1/floris/parallel_floris_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:44:03.651120 floris-4.0.1/floris/turbine_library/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-24 20:43:55.000000 floris-4.0.1/floris/turbine_library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-24 20:43:55.000000 floris-4.0.1/floris/turbine_library/iea_10MW.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-24 20:43:55.000000 floris-4.0.1/floris/turbine_library/iea_15MW.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-24 20:43:55.000000 floris-4.0.1/floris/turbine_library/iea_15MW_floating_multi_dim_cp_ct.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-24 20:43:55.000000 floris-4.0.1/floris/turbine_library/iea_15MW_multi_dim_cp_ct.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-04-24 20:43:55.000000 floris-4.0.1/floris/turbine_library/nrel_5MW.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    34909 2024-04-24 20:43:55.000000 floris-4.0.1/floris/turbine_library/turbine_previewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-04-24 20:43:55.000000 floris-4.0.1/floris/turbine_library/turbine_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-04-24 20:43:55.000000 floris-4.0.1/floris/type_dec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36981 2024-04-24 20:43:55.000000 floris-4.0.1/floris/uncertain_floris_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10222 2024-04-24 20:43:55.000000 floris-4.0.1/floris/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 20:43:55.000000 floris-4.0.1/floris/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)   104097 2024-04-24 20:43:55.000000 floris-4.0.1/floris/wind_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-04-24 20:43:55.000000 floris-4.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 20:44:03.651120 floris-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-24 20:43:55.000000 floris-4.0.1/setup.py
```

### Comparing `FLORIS-4/FLORIS.egg-info/PKG-INFO` & `floris-4.0.1/FLORIS.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FLORIS
-Version: 4
+Version: 4.0.1
 Summary: A controls-oriented engineering wake model.
 Home-page: https://github.com/NREL/FLORIS
 Author: NREL National Wind Technology Center
 Author-email: rafael.mudafort@nrel.gov
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -22,19 +22,19 @@
 Requires-Dist: numpy~=1.20
 Requires-Dist: scipy~=1.1
 Requires-Dist: matplotlib~=3.0
 Requires-Dist: pandas~=2.0
 Requires-Dist: shapely~=2.0
 Requires-Dist: coloredlogs~=10.0
 Provides-Extra: docs
-Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
+Requires-Dist: sphinxcontrib.mermaid; extra == "docs"
 Requires-Dist: sphinxcontrib-autoyaml; extra == "docs"
 Requires-Dist: sphinx-book-theme; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
 Requires-Dist: jupyter-book; extra == "docs"
-Requires-Dist: sphinxcontrib.mermaid; extra == "docs"
 Provides-Extra: develop
 Requires-Dist: pre-commit; extra == "develop"
 Requires-Dist: pytest; extra == "develop"
 Requires-Dist: isort; extra == "develop"
 Requires-Dist: ruff; extra == "develop"
 
 A controls-oriented engineering wake model.
```

### Comparing `FLORIS-4/FLORIS.egg-info/SOURCES.txt` & `floris-4.0.1/FLORIS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FLORIS-4/LICENSE.txt` & `floris-4.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `FLORIS-4/PKG-INFO` & `floris-4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FLORIS
-Version: 4
+Version: 4.0.1
 Summary: A controls-oriented engineering wake model.
 Home-page: https://github.com/NREL/FLORIS
 Author: NREL National Wind Technology Center
 Author-email: rafael.mudafort@nrel.gov
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -22,19 +22,19 @@
 Requires-Dist: numpy~=1.20
 Requires-Dist: scipy~=1.1
 Requires-Dist: matplotlib~=3.0
 Requires-Dist: pandas~=2.0
 Requires-Dist: shapely~=2.0
 Requires-Dist: coloredlogs~=10.0
 Provides-Extra: docs
-Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
+Requires-Dist: sphinxcontrib.mermaid; extra == "docs"
 Requires-Dist: sphinxcontrib-autoyaml; extra == "docs"
 Requires-Dist: sphinx-book-theme; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
 Requires-Dist: jupyter-book; extra == "docs"
-Requires-Dist: sphinxcontrib.mermaid; extra == "docs"
 Provides-Extra: develop
 Requires-Dist: pre-commit; extra == "develop"
 Requires-Dist: pytest; extra == "develop"
 Requires-Dist: isort; extra == "develop"
 Requires-Dist: ruff; extra == "develop"
 
 A controls-oriented engineering wake model.
```

### Comparing `FLORIS-4/README.md` & `floris-4.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # FLORIS Wake Modeling and Wind Farm Controls Software
 
 FLORIS is a controls-focused wind farm simulation software incorporating
 steady-state engineering wake models into a performance-focused Python
 framework. It has been in active development at NREL since 2013 and the latest
-release is [FLORIS v4.0](https://github.com/NREL/floris/releases/latest).
+release is [FLORIS v4.0.1](https://github.com/NREL/floris/releases/latest).
 Online documentation is available at https://nrel.github.io/floris.
 
 The software is in active development and engagement with the development team
 is highly encouraged. If you are interested in using FLORIS to conduct studies
 of a wind farm or extending FLORIS to include your own wake model, please join
 the conversation in [GitHub Discussions](https://github.com/NREL/floris/discussions/)!
 
@@ -88,54 +88,54 @@
 It is important to regularly check for new updates and releases as new
 features, improvements, and bug fixes will be issued on an ongoing basis.
 
 ## Quick Start
 
 FLORIS is a Python package run on the command line typically by providing
 an input file with an initial configuration. It can be installed with
-```pip install floris``` (see [installation](https://github.nrel.io/floris/installation)).
+```pip install floris``` (see [installation](https://nrel.github.io/floris/installation.html)).
 The typical entry point is
-[FlorisModel](https://nrel.github.io/floris/_autosummary/floris.floris_model.FlorisModel.html#floris.floris_model.FlorisModel)
+[FlorisModel](https://nrel.github.io/floris/_autosummary/floris.floris_model.html)
 which accepts the path to the input file as an argument. From there,
 changes can be made to the initial configuration through the
-[FlorisModel.set](https://nrel.github.io/floris/_autosummary/floris.floris_model.FlorisModel.html#floris.floris_model.FlorisModel.set)
+[FlorisModel.set](https://nrel.github.io/floris/_autosummary/floris.floris_model.html#floris.floris_model.FlorisModel.set)
 routine, and the simulation is executed with
-[FlorisModel.run](https://nrel.github.io/floris/_autosummary/floris.floris_model.FlorisModel.html#floris.floris_model.FlorisModel.run).
+[FlorisModel.run](https://nrel.github.io/floris/_autosummary/floris.floris_model.html#floris.floris_model.FlorisModel.run).
 
 ```python
 from floris import FlorisModel
 fmodel = FlorisModel("path/to/input.yaml")
 fmodel.set(
     wind_directions=[i for i in range(10)],
     wind_speeds=[8.0]*10,
     turbulence_intensities=[0.06]*10
 )
 fmodel.run()
 ```
 
 Finally, results can be analyzed via post-processing functions available within
-[FlorisModel](https://nrel.github.io/floris/_autosummary/floris.floris_model.FlorisModel.html#floris.floris_model.FlorisModel)
+[FlorisModel](https://nrel.github.io/floris/_autosummary/floris.floris_model.html#floris.floris_model.FlorisModel)
 such as
-- [FlorisModel.get_turbine_layout](https://nrel.github.io/floris/_autosummary/floris.floris_model.FlorisModel.html#floris.floris_model.FlorisModel.get_turbine_layout)
-- [FlorisModel.get_turbine_powers](https://nrel.github.io/floris/_autosummary/floris.floris_model.FlorisModel.html#floris.floris_model.FlorisModel.get_turbine_powers)
-- [FlorisModel.get_farm_AEP](https://nrel.github.io/floris/_autosummary/floris.floris_model.FlorisModel.html#floris.floris_model.FlorisModel.get_farm_AEP)
+- [FlorisModel.get_turbine_layout](https://nrel.github.io/floris/_autosummary/floris.floris_model.html#floris.floris_model.FlorisModel.get_turbine_layout)
+- [FlorisModel.get_turbine_powers](https://nrel.github.io/floris/_autosummary/floris.floris_model.html#floris.floris_model.FlorisModel.get_turbine_powers)
+- [FlorisModel.get_farm_AEP](https://nrel.github.io/floris/_autosummary/floris.floris_model.html#floris.floris_model.FlorisModel.get_farm_AEP)
 
 and in two visualization packages: [layoutviz](https://nrel.github.io/floris/_autosummary/floris.layout_visualization.html) and [flowviz](https://nrel.github.io/floris/_autosummary/floris.flow_visualization.html).
 A collection of examples describing the creation of simulations as well as
 analysis and post processing are included in the
-[repository](https://github.com/NREL/floris/tree/main/examples)
-and described in [Examples Index](https://github.nrel.io/floris/examples).
+[repository](https://github.com/NREL/floris/tree/main/examples). Examples are also listed
+in the [online documentation](https://nrel.github.io/floris/examples/001_opening_floris_computing_power.html).
 
 ## Engaging on GitHub
 
 FLORIS leverages the following GitHub features to coordinate support and development efforts:
 
 - [Discussions](https://github.com/NREL/floris/discussions): Collaborate to develop ideas for new use cases, features, and software designs, and get support for usage questions
 - [Issues](https://github.com/NREL/floris/issues): Report potential bugs and well-developed feature requests
-- [Projects](https://github.com/orgs/NREL/projects/18/): Include current and future work on a timeline and assign a person to "own" it
+- [Projects](https://github.com/orgs/NREL/projects/96): Include current and future work on a timeline and assign a person to "own" it
 
 Generally, the first entry point for the community will be within one of the
 categories in Discussions.
 [Ideas](https://github.com/NREL/floris/discussions/categories/ideas) is a great spot to develop the
 details for a feature request. [Q&A](https://github.com/NREL/floris/discussions/categories/q-a)
 is where to get usage support.
 [Show and tell](https://github.com/NREL/floris/discussions/categories/show-and-tell) is a free-form
```

### Comparing `FLORIS-4/floris/convert_floris_input_v3_to_v4.py` & `floris-4.0.1/floris/convert_floris_input_v3_to_v4.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,14 +57,17 @@
             + "turbines in FLORIS v4. "
             + "You will also need to convert your multidimensional turbine yaml files and their "
             + "corresponding power/thrust csv files to be compatible with FLORIS v4 and to reflect "
             + " the absolute power curve, rather than the power coefficient curve."
         )
         v4_floris_input_dict["wake"]["model_strings"]["velocity_model"] = "gauss"
 
+    # Add enable_active_wake_mixing field
+    v4_floris_input_dict["wake"]["enable_active_wake_mixing"] = False
+
     yaml.dump(
             v4_floris_input_dict,
             open(output_path, "w"),
             sort_keys=False
         )
 
     print(output_path, "created.")
```

### Comparing `FLORIS-4/floris/convert_turbine_v3_to_v4.py` & `floris-4.0.1/floris/convert_turbine_v3_to_v4.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/core/__init__.py` & `floris-4.0.1/floris/core/__init__.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/core/base.py` & `floris-4.0.1/floris/core/base.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/core/core.py` & `floris-4.0.1/floris/core/core.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/core/farm.py` & `floris-4.0.1/floris/core/farm.py`

 * *Files 0% similar despite different names*

```diff
@@ -461,15 +461,15 @@
 
     @property
     def coordinates(self):
         return np.array([
             np.array([x, y, z]) for x, y, z in zip(
                 self.layout_x,
                 self.layout_y,
-                self.hub_heights if len(self.hub_heights.shape) == 1 else self.hub_heights[0,0]
+                self.hub_heights if len(self.hub_heights.shape) == 1 else self.hub_heights[0]
             )
         ])
 
     @property
     def n_turbines(self):
         return len(self.layout_x)
```

### Comparing `FLORIS-4/floris/core/flow_field.py` & `floris-4.0.1/floris/core/flow_field.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/core/grid.py` & `floris-4.0.1/floris/core/grid.py`

 * *Files 1% similar despite different names*

```diff
@@ -313,41 +313,44 @@
                 self.n_findex,
                 self.n_turbines,
                 len(yv),  # Number of coordinates
                 1,
             ),
             dtype=floris_float_type
         )
-        _x = x[:, :, :, None, None] * template_grid
-        _y = y[:, :, :, None, None] * template_grid
-        _z = z[:, :, :, None, None] * template_grid
+        _x = x[:, :, None, None] * template_grid
+        _y = y[:, :, None, None] * template_grid
+        _z = z[:, :, None, None] * template_grid
+
+        n_coordinates = len(yv)
+        yv = np.broadcast_to(yv, (self.n_findex, self.n_turbines, n_coordinates))
+        yv = np.expand_dims(yv, axis=-1)
+        zv = np.broadcast_to(zv, (self.n_findex, self.n_turbines, n_coordinates))
+        zv = np.expand_dims(zv, axis=-1)
+
         for ti in range(self.n_turbines):
-            _y[:, :, ti, :, :] += yv[None, None, :, None]*self.turbine_diameters[ti] / 2.0
-            _z[:, :, ti, :, :] += zv[None, None, :, None]*self.turbine_diameters[ti] / 2.0
+            _y[:, ti, :, :] += yv[:, ti] * self.turbine_diameters[ti] / 2.0
+            _z[:, ti, :, :] += zv[:, ti] * self.turbine_diameters[ti] / 2.0
 
         # Sort the turbines at each wind direction
 
         # Get the sorted indices for the x coordinates. These are the indices
         # to sort the turbines from upstream to downstream for all wind directions.
         # Also, store the indices to sort them back for when the calculation finishes.
-        self.sorted_indices = _x.argsort(axis=2)
-        self.sorted_coord_indices = x.argsort(axis=2)
-        self.unsorted_indices = self.sorted_indices.argsort(axis=2)
+        self.sorted_indices = _x.argsort(axis=1)
+        self.sorted_coord_indices = x.argsort(axis=1)
+        self.unsorted_indices = self.sorted_indices.argsort(axis=1)
 
         # Put the turbine coordinates into the final arrays in their sorted order
         # These are the coordinates that should be used within the internal calculations
         # such as the wake models and the solvers.
         self.x_sorted = np.take_along_axis(_x, self.sorted_indices, axis=1)
         self.y_sorted = np.take_along_axis(_y, self.sorted_indices, axis=1)
         self.z_sorted = np.take_along_axis(_z, self.sorted_indices, axis=1)
 
-        self.x = np.take_along_axis(self.x_sorted, self.unsorted_indices, axis=1)
-        self.y = np.take_along_axis(self.y_sorted, self.unsorted_indices, axis=1)
-        self.z = np.take_along_axis(self.z_sorted, self.unsorted_indices, axis=1)
-
     @classmethod
     def get_cubature_coefficients(cls, N: int):
         """
         Retrieve cubature integration coefficients. This is a class-method, and therefore
         the coefficients can be accessed without creating an instance of the class.
 
         Args:
@@ -355,15 +358,15 @@
             number of rotor points will be N^2. Must be an integer in the range [1, 10].
 
         Returns:
             cubature_coefficients (dict): A dictionary containing the cubature
             integration coefficients, "r", "t", "q", "A" and "B".
         """
 
-        if N < 1 and N < 10:
+        if N < 1 or N > 10:
             raise ValueError(
                 f"Order of cubature integration must be between '1' and '10', given {N}."
             )
 
         elif N == 1:
             r = [0.0000000000000000000000000]
             t = [0.0000000000000000000000000]
```

### Comparing `FLORIS-4/floris/core/rotor_velocity.py` & `floris-4.0.1/floris/core/rotor_velocity.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/core/solver.py` & `floris-4.0.1/floris/core/solver.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/core/turbine/operation_models.py` & `floris-4.0.1/floris/core/turbine/operation_models.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/core/turbine/turbine.py` & `floris-4.0.1/floris/core/turbine/turbine.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/core/wake.py` & `floris-4.0.1/floris/core/wake.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/core/wake_combination/fls.py` & `floris-4.0.1/floris/core/wake_combination/fls.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/core/wake_combination/max.py` & `floris-4.0.1/floris/core/wake_combination/max.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/core/wake_combination/sosfs.py` & `floris-4.0.1/floris/core/wake_combination/sosfs.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/core/wake_deflection/empirical_gauss.py` & `floris-4.0.1/floris/core/wake_deflection/empirical_gauss.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/core/wake_deflection/gauss.py` & `floris-4.0.1/floris/core/wake_deflection/gauss.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/core/wake_deflection/jimenez.py` & `floris-4.0.1/floris/core/wake_deflection/jimenez.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/core/wake_deflection/none.py` & `floris-4.0.1/floris/core/wake_deflection/none.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/core/wake_turbulence/crespo_hernandez.py` & `floris-4.0.1/floris/core/wake_turbulence/crespo_hernandez.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/core/wake_turbulence/none.py` & `floris-4.0.1/floris/core/wake_turbulence/none.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/core/wake_turbulence/wake_induced_mixing.py` & `floris-4.0.1/floris/core/wake_turbulence/wake_induced_mixing.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/core/wake_velocity/cumulative_gauss_curl.py` & `floris-4.0.1/floris/core/wake_velocity/cumulative_gauss_curl.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/core/wake_velocity/empirical_gauss.py` & `floris-4.0.1/floris/core/wake_velocity/empirical_gauss.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/core/wake_velocity/gauss.py` & `floris-4.0.1/floris/core/wake_velocity/gauss.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/core/wake_velocity/jensen.py` & `floris-4.0.1/floris/core/wake_velocity/jensen.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/core/wake_velocity/none.py` & `floris-4.0.1/floris/core/wake_velocity/none.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/core/wake_velocity/turbopark.py` & `floris-4.0.1/floris/core/wake_velocity/turbopark.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/core/wake_velocity/turbopark_lookup_table.mat` & `floris-4.0.1/floris/core/wake_velocity/turbopark_lookup_table.mat`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/cut_plane.py` & `floris-4.0.1/floris/cut_plane.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/floris_model.py` & `floris-4.0.1/floris/floris_model.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/flow_visualization.py` & `floris-4.0.1/floris/flow_visualization.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/layout_visualization.py` & `floris-4.0.1/floris/layout_visualization.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/logging_manager.py` & `floris-4.0.1/floris/logging_manager.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/optimization/layout_optimization/layout_optimization_base.py` & `floris-4.0.1/floris/optimization/layout_optimization/layout_optimization_base.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/optimization/layout_optimization/layout_optimization_boundary_grid.py` & `floris-4.0.1/floris/optimization/layout_optimization/layout_optimization_boundary_grid.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/optimization/layout_optimization/layout_optimization_pyoptsparse.py` & `floris-4.0.1/floris/optimization/layout_optimization/layout_optimization_pyoptsparse.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/optimization/layout_optimization/layout_optimization_pyoptsparse_spread.py` & `floris-4.0.1/floris/optimization/layout_optimization/layout_optimization_pyoptsparse_spread.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/optimization/layout_optimization/layout_optimization_scipy.py` & `floris-4.0.1/floris/optimization/layout_optimization/layout_optimization_scipy.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/optimization/other/boundary_grid.py` & `floris-4.0.1/floris/optimization/other/boundary_grid.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/optimization/yaw_optimization/yaw_optimization_base.py` & `floris-4.0.1/floris/optimization/yaw_optimization/yaw_optimization_base.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/optimization/yaw_optimization/yaw_optimization_tools.py` & `floris-4.0.1/floris/optimization/yaw_optimization/yaw_optimization_tools.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/optimization/yaw_optimization/yaw_optimizer_geometric.py` & `floris-4.0.1/floris/optimization/yaw_optimization/yaw_optimizer_geometric.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/optimization/yaw_optimization/yaw_optimizer_scipy.py` & `floris-4.0.1/floris/optimization/yaw_optimization/yaw_optimizer_scipy.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/optimization/yaw_optimization/yaw_optimizer_sr.py` & `floris-4.0.1/floris/optimization/yaw_optimization/yaw_optimizer_sr.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/parallel_floris_model.py` & `floris-4.0.1/floris/parallel_floris_model.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/turbine_library/iea_10MW.yaml` & `floris-4.0.1/floris/turbine_library/iea_10MW.yaml`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/turbine_library/iea_15MW.yaml` & `floris-4.0.1/floris/turbine_library/iea_15MW.yaml`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/turbine_library/iea_15MW_floating_multi_dim_cp_ct.yaml` & `floris-4.0.1/floris/turbine_library/iea_15MW_floating_multi_dim_cp_ct.yaml`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/turbine_library/nrel_5MW.yaml` & `floris-4.0.1/floris/turbine_library/nrel_5MW.yaml`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/turbine_library/turbine_previewer.py` & `floris-4.0.1/floris/turbine_library/turbine_previewer.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/turbine_library/turbine_utilities.py` & `floris-4.0.1/floris/turbine_library/turbine_utilities.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/type_dec.py` & `floris-4.0.1/floris/type_dec.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/uncertain_floris_model.py` & `floris-4.0.1/floris/uncertain_floris_model.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/utilities.py` & `floris-4.0.1/floris/utilities.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/floris/wind_data.py` & `floris-4.0.1/floris/wind_data.py`

 * *Files identical despite different names*

### Comparing `FLORIS-4/pyproject.toml` & `floris-4.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `FLORIS-4/setup.py` & `floris-4.0.1/setup.py`

 * *Files identical despite different names*

