# Comparing `tmp/HOPP-2.1.0.tar.gz` & `tmp/HOPP-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HOPP-2.1.0.tar", last modified: Mon Nov 27 19:08:03 2023, max compression
+gzip compressed data, was "HOPP-2.2.0.tar", last modified: Wed Apr 24 15:51:19 2024, max compression
```

## Comparing `HOPP-2.1.0.tar` & `HOPP-2.2.0.tar`

### file list

```diff
@@ -1,255 +1,256 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:08:03.211581 HOPP-2.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:08:03.183581 HOPP-2.1.0/HOPP.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4209 2023-11-27 19:08:02.000000 HOPP-2.1.0/HOPP.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10378 2023-11-27 19:08:03.000000 HOPP-2.1.0/HOPP.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-27 19:08:02.000000 HOPP-2.1.0/HOPP.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      450 2023-11-27 19:08:02.000000 HOPP-2.1.0/HOPP.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-11-27 19:08:02.000000 HOPP-2.1.0/HOPP.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2023-11-27 19:07:53.000000 HOPP-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4209 2023-11-27 19:08:03.211581 HOPP-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2023-11-27 19:07:53.000000 HOPP-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:08:03.183581 HOPP-2.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 19:07:53.000000 HOPP-2.1.0/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:08:03.183581 HOPP-2.1.0/hopp/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5066 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/logging_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:08:03.183581 HOPP-2.1.0/hopp/simulation/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/hopp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/hopp_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    54249 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/hybrid_simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:08:03.183581 HOPP-2.1.0/hopp/simulation/technologies/
--rw-r--r--   0 runner    (1001) docker     (127)      801 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:08:03.183581 HOPP-2.1.0/hopp/simulation/technologies/battery/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/battery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19690 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/battery/battery.py
--rw-r--r--   0 runner    (1001) docker     (127)    10223 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/battery/battery_stateless.py
--rw-r--r--   0 runner    (1001) docker     (127)    50507 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/clustering.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:08:03.183581 HOPP-2.1.0/hopp/simulation/technologies/csp/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/csp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46616 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/csp/csp_plant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:08:03.187581 HOPP-2.1.0/hopp/simulation/technologies/csp/pySSC_daotk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/csp/pySSC_daotk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27205 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/csp/pySSC_daotk/ssc_wrap.py
--rw-r--r--   0 runner    (1001) docker     (127)    22542 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/csp/tower_plant.py
--rw-r--r--   0 runner    (1001) docker     (127)     8896 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/csp/trough_plant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:08:03.187581 HOPP-2.1.0/hopp/simulation/technologies/dispatch/
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/dispatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/dispatch/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/dispatch/dispatch_problem_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     9883 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/dispatch/grid_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)    20939 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/dispatch/hybrid_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)    28604 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/dispatch/hybrid_dispatch_builder_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     6133 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/dispatch/hybrid_dispatch_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:08:03.187581 HOPP-2.1.0/hopp/simulation/technologies/dispatch/power_sources/
--rw-r--r--   0 runner    (1001) docker     (127)      375 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/dispatch/power_sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    69331 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/dispatch/power_sources/csp_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4276 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/dispatch/power_sources/power_source_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/dispatch/power_sources/pv_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/dispatch/power_sources/tower_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/dispatch/power_sources/trough_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/dispatch/power_sources/wave_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/dispatch/power_sources/wind_dispatch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:08:03.187581 HOPP-2.1.0/hopp/simulation/technologies/dispatch/power_storage/
--rw-r--r--   0 runner    (1001) docker     (127)      763 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/dispatch/power_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11460 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/dispatch/power_storage/linear_voltage_convex_battery_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)    14878 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/dispatch/power_storage/linear_voltage_nonconvex_battery_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     7919 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/dispatch/power_storage/one_cycle_battery_dispatch_heuristic.py
--rw-r--r--   0 runner    (1001) docker     (127)    19138 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/dispatch/power_storage/power_storage_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/dispatch/power_storage/simple_battery_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6602 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/dispatch/power_storage/simple_battery_dispatch_heuristic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:08:03.191581 HOPP-2.1.0/hopp/simulation/technologies/financial/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/financial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13927 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/financial/custom_financial_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9838 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/financial/mhk_cost_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9791 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/grid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:08:03.191581 HOPP-2.1.0/hopp/simulation/technologies/hydrogen/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/hydrogen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:08:03.191581 HOPP-2.1.0/hopp/simulation/technologies/hydrogen/electrolysis/
--rw-r--r--   0 runner    (1001) docker     (127)    19860 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/hydrogen/electrolysis/PEM_H2_LT_electrolyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)    42850 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/hydrogen/electrolysis/PEM_H2_LT_electrolyzer_Clusters.py
--rw-r--r--   0 runner    (1001) docker     (127)    15565 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/hydrogen/electrolysis/PEM_costs_Singlitico_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    26612 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/hydrogen/electrolysis/PEM_electrolyzer_IVcurve.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/hydrogen/electrolysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5982 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/hydrogen/electrolysis/optimization_utils_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/hydrogen/electrolysis/pem_mass_and_footprint.py
--rw-r--r--   0 runner    (1001) docker     (127)    12190 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/hydrogen/electrolysis/run_PEM_master.py
--rw-r--r--   0 runner    (1001) docker     (127)     9726 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/hydrogen/electrolysis/run_h2_PEM.py
--rw-r--r--   0 runner    (1001) docker     (127)     8721 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/hydrogen/electrolysis/run_h2_clusters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:08:03.191581 HOPP-2.1.0/hopp/simulation/technologies/hydrogen/h2_storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/hydrogen/h2_storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:08:03.191581 HOPP-2.1.0/hopp/simulation/technologies/hydrogen/h2_storage/on_turbine/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/hydrogen/h2_storage/on_turbine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19950 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/hydrogen/h2_storage/on_turbine/on_turbine_hydrogen_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:08:03.191581 HOPP-2.1.0/hopp/simulation/technologies/hydrogen/h2_storage/pipe_storage/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/hydrogen/h2_storage/pipe_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8019 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/hydrogen/h2_storage/pipe_storage/underground_pipe_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:08:03.191581 HOPP-2.1.0/hopp/simulation/technologies/hydrogen/h2_storage/pressure_vessel/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/hydrogen/h2_storage/pressure_vessel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:08:03.191581 HOPP-2.1.0/hopp/simulation/technologies/hydrogen/h2_storage/pressure_vessel/compressed_gas_storage_model_20221021/
--rw-r--r--   0 runner    (1001) docker     (127)     8970 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/hydrogen/h2_storage/pressure_vessel/compressed_gas_storage_model_20221021/Compressed_all.py
--rw-r--r--   0 runner    (1001) docker     (127)    31441 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/hydrogen/h2_storage/pressure_vessel/compressed_gas_storage_model_20221021/Compressed_gas_function.py
--rw-r--r--   0 runner    (1001) docker     (127)      306 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/hydrogen/h2_storage/pressure_vessel/compressed_gas_storage_model_20221021/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28451 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/hydrogen/h2_storage/pressure_vessel/tankinator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2904 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/hydrogen/h2_storage/pressure_vessel/von_mises.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:08:03.195581 HOPP-2.1.0/hopp/simulation/technologies/layout/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2023-11-27 19:07:53.000000 HOPP-2.1.0/hopp/simulation/technologies/layout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28572 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/simulation/technologies/layout/flicker_mismatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     8050 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/simulation/technologies/layout/flicker_mismatch_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     6843 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/simulation/technologies/layout/hybrid_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/simulation/technologies/layout/layout_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     8896 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/simulation/technologies/layout/pv_design_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9584 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/simulation/technologies/layout/pv_inverter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10757 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/simulation/technologies/layout/pv_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)    14323 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/simulation/technologies/layout/pv_layout_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    14200 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/simulation/technologies/layout/pv_module.py
--rw-r--r--   0 runner    (1001) docker     (127)    19226 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/simulation/technologies/layout/shadow_flicker.py
--rw-r--r--   0 runner    (1001) docker     (127)     6523 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/simulation/technologies/layout/simple_flicker.py
--rw-r--r--   0 runner    (1001) docker     (127)     8942 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/simulation/technologies/layout/wind_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)    10562 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/simulation/technologies/layout/wind_layout_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    31351 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/simulation/technologies/power_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:08:03.195581 HOPP-2.1.0/hopp/simulation/technologies/pv/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/simulation/technologies/pv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18130 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/simulation/technologies/pv/detailed_pv_plant.py
--rw-r--r--   0 runner    (1001) docker     (127)     8478 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/simulation/technologies/pv/pv_plant.py
--rw-r--r--   0 runner    (1001) docker     (127)    15283 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/simulation/technologies/reopt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:08:03.195581 HOPP-2.1.0/hopp/simulation/technologies/resource/
--rw-r--r--   0 runner    (1001) docker     (127)      381 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/simulation/technologies/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/simulation/technologies/resource/elec_prices.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/simulation/technologies/resource/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     5446 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/simulation/technologies/resource/solar_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/simulation/technologies/resource/wave_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     6908 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/simulation/technologies/resource/wind_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     7253 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/simulation/technologies/run_power_losses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:08:03.199581 HOPP-2.1.0/hopp/simulation/technologies/sites/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/simulation/technologies/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/simulation/technologies/sites/circular_site.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/simulation/technologies/sites/flatirons_site.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/simulation/technologies/sites/irregular_site.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/simulation/technologies/sites/locations.py
--rw-r--r--   0 runner    (1001) docker     (127)    13436 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/simulation/technologies/sites/site_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/simulation/technologies/utility_rate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:08:03.199581 HOPP-2.1.0/hopp/simulation/technologies/wave/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/simulation/technologies/wave/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10008 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/simulation/technologies/wave/mhk_wave_plant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:08:03.199581 HOPP-2.1.0/hopp/simulation/technologies/wind/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/simulation/technologies/wind/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5285 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/simulation/technologies/wind/floris.py
--rw-r--r--   0 runner    (1001) docker     (127)    12390 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/simulation/technologies/wind/wind_plant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:08:03.199581 HOPP-2.1.0/hopp/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:08:03.199581 HOPP-2.1.0/hopp/tools/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:08:03.199581 HOPP-2.1.0/hopp/tools/analysis/bos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/analysis/bos/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2997 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/analysis/bos/atb_lookup.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3808 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/analysis/bos/bos_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/analysis/bos/bos_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/analysis/bos/calculate_installed_costs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9781 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/analysis/bos/cost_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4518 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/analysis/bos/hybrid_bosse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/analysis/bos/hybridbosse_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/analysis/determine_curtailment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:08:03.199581 HOPP-2.1.0/hopp/tools/dispatch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/dispatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21482 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/dispatch/csp_pv_battery_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    18964 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/dispatch/plot_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:08:03.199581 HOPP-2.1.0/hopp/tools/layout/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/layout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/layout/plot_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:08:03.203581 HOPP-2.1.0/hopp/tools/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/optimization/candidate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:08:03.203581 HOPP-2.1.0/hopp/tools/optimization/candidate_converter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/optimization/candidate_converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/optimization/candidate_converter/candidate_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/optimization/candidate_converter/dict_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8424 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/optimization/candidate_converter/object_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/optimization/candidate_converter/passthrough_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:08:03.203581 HOPP-2.1.0/hopp/tools/optimization/command_line_tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/optimization/command_line_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/optimization/command_line_tools/config_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     5208 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/optimization/command_line_tools/run_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:08:03.203581 HOPP-2.1.0/hopp/tools/optimization/data_logging/
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/optimization/data_logging/JSON_lines_record_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/optimization/data_logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/optimization/data_logging/a_data_recorder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/optimization/data_logging/data_recorder.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/optimization/data_logging/null_data_recorder.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/optimization/data_logging/null_record_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/optimization/data_logging/record_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/optimization/data_logging/table_data_recorder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:08:03.203581 HOPP-2.1.0/hopp/tools/optimization/driver/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/optimization/driver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/optimization/driver/ask_tell_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/optimization/driver/ask_tell_parallel_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/optimization/driver/ask_tell_parallel_driver_fns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/optimization/driver/ask_tell_serial_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)    11902 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/optimization/optimization_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3981 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/optimization/optimization_problem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:08:03.207581 HOPP-2.1.0/hopp/tools/optimization/optimizer/
--rw-r--r--   0 runner    (1001) docker     (127)     4227 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/optimization/optimizer/CEM_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    21521 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/optimization/optimizer/CMA_ES_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3794 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/optimization/optimizer/DCEM_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4974 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/optimization/optimizer/GA_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/optimization/optimizer/IDCEM.py
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/optimization/optimizer/IPDCEM.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/optimization/optimizer/IWDCEM.py
--rw-r--r--   0 runner    (1001) docker     (127)     6590 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/optimization/optimizer/KFDCEM.py
--rw-r--r--   0 runner    (1001) docker     (127)     6089 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/optimization/optimizer/SPSA_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/optimization/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/optimization/optimizer/ask_tell_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4207 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/optimization/optimizer/particle_gradient_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/optimization/optimizer/stationary_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2738 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/optimization/problem_parametrization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:08:03.207581 HOPP-2.1.0/hopp/tools/resource/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/resource/download_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:08:03.207581 HOPP-2.1.0/hopp/tools/resource/resource_loader/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/resource/resource_loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5154 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/resource/resource_loader/resource_loader_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/resource/resource_loader/site_details_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3208 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/resource/resource_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/tools/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7102 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/type_dec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:08:03.207581 HOPP-2.1.0/hopp/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/utilities/keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/utilities/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/utilities/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/utilities/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-11-27 19:07:54.000000 HOPP-2.1.0/hopp/version.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-27 19:08:03.211581 HOPP-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2023-11-27 19:07:54.000000 HOPP-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:08:03.207581 HOPP-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-11-27 19:07:54.000000 HOPP-2.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2023-11-27 19:07:54.000000 HOPP-2.1.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 19:08:03.211581 HOPP-2.1.0/tests/hopp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 19:07:54.000000 HOPP-2.1.0/tests/hopp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2023-11-27 19:07:54.000000 HOPP-2.1.0/tests/hopp/test_battery.py
--rw-r--r--   0 runner    (1001) docker     (127)     9751 2023-11-27 19:07:54.000000 HOPP-2.1.0/tests/hopp/test_battery_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2023-11-27 19:07:54.000000 HOPP-2.1.0/tests/hopp/test_battery_stateless.py
--rw-r--r--   0 runner    (1001) docker     (127)    20271 2023-11-27 19:07:54.000000 HOPP-2.1.0/tests/hopp/test_clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     6811 2023-11-27 19:07:54.000000 HOPP-2.1.0/tests/hopp/test_cost_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)    15807 2023-11-27 19:07:54.000000 HOPP-2.1.0/tests/hopp/test_csp.py
--rw-r--r--   0 runner    (1001) docker     (127)    14429 2023-11-27 19:07:54.000000 HOPP-2.1.0/tests/hopp/test_custom_financial.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2023-11-27 19:07:54.000000 HOPP-2.1.0/tests/hopp/test_detailed_pv_plant.py
--rw-r--r--   0 runner    (1001) docker     (127)    42710 2023-11-27 19:07:54.000000 HOPP-2.1.0/tests/hopp/test_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5840 2023-11-27 19:07:54.000000 HOPP-2.1.0/tests/hopp/test_flicker.py
--rw-r--r--   0 runner    (1001) docker     (127)     7630 2023-11-27 19:07:54.000000 HOPP-2.1.0/tests/hopp/test_flicker_mismatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2023-11-27 19:07:54.000000 HOPP-2.1.0/tests/hopp/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)    45942 2023-11-27 19:07:54.000000 HOPP-2.1.0/tests/hopp/test_hybrid.py
--rw-r--r--   0 runner    (1001) docker     (127)    25258 2023-11-27 19:07:54.000000 HOPP-2.1.0/tests/hopp/test_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2023-11-27 19:07:54.000000 HOPP-2.1.0/tests/hopp/test_pv_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2023-11-27 19:07:54.000000 HOPP-2.1.0/tests/hopp/test_reopt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2023-11-27 19:07:54.000000 HOPP-2.1.0/tests/hopp/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3895 2023-11-27 19:07:54.000000 HOPP-2.1.0/tests/hopp/test_resource_download.py
--rw-r--r--   0 runner    (1001) docker     (127)     4763 2023-11-27 19:07:54.000000 HOPP-2.1.0/tests/hopp/test_site_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5234 2023-11-27 19:07:54.000000 HOPP-2.1.0/tests/hopp/test_solar_wind.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2023-11-27 19:07:54.000000 HOPP-2.1.0/tests/hopp/test_tower_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2023-11-27 19:07:54.000000 HOPP-2.1.0/tests/hopp/test_trough_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2023-11-27 19:07:54.000000 HOPP-2.1.0/tests/hopp/test_utility_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8715 2023-11-27 19:07:54.000000 HOPP-2.1.0/tests/hopp/test_wave.py
--rw-r--r--   0 runner    (1001) docker     (127)     6677 2023-11-27 19:07:54.000000 HOPP-2.1.0/tests/hopp/test_wind.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2023-11-27 19:07:54.000000 HOPP-2.1.0/tests/hopp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:19.061724 HOPP-2.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:19.029724 HOPP-2.2.0/HOPP.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-04-24 15:51:18.000000 HOPP-2.2.0/HOPP.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10467 2024-04-24 15:51:18.000000 HOPP-2.2.0/HOPP.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 15:51:18.000000 HOPP-2.2.0/HOPP.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-24 15:51:18.000000 HOPP-2.2.0/HOPP.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-24 15:51:18.000000 HOPP-2.2.0/HOPP.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-24 15:51:09.000000 HOPP-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-04-24 15:51:19.061724 HOPP-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-24 15:51:09.000000 HOPP-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:19.029724 HOPP-2.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:09.000000 HOPP-2.2.0/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:19.029724 HOPP-2.2.0/hopp/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-24 15:51:09.000000 HOPP-2.2.0/hopp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-04-24 15:51:09.000000 HOPP-2.2.0/hopp/logging_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:19.029724 HOPP-2.2.0/hopp/simulation/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-24 15:51:09.000000 HOPP-2.2.0/hopp/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-24 15:51:09.000000 HOPP-2.2.0/hopp/simulation/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-24 15:51:09.000000 HOPP-2.2.0/hopp/simulation/hopp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-24 15:51:09.000000 HOPP-2.2.0/hopp/simulation/hopp_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54365 2024-04-24 15:51:09.000000 HOPP-2.2.0/hopp/simulation/hybrid_simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:19.029724 HOPP-2.2.0/hopp/simulation/technologies/
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-24 15:51:09.000000 HOPP-2.2.0/hopp/simulation/technologies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:19.033724 HOPP-2.2.0/hopp/simulation/technologies/battery/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-24 15:51:09.000000 HOPP-2.2.0/hopp/simulation/technologies/battery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19690 2024-04-24 15:51:09.000000 HOPP-2.2.0/hopp/simulation/technologies/battery/battery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10223 2024-04-24 15:51:09.000000 HOPP-2.2.0/hopp/simulation/technologies/battery/battery_stateless.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50507 2024-04-24 15:51:09.000000 HOPP-2.2.0/hopp/simulation/technologies/clustering.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:19.033724 HOPP-2.2.0/hopp/simulation/technologies/csp/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-24 15:51:09.000000 HOPP-2.2.0/hopp/simulation/technologies/csp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46616 2024-04-24 15:51:09.000000 HOPP-2.2.0/hopp/simulation/technologies/csp/csp_plant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:19.033724 HOPP-2.2.0/hopp/simulation/technologies/csp/pySSC_daotk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:09.000000 HOPP-2.2.0/hopp/simulation/technologies/csp/pySSC_daotk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27205 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/csp/pySSC_daotk/ssc_wrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22542 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/csp/tower_plant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8896 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/csp/trough_plant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:19.033724 HOPP-2.2.0/hopp/simulation/technologies/dispatch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/dispatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/dispatch/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/dispatch/dispatch_problem_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13295 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/dispatch/grid_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10606 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/dispatch/hybrid_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31154 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/dispatch/hybrid_dispatch_builder_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7098 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/dispatch/hybrid_dispatch_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:19.033724 HOPP-2.2.0/hopp/simulation/technologies/dispatch/power_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/dispatch/power_sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77620 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/dispatch/power_sources/csp_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/dispatch/power_sources/power_source_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/dispatch/power_sources/pv_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6352 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/dispatch/power_sources/tower_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5781 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/dispatch/power_sources/trough_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/dispatch/power_sources/wave_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/dispatch/power_sources/wind_dispatch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:19.037724 HOPP-2.2.0/hopp/simulation/technologies/dispatch/power_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/dispatch/power_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/dispatch/power_storage/heuristic_load_following_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13407 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/dispatch/power_storage/linear_voltage_convex_battery_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17501 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/dispatch/power_storage/linear_voltage_nonconvex_battery_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8413 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/dispatch/power_storage/one_cycle_battery_dispatch_heuristic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25403 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/dispatch/power_storage/power_storage_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/dispatch/power_storage/simple_battery_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8813 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/dispatch/power_storage/simple_battery_dispatch_heuristic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:19.037724 HOPP-2.2.0/hopp/simulation/technologies/financial/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/financial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13927 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/financial/custom_financial_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9838 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/financial/mhk_cost_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13716 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/grid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:19.037724 HOPP-2.2.0/hopp/simulation/technologies/hydrogen/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/hydrogen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:19.037724 HOPP-2.2.0/hopp/simulation/technologies/hydrogen/electrolysis/
+-rw-r--r--   0 runner    (1001) docker     (127)    19860 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/hydrogen/electrolysis/PEM_H2_LT_electrolyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42850 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/hydrogen/electrolysis/PEM_H2_LT_electrolyzer_Clusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15565 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/hydrogen/electrolysis/PEM_costs_Singlitico_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26612 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/hydrogen/electrolysis/PEM_electrolyzer_IVcurve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/hydrogen/electrolysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/hydrogen/electrolysis/optimization_utils_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/hydrogen/electrolysis/pem_mass_and_footprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12190 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/hydrogen/electrolysis/run_PEM_master.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9726 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/hydrogen/electrolysis/run_h2_PEM.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/hydrogen/electrolysis/run_h2_clusters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:19.037724 HOPP-2.2.0/hopp/simulation/technologies/hydrogen/h2_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/hydrogen/h2_storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:19.041724 HOPP-2.2.0/hopp/simulation/technologies/hydrogen/h2_storage/on_turbine/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/hydrogen/h2_storage/on_turbine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19950 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/hydrogen/h2_storage/on_turbine/on_turbine_hydrogen_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:19.041724 HOPP-2.2.0/hopp/simulation/technologies/hydrogen/h2_storage/pipe_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/hydrogen/h2_storage/pipe_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8019 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/hydrogen/h2_storage/pipe_storage/underground_pipe_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:19.041724 HOPP-2.2.0/hopp/simulation/technologies/hydrogen/h2_storage/pressure_vessel/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/hydrogen/h2_storage/pressure_vessel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:19.041724 HOPP-2.2.0/hopp/simulation/technologies/hydrogen/h2_storage/pressure_vessel/compressed_gas_storage_model_20221021/
+-rw-r--r--   0 runner    (1001) docker     (127)     8970 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/hydrogen/h2_storage/pressure_vessel/compressed_gas_storage_model_20221021/Compressed_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31441 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/hydrogen/h2_storage/pressure_vessel/compressed_gas_storage_model_20221021/Compressed_gas_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/hydrogen/h2_storage/pressure_vessel/compressed_gas_storage_model_20221021/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28451 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/hydrogen/h2_storage/pressure_vessel/tankinator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/hydrogen/h2_storage/pressure_vessel/von_mises.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:19.041724 HOPP-2.2.0/hopp/simulation/technologies/layout/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/layout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28572 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/layout/flicker_mismatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8050 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/layout/flicker_mismatch_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/layout/hybrid_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/layout/layout_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8896 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/layout/pv_design_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9584 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/layout/pv_inverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10757 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/layout/pv_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14323 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/layout/pv_layout_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14200 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/layout/pv_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19226 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/layout/shadow_flicker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/layout/simple_flicker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8942 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/layout/wind_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10562 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/layout/wind_layout_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31351 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/power_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:19.045724 HOPP-2.2.0/hopp/simulation/technologies/pv/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/pv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18130 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/pv/detailed_pv_plant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8478 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/pv/pv_plant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15283 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/reopt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:19.045724 HOPP-2.2.0/hopp/simulation/technologies/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/resource/elec_prices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/resource/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5496 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/resource/solar_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/resource/wave_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6958 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/resource/wind_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7253 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/run_power_losses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:19.045724 HOPP-2.2.0/hopp/simulation/technologies/sites/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/sites/circular_site.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/sites/flatirons_site.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/sites/irregular_site.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/sites/locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13436 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/sites/site_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/utility_rate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:19.045724 HOPP-2.2.0/hopp/simulation/technologies/wave/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/wave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10008 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/wave/mhk_wave_plant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:19.045724 HOPP-2.2.0/hopp/simulation/technologies/wind/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/wind/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/wind/floris.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12390 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/simulation/technologies/wind/wind_plant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:19.045724 HOPP-2.2.0/hopp/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:19.045724 HOPP-2.2.0/hopp/tools/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:19.049724 HOPP-2.2.0/hopp/tools/analysis/bos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/analysis/bos/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2997 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/analysis/bos/atb_lookup.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3808 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/analysis/bos/bos_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/analysis/bos/bos_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/analysis/bos/calculate_installed_costs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9781 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/analysis/bos/cost_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/analysis/bos/hybrid_bosse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/analysis/bos/hybridbosse_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/analysis/determine_curtailment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:19.049724 HOPP-2.2.0/hopp/tools/dispatch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/dispatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21482 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/dispatch/csp_pv_battery_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19352 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/dispatch/plot_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:19.049724 HOPP-2.2.0/hopp/tools/layout/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/layout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/layout/plot_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:19.049724 HOPP-2.2.0/hopp/tools/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/optimization/candidate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:19.049724 HOPP-2.2.0/hopp/tools/optimization/candidate_converter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/optimization/candidate_converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/optimization/candidate_converter/candidate_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/optimization/candidate_converter/dict_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/optimization/candidate_converter/object_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/optimization/candidate_converter/passthrough_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:19.049724 HOPP-2.2.0/hopp/tools/optimization/command_line_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/optimization/command_line_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/optimization/command_line_tools/config_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/optimization/command_line_tools/run_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:19.053724 HOPP-2.2.0/hopp/tools/optimization/data_logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/optimization/data_logging/JSON_lines_record_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/optimization/data_logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/optimization/data_logging/a_data_recorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/optimization/data_logging/data_recorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/optimization/data_logging/null_data_recorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/optimization/data_logging/null_record_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/optimization/data_logging/record_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/optimization/data_logging/table_data_recorder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:19.053724 HOPP-2.2.0/hopp/tools/optimization/driver/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/optimization/driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/optimization/driver/ask_tell_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/optimization/driver/ask_tell_parallel_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/optimization/driver/ask_tell_parallel_driver_fns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/optimization/driver/ask_tell_serial_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11902 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/optimization/optimization_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/optimization/optimization_problem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:19.053724 HOPP-2.2.0/hopp/tools/optimization/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)     4227 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/optimization/optimizer/CEM_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21521 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/optimization/optimizer/CMA_ES_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/optimization/optimizer/DCEM_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/optimization/optimizer/GA_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/optimization/optimizer/IDCEM.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/optimization/optimizer/IPDCEM.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/optimization/optimizer/IWDCEM.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6590 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/optimization/optimizer/KFDCEM.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6089 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/optimization/optimizer/SPSA_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/optimization/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/optimization/optimizer/ask_tell_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/optimization/optimizer/particle_gradient_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/optimization/optimizer/stationary_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/optimization/problem_parametrization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:19.053724 HOPP-2.2.0/hopp/tools/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/resource/download_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:19.057724 HOPP-2.2.0/hopp/tools/resource/resource_loader/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/resource/resource_loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/resource/resource_loader/resource_loader_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/resource/resource_loader/site_details_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/resource/resource_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/tools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/type_dec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:19.057724 HOPP-2.2.0/hopp/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/utilities/keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/utilities/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/utilities/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/utilities/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 15:51:10.000000 HOPP-2.2.0/hopp/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 15:51:19.061724 HOPP-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-24 15:51:10.000000 HOPP-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:19.057724 HOPP-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-24 15:51:10.000000 HOPP-2.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-24 15:51:10.000000 HOPP-2.2.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:19.061724 HOPP-2.2.0/tests/hopp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:51:10.000000 HOPP-2.2.0/tests/hopp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-24 15:51:10.000000 HOPP-2.2.0/tests/hopp/test_battery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9754 2024-04-24 15:51:10.000000 HOPP-2.2.0/tests/hopp/test_battery_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-24 15:51:10.000000 HOPP-2.2.0/tests/hopp/test_battery_stateless.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20271 2024-04-24 15:51:10.000000 HOPP-2.2.0/tests/hopp/test_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-04-24 15:51:10.000000 HOPP-2.2.0/tests/hopp/test_cost_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15807 2024-04-24 15:51:10.000000 HOPP-2.2.0/tests/hopp/test_csp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14575 2024-04-24 15:51:10.000000 HOPP-2.2.0/tests/hopp/test_custom_financial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-24 15:51:10.000000 HOPP-2.2.0/tests/hopp/test_detailed_pv_plant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43865 2024-04-24 15:51:10.000000 HOPP-2.2.0/tests/hopp/test_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-04-24 15:51:10.000000 HOPP-2.2.0/tests/hopp/test_flicker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7630 2024-04-24 15:51:10.000000 HOPP-2.2.0/tests/hopp/test_flicker_mismatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-04-24 15:51:10.000000 HOPP-2.2.0/tests/hopp/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47428 2024-04-24 15:51:10.000000 HOPP-2.2.0/tests/hopp/test_hybrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25258 2024-04-24 15:51:10.000000 HOPP-2.2.0/tests/hopp/test_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-24 15:51:10.000000 HOPP-2.2.0/tests/hopp/test_pv_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-24 15:51:10.000000 HOPP-2.2.0/tests/hopp/test_reopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-24 15:51:10.000000 HOPP-2.2.0/tests/hopp/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-04-24 15:51:10.000000 HOPP-2.2.0/tests/hopp/test_resource_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-04-24 15:51:10.000000 HOPP-2.2.0/tests/hopp/test_site_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-04-24 15:51:10.000000 HOPP-2.2.0/tests/hopp/test_solar_wind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-24 15:51:10.000000 HOPP-2.2.0/tests/hopp/test_tower_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-24 15:51:10.000000 HOPP-2.2.0/tests/hopp/test_trough_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-24 15:51:10.000000 HOPP-2.2.0/tests/hopp/test_utility_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-04-24 15:51:10.000000 HOPP-2.2.0/tests/hopp/test_wave.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-04-24 15:51:10.000000 HOPP-2.2.0/tests/hopp/test_wind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-24 15:51:10.000000 HOPP-2.2.0/tests/hopp/utils.py
```

### Comparing `HOPP-2.1.0/HOPP.egg-info/PKG-INFO` & `HOPP-2.2.0/HOPP.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HOPP
-Version: 2.1.0
+Version: 2.2.0
 Summary: Hybrid Systems Optimization and Performance Platform.
 Home-page: https://github.com/NREL/HOPP
 Author: NREL
 Author-email: dguittet@nrel.gov
 License: BSD 3-Clause
 Description: # Release Notes
```

### Comparing `HOPP-2.1.0/HOPP.egg-info/SOURCES.txt` & `HOPP-2.2.0/HOPP.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 hopp/simulation/technologies/dispatch/power_sources/power_source_dispatch.py
 hopp/simulation/technologies/dispatch/power_sources/pv_dispatch.py
 hopp/simulation/technologies/dispatch/power_sources/tower_dispatch.py
 hopp/simulation/technologies/dispatch/power_sources/trough_dispatch.py
 hopp/simulation/technologies/dispatch/power_sources/wave_dispatch.py
 hopp/simulation/technologies/dispatch/power_sources/wind_dispatch.py
 hopp/simulation/technologies/dispatch/power_storage/__init__.py
+hopp/simulation/technologies/dispatch/power_storage/heuristic_load_following_dispatch.py
 hopp/simulation/technologies/dispatch/power_storage/linear_voltage_convex_battery_dispatch.py
 hopp/simulation/technologies/dispatch/power_storage/linear_voltage_nonconvex_battery_dispatch.py
 hopp/simulation/technologies/dispatch/power_storage/one_cycle_battery_dispatch_heuristic.py
 hopp/simulation/technologies/dispatch/power_storage/power_storage_dispatch.py
 hopp/simulation/technologies/dispatch/power_storage/simple_battery_dispatch.py
 hopp/simulation/technologies/dispatch/power_storage/simple_battery_dispatch_heuristic.py
 hopp/simulation/technologies/financial/__init__.py
```

### Comparing `HOPP-2.1.0/LICENSE` & `HOPP-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/PKG-INFO` & `HOPP-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HOPP
-Version: 2.1.0
+Version: 2.2.0
 Summary: Hybrid Systems Optimization and Performance Platform.
 Home-page: https://github.com/NREL/HOPP
 Author: NREL
 Author-email: dguittet@nrel.gov
 License: BSD 3-Clause
 Description: # Release Notes
```

### Comparing `HOPP-2.1.0/README.md` & `HOPP-2.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -55,20 +55,20 @@
     ```
 
 6. The functions which download resource data require an NREL API key. Obtain a key from:
     
     [https://developer.nrel.gov/signup/](https://developer.nrel.gov/signup/)
     
 
-7. To set up the `NREL_API_KEY` required for resource downloads, you can create an Environment Variable called 
-   `NREL_API_KEY`. Otherwise, you can keep the key in a new file called ".env" in the root directory of this project. 
+7. To set up the `NREL_API_KEY` and `NREL_API_EMAIL` required for resource downloads, you can create Environment Variables called `NREL_API_KEY` and `NREL_API_EMAIL`. Otherwise, you can keep the key in a new file called ".env" in the root directory of this project. 
 
     Create a file ".env" that contains the single line:
-     ```
+    ```
     NREL_API_KEY=key
+    NREL_API_EMAIL=your.name@email.com
     ```
 
 8. Verify setup by running tests:
     ```
     pytest tests/hopp
     ```
```

### Comparing `HOPP-2.1.0/hopp/logging_manager.py` & `HOPP-2.2.0/hopp/logging_manager.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/base.py` & `HOPP-2.2.0/hopp/simulation/base.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/hopp.py` & `HOPP-2.2.0/hopp/simulation/hopp.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/hopp_interface.py` & `HOPP-2.2.0/hopp/simulation/hopp_interface.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/hybrid_simulation.py` & `HOPP-2.2.0/hopp/simulation/hybrid_simulation.py`

 * *Files 0% similar despite different names*

```diff
@@ -656,15 +656,22 @@
                     total_gen += project_life_gen
                     model.gen_max_feasible = model.calc_gen_max_feasible_kwh(self.interconnect_kw)
                     total_gen_max_feasible_year1 += model.gen_max_feasible
 
         # Consolidate grid generation by copying over power and storage generation information
         if self.battery:
             self.grid.generation_profile_wo_battery = total_gen_before_battery
-        self.grid.simulate_grid_connection(hybrid_size_kw, total_gen, project_life, lifetime_sim, total_gen_max_feasible_year1)
+        self.grid.simulate_grid_connection(
+            hybrid_size_kw, 
+            total_gen, 
+            project_life, 
+            lifetime_sim,
+            total_gen_max_feasible_year1,
+            self.dispatch_builder.options
+        )
         self.grid.hybrid_nominal_capacity = hybrid_nominal_capacity
         self.grid.total_gen_max_feasible_year1 = total_gen_max_feasible_year1
         logger.info(f"Hybrid Peformance Simulation Complete. AEPs are {self.annual_energies}.")
 
     def simulate_financials(self, project_life):
         """
         Runs the finanical models for individual sub-systems and the hybrid system as a whole
```

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/__init__.py` & `HOPP-2.2.0/hopp/simulation/technologies/__init__.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/battery/battery.py` & `HOPP-2.2.0/hopp/simulation/technologies/battery/battery.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/battery/battery_stateless.py` & `HOPP-2.2.0/hopp/simulation/technologies/battery/battery_stateless.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/clustering.py` & `HOPP-2.2.0/hopp/simulation/technologies/clustering.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/csp/csp_plant.py` & `HOPP-2.2.0/hopp/simulation/technologies/csp/csp_plant.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/csp/pySSC_daotk/ssc_wrap.py` & `HOPP-2.2.0/hopp/simulation/technologies/csp/pySSC_daotk/ssc_wrap.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/csp/tower_plant.py` & `HOPP-2.2.0/hopp/simulation/technologies/csp/tower_plant.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/csp/trough_plant.py` & `HOPP-2.2.0/hopp/simulation/technologies/csp/trough_plant.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/dispatch/__init__.py` & `HOPP-2.2.0/hopp/simulation/technologies/dispatch/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,26 @@
 from hopp.simulation.technologies.dispatch.power_sources.pv_dispatch import PvDispatch
-from hopp.simulation.technologies.dispatch.power_sources.wind_dispatch import WindDispatch
+from hopp.simulation.technologies.dispatch.power_sources.wind_dispatch import (
+    WindDispatch,
+)
 from hopp.simulation.technologies.dispatch.power_sources.csp_dispatch import CspDispatch
-from hopp.simulation.technologies.dispatch.power_sources.trough_dispatch import TroughDispatch
-from hopp.simulation.technologies.dispatch.power_sources.tower_dispatch import TowerDispatch
-from hopp.simulation.technologies.dispatch.power_sources.wave_dispatch import WaveDispatch
+from hopp.simulation.technologies.dispatch.power_sources.trough_dispatch import (
+    TroughDispatch,
+)
+from hopp.simulation.technologies.dispatch.power_sources.tower_dispatch import (
+    TowerDispatch,
+)
+from hopp.simulation.technologies.dispatch.power_sources.wave_dispatch import (
+    WaveDispatch,
+)
 
 from hopp.simulation.technologies.dispatch.grid_dispatch import GridDispatch
-from hopp.simulation.technologies.dispatch.hybrid_dispatch_options import HybridDispatchOptions
+from hopp.simulation.technologies.dispatch.hybrid_dispatch_options import (
+    HybridDispatchOptions,
+)
 from hopp.simulation.technologies.dispatch.hybrid_dispatch import HybridDispatch
-from hopp.simulation.technologies.dispatch.dispatch_problem_state import DispatchProblemState
-from hopp.simulation.technologies.dispatch.power_storage.simple_battery_dispatch import SimpleBatteryDispatch
+from hopp.simulation.technologies.dispatch.dispatch_problem_state import (
+    DispatchProblemState,
+)
+from hopp.simulation.technologies.dispatch.power_storage.simple_battery_dispatch import (
+    SimpleBatteryDispatch,
+)
```

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/dispatch/dispatch.py` & `HOPP-2.2.0/hopp/simulation/technologies/dispatch/dispatch.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,55 @@
 import pyomo.environ as pyomo
 from pyomo.environ import units as u
 
 try:
     u.USD
 except AttributeError:
-    u.load_definitions_from_strings(['USD = [currency]', 'lifecycle = [energy] / [energy]'])
+    u.load_definitions_from_strings(
+        ["USD = [currency]", "lifecycle = [energy] / [energy]"]
+    )
+
 
 class Dispatch:
-    """
+    """ """
 
-    """
-    def __init__(self,
-                 pyomo_model: pyomo.ConcreteModel,
-                 index_set: pyomo.Set,
-                 system_model,
-                 financial_model,
-                 block_set_name: str = 'dispatch'):
+    def __init__(
+        self,
+        pyomo_model: pyomo.ConcreteModel,
+        index_set: pyomo.Set,
+        system_model,
+        financial_model,
+        block_set_name: str = "dispatch",
+    ):
 
         self.block_set_name = block_set_name
         self.round_digits = int(4)
 
         self._model = pyomo_model
         self._blocks = pyomo.Block(index_set, rule=self.dispatch_block_rule)
         setattr(self.model, self.block_set_name, self.blocks)
 
         self._system_model = system_model
         self._financial_model = financial_model
 
     @staticmethod
     def dispatch_block_rule(block, t):
-        raise NotImplemented("This function must be overridden for specific dispatch model")
+        raise NotImplemented(
+            "This function must be overridden for specific dispatch model"
+        )
 
     def initialize_parameters(self):
-        raise NotImplemented("This function must be overridden for specific dispatch model")
+        raise NotImplemented(
+            "This function must be overridden for specific dispatch model"
+        )
 
     def update_time_series_parameters(self, start_time: int):
-        raise NotImplemented("This function must be overridden for specific dispatch model")
+        raise NotImplemented(
+            "This function must be overridden for specific dispatch model"
+        )
 
     @staticmethod
     def _check_efficiency_value(efficiency):
         """Checks efficiency is between 0 and 1 or 0 and 100. Returns fractional value"""
         if efficiency < 0:
             raise ValueError("Efficiency value must greater than 0")
         elif efficiency > 1:
```

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/dispatch/dispatch_problem_state.py` & `HOPP-2.2.0/hopp/simulation/technologies/dispatch/dispatch_problem_state.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,17 @@
         self._lower_bound = ()
         self._constraints = ()
         self._variables = ()
         self._non_zeros = ()
         self._gap = ()
         self._n_non_optimal_solves = 0
 
-    def store_problem_metrics(self, solver_results, start_time, n_days, objective_value):
+    def store_problem_metrics(
+        self, solver_results, start_time, n_days, objective_value
+    ):
         self.start_time = start_time
         self.n_days = n_days
         self.termination_condition = str(solver_results.solver.termination_condition)
         try:
             self.solve_time = solver_results.solver.time
         except AttributeError:
             self.solve_time = solver_results.solver.wallclock_time
@@ -31,113 +33,117 @@
         self.lower_bound = solver_results.problem.lower_bound
         self.constraints = solver_results.problem.number_of_constraints
         self.variables = solver_results.problem.number_of_variables
         self.non_zeros = solver_results.problem.number_of_nonzeros
 
         # solver_results.solution.Gap not define
         if solver_results.problem.upper_bound != 0.0:
-            self.gap = (abs(solver_results.problem.upper_bound - solver_results.problem.lower_bound)
-                        / abs(solver_results.problem.upper_bound))
+            self.gap = abs(
+                solver_results.problem.upper_bound - solver_results.problem.lower_bound
+            ) / abs(solver_results.problem.upper_bound)
         elif solver_results.problem.lower_bound == 0.0:
             self.gap = 0.0
         else:
-            self.gap = float('inf')
+            self.gap = float("inf")
 
-        if not solver_results.solver.termination_condition == TerminationCondition.optimal:
+        if (
+            not solver_results.solver.termination_condition
+            == TerminationCondition.optimal
+        ):
             self._n_non_optimal_solves += 1
 
     def _update_metric(self, metric_name, value):
         data = list(getattr(self, metric_name))
         data.append(value)
-        setattr(self, '_' + metric_name, tuple(data))
+        setattr(self, "_" + metric_name, tuple(data))
 
     @property
     def start_time(self) -> tuple:
         return self._start_time
 
     @start_time.setter
     def start_time(self, start_hour: int):
-        self._update_metric('start_time', start_hour)
+        self._update_metric("start_time", start_hour)
 
     @property
     def n_days(self) -> tuple:
         return self._n_days
 
     @n_days.setter
     def n_days(self, solve_days: int):
-        self._update_metric('n_days', solve_days)
+        self._update_metric("n_days", solve_days)
 
     @property
     def termination_condition(self) -> tuple:
         return self._termination_condition
 
     @termination_condition.setter
     def termination_condition(self, condition: str):
-        self._update_metric('termination_condition', condition)
+        self._update_metric("termination_condition", condition)
 
     @property
     def solve_time(self) -> tuple:
         return self._solve_time
 
     @solve_time.setter
     def solve_time(self, time: float):
-        self._update_metric('solve_time', time)
+        self._update_metric("solve_time", time)
 
     @property
     def objective(self) -> tuple:
         return self._objective
 
     @objective.setter
     def objective(self, objective_value: float):
-        self._update_metric('objective', objective_value)
+        self._update_metric("objective", objective_value)
 
     @property
     def upper_bound(self) -> tuple:
         return self._upper_bound
 
     @upper_bound.setter
     def upper_bound(self, bound: float):
-        self._update_metric('upper_bound', bound)
+        self._update_metric("upper_bound", bound)
 
     @property
     def lower_bound(self) -> tuple:
         return self._lower_bound
 
     @lower_bound.setter
     def lower_bound(self, bound: float):
-        self._update_metric('lower_bound', bound)
+        self._update_metric("lower_bound", bound)
 
     @property
     def constraints(self) -> tuple:
         return self._constraints
 
     @constraints.setter
     def constraints(self, constraint_count: int):
-        self._update_metric('constraints', constraint_count)
+        self._update_metric("constraints", constraint_count)
 
     @property
     def variables(self) -> tuple:
         return self._variables
 
     @variables.setter
     def variables(self, variable_count: int):
-        self._update_metric('variables', variable_count)
+        self._update_metric("variables", variable_count)
 
     @property
     def non_zeros(self) -> tuple:
         return self._non_zeros
 
     @non_zeros.setter
     def non_zeros(self, non_zeros_count: int):
-        self._update_metric('non_zeros', non_zeros_count)
+        self._update_metric("non_zeros", non_zeros_count)
 
     @property
     def gap(self) -> tuple:
         return self._gap
 
     @gap.setter
     def gap(self, mip_gap: int):
-        self._update_metric('gap', mip_gap)
+        self._update_metric("gap", mip_gap)
 
     @property
     def n_non_optimal_solves(self) -> int:
         return self._n_non_optimal_solves
```

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/dispatch/grid_dispatch.py` & `HOPP-2.2.0/hopp/simulation/technologies/dispatch/grid_dispatch.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,206 +1,332 @@
+from typing import Union
+
 import pyomo.environ as pyomo
 from pyomo.network import Port, Arc
 from pyomo.environ import units as u
 
 from hopp.simulation.technologies.dispatch.dispatch import Dispatch
 
 
 class GridDispatch(Dispatch):
+    grid_obj: Union[pyomo.Expression, float]
     _model: pyomo.ConcreteModel
     _blocks: pyomo.Block
     """
 
     """
 
-    def __init__(self,
-                 pyomo_model: pyomo.ConcreteModel,
-                 index_set: pyomo.Set,
-                 system_model,
-                 financial_model,
-                 block_set_name: str = 'grid'):
-
-        super().__init__(pyomo_model,
-                         index_set,
-                         system_model,
-                         financial_model,
-                         block_set_name=block_set_name)
+    def __init__(
+        self,
+        pyomo_model: pyomo.ConcreteModel,
+        index_set: pyomo.Set,
+        system_model,
+        financial_model,
+        block_set_name: str = "grid",
+    ):
+
+        super().__init__(
+            pyomo_model,
+            index_set,
+            system_model,
+            financial_model,
+            block_set_name=block_set_name,
+        )
 
     def dispatch_block_rule(self, grid):
         # Parameters
         self._create_grid_parameters(grid)
         # Variables
         self._create_grid_variables(grid)
         # Constraints
         self._create_grid_constraints(grid)
         # Ports
         self._create_grid_ports(grid)
 
+    def max_gross_profit_objective(self, hybrid_blocks):
+        self.obj = pyomo.Expression(
+            expr=sum(
+                hybrid_blocks[t].time_weighting_factor
+                * self.blocks[t].time_duration
+                * self.blocks[t].electricity_sell_price
+                * hybrid_blocks[t].electricity_sold
+                - (1 / hybrid_blocks[t].time_weighting_factor)
+                * self.blocks[t].time_duration
+                * self.blocks[t].electricity_purchase_price
+                * hybrid_blocks[t].electricity_purchased
+                - self.blocks[t].epsilon * self.blocks[t].is_generating
+                for t in hybrid_blocks.index_set()
+            )
+        )
+
+    def min_operating_cost_objective(self, hybrid_blocks):
+        self.obj = sum(
+            hybrid_blocks[t].time_weighting_factor
+            * self.blocks[t].time_duration
+            * self.blocks[t].electricity_sell_price
+            * (
+                self.blocks[t].generation_transmission_limit
+                - hybrid_blocks[t].electricity_sold
+            )
+            + (
+                hybrid_blocks[t].time_weighting_factor
+                * self.blocks[t].time_duration
+                * self.blocks[t].electricity_purchase_price
+                * hybrid_blocks[t].electricity_purchased
+            )
+            + (self.blocks[t].epsilon * self.blocks[t].is_generating)
+            for t in hybrid_blocks.index_set()
+        )
+
+    def _create_variables(self, hybrid):
+        hybrid.system_generation = pyomo.Var(
+            doc="System generation [MW]",
+            domain=pyomo.NonNegativeReals,
+            units=u.MW,
+        )
+        hybrid.system_load = pyomo.Var(
+            doc="System load [MW]",
+            domain=pyomo.NonNegativeReals,
+            units=u.MW,
+        )
+        hybrid.electricity_sold = pyomo.Var(
+            doc="Electricity sold [MW]",
+            domain=pyomo.NonNegativeReals,
+            units=u.MW,
+        )
+        hybrid.electricity_purchased = pyomo.Var(
+            doc="Electricity purchased [MW]",
+            domain=pyomo.NonNegativeReals,
+            units=u.MW,
+        )
+
+        return 0, 0
+
+    def _create_port(self, hybrid):
+        hybrid.grid_port = Port(
+            initialize={
+                "system_generation": hybrid.system_generation,
+                "system_load": hybrid.system_load,
+                "electricity_sold": hybrid.electricity_sold,
+                "electricity_purchased": hybrid.electricity_purchased,
+            }
+        )
+        return hybrid.grid_port
+
+    def _create_constraints(self, hybrid, t):
+        hybrid.generation_total = pyomo.Constraint(
+            doc="hybrid system generation total",
+            rule=hybrid.system_generation == sum(self.power_source_gen_vars[t]),
+        )
+
     @staticmethod
     def _create_grid_parameters(grid):
         ##################################
         # Parameters                     #
         ##################################
         grid.epsilon = pyomo.Param(
             doc="A small value used in objective for binary logic",
             default=1e-3,
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.USD)
+            units=u.USD,
+        )
         grid.time_duration = pyomo.Param(
             doc="Time step [hour]",
             default=1.0,
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.hr)
+            units=u.hr,
+        )
         grid.electricity_sell_price = pyomo.Param(
             doc="Electricity sell price [$/MWh]",
             default=0.0,
             within=pyomo.Reals,
             mutable=True,
-            units=u.USD / u.MWh)
+            units=u.USD / u.MWh,
+        )
         grid.electricity_purchase_price = pyomo.Param(
             doc="Electricity purchase price [$/MWh]",
             default=0.0,
             within=pyomo.Reals,
             mutable=True,
-            units=u.USD / u.MWh)
+            units=u.USD / u.MWh,
+        )
         grid.generation_transmission_limit = pyomo.Param(
             doc="Grid transmission limit for generation [MW]",
             default=1000.0,
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.MW)
+            units=u.MW,
+        )
         grid.load_transmission_limit = pyomo.Param(
             doc="Grid transmission limit for load [MW]",
             default=1000.0,
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.MW)
+            units=u.MW,
+        )
 
     @staticmethod
     def _create_grid_variables(grid):
         ##################################
         # Variables                      #
         ##################################
         grid.system_generation = pyomo.Var(
-            doc="System generation [MW]",
-            domain=pyomo.NonNegativeReals,
-            units=u.MW)
+            doc="System generation [MW]", domain=pyomo.NonNegativeReals, units=u.MW
+        )
         grid.system_load = pyomo.Var(
-            doc="System load [MW]",
-            domain=pyomo.NonNegativeReals,
-            units=u.MW)
+            doc="System load [MW]", domain=pyomo.NonNegativeReals, units=u.MW
+        )
         grid.electricity_sold = pyomo.Var(
             doc="Electricity sold to the grid [MW]",
             domain=pyomo.NonNegativeReals,
             bounds=(0, grid.generation_transmission_limit),
-            units=u.MW)
+            units=u.MW,
+        )
         grid.electricity_purchased = pyomo.Var(
             doc="Electricity purchased from the grid [MW]",
             domain=pyomo.NonNegativeReals,
             bounds=(0, grid.load_transmission_limit),
-            units=u.MW)
+            units=u.MW,
+        )
         grid.is_generating = pyomo.Var(
-            doc="System is generating power",
-            domain=pyomo.Binary,
-            units=u.dimensionless)
+            doc="System is generating power", domain=pyomo.Binary, units=u.dimensionless
+        )
 
     @staticmethod
     def _create_grid_constraints(grid):
         ##################################
         # Constraints                    #
         ##################################
         grid.balance = pyomo.Constraint(
             doc="Transmission energy balance",
-            expr=grid.electricity_sold - grid.electricity_purchased == grid.system_generation - grid.system_load
+            expr=(
+                grid.electricity_sold - grid.electricity_purchased
+                == grid.system_generation - grid.system_load
+            ),
         )
         grid.sales_transmission_limit = pyomo.Constraint(
             doc="Transmission limit on electricity sales",
-            expr=grid.electricity_sold <= grid.generation_transmission_limit * grid.is_generating
+            expr=grid.electricity_sold
+            <= grid.generation_transmission_limit * grid.is_generating,
         )
         grid.purchases_transmission_limit = pyomo.Constraint(
             doc="Transmission limit on electricity purchases",
-            expr=grid.electricity_purchased <= grid.load_transmission_limit * (1 - grid.is_generating)
+            expr=(
+                grid.electricity_purchased
+                <= grid.load_transmission_limit * (1 - grid.is_generating)
+            ),
         )
 
     @staticmethod
     def _create_grid_ports(grid):
         ##################################
         # Ports                          #
         ##################################
         grid.port = Port()
         grid.port.add(grid.system_generation)
         grid.port.add(grid.system_load)
         grid.port.add(grid.electricity_sold)
         grid.port.add(grid.electricity_purchased)
 
     def initialize_parameters(self):
-        grid_limit_kw = self._system_model.value('grid_interconnection_limit_kwac')
-        self.generation_transmission_limit = [grid_limit_kw / 1e3] * len(self.blocks.index_set())
-        self.load_transmission_limit = [grid_limit_kw / 1e3] * len(self.blocks.index_set())
+        grid_limit_kw = self._system_model.value("grid_interconnection_limit_kwac")
+        self.generation_transmission_limit = [grid_limit_kw / 1e3] * len(
+            self.blocks.index_set()
+        )
+        self.load_transmission_limit = [grid_limit_kw / 1e3] * len(
+            self.blocks.index_set()
+        )
 
     def update_time_series_parameters(self, start_time: int):
         n_horizon = len(self.blocks.index_set())
         dispatch_factors = self._financial_model.value("dispatch_factors_ts")
         ppa_price = self._financial_model.value("ppa_price_input")[0]
         if start_time + n_horizon > len(dispatch_factors):
             prices = list(dispatch_factors[start_time:])
-            prices.extend(list(dispatch_factors[0:n_horizon - len(prices)]))
+            prices.extend(list(dispatch_factors[0 : n_horizon - len(prices)]))
         else:
-            prices = dispatch_factors[start_time:start_time + n_horizon]
+            prices = dispatch_factors[start_time : start_time + n_horizon]
         # NOTE: Assuming the same prices
-        self.electricity_sell_price = [norm_price * ppa_price * 1e3 for norm_price in prices]
-        self.electricity_purchase_price = [norm_price * ppa_price * 1e3 for norm_price in prices]
+        self.electricity_sell_price = [
+            norm_price * ppa_price * 1e3 for norm_price in prices
+        ]
+        self.electricity_purchase_price = [
+            norm_price * ppa_price * 1e3 for norm_price in prices
+        ]
 
     @property
     def electricity_sell_price(self) -> list:
-        return [self.blocks[t].electricity_sell_price.value for t in self.blocks.index_set()]
+        return [
+            self.blocks[t].electricity_sell_price.value for t in self.blocks.index_set()
+        ]
 
     @electricity_sell_price.setter
     def electricity_sell_price(self, price_per_mwh: list):
         if len(price_per_mwh) == len(self.blocks):
             for t, price in zip(self.blocks, price_per_mwh):
-                self.blocks[t].electricity_sell_price.set_value(round(price, self.round_digits))
+                self.blocks[t].electricity_sell_price.set_value(
+                    round(price, self.round_digits)
+                )
         else:
-            raise ValueError("'price_per_mwh' list must be the same length as time horizon")
+            raise ValueError(
+                "'price_per_mwh' list must be the same length as time horizon"
+            )
 
     @property
     def electricity_purchase_price(self) -> list:
-        return [self.blocks[t].electricity_purchase_price.value for t in self.blocks.index_set()]
+        return [
+            self.blocks[t].electricity_purchase_price.value
+            for t in self.blocks.index_set()
+        ]
 
     @electricity_purchase_price.setter
     def electricity_purchase_price(self, price_per_mwh: list):
         if len(price_per_mwh) == len(self.blocks):
             for t, price in zip(self.blocks, price_per_mwh):
-                self.blocks[t].electricity_purchase_price.set_value(round(price, self.round_digits))
+                self.blocks[t].electricity_purchase_price.set_value(
+                    round(price, self.round_digits)
+                )
         else:
-            raise ValueError("'price_per_mwh' list must be the same length as time horizon")
+            raise ValueError(
+                "'price_per_mwh' list must be the same length as time horizon"
+            )
 
     @property
     def generation_transmission_limit(self) -> list:
-        return [self.blocks[t].generation_transmission_limit.value for t in self.blocks.index_set()]
+        return [
+            self.blocks[t].generation_transmission_limit.value
+            for t in self.blocks.index_set()
+        ]
 
     @generation_transmission_limit.setter
     def generation_transmission_limit(self, limit_mw: list):
         if len(limit_mw) == len(self.blocks):
             for t, limit in zip(self.blocks, limit_mw):
-                self.blocks[t].generation_transmission_limit.set_value(round(limit, self.round_digits))
+                self.blocks[t].generation_transmission_limit.set_value(
+                    round(limit, self.round_digits)
+                )
         else:
             raise ValueError("'limit_mw' list must be the same length as time horizon")
 
     @property
     def load_transmission_limit(self) -> list:
-        return [self.blocks[t].load_transmission_limit.value for t in self.blocks.index_set()]
+        return [
+            self.blocks[t].load_transmission_limit.value
+            for t in self.blocks.index_set()
+        ]
 
     @load_transmission_limit.setter
     def load_transmission_limit(self, limit_mw: list):
         if len(limit_mw) == len(self.blocks):
             for t, limit in zip(self.blocks, limit_mw):
-                self.blocks[t].load_transmission_limit.set_value(round(limit, self.round_digits))
+                self.blocks[t].load_transmission_limit.set_value(
+                    round(limit, self.round_digits)
+                )
         else:
             raise ValueError("'limit_mw' list must be the same length as time horizon")
 
     @property
     def system_generation(self) -> list:
         return [self.blocks[t].system_generation.value for t in self.blocks.index_set()]
 
@@ -226,15 +352,17 @@
 
     @property
     def electricity_sold(self) -> list:
         return [self.blocks[t].electricity_sold.value for t in self.blocks.index_set()]
 
     @property
     def electricity_purchased(self) -> list:
-        return [self.blocks[t].electricity_purchased.value for t in self.blocks.index_set()]
+        return [
+            self.blocks[t].electricity_purchased.value for t in self.blocks.index_set()
+        ]
 
     @property
     def is_generating(self) -> list:
         return [self.blocks[t].is_generating.value for t in self.blocks.index_set()]
 
     @property
     def not_generating(self) -> list:
```

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/dispatch/hybrid_dispatch_builder_solver.py` & `HOPP-2.2.0/hopp/simulation/technologies/dispatch/hybrid_dispatch_builder_solver.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,26 +3,30 @@
 import time
 
 import pyomo.environ as pyomo
 from pyomo.opt import TerminationCondition
 from pyomo.util.check_units import assert_units_consistent
 
 from hopp.simulation.technologies.sites.site_info import SiteInfo
-from hopp.simulation.technologies.dispatch import HybridDispatch, HybridDispatchOptions, DispatchProblemState
+from hopp.simulation.technologies.dispatch import (
+    HybridDispatch,
+    HybridDispatchOptions,
+    DispatchProblemState,
+)
 from hopp.simulation.technologies.clustering import Clustering
 from hopp.utilities.log import hybrid_logger as logger
 
 
 class HybridDispatchBuilderSolver:
     """Helper class for building hybrid system dispatch problem, solving dispatch problem, and simulating system
     with dispatch solution."""
-    def __init__(self,
-                 site: SiteInfo,
-                 power_sources: dict,
-                 dispatch_options: dict = None):
+
+    def __init__(
+        self, site: SiteInfo, power_sources: dict, dispatch_options: dict = None
+    ):
         """
 
         Parameters
         ----------
         dispatch_options :
             Contains attribute key, value pairs to change default dispatch options.
             For details see HybridDispatchOptions in hybrid_dispatch_options.py
@@ -33,309 +37,402 @@
         self.power_sources = power_sources
         self.options = HybridDispatchOptions(dispatch_options)
 
         # deletes previous log file under same name
         if os.path.isfile(self.options.log_name):
             os.remove(self.options.log_name)
 
-        self.needs_dispatch = any(item in ['battery', 'tower', 'trough'] for item in self.power_sources.keys())
+        self.needs_dispatch = any(
+            item in ["battery", "tower", "trough"] for item in self.power_sources.keys()
+        )
 
         if self.needs_dispatch:
             self._pyomo_model = self._create_dispatch_optimization_model()
             if self.site.follow_desired_schedule:
                 self.dispatch.create_min_operating_cost_objective()
             else:
                 self.dispatch.create_max_gross_profit_objective()
             self.dispatch.create_arcs()
             assert_units_consistent(self.pyomo_model)
             self.problem_state = DispatchProblemState()
-        
+
         # Clustering (optional)
         self.clustering = None
         if self.options.use_clustering:
-            #TODO: Add resource data for wind
-            self.clustering = Clustering(power_sources.keys(), self.site.solar_resource.filename, wind_resource_data = None, price_data = self.site.elec_prices.data)
+            # TODO: Add resource data for wind
+            self.clustering = Clustering(
+                power_sources.keys(),
+                self.site.solar_resource.filename,
+                wind_resource_data=None,
+                price_data=self.site.elec_prices.data,
+            )
             self.clustering.n_cluster = self.options.n_clusters
             if len(self.options.clustering_weights.keys()) == 0:
                 self.clustering.use_default_weights = True
-            elif self.options.clustering_divisions.keys() != self.options.clustering_weights.keys():
-                print ('Warning: Keys in user-specified dictionaries for clustering weights and divisions do not match. Reverting to default weights/divisions')
+            elif (
+                self.options.clustering_divisions.keys()
+                != self.options.clustering_weights.keys()
+            ):
+                print(
+                    "Warning: Keys in user-specified dictionaries for clustering weights and divisions do not match. Reverting to default weights/divisions"
+                )
                 self.clustering.use_default_weights = True
             else:
                 self.clustering.weights = self.options.clustering_weights
                 self.clustering.divisions = self.options.clustering_divisions
                 self.clustering.use_default_weights = False
             self.clustering.run_clustering()  # Create clusters and find exemplar days for simulation
 
     def _create_dispatch_optimization_model(self):
         """
         Creates monolith dispatch model
         """
-        model = pyomo.ConcreteModel(name='hybrid_dispatch')
+        model = pyomo.ConcreteModel(name="hybrid_dispatch")
         #################################
         # Sets                          #
         #################################
-        model.forecast_horizon = pyomo.Set(doc="Set of time periods in time horizon",
-                                           initialize=range(self.options.n_look_ahead_periods))
+        model.forecast_horizon = pyomo.Set(
+            doc="Set of time periods in time horizon",
+            initialize=range(self.options.n_look_ahead_periods),
+        )
         #################################
         # Blocks (technologies)         #
         #################################
         module = getattr(__import__("hopp").simulation.technologies, "dispatch")
         for source, tech in self.power_sources.items():
-            if source == 'battery':
+            if source == "battery":
                 tech._dispatch = self.options.battery_dispatch_class(
                     model,
                     model.forecast_horizon,
                     tech._system_model,
                     tech._financial_model,
                     block_set_name=source,
-                    dispatch_options=self.options)
+                    dispatch_options=self.options,
+                )
             else:
                 try:
-                    dispatch_class_name = getattr(module, source.capitalize() + "Dispatch")
+                    dispatch_class_name = getattr(
+                        module, source.capitalize() + "Dispatch"
+                    )
                 except AttributeError:
-                    raise ValueError("Could not find {} in dispatch module. Is {} supported in the hybrid "
-                                     "dispatch model?".format(source.capitalize() + "Dispatch", source))
+                    raise ValueError(
+                        "Could not find {} in dispatch module. Is {} supported in the hybrid "
+                        "dispatch model?".format(
+                            source.capitalize() + "Dispatch", source
+                        )
+                    )
                 tech._dispatch = dispatch_class_name(
                     model,
                     model.forecast_horizon,
                     tech._system_model,
-                    tech._financial_model)
+                    tech._financial_model,
+                )
 
         self._dispatch = HybridDispatch(
-            model,
-            model.forecast_horizon,
-            self.power_sources,
-            self.options)
+            model, model.forecast_horizon, self.power_sources, self.options
+        )
         return model
 
     def solve_dispatch_model(self, start_time: int, n_days: int):
         # Solve dispatch model
-        if self.options.solver == 'glpk':
+        if self.options.solver == "glpk":
             solver_results = self.glpk_solve()
-        elif self.options.solver == 'cbc':
+        elif self.options.solver == "cbc":
             solver_results = self.cbc_solve()
-        elif self.options.solver == 'xpress':
+        elif self.options.solver == "xpress":
             solver_results = self.xpress_solve()
-        elif self.options.solver == 'xpress_persistent':
+        elif self.options.solver == "xpress_persistent":
             solver_results = self.xpress_persistent_solve()
-        elif self.options.solver == 'gurobi_ampl':
+        elif self.options.solver == "gurobi_ampl":
             solver_results = self.gurobi_ampl_solve()
-        elif self.options.solver == 'gurobi':
+        elif self.options.solver == "gurobi":
             solver_results = self.gurobi_solve()
         else:
             raise ValueError("{} is not a supported solver".format(self.options.solver))
 
-        self.problem_state.store_problem_metrics(solver_results, start_time, n_days,
-                                                 self.dispatch.objective_value)
+        self.problem_state.store_problem_metrics(
+            solver_results, start_time, n_days, self.dispatch.objective_value
+        )
 
     @staticmethod
-    def glpk_solve_call(pyomo_model: pyomo.ConcreteModel,
-                        log_name: str = "",
-                        user_solver_options: dict = None):
+    def glpk_solve_call(
+        pyomo_model: pyomo.ConcreteModel,
+        log_name: str = "",
+        user_solver_options: dict = None,
+    ):
 
         # log_name = "annual_solve_GLPK.log"  # For debugging MILP solver
         # Ref. on solver options: https://en.wikibooks.org/wiki/GLPK/Using_GLPSOL
-        glpk_solver_options = {'cuts': None,
-                               'presol': None,
-                               # 'mostf': None,
-                               # 'mipgap': 0.001,
-                               'tmlim': 30
-                               }
-        solver_options = SolverOptions(glpk_solver_options, log_name, user_solver_options,'log')
-        with pyomo.SolverFactory('glpk') as solver:
+        glpk_solver_options = {
+            "cuts": None,
+            "presol": None,
+            # 'mostf': None,
+            # 'mipgap': 0.001,
+            "tmlim": 30,
+        }
+        solver_options = SolverOptions(
+            glpk_solver_options, log_name, user_solver_options, "log"
+        )
+        with pyomo.SolverFactory("glpk") as solver:
             results = solver.solve(pyomo_model, options=solver_options.constructed)
-        HybridDispatchBuilderSolver.log_and_solution_check(log_name, solver_options.instance_log, results.solver.termination_condition, pyomo_model)
+        HybridDispatchBuilderSolver.log_and_solution_check(
+            log_name,
+            solver_options.instance_log,
+            results.solver.termination_condition,
+            pyomo_model,
+        )
         return results
-        
+
     def glpk_solve(self):
-        return HybridDispatchBuilderSolver.glpk_solve_call(self.pyomo_model,
-                                                           self.options.log_name,
-                                                           self.options.solver_options)
-        
-    @staticmethod
-    def gurobi_ampl_solve_call(pyomo_model: pyomo.ConcreteModel,
-                               log_name: str = "",
-                               user_solver_options: dict = None):
+        return HybridDispatchBuilderSolver.glpk_solve_call(
+            self.pyomo_model, self.options.log_name, self.options.solver_options
+        )
 
-        # Ref. on solver options: https://www.gurobi.com/documentation/9.1/ampl-gurobi/parameters.html
-        gurobi_solver_options = {'timelim': 60,
-                                 'threads': 1}
-        solver_options = SolverOptions(gurobi_solver_options, log_name, user_solver_options,'logfile')
+    @staticmethod
+    def gurobi_ampl_solve_call(
+        pyomo_model: pyomo.ConcreteModel,
+        log_name: str = "",
+        user_solver_options: dict = None,
+    ):
 
-        with pyomo.SolverFactory('gurobi', executable='/opt/solvers/gurobi', solver_io='nl') as solver:
+        # Ref. on solver options: https://www.gurobi.com/documentation/9.1/ampl-gurobi/parameters.html
+        gurobi_solver_options = {"timelim": 60, "threads": 1}
+        solver_options = SolverOptions(
+            gurobi_solver_options, log_name, user_solver_options, "logfile"
+        )
+
+        with pyomo.SolverFactory(
+            "gurobi", executable="/opt/solvers/gurobi", solver_io="nl"
+        ) as solver:
             results = solver.solve(pyomo_model, options=solver_options.constructed)
-        HybridDispatchBuilderSolver.log_and_solution_check(log_name, solver_options.instance_log, results.solver.termination_condition, pyomo_model)
+        HybridDispatchBuilderSolver.log_and_solution_check(
+            log_name,
+            solver_options.instance_log,
+            results.solver.termination_condition,
+            pyomo_model,
+        )
         return results
 
     def gurobi_ampl_solve(self):
-        return HybridDispatchBuilderSolver.gurobi_ampl_solve_call(self.pyomo_model,
-                                                                  self.options.log_name,
-                                                                  self.options.solver_options)
-                                                                  
-    @staticmethod
-    def gurobi_solve_call(opt: pyomo.SolverFactory,
-                          pyomo_model: pyomo.ConcreteModel,
-                          log_name: str = "",
-                          user_solver_options: dict = None):
+        return HybridDispatchBuilderSolver.gurobi_ampl_solve_call(
+            self.pyomo_model, self.options.log_name, self.options.solver_options
+        )
+
+    @staticmethod
+    def gurobi_solve_call(
+        opt: pyomo.SolverFactory,
+        pyomo_model: pyomo.ConcreteModel,
+        log_name: str = "",
+        user_solver_options: dict = None,
+    ):
 
         # Ref. on solver options: https://www.gurobi.com/documentation/9.1/ampl-gurobi/parameters.html
-        gurobi_solver_options = {'timelim': 60,
-                                 'threads': 1}
-        solver_options = SolverOptions(gurobi_solver_options, log_name, user_solver_options,'logfile')
-        
+        gurobi_solver_options = {"timelim": 60, "threads": 1}
+        solver_options = SolverOptions(
+            gurobi_solver_options, log_name, user_solver_options, "logfile"
+        )
+
         opt.options.update(solver_options.constructed)
         opt.set_instance(pyomo_model)
         results = opt.solve(save_results=False)
-        HybridDispatchBuilderSolver.log_and_solution_check(log_name, solver_options.instance_log, results.solver.termination_condition, pyomo_model)
+        HybridDispatchBuilderSolver.log_and_solution_check(
+            log_name,
+            solver_options.instance_log,
+            results.solver.termination_condition,
+            pyomo_model,
+        )
         return results
 
     def gurobi_solve(self):
         if self.opt is None:
-            self.opt = pyomo.SolverFactory('gurobi', solver_io='persistent') 
-    
-        return HybridDispatchBuilderSolver.gurobi_solve_call(self.opt,
-                                                             self.pyomo_model,
-                                                             self.options.log_name,
-                                                             self.options.solver_options)
+            self.opt = pyomo.SolverFactory("gurobi", solver_io="persistent")
+
+        return HybridDispatchBuilderSolver.gurobi_solve_call(
+            self.opt,
+            self.pyomo_model,
+            self.options.log_name,
+            self.options.solver_options,
+        )
 
     @staticmethod
-    def cbc_solve_call(pyomo_model: pyomo.ConcreteModel,
-                       log_name: str = "",
-                       user_solver_options: dict = None):
+    def cbc_solve_call(
+        pyomo_model: pyomo.ConcreteModel,
+        log_name: str = "",
+        user_solver_options: dict = None,
+    ):
         # log_name = "annual_solve_CBC.log"
         # Solver options can be found by launching executable 'start cbc.exe', verbose 15, ?
         # https://coin-or.github.io/Cbc/faq.html (a bit outdated)
-        cbc_solver_options = {  # 'ratioGap': 0.001,
-                              'seconds': 60}
-        solver_options = SolverOptions(cbc_solver_options, log_name, user_solver_options,'log')
+        cbc_solver_options = {"seconds": 60}  # 'ratioGap': 0.001,
+        solver_options = SolverOptions(
+            cbc_solver_options, log_name, user_solver_options, "log"
+        )
 
-        if sys.platform == 'win32' or sys.platform == 'cygwin':
+        if sys.platform == "win32" or sys.platform == "cygwin":
             cbc_path = Path(__file__).parent / "cbc_solver" / "cbc-win64" / "cbc"
             if log_name != "":
-                logger.warning("Warning: CBC solver logging is active... This will significantly increase simulation time.")
-                solver_options.constructed['log'] = 2
-                solver = pyomo.SolverFactory('asl:cbc', executable=cbc_path)
-                results = solver.solve(pyomo_model, logfile=solver_options.instance_log, options=solver_options.constructed)
+                logger.warning(
+                    "Warning: CBC solver logging is active... This will significantly increase simulation time."
+                )
+                solver_options.constructed["log"] = 2
+                solver = pyomo.SolverFactory("asl:cbc", executable=cbc_path)
+                results = solver.solve(
+                    pyomo_model,
+                    logfile=solver_options.instance_log,
+                    options=solver_options.constructed,
+                )
             else:
-                solver = pyomo.SolverFactory('cbc', executable=cbc_path, solver_io='nl')
+                solver = pyomo.SolverFactory("cbc", executable=cbc_path, solver_io="nl")
                 results = solver.solve(pyomo_model, options=solver_options.constructed)
-        elif sys.platform == 'darwin' or sys.platform == 'linux':
-            solver = pyomo.SolverFactory('cbc')
+        elif sys.platform == "darwin" or sys.platform == "linux":
+            solver = pyomo.SolverFactory("cbc")
             results = solver.solve(pyomo_model, options=solver_options.constructed)
         else:
-            raise SystemError('Platform not supported ', sys.platform)
-        
-        HybridDispatchBuilderSolver.log_and_solution_check(log_name, solver_options.instance_log, results.solver.termination_condition, pyomo_model)
+            raise SystemError("Platform not supported ", sys.platform)
+
+        HybridDispatchBuilderSolver.log_and_solution_check(
+            log_name,
+            solver_options.instance_log,
+            results.solver.termination_condition,
+            pyomo_model,
+        )
         return results
 
     def cbc_solve(self):
-        return HybridDispatchBuilderSolver.cbc_solve_call(self.pyomo_model,
-                                                          self.options.log_name,
-                                                          self.options.solver_options)
+        return HybridDispatchBuilderSolver.cbc_solve_call(
+            self.pyomo_model, self.options.log_name, self.options.solver_options
+        )
 
     @staticmethod
-    def xpress_solve_call(pyomo_model: pyomo.ConcreteModel,
-                          log_name: str = "",
-                          user_solver_options: dict = None):
+    def xpress_solve_call(
+        pyomo_model: pyomo.ConcreteModel,
+        log_name: str = "",
+        user_solver_options: dict = None,
+    ):
 
         # FIXME: Logging does not work
         # log_name = "annual_solve_Xpress.log"  # For debugging MILP solver
         # Ref. on solver options: https://ampl.com/products/solvers/solvers-we-sell/xpress/options/
-        xpress_solver_options = {'mipgap': 0.001,
-                                 'maxtime': 30}
-        solver_options = SolverOptions(xpress_solver_options, log_name, user_solver_options,'LOGFILE')
+        xpress_solver_options = {"mipgap": 0.001, "maxtime": 30}
+        solver_options = SolverOptions(
+            xpress_solver_options, log_name, user_solver_options, "LOGFILE"
+        )
 
-        with pyomo.SolverFactory('xpress_direct') as solver:
+        with pyomo.SolverFactory("xpress_direct") as solver:
             results = solver.solve(pyomo_model, options=solver_options.constructed)
-        HybridDispatchBuilderSolver.log_and_solution_check(log_name, solver_options.instance_log, results.solver.termination_condition, pyomo_model)
+        HybridDispatchBuilderSolver.log_and_solution_check(
+            log_name,
+            solver_options.instance_log,
+            results.solver.termination_condition,
+            pyomo_model,
+        )
         return results
 
     def xpress_solve(self):
-        return HybridDispatchBuilderSolver.xpress_solve_call(self.pyomo_model,
-                                                             self.options.log_name,
-                                                             self.options.solver_options)
+        return HybridDispatchBuilderSolver.xpress_solve_call(
+            self.pyomo_model, self.options.log_name, self.options.solver_options
+        )
 
     @staticmethod
-    def xpress_persistent_solve_call(opt: pyomo.SolverFactory,
-                                     pyomo_model: pyomo.ConcreteModel,
-                                     log_name: str = "",
-                                     user_solver_options: dict = None):
+    def xpress_persistent_solve_call(
+        opt: pyomo.SolverFactory,
+        pyomo_model: pyomo.ConcreteModel,
+        log_name: str = "",
+        user_solver_options: dict = None,
+    ):
 
         # log_name = "annual_solve_Xpress.log"  # For debugging MILP solver
         # Ref. on solver options: https://ampl.com/products/solvers/solvers-we-sell/xpress/options/
-        xpress_solver_options = {'mipgap': 0.001,
-                                 'MAXTIME': 30}
-        solver_options = SolverOptions(xpress_solver_options, log_name, user_solver_options,'LOGFILE')
+        xpress_solver_options = {"mipgap": 0.001, "MAXTIME": 30}
+        solver_options = SolverOptions(
+            xpress_solver_options, log_name, user_solver_options, "LOGFILE"
+        )
 
         opt.options.update(solver_options.constructed)
         opt.set_instance(pyomo_model)
         results = opt.solve(save_results=False)
-        HybridDispatchBuilderSolver.log_and_solution_check(log_name, solver_options.instance_log, results.solver.termination_condition, pyomo_model)
+        HybridDispatchBuilderSolver.log_and_solution_check(
+            log_name,
+            solver_options.instance_log,
+            results.solver.termination_condition,
+            pyomo_model,
+        )
         return results
 
     def xpress_persistent_solve(self):
         if self.opt is None:
-            self.opt = pyomo.SolverFactory('xpress', solver_io='persistent')
+            self.opt = pyomo.SolverFactory("xpress", solver_io="persistent")
+
+        return HybridDispatchBuilderSolver.xpress_persistent_solve_call(
+            self.opt,
+            self.pyomo_model,
+            self.options.log_name,
+            self.options.solver_options,
+        )
 
-        return HybridDispatchBuilderSolver.xpress_persistent_solve_call(self.opt,
-                                                                        self.pyomo_model,
-                                                                        self.options.log_name,
-                                                                        self.options.solver_options)
     @staticmethod
-    def mindtpy_solve_call(pyomo_model: pyomo.ConcreteModel,
-                           log_name: str = ""):
+    def mindtpy_solve_call(pyomo_model: pyomo.ConcreteModel, log_name: str = ""):
         raise NotImplementedError
-        solver = pyomo.SolverFactory('mindtpy')
-        results = solver.solve(pyomo_model,
-                               mip_solver='glpk',
-                               nlp_solver='ipopt',
-                               tee=True)
-
-        HybridDispatchBuilderSolver.log_and_solution_check("", "", results.solver.termination_condition, pyomo_model)
+        solver = pyomo.SolverFactory("mindtpy")
+        results = solver.solve(
+            pyomo_model, mip_solver="glpk", nlp_solver="ipopt", tee=True
+        )
+
+        HybridDispatchBuilderSolver.log_and_solution_check(
+            "", "", results.solver.termination_condition, pyomo_model
+        )
         return results
 
     @staticmethod
-    def log_and_solution_check(log_name:str, solve_log: str, solver_termination_condition, pyomo_model):
+    def log_and_solution_check(
+        log_name: str, solve_log: str, solver_termination_condition, pyomo_model
+    ):
         if log_name != "":
             HybridDispatchBuilderSolver.append_solve_to_log(log_name, solve_log)
-        HybridDispatchBuilderSolver.check_solve_condition(solver_termination_condition, pyomo_model)
+        HybridDispatchBuilderSolver.check_solve_condition(
+            solver_termination_condition, pyomo_model
+        )
 
     @staticmethod
     def check_solve_condition(solver_termination_condition, pyomo_model):
         if solver_termination_condition == TerminationCondition.infeasible:
             HybridDispatchBuilderSolver.print_infeasible_problem(pyomo_model)
         elif not solver_termination_condition == TerminationCondition.optimal:
-            logger.warning("Warning: Dispatch problem termination condition was '"
-                  + str(solver_termination_condition) + "'")
+            logger.warning(
+                "Warning: Dispatch problem termination condition was '"
+                + str(solver_termination_condition)
+                + "'"
+            )
 
     @staticmethod
     def append_solve_to_log(log_name: str, solve_log: str):
         # Appends single problem instance log to annual log file
-        fin = open(solve_log, 'r')
+        fin = open(solve_log, "r")
         data = fin.read()
         fin.close()
 
-        ann_log = open(log_name, 'a+')
+        ann_log = open(log_name, "a+")
         ann_log.write("=" * 50 + "\n")
         ann_log.write(data)
         ann_log.close()
 
     @staticmethod
     def print_infeasible_problem(model: pyomo.ConcreteModel):
         original_stdout = sys.stdout
-        with open('infeasible_instance.txt', 'w') as f:
+        with open("infeasible_instance.txt", "w") as f:
             sys.stdout = f
-            print('\n' + '#' * 20 + ' Model Parameter Values ' + '#' * 20 + '\n')
+            print("\n" + "#" * 20 + " Model Parameter Values " + "#" * 20 + "\n")
             HybridDispatchBuilderSolver.print_all_parameters(model)
-            print('\n' + '#' * 20 + ' Model Blocks Display ' + '#' * 20 + '\n')
+            print("\n" + "#" * 20 + " Model Blocks Display " + "#" * 20 + "\n")
             HybridDispatchBuilderSolver.display_all_blocks(model)
             sys.stdout = original_stdout
-        raise ValueError("Dispatch optimization model is infeasible.\n"
-                         "See 'infeasible_instance.txt' for parameter values.")
+        raise ValueError(
+            "Dispatch optimization model is infeasible.\n"
+            "See 'infeasible_instance.txt' for parameter values."
+        )
 
     @staticmethod
     def print_all_parameters(model: pyomo.ConcreteModel):
         param_list = list()
         block_list = list()
         for param_object in model.component_objects(pyomo.Param, active=True):
             name_to_print = param_object.getname()
@@ -343,15 +440,17 @@
             block_name = parent_block.getname()
             if (name_to_print not in param_list) or (block_name not in block_list):
                 block_list.append(block_name)
                 param_list.append(name_to_print)
                 print("\nParent Block Name: ", block_name)
                 print("Parameter: ", name_to_print)
                 for index in parent_block.index_set():
-                    val_to_print = pyomo.value(getattr(parent_block[index], param_object.getname()))
+                    val_to_print = pyomo.value(
+                        getattr(parent_block[index], param_object.getname())
+                    )
                     print("\t", index, "\t", val_to_print)
 
     @staticmethod
     def display_all_blocks(model: pyomo.ConcreteModel):
         for block_object in model.component_objects(pyomo.Block, active=True):
             for index in block_object.index_set():
                 block_object[index].display()
@@ -366,168 +465,279 @@
         ti = list(range(0, self.site.n_timesteps, self.options.n_roll_periods))
         self.dispatch.initialize_parameters()
 
         if self.clustering is None:
             # Solving the year in series
             for i, t in enumerate(ti):
                 if self.options.is_test_start_year or self.options.is_test_end_year:
-                    if (self.options.is_test_start_year and i < 5) or (self.options.is_test_end_year and i > 359):
+                    if (self.options.is_test_start_year and i < 5) or (
+                        self.options.is_test_end_year and i > 359
+                    ):
                         start_time = time.time()
                         self.simulate_with_dispatch(t)
                         sim_w_dispath_time = time.time()
-                        logger.info('Day {} dispatch optimized.'.format(i))
-                        logger.info("      %6.2f seconds required to simulate with dispatch" % (sim_w_dispath_time - start_time))
+                        logger.info("Day {} dispatch optimized.".format(i))
+                        logger.info(
+                            "      %6.2f seconds required to simulate with dispatch"
+                            % (sim_w_dispath_time - start_time)
+                        )
                     else:
                         continue
                         # TODO: can we make the csp and battery model run with heuristic dispatch here?
                         #  Maybe calling a simulate_with_heuristic() method
                 else:
                     if (i % 73) == 0:
-                        logger.info("\t {:.0f} % complete".format(i*20/73))
+                        logger.info("\t {:.0f} % complete".format(i * 20 / 73))
                     self.simulate_with_dispatch(t)
         else:
 
-            initial_states = {tech:{'day':[], 'soc':[], 'load':[]} for tech in ['trough', 'tower', 'battery'] if tech in self.power_sources.keys()}  # List of known charge states at 12 am from completed simulations
-            npercluster = self.clustering.clusters['count']
-            inds = sorted(range(len(npercluster)), key=npercluster.__getitem__)  # Indicies to sort clusters by low-to-high number of days represented
-            for i in range(self.clustering.clusters['n_cluster']):
+            initial_states = {
+                tech: {"day": [], "soc": [], "load": []}
+                for tech in ["trough", "tower", "battery"]
+                if tech in self.power_sources.keys()
+            }  # List of known charge states at 12 am from completed simulations
+            npercluster = self.clustering.clusters["count"]
+            inds = sorted(
+                range(len(npercluster)), key=npercluster.__getitem__
+            )  # Indicies to sort clusters by low-to-high number of days represented
+            for i in range(self.clustering.clusters["n_cluster"]):
                 j = inds[i]  # cluster index
                 time_start, time_stop = self.clustering.get_sim_start_end_times(j)
-                battery_soc = self.clustering.battery_soc_heuristic(j, initial_states['battery']) if 'battery' in self.power_sources.keys() else None
+                battery_soc = (
+                    self.clustering.battery_soc_heuristic(j, initial_states["battery"])
+                    if "battery" in self.power_sources.keys()
+                    else None
+                )
 
                 # Set CSP initial states (need to do this prior to update_time_series_parameters() or update_initial_conditions(), both pull from the stored plant state)
-                for tech in ['trough', 'tower']:
+                for tech in ["trough", "tower"]:
                     if tech in self.power_sources.keys():
-                        self.power_sources[tech].plant_state = self.power_sources[tech].set_initial_plant_state()  # Reset to default initial state
-                        csp_soc, is_cycle_on, initial_cycle_load = self.clustering.csp_initial_state_heuristic(j, self.power_sources[tech].solar_multiple, initial_states[tech])
-                        self.power_sources[tech].set_tes_soc(csp_soc)  
-                        self.power_sources[tech].set_cycle_state(is_cycle_on)  
+                        self.power_sources[tech].plant_state = self.power_sources[
+                            tech
+                        ].set_initial_plant_state()  # Reset to default initial state
+                        csp_soc, is_cycle_on, initial_cycle_load = (
+                            self.clustering.csp_initial_state_heuristic(
+                                j,
+                                self.power_sources[tech].solar_multiple,
+                                initial_states[tech],
+                            )
+                        )
+                        self.power_sources[tech].set_tes_soc(csp_soc)
+                        self.power_sources[tech].set_cycle_state(is_cycle_on)
                         self.power_sources[tech].set_cycle_load(initial_cycle_load)
 
-                self.simulate_with_dispatch(time_start, self.clustering.ndays+1, battery_soc, n_initial_sims = 1)  
+                self.simulate_with_dispatch(
+                    time_start, self.clustering.ndays + 1, battery_soc, n_initial_sims=1
+                )
 
                 # Update lists of known states at 12am
-                for tech in ['trough', 'tower', 'battery']: 
+                for tech in ["trough", "tower", "battery"]:
                     if tech in self.power_sources.keys():
                         for d in range(self.clustering.ndays):
-                            day  = self.clustering.sim_start_days[j]+d
-                            initial_states[tech]['day'].append(day)
-                            if tech in ['trough', 'tower']:
-                                initial_states[tech]['soc'].append(self.power_sources[tech].get_tes_soc(day*24))
-                                initial_states[tech]['load'].append(self.power_sources[tech].get_cycle_load(day*24))
-                            elif tech in ['battery']:
-                                step = day*24 * int(self.site.n_timesteps/8760)
-                                initial_states[tech]['soc'].append(self.power_sources[tech].Outputs.SOC[step])
+                            day = self.clustering.sim_start_days[j] + d
+                            initial_states[tech]["day"].append(day)
+                            if tech in ["trough", "tower"]:
+                                initial_states[tech]["soc"].append(
+                                    self.power_sources[tech].get_tes_soc(day * 24)
+                                )
+                                initial_states[tech]["load"].append(
+                                    self.power_sources[tech].get_cycle_load(day * 24)
+                                )
+                            elif tech in ["battery"]:
+                                step = day * 24 * int(self.site.n_timesteps / 8760)
+                                initial_states[tech]["soc"].append(
+                                    self.power_sources[tech].Outputs.SOC[step]
+                                )
 
             # After exemplar simulations, update to full annual generation array for dispatchable technologies
             for tech in self.power_sources.keys():
-                if tech in ['battery']:
-                    for key in ['gen', 'P', 'SOC']:
+                if tech in ["battery"]:
+                    for key in ["gen", "P", "SOC"]:
                         val = getattr(self.power_sources[tech].Outputs, key)
-                        setattr(self.power_sources[tech].Outputs, key, list(self.clustering.compute_annual_array_from_cluster_exemplar_data(val)))
-                elif tech in ['trough', 'tower']:
-                    for key in ['gen', 'P_out_net', 'P_cycle', 'q_dot_pc_startup', 'q_pc_startup', 'e_ch_tes', 'eta', 'q_pb']:  # Data quantities used in capacity value calculations
-                        self.power_sources[tech].outputs.ssc_time_series[key] = list(self.clustering.compute_annual_array_from_cluster_exemplar_data(self.power_sources[tech].outputs.ssc_time_series[key])) 
-
-    def simulate_with_dispatch(self,
-                               start_time: int,
-                               n_days: int = 1,
-                               initial_soc: float = None,
-                               n_initial_sims: int = 0):
+                        setattr(
+                            self.power_sources[tech].Outputs,
+                            key,
+                            list(
+                                self.clustering.compute_annual_array_from_cluster_exemplar_data(
+                                    val
+                                )
+                            ),
+                        )
+                elif tech in ["trough", "tower"]:
+                    for key in [
+                        "gen",
+                        "P_out_net",
+                        "P_cycle",
+                        "q_dot_pc_startup",
+                        "q_pc_startup",
+                        "e_ch_tes",
+                        "eta",
+                        "q_pb",
+                    ]:  # Data quantities used in capacity value calculations
+                        self.power_sources[tech].outputs.ssc_time_series[key] = list(
+                            self.clustering.compute_annual_array_from_cluster_exemplar_data(
+                                self.power_sources[tech].outputs.ssc_time_series[key]
+                            )
+                        )
+
+    def simulate_with_dispatch(
+        self,
+        start_time: int,
+        n_days: int = 1,
+        initial_soc: float = None,
+        n_initial_sims: int = 0,
+    ):
         # this is needed for clustering effort
-        update_dispatch_times = list(range(start_time,
-                                           start_time + n_days * self.site.n_periods_per_day,
-                                           self.options.n_roll_periods))
+        update_dispatch_times = list(
+            range(
+                start_time,
+                start_time + n_days * self.site.n_periods_per_day,
+                self.options.n_roll_periods,
+            )
+        )
 
         for i, sim_start_time in enumerate(update_dispatch_times):
             # Update battery initial state of charge
-            if 'battery' in self.power_sources.keys():
-                self.power_sources['battery'].dispatch.update_dispatch_initial_soc(initial_soc=initial_soc)
+            if "battery" in self.power_sources.keys():
+                self.power_sources["battery"].dispatch.update_dispatch_initial_soc(
+                    initial_soc=initial_soc
+                )
                 initial_soc = None
 
             for model in self.power_sources.values():
                 if model.system_capacity_kw == 0:
                     continue
                 model.dispatch.update_time_series_parameters(sim_start_time)
 
             if self.site.follow_desired_schedule:
-                n_horizon = len(self.power_sources['grid'].dispatch.blocks.index_set())
+                n_horizon = len(self.power_sources["grid"].dispatch.blocks.index_set())
                 if start_time + n_horizon > len(self.site.desired_schedule):
                     system_limit = list(self.site.desired_schedule[start_time:])
-                    system_limit.extend(list(self.site.desired_schedule[0:n_horizon - len(system_limit)]))
+                    system_limit.extend(
+                        list(
+                            self.site.desired_schedule[
+                                0 : n_horizon - len(system_limit)
+                            ]
+                        )
+                    )
                 else:
-                    system_limit = self.site.desired_schedule[start_time:start_time + n_horizon]
-
-                transmission_limit = self.power_sources['grid'].value('grid_interconnection_limit_kwac') / 1e3
+                    system_limit = self.site.desired_schedule[
+                        start_time : start_time + n_horizon
+                    ]
+
+                transmission_limit = (
+                    self.power_sources["grid"].value("grid_interconnection_limit_kwac")
+                    / 1e3
+                )
                 for count, value in enumerate(system_limit):
                     if value > transmission_limit:
-                        logger.warning('Warning: Desired schedule is greater than transmission limit. '
-                              'Overwriting schedule to transmission limit')
+                        logger.warning(
+                            "Warning: Desired schedule is greater than transmission limit. "
+                            "Overwriting schedule to transmission limit"
+                        )
                         system_limit[count] = transmission_limit
 
-                self.power_sources['grid'].dispatch.generation_transmission_limit = system_limit
+                self.power_sources["grid"].dispatch.generation_transmission_limit = (
+                    system_limit
+                )
 
-            if 'heuristic' in self.options.battery_dispatch:
+            if "heuristic" in self.options.battery_dispatch:
                 # TODO: this is not a good way to do this... This won't work with CSP addition...
                 self.battery_heuristic()
                 # TODO: we could just run the csp model without dispatch here
             else:
                 self.solve_dispatch_model(start_time, n_days)
 
             store_outputs = True
             battery_sim_start_time = sim_start_time
             if i < n_initial_sims:
                 store_outputs = False
                 battery_sim_start_time = None
 
             # simulate using dispatch solution
-            if 'battery' in self.power_sources.keys():
-                self.power_sources['battery'].simulate_with_dispatch(self.options.n_roll_periods,
-                                                                     sim_start_time=battery_sim_start_time)
-
-            if 'trough' in self.power_sources.keys():
-                self.power_sources['trough'].simulate_with_dispatch(self.options.n_roll_periods,
-                                                                    sim_start_time=sim_start_time,
-                                                                    store_outputs=store_outputs)
-            if 'tower' in self.power_sources.keys():
-                self.power_sources['tower'].simulate_with_dispatch(self.options.n_roll_periods,
-                                                                   sim_start_time=sim_start_time,
-                                                                   store_outputs=store_outputs)
+            if "battery" in self.power_sources.keys():
+                self.power_sources["battery"].simulate_with_dispatch(
+                    self.options.n_roll_periods, sim_start_time=battery_sim_start_time
+                )
+
+            if "trough" in self.power_sources.keys():
+                self.power_sources["trough"].simulate_with_dispatch(
+                    self.options.n_roll_periods,
+                    sim_start_time=sim_start_time,
+                    store_outputs=store_outputs,
+                )
+            if "tower" in self.power_sources.keys():
+                self.power_sources["tower"].simulate_with_dispatch(
+                    self.options.n_roll_periods,
+                    sim_start_time=sim_start_time,
+                    store_outputs=store_outputs,
+                )
 
     def battery_heuristic(self):
-        tot_gen = [0.0]*self.options.n_look_ahead_periods
-        if 'pv' in self.power_sources.keys():
-            pv_gen = self.power_sources['pv'].dispatch.available_generation
+        tot_gen = [0.0] * self.options.n_look_ahead_periods
+        if "pv" in self.power_sources.keys():
+            pv_gen = self.power_sources["pv"].dispatch.available_generation
             tot_gen = [pv + gen for pv, gen in zip(pv_gen, tot_gen)]
-        if 'wind' in self.power_sources.keys():
-            wind_gen = self.power_sources['wind'].dispatch.available_generation
+        if "wind" in self.power_sources.keys():
+            wind_gen = self.power_sources["wind"].dispatch.available_generation
             tot_gen = [wind + gen for wind, gen in zip(wind_gen, tot_gen)]
 
-        grid_limit = self.power_sources['grid'].dispatch.generation_transmission_limit
+        grid_limit = self.power_sources["grid"].dispatch.generation_transmission_limit
 
-        if 'one_cycle' in self.options.battery_dispatch:
+        if "one_cycle" in self.options.battery_dispatch:
             # Get prices for one cycle heuristic
-            prices = self.power_sources['grid'].dispatch.electricity_sell_price
-            self.power_sources['battery'].dispatch.prices = prices
+            prices = self.power_sources["grid"].dispatch.electricity_sell_price
+            self.power_sources["battery"].dispatch.prices = prices
 
-        self.power_sources['battery'].dispatch.set_fixed_dispatch(tot_gen, grid_limit)
+        if "load_following" in self.options.battery_dispatch:
+            # TODO: Look into how to define a system as load following or not in the config file
+            required_keys = ["desired_load"]
+            if self.site.follow_desired_schedule:
+                # Get difference between baseload demand and power generation and control scenario variables
+                load_value = self.site.desired_schedule
+                load_difference = [
+                    (load_value[x] - tot_gen[x]) for x in range(len(tot_gen))
+                ]
+                self.power_sources["battery"].dispatch.load_difference = load_difference
+            else:
+                raise ValueError(
+                    type(self).__name__ + " requires the following : desired_schedule"
+                )
+            # Adding goal_power for the simple battery heuristic method for power setpoint tracking
+            goal_power = [load_value] * self.options.n_look_ahead_periods
+            ### Note: the inputs grid_limit and goal_power are in MW ###
+            self.power_sources["battery"].dispatch.set_fixed_dispatch(
+                tot_gen, grid_limit, load_value
+            )
+        else:
+            self.power_sources["battery"].dispatch.set_fixed_dispatch(
+                tot_gen, grid_limit
+            )
 
     @property
     def pyomo_model(self) -> pyomo.ConcreteModel:
         return self._pyomo_model
 
     @property
     def dispatch(self) -> HybridDispatch:
         return self._dispatch
 
+
 class SolverOptions:
     """Class for housing solver options"""
-    def __init__(self, solver_spec_options: dict, log_name: str="", user_solver_options: dict = None, solver_spec_log_key: str="logfile"):
+
+    def __init__(
+        self,
+        solver_spec_options: dict,
+        log_name: str = "",
+        user_solver_options: dict = None,
+        solver_spec_log_key: str = "logfile",
+    ):
         self.instance_log = "dispatch_solver.log"
         self.solver_spec_options = solver_spec_options
         self.user_solver_options = user_solver_options
-        
+
         self.constructed = solver_spec_options
         if log_name != "":
             self.constructed[solver_spec_log_key] = self.instance_log
         if user_solver_options is not None:
-            self.constructed.update(user_solver_options)
+            self.constructed.update(user_solver_options)
```

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/dispatch/hybrid_dispatch_options.py` & `HOPP-2.2.0/hopp/simulation/technologies/dispatch/hybrid_dispatch_options.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import numpy as np
 
 from hopp.simulation.technologies.dispatch.power_storage import (
     OneCycleBatteryDispatchHeuristic,
     SimpleBatteryDispatchHeuristic,
     SimpleBatteryDispatch,
     NonConvexLinearVoltageBatteryDispatch,
-    ConvexLinearVoltageBatteryDispatch
+    ConvexLinearVoltageBatteryDispatch,
+    HeuristicLoadFollowingDispatch,
 )
 
 
 class HybridDispatchOptions:
     """
     Class for setting dispatch options through HybridSimulation class.
 
     Args:
-        dispatch_options (dict): Contains attribute key-value pairs to change default options. 
+        dispatch_options (dict): Contains attribute key-value pairs to change default options.
 
             - **solver** (str, default='cbc'): MILP solver used for dispatch optimization problem. Options are `('glpk', 'cbc', 'xpress', 'xpress_persistent', 'gurobi_ampl', 'gurobi')`.
 
             - **solver_options** (dict): Dispatch solver options.
 
             - **battery_dispatch** (str, default='simple'): Sets the battery dispatch model to use for dispatch. Options are `('simple', 'one_cycle_heuristic', 'heuristic', 'non_convex_LV', 'convex_LV')`.
 
@@ -48,70 +49,102 @@
 
             - **n_clusters** (int, default=30).
 
             - **clustering_weights** (dict, default={}): Custom weights used for classification metrics for data clustering. If empty, default weights will be used.
 
             - **clustering_divisions** (dict, default={}): Custom number of averaging periods for classification metrics for data clustering. If empty, default values will be used.
 
+            - **use_higher_hours** bool (default = False): if True, the simulation will run extra hours analysis (must be used with load following)
+
+            - **higher_hours** (dict, default = {}): Higher hour count parameters: the value of power that must be available above the schedule and the number of hours in a row
+
     """
+
     def __init__(self, dispatch_options: dict = None):
-        self.solver: str = 'cbc'
-        self.solver_options: dict = {}   # used to update solver options, look at specific solver for option names
-        self.battery_dispatch: str = 'simple'
+        self.solver: str = "cbc"
+        self.solver_options: dict = (
+            {}
+        )  # used to update solver options, look at specific solver for option names
+        self.battery_dispatch: str = "simple"
         self.include_lifecycle_count: bool = True
-        self.lifecycle_cost_per_kWh_cycle: float = 0.0265  # Estimated using SAM output (lithium-ion battery)
+        self.lifecycle_cost_per_kWh_cycle: float = (
+            0.0265  # Estimated using SAM output (lithium-ion battery)
+        )
         self.max_lifecycle_per_day: int = np.inf
         self.grid_charging: bool = True
         self.pv_charging_only: bool = False
         self.n_look_ahead_periods: int = 48
         self.time_weighting_factor: float = 0.995
         self.n_roll_periods: int = 24
-        self.log_name: str = ''  # NOTE: Logging is not thread safe
+        self.log_name: str = ""  # NOTE: Logging is not thread safe
         self.is_test_start_year: bool = False
         self.is_test_end_year: bool = False
 
         self.use_clustering: bool = False
         self.n_clusters: int = 30
         self.clustering_weights: dict = {}
         self.clustering_divisions: dict = {}
 
+        self.use_higher_hours: bool = False
+        self.higher_hours: dict = {}
+
         if dispatch_options is not None:
             for key, value in dispatch_options.items():
                 if hasattr(self, key):
                     if type(getattr(self, key)) == type(value):
                         setattr(self, key, value)
                     else:
                         try:
                             value = type(getattr(self, key))(value)
                             setattr(self, key, value)
                         except:
-                            raise ValueError("'{}' is the wrong data type. Should be {}".format(key, type(getattr(self, key))))
+                            raise ValueError(
+                                "'{}' is the wrong data type. Should be {}".format(
+                                    key, type(getattr(self, key))
+                                )
+                            )
                 else:
-                    raise NameError("'{}' is not an attribute in {}".format(key, type(self).__name__))
+                    raise NameError(
+                        "'{}' is not an attribute in {}".format(
+                            key, type(self).__name__
+                        )
+                    )
 
         if self.is_test_start_year and self.is_test_end_year:
-            print('WARNING: Dispatch optimization START and END of year testing is enabled!')
+            print(
+                "WARNING: Dispatch optimization START and END of year testing is enabled!"
+            )
         elif self.is_test_start_year:
-            print('WARNING: Dispatch optimization START of year testing is enabled!')
+            print("WARNING: Dispatch optimization START of year testing is enabled!")
         elif self.is_test_end_year:
-            print('WARNING: Dispatch optimization END of year testing is enabled!')
+            print("WARNING: Dispatch optimization END of year testing is enabled!")
 
         if self.pv_charging_only and self.grid_charging:
-            raise ValueError("Battery cannot be restricted to charge from PV only if grid_charging is enabled")
+            raise ValueError(
+                "Battery cannot be restricted to charge from PV only if grid_charging is enabled"
+            )
 
         self._battery_dispatch_model_options = {
-            'one_cycle_heuristic': OneCycleBatteryDispatchHeuristic,
-            'heuristic': SimpleBatteryDispatchHeuristic,
-            'simple': SimpleBatteryDispatch,
-            'non_convex_LV': NonConvexLinearVoltageBatteryDispatch,
-            'convex_LV': ConvexLinearVoltageBatteryDispatch}
+            "one_cycle_heuristic": OneCycleBatteryDispatchHeuristic,
+            "heuristic": SimpleBatteryDispatchHeuristic,
+            "simple": SimpleBatteryDispatch,
+            "non_convex_LV": NonConvexLinearVoltageBatteryDispatch,
+            "convex_LV": ConvexLinearVoltageBatteryDispatch,
+            "load_following_heuristic": HeuristicLoadFollowingDispatch,
+        }
         if self.battery_dispatch in self._battery_dispatch_model_options:
-            self.battery_dispatch_class = self._battery_dispatch_model_options[self.battery_dispatch]
-            if 'heuristic' in self.battery_dispatch:
+            self.battery_dispatch_class = self._battery_dispatch_model_options[
+                self.battery_dispatch
+            ]
+            if "heuristic" in self.battery_dispatch:
                 # FIXME: This should be set to the number of time steps within a day.
                 #  Dispatch time duration is not set as of now...
                 self.n_roll_periods = 24
                 self.n_look_ahead_periods = self.n_roll_periods
                 # dispatch cycle counting is not available in heuristics
                 self.include_lifecycle_count = False
         else:
-            raise ValueError("'{}' is not currently a battery dispatch class.".format(self.battery_dispatch))
+            raise ValueError(
+                "'{}' is not currently a battery dispatch class.".format(
+                    self.battery_dispatch
+                )
+            )
```

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/dispatch/power_sources/csp_dispatch.py` & `HOPP-2.2.0/hopp/simulation/technologies/dispatch/power_sources/csp_dispatch.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,37 +5,57 @@
 import datetime
 import numpy as np
 
 from hopp.simulation.technologies.dispatch.dispatch import Dispatch
 
 
 class CspDispatch(Dispatch):
-    """
-    Dispatch model for Concentrating Solar Power (CSP) with thermal energy storage.
-    """
-
-    def __init__(self,
-                 pyomo_model: pyomo.ConcreteModel,
-                 index_set: pyomo.Set,
-                 system_model,
-                 financial_model,
-                 block_set_name: str = 'csp'):
+    """Dispatch model for Concentrating Solar Power (CSP) with thermal energy storage."""
 
-        super().__init__(pyomo_model, index_set, system_model, financial_model, block_set_name=block_set_name)
+    def __init__(
+        self,
+        pyomo_model: pyomo.ConcreteModel,
+        index_set: pyomo.Set,
+        system_model,
+        financial_model,
+        block_set_name: str = "csp",
+    ):
+        """Initialize a CSP dispatch model.
+
+        Args:
+            pyomo_model (pyomo.ConcreteModel): Pyomo model instance.
+            index_set (pyomo.Set): Index set for the model.
+            system_model: System model.
+            financial_model: Financial model.
+            block_set_name (str, optional): Name of the block. Defaults to 'csp'.
+
+        """
+        super().__init__(
+            pyomo_model,
+            index_set,
+            system_model,
+            financial_model,
+            block_set_name=block_set_name,
+        )
         self._create_linking_constraints()
 
-        self.objective_cost_terms = {'cost_per_field_generation': 0.5,
-                                     'cost_per_field_start_rel': 1.5,
-                                     'cost_per_cycle_generation': 2.0,
-                                     'cost_per_cycle_start_rel': 40.0,
-                                     'cost_per_change_thermal_input': 0.5}
+        self.objective_cost_terms = {
+            "cost_per_field_generation": 0.5,
+            "cost_per_field_start_rel": 1.5,
+            "cost_per_cycle_generation": 2.0,
+            "cost_per_cycle_start_rel": 40.0,
+            "cost_per_change_thermal_input": 0.5,
+        }
 
     def dispatch_block_rule(self, csp):
-        """
-        Called during Dispatch's __init__
+        """Called during Dispatch's __init__. Define dispatch block rules.
+
+        Args:
+            csp: CSP instance.
+
         """
         # Parameters
         self._create_storage_parameters(csp)
         self._create_receiver_parameters(csp)
         self._create_cycle_parameters(csp)
         # Variables
         self._create_storage_variables(csp)
@@ -51,1060 +71,1585 @@
     ##################################
     # Parameters                     #
     ##################################
     # TODO: Commenting out all of the parameters currently not be used.
 
     @staticmethod
     def _create_storage_parameters(csp):
+        """Create parameters related to thermal energy storage.
+
+        Args:
+            csp: CSP instance.
+
+        """
+
         csp.time_duration = pyomo.Param(
             doc="Time step [hour]",
             default=1.0,
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.hr)
+            units=u.hr,
+        )
         csp.storage_capacity = pyomo.Param(
             doc="Thermal energy storage capacity [MWht]",
             default=0.0,
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.MWh)
+            units=u.MWh,
+        )
 
     @staticmethod
     def _create_receiver_parameters(csp):
+        """Create parameters related to CSP receiver.
+
+        Args:
+            csp: CSP instance.
+
+        """
         # Cost Parameters
         csp.cost_per_field_generation = pyomo.Param(
             doc="Generation cost for the CSP field and receiver [$/MWht]",
             default=0.0,
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.USD / u.MWh)
+            units=u.USD / u.MWh,
+        )
         csp.cost_per_field_start = pyomo.Param(
             doc="Fixed cost for receiver start-up [$/start]",
             default=0.0,
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.USD)  # $/start
+            units=u.USD,
+        )  # $/start
         # Performance Parameters
         csp.available_thermal_generation = pyomo.Param(
             doc="Available thermal power generated by the CSP heliostat field [MWt]",
             default=0.0,
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.MW)
+            units=u.MW,
+        )
         csp.receiver_startup_fraction = pyomo.Param(
             doc="Estimated fraction of time period required for receiver start-up [-]",
             default=1.0,
             within=pyomo.PercentFraction,
             mutable=True,
-            units=u.dimensionless)
+            units=u.dimensionless,
+        )
         csp.min_receiver_start_time = pyomo.Param(
             doc="Minimum time to start the receiver [hr]",
             default=0.5,
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.hr)
+            units=u.hr,
+        )
         csp.field_startup_losses = pyomo.Param(
             doc="Heliostat field startup or shut down parasitic loss [MWhe]",
             default=0.0,
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.MWh)
+            units=u.MWh,
+        )
         csp.receiver_required_startup_energy = pyomo.Param(
             doc="Required energy expended to start receiver [MWht]",
             default=0.0,
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.MWh)
+            units=u.MWh,
+        )
         csp.receiver_pumping_losses = pyomo.Param(
             doc="Solar field and/or receiver pumping power per unit power produced [MWe/MWt]",
             default=0.0,
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.dimensionless)
+            units=u.dimensionless,
+        )
         csp.minimum_receiver_power = pyomo.Param(
             doc="Minimum operational thermal power delivered by receiver [MWt]",
             default=1.0,
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.MW)
+            units=u.MW,
+        )
         csp.allowable_receiver_startup_power = pyomo.Param(
             doc="Allowable power per period for receiver start-up [MWt]",
             default=0.0,
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.MW)
+            units=u.MW,
+        )
         csp.field_track_losses = pyomo.Param(
             doc="Solar field tracking parasitic loss [MWe]",
             default=0.0,
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.MW)
+            units=u.MW,
+        )
         # csp.heat_trace_losses = pyomo.Param(
         #     doc="Piping heat trace parasitic loss [MWe]",
         #     default=0.0,
         #     within=pyomo.NonNegativeReals,
         #     mutable=True,
         #     units=u.MW)
 
     @staticmethod
     def _create_cycle_parameters(csp):
+        """Create parameters related to the power cycle.
+
+        Args:
+            csp: CSP instance.
+
+        """
         # Cost parameters
         csp.cost_per_cycle_generation = pyomo.Param(
             doc="Generation cost for power cycle [$/MWh]",
             default=0.0,
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.USD / u.MWh)  # Electric
+            units=u.USD / u.MWh,
+        )  # Electric
         csp.cost_per_cycle_start = pyomo.Param(
             doc="Fixed cost for power cycle start [$/start]",
             default=0.0,
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.USD)  # $/start
+            units=u.USD,
+        )  # $/start
         csp.cost_per_change_thermal_input = pyomo.Param(
             doc="Penalty for change in power cycle thermal input [$/MWt]",
             default=0.0,
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.USD / u.MW)  # $/(Delta)MW (thermal)
+            units=u.USD / u.MW,
+        )  # $/(Delta)MW (thermal)
         # Performance parameters
         csp.cycle_ambient_efficiency_correction = pyomo.Param(
             doc="Cycle efficiency ambient temperature adjustment [-]",
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.dimensionless)
+            units=u.dimensionless,
+        )
         csp.condenser_losses = pyomo.Param(
             doc="Normalized condenser parasitic losses [-]",
             default=0.0,
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.dimensionless)
+            units=u.dimensionless,
+        )
         csp.cycle_required_startup_energy = pyomo.Param(
             doc="Required energy expended to start cycle [MWht]",
             default=0.0,
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.MWh)
+            units=u.MWh,
+        )
         csp.cycle_nominal_efficiency = pyomo.Param(
             doc="Power cycle nominal efficiency [-]",
             default=0.0,
             within=pyomo.PercentFraction,
             mutable=True,
-            units=u.dimensionless)
+            units=u.dimensionless,
+        )
         csp.cycle_performance_slope = pyomo.Param(
             doc="Slope of linear approximation of power cycle performance curve [MWe/MWt]",
             default=0.0,
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.dimensionless)
+            units=u.dimensionless,
+        )
         csp.cycle_pumping_losses = pyomo.Param(
             doc="Cycle heat transfer fluid pumping power per unit energy expended [MWe/MWt]",
             default=0.0,
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.dimensionless)
+            units=u.dimensionless,
+        )
         csp.allowable_cycle_startup_power = pyomo.Param(
             doc="Allowable power per period for cycle start-up [MWt]",
             default=0.0,
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.MW)
+            units=u.MW,
+        )
         csp.minimum_cycle_thermal_power = pyomo.Param(
             doc="Minimum operational thermal power delivered to the power cycle [MWt]",
             default=0.0,
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.MW)
+            units=u.MW,
+        )
         csp.maximum_cycle_thermal_power = pyomo.Param(
             doc="Maximum operational thermal power delivered to the power cycle [MWt]",
             default=0.0,
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.MW)
+            units=u.MW,
+        )
         # csp.minimum_cycle_power = pyomo.Param(
         #     doc="Minimum cycle electric power output [MWe]",
         #     default=0.0,
         #     within=pyomo.NonNegativeReals,
         #     mutable=True,
         #     units=u.MW)
         csp.maximum_cycle_power = pyomo.Param(
             doc="Maximum cycle electric power output [MWe]",
             default=0.0,
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.MW)
+            units=u.MW,
+        )
 
     ##################################
     # Variables                      #
     ##################################
 
     @staticmethod
     def _create_storage_variables(csp):
+        """Create variables related to thermal energy storage.
+
+        Args:
+            csp: CSP instance.
+
+        """
         csp.thermal_energy_storage = pyomo.Var(
             doc="Thermal energy storage reserve quantity [MWht]",
             domain=pyomo.NonNegativeReals,
             bounds=(0, csp.storage_capacity),
-            units=u.MWh)
+            units=u.MWh,
+        )
         # initial variables
         csp.previous_thermal_energy_storage = pyomo.Var(
             doc="Thermal energy storage reserve quantity at the beginning of the period [MWht]",
             domain=pyomo.NonNegativeReals,
             bounds=(0, csp.storage_capacity),
-            units=u.MWh)
+            units=u.MWh,
+        )
 
     @staticmethod
     def _create_receiver_variables(csp):
+        """Create variables related to the receiver.
+
+        Args:
+            csp: CSP instance.
+
+        """
         csp.receiver_startup_inventory = pyomo.Var(
             doc="Receiver start-up energy inventory [MWht]",
             domain=pyomo.NonNegativeReals,
-            units=u.MWh)
+            units=u.MWh,
+        )
         csp.receiver_thermal_power = pyomo.Var(
             doc="Thermal power delivered by the receiver [MWt]",
             domain=pyomo.NonNegativeReals,
-            units=u.MW)
+            units=u.MW,
+        )
         csp.receiver_startup_consumption = pyomo.Var(
             doc="Receiver start-up power consumption [MWt]",
             domain=pyomo.NonNegativeReals,
-            units=u.MW)
+            units=u.MW,
+        )
         csp.is_field_generating = pyomo.Var(
             doc="1 if solar field is generating 'usable' thermal power; 0 Otherwise [-]",
             domain=pyomo.Binary,
-            units=u.dimensionless)
+            units=u.dimensionless,
+        )
         csp.is_field_starting = pyomo.Var(
             doc="1 if solar field is starting up; 0 Otherwise [-]",
             domain=pyomo.Binary,
-            units=u.dimensionless)
+            units=u.dimensionless,
+        )
         csp.incur_field_start = pyomo.Var(
             doc="1 if solar field start-up penalty is incurred; 0 Otherwise [-]",
             domain=pyomo.Binary,
-            units=u.dimensionless)
+            units=u.dimensionless,
+        )
         # initial variables
         csp.previous_receiver_startup_inventory = pyomo.Var(
             doc="Previous receiver start-up energy inventory [MWht]",
             domain=pyomo.NonNegativeReals,
-            units=u.MWh)
+            units=u.MWh,
+        )
         csp.was_field_generating = pyomo.Var(
             doc="1 if solar field was generating 'usable' thermal power in the previous time period; 0 Otherwise [-]",
             domain=pyomo.Binary,
-            units=u.dimensionless)
+            units=u.dimensionless,
+        )
         csp.was_field_starting = pyomo.Var(
             doc="1 if solar field was starting up in the previous time period; 0 Otherwise [-]",
             domain=pyomo.Binary,
-            units=u.dimensionless)
+            units=u.dimensionless,
+        )
 
     @staticmethod
     def _create_cycle_variables(csp):
+        """Create variables related to the power cycle.
+
+        Args:
+            csp: CSP instance.
+
+        """
         csp.system_load = pyomo.Var(
-            doc="Load of csp system [MWe]",
-            domain=pyomo.NonNegativeReals,
-            units=u.MW)
+            doc="Load of csp system [MWe]", domain=pyomo.NonNegativeReals, units=u.MW
+        )
         csp.cycle_startup_inventory = pyomo.Var(
             doc="Cycle start-up energy inventory [MWht]",
             domain=pyomo.NonNegativeReals,
-            units=u.MWh)
+            units=u.MWh,
+        )
         csp.cycle_generation = pyomo.Var(
             doc="Power cycle electricity generation [MWe]",
             domain=pyomo.NonNegativeReals,
-            units=u.MW)
+            units=u.MW,
+        )
         csp.cycle_thermal_ramp = pyomo.Var(
             doc="Power cycle positive change in thermal energy input [MWt]",
             domain=pyomo.NonNegativeReals,
             bounds=(0, csp.maximum_cycle_thermal_power),
-            units=u.MW)
+            units=u.MW,
+        )
         csp.cycle_thermal_power = pyomo.Var(
             doc="Cycle thermal power utilization [MWt]",
             domain=pyomo.NonNegativeReals,
             bounds=(0, csp.maximum_cycle_thermal_power),
-            units=u.MW)
+            units=u.MW,
+        )
         csp.is_cycle_generating = pyomo.Var(
             doc="1 if cycle is generating electric power; 0 Otherwise [-]",
             domain=pyomo.Binary,
-            units=u.dimensionless)
+            units=u.dimensionless,
+        )
         csp.is_cycle_starting = pyomo.Var(
             doc="1 if cycle is starting up; 0 Otherwise [-]",
             domain=pyomo.Binary,
-            units=u.dimensionless)
+            units=u.dimensionless,
+        )
         csp.incur_cycle_start = pyomo.Var(
             doc="1 if cycle start-up penalty is incurred; 0 Otherwise [-]",
             domain=pyomo.Binary,
-            units=u.dimensionless)
+            units=u.dimensionless,
+        )
         # Initial variables
         csp.previous_cycle_startup_inventory = pyomo.Var(
             doc="Previous cycle start-up energy inventory [MWht]",
             domain=pyomo.NonNegativeReals,
-            units=u.MWh)
+            units=u.MWh,
+        )
         csp.previous_cycle_thermal_power = pyomo.Var(
             doc="Cycle thermal power in the previous period [MWt]",
             domain=pyomo.NonNegativeReals,
             bounds=(0, csp.maximum_cycle_thermal_power),
-            units=u.MW)
+            units=u.MW,
+        )
         csp.was_cycle_generating = pyomo.Var(
             doc="1 if cycle was generating electric power in previous time period; 0 Otherwise [-]",
             domain=pyomo.Binary,
-            units=u.dimensionless)
+            units=u.dimensionless,
+        )
         csp.was_cycle_starting = pyomo.Var(
             doc="1 if cycle was starting up in previous time period; 0 Otherwise [-]",
             domain=pyomo.Binary,
-            units=u.dimensionless)
+            units=u.dimensionless,
+        )
 
     ##################################
     # Constraints                    #
     ##################################
 
     @staticmethod
     def _create_storage_constraints(csp):
+        """Create constraints related to thermal energy storage.
+
+        Args:
+            csp: CSP instance.
+
+        """
         csp.storage_inventory = pyomo.Constraint(
             doc="Thermal energy storage energy balance",
-            expr=(csp.thermal_energy_storage - csp.previous_thermal_energy_storage ==
-                  csp.time_duration * (csp.receiver_thermal_power
-                                       - (csp.allowable_cycle_startup_power * csp.is_cycle_starting
-                                          + csp.cycle_thermal_power)
-                                       )
-                  ))
+            expr=(
+                csp.thermal_energy_storage - csp.previous_thermal_energy_storage
+                == csp.time_duration
+                * (
+                    csp.receiver_thermal_power
+                    - (
+                        csp.allowable_cycle_startup_power * csp.is_cycle_starting
+                        + csp.cycle_thermal_power
+                    )
+                )
+            ),
+        )
         csp.receiver_startup = pyomo.Constraint(
             doc="If receiver is starting up, then there must be a sufficient charge level "
-                "in the TES in the previous time period",
-            expr=(csp.previous_thermal_energy_storage >= csp.time_duration * csp.receiver_startup_fraction
-                  * (csp.maximum_cycle_thermal_power * (-3 + csp.is_field_starting
-                                                        + csp.was_cycle_generating + csp.is_cycle_generating)
-                     + csp.cycle_thermal_power))
+            "in the TES in the previous time period",
+            expr=(
+                csp.previous_thermal_energy_storage
+                >= csp.time_duration
+                * csp.receiver_startup_fraction
+                * (
+                    csp.maximum_cycle_thermal_power
+                    * (
+                        -3
+                        + csp.is_field_starting
+                        + csp.was_cycle_generating
+                        + csp.is_cycle_generating
+                    )
+                    + csp.cycle_thermal_power
+                )
+            ),
         )
 
     @staticmethod
     def _create_receiver_constraints(csp):
+        """Create constraints related to the receiver.
+
+        Args:
+            csp: CSP instance.
+
+        """
         # Start-up
         csp.receiver_startup_inventory_balance = pyomo.Constraint(
             doc="Receiver startup energy inventory balance",
-            expr=csp.receiver_startup_inventory <= (csp.previous_receiver_startup_inventory
-                                                    + csp.time_duration * csp.receiver_startup_consumption))
+            expr=csp.receiver_startup_inventory
+            <= (
+                csp.previous_receiver_startup_inventory
+                + csp.time_duration * csp.receiver_startup_consumption
+            ),
+        )
         csp.receiver_startup_inventory_reset = pyomo.Constraint(
             doc="Resets receiver and/or field startup inventory when startup is completed",
-            expr=csp.receiver_startup_inventory <= csp.receiver_required_startup_energy * csp.is_field_starting)
+            expr=csp.receiver_startup_inventory
+            <= csp.receiver_required_startup_energy * csp.is_field_starting,
+        )
         csp.receiver_operation_startup = pyomo.Constraint(
             doc="Thermal production is allowed only upon completion of start-up or operating in previous time period",
-            expr=csp.is_field_generating <= (csp.receiver_startup_inventory
-                                             / csp.receiver_required_startup_energy) + csp.was_field_generating)
+            expr=csp.is_field_generating
+            <= (csp.receiver_startup_inventory / csp.receiver_required_startup_energy)
+            + csp.was_field_generating,
+        )
         csp.receiver_startup_delay = pyomo.Constraint(
             doc="If field previously was producing, it cannot startup this period",
-            expr=csp.is_field_starting + csp.was_field_generating <= 1)
+            expr=csp.is_field_starting + csp.was_field_generating <= 1,
+        )
         csp.receiver_startup_limit = pyomo.Constraint(
             doc="Receiver and/or field startup energy consumption limit",
-            expr=csp.receiver_startup_consumption <= (csp.allowable_receiver_startup_power
-                                                      * csp.is_field_starting))
+            expr=csp.receiver_startup_consumption
+            <= (csp.allowable_receiver_startup_power * csp.is_field_starting),
+        )
         csp.receiver_startup_cut = pyomo.Constraint(
             doc="Receiver and/or field trivial resource startup cut",
-            expr=csp.is_field_starting <= csp.available_thermal_generation / csp.minimum_receiver_power)
+            expr=csp.is_field_starting
+            <= csp.available_thermal_generation / csp.minimum_receiver_power,
+        )
         # Supply and demand
         csp.receiver_energy_balance = pyomo.Constraint(
             doc="Receiver generation and startup usage must be below available",
-            expr=csp.available_thermal_generation >= csp.receiver_thermal_power + csp.receiver_startup_consumption)
+            expr=csp.available_thermal_generation
+            >= csp.receiver_thermal_power + csp.receiver_startup_consumption,
+        )
         csp.maximum_field_generation = pyomo.Constraint(
             doc="Receiver maximum generation limit",
-            expr=csp.receiver_thermal_power <= csp.available_thermal_generation * csp.is_field_generating)
+            expr=csp.receiver_thermal_power
+            <= csp.available_thermal_generation * csp.is_field_generating,
+        )
         csp.minimum_field_generation = pyomo.Constraint(
             doc="Receiver minimum generation limit",
-            expr=csp.receiver_thermal_power >= csp.minimum_receiver_power * csp.is_field_generating)
+            expr=csp.receiver_thermal_power
+            >= csp.minimum_receiver_power * csp.is_field_generating,
+        )
         csp.receiver_generation_cut = pyomo.Constraint(
             doc="Receiver and/or field trivial resource generation cut",
-            expr=csp.is_field_generating <= csp.available_thermal_generation / csp.minimum_receiver_power)
+            expr=csp.is_field_generating
+            <= csp.available_thermal_generation / csp.minimum_receiver_power,
+        )
         # Logic associated with receiver modes
         csp.field_startup = pyomo.Constraint(
             doc="Ensures that field start is accounted",
-            expr=csp.incur_field_start >= csp.is_field_starting - csp.was_field_starting)
+            expr=csp.incur_field_start
+            >= csp.is_field_starting - csp.was_field_starting,
+        )
 
     @staticmethod
     def _create_cycle_constraints(csp):
+        """Create constraints related to the power cycle.
+
+        Args:
+            csp: CSP instance.
+
+        """
         # Start-up
         csp.cycle_startup_inventory_balance = pyomo.Constraint(
             doc="Cycle startup energy inventory balance",
-            expr=csp.cycle_startup_inventory <= (csp.previous_cycle_startup_inventory
-                                                 + (csp.time_duration
-                                                    * csp.allowable_cycle_startup_power
-                                                    * csp.is_cycle_starting)))
+            expr=csp.cycle_startup_inventory
+            <= (
+                csp.previous_cycle_startup_inventory
+                + (
+                    csp.time_duration
+                    * csp.allowable_cycle_startup_power
+                    * csp.is_cycle_starting
+                )
+            ),
+        )
         csp.cycle_startup_inventory_reset = pyomo.Constraint(
             doc="Resets power cycle startup inventory when startup is completed",
-            expr=csp.cycle_startup_inventory <= csp.cycle_required_startup_energy * csp.is_cycle_starting)
+            expr=csp.cycle_startup_inventory
+            <= csp.cycle_required_startup_energy * csp.is_cycle_starting,
+        )
         csp.cycle_operation_startup = pyomo.Constraint(
             doc="Electric production is allowed only upon completion of start-up or operating in previous time period",
-            expr=csp.is_cycle_generating <= (csp.cycle_startup_inventory
-                                             / csp.cycle_required_startup_energy) + csp.was_cycle_generating)
+            expr=csp.is_cycle_generating
+            <= (csp.cycle_startup_inventory / csp.cycle_required_startup_energy)
+            + csp.was_cycle_generating,
+        )
         csp.cycle_startup_delay = pyomo.Constraint(
             doc="If cycle previously was generating, it cannot startup this period",
-            expr=csp.is_cycle_starting + csp.was_cycle_generating <= 1)
+            expr=csp.is_cycle_starting + csp.was_cycle_generating <= 1,
+        )
         # Supply and demand
         # TODO: do we penalize start-up on valuable hours? I don't think I need this...
         csp.maximum_cycle_thermal_consumption_startup = pyomo.Constraint(
             doc="Power cycle maximum thermal energy consumption maximum limit including startup",
-            expr=(csp.cycle_thermal_power
-                  + (csp.cycle_required_startup_energy / csp.time_duration) * csp.is_cycle_starting
-                  <= csp.maximum_cycle_thermal_power))
+            expr=(
+                csp.cycle_thermal_power
+                + (csp.cycle_required_startup_energy / csp.time_duration)
+                * csp.is_cycle_starting
+                <= csp.maximum_cycle_thermal_power
+            ),
+        )
         csp.maximum_cycle_thermal_consumption = pyomo.Constraint(
             doc="Power cycle maximum thermal energy consumption maximum limit",
-            expr=csp.cycle_thermal_power <= csp.maximum_cycle_thermal_power * csp.is_cycle_generating)
+            expr=csp.cycle_thermal_power
+            <= csp.maximum_cycle_thermal_power * csp.is_cycle_generating,
+        )
         csp.minimum_cycle_thermal_consumption = pyomo.Constraint(
             doc="Power cycle minimum thermal energy consumption minimum limit",
-            expr=csp.cycle_thermal_power >= csp.minimum_cycle_thermal_power * csp.is_cycle_generating)
+            expr=csp.cycle_thermal_power
+            >= csp.minimum_cycle_thermal_power * csp.is_cycle_generating,
+        )
         csp.cycle_performance_curve = pyomo.Constraint(
             doc="Power cycle relationship between electrical power and thermal input with corrections "
-                "for ambient temperature",
-            expr=(csp.cycle_generation ==
-                  (csp.cycle_ambient_efficiency_correction / csp.cycle_nominal_efficiency)
-                  * (csp.cycle_performance_slope * csp.cycle_thermal_power
-                     + (csp.maximum_cycle_power - csp.cycle_performance_slope
-                        * csp.maximum_cycle_thermal_power) * csp.is_cycle_generating)))
+            "for ambient temperature",
+            expr=(
+                csp.cycle_generation
+                == (
+                    csp.cycle_ambient_efficiency_correction
+                    / csp.cycle_nominal_efficiency
+                )
+                * (
+                    csp.cycle_performance_slope * csp.cycle_thermal_power
+                    + (
+                        csp.maximum_cycle_power
+                        - csp.cycle_performance_slope * csp.maximum_cycle_thermal_power
+                    )
+                    * csp.is_cycle_generating
+                )
+            ),
+        )
         csp.cycle_thermal_ramp_constraint = pyomo.Constraint(
             doc="Positive ramping of power cycle thermal power",
-            expr=csp.cycle_thermal_ramp >= csp.cycle_thermal_power - csp.previous_cycle_thermal_power)
+            expr=csp.cycle_thermal_ramp
+            >= csp.cycle_thermal_power - csp.previous_cycle_thermal_power,
+        )
         # System load
         csp.generation_balance = pyomo.Constraint(
             doc="Calculates csp system load for grid model",
-            expr=csp.system_load == (csp.cycle_generation * csp.condenser_losses
-                                     + csp.receiver_pumping_losses * (csp.receiver_thermal_power
-                                                                      + csp.receiver_startup_consumption)
-                                     + csp.cycle_pumping_losses * (csp.cycle_thermal_power
-                                                                   + (csp.allowable_cycle_startup_power
-                                                                      * csp.is_cycle_starting))
-                                     + csp.field_track_losses * csp.is_field_generating
-                                     # + csp.heat_trace_losses * csp.is_field_starting
-                                     + (csp.field_startup_losses/csp.time_duration) * csp.is_field_starting))
+            expr=csp.system_load
+            == (
+                csp.cycle_generation * csp.condenser_losses
+                + csp.receiver_pumping_losses
+                * (csp.receiver_thermal_power + csp.receiver_startup_consumption)
+                + csp.cycle_pumping_losses
+                * (
+                    csp.cycle_thermal_power
+                    + (csp.allowable_cycle_startup_power * csp.is_cycle_starting)
+                )
+                + csp.field_track_losses * csp.is_field_generating
+                # + csp.heat_trace_losses * csp.is_field_starting
+                + (csp.field_startup_losses / csp.time_duration) * csp.is_field_starting
+            ),
+        )
         # Logic governing cycle modes
         csp.cycle_startup = pyomo.Constraint(
             doc="Ensures that cycle start is accounted",
-            expr=csp.incur_cycle_start >= csp.is_cycle_starting - csp.was_cycle_starting)
+            expr=csp.incur_cycle_start
+            >= csp.is_cycle_starting - csp.was_cycle_starting,
+        )
 
     ##################################
     # Ports                          #
     ##################################
 
     @staticmethod
     def _create_csp_port(csp):
+        """Create pyomo ports related to CSP instance.
+
+        Args:
+            csp: CSP instance.
+
+        """
         csp.port = Port()
         csp.port.add(csp.cycle_generation)
         csp.port.add(csp.system_load)
 
     ##################################
     # Linking Constraints            #
     ##################################
 
     def _create_linking_constraints(self):
+        """Create linking constraints for storage, receiver and cycle."""
         self._create_storage_linking_constraints()
         self._create_receiver_linking_constraints()
         self._create_cycle_linking_constraints()
 
     ##################################
     # Initial Parameters             #
     ##################################
 
     def _create_storage_linking_constraints(self):
+        """Create constraints for linking storage."""
         self.model.initial_thermal_energy_storage = pyomo.Param(
             doc="Initial thermal energy storage reserve quantity at beginning of the horizon [MWht]",
             default=0.0,
             within=pyomo.NonNegativeReals,
             # validate= # TODO: Might be worth looking into
             mutable=True,
-            units=u.MWh)
+            units=u.MWh,
+        )
 
         def tes_linking_rule(m, t):
             if t == self.blocks.index_set().first():
-                return self.blocks[t].previous_thermal_energy_storage == self.model.initial_thermal_energy_storage
-            return self.blocks[t].previous_thermal_energy_storage == self.blocks[t - 1].thermal_energy_storage
+                return (
+                    self.blocks[t].previous_thermal_energy_storage
+                    == self.model.initial_thermal_energy_storage
+                )
+            return (
+                self.blocks[t].previous_thermal_energy_storage
+                == self.blocks[t - 1].thermal_energy_storage
+            )
+
         self.model.tes_linking = pyomo.Constraint(
             self.blocks.index_set(),
             doc="Thermal energy storage block linking constraint",
-            rule=tes_linking_rule)
+            rule=tes_linking_rule,
+        )
 
     def _create_receiver_linking_constraints(self):
+        """Create constraints for linking receiver."""
         self.model.initial_receiver_startup_inventory = pyomo.Param(
             doc="Initial receiver start-up energy inventory at beginning of the horizon [MWht]",
             default=0.0,
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.MWh)
+            units=u.MWh,
+        )
         self.model.is_field_generating_initial = pyomo.Param(
             doc="1 if solar field is generating 'usable' thermal power at beginning of the horizon; 0 Otherwise [-]",
             default=0.0,
             within=pyomo.Binary,
             mutable=True,
-            units=u.dimensionless)
+            units=u.dimensionless,
+        )
         self.model.is_field_starting_initial = pyomo.Param(
             doc="1 if solar field is starting up at beginning of the horizon; 0 Otherwise [-]",
             default=0.0,
             within=pyomo.Binary,
             mutable=True,
-            units=u.dimensionless)
+            units=u.dimensionless,
+        )
 
         def receiver_startup_inventory_linking_rule(m, t):
             if t == self.blocks.index_set().first():
-                return self.blocks[t].previous_receiver_startup_inventory == self.model.initial_receiver_startup_inventory
-            return self.blocks[t].previous_receiver_startup_inventory == self.blocks[t - 1].receiver_startup_inventory
+                return (
+                    self.blocks[t].previous_receiver_startup_inventory
+                    == self.model.initial_receiver_startup_inventory
+                )
+            return (
+                self.blocks[t].previous_receiver_startup_inventory
+                == self.blocks[t - 1].receiver_startup_inventory
+            )
+
         self.model.receiver_startup_inventory_linking = pyomo.Constraint(
             self.blocks.index_set(),
             doc="Receiver startup inventory block linking constraint",
-            rule=receiver_startup_inventory_linking_rule)
+            rule=receiver_startup_inventory_linking_rule,
+        )
 
         def field_generating_linking_rule(m, t):
             if t == self.blocks.index_set().first():
-                return self.blocks[t].was_field_generating == self.model.is_field_generating_initial
-            return self.blocks[t].was_field_generating == self.blocks[t - 1].is_field_generating
+                return (
+                    self.blocks[t].was_field_generating
+                    == self.model.is_field_generating_initial
+                )
+            return (
+                self.blocks[t].was_field_generating
+                == self.blocks[t - 1].is_field_generating
+            )
+
         self.model.field_generating_linking = pyomo.Constraint(
             self.blocks.index_set(),
             doc="Is field generating binary block linking constraint",
-            rule=field_generating_linking_rule)
+            rule=field_generating_linking_rule,
+        )
 
         def field_starting_linking_rule(m, t):
             if t == self.blocks.index_set().first():
-                return self.blocks[t].was_field_starting == self.model.is_field_starting_initial
-            return self.blocks[t].was_field_starting == self.blocks[t - 1].is_field_starting
+                return (
+                    self.blocks[t].was_field_starting
+                    == self.model.is_field_starting_initial
+                )
+            return (
+                self.blocks[t].was_field_starting
+                == self.blocks[t - 1].is_field_starting
+            )
+
         self.model.field_starting_linking = pyomo.Constraint(
             self.blocks.index_set(),
             doc="Is field starting up binary block linking constraint",
-            rule=field_starting_linking_rule)
+            rule=field_starting_linking_rule,
+        )
 
     def _create_cycle_linking_constraints(self):
+        """Create constraints for linking cycle."""
         self.model.initial_cycle_startup_inventory = pyomo.Param(
             doc="Initial cycle start-up energy inventory at beginning of the horizon [MWht]",
             default=0.0,
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.MWh)
+            units=u.MWh,
+        )
         self.model.initial_cycle_thermal_power = pyomo.Param(
             doc="Initial cycle thermal power at beginning of the horizon [MWt]",
             default=0.0,
             within=pyomo.NonNegativeReals,
             # validate= # TODO: bounds->(0, csp.maximum_cycle_thermal_power), Sec. 4.7.1
             mutable=True,
-            units=u.MW)
+            units=u.MW,
+        )
         self.model.is_cycle_generating_initial = pyomo.Param(
             doc="1 if cycle is generating electric power at beginning of the horizon; 0 Otherwise [-]",
             default=0.0,
             within=pyomo.Binary,
             mutable=True,
-            units=u.dimensionless)
+            units=u.dimensionless,
+        )
         self.model.is_cycle_starting_initial = pyomo.Param(
             doc="1 if cycle is starting up at beginning of the horizon; 0 Otherwise [-]",
             default=0.0,
             within=pyomo.Binary,
             mutable=True,
-            units=u.dimensionless)
+            units=u.dimensionless,
+        )
 
         def cycle_startup_inventory_linking_rule(m, t):
             if t == self.blocks.index_set().first():
-                return self.blocks[t].previous_cycle_startup_inventory == self.model.initial_cycle_startup_inventory
-            return self.blocks[t].previous_cycle_startup_inventory == self.blocks[t - 1].cycle_startup_inventory
+                return (
+                    self.blocks[t].previous_cycle_startup_inventory
+                    == self.model.initial_cycle_startup_inventory
+                )
+            return (
+                self.blocks[t].previous_cycle_startup_inventory
+                == self.blocks[t - 1].cycle_startup_inventory
+            )
+
         self.model.cycle_startup_inventory_linking = pyomo.Constraint(
             self.blocks.index_set(),
             doc="Cycle startup inventory block linking constraint",
-            rule=cycle_startup_inventory_linking_rule)
+            rule=cycle_startup_inventory_linking_rule,
+        )
 
         def cycle_thermal_power_linking_rule(m, t):
             if t == self.blocks.index_set().first():
-                return self.blocks[t].previous_cycle_thermal_power == self.model.initial_cycle_thermal_power
-            return self.blocks[t].previous_cycle_thermal_power == self.blocks[t - 1].cycle_thermal_power
+                return (
+                    self.blocks[t].previous_cycle_thermal_power
+                    == self.model.initial_cycle_thermal_power
+                )
+            return (
+                self.blocks[t].previous_cycle_thermal_power
+                == self.blocks[t - 1].cycle_thermal_power
+            )
+
         self.model.cycle_thermal_power_linking = pyomo.Constraint(
             self.blocks.index_set(),
             doc="Cycle thermal power block linking constraint",
-            rule=cycle_thermal_power_linking_rule)
+            rule=cycle_thermal_power_linking_rule,
+        )
 
         def cycle_generating_linking_rule(m, t):
             if t == self.blocks.index_set().first():
-                return self.blocks[t].was_cycle_generating == self.model.is_cycle_generating_initial
-            return self.blocks[t].was_cycle_generating == self.blocks[t - 1].is_cycle_generating
+                return (
+                    self.blocks[t].was_cycle_generating
+                    == self.model.is_cycle_generating_initial
+                )
+            return (
+                self.blocks[t].was_cycle_generating
+                == self.blocks[t - 1].is_cycle_generating
+            )
+
         self.model.cycle_generating_linking = pyomo.Constraint(
             self.blocks.index_set(),
             doc="Is cycle generating binary block linking constraint",
-            rule=cycle_generating_linking_rule)
+            rule=cycle_generating_linking_rule,
+        )
 
         def cycle_starting_linking_rule(m, t):
             if t == self.blocks.index_set().first():
-                return self.blocks[t].was_cycle_starting == self.model.is_cycle_starting_initial
-            return self.blocks[t].was_cycle_starting == self.blocks[t - 1].is_cycle_starting
+                return (
+                    self.blocks[t].was_cycle_starting
+                    == self.model.is_cycle_starting_initial
+                )
+            return (
+                self.blocks[t].was_cycle_starting
+                == self.blocks[t - 1].is_cycle_starting
+            )
+
         self.model.cycle_starting_linking = pyomo.Constraint(
             self.blocks.index_set(),
             doc="Is cycle starting up binary block linking constraint",
-            rule=cycle_starting_linking_rule)
+            rule=cycle_starting_linking_rule,
+        )
 
     def initialize_parameters(self):
+        """Initialize parameters for the CSP model."""
         csp = self._system_model
 
         cycle_rated_thermal = csp.cycle_thermal_rating
         field_rated_thermal = csp.field_thermal_rating
 
         # Cost Parameters
-        self.cost_per_field_generation = self.objective_cost_terms['cost_per_field_generation']
-        self.cost_per_field_start = self.objective_cost_terms['cost_per_field_start_rel'] * field_rated_thermal
-        self.cost_per_cycle_generation = self.objective_cost_terms['cost_per_cycle_generation']
-        self.cost_per_cycle_start = self.objective_cost_terms['cost_per_cycle_start_rel'] * csp.value('P_ref')
-        self.cost_per_change_thermal_input = self.objective_cost_terms['cost_per_change_thermal_input']
+        self.cost_per_field_generation = self.objective_cost_terms[
+            "cost_per_field_generation"
+        ]
+        self.cost_per_field_start = (
+            self.objective_cost_terms["cost_per_field_start_rel"] * field_rated_thermal
+        )
+        self.cost_per_cycle_generation = self.objective_cost_terms[
+            "cost_per_cycle_generation"
+        ]
+        self.cost_per_cycle_start = self.objective_cost_terms[
+            "cost_per_cycle_start_rel"
+        ] * csp.value("P_ref")
+        self.cost_per_change_thermal_input = self.objective_cost_terms[
+            "cost_per_change_thermal_input"
+        ]
 
         # Solar field and thermal energy storage performance parameters
-        self.field_startup_losses = csp.value('p_start') * csp.number_of_reflector_units / 1e3
-        self.receiver_required_startup_energy = csp.value('rec_qf_delay') * field_rated_thermal
+        self.field_startup_losses = (
+            csp.value("p_start") * csp.number_of_reflector_units / 1e3
+        )
+        self.receiver_required_startup_energy = (
+            csp.value("rec_qf_delay") * field_rated_thermal
+        )
         self.storage_capacity = csp.tes_hours * cycle_rated_thermal
-        self.minimum_receiver_power = csp.minimum_receiver_power_fraction * field_rated_thermal
-        self.allowable_receiver_startup_power = self.receiver_required_startup_energy / csp.value('rec_su_delay')
+        self.minimum_receiver_power = (
+            csp.minimum_receiver_power_fraction * field_rated_thermal
+        )
+        self.allowable_receiver_startup_power = (
+            self.receiver_required_startup_energy / csp.value("rec_su_delay")
+        )
         self.receiver_pumping_losses = csp.estimate_receiver_pumping_parasitic()
         self.field_track_losses = csp.field_tracking_power
-        #self.heat_trace_losses = 0.00163 * field_rated_thermal     # TODO: need to update for troughs
+        # self.heat_trace_losses = 0.00163 * field_rated_thermal     # TODO: need to update for troughs
 
         # Power cycle performance
-        self.cycle_required_startup_energy = csp.value('startup_frac') * cycle_rated_thermal
+        self.cycle_required_startup_energy = (
+            csp.value("startup_frac") * cycle_rated_thermal
+        )
         self.cycle_nominal_efficiency = csp.cycle_nominal_efficiency
 
         design_mass_flow = csp.get_cycle_design_mass_flow()
-        self.cycle_pumping_losses = csp.value('pb_pump_coef') * design_mass_flow / (cycle_rated_thermal * 1e3)
-        self.allowable_cycle_startup_power = self.cycle_required_startup_energy / csp.value('startup_time')
-        self.minimum_cycle_thermal_power = csp.value('cycle_cutoff_frac') * cycle_rated_thermal
-        self.maximum_cycle_thermal_power = csp.value('cycle_max_frac') * cycle_rated_thermal
+        self.cycle_pumping_losses = (
+            csp.value("pb_pump_coef") * design_mass_flow / (cycle_rated_thermal * 1e3)
+        )
+        self.allowable_cycle_startup_power = (
+            self.cycle_required_startup_energy / csp.value("startup_time")
+        )
+        self.minimum_cycle_thermal_power = (
+            csp.value("cycle_cutoff_frac") * cycle_rated_thermal
+        )
+        self.maximum_cycle_thermal_power = (
+            csp.value("cycle_max_frac") * cycle_rated_thermal
+        )
         self.set_part_load_cycle_parameters()
 
     def update_time_series_parameters(self, start_time: int):
-        """
-        Sets up SSC simulation to get time series performance parameters after simulation.
-        : param start_time: hour of the year starting dispatch horizon
+        """Sets up SSC simulation to get time series performance parameters after simulation.
+
+        Args:
+            start_time (int): Hour of the year starting dispatch horizon.
+
         """
         n_horizon = len(self.blocks.index_set())
         self.time_duration = [1.0] * n_horizon  # assume hourly for now
 
         # Set available thermal energy based on forecast
         thermal_resource = self._system_model.solar_thermal_resource
         temperature = list(self._system_model.year_weather_df.Temperature.values)
         if start_time + n_horizon > len(thermal_resource):
             field_gen = list(thermal_resource[start_time:])
-            field_gen.extend(list(thermal_resource[0:n_horizon - len(field_gen)]))
+            field_gen.extend(list(thermal_resource[0 : n_horizon - len(field_gen)]))
 
             dry_bulb_temperature = list(temperature[start_time:])
-            dry_bulb_temperature.extend(list(temperature[0:n_horizon - len(dry_bulb_temperature)]))
+            dry_bulb_temperature.extend(
+                list(temperature[0 : n_horizon - len(dry_bulb_temperature)])
+            )
         else:
-            field_gen = thermal_resource[start_time:start_time + n_horizon]
-            dry_bulb_temperature = temperature[start_time:start_time + n_horizon]
+            field_gen = thermal_resource[start_time : start_time + n_horizon]
+            dry_bulb_temperature = temperature[start_time : start_time + n_horizon]
 
         self.available_thermal_generation = field_gen
         # Set cycle performance parameters that depend on ambient temperature
         self.set_ambient_temperature_cycle_parameters(dry_bulb_temperature)
         self.set_receiver_require_startup_time_fraction(field_gen)
 
         self.update_initial_conditions()  # other dispatch models do not have this method
 
     def set_part_load_cycle_parameters(self):
         """Set parameters in dispatch model for off-design cycle performance."""
         # --- Cycle part-load efficiency
         tables = self._system_model.cycle_efficiency_tables
-        if 'cycle_eff_load_table' in tables:
+        if "cycle_eff_load_table" in tables:
             q_pb_design = self._system_model.cycle_thermal_rating
-            num_pts = len(tables['cycle_eff_load_table'])
-            norm_heat_pts = [tables['cycle_eff_load_table'][i][0] / q_pb_design for i in range(num_pts)]  # Load fraction
-            efficiency_pts = [tables['cycle_eff_load_table'][i][1] for i in range(num_pts)]  # Efficiency
+            num_pts = len(tables["cycle_eff_load_table"])
+            norm_heat_pts = [
+                tables["cycle_eff_load_table"][i][0] / q_pb_design
+                for i in range(num_pts)
+            ]  # Load fraction
+            efficiency_pts = [
+                tables["cycle_eff_load_table"][i][1] for i in range(num_pts)
+            ]  # Efficiency
             self.set_linearized_cycle_part_load_params(norm_heat_pts, efficiency_pts)
-        elif 'ud_ind_od' in tables:
+        elif "ud_ind_od" in tables:
             # Tables not returned from ssc, but can be taken from user-defined cycle inputs
-            D = self.interpret_user_defined_cycle_data(tables['ud_ind_od'])
-            k = 3 * D['nT'] + D['nm']
-            norm_heat_pts = D['mpts']  # Load fraction
-            efficiency_pts = [self._system_model.cycle_nominal_efficiency * (tables['ud_ind_od'][k + p][3] / tables['ud_ind_od'][k + p][4])
-                              for p in range(len(norm_heat_pts))]  # Efficiency
+            D = self.interpret_user_defined_cycle_data(tables["ud_ind_od"])
+            k = 3 * D["nT"] + D["nm"]
+            norm_heat_pts = D["mpts"]  # Load fraction
+            efficiency_pts = [
+                self._system_model.cycle_nominal_efficiency
+                * (tables["ud_ind_od"][k + p][3] / tables["ud_ind_od"][k + p][4])
+                for p in range(len(norm_heat_pts))
+            ]  # Efficiency
             self.set_linearized_cycle_part_load_params(norm_heat_pts, efficiency_pts)
         else:
-            print('WARNING: Dispatch optimization cycle part-load efficiency is not set. '
-                  'Defaulting to constant efficiency vs load.')
+            print(
+                "WARNING: Dispatch optimization cycle part-load efficiency is not set. "
+                "Defaulting to constant efficiency vs load."
+            )
             self.cycle_performance_slope = self._system_model.cycle_nominal_efficiency
             # self.minimum_cycle_power = self.minimum_cycle_thermal_power * self._system_model.cycle_nominal_efficiency
-            self.maximum_cycle_power = self.maximum_cycle_thermal_power * self._system_model.cycle_nominal_efficiency
+            self.maximum_cycle_power = (
+                self.maximum_cycle_thermal_power
+                * self._system_model.cycle_nominal_efficiency
+            )
 
     def set_linearized_cycle_part_load_params(self, norm_heat_pts, efficiency_pts):
+        """Set linearized part-load parameters for the power cycle.
+
+        Args:
+            norm_heat_pts (list): Normalized heat points for the power cycle.
+            efficiency_pts (list): Efficiency points for the power cycle.
+
+        """
         q_pb_design = self._system_model.cycle_thermal_rating
-        fpts = [self._system_model.value('cycle_cutoff_frac'), self._system_model.value('cycle_max_frac')]
+        fpts = [
+            self._system_model.value("cycle_cutoff_frac"),
+            self._system_model.value("cycle_max_frac"),
+        ]
         step = norm_heat_pts[1] - norm_heat_pts[0]
-        q, eta = [ [] for v in range(2)]
+        q, eta = [[] for v in range(2)]
         for j in range(2):
             # Find first point in user-defined array of load fractions
-            p = max(0, min(int((fpts[j] - norm_heat_pts[0]) / step), len(norm_heat_pts) - 2))
-            eta.append(efficiency_pts[p] + (efficiency_pts[p + 1] - efficiency_pts[p]) / step * (fpts[j] - norm_heat_pts[p]))
-            q.append(fpts[j]*q_pb_design)
-        etap = (q[1]*eta[1]-q[0]*eta[0])/(q[1]-q[0])
-        b = q[1]*(eta[1] - etap)
+            p = max(
+                0, min(int((fpts[j] - norm_heat_pts[0]) / step), len(norm_heat_pts) - 2)
+            )
+            eta.append(
+                efficiency_pts[p]
+                + (efficiency_pts[p + 1] - efficiency_pts[p])
+                / step
+                * (fpts[j] - norm_heat_pts[p])
+            )
+            q.append(fpts[j] * q_pb_design)
+        etap = (q[1] * eta[1] - q[0] * eta[0]) / (q[1] - q[0])
+        b = q[1] * (eta[1] - etap)
         self.cycle_performance_slope = etap
         # self.minimum_cycle_power = b + self.minimum_cycle_thermal_power * self.cycle_performance_slope
-        self.maximum_cycle_power = b + self.maximum_cycle_thermal_power * self.cycle_performance_slope
+        self.maximum_cycle_power = (
+            b + self.maximum_cycle_thermal_power * self.cycle_performance_slope
+        )
         return
 
     def set_ambient_temperature_cycle_parameters(self, dry_bulb_temperature):
-        """Set ambient temperature dependent cycle performance parameters."""
+        """Set ambient temperature dependent cycle performance parameters.
+
+        Args:
+            dry_bulb_temperature (float or list): Ambient dry bulb temperature(s) [°C].
+
+        Returns:
+            None
+
+        Notes:
+            This method sets up ambient temperature dependent cycle performance parameters
+            such as cycle efficiency corrections and condenser losses based on the provided
+            dry bulb temperature(s).
+
+        """
         # --- Cycle ambient-temperature efficiency corrections
         tables = self._system_model.cycle_efficiency_tables
-        if 'cycle_eff_Tdb_table' in tables:
-            nT = len(tables['cycle_eff_Tdb_table'])
-            Tpts = [tables['cycle_eff_Tdb_table'][i][0] for i in range(nT)]
-            efficiency_pts = [tables['cycle_eff_Tdb_table'][i][1] * self._system_model.cycle_nominal_efficiency for i in range(nT)]  # Efficiency
-            wcondfpts = [tables['cycle_wcond_Tdb_table'][i][1] for i in range(nT)]  # Fraction of cycle design gross output consumed by cooling
-            self.set_cycle_ambient_corrections(dry_bulb_temperature, Tpts, efficiency_pts, wcondfpts)
-        elif 'ud_ind_od' in tables:
+        if "cycle_eff_Tdb_table" in tables:
+            nT = len(tables["cycle_eff_Tdb_table"])
+            Tpts = [tables["cycle_eff_Tdb_table"][i][0] for i in range(nT)]
+            efficiency_pts = [
+                tables["cycle_eff_Tdb_table"][i][1]
+                * self._system_model.cycle_nominal_efficiency
+                for i in range(nT)
+            ]  # Efficiency
+            wcondfpts = [
+                tables["cycle_wcond_Tdb_table"][i][1] for i in range(nT)
+            ]  # Fraction of cycle design gross output consumed by cooling
+            self.set_cycle_ambient_corrections(
+                dry_bulb_temperature, Tpts, efficiency_pts, wcondfpts
+            )
+        elif "ud_ind_od" in tables:
             # Tables not returned from ssc, but can be taken from user-defined cycle inputs
-            D = self.interpret_user_defined_cycle_data(tables['ud_ind_od'])
-            k = 3 * D['nT'] + 3 * D['nm'] + D[
-                'nTamb']  # first index in udpc data corresponding to performance at design point HTF T, and design point mass flow
-            npts = D['nTamb']
-            efficiency_pts = [self._system_model.cycle_nominal_efficiency * (tables['ud_ind_od'][j][3] / tables['ud_ind_od'][j][4])
-                              for j in range(k, k + npts)]  # Efficiency
-            wcondfpts = [(self._system_model.value('ud_f_W_dot_cool_des') / 100.) * tables['ud_ind_od'][j][5] for j in
-                         range(k, k + npts)]  # Fraction of cycle design gross output consumed by cooling
-            self.set_cycle_ambient_corrections(dry_bulb_temperature, D['Tambpts'], efficiency_pts, wcondfpts)
+            D = self.interpret_user_defined_cycle_data(tables["ud_ind_od"])
+            k = (
+                3 * D["nT"] + 3 * D["nm"] + D["nTamb"]
+            )  # first index in udpc data corresponding to performance at design point HTF T, and design point mass flow
+            npts = D["nTamb"]
+            efficiency_pts = [
+                self._system_model.cycle_nominal_efficiency
+                * (tables["ud_ind_od"][j][3] / tables["ud_ind_od"][j][4])
+                for j in range(k, k + npts)
+            ]  # Efficiency
+            wcondfpts = [
+                (self._system_model.value("ud_f_W_dot_cool_des") / 100.0)
+                * tables["ud_ind_od"][j][5]
+                for j in range(k, k + npts)
+            ]  # Fraction of cycle design gross output consumed by cooling
+            self.set_cycle_ambient_corrections(
+                dry_bulb_temperature, D["Tambpts"], efficiency_pts, wcondfpts
+            )
         else:
-            print('WARNING: Dispatch optimization cycle ambient temperature corrections are not set up.')
+            print(
+                "WARNING: Dispatch optimization cycle ambient temperature corrections are not set up."
+            )
             n = len(dry_bulb_temperature)
-            self.cycle_ambient_efficiency_correction = [self._system_model.cycle_nominal_efficiency] * n
+            self.cycle_ambient_efficiency_correction = [
+                self._system_model.cycle_nominal_efficiency
+            ] * n
             self.condenser_losses = [0.0] * n
         return
 
     def set_cycle_ambient_corrections(self, Tdb, Tpts, etapts, wcondfpts):
-        n = len(Tdb)            # Tdb = set of ambient temperature points for each dispatch time step
-        npts = len(Tpts)        # Tpts = ambient temperature points with tabulated values
-        cycle_ambient_efficiency_correction = [1.0]*n
-        condenser_losses = [0.0]*n
+        """Set cycle ambient corrections based on ambient temperature.
+
+        Args:
+            Tdb (float or list): Ambient temperature(s) for each dispatch time step [°C].
+            Tpts (list): Ambient temperature points with tabulated values [°C].
+            etapts (list): Efficiency values corresponding to each Tpts.
+            wcondfpts (list): Fraction of cycle design gross output consumed by cooling corresponding to each Tpts.
+
+        Returns:
+            None
+
+        Notes:
+            This method calculates cycle ambient efficiency correction and condenser losses based on the provided
+            ambient temperature(s) and tabulated values. The corrections are set for each dispatch time step.
+
+        """
+        n = len(
+            Tdb
+        )  # Tdb = set of ambient temperature points for each dispatch time step
+        npts = len(Tpts)  # Tpts = ambient temperature points with tabulated values
+        cycle_ambient_efficiency_correction = [1.0] * n
+        condenser_losses = [0.0] * n
         Tstep = Tpts[1] - Tpts[0]
         for j in range(n):
-            i = max(0, min( int((Tdb[j] - Tpts[0]) / Tstep), npts-2) )
+            i = max(0, min(int((Tdb[j] - Tpts[0]) / Tstep), npts - 2))
             r = (Tdb[j] - Tpts[i]) / Tstep
-            cycle_ambient_efficiency_correction[j] = etapts[i] + (etapts[i + 1] - etapts[i]) * r
+            cycle_ambient_efficiency_correction[j] = (
+                etapts[i] + (etapts[i + 1] - etapts[i]) * r
+            )
             condenser_losses[j] = wcondfpts[i] + (wcondfpts[i + 1] - wcondfpts[i]) * r
         self.cycle_ambient_efficiency_correction = cycle_ambient_efficiency_correction
         self.condenser_losses = condenser_losses
         return
 
     @staticmethod
     def interpret_user_defined_cycle_data(ud_ind_od):
+        """Interpret user-defined cycle data.
+
+        Args:
+            ud_ind_od (list): User-defined cycle data.
+
+        Returns:
+            dict: Dictionary containing interpreted data with keys:
+                - 'nT': Number of temperature points
+                - 'Tpts': Ambient temperature points
+                - 'Tlevels': Levels of temperature
+                - 'nm': Number of mass flow rate points
+                - 'mpts': Mass flow rate points
+                - 'mlevels': Levels of mass flow rate
+                - 'nTamb': Number of ambient temperature points
+                - 'Tambpts': Ambient temperature points
+                - 'Tamblevels': Levels of ambient temperature
+
+        Notes:
+            This method interprets user-defined cycle data and organizes it into a dictionary
+            containing relevant information about temperature points, mass flow rate points, and
+            ambient temperature points.
+
+        """
+
         data = np.array(ud_ind_od)
 
         i0 = 0
         nT = np.where(np.diff(data[i0::, 0]) < 0)[0][0] + 1
-        Tpts = data[i0:i0 + nT, 0]
+        Tpts = data[i0 : i0 + nT, 0]
         mlevels = [data[j, 1] for j in [i0, i0 + nT, i0 + 2 * nT]]
 
         i0 = 3 * nT
         nm = np.where(np.diff(data[i0::, 1]) < 0)[0][0] + 1
-        mpts = data[i0:i0 + nm, 1]
+        mpts = data[i0 : i0 + nm, 1]
         Tamblevels = [data[j, 2] for j in [i0, i0 + nm, i0 + 2 * nm]]
 
         i0 = 3 * nT + 3 * nm
         nTamb = np.where(np.diff(data[i0::, 2]) < 0)[0][0] + 1
-        Tambpts = data[i0:i0 + nTamb, 2]
+        Tambpts = data[i0 : i0 + nTamb, 2]
         Tlevels = [data[j, 0] for j in [i0, i0 + nm, i0 + 2 * nm]]
 
-        return {'nT': nT, 'Tpts': Tpts, 'Tlevels': Tlevels, 'nm': nm, 'mpts': mpts, 'mlevels': mlevels, 'nTamb': nTamb,
-                'Tambpts': Tambpts, 'Tamblevels': Tamblevels}
+        return {
+            "nT": nT,
+            "Tpts": Tpts,
+            "Tlevels": Tlevels,
+            "nm": nm,
+            "mpts": mpts,
+            "mlevels": mlevels,
+            "nTamb": nTamb,
+            "Tambpts": Tambpts,
+            "Tamblevels": Tamblevels,
+        }
 
     def set_receiver_require_startup_time_fraction(self, field_gen: list):
-        """Estimates the fraction of time period required for receiver start-up."""
-        self.min_receiver_start_time = self._system_model.value('rec_su_delay')
+        """Estimates the fraction of time period required for receiver start-up.
+
+        Args:
+            field_gen (list): Field generation profile.
+
+        Notes:
+            This method estimates the fraction of time period required for the receiver start-up
+            based on the field generation profile.
+
+        """
+        self.min_receiver_start_time = self._system_model.value("rec_su_delay")
 
         su_fraction = [1.0] * len(field_gen)
         epsilon = 1e-6
         time_duration = self.time_duration
 
         for i in range(len(field_gen)):
-            su_fraction[i] = min(1.0,
-                                 max(self.min_receiver_start_time / time_duration[i],
-                                     self.receiver_required_startup_energy / max(1e-6,
-                                                                                 field_gen[i] * time_duration[i])
-                                     )
-                                 )
+            su_fraction[i] = min(
+                1.0,
+                max(
+                    self.min_receiver_start_time / time_duration[i],
+                    self.receiver_required_startup_energy
+                    / max(1e-6, field_gen[i] * time_duration[i]),
+                ),
+            )
 
         self.receiver_startup_fraction = su_fraction
 
     def update_initial_conditions(self):
+        """This method updates the initial conditions for the dispatch optimization,
+        including the initial thermal energy storage, initial cycle startup inventory,
+        and initial cycle thermal power.
+
+        """
         csp = self._system_model
 
         m_des = csp.get_design_storage_mass()
-        m_hot = csp.initial_tes_hot_mass_fraction * m_des  # Available active mass in hot tank
-        cp = csp.get_cp_htf(0.5 * (csp.plant_state['T_tank_hot_init'] + csp.htf_cold_design_temperature))  # J/kg/K
-        self.initial_thermal_energy_storage = min(self.storage_capacity,
-                                                  m_hot * cp * (csp.plant_state['T_tank_hot_init']
-                                                                - csp.htf_cold_design_temperature) * 1.e-6 / 3600)
+        m_hot = (
+            csp.initial_tes_hot_mass_fraction * m_des
+        )  # Available active mass in hot tank
+        cp = csp.get_cp_htf(
+            0.5 * (csp.plant_state["T_tank_hot_init"] + csp.htf_cold_design_temperature)
+        )  # J/kg/K
+        self.initial_thermal_energy_storage = min(
+            self.storage_capacity,
+            m_hot
+            * cp
+            * (csp.plant_state["T_tank_hot_init"] - csp.htf_cold_design_temperature)
+            * 1.0e-6
+            / 3600,
+        )
 
-        self.is_field_generating_initial = (csp.plant_state['rec_op_mode_initial'] == 2)
-        self.is_field_starting_initial = (csp.plant_state['rec_op_mode_initial'] == 1)
+        self.is_field_generating_initial = csp.plant_state["rec_op_mode_initial"] == 2
+        self.is_field_starting_initial = csp.plant_state["rec_op_mode_initial"] == 1
 
         # Initial startup energy accumulated
         # ssc seems to report nan when startup is completed
-        if csp.plant_state['pc_startup_energy_remain_initial'] != csp.plant_state['pc_startup_energy_remain_initial']:
+        if (
+            csp.plant_state["pc_startup_energy_remain_initial"]
+            != csp.plant_state["pc_startup_energy_remain_initial"]
+        ):
             self.initial_cycle_startup_inventory = self.cycle_required_startup_energy
         else:
-            self.initial_cycle_startup_inventory = max(0.0, self.cycle_required_startup_energy
-                                                       - csp.plant_state['pc_startup_energy_remain_initial'] / 1e3)
-            if self.initial_cycle_startup_inventory > (1.0 - 1.e-6) * self.cycle_required_startup_energy:
-                self.initial_cycle_startup_inventory = self.cycle_required_startup_energy
-
-        self.is_cycle_generating_initial = (csp.plant_state['pc_op_mode_initial'] == 1)
-        self.is_cycle_starting_initial = (csp.plant_state['pc_op_mode_initial'] == 0
-                                          or csp.plant_state['pc_op_mode_initial'] == 4)
+            self.initial_cycle_startup_inventory = max(
+                0.0,
+                self.cycle_required_startup_energy
+                - csp.plant_state["pc_startup_energy_remain_initial"] / 1e3,
+            )
+            if (
+                self.initial_cycle_startup_inventory
+                > (1.0 - 1.0e-6) * self.cycle_required_startup_energy
+            ):
+                self.initial_cycle_startup_inventory = (
+                    self.cycle_required_startup_energy
+                )
+
+        self.is_cycle_generating_initial = csp.plant_state["pc_op_mode_initial"] == 1
+        self.is_cycle_starting_initial = (
+            csp.plant_state["pc_op_mode_initial"] == 0
+            or csp.plant_state["pc_op_mode_initial"] == 4
+        )
         # self.ycsb0 = (plant.state['pc_op_mode_initial'] == 2)
 
         if self.is_cycle_generating_initial:
-            self.initial_cycle_thermal_power = csp.plant_state['heat_into_cycle']
+            self.initial_cycle_thermal_power = csp.plant_state["heat_into_cycle"]
         else:
             self.initial_cycle_thermal_power = 0.0
 
     @staticmethod
     def get_start_end_datetime(start_time: int, n_horizon: int):
+        """Get start and end datetimes based on simulation start time and horizon length.
+
+        Args:
+            start_time (int): Start time of the simulation in hours.
+            n_horizon (int): Length of the simulation horizon in hours.
+
+        Returns:
+            tuple: A tuple containing the start and end datetime objects.
+
+        Notes:
+            This method calculates the start and end datetimes based on the provided start time
+            and horizon length, assuming hourly data.
+
+        """
         # Setting simulation times
         start_datetime = CspDispatch.get_start_datetime_by_hour(start_time)
         # Handling end of simulation horizon -> assumes hourly data
         if start_time + n_horizon > 8760:
             end_datetime = start_datetime + datetime.timedelta(hours=8760 - start_time)
         else:
             end_datetime = start_datetime + datetime.timedelta(hours=n_horizon)
         return start_datetime, end_datetime
 
     @staticmethod
     def get_start_datetime_by_hour(start_time: int):
-        """
-        Get datetime for start_time hour of the year
-        : param start_time: hour of year
-        : return: datetime object
+        """Get the datetime object corresponding to the start time of year in hours.
+
+        Args:
+            start_time (int): Start time of the simulation in hours.
+
+        Returns:
+            datetime.datetime: Datetime object corresponding to the start time.
+
+        Notes:
+            This method calculates the datetime object corresponding to the start time
+            in hours relative to the beginning of the year.
+            
         """
         # TODO: bring in the correct year from site data - or replace outside of function?
         beginning_of_year = datetime.datetime(2009, 1, 1, 0)
         return beginning_of_year + datetime.timedelta(hours=start_time)
 
     @staticmethod
     def seconds_since_newyear(dt):
+        """Get the number of seconds elapsed since the beginning of the year.
+
+        Args:
+            dt (datetime.datetime): Datetime object.
+
+        Returns:
+            int: Number of seconds elapsed since the beginning of the year.
+
+        Notes:
+            This method calculates the number of seconds elapsed since the beginning of the year,
+            using a non-leap year (2009) for consistency with a multiple of 8760 hours assumption.
+
+        """
         # Substitute a non-leap year (2009) to keep multiple of 8760 assumption:
         newyear = datetime.datetime(2009, 1, 1, 0, 0, 0, 0)
         time_diff = dt - newyear
         return int(time_diff.total_seconds())
 
-
     #################################
     # INPUTS                        #
     #################################
     @property
     def time_duration(self) -> list:
         """Dispatch horizon time steps [hour]"""
         # TODO: Should we make this constant within dispatch horizon?
         return [self.blocks[t].time_duration.value for t in self.blocks.index_set()]
 
     @time_duration.setter
     def time_duration(self, time_duration: list):
-        """Dispatch horizon time steps [hour]"""
         if len(time_duration) == len(self.blocks):
             for t, delta in zip(self.blocks, time_duration):
                 self.blocks[t].time_duration = round(delta, self.round_digits)
         else:
-            raise ValueError(self.time_duration.__name__ + " list must be the same length as time horizon")
+            raise ValueError(
+                self.time_duration.__name__
+                + " list must be the same length as time horizon"
+            )
 
     @property
     def available_thermal_generation(self) -> list:
         """Available solar thermal generation from the csp field [MWt]"""
-        return [self.blocks[t].available_thermal_generation.value for t in self.blocks.index_set()]
+        return [
+            self.blocks[t].available_thermal_generation.value
+            for t in self.blocks.index_set()
+        ]
 
     @available_thermal_generation.setter
     def available_thermal_generation(self, available_thermal_generation: list):
-        """Available solar thermal generation from the csp field [MWt]"""
         if len(available_thermal_generation) == len(self.blocks):
             for t, value in zip(self.blocks, available_thermal_generation):
-                self.blocks[t].available_thermal_generation = round(value, self.round_digits)
+                self.blocks[t].available_thermal_generation = round(
+                    value, self.round_digits
+                )
         else:
-            raise ValueError(self.available_thermal_generation.__name__ + " list must be the same length as time horizon")
+            raise ValueError(
+                self.available_thermal_generation.__name__
+                + " list must be the same length as time horizon"
+            )
 
     @property
     def cycle_ambient_efficiency_correction(self) -> list:
         """Cycle efficiency ambient temperature adjustment factor [-]"""
-        return [self.blocks[t].cycle_ambient_efficiency_correction.value for t in self.blocks.index_set()]
+        return [
+            self.blocks[t].cycle_ambient_efficiency_correction.value
+            for t in self.blocks.index_set()
+        ]
 
     @cycle_ambient_efficiency_correction.setter
-    def cycle_ambient_efficiency_correction(self, cycle_ambient_efficiency_correction: list):
-        """Cycle efficiency ambient temperature adjustment factor [-]"""
+    def cycle_ambient_efficiency_correction(
+        self, cycle_ambient_efficiency_correction: list
+    ):
         if len(cycle_ambient_efficiency_correction) == len(self.blocks):
             for t, value in zip(self.blocks, cycle_ambient_efficiency_correction):
-                self.blocks[t].cycle_ambient_efficiency_correction = round(value, self.round_digits)
+                self.blocks[t].cycle_ambient_efficiency_correction = round(
+                    value, self.round_digits
+                )
         else:
-            raise ValueError(self.cycle_ambient_efficiency_correction.__name__ + " list must be the same length as time horizon")
+            raise ValueError(
+                self.cycle_ambient_efficiency_correction.__name__
+                + " list must be the same length as time horizon"
+            )
 
     @property
     def condenser_losses(self) -> list:
         """Normalized condenser parasitic losses [-]"""
         return [self.blocks[t].condenser_losses.value for t in self.blocks.index_set()]
 
     @condenser_losses.setter
     def condenser_losses(self, condenser_losses: list):
-        """Normalized condenser parasitic losses [-]"""
         if len(condenser_losses) == len(self.blocks):
             for t, value in zip(self.blocks, condenser_losses):
                 self.blocks[t].condenser_losses = round(value, self.round_digits)
         else:
-            raise ValueError(self.condenser_losses.__name__ + " list must be the same length as time horizon")
+            raise ValueError(
+                self.condenser_losses.__name__
+                + " list must be the same length as time horizon"
+            )
 
     @property
     def receiver_startup_fraction(self) -> list:
         """Estimated fraction of time period required for receiver start-up [-]"""
-        return [self.blocks[t].receiver_startup_fraction.value for t in self.blocks.index_set()]
+        return [
+            self.blocks[t].receiver_startup_fraction.value
+            for t in self.blocks.index_set()
+        ]
 
     @receiver_startup_fraction.setter
     def receiver_startup_fraction(self, receiver_startup_fraction: list):
-        """Estimated fraction of time period required for receiver start-up [-]"""
         if len(receiver_startup_fraction) == len(self.blocks):
             for t, value in zip(self.blocks, receiver_startup_fraction):
-                self.blocks[t].receiver_startup_fraction = round(value, self.round_digits)
+                self.blocks[t].receiver_startup_fraction = round(
+                    value, self.round_digits
+                )
         else:
-            raise ValueError(self.receiver_startup_fraction.__name__ + " list must be the same length as time horizon")
+            raise ValueError(
+                self.receiver_startup_fraction.__name__
+                + " list must be the same length as time horizon"
+            )
 
     @property
     def min_receiver_start_time(self) -> float:
         """Minimum time to start the receiver [hr]"""
         for t in self.blocks.index_set():
             return self.blocks[t].min_receiver_start_time.value
 
     @min_receiver_start_time.setter
     def min_receiver_start_time(self, min_receiver_start_time_hr: float):
-        """Minimum time to start the receiver [hr]"""
         for t in self.blocks.index_set():
-            self.blocks[t].min_receiver_start_time.set_value(round(min_receiver_start_time_hr, self.round_digits))
+            self.blocks[t].min_receiver_start_time.set_value(
+                round(min_receiver_start_time_hr, self.round_digits)
+            )
 
     @property
     def cost_per_field_generation(self) -> float:
         """Generation cost for the csp field [$/MWht]"""
         for t in self.blocks.index_set():
             return self.blocks[t].cost_per_field_generation.value
 
     @cost_per_field_generation.setter
     def cost_per_field_generation(self, om_dollar_per_mwh_thermal: float):
-        """Generation cost for the csp field [$/MWht]"""
         for t in self.blocks.index_set():
-            self.blocks[t].cost_per_field_generation.set_value(round(om_dollar_per_mwh_thermal, self.round_digits))
+            self.blocks[t].cost_per_field_generation.set_value(
+                round(om_dollar_per_mwh_thermal, self.round_digits)
+            )
 
     @property
     def cost_per_field_start(self) -> float:
         """Penalty for field start-up [$/start]"""
         for t in self.blocks.index_set():
             return self.blocks[t].cost_per_field_start.value
 
     @cost_per_field_start.setter
     def cost_per_field_start(self, dollars_per_start: float):
-        """Penalty for field start-up [$/start]"""
         for t in self.blocks.index_set():
-            self.blocks[t].cost_per_field_start.set_value(round(dollars_per_start, self.round_digits))
+            self.blocks[t].cost_per_field_start.set_value(
+                round(dollars_per_start, self.round_digits)
+            )
 
     @property
     def cost_per_cycle_generation(self) -> float:
         """Generation cost for power cycle [$/MWhe]"""
         for t in self.blocks.index_set():
             return self.blocks[t].cost_per_cycle_generation.value
 
     @cost_per_cycle_generation.setter
     def cost_per_cycle_generation(self, om_dollar_per_mwh_electric: float):
-        """Generation cost for power cycle [$/MWhe]"""
         for t in self.blocks.index_set():
-            self.blocks[t].cost_per_cycle_generation.set_value(round(om_dollar_per_mwh_electric, self.round_digits))
+            self.blocks[t].cost_per_cycle_generation.set_value(
+                round(om_dollar_per_mwh_electric, self.round_digits)
+            )
 
     @property
     def cost_per_cycle_start(self) -> float:
         """Penalty for power cycle start [$/start]"""
         for t in self.blocks.index_set():
             return self.blocks[t].cost_per_cycle_start.value
 
     @cost_per_cycle_start.setter
     def cost_per_cycle_start(self, dollars_per_start: float):
-        """Penalty for power cycle start [$/start]"""
         for t in self.blocks.index_set():
-            self.blocks[t].cost_per_cycle_start.set_value(round(dollars_per_start, self.round_digits))
+            self.blocks[t].cost_per_cycle_start.set_value(
+                round(dollars_per_start, self.round_digits)
+            )
 
     @property
     def cost_per_change_thermal_input(self) -> float:
         """Penalty for change in power cycle thermal input [$/MWt]"""
         for t in self.blocks.index_set():
             return self.blocks[t].cost_per_change_thermal_input.value
 
     @cost_per_change_thermal_input.setter
     def cost_per_change_thermal_input(self, dollars_per_thermal_power: float):
-        """Penalty for change in power cycle thermal input [$/MWt]"""
         for t in self.blocks.index_set():
-            self.blocks[t].cost_per_change_thermal_input.set_value(round(dollars_per_thermal_power, self.round_digits))
+            self.blocks[t].cost_per_change_thermal_input.set_value(
+                round(dollars_per_thermal_power, self.round_digits)
+            )
 
     @property
     def field_startup_losses(self) -> float:
         """Solar field startup or shutdown parasitic loss [MWhe]"""
         for t in self.blocks.index_set():
             return self.blocks[t].field_startup_losses.value
 
     @field_startup_losses.setter
     def field_startup_losses(self, field_startup_losses: float):
-        """Solar field startup or shutdown parasitic loss [MWhe]"""
         for t in self.blocks.index_set():
-            self.blocks[t].field_startup_losses.set_value(round(field_startup_losses, self.round_digits))
+            self.blocks[t].field_startup_losses.set_value(
+                round(field_startup_losses, self.round_digits)
+            )
 
     @property
     def receiver_required_startup_energy(self) -> float:
         """Required energy expended to start receiver [MWht]"""
         for t in self.blocks.index_set():
             return self.blocks[t].receiver_required_startup_energy.value
 
     @receiver_required_startup_energy.setter
     def receiver_required_startup_energy(self, energy: float):
-        """Required energy expended to start receiver [MWht]"""
         for t in self.blocks.index_set():
-            self.blocks[t].receiver_required_startup_energy.set_value(round(energy, self.round_digits))
+            self.blocks[t].receiver_required_startup_energy.set_value(
+                round(energy, self.round_digits)
+            )
 
     @property
     def storage_capacity(self) -> float:
         """Thermal energy storage capacity [MWht]"""
         for t in self.blocks.index_set():
             return self.blocks[t].storage_capacity.value
 
     @storage_capacity.setter
     def storage_capacity(self, energy: float):
-        """Thermal energy storage capacity [MWht]"""
         for t in self.blocks.index_set():
             self.blocks[t].storage_capacity.set_value(round(energy, self.round_digits))
 
     @property
     def receiver_pumping_losses(self) -> float:
         """Solar field and/or receiver pumping power per unit power produced [MWe/MWt]"""
         for t in self.blocks.index_set():
             return self.blocks[t].receiver_pumping_losses.value
 
     @receiver_pumping_losses.setter
     def receiver_pumping_losses(self, electric_per_thermal: float):
-        """Solar field and/or receiver pumping power per unit power produced [MWe/MWt]"""
         for t in self.blocks.index_set():
-            self.blocks[t].receiver_pumping_losses.set_value(round(electric_per_thermal, self.round_digits))
+            self.blocks[t].receiver_pumping_losses.set_value(
+                round(electric_per_thermal, self.round_digits)
+            )
 
     @property
     def minimum_receiver_power(self) -> float:
         """Minimum operational thermal power delivered by receiver [MWht]"""
         for t in self.blocks.index_set():
             return self.blocks[t].minimum_receiver_power.value
 
     @minimum_receiver_power.setter
     def minimum_receiver_power(self, thermal_power: float):
-        """Minimum operational thermal power delivered by receiver [MWt]"""
         for t in self.blocks.index_set():
-            self.blocks[t].minimum_receiver_power.set_value(round(thermal_power, self.round_digits))
+            self.blocks[t].minimum_receiver_power.set_value(
+                round(thermal_power, self.round_digits)
+            )
 
     @property
     def allowable_receiver_startup_power(self) -> float:
         """Allowable power per period for receiver start-up [MWt]"""
         for t in self.blocks.index_set():
             return self.blocks[t].allowable_receiver_startup_power.value
 
     @allowable_receiver_startup_power.setter
     def allowable_receiver_startup_power(self, thermal_power: float):
-        """Allowable power per period for receiver start-up [MWt]"""
         for t in self.blocks.index_set():
-            self.blocks[t].allowable_receiver_startup_power.set_value(round(thermal_power, self.round_digits))
+            self.blocks[t].allowable_receiver_startup_power.set_value(
+                round(thermal_power, self.round_digits)
+            )
 
     @property
     def field_track_losses(self) -> float:
         """Solar field tracking parasitic loss [MWe]"""
         for t in self.blocks.index_set():
             return self.blocks[t].field_track_losses.value
 
     @field_track_losses.setter
     def field_track_losses(self, electric_power: float):
-        """Solar field tracking parasitic loss [MWe]"""
         for t in self.blocks.index_set():
-            self.blocks[t].field_track_losses.set_value(round(electric_power, self.round_digits))
+            self.blocks[t].field_track_losses.set_value(
+                round(electric_power, self.round_digits)
+            )
 
     # @property
     # def heat_trace_losses(self) -> float:
     #     """Piping heat trace parasitic loss [MWe]"""
     #     for t in self.blocks.index_set():
     #         return self.blocks[t].heat_trace_losses.value
     #
@@ -1118,90 +1663,97 @@
     def cycle_required_startup_energy(self) -> float:
         """Required energy expended to start cycle [MWht]"""
         for t in self.blocks.index_set():
             return self.blocks[t].cycle_required_startup_energy.value
 
     @cycle_required_startup_energy.setter
     def cycle_required_startup_energy(self, thermal_energy: float):
-        """Required energy expended to start cycle [MWht]"""
         for t in self.blocks.index_set():
-            self.blocks[t].cycle_required_startup_energy.set_value(round(thermal_energy, self.round_digits))
+            self.blocks[t].cycle_required_startup_energy.set_value(
+                round(thermal_energy, self.round_digits)
+            )
 
     @property
     def cycle_nominal_efficiency(self) -> float:
         """Power cycle nominal efficiency [-]"""
         for t in self.blocks.index_set():
             return self.blocks[t].cycle_nominal_efficiency.value
 
     @cycle_nominal_efficiency.setter
     def cycle_nominal_efficiency(self, efficiency: float):
-        """Power cycle nominal efficiency [-]"""
         efficiency = self._check_efficiency_value(efficiency)
         for t in self.blocks.index_set():
-            self.blocks[t].cycle_nominal_efficiency.set_value(round(efficiency, self.round_digits))
+            self.blocks[t].cycle_nominal_efficiency.set_value(
+                round(efficiency, self.round_digits)
+            )
 
     @property
     def cycle_performance_slope(self) -> float:
         """Slope of linear approximation of power cycle performance curve [MWe/MWt]"""
         for t in self.blocks.index_set():
             return self.blocks[t].cycle_performance_slope.value
 
     @cycle_performance_slope.setter
     def cycle_performance_slope(self, slope: float):
-        """Slope of linear approximation of power cycle performance curve [MWe/MWt]"""
         for t in self.blocks.index_set():
-            self.blocks[t].cycle_performance_slope.set_value(round(slope, self.round_digits))
+            self.blocks[t].cycle_performance_slope.set_value(
+                round(slope, self.round_digits)
+            )
 
     @property
     def cycle_pumping_losses(self) -> float:
         """Cycle heat transfer fluid pumping power per unit energy expended [MWe/MWt]"""
         for t in self.blocks.index_set():
             return self.blocks[t].cycle_pumping_losses.value
 
     @cycle_pumping_losses.setter
     def cycle_pumping_losses(self, electric_per_thermal: float):
-        """Cycle heat transfer fluid pumping power per unit energy expended [MWe/MWt]"""
         for t in self.blocks.index_set():
-            self.blocks[t].cycle_pumping_losses.set_value(round(electric_per_thermal, self.round_digits))
+            self.blocks[t].cycle_pumping_losses.set_value(
+                round(electric_per_thermal, self.round_digits)
+            )
 
     @property
     def allowable_cycle_startup_power(self) -> float:
         """Allowable power per period for cycle start-up [MWt]"""
         for t in self.blocks.index_set():
             return self.blocks[t].allowable_cycle_startup_power.value
 
     @allowable_cycle_startup_power.setter
     def allowable_cycle_startup_power(self, thermal_power: float):
-        """Allowable power per period for cycle start-up [MWt]"""
         for t in self.blocks.index_set():
-            self.blocks[t].allowable_cycle_startup_power.set_value(round(thermal_power, self.round_digits))
+            self.blocks[t].allowable_cycle_startup_power.set_value(
+                round(thermal_power, self.round_digits)
+            )
 
     @property
     def minimum_cycle_thermal_power(self) -> float:
         """Minimum operational thermal power delivered to the power cycle [MWt]"""
         for t in self.blocks.index_set():
             return self.blocks[t].minimum_cycle_thermal_power.value
 
     @minimum_cycle_thermal_power.setter
     def minimum_cycle_thermal_power(self, thermal_power: float):
-        """Minimum operational thermal power delivered to the power cycle [MWt]"""
         for t in self.blocks.index_set():
-            self.blocks[t].minimum_cycle_thermal_power.set_value(round(thermal_power, self.round_digits))
+            self.blocks[t].minimum_cycle_thermal_power.set_value(
+                round(thermal_power, self.round_digits)
+            )
 
     @property
     def maximum_cycle_thermal_power(self) -> float:
         """Maximum operational thermal power delivered to the power cycle [MWt]"""
         for t in self.blocks.index_set():
             return self.blocks[t].maximum_cycle_thermal_power.value
 
     @maximum_cycle_thermal_power.setter
     def maximum_cycle_thermal_power(self, thermal_power: float):
-        """Maximum operational thermal power delivered to the power cycle [MWt]"""
         for t in self.blocks.index_set():
-            self.blocks[t].maximum_cycle_thermal_power.set_value(round(thermal_power, self.round_digits))
+            self.blocks[t].maximum_cycle_thermal_power.set_value(
+                round(thermal_power, self.round_digits)
+            )
 
     # @property
     # def minimum_cycle_power(self) -> float:
     #     """Minimum cycle electric power output [MWe]"""
     #     for t in self.blocks.index_set():
     #         return self.blocks[t].minimum_cycle_power.value
     #
@@ -1215,170 +1767,212 @@
     def maximum_cycle_power(self) -> float:
         """Maximum cycle electric power output [MWe]"""
         for t in self.blocks.index_set():
             return self.blocks[t].maximum_cycle_power.value
 
     @maximum_cycle_power.setter
     def maximum_cycle_power(self, electric_power: float):
-        """Maximum cycle electric power output [MWe]"""
         for t in self.blocks.index_set():
-            self.blocks[t].maximum_cycle_power.set_value(round(electric_power, self.round_digits))
+            self.blocks[t].maximum_cycle_power.set_value(
+                round(electric_power, self.round_digits)
+            )
 
     # INITIAL CONDITIONS
     @property
     def initial_thermal_energy_storage(self) -> float:
         """Initial thermal energy storage reserve quantity at beginning of the horizon [MWht]"""
         return self.model.initial_thermal_energy_storage.value
 
     @initial_thermal_energy_storage.setter
     def initial_thermal_energy_storage(self, initial_energy: float):
-        """Initial thermal energy storage reserve quantity at beginning of the horizon [MWht]"""
-        self.model.initial_thermal_energy_storage = round(initial_energy, self.round_digits)
+        self.model.initial_thermal_energy_storage = round(
+            initial_energy, self.round_digits
+        )
 
     @property
     def initial_receiver_startup_inventory(self) -> float:
         """Initial receiver start-up energy inventory at beginning of the horizon [MWht]"""
         return self.model.initial_receiver_startup_inventory.value
 
     @initial_receiver_startup_inventory.setter
     def initial_receiver_startup_inventory(self, initial_energy: float):
-        """Initial receiver start-up energy inventory at beginning of the horizon [MWht]"""
-        self.model.initial_receiver_startup_inventory = round(initial_energy, self.round_digits)
+        self.model.initial_receiver_startup_inventory = round(
+            initial_energy, self.round_digits
+        )
 
     @property
     def is_field_generating_initial(self) -> bool:
         """True (1) if solar field is generating 'usable' thermal power at beginning of the horizon;
-         False (0) Otherwise [-]"""
+        False (0) Otherwise [-]"""
         return bool(self.model.is_field_generating_initial.value)
 
     @is_field_generating_initial.setter
     def is_field_generating_initial(self, is_field_generating: Union[bool, int]):
-        """True (1) if solar field is generating 'usable' thermal power at beginning of the horizon;
-         False (0) Otherwise [-]"""
         self.model.is_field_generating_initial = int(is_field_generating)
 
     @property
     def is_field_starting_initial(self) -> bool:
         """True (1) if solar field  is starting up at beginning of the horizon; False (0) Otherwise [-]"""
         return bool(self.model.is_field_starting_initial.value)
 
     @is_field_starting_initial.setter
     def is_field_starting_initial(self, is_field_starting: Union[bool, int]):
-        """True (1) if solar field  is starting up at beginning of the horizon; False (0) Otherwise [-]"""
         self.model.is_field_starting_initial = int(is_field_starting)
 
     @property
     def initial_cycle_startup_inventory(self) -> float:
         """Initial cycle start-up energy inventory at beginning of the horizon [MWht]"""
         return self.model.initial_cycle_startup_inventory.value
 
     @initial_cycle_startup_inventory.setter
     def initial_cycle_startup_inventory(self, initial_energy: float):
-        """Initial cycle start-up energy inventory at beginning of the horizon [MWht]"""
-        self.model.initial_cycle_startup_inventory = round(initial_energy, self.round_digits)
+        self.model.initial_cycle_startup_inventory = round(
+            initial_energy, self.round_digits
+        )
 
     @property
     def initial_cycle_thermal_power(self) -> float:
         """Initial cycle thermal power at beginning of the horizon [MWt]"""
         return self.model.initial_cycle_thermal_power.value
 
     @initial_cycle_thermal_power.setter
     def initial_cycle_thermal_power(self, initial_power: float):
-        """Initial cycle thermal power at beginning of the horizon [MWt]"""
         self.model.initial_cycle_thermal_power = round(initial_power, self.round_digits)
 
     @property
     def is_cycle_generating_initial(self) -> bool:
         """True (1) if cycle is generating electric power at beginning of the horizon; False (0) Otherwise [-]"""
         return bool(self.model.is_cycle_generating_initial.value)
 
     @is_cycle_generating_initial.setter
     def is_cycle_generating_initial(self, is_cycle_generating: Union[bool, int]):
-        """True (1) if cycle is generating electric power at beginning of the horizon; False (0) Otherwise [-]"""
         self.model.is_cycle_generating_initial = int(is_cycle_generating)
 
     @property
     def is_cycle_starting_initial(self) -> bool:
         """True (1) if cycle is starting up at beginning of the horizon; False (0) Otherwise [-]"""
         return bool(self.model.is_cycle_starting_initial.value)
 
     @is_cycle_starting_initial.setter
     def is_cycle_starting_initial(self, is_cycle_starting: Union[bool, int]):
-        """True (1) if cycle is starting up at beginning of the horizon; False (0) Otherwise [-]"""
         self.model.is_cycle_starting_initial = int(is_cycle_starting)
 
     # OUTPUTS
     @property
     def thermal_energy_storage(self) -> list:
         """Thermal energy storage reserve quantity [MWht]"""
-        return [round(self.blocks[t].thermal_energy_storage.value, self.round_digits) for t in self.blocks.index_set()]
+        return [
+            round(self.blocks[t].thermal_energy_storage.value, self.round_digits)
+            for t in self.blocks.index_set()
+        ]
 
     @property
     def receiver_startup_inventory(self) -> list:
         """Receiver start-up energy inventory [MWht]"""
-        return [round(self.blocks[t].receiver_startup_inventory.value, self.round_digits) for t in self.blocks.index_set()]
+        return [
+            round(self.blocks[t].receiver_startup_inventory.value, self.round_digits)
+            for t in self.blocks.index_set()
+        ]
 
     @property
     def receiver_thermal_power(self) -> list:
         """Thermal power delivered by the receiver [MWt]"""
-        return [round(self.blocks[t].receiver_thermal_power.value, self.round_digits) for t in self.blocks.index_set()]
+        return [
+            round(self.blocks[t].receiver_thermal_power.value, self.round_digits)
+            for t in self.blocks.index_set()
+        ]
 
     @property
     def receiver_startup_consumption(self) -> list:
         """Receiver start-up power consumption [MWt]"""
-        return [round(self.blocks[t].receiver_startup_consumption.value, self.round_digits) for t in self.blocks.index_set()]
+        return [
+            round(self.blocks[t].receiver_startup_consumption.value, self.round_digits)
+            for t in self.blocks.index_set()
+        ]
 
     @property
     def is_field_generating(self) -> list:
         """1 if solar field is generating 'usable' thermal power; 0 Otherwise [-]"""
-        return [round(self.blocks[t].is_field_generating.value, self.round_digits) for t in self.blocks.index_set()]
+        return [
+            round(self.blocks[t].is_field_generating.value, self.round_digits)
+            for t in self.blocks.index_set()
+        ]
 
     @property
     def is_field_starting(self) -> list:
         """1 if solar field is starting up; 0 Otherwise [-]"""
-        return [round(self.blocks[t].is_field_starting.value, self.round_digits) for t in self.blocks.index_set()]
+        return [
+            round(self.blocks[t].is_field_starting.value, self.round_digits)
+            for t in self.blocks.index_set()
+        ]
 
     @property
     def incur_field_start(self) -> list:
         """1 if solar field start-up penalty is incurred; 0 Otherwise [-]"""
-        return [round(self.blocks[t].incur_field_start.value, self.round_digits) for t in self.blocks.index_set()]
+        return [
+            round(self.blocks[t].incur_field_start.value, self.round_digits)
+            for t in self.blocks.index_set()
+        ]
 
     @property
     def cycle_startup_inventory(self) -> list:
         """Cycle start-up energy inventory [MWht]"""
-        return [round(self.blocks[t].cycle_startup_inventory.value, self.round_digits) for t in self.blocks.index_set()]
+        return [
+            round(self.blocks[t].cycle_startup_inventory.value, self.round_digits)
+            for t in self.blocks.index_set()
+        ]
 
     @property
     def system_load(self) -> list:
         """Net generation of csp system [MWe]"""
-        return [round(self.blocks[t].system_load.value, self.round_digits) for t in self.blocks.index_set()]
+        return [
+            round(self.blocks[t].system_load.value, self.round_digits)
+            for t in self.blocks.index_set()
+        ]
 
     @property
     def cycle_generation(self) -> list:
         """Power cycle electricity generation [MWe]"""
-        return [round(self.blocks[t].cycle_generation.value, self.round_digits) for t in self.blocks.index_set()]
+        return [
+            round(self.blocks[t].cycle_generation.value, self.round_digits)
+            for t in self.blocks.index_set()
+        ]
 
     @property
     def cycle_thermal_ramp(self) -> list:
         """Power cycle positive change in thermal energy input [MWt]"""
-        return [round(self.blocks[t].cycle_thermal_ramp.value, self.round_digits) for t in self.blocks.index_set()]
+        return [
+            round(self.blocks[t].cycle_thermal_ramp.value, self.round_digits)
+            for t in self.blocks.index_set()
+        ]
 
     @property
     def cycle_thermal_power(self) -> list:
         """Cycle thermal power utilization [MWt]"""
-        return [round(self.blocks[t].cycle_thermal_power.value, self.round_digits) for t in self.blocks.index_set()]
+        return [
+            round(self.blocks[t].cycle_thermal_power.value, self.round_digits)
+            for t in self.blocks.index_set()
+        ]
 
     @property
     def is_cycle_generating(self) -> list:
         """1 if cycle is generating electric power; 0 Otherwise [-]"""
-        return [round(self.blocks[t].is_cycle_generating.value, self.round_digits) for t in self.blocks.index_set()]
+        return [
+            round(self.blocks[t].is_cycle_generating.value, self.round_digits)
+            for t in self.blocks.index_set()
+        ]
 
     @property
     def is_cycle_starting(self) -> list:
         """1 if cycle is starting up; 0 Otherwise [-]"""
-        return [round(self.blocks[t].is_cycle_starting.value, self.round_digits) for t in self.blocks.index_set()]
+        return [
+            round(self.blocks[t].is_cycle_starting.value, self.round_digits)
+            for t in self.blocks.index_set()
+        ]
 
     @property
     def incur_cycle_start(self) -> list:
         """1 if cycle start-up penalty is incurred; 0 Otherwise [-]"""
-        return [round(self.blocks[t].incur_cycle_start.value, self.round_digits) for t in self.blocks.index_set()]
-
+        return [
+            round(self.blocks[t].incur_cycle_start.value, self.round_digits)
+            for t in self.blocks.index_set()
+        ]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/dispatch/power_storage/linear_voltage_convex_battery_dispatch.py` & `HOPP-2.2.0/hopp/simulation/technologies/dispatch/power_storage/linear_voltage_convex_battery_dispatch.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,186 +1,329 @@
 import pyomo.environ as pyomo
 from pyomo.environ import units as u
 
 import PySAM.BatteryStateful as BatteryModel
 import PySAM.Singleowner as Singleowner
 
-from hopp.simulation.technologies.dispatch.power_storage.linear_voltage_nonconvex_battery_dispatch import NonConvexLinearVoltageBatteryDispatch
+from hopp.simulation.technologies.dispatch.power_storage.linear_voltage_nonconvex_battery_dispatch import (
+    NonConvexLinearVoltageBatteryDispatch,
+)
 
 
 class ConvexLinearVoltageBatteryDispatch(NonConvexLinearVoltageBatteryDispatch):
+    """This class represents a convex linear voltage battery dispatch model.
+
+    It extends the NonConvexLinearVoltageBatteryDispatch model and adds additional formulation to enforce convexity.
+
     """
-    
-    """
+
     # TODO: add a reference to original paper
 
-    def __init__(self,
-                 pyomo_model: pyomo.ConcreteModel,
-                 index_set: pyomo.Set,
-                 system_model: BatteryModel.BatteryStateful,
-                 financial_model: Singleowner.Singleowner,
-                 block_set_name: str = 'convex_LV_battery',
-                 dispatch_options: dict = None,
-                 use_exp_voltage_point: bool = False):
+    def __init__(
+        self,
+        pyomo_model: pyomo.ConcreteModel,
+        index_set: pyomo.Set,
+        system_model: BatteryModel.BatteryStateful,
+        financial_model: Singleowner.Singleowner,
+        block_set_name: str = "convex_LV_battery",
+        dispatch_options: dict = None,
+        use_exp_voltage_point: bool = False,
+    ):
+        """Initialize ConvexLinearVoltageBatteryDispatch.
+
+        Args:
+            pyomo_model (pyomo.ConcreteModel): Pyomo concrete model.
+            index_set (pyomo.Set): Indexed set.
+            system_model (BatteryModel.BatteryStateful): Battery system model.
+            financial_model (Singleowner.Singleowner): Financial model.
+            block_set_name (str, optional): Name of the block set. Defaults to 'convex_LV_battery'.
+            dispatch_options (dict, optional): Dispatch options. Defaults to None.
+            use_exp_voltage_point (bool, optional): Boolean indicating whether to use the exponential voltage point. Defaults to False.
+
+        """
         if dispatch_options is None:
             dispatch_options = {}
-        super().__init__(pyomo_model,
-                         index_set,
-                         system_model,
-                         financial_model,
-                         block_set_name=block_set_name,
-                         dispatch_options=dispatch_options,
-                         use_exp_voltage_point=use_exp_voltage_point)
+        super().__init__(
+            pyomo_model,
+            index_set,
+            system_model,
+            financial_model,
+            block_set_name=block_set_name,
+            dispatch_options=dispatch_options,
+            use_exp_voltage_point=use_exp_voltage_point,
+        )
 
     def dispatch_block_rule(self, battery):
+        """Additional formulation for dispatch block rule.
+
+        Args:
+            battery: Battery instance.
+
+        """
         # Additional formulation
         # Variables
         self._create_lv_battery_auxiliary_variables(battery)
         super().dispatch_block_rule(battery)
 
     @staticmethod
     def _create_lv_battery_auxiliary_variables(battery):
+        """Create auxiliary variables for the battery model.
+
+        Args:
+            battery: Battery instance.
+
+        """
         # Auxiliary Variables
         battery.aux_charge_current_soc = pyomo.Var(
             doc="Auxiliary bi-linear term equal to the product of charge current and previous state-of-charge [MA]",
             domain=pyomo.NonNegativeReals,
-            units=u.MA)  # = charge_current[t] * soc[t-1]
+            units=u.MA,
+        )  # = charge_current[t] * soc[t-1]
         battery.aux_charge_current_is_charging = pyomo.Var(
             doc="Auxiliary bi-linear term equal to the product of charge current and charging binary [MA]",
             domain=pyomo.NonNegativeReals,
-            units=u.MA)  # = charge_current[t] * is_charging[t]
+            units=u.MA,
+        )  # = charge_current[t] * is_charging[t]
         battery.aux_discharge_current_soc = pyomo.Var(
             doc="Auxiliary bi-linear equal to the product of discharge current and previous state-of-charge [MA]",
             domain=pyomo.NonNegativeReals,
-            units=u.MA)  # = discharge_current[t] * soc[t-1]
+            units=u.MA,
+        )  # = discharge_current[t] * soc[t-1]
         battery.aux_discharge_current_is_discharging = pyomo.Var(
             doc="Auxiliary bi-linear term equal to the product of discharge current and discharging binary [MA]",
             domain=pyomo.NonNegativeReals,
-            units=u.MA)  # = discharge_current[t] * is_discharging[t]
+            units=u.MA,
+        )  # = discharge_current[t] * is_discharging[t]
 
     @staticmethod
     def _create_lv_battery_power_equation_constraints(battery):
+        """Create power equation constraints for the battery model.
+
+        Args:
+            battery: Battery instance.
+
+        """
         battery.charge_power_equation = pyomo.Constraint(
             doc="Battery charge power equation equal to the product of current and voltage",
-            expr=battery.charge_power == (battery.voltage_slope * battery.aux_charge_current_soc
-                                          + (battery.voltage_intercept
-                                             + battery.average_current * battery.internal_resistance
-                                             ) * battery.aux_charge_current_is_charging))
+            expr=battery.charge_power
+            == (
+                battery.voltage_slope * battery.aux_charge_current_soc
+                + (
+                    battery.voltage_intercept
+                    + battery.average_current * battery.internal_resistance
+                )
+                * battery.aux_charge_current_is_charging
+            ),
+        )
         battery.discharge_power_equation = pyomo.Constraint(
             doc="Battery discharge power equation equal to the product of current and voltage",
-            expr=battery.discharge_power == (battery.voltage_slope * battery.aux_discharge_current_soc
-                                             + (battery.voltage_intercept
-                                                - battery.average_current * battery.internal_resistance
-                                                ) * battery.aux_discharge_current_is_discharging))
+            expr=battery.discharge_power
+            == (
+                battery.voltage_slope * battery.aux_discharge_current_soc
+                + (
+                    battery.voltage_intercept
+                    - battery.average_current * battery.internal_resistance
+                )
+                * battery.aux_discharge_current_is_discharging
+            ),
+        )
         # Auxiliary Variable bounds (binary*continuous exact linearization)
         # Charge current * charging binary
         battery.aux_charge_lb = pyomo.Constraint(
             doc="Charge current * charge binary lower bound",
-            expr=battery.aux_charge_current_is_charging >= battery.minimum_charge_current * battery.is_charging)
+            expr=battery.aux_charge_current_is_charging
+            >= battery.minimum_charge_current * battery.is_charging,
+        )
         battery.aux_charge_ub = pyomo.Constraint(
             doc="Charge current * charge binary upper bound",
-            expr=battery.aux_charge_current_is_charging <= battery.maximum_charge_current * battery.is_charging)
+            expr=battery.aux_charge_current_is_charging
+            <= battery.maximum_charge_current * battery.is_charging,
+        )
         battery.aux_charge_diff_lb = pyomo.Constraint(
             doc="Charge current and auxiliary difference lower bound",
-            expr=(battery.charge_current - battery.aux_charge_current_is_charging
-                  >= - battery.maximum_charge_current * (1 - battery.is_charging)))
+            expr=(
+                battery.charge_current - battery.aux_charge_current_is_charging
+                >= -battery.maximum_charge_current * (1 - battery.is_charging)
+            ),
+        )
         battery.aux_charge_diff_ub = pyomo.Constraint(
             doc="Charge current and auxiliary difference upper bound",
-            expr=(battery.charge_current - battery.aux_charge_current_is_charging
-                  <= battery.maximum_charge_current * (1 - battery.is_charging)))
+            expr=(
+                battery.charge_current - battery.aux_charge_current_is_charging
+                <= battery.maximum_charge_current * (1 - battery.is_charging)
+            ),
+        )
         # Discharge current * discharging binary
         battery.aux_discharge_lb = pyomo.Constraint(
             doc="discharge current * discharge binary lower bound",
-            expr=(battery.aux_discharge_current_is_discharging
-                  >= battery.minimum_discharge_current * battery.is_discharging))
+            expr=(
+                battery.aux_discharge_current_is_discharging
+                >= battery.minimum_discharge_current * battery.is_discharging
+            ),
+        )
         battery.aux_discharge_ub = pyomo.Constraint(
             doc="discharge current * discharge binary upper bound",
-            expr=(battery.aux_discharge_current_is_discharging
-                  <= battery.maximum_discharge_current * battery.is_discharging))
+            expr=(
+                battery.aux_discharge_current_is_discharging
+                <= battery.maximum_discharge_current * battery.is_discharging
+            ),
+        )
         battery.aux_discharge_diff_lb = pyomo.Constraint(
             doc="discharge current and auxiliary difference lower bound",
-            expr=(battery.discharge_current - battery.aux_discharge_current_is_discharging
-                  >= - battery.maximum_discharge_current * (1 - battery.is_discharging)))
+            expr=(
+                battery.discharge_current - battery.aux_discharge_current_is_discharging
+                >= -battery.maximum_discharge_current * (1 - battery.is_discharging)
+            ),
+        )
         battery.aux_discharge_diff_ub = pyomo.Constraint(
             doc="discharge current and auxiliary difference upper bound",
-            expr=(battery.discharge_current - battery.aux_discharge_current_is_discharging
-                  <= battery.maximum_discharge_current * (1 - battery.is_discharging)))
+            expr=(
+                battery.discharge_current - battery.aux_discharge_current_is_discharging
+                <= battery.maximum_discharge_current * (1 - battery.is_discharging)
+            ),
+        )
         # Auxiliary Variable bounds (continuous*continuous approx. linearization)
         # TODO: The error in these constraints should be quantified
         # TODO: scaling the problem to between [0,1] might help
         battery.aux_charge_soc_lower1 = pyomo.Constraint(
             doc="McCormick envelope underestimate 1",
-            expr=battery.aux_charge_current_soc >= (battery.maximum_charge_current * battery.soc0
-                                                    + battery.maximum_soc * battery.charge_current
-                                                    - battery.maximum_soc * battery.maximum_charge_current))
+            expr=battery.aux_charge_current_soc
+            >= (
+                battery.maximum_charge_current * battery.soc0
+                + battery.maximum_soc * battery.charge_current
+                - battery.maximum_soc * battery.maximum_charge_current
+            ),
+        )
         battery.aux_charge_soc_lower2 = pyomo.Constraint(
             doc="McCormick envelope underestimate 2",
-            expr=battery.aux_charge_current_soc >= (battery.minimum_charge_current * battery.soc0
-                                                    + battery.minimum_soc * battery.charge_current
-                                                    - battery.minimum_soc * battery.minimum_charge_current))
+            expr=battery.aux_charge_current_soc
+            >= (
+                battery.minimum_charge_current * battery.soc0
+                + battery.minimum_soc * battery.charge_current
+                - battery.minimum_soc * battery.minimum_charge_current
+            ),
+        )
         battery.aux_charge_soc_upper1 = pyomo.Constraint(
             doc="McCormick envelope overestimate 1",
-            expr=battery.aux_charge_current_soc <= (battery.maximum_charge_current * battery.soc0
-                                                    + battery.minimum_soc * battery.charge_current
-                                                    - battery.minimum_soc * battery.maximum_charge_current))
+            expr=battery.aux_charge_current_soc
+            <= (
+                battery.maximum_charge_current * battery.soc0
+                + battery.minimum_soc * battery.charge_current
+                - battery.minimum_soc * battery.maximum_charge_current
+            ),
+        )
         battery.aux_charge_soc_upper2 = pyomo.Constraint(
             doc="McCormick envelope overestimate 2",
-            expr=battery.aux_charge_current_soc <= (battery.minimum_charge_current * battery.soc0
-                                                    + battery.maximum_soc * battery.charge_current
-                                                    - battery.maximum_soc * battery.minimum_charge_current))
+            expr=battery.aux_charge_current_soc
+            <= (
+                battery.minimum_charge_current * battery.soc0
+                + battery.maximum_soc * battery.charge_current
+                - battery.maximum_soc * battery.minimum_charge_current
+            ),
+        )
 
         battery.aux_discharge_soc_lower1 = pyomo.Constraint(
             doc="McCormick envelope underestimate 1",
-            expr=battery.aux_discharge_current_soc >= (battery.maximum_discharge_current * battery.soc0
-                                                       + battery.maximum_soc * battery.discharge_current
-                                                       - battery.maximum_soc * battery.maximum_discharge_current))
+            expr=battery.aux_discharge_current_soc
+            >= (
+                battery.maximum_discharge_current * battery.soc0
+                + battery.maximum_soc * battery.discharge_current
+                - battery.maximum_soc * battery.maximum_discharge_current
+            ),
+        )
         battery.aux_discharge_soc_lower2 = pyomo.Constraint(
             doc="McCormick envelope underestimate 2",
-            expr=battery.aux_discharge_current_soc >= (battery.minimum_discharge_current * battery.soc0
-                                                       + battery.minimum_soc * battery.discharge_current
-                                                       - battery.minimum_soc * battery.minimum_discharge_current))
+            expr=battery.aux_discharge_current_soc
+            >= (
+                battery.minimum_discharge_current * battery.soc0
+                + battery.minimum_soc * battery.discharge_current
+                - battery.minimum_soc * battery.minimum_discharge_current
+            ),
+        )
         battery.aux_discharge_soc_upper1 = pyomo.Constraint(
             doc="McCormick envelope overestimate 1",
-            expr=battery.aux_discharge_current_soc <= (battery.maximum_discharge_current * battery.soc0
-                                                       + battery.minimum_soc * battery.discharge_current
-                                                       - battery.minimum_soc * battery.maximum_discharge_current))
+            expr=battery.aux_discharge_current_soc
+            <= (
+                battery.maximum_discharge_current * battery.soc0
+                + battery.minimum_soc * battery.discharge_current
+                - battery.minimum_soc * battery.maximum_discharge_current
+            ),
+        )
         battery.aux_discharge_soc_upper2 = pyomo.Constraint(
             doc="McCormick envelope overestimate 2",
-            expr=battery.aux_discharge_current_soc <= (battery.minimum_discharge_current * battery.soc0
-                                                       + battery.maximum_soc * battery.discharge_current
-                                                       - battery.maximum_soc * battery.minimum_discharge_current))
+            expr=battery.aux_discharge_current_soc
+            <= (
+                battery.minimum_discharge_current * battery.soc0
+                + battery.maximum_soc * battery.discharge_current
+                - battery.maximum_soc * battery.minimum_discharge_current
+            ),
+        )
 
     def _lifecycle_count_rule(self, m, i):
+        """Lifecycle count rule.
+
+        Args:
+            m: Model instance.
+            i: Index.
+
+        """
         # current accounting
         # TODO: Check for cheating -> there seems to be a lot of error
         start = int(i * self.timesteps_per_day)
         end = int((i + 1) * self.timesteps_per_day)
-        return self.model.lifecycles[i] == sum(self.blocks[t].time_duration
-                                            * (0.8 * self.blocks[t].discharge_current
-                                               - 0.8 * self.blocks[t].aux_discharge_current_soc)
-                                            / self.blocks[t].capacity for t in range(start, end))
+        return self.model.lifecycles[i] == sum(
+            self.blocks[t].time_duration
+            * (
+                0.8 * self.blocks[t].discharge_current
+                - 0.8 * self.blocks[t].aux_discharge_current_soc
+            )
+            / self.blocks[t].capacity
+            for t in range(start, end)
+        )
 
     # Auxiliary Variables
     @property
     def aux_charge_current_soc(self) -> list:
-        return [self.blocks[t].aux_charge_current_soc.value for t in self.blocks.index_set()]
+        """List of auxiliary charge current state of charge."""
+        return [
+            self.blocks[t].aux_charge_current_soc.value for t in self.blocks.index_set()
+        ]
 
     @property
     def real_charge_current_soc(self) -> list:
-        return [self.blocks[t].charge_current.value * self.blocks[t].soc0.value for t in self.blocks.index_set()]
+        """List of real charge current state of charge."""
+        return [
+            self.blocks[t].charge_current.value * self.blocks[t].soc0.value
+            for t in self.blocks.index_set()
+        ]
 
     @property
     def aux_charge_current_is_charging(self) -> list:
-        return [self.blocks[t].aux_charge_current_is_charging.value for t in self.blocks.index_set()]
+        """List of auxiliary charge current charging status."""
+        return [
+            self.blocks[t].aux_charge_current_is_charging.value
+            for t in self.blocks.index_set()
+        ]
 
     @property
     def aux_discharge_current_soc(self) -> list:
-        return [self.blocks[t].aux_discharge_current_soc.value for t in self.blocks.index_set()]
+        """List of auxiliary discharge current state of charge."""
+        return [
+            self.blocks[t].aux_discharge_current_soc.value
+            for t in self.blocks.index_set()
+        ]
 
     @property
     def real_discharge_current_soc(self) -> list:
-        return [self.blocks[t].discharge_current.value * self.blocks[t].soc0.value for t in self.blocks.index_set()]
+        """List of real discharge current state of charge."""
+        return [
+            self.blocks[t].discharge_current.value * self.blocks[t].soc0.value
+            for t in self.blocks.index_set()
+        ]
 
     @property
     def aux_discharge_current_is_discharging(self) -> list:
-        return [self.blocks[t].aux_discharge_current_is_discharging.value for t in self.blocks.index_set()]
-
+        """List of auxiliary discharge current discharging status."""
+        return [
+            self.blocks[t].aux_discharge_current_is_discharging.value
+            for t in self.blocks.index_set()
+        ]
```

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/dispatch/power_storage/linear_voltage_nonconvex_battery_dispatch.py` & `HOPP-2.2.0/hopp/simulation/technologies/dispatch/power_storage/linear_voltage_nonconvex_battery_dispatch.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,200 +1,323 @@
 import pyomo.environ as pyomo
 from pyomo.environ import units as u
 
 import PySAM.BatteryStateful as BatteryModel
 import PySAM.Singleowner as Singleowner
 
-from hopp.simulation.technologies.dispatch.power_storage.simple_battery_dispatch import SimpleBatteryDispatch
+from hopp.simulation.technologies.dispatch.power_storage.simple_battery_dispatch import (
+    SimpleBatteryDispatch,
+)
 
 
 class NonConvexLinearVoltageBatteryDispatch(SimpleBatteryDispatch):
-    """
+    """This class represents a non-convex linear voltage battery dispatch model.
 
+    It extends the SimpleBatteryDispatch model and adds additional formulation to handle non-convex behavior.
+    
     """
+
     # TODO: add a reference to original paper
 
-    def __init__(self,
-                 pyomo_model: pyomo.ConcreteModel,
-                 index_set: pyomo.Set,
-                 system_model: BatteryModel.BatteryStateful,
-                 financial_model: Singleowner.Singleowner,
-                 block_set_name: str = 'LV_battery',
-                 dispatch_options: dict = None,
-                 use_exp_voltage_point: bool = False):
-        u.load_definitions_from_strings(['amp_hour = amp * hour = Ah = amphour'])
+    def __init__(
+        self,
+        pyomo_model: pyomo.ConcreteModel,
+        index_set: pyomo.Set,
+        system_model: BatteryModel.BatteryStateful,
+        financial_model: Singleowner.Singleowner,
+        block_set_name: str = "LV_battery",
+        dispatch_options: dict = None,
+        use_exp_voltage_point: bool = False,
+    ):
+        """Initialize NonConvexLinearVoltageBatteryDispatch.
+
+        Args:
+            pyomo_model (pyomo.ConcreteModel): Pyomo concrete model.
+            index_set (pyomo.Set): Indexed set.
+            system_model (BatteryModel.BatteryStateful): Battery system model.
+            financial_model (Singleowner.Singleowner): Financial model.
+            block_set_name (str, optional): Name of the block set. Defaults to 'LV_battery'.
+            dispatch_options (dict, optional): Dispatch options. Defaults to None.
+            use_exp_voltage_point (bool, optional): Boolean indicating whether to use the exponential voltage point. Defaults to False.
+
+        """
+        u.load_definitions_from_strings(["amp_hour = amp * hour = Ah = amphour"])
         if dispatch_options is None:
             dispatch_options = {}
-        super().__init__(pyomo_model,
-                         index_set,
-                         system_model,
-                         financial_model,
-                         block_set_name=block_set_name,
-                         dispatch_options=dispatch_options)
+        super().__init__(
+            pyomo_model,
+            index_set,
+            system_model,
+            financial_model,
+            block_set_name=block_set_name,
+            dispatch_options=dispatch_options,
+        )
         self.use_exp_voltage_point = use_exp_voltage_point
 
     def dispatch_block_rule(self, battery):
+        """Additional formulation for dispatch block rule.
+
+        Args:
+            battery: Battery instance.
+
+        """
         # Parameters
         self._create_lv_battery_parameters(battery)
         # Variables
         self._create_lv_battery_variables(battery)
         # Base storage dispatch (parameters, variables, and constraints)
         super().dispatch_block_rule(battery)
         # Constraints
         self._create_lv_battery_constraints(battery)
         self._create_lv_battery_power_equation_constraints(battery)
 
     def _create_efficiency_parameters(self, battery):
+        """Not defined in this formulation."""
         # Not defined in this formulation
         pass
 
     def _create_capacity_parameter(self, battery):
+        """Create capacity parameter for the battery model.
+
+        Args:
+            battery: Battery instance.
+
+        """
         battery.capacity = pyomo.Param(
             doc=self.block_set_name + " capacity [MAh]",
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.MAh)
+            units=u.MAh,
+        )
 
     def _create_lv_battery_parameters(self, battery):
+        """Create parameters for the battery model.
+
+        Args:
+            battery: Battery instance.
+
+        """
         battery.voltage_slope = pyomo.Param(
             doc=self.block_set_name + " linear voltage model slope coefficient [V]",
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.V)
+            units=u.V,
+        )
         battery.voltage_intercept = pyomo.Param(
             doc=self.block_set_name + " linear voltage model intercept coefficient [V]",
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.V)
+            units=u.V,
+        )
         # TODO: Add this if wanted
         # self.alphaP = Param(None)  # [kW_DC]    Bi-directional intercept for charge
         # self.betaP = Param(None)  # [-]         Bi-directional slope for charge
         # self.alphaN = Param(None)  # [kW_DC]    Bi-directional intercept for discharge
         # self.betaN = Param(None)  # [-]         Bi-directional slope for discharge
         battery.average_current = pyomo.Param(
             doc="Typical cell current for both charge and discharge [A]",
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.A)
+            units=u.A,
+        )
         battery.internal_resistance = pyomo.Param(
             doc=self.block_set_name + " internal resistance [Ohm]",
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.ohm)
+            units=u.ohm,
+        )
         battery.minimum_charge_current = pyomo.Param(
             doc=self.block_set_name + " minimum charge current [MA]",
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.MA)
+            units=u.MA,
+        )
         battery.maximum_charge_current = pyomo.Param(
             doc=self.block_set_name + " maximum charge current [MA]",
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.MA)
+            units=u.MA,
+        )
         battery.minimum_discharge_current = pyomo.Param(
             doc=self.block_set_name + " minimum discharge current [MA]",
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.MA)
+            units=u.MA,
+        )
         battery.maximum_discharge_current = pyomo.Param(
             doc=self.block_set_name + " maximum discharge current [MA]",
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.MA)
+            units=u.MA,
+        )
 
     @staticmethod
     def _create_lv_battery_variables(battery):
+        """Create variables for the battery model.
+
+        Args:
+            battery: Battery instance.
+
+        """
         battery.charge_current = pyomo.Var(
             doc="Current into the battery [MA]",
             domain=pyomo.NonNegativeReals,
-            units=u.MA)
+            units=u.MA,
+        )
         battery.discharge_current = pyomo.Var(
             doc="Current out of the battery [MA]",
             domain=pyomo.NonNegativeReals,
-            units=u.MA)
+            units=u.MA,
+        )
 
     def _create_soc_inventory_constraint(self, storage):
+        """Create state-of-charge inventory balance constraint.
+
+        Args:
+            battery: Battery instance.
+
+        """
+
         def soc_inventory_rule(m):
             # TODO: add alpha and beta terms
-            return m.soc == (m.soc0 + m.time_duration * (m.charge_current - m.discharge_current) / m.capacity)
+            return m.soc == (
+                m.soc0
+                + m.time_duration
+                * (m.charge_current - m.discharge_current)
+                / m.capacity
+            )
+
         # Storage State-of-charge balance
         storage.soc_inventory = pyomo.Constraint(
             doc=self.block_set_name + " state-of-charge inventory balance",
-            rule=soc_inventory_rule)
+            rule=soc_inventory_rule,
+        )
 
     @staticmethod
     def _create_lv_battery_constraints(battery):
+        """Create constraints for the battery model.
+
+        Args:
+            battery: Battery instance.
+
+        """
         # Charge current bounds
         battery.charge_current_lb = pyomo.Constraint(
             doc="Battery Charging current lower bound",
-            expr=battery.charge_current >= battery.minimum_charge_current * battery.is_charging)
+            expr=battery.charge_current
+            >= battery.minimum_charge_current * battery.is_charging,
+        )
         battery.charge_current_ub = pyomo.Constraint(
             doc="Battery Charging current upper bound",
-            expr=battery.charge_current <= battery.maximum_charge_current * battery.is_charging)
+            expr=battery.charge_current
+            <= battery.maximum_charge_current * battery.is_charging,
+        )
         battery.charge_current_ub_soc = pyomo.Constraint(
             doc="Battery Charging current upper bound state-of-charge dependence",
-            expr=battery.charge_current <= battery.capacity * (1.0 - battery.soc0) / battery.time_duration)
+            expr=battery.charge_current
+            <= battery.capacity * (1.0 - battery.soc0) / battery.time_duration,
+        )
         # Discharge current bounds
         battery.discharge_current_lb = pyomo.Constraint(
             doc="Battery Discharging current lower bound",
-            expr=battery.discharge_current >= battery.minimum_discharge_current * battery.is_discharging)
+            expr=battery.discharge_current
+            >= battery.minimum_discharge_current * battery.is_discharging,
+        )
         battery.discharge_current_ub = pyomo.Constraint(
             doc="Battery Discharging current upper bound",
-            expr=battery.discharge_current <= battery.maximum_discharge_current * battery.is_discharging)
+            expr=battery.discharge_current
+            <= battery.maximum_discharge_current * battery.is_discharging,
+        )
         battery.discharge_current_ub_soc = pyomo.Constraint(
             doc="Battery Discharging current upper bound state-of-charge dependence",
-            expr=battery.discharge_current <= battery.maximum_discharge_current * battery.soc0)
+            expr=battery.discharge_current
+            <= battery.maximum_discharge_current * battery.soc0,
+        )
 
     @staticmethod
     def _create_lv_battery_power_equation_constraints(battery):
+        """Create power equation constraints for the battery model.
+
+        Args:
+            battery: Battery instance.
+
+        """
         battery.charge_power_equation = pyomo.Constraint(
             doc="Battery charge power equation equal to the product of current and voltage",
-            expr=battery.charge_power == battery.charge_current * (battery.voltage_slope * battery.soc0
-                                                                   + (battery.voltage_intercept
-                                                                      + battery.average_current
-                                                                      * battery.internal_resistance)))
+            expr=battery.charge_power
+            == battery.charge_current
+            * (
+                battery.voltage_slope * battery.soc0
+                + (
+                    battery.voltage_intercept
+                    + battery.average_current * battery.internal_resistance
+                )
+            ),
+        )
         battery.discharge_power_equation = pyomo.Constraint(
             doc="Battery discharge power equation equal to the product of current and voltage",
-            expr=battery.discharge_power == battery.discharge_current * (battery.voltage_slope * battery.soc0
-                                                                         + (battery.voltage_intercept
-                                                                            - battery.average_current
-                                                                            * battery.internal_resistance)))
+            expr=battery.discharge_power
+            == battery.discharge_current
+            * (
+                battery.voltage_slope * battery.soc0
+                + (
+                    battery.voltage_intercept
+                    - battery.average_current * battery.internal_resistance
+                )
+            ),
+        )
 
     def _lifecycle_count_rule(self, m, i):
+        """Lifecycle count rule.
+
+        Args:
+            m: Model instance.
+            i: Index.
+
+        """
         # current accounting
         start = int(i * self.timesteps_per_day)
         end = int((i + 1) * self.timesteps_per_day)
-        return self.model.lifecycles[i] == sum(self.blocks[t].time_duration
-                                            * (0.8 * self.blocks[t].discharge_current
-                                               - 0.8 * self.blocks[t].discharge_current * self.blocks[t].soc0)
-                                            / self.blocks[t].capacity for t in range(start, end))
+        return self.model.lifecycles[i] == sum(
+            self.blocks[t].time_duration
+            * (
+                0.8 * self.blocks[t].discharge_current
+                - 0.8 * self.blocks[t].discharge_current * self.blocks[t].soc0
+            )
+            / self.blocks[t].capacity
+            for t in range(start, end)
+        )
 
     def _set_control_mode(self):
+        """Set control mode."""
         self._system_model.value("control_mode", 0.0)  # Current control
         self.control_variable = "input_current"
 
     def _set_model_specific_parameters(self):
+        """Set model-specific parameters."""
         # Getting information from system_model
-        nominal_voltage = self._system_model.value('nominal_voltage')
-        nominal_energy = self._system_model.value('nominal_energy')
-        Vnom_default = self._system_model.value('Vnom_default')
-        C_rate = self._system_model.value('C_rate')
-        resistance = self._system_model.value('resistance')
-
-        Qfull = self._system_model.value('Qfull')
-        Qnom = self._system_model.value('Qnom')
-        Qexp = self._system_model.value('Qexp')
-
-        Vfull = self._system_model.value('Vfull')
-        Vnom = self._system_model.value('Vnom')
-        Vexp = self._system_model.value('Vexp')
+        nominal_voltage = self._system_model.value("nominal_voltage")
+        nominal_energy = self._system_model.value("nominal_energy")
+        Vnom_default = self._system_model.value("Vnom_default")
+        C_rate = self._system_model.value("C_rate")
+        resistance = self._system_model.value("resistance")
+
+        Qfull = self._system_model.value("Qfull")
+        Qnom = self._system_model.value("Qnom")
+        Qexp = self._system_model.value("Qexp")
+
+        Vfull = self._system_model.value("Vfull")
+        Vnom = self._system_model.value("Vnom")
+        Vexp = self._system_model.value("Vexp")
 
         # Using the Ceiling for both these -> Ceil(a/b) = -(-a//b)
-        cells_in_series = - (- nominal_voltage // Vnom_default)
-        strings_in_parallel = - (- nominal_energy * 1e3 // (Qfull * cells_in_series * Vnom_default))
+        cells_in_series = -(-nominal_voltage // Vnom_default)
+        strings_in_parallel = -(
+            -nominal_energy * 1e3 // (Qfull * cells_in_series * Vnom_default)
+        )
 
         self.capacity = Qfull * strings_in_parallel / 1e6  # [MAh]
 
         # Calculating linear approximation for Voltage as a function of state-of-charge
         soc_nom = (Qfull - Qnom) / Qfull
         if self.use_exp_voltage_point:
             # Using cell exp and nom voltage points
@@ -207,115 +330,140 @@
         else:
             # Using Cell full and nom voltage points
             a = (Vfull - Vnom) / (1.0 - soc_nom)
             b = Vfull - a
 
         self.voltage_slope = cells_in_series * a
         self.voltage_intercept = cells_in_series * b
-        self.average_current = (Qfull * strings_in_parallel * C_rate / 2.)
+        self.average_current = Qfull * strings_in_parallel * C_rate / 2.0
         self.internal_resistance = resistance * cells_in_series / strings_in_parallel
         # TODO: These parameters might need updating
         self.minimum_charge_current = 0.0
         self.maximum_charge_current = (Qfull * strings_in_parallel * C_rate) / 1e6
         self.minimum_discharge_current = 0.0
         self.maximum_discharge_current = (Qfull * strings_in_parallel * C_rate) / 1e6
 
     # Inputs
     @property
     def voltage_slope(self) -> float:
+        """Voltage slope."""
         for t in self.blocks.index_set():
             return self.blocks[t].voltage_slope.value
 
     @voltage_slope.setter
     def voltage_slope(self, voltage_slope: float):
         for t in self.blocks.index_set():
             self.blocks[t].voltage_slope = round(voltage_slope, self.round_digits)
 
     @property
     def voltage_intercept(self) -> float:
+        """Voltage intercept."""
         for t in self.blocks.index_set():
             return self.blocks[t].voltage_intercept.value
 
     @voltage_intercept.setter
     def voltage_intercept(self, voltage_intercept: float):
         for t in self.blocks.index_set():
-            self.blocks[t].voltage_intercept = round(voltage_intercept, self.round_digits)
+            self.blocks[t].voltage_intercept = round(
+                voltage_intercept, self.round_digits
+            )
 
     # # TODO: Add this if wanted
     # # self.alphaP = Param(None)  # [kW_DC]    Bi-directional intercept for charge
     # # self.betaP = Param(None)  # [-]         Bi-directional slope for charge
     # # self.alphaN = Param(None)  # [kW_DC]    Bi-directional intercept for discharge
     # # self.betaN = Param(None)  # [-]         Bi-directional slope for discharge
 
     @property
     def average_current(self) -> float:
+        """Average current."""
         for t in self.blocks.index_set():
             return self.blocks[t].average_current.value
 
     @average_current.setter
     def average_current(self, average_current: float):
         for t in self.blocks.index_set():
             self.blocks[t].average_current = round(average_current, self.round_digits)
 
     @property
     def internal_resistance(self) -> float:
+        """Internal resistance."""
         for t in self.blocks.index_set():
             return self.blocks[t].internal_resistance.value
 
     @internal_resistance.setter
     def internal_resistance(self, internal_resistance: float):
         for t in self.blocks.index_set():
-            self.blocks[t].internal_resistance = round(internal_resistance, self.round_digits)
+            self.blocks[t].internal_resistance = round(
+                internal_resistance, self.round_digits
+            )
 
     @property
     def minimum_charge_current(self) -> float:
+        """Minimum charge current."""
         for t in self.blocks.index_set():
             return self.blocks[t].minimum_charge_current.value
 
     @minimum_charge_current.setter
     def minimum_charge_current(self, minimum_charge_current: float):
         for t in self.blocks.index_set():
-            self.blocks[t].minimum_charge_current = round(minimum_charge_current, self.round_digits)
+            self.blocks[t].minimum_charge_current = round(
+                minimum_charge_current, self.round_digits
+            )
 
     @property
     def maximum_charge_current(self) -> float:
+        """Maximum charge current."""
         for t in self.blocks.index_set():
             return self.blocks[t].maximum_charge_current.value
 
     @maximum_charge_current.setter
     def maximum_charge_current(self, maximum_charge_current: float):
         for t in self.blocks.index_set():
-            self.blocks[t].maximum_charge_current = round(maximum_charge_current, self.round_digits)
+            self.blocks[t].maximum_charge_current = round(
+                maximum_charge_current, self.round_digits
+            )
 
     @property
     def minimum_discharge_current(self) -> float:
+        """Minimum discharge current."""
         for t in self.blocks.index_set():
             return self.blocks[t].minimum_discharge_current.value
 
     @minimum_discharge_current.setter
     def minimum_discharge_current(self, minimum_discharge_current: float):
         for t in self.blocks.index_set():
-            self.blocks[t].minimum_discharge_current = round(minimum_discharge_current, self.round_digits)
+            self.blocks[t].minimum_discharge_current = round(
+                minimum_discharge_current, self.round_digits
+            )
 
     @property
     def maximum_discharge_current(self) -> float:
+        """Maximum discharge current."""
         for t in self.blocks.index_set():
             return self.blocks[t].maximum_discharge_current.value
 
     @maximum_discharge_current.setter
     def maximum_discharge_current(self, maximum_discharge_current: float):
         for t in self.blocks.index_set():
-            self.blocks[t].maximum_discharge_current = round(maximum_discharge_current, self.round_digits)
+            self.blocks[t].maximum_discharge_current = round(
+                maximum_discharge_current, self.round_digits
+            )
 
     # Outputs
     @property
     def charge_current(self) -> list:
+        """Charge current."""
         return [self.blocks[t].charge_current.value for t in self.blocks.index_set()]
 
     @property
     def discharge_current(self) -> list:
+        """Discharge current."""
         return [self.blocks[t].discharge_current.value for t in self.blocks.index_set()]
 
     @property
     def current(self) -> list:
-        return [self.blocks[t].discharge_current.value - self.blocks[t].charge_current.value
-                for t in self.blocks.index_set()]
+        """Current."""
+        return [
+            self.blocks[t].discharge_current.value - self.blocks[t].charge_current.value
+            for t in self.blocks.index_set()
+        ]
```

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/dispatch/power_storage/one_cycle_battery_dispatch_heuristic.py` & `HOPP-2.2.0/hopp/simulation/technologies/dispatch/power_storage/one_cycle_battery_dispatch_heuristic.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,99 +1,128 @@
 from typing import Tuple
 import pyomo.environ as pyomo
 from pyomo.environ import units as u
 
 import PySAM.BatteryStateful as BatteryModel
 import PySAM.Singleowner as Singleowner
 
-from hopp.simulation.technologies.dispatch.power_storage.simple_battery_dispatch_heuristic import SimpleBatteryDispatchHeuristic
+from hopp.simulation.technologies.dispatch.power_storage.simple_battery_dispatch_heuristic import (
+    SimpleBatteryDispatchHeuristic,
+)
 
 
 class OneCycleBatteryDispatchHeuristic(SimpleBatteryDispatchHeuristic):
-    """
+    """One cycle per day heuristic battery dispatch."""
 
-    fixed_dispatch: list of normalized values [-1, 1] (Charging (-), Discharging (+))
-    """
-    def __init__(self,
-                 pyomo_model: pyomo.ConcreteModel,
-                 index_set: pyomo.Set,
-                 system_model: BatteryModel.BatteryStateful,
-                 financial_model: Singleowner.Singleowner,
-                 block_set_name: str = 'one_cycle_heuristic_battery',
-                 dispatch_options: dict = None):
+    def __init__(
+        self,
+        pyomo_model: pyomo.ConcreteModel,
+        index_set: pyomo.Set,
+        system_model: BatteryModel.BatteryStateful,
+        financial_model: Singleowner.Singleowner,
+        block_set_name: str = "one_cycle_heuristic_battery",
+        dispatch_options: dict = None,
+    ):
+        """Initialize OneCycleBatteryDispatchHeuristic.
+
+        Args:
+            pyomo_model (pyomo.ConcreteModel): Pyomo concrete model.
+            index_set (pyomo.Set): Indexed set.
+            system_model (BatteryModel.BatteryStateful): Battery system model.
+            financial_model (Singleowner.Singleowner): Financial model.
+            block_set_name (str, optional):Name of the block set. Defaults to 'one_cycle_heuristic_battery'.
+            dispatch_options (dict, optional): Dispatch options. Defaults to None.
+            
+        """
         if dispatch_options is None:
             dispatch_options = {}
-        super().__init__(pyomo_model,
-                         index_set,
-                         system_model,
-                         financial_model,
-                         block_set_name=block_set_name,
-                         dispatch_options=dispatch_options)
+        super().__init__(
+            pyomo_model,
+            index_set,
+            system_model,
+            financial_model,
+            block_set_name=block_set_name,
+            dispatch_options=dispatch_options,
+        )
         self.prices = list([0.0] * len(self.blocks.index_set()))
 
     def _heuristic_method(self, gen):
-        """This sets battery dispatch using a 1 cycle per day assumption.
+        """Sets battery dispatch using a one cycle per day assumption.
 
         Method:
-         1. Sort input prices
-         2. Determine the duration required to fully discharge and charge the battery
-         3. Set discharge and charge operations based on sorted prices
-         3. Check SOC feasibility
-         4. If infeasible, find infeasibility, shift operation to the next sorted price periods
-         5. Repeat step 4 until SOC feasible
-                NOTE: If operation is tried on half of time periods, then operation defaults to 'do nothing'
+            - Sort input prices
+            - Determine the duration required to fully discharge and charge the battery
+            - Set discharge and charge operations based on sorted prices
+            - Check SOC feasibility
+            - If infeasible, find infeasibility, shift operation to the next sorted price periods
+            - Repeat step 4 until SOC feasible
+
+            NOTE: If operation is tried on half of time periods, then operation defaults to 'do nothing'
+
         """
         if sum(self.prices) == 0.0 and max(self.prices) == 0.0:
             raise ValueError("prices must be set before calling heuristic method.")
 
         discharge_time, charge_time = self._get_duration_battery_full_cycle()
         fixed_dispatch = [0.0] * len(self.prices)
         price_and_gen = zip(range(0, len(self.prices)), self.prices, gen)
         sorted_prices = sorted(price_and_gen, key=lambda i: i[2], reverse=True)
         sorted_prices = sorted(sorted_prices, key=lambda i: i[1])
 
         # Set initial fixed dispatch
-        fixed_dispatch, next_charge_idx = self._charge_battery(charge_time, 0,
-                                                               sorted_prices,
-                                                               fixed_dispatch)
-
-        fixed_dispatch, next_discharge_idx = self._discharge_battery(discharge_time, 0,
-                                                                     sorted_prices,
-                                                                     fixed_dispatch)
+        fixed_dispatch, next_charge_idx = self._charge_battery(
+            charge_time, 0, sorted_prices, fixed_dispatch
+        )
+
+        fixed_dispatch, next_discharge_idx = self._discharge_battery(
+            discharge_time, 0, sorted_prices, fixed_dispatch
+        )
 
         # test feasibility and find infeasibility
         feasible = self.test_soc_feasibility(fixed_dispatch)
         while not feasible[0]:
             # TODO: Improve algorithm
             idx_infeasible = feasible[1]
             infeasible_value = fixed_dispatch[idx_infeasible]
             if infeasible_value > 0:  # Discharging
-                discharge_remaining = fixed_dispatch[idx_infeasible] * self.time_duration[idx_infeasible]
+                discharge_remaining = (
+                    fixed_dispatch[idx_infeasible] * self.time_duration[idx_infeasible]
+                )
                 fixed_dispatch[idx_infeasible] = 0
-                if next_discharge_idx < len(sorted_prices)/2:
-                    fixed_dispatch, next_discharge_idx = self._discharge_battery(discharge_remaining,
-                                                                                 next_discharge_idx,
-                                                                                 sorted_prices,
-                                                                                 fixed_dispatch)
-            elif infeasible_value < 0:    # Charging
-                charge_remaining = -fixed_dispatch[idx_infeasible] * self.time_duration[idx_infeasible]
+                if next_discharge_idx < len(sorted_prices) / 2:
+                    fixed_dispatch, next_discharge_idx = self._discharge_battery(
+                        discharge_remaining,
+                        next_discharge_idx,
+                        sorted_prices,
+                        fixed_dispatch,
+                    )
+            elif infeasible_value < 0:  # Charging
+                charge_remaining = (
+                    -fixed_dispatch[idx_infeasible] * self.time_duration[idx_infeasible]
+                )
                 fixed_dispatch[idx_infeasible] = 0
-                if next_charge_idx < len(sorted_prices)/2:  # TODO: maybe too restrictive
-                    fixed_dispatch, next_charge_idx = self._charge_battery(charge_remaining,
-                                                                           next_charge_idx,
-                                                                           sorted_prices,
-                                                                           fixed_dispatch)
+                if (
+                    next_charge_idx < len(sorted_prices) / 2
+                ):  # TODO: maybe too restrictive
+                    fixed_dispatch, next_charge_idx = self._charge_battery(
+                        charge_remaining, next_charge_idx, sorted_prices, fixed_dispatch
+                    )
             feasible = self.test_soc_feasibility(fixed_dispatch)
 
         self._fixed_dispatch = fixed_dispatch
 
-    def _discharge_battery(self, discharge_remaining, next_discharge_idx, sorted_prices, fixed_dispatch):
-        """Discharge battery using the remaining discharge and the next best discharge period.
+    def _discharge_battery(
+        self, discharge_remaining, next_discharge_idx, sorted_prices, fixed_dispatch
+    ):
+        """Discharges battery using the remaining discharge and the next best discharge period.
+
+        Returns:
+            Tuple[list, int]: Adjusted fixed dispatch and next discharge index to be tried.
 
-        Returns adjusted fixed_dispatch and next discharge index to be tried."""
+        """
         period_count = next_discharge_idx
         while discharge_remaining > 0:
             if period_count < len(sorted_prices):
                 idx = sorted_prices[-(period_count + 1)][0]
                 if self.max_discharge_fraction[idx] < discharge_remaining:
                     fixed_dispatch[idx] = self.max_discharge_fraction[idx]
                 else:
@@ -102,57 +131,80 @@
                 discharge_remaining -= fixed_dispatch[idx] * self.time_duration[idx]
                 period_count += 1
             else:
                 break
         next_discharge_idx = period_count
         return fixed_dispatch, next_discharge_idx
 
-    def _charge_battery(self, charge_remaining, next_charge_idx, sorted_prices, fixed_dispatch):
-        """Charge battery using the remaining charge and the next best charge period.
+    def _charge_battery(
+        self, charge_remaining, next_charge_idx, sorted_prices, fixed_dispatch
+    ):
+        """Charges battery using the remaining charge and the next best charge period.
+
+        Returns:
+            Tuple[list, int]: Adjusted fixed dispatch and next charge index to be tried.
 
-        Returns adjusted fixed_dispatch and next charge index to be tried."""
+        """
         period_count = next_charge_idx
         while charge_remaining > 0:
             if period_count < len(sorted_prices):
                 idx = sorted_prices[period_count][0]
                 if self.max_charge_fraction[idx] < charge_remaining:
-                    fixed_dispatch[idx] = - self.max_charge_fraction[idx]
+                    fixed_dispatch[idx] = -self.max_charge_fraction[idx]
                 else:
-                    fixed_dispatch[idx] = - charge_remaining
+                    fixed_dispatch[idx] = -charge_remaining
                 # update count and remaining discharge
                 charge_remaining += fixed_dispatch[idx] * self.time_duration[idx]
                 period_count += 1
             else:
                 break
         next_charge_idx = period_count
         return fixed_dispatch, next_charge_idx
 
     def _get_duration_battery_full_cycle(self) -> Tuple[float, float]:
-        """ Calculates discharge and charge hours required to fully cycle the battery."""
+        """Calculates discharge and charge hours required to fully cycle the battery.
+
+        Returns:
+            Tuple[float, float]: Discharge and charge hours.
+
+        """
         true_capacity = (self.maximum_soc - self.minimum_soc) * self.capacity / 100.0
 
-        n_discharge = true_capacity / (1/(self.discharge_efficiency/100.) * self.maximum_power)
-        n_charge = true_capacity / (self.charge_efficiency / 100. * self.maximum_power)
+        n_discharge = true_capacity / (
+            1 / (self.discharge_efficiency / 100.0) * self.maximum_power
+        )
+        n_charge = true_capacity / (self.charge_efficiency / 100.0 * self.maximum_power)
         return n_discharge, n_charge
 
     def test_soc_feasibility(self, fixed_dispatch) -> Tuple[bool, int]:
-        """Steps through fixed_dispatch and test SOC feasibility.
+        """Steps through fixed_dispatch and tests SOC feasibility.
+
+        Returns:
+            Tuple[bool, int]: Tuple indicating SOC feasibility and index of first infeasible operation.
 
-        If fixed_dispatch is infeasible, return index of first infeasibility operation.
         """
         soc0 = self.model.initial_soc.value
         for idx, fd in enumerate(fixed_dispatch):
             soc = self.update_soc(fd, soc0)
-            if round(soc, 6)*100. < self.minimum_soc or round(soc, 6)*100. > self.maximum_soc:
+            if (
+                round(soc, 6) * 100.0 < self.minimum_soc
+                or round(soc, 6) * 100.0 > self.maximum_soc
+            ):
                 return False, idx
             soc0 = soc
         return True, None
 
     @property
     def prices(self) -> list:
+        """List of normalized prices [-1, 1] (Charging (-), Discharging (+)).
+
+        Returns:
+            list: Prices.
+
+        """
         return self._prices
 
     @prices.setter
     def prices(self, prices: list):
         if len(prices) != len(self.blocks.index_set()):
             raise ValueError("prices must be the same length as dispatch index set.")
         self._prices = prices
```

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/dispatch/power_storage/power_storage_dispatch.py` & `HOPP-2.2.0/hopp/simulation/technologies/dispatch/power_storage/power_storage_dispatch.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,470 +3,726 @@
 from pyomo.network import Port
 from pyomo.environ import units as u
 
 from hopp.simulation.technologies.dispatch.dispatch import Dispatch
 
 
 class PowerStorageDispatch(Dispatch):
-    """
+    """Dispatch algorithm for power storage."""
 
-    """
+    def __init__(
+        self,
+        pyomo_model: pyomo.ConcreteModel,
+        index_set: pyomo.Set,
+        system_model,
+        financial_model,
+        block_set_name: str,
+        dispatch_options,
+    ):
+        """Intialize PowerStorageDispatch.
+
+        Args:
+            pyomo_model (pyomo.ConcreteModel): Pyomo concrete model.
+            index_set (pyomo.Set): Indexed set.
+            system_model: System model.
+            financial_model: Financial model.
+            block_set_name (str, optional): Name of the block set.
+            dispatch_options (dict, optional): Dispatch options.
 
-    def __init__(self,
-                 pyomo_model: pyomo.ConcreteModel,
-                 index_set: pyomo.Set,
-                 system_model,
-                 financial_model,
-                 block_set_name: str,
-                 dispatch_options):
+        """
 
-        super().__init__(pyomo_model, index_set, system_model, financial_model, block_set_name=block_set_name)
+        super().__init__(
+            pyomo_model,
+            index_set,
+            system_model,
+            financial_model,
+            block_set_name=block_set_name,
+        )
         self._create_soc_linking_constraint()
 
         # TODO: we could remove this option and just have lifecycle count default
         self.options = dispatch_options
         if self.options.include_lifecycle_count:
             self._create_lifecycle_model()
             if self.options.max_lifecycle_per_day < np.inf:
                 self._create_lifecycle_count_constraint()
 
     def dispatch_block_rule(self, storage):
-        """
-        Called during Dispatch's __init__
+        """Initializes storage parameters, variables, and constraints.
+            Called during Dispatch's __init__.
+
+        Args:
+            storage: Storage instance.
+
         """
         # Parameters
         self._create_storage_parameters(storage)
         self._create_efficiency_parameters(storage)
         self._create_capacity_parameter(storage)
         # Variables
         self._create_storage_variables(storage)
         # Constraints
         self._create_storage_constraints(storage)
         self._create_soc_inventory_constraint(storage)
         # Ports
         self._create_storage_port(storage)
 
+    def max_gross_profit_objective(self, hybrid_blocks):
+        """Sets the max gross profit objective for the dispatch.
+
+        Args:
+            hybrid_blocks (Pyomo.block): A generalized container for defining hierarchical
+                models by adding modeling components as attributes.
+
+        """
+
+        def battery_profit_objective_rule(m):
+            objective = 0
+            objective += sum(
+                -(1 / hybrid_blocks[t].time_weighting_factor)
+                * self.blocks[t].time_duration
+                * (
+                    self.blocks[t].cost_per_charge * hybrid_blocks[t].battery_charge
+                    + self.blocks[t].cost_per_discharge
+                    * hybrid_blocks[t].battery_discharge
+                )
+                for t in hybrid_blocks.index_set()
+            )
+            if self.options.include_lifecycle_count:
+                objective -= self.model.lifecycle_cost * sum(self.model.lifecycles)
+            return objective
+
+        self.obj = pyomo.Expression(rule=battery_profit_objective_rule)
+
+    def min_operating_cost_objective(self, hybrid_blocks):
+        """Sets the min operating cost objective for the dispatch.
+
+        Args:
+            hybrid_blocks (Pyomo.block): A generalized container for defining hierarchical
+                models by adding modeling components as attributes.
+
+        """
+        objective = sum(
+            hybrid_blocks[t].time_weighting_factor
+            * self.blocks[t].time_duration
+            * (
+                self.blocks[t].cost_per_discharge * hybrid_blocks[t].battery_discharge
+                - self.blocks[t].cost_per_charge * hybrid_blocks[t].battery_charge
+            )  # Try to incentivize battery charging
+            for t in self.blocks.index_set()
+        )
+        if self.options.include_lifecycle_count:
+            objective += self.model.lifecycle_cost * self.model.lifecycles
+
+        self.obj = objective
+
+    def _create_variables(self, hybrid):
+        """Creates storage variables.
+
+        Args:
+            hybrid: Hybrid instance.
+
+        Returns:
+            Tuple: Tuple containing battery discharge and charge variables.
+
+        """
+        hybrid.battery_charge = pyomo.Var(
+            doc="Power charging the electric battery [MW]",
+            domain=pyomo.NonNegativeReals,
+            units=u.MW,
+            initialize=0.0,
+        )
+        hybrid.battery_discharge = pyomo.Var(
+            doc="Power discharging the electric battery [MW]",
+            domain=pyomo.NonNegativeReals,
+            units=u.MW,
+            initialize=0.0,
+        )
+        return hybrid.battery_discharge, hybrid.battery_charge
+
+    def _create_port(self, hybrid):
+        """Creates storage port.
+
+        Args:
+            hybrid: Hybrid instance.
+
+        Returns:
+            Port: Storage port.
+
+        """
+        hybrid.battery_port = Port(
+            initialize={
+                "charge_power": hybrid.battery_charge,
+                "discharge_power": hybrid.battery_discharge,
+            }
+        )
+        return hybrid.battery_port
+
     def _create_storage_parameters(self, storage):
+        """Creates storage parameters.
+
+        Args:
+            storage: Storage instance.
+
+        """
         ##################################
         # Parameters                     #
         ##################################
         storage.time_duration = pyomo.Param(
             doc="Time step [hour]",
             default=1.0,
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.hr)
+            units=u.hr,
+        )
         storage.cost_per_charge = pyomo.Param(
             doc="Operating cost of " + self.block_set_name + " charging [$/MWh]",
-            default=0.,
+            default=0.0,
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.USD / u.MWh)
+            units=u.USD / u.MWh,
+        )
         storage.cost_per_discharge = pyomo.Param(
             doc="Operating cost of " + self.block_set_name + " discharging [$/MWh]",
-            default=0.,
+            default=0.0,
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.USD / u.MWh)
+            units=u.USD / u.MWh,
+        )
         storage.minimum_power = pyomo.Param(
             doc=self.block_set_name + " minimum power rating [MW]",
             default=0.0,
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.MW)
+            units=u.MW,
+        )
         storage.maximum_power = pyomo.Param(
             doc=self.block_set_name + " maximum power rating [MW]",
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.MW)
+            units=u.MW,
+        )
         storage.minimum_soc = pyomo.Param(
             doc=self.block_set_name + " minimum state-of-charge [-]",
             default=0.1,
             within=pyomo.PercentFraction,
             mutable=True,
-            units=u.dimensionless)
+            units=u.dimensionless,
+        )
         storage.maximum_soc = pyomo.Param(
             doc=self.block_set_name + " maximum state-of-charge [-]",
             default=0.9,
             within=pyomo.PercentFraction,
             mutable=True,
-            units=u.dimensionless)
+            units=u.dimensionless,
+        )
 
     def _create_efficiency_parameters(self, storage):
+        """Creates storage efficiency parameters.
+
+        Args:
+            storage: Storage instance.
+
+        """
         storage.charge_efficiency = pyomo.Param(
             doc=self.block_set_name + " Charging efficiency [-]",
             default=0.938,
             within=pyomo.PercentFraction,
             mutable=True,
-            units=u.dimensionless)
+            units=u.dimensionless,
+        )
         storage.discharge_efficiency = pyomo.Param(
             doc=self.block_set_name + " discharging efficiency [-]",
             default=0.938,
             within=pyomo.PercentFraction,
             mutable=True,
-            units=u.dimensionless)
+            units=u.dimensionless,
+        )
 
     def _create_capacity_parameter(self, storage):
+        """Creates storage capacity parameter.
+
+        Args:
+            storage: Storage instance.
+
+        """
         storage.capacity = pyomo.Param(
             doc=self.block_set_name + " capacity [MWh]",
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.MWh)
+            units=u.MWh,
+        )
 
     def _create_storage_variables(self, storage):
+        """Creates storage variables.
+
+        Args:
+            storage: Storage instance.
+
+        """
         ##################################
         # Variables                      #
         ##################################
         storage.is_charging = pyomo.Var(
             doc="1 if " + self.block_set_name + " is charging; 0 Otherwise [-]",
             domain=pyomo.Binary,
-            units=u.dimensionless)
+            units=u.dimensionless,
+        )
         storage.is_discharging = pyomo.Var(
             doc="1 if " + self.block_set_name + " is discharging; 0 Otherwise [-]",
             domain=pyomo.Binary,
-            units=u.dimensionless)
+            units=u.dimensionless,
+        )
         storage.soc0 = pyomo.Var(
-            doc=self.block_set_name + " initial state-of-charge at beginning of period[-]",
+            doc=self.block_set_name
+            + " initial state-of-charge at beginning of period[-]",
             domain=pyomo.PercentFraction,
             bounds=(storage.minimum_soc, storage.maximum_soc),
-            units=u.dimensionless)
+            units=u.dimensionless,
+        )
         storage.soc = pyomo.Var(
             doc=self.block_set_name + " state-of-charge at end of period [-]",
             domain=pyomo.PercentFraction,
             bounds=(storage.minimum_soc, storage.maximum_soc),
-            units=u.dimensionless)
+            units=u.dimensionless,
+        )
         storage.charge_power = pyomo.Var(
             doc="Power into " + self.block_set_name + " [MW]",
             domain=pyomo.NonNegativeReals,
-            units=u.MW)
+            units=u.MW,
+        )
         storage.discharge_power = pyomo.Var(
             doc="Power out of " + self.block_set_name + " [MW]",
             domain=pyomo.NonNegativeReals,
-            units=u.MW)
+            units=u.MW,
+        )
 
     def _create_storage_constraints(self, storage):
         ##################################
         # Constraints                    #
         ##################################
         # Charge power bounds
         storage.charge_power_ub = pyomo.Constraint(
             doc=self.block_set_name + " charging power upper bound",
-            expr=storage.charge_power <= storage.maximum_power * storage.is_charging)
+            expr=storage.charge_power <= storage.maximum_power * storage.is_charging,
+        )
         storage.charge_power_lb = pyomo.Constraint(
             doc=self.block_set_name + " charging power lower bound",
-            expr=storage.charge_power >= storage.minimum_power * storage.is_charging)
+            expr=storage.charge_power >= storage.minimum_power * storage.is_charging,
+        )
         # Discharge power bounds
         storage.discharge_power_lb = pyomo.Constraint(
             doc=self.block_set_name + " Discharging power lower bound",
-            expr=storage.discharge_power >= storage.minimum_power * storage.is_discharging)
+            expr=storage.discharge_power
+            >= storage.minimum_power * storage.is_discharging,
+        )
         storage.discharge_power_ub = pyomo.Constraint(
             doc=self.block_set_name + " Discharging power upper bound",
-            expr=storage.discharge_power <= storage.maximum_power * storage.is_discharging)
+            expr=storage.discharge_power
+            <= storage.maximum_power * storage.is_discharging,
+        )
         # Storage packing constraint
         storage.charge_discharge_packing = pyomo.Constraint(
-            doc=self.block_set_name + " packing constraint for charging and discharging binaries",
-            expr=storage.is_charging + storage.is_discharging <= 1)
+            doc=self.block_set_name
+            + " packing constraint for charging and discharging binaries",
+            expr=storage.is_charging + storage.is_discharging <= 1,
+        )
 
     def _create_soc_inventory_constraint(self, storage):
+        """Creates state-of-charge inventory constraint for storage.
+
+        Args:
+            storage: Storage instance.
+
+        """
+
         def soc_inventory_rule(m):
-            return m.soc == (m.soc0 + m.time_duration * (m.charge_efficiency * m.charge_power
-                                                         - (1 / m.discharge_efficiency) * m.discharge_power) / m.capacity)
+            return m.soc == (
+                m.soc0
+                + m.time_duration
+                * (
+                    m.charge_efficiency * m.charge_power
+                    - (1 / m.discharge_efficiency) * m.discharge_power
+                )
+                / m.capacity
+            )
+
         # Storage State-of-charge balance
         storage.soc_inventory = pyomo.Constraint(
             doc=self.block_set_name + " state-of-charge inventory balance",
-            rule=soc_inventory_rule)
+            rule=soc_inventory_rule,
+        )
 
     @staticmethod
     def _create_storage_port(storage):
+        """Creates storage port.
+
+        Args:
+            storage: Storage instance.
+
+        """
         ##################################
         # Ports                          #
         ##################################
         storage.port = Port()
         storage.port.add(storage.charge_power)
         storage.port.add(storage.discharge_power)
 
     def _create_soc_linking_constraint(self):
+        """Creates state-of-charge linking constraint."""
         ##################################
         # Parameters                     #
         ##################################
         self.model.initial_soc = pyomo.Param(
-            doc=self.block_set_name + " initial state-of-charge at beginning of the horizon[-]",
+            doc=self.block_set_name
+            + " initial state-of-charge at beginning of the horizon[-]",
             within=pyomo.PercentFraction,
             default=0.5,
             mutable=True,
-            units=u.dimensionless)
+            units=u.dimensionless,
+        )
         ##################################
         # Constraints                    #
         ##################################
 
         # Linking time periods together
         def storage_soc_linking_rule(m, t):
             if t == self.blocks.index_set().first():
                 return self.blocks[t].soc0 == self.model.initial_soc
             return self.blocks[t].soc0 == self.blocks[t - 1].soc
+
         self.model.soc_linking = pyomo.Constraint(
             self.blocks.index_set(),
             doc=self.block_set_name + " state-of-charge block linking constraint",
-            rule=storage_soc_linking_rule)
+            rule=storage_soc_linking_rule,
+        )
 
     def _lifecycle_count_rule(self, m, i):
+        """Calculates lifecycle count rule.
+
+        Args:
+            m: Model instance.
+            i: Index.
+
+        Returns:
+            float: Lifecycle count.
+
+        """
         # Use full-energy cycles
         start = int(i * self.timesteps_per_day)
         end = int((i + 1) * self.timesteps_per_day)
-        return m.lifecycles[i] == sum(self.blocks[t].time_duration
-                                            * self.blocks[t].discharge_power
-                                            / self.blocks[t].capacity for t in range(start, end))
+        return m.lifecycles[i] == sum(
+            self.blocks[t].time_duration
+            * self.blocks[t].discharge_power
+            / self.blocks[t].capacity
+            for t in range(start, end)
+        )
 
     def _create_lifecycle_model(self):
+        """Creates lifecycle model."""
         ##################################
         # Parameters                     #
         ##################################
         self.timesteps_per_day = 24 / pyomo.value(self.blocks[0].time_duration)
-        self.model.days = pyomo.RangeSet(0, int(len(self.blocks)) / self.timesteps_per_day - 1)
+        self.model.days = pyomo.RangeSet(
+            0, int(len(self.blocks)) / self.timesteps_per_day - 1
+        )
         self.model.lifecycle_cost = pyomo.Param(
             doc="Lifecycle cost of " + self.block_set_name + " [$/lifecycle]",
             default=0.0,
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.USD / u.lifecycle)
+            units=u.USD / u.lifecycle,
+        )
         ##################################
         # Variables                      #
         ##################################
         self.model.lifecycles = pyomo.Var(
             self.model.days,
             doc=self.block_set_name + " lifecycle count",
             domain=pyomo.NonNegativeReals,
-            units=u.lifecycle)
+            units=u.lifecycle,
+        )
         ##################################
         # Constraints                    #
         ##################################
         self.model.lifecycle_count = pyomo.Constraint(
             self.model.days,
             doc=self.block_set_name + " lifecycle counting",
-            rule=self._lifecycle_count_rule
+            rule=self._lifecycle_count_rule,
         )
         ##################################
         # Ports                          #
         ##################################
         self.model.lifecycles_port = Port()
         self.model.lifecycles_port.add(self.model.lifecycles)
         self.model.lifecycles_port.add(self.model.lifecycle_cost)
 
-
     def _create_lifecycle_count_constraint(self):
+        """Creates lifecycle count constraint."""
         self.model.max_cycles_per_day = pyomo.Param(
             doc="Max number of full energy cycles per day for " + self.block_set_name,
             default=self.options.max_lifecycle_per_day,
             within=pyomo.NonNegativeReals,
             mutable=True,
-            units=u.lifecycle)
-        
+            units=u.lifecycle,
+        )
+
         self.model.lifecycle_count_constraint = pyomo.Constraint(
-            self.model.days,
-            rule=lambda m, i: m.lifecycles[i] <= m.max_cycles_per_day
+            self.model.days, rule=lambda m, i: m.lifecycles[i] <= m.max_cycles_per_day
         )
 
     def _check_initial_soc(self, initial_soc):
+        """Checks initial state-of-charge.
+
+        Args:
+            initial_soc: Initial state-of-charge value.
+
+        Returns:
+            float: Checked initial state-of-charge.
+            
+        """
         if initial_soc > 1:
-            initial_soc /= 100.
+            initial_soc /= 100.0
         initial_soc = round(initial_soc, self.round_digits)
-        if initial_soc > self.maximum_soc/100:
-            print("Warning: Storage dispatch was initialized with a state-of-charge greater than maximum value!")
+        if initial_soc > self.maximum_soc / 100:
+            print(
+                "Warning: Storage dispatch was initialized with a state-of-charge greater than "
+                "maximum value!"
+            )
             print("Initial SOC = {}".format(initial_soc))
             print("Initial SOC was set to maximum value.")
             initial_soc = self.maximum_soc / 100
-        elif initial_soc < self.minimum_soc/100:
-            print("Warning: Storage dispatch was initialized with a state-of-charge less than minimum value!")
+        elif initial_soc < self.minimum_soc / 100:
+            print(
+                "Warning: Storage dispatch was initialized with a state-of-charge less than "
+                "minimum value!"
+            )
             print("Initial SOC = {}".format(initial_soc))
             print("Initial SOC was set to minimum value.")
             initial_soc = self.minimum_soc / 100
         return initial_soc
 
     def update_dispatch_initial_soc(self, initial_soc: float = None):
-        raise NotImplemented("This function must be overridden for specific storage dispatch model")
+        raise NotImplemented(
+            "This function must be overridden for specific storage dispatch model"
+        )
 
     # INPUTS
     @property
     def time_duration(self) -> list:
+        """Time duration."""
         return [self.blocks[t].time_duration.value for t in self.blocks.index_set()]
 
     @time_duration.setter
     def time_duration(self, time_duration: list):
         if len(time_duration) == len(self.blocks):
             for t, delta in zip(self.blocks, time_duration):
                 self.blocks[t].time_duration = round(delta, self.round_digits)
         else:
-            raise ValueError(self.time_duration.__name__ + " list must be the same length as time horizon")
+            raise ValueError(
+                self.time_duration.__name__
+                + " list must be the same length as time horizon"
+            )
 
     @property
     def cost_per_charge(self) -> float:
+        """Cost per charge."""
         for t in self.blocks.index_set():
             return self.blocks[t].cost_per_charge.value
 
     @cost_per_charge.setter
     def cost_per_charge(self, om_dollar_per_mwh: float):
         for t in self.blocks.index_set():
             self.blocks[t].cost_per_charge = round(om_dollar_per_mwh, self.round_digits)
 
     @property
     def cost_per_discharge(self) -> float:
+        """Cost per discharge."""
         for t in self.blocks.index_set():
             return self.blocks[t].cost_per_discharge.value
 
     @cost_per_discharge.setter
     def cost_per_discharge(self, om_dollar_per_mwh: float):
         for t in self.blocks.index_set():
-            self.blocks[t].cost_per_discharge = round(om_dollar_per_mwh, self.round_digits)
+            self.blocks[t].cost_per_discharge = round(
+                om_dollar_per_mwh, self.round_digits
+            )
 
     @property
     def minimum_power(self) -> float:
+        """Minimum power."""
         for t in self.blocks.index_set():
             return self.blocks[t].minimum_power.value
 
     @minimum_power.setter
     def minimum_power(self, minimum_power_mw: float):
         for t in self.blocks.index_set():
             self.blocks[t].minimum_power = round(minimum_power_mw, self.round_digits)
 
     @property
     def maximum_power(self) -> float:
+        """Maximum power."""
         for t in self.blocks.index_set():
             return self.blocks[t].maximum_power.value
 
     @maximum_power.setter
     def maximum_power(self, maximum_power_mw: float):
         for t in self.blocks.index_set():
             self.blocks[t].maximum_power = round(maximum_power_mw, self.round_digits)
 
     @property
     def minimum_soc(self) -> float:
+        """Minimum state-of-charge."""
         for t in self.blocks.index_set():
-            return self.blocks[t].minimum_soc.value * 100.
+            return self.blocks[t].minimum_soc.value * 100.0
 
     @minimum_soc.setter
     def minimum_soc(self, minimum_soc: float):
         if minimum_soc > 1:
-            minimum_soc /= 100.
+            minimum_soc /= 100.0
         for t in self.blocks.index_set():
             self.blocks[t].minimum_soc = round(minimum_soc, self.round_digits)
 
     @property
     def maximum_soc(self) -> float:
+        """Maximum state-of-charge."""
         for t in self.blocks.index_set():
-            return self.blocks[t].maximum_soc.value * 100.
+            return self.blocks[t].maximum_soc.value * 100.0
 
     @maximum_soc.setter
     def maximum_soc(self, maximum_soc: float):
         if maximum_soc > 1:
-            maximum_soc /= 100.
+            maximum_soc /= 100.0
         for t in self.blocks.index_set():
             self.blocks[t].maximum_soc = round(maximum_soc, self.round_digits)
 
     @property
     def charge_efficiency(self) -> float:
+        """Charge efficiency."""
         for t in self.blocks.index_set():
-            return self.blocks[t].charge_efficiency.value * 100.
+            return self.blocks[t].charge_efficiency.value * 100.0
 
     @charge_efficiency.setter
     def charge_efficiency(self, efficiency: float):
         efficiency = self._check_efficiency_value(efficiency)
         for t in self.blocks.index_set():
             self.blocks[t].charge_efficiency = round(efficiency, self.round_digits)
 
     @property
     def discharge_efficiency(self) -> float:
+        """Discharge efficiency."""
         for t in self.blocks.index_set():
-            return self.blocks[t].discharge_efficiency.value * 100.
+            return self.blocks[t].discharge_efficiency.value * 100.0
 
     @discharge_efficiency.setter
     def discharge_efficiency(self, efficiency: float):
         efficiency = self._check_efficiency_value(efficiency)
         for t in self.blocks.index_set():
             self.blocks[t].discharge_efficiency = round(efficiency, self.round_digits)
 
     @property
     def round_trip_efficiency(self) -> float:
-        return self.charge_efficiency * self.discharge_efficiency / 100.
+        """Round trip efficiency."""
+        return self.charge_efficiency * self.discharge_efficiency / 100.0
 
     @round_trip_efficiency.setter
     def round_trip_efficiency(self, round_trip_efficiency: float):
         round_trip_efficiency = self._check_efficiency_value(round_trip_efficiency)
-        efficiency = round_trip_efficiency ** (1 / 2)  # Assumes equal charge and discharge efficiencies
+        # Assumes equal charge and discharge efficiencies
+        efficiency = round_trip_efficiency ** (1 / 2)
         self.charge_efficiency = efficiency
         self.discharge_efficiency = efficiency
 
     @property
     def capacity(self) -> float:
+        """Capacity."""
         for t in self.blocks.index_set():
             return self.blocks[t].capacity.value
 
     @capacity.setter
     def capacity(self, capacity_mwh: float):
         for t in self.blocks.index_set():
             self.blocks[t].capacity = round(capacity_mwh, self.round_digits)
 
     @property
     def initial_soc(self) -> float:
-        return self.model.initial_soc.value * 100.
+        """Initial state-of-charge."""
+        return self.model.initial_soc.value * 100.0
 
     @initial_soc.setter
     def initial_soc(self, initial_soc: float):
         initial_soc = self._check_initial_soc(initial_soc)
         self.model.initial_soc = round(initial_soc, self.round_digits)
 
     @property
     def lifecycle_cost(self) -> float:
+        """Lifecycle cost."""
         return self.model.lifecycle_cost.value
 
     @lifecycle_cost.setter
     def lifecycle_cost(self, lifecycle_cost: float):
         self.model.lifecycle_cost = lifecycle_cost
 
     @property
     def lifecycle_cost_per_kWh_cycle(self) -> float:
+        """Lifecycle cost per kWh cycle."""
         return self.options.lifecycle_cost_per_kWh_cycle
 
     @lifecycle_cost_per_kWh_cycle.setter
     def lifecycle_cost_per_kWh_cycle(self, lifecycle_cost_per_kWh_cycle: float):
         self.options.lifecycle_cost_per_kWh_cycle = lifecycle_cost_per_kWh_cycle
-        self.model.lifecycle_cost = lifecycle_cost_per_kWh_cycle * self._system_model.value('nominal_energy')
+        self.model.lifecycle_cost = (
+            lifecycle_cost_per_kWh_cycle * self._system_model.value("nominal_energy")
+        )
 
     # Outputs
     @property
     def is_charging(self) -> list:
+        """Storage is charging."""
         return [self.blocks[t].is_charging.value for t in self.blocks.index_set()]
 
     @property
     def is_discharging(self) -> list:
+        """Storage is discharging."""
         return [self.blocks[t].is_discharging.value for t in self.blocks.index_set()]
 
     @property
     def soc(self) -> list:
+        """State-of-charge."""
         return [self.blocks[t].soc.value * 100.0 for t in self.blocks.index_set()]
 
     @property
     def charge_power(self) -> list:
+        """Charge power."""
         return [self.blocks[t].charge_power.value for t in self.blocks.index_set()]
 
     @property
     def discharge_power(self) -> list:
+        """Discharge power."""
         return [self.blocks[t].discharge_power.value for t in self.blocks.index_set()]
 
     @property
     def lifecycles(self) -> float:
+        """Lifecycles."""
         if self.options.include_lifecycle_count:
             return [pyomo.value(i) for _, i in self.model.lifecycles.items()]
         else:
             return []
 
     @property
     def power(self) -> list:
-        return [self.blocks[t].discharge_power.value - self.blocks[t].charge_power.value
-                for t in self.blocks.index_set()]
+        """Power."""
+        return [
+            self.blocks[t].discharge_power.value - self.blocks[t].charge_power.value
+            for t in self.blocks.index_set()
+        ]
 
     @property
     def current(self) -> list:
+        """Current."""
         return [0.0 for t in self.blocks.index_set()]
 
     @property
     def generation(self) -> list:
+        """Generation."""
         return self.power
```

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/dispatch/power_storage/simple_battery_dispatch.py` & `HOPP-2.2.0/hopp/simulation/technologies/dispatch/power_storage/simple_battery_dispatch.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,67 +1,109 @@
 import pyomo.environ as pyomo
 from pyomo.environ import units as u
 
 import PySAM.BatteryStateful as BatteryModel
-import PySAM.Singleowner as Singleowner
 
-from hopp.simulation.technologies.dispatch.power_storage.power_storage_dispatch import PowerStorageDispatch
+from hopp.simulation.technologies.dispatch.power_storage.power_storage_dispatch import (
+    PowerStorageDispatch,
+)
 from hopp.simulation.technologies.financial import FinancialModelType
 
 
 class SimpleBatteryDispatch(PowerStorageDispatch):
-    _system_model: BatteryModel.BatteryStateful
-    _financial_model: Singleowner.Singleowner
-    """
-
-    """
-
-    def __init__(self,
-                 pyomo_model: pyomo.ConcreteModel,
-                 index_set: pyomo.Set,
-                 system_model: BatteryModel.BatteryStateful,
-                 financial_model: FinancialModelType,
-                 block_set_name: str,
-                 dispatch_options):
-        super().__init__(pyomo_model,
-                         index_set,
-                         system_model,
-                         financial_model,
-                         block_set_name=block_set_name,
-                         dispatch_options=dispatch_options)
+    """A dispatch class for simple battery operations."""
+
+    def __init__(
+        self,
+        pyomo_model: pyomo.ConcreteModel,
+        index_set: pyomo.Set,
+        system_model: BatteryModel.BatteryStateful,
+        financial_model: FinancialModelType,
+        block_set_name: str,
+        dispatch_options,
+    ):
+        """Initializes SimpleBatteryDispatch.
+
+        Args:
+            pyomo_model (pyomo.ConcreteModel): The Pyomo model instance.
+            index_set (pyomo.Set): The Pyomo index set.
+            system_model (BatteryModel.BatteryStateful): The battery stateful model.
+            financial_model (FinancialModelType): The financial model type.
+            block_set_name (str): Name of the block set.
+            dispatch_options: Dispatch options.
+            
+        """
+        super().__init__(
+            pyomo_model,
+            index_set,
+            system_model,
+            financial_model,
+            block_set_name=block_set_name,
+            dispatch_options=dispatch_options,
+        )
 
     def initialize_parameters(self):
+        """Initializes parameters."""
         if self.options.include_lifecycle_count:
-            self.lifecycle_cost = self.options.lifecycle_cost_per_kWh_cycle * self._system_model.value('nominal_energy')
-
-        self.cost_per_charge = 0.75  # [$/MWh]
-        self.cost_per_discharge = 0.75  # [$/MWh]
+            self.lifecycle_cost = (
+                self.options.lifecycle_cost_per_kWh_cycle
+                * self._system_model.value("nominal_energy")
+            )
+
+        self.cost_per_charge = self._financial_model.value("om_batt_variable_cost")[
+            0
+        ]  # [$/MWh]
+        self.cost_per_discharge = self._financial_model.value("om_batt_variable_cost")[
+            0
+        ]  # [$/MWh]
         self.minimum_power = 0.0
         # FIXME: Change C_rate call to user set system_capacity_kw
         # self.maximum_power = self._system_model.value('nominal_energy') * self._system_model.value('C_rate') / 1e3
         self.maximum_power = self._financial_model.value("system_capacity") / 1e3
-        self.minimum_soc = self._system_model.value('minimum_SOC')
-        self.maximum_soc = self._system_model.value('maximum_SOC')
-        self.initial_soc = self._system_model.value('initial_SOC')
+        self.minimum_soc = self._system_model.value("minimum_SOC")
+        self.maximum_soc = self._system_model.value("maximum_SOC")
+        self.initial_soc = self._system_model.value("initial_SOC")
 
         self._set_control_mode()
         self._set_model_specific_parameters()
 
     def _set_control_mode(self):
+        """Sets control mode."""
         if isinstance(self._system_model, BatteryModel.BatteryStateful):
             self._system_model.value("control_mode", 1.0)  # Power control
-            self._system_model.value("input_power", 0.)
+            self._system_model.value("input_power", 0.0)
             self.control_variable = "input_power"
 
-    def _set_model_specific_parameters(self):
-        self.round_trip_efficiency = 88.0  # Including converter efficiency
-        self.capacity = self._system_model.value('nominal_energy') / 1e3  # [MWh]
+    def _set_model_specific_parameters(self, round_trip_efficiency=88.0):
+        """Sets model-specific parameters.
+
+        Args:
+            round_trip_efficiency (float, optional): The round-trip efficiency including converter efficiency.
+                Defaults to 88.0, which includes converter efficiency.
+
+        """
+        self.round_trip_efficiency = (
+            round_trip_efficiency  # Including converter efficiency
+        )
+        self.capacity = self._system_model.value("nominal_energy") / 1e3  # [MWh]
 
     def update_time_series_parameters(self, start_time: int):
+        """Updates time series parameters.
+
+        Args:
+            start_time (int): The start time.
+
+        """
         # TODO: provide more control
         self.time_duration = [1.0] * len(self.blocks.index_set())
 
     def update_dispatch_initial_soc(self, initial_soc: float = None):
+        """Updates dispatch initial state of charge (SOC).
+
+        Args:
+            initial_soc (float, optional): Initial state of charge. Defaults to None.
+
+        """
         if initial_soc is not None:
             self._system_model.value("initial_SOC", initial_soc)
             self._system_model.setup()  # TODO: Do I need to re-setup stateful battery?
-        self.initial_soc = self._system_model.value('SOC')
+        self.initial_soc = self._system_model.value("SOC")
```

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/dispatch/power_storage/simple_battery_dispatch_heuristic.py` & `HOPP-2.2.0/hopp/simulation/technologies/dispatch/power_storage/simple_battery_dispatch_heuristic.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,117 +1,195 @@
+from typing import Optional, List, Dict
+
 import pyomo.environ as pyomo
 from pyomo.environ import units as u
 
 import PySAM.BatteryStateful as BatteryModel
 import PySAM.Singleowner as Singleowner
 
-from hopp.simulation.technologies.dispatch.power_storage.simple_battery_dispatch import SimpleBatteryDispatch
+from hopp.simulation.technologies.dispatch.power_storage.simple_battery_dispatch import (
+    SimpleBatteryDispatch,
+)
 
 
 class SimpleBatteryDispatchHeuristic(SimpleBatteryDispatch):
     """Fixes battery dispatch operations based on user input.
 
-    Currently, enforces available generation and grid limit assuming no battery charging from grid
+    Currently, enforces available generation and grid limit assuming no battery charging from grid.
+
     """
-    def __init__(self,
-                 pyomo_model: pyomo.ConcreteModel,
-                 index_set: pyomo.Set,
-                 system_model: BatteryModel.BatteryStateful,
-                 financial_model: Singleowner.Singleowner,
-                 fixed_dispatch: list = None,
-                 block_set_name: str = 'heuristic_battery',
-                 dispatch_options: dict = None):
-        """
 
-        :param fixed_dispatch: list of normalized values [-1, 1] (Charging (-), Discharging (+))
+    def __init__(
+        self,
+        pyomo_model: pyomo.ConcreteModel,
+        index_set: pyomo.Set,
+        system_model: BatteryModel.BatteryStateful,
+        financial_model: Singleowner.Singleowner,
+        fixed_dispatch: Optional[List] = None,
+        block_set_name: str = "heuristic_battery",
+        dispatch_options: Optional[Dict] = None,
+    ):
+        """Initialize SimpleBatteryDispatchHeuristic.
+
+        Args:
+            pyomo_model (pyomo.ConcreteModel): Pyomo concrete model.
+            index_set (pyomo.Set): Indexed set.
+            system_model (BatteryModel.BatteryStateful): Battery system model.
+            financial_model (Singleowner.Singleowner): Financial model.
+            fixed_dispatch (Optional[List], optional): List of normalized values [-1, 1] (Charging (-), Discharging (+)). Defaults to None.
+            block_set_name (str, optional): Name of block set. Defaults to 'heuristic_battery'.
+            dispatch_options (dict, optional): Dispatch options. Defaults to None.
+
         """
         if dispatch_options is None:
             dispatch_options = {}
-        super().__init__(pyomo_model,
-                         index_set,
-                         system_model,
-                         financial_model,
-                         block_set_name=block_set_name,
-                         dispatch_options=dispatch_options)
-
-        self.max_charge_fraction = list([0.0]*len(self.blocks.index_set()))
-        self.max_discharge_fraction = list([0.0]*len(self.blocks.index_set()))
-        self.user_fixed_dispatch = list([0.0]*len(self.blocks.index_set()))
+        super().__init__(
+            pyomo_model,
+            index_set,
+            system_model,
+            financial_model,
+            block_set_name=block_set_name,
+            dispatch_options=dispatch_options,
+        )
+
+        self.max_charge_fraction = list([0.0] * len(self.blocks.index_set()))
+        self.max_discharge_fraction = list([0.0] * len(self.blocks.index_set()))
+        self.user_fixed_dispatch = list([0.0] * len(self.blocks.index_set()))
         # TODO: should I enforce either a day schedule or a year schedule year and save it as user input.
         #  Additionally, Should I drop it as input in the init function?
         if fixed_dispatch is not None:
             self.user_fixed_dispatch = fixed_dispatch
 
         self._fixed_dispatch = list([0.0] * len(self.blocks.index_set()))
 
     def set_fixed_dispatch(self, gen: list, grid_limit: list):
         """Sets charge and discharge power of battery dispatch using fixed_dispatch attribute and enforces available
         generation and grid limits.
 
+        Args:
+            gen (list): Generation blocks.
+            grid_limit (list): Grid capacity.
+
+        Raises:
+            ValueError: If gen or grid_limit length does not match fixed_dispatch length.
+
         """
         self.check_gen_grid_limit(gen, grid_limit)
         self._set_power_fraction_limits(gen, grid_limit)
         self._heuristic_method(gen)
         self._fix_dispatch_model_variables()
 
     def check_gen_grid_limit(self, gen: list, grid_limit: list):
+        """Checks if generation and grid limit lengths match fixed_dispatch length.
+
+        Args:
+            gen (list): Generation blocks.
+            grid_limit (list): Grid capacity.
+
+        Raises:
+            ValueError: If gen or grid_limit length does not match fixed_dispatch length.
+
+        """
         if len(gen) != len(self.fixed_dispatch):
             raise ValueError("gen must be the same length as fixed_dispatch.")
         elif len(grid_limit) != len(self.fixed_dispatch):
             raise ValueError("grid_limit must be the same length as fixed_dispatch.")
 
     def _set_power_fraction_limits(self, gen: list, grid_limit: list):
-        """Set battery charge and discharge power fraction limits based on available generation and grid capacity,
-        respectively.
+        """Set battery charge and discharge power fraction limits based on
+        available generation and grid capacity, respectively.
+
+        Args:
+            gen (list): Generation blocks.
+            grid_limit (list): Grid capacity.
 
         NOTE: This method assumes that battery cannot be charged by the grid.
+
         """
         for t in self.blocks.index_set():
-            self.max_charge_fraction[t] = self.enforce_power_fraction_simple_bounds(gen[t] / self.maximum_power)
-            self.max_discharge_fraction[t] = self.enforce_power_fraction_simple_bounds((grid_limit[t] - gen[t])
-                                                                                       / self.maximum_power)
+            self.max_charge_fraction[t] = self.enforce_power_fraction_simple_bounds(
+                gen[t] / self.maximum_power
+            )
+            self.max_discharge_fraction[t] = self.enforce_power_fraction_simple_bounds(
+                (grid_limit[t] - gen[t]) / self.maximum_power
+            )
 
     @staticmethod
-    def enforce_power_fraction_simple_bounds(power_fraction) -> float:
-        """ Enforces simple bounds (0,1) for battery power fractions."""
-        if power_fraction > 1.0:
-            power_fraction = 1.0
+    def enforce_power_fraction_simple_bounds(power_fraction: float) -> float:
+        """Enforces simple bounds (0, .9) for battery power fractions.
+
+        Args:
+            power_fraction (float): Power fraction from heuristic method.
+
+        Returns:
+            power_fraction (float): Bounded power fraction.
+
+        """
+        if power_fraction > 0.9:
+            power_fraction = 0.9
         elif power_fraction < 0.0:
             power_fraction = 0.0
         return power_fraction
 
-    def update_soc(self, power_fraction, soc0) -> float:
+    def update_soc(self, power_fraction: float, soc0: float) -> float:
+        """Updates SOC based on power fraction threshold (0.1).
+
+        Args:
+            power_fraction (float): Power fraction from heuristic method. Below threshold
+                is charging, above is discharging.
+            soc0 (float): Initial SOC.
+
+        Returns:
+            soc (float): Updated SOC.
+            
+        """
         if power_fraction > 0.0:
             discharge_power = power_fraction * self.maximum_power
-            soc = soc0 - self.time_duration[0] * (1/(self.discharge_efficiency/100.) * discharge_power) / self.capacity
+            soc = (
+                soc0
+                - self.time_duration[0]
+                * (1 / (self.discharge_efficiency / 100.0) * discharge_power)
+                / self.capacity
+            )
         elif power_fraction < 0.0:
-            charge_power = - power_fraction * self.maximum_power
-            soc = soc0 + self.time_duration[0] * (self.charge_efficiency / 100. * charge_power) / self.capacity
+            charge_power = -power_fraction * self.maximum_power
+            soc = (
+                soc0
+                + self.time_duration[0]
+                * (self.charge_efficiency / 100.0 * charge_power)
+                / self.capacity
+            )
         else:
             soc = soc0
-        soc = max(0, min(1, soc))
+
+        min_soc = self._system_model.value("minimum_SOC") / 100
+        max_soc = self._system_model.value("maximum_SOC") / 100
+
+        soc = max(min_soc, min(max_soc, soc))
+
         return soc
 
     def _heuristic_method(self, _):
-        """ Does specific heuristic method to fix battery dispatch."""
+        """Executes specific heuristic method to fix battery dispatch."""
         self._enforce_power_fraction_limits()
 
     def _enforce_power_fraction_limits(self):
-        """ Enforces battery power fraction limits and sets _fixed_dispatch attribute"""
+        """Enforces battery power fraction limits and sets _fixed_dispatch attribute."""
         for t in self.blocks.index_set():
             fd = self.user_fixed_dispatch[t]
-            if fd > 0.0:    # Discharging
+            if fd > 0.0:  # Discharging
                 if fd > self.max_discharge_fraction[t]:
                     fd = self.max_discharge_fraction[t]
             elif fd < 0.0:  # Charging
-                if - fd > self.max_charge_fraction[t]:
-                    fd = - self.max_charge_fraction[t]
+                if -fd > self.max_charge_fraction[t]:
+                    fd = -self.max_charge_fraction[t]
             self._fixed_dispatch[t] = fd
 
     def _fix_dispatch_model_variables(self):
+        """Fixes dispatch model variables based on the fixed dispatch values."""
         soc0 = self.model.initial_soc.value
         for t in self.blocks.index_set():
             dispatch_factor = self._fixed_dispatch[t]
             self.blocks[t].soc.fix(self.update_soc(dispatch_factor, soc0))
             soc0 = self.blocks[t].soc.value
 
             if dispatch_factor == 0.0:
@@ -121,27 +199,32 @@
             elif dispatch_factor > 0.0:
                 # Discharging
                 self.blocks[t].charge_power.fix(0.0)
                 self.blocks[t].discharge_power.fix(dispatch_factor * self.maximum_power)
             elif dispatch_factor < 0.0:
                 # Charging
                 self.blocks[t].discharge_power.fix(0.0)
-                self.blocks[t].charge_power.fix(- dispatch_factor * self.maximum_power)
+                self.blocks[t].charge_power.fix(-dispatch_factor * self.maximum_power)
 
     @property
     def fixed_dispatch(self) -> list:
+        """list: List of fixed dispatch."""
         return self._fixed_dispatch
 
     @property
     def user_fixed_dispatch(self) -> list:
+        """list: List of user fixed dispatch."""
         return self._user_fixed_dispatch
 
     @user_fixed_dispatch.setter
     def user_fixed_dispatch(self, fixed_dispatch: list):
         # TODO: Annual dispatch array...
         if len(fixed_dispatch) != len(self.blocks.index_set()):
-            raise ValueError("fixed_dispatch must be the same length as dispatch index set.")
+            raise ValueError(
+                "fixed_dispatch must be the same length as dispatch index set."
+            )
         elif max(fixed_dispatch) > 1.0 or min(fixed_dispatch) < -1.0:
-            raise ValueError("fixed_dispatch must be normalized values between -1 and 1.")
+            raise ValueError(
+                "fixed_dispatch must be normalized values between -1 and 1."
+            )
         else:
             self._user_fixed_dispatch = fixed_dispatch
-
```

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/financial/custom_financial_model.py` & `HOPP-2.2.0/hopp/simulation/technologies/financial/custom_financial_model.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/financial/mhk_cost_model.py` & `HOPP-2.2.0/hopp/simulation/technologies/financial/mhk_cost_model.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/grid.py` & `HOPP-2.2.0/hopp/simulation/technologies/grid.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-from typing import Iterable, List, Sequence, Optional, Union
+from typing import Iterable, List, Sequence, Optional, Union, TYPE_CHECKING
 
 import numpy as np
 from attrs import define, field
 import PySAM.Grid as GridModel
 import PySAM.Singleowner as Singleowner
 
 from hopp.simulation.technologies.sites import SiteInfo
 from hopp.simulation.technologies.power_source import PowerSource
 from hopp.simulation.base import BaseClass
 from hopp.simulation.technologies.financial import FinancialModelType, CustomFinancialModel
 from hopp.type_dec import NDArrayFloat
 from hopp.utilities.validators import gt_zero
+from hopp.utilities.log import hybrid_logger as logger
 
+if TYPE_CHECKING:
+    from hopp.simulation.technologies.dispatch.hybrid_dispatch_options import HybridDispatchOptions
 
 @define
 class GridConfig(BaseClass):
     """
     Configuration data class for Grid. 
 
     Args:
@@ -87,15 +90,16 @@
     def simulate_grid_connection(
         # TODO: update args to use numpy types, once PowerSource is refactored
         self,
         hybrid_size_kw: float, 
         total_gen: Union[List[float], NDArrayFloat], 
         project_life: int, 
         lifetime_sim: bool, 
-        total_gen_max_feasible_year1: Union[List[float], NDArrayFloat]
+        total_gen_max_feasible_year1: Union[List[float], NDArrayFloat],
+        dispatch_options: Optional["HybridDispatchOptions"] = None
     ):
         """
         Sets up and simulates hybrid system grid connection. Additionally,
         calculates missed load and curtailment (due to schedule) when a
         desired load is provided.
 
         Args:
@@ -104,14 +108,16 @@
             project_life: Number of year in the analysis period (expected project
                 lifetime) [years]
             lifetime_sim: For simulation modules which support simulating each year of
                 the project_life, whether or not to do so; otherwise the first year
                 data is repeated
             total_gen_max_feasible_year1: Maximum generation profile of the hybrid
                 system (for capacity payments) [kWh]
+            dispatch_options: Hybrid dispatch options class, deliminates if the higher
+                power analysis for frequency regulation is run
 
         """
         if self.site.follow_desired_schedule:
             # Desired schedule sets the upper bound of the system output, any over generation is curtailed
             lifetime_schedule: NDArrayFloat = np.tile([
                 x * 1e3 for x in self.site.desired_schedule],
                 int(project_life / (len(self.site.desired_schedule) // self.site.n_timesteps))
@@ -121,16 +127,73 @@
             self.missed_load = np.array([schedule - gen if gen > 0 else schedule for (schedule, gen) in
                                      zip(lifetime_schedule, self.generation_profile)])
             self.missed_load_percentage = sum(self.missed_load)/sum(lifetime_schedule)
 
             self.schedule_curtailed = np.array([gen - schedule if gen > schedule else 0. for (gen, schedule) in
                                             zip(total_gen, lifetime_schedule)])
             self.schedule_curtailed_percentage = sum(self.schedule_curtailed)/sum(lifetime_schedule)
+
+            # NOTE: This is currently only happening for load following, would be good to make it more general
+            #           i.e. so that this analysis can be used when load following isn't being used (without storage)
+            #           for comparison 
+            N_hybrid = len(self.generation_profile)
+
+            final_power_production = total_gen
+            schedule = [x for x in lifetime_schedule]
+            hybrid_power = [(final_power_production[x] - (schedule[x]*0.95)) for x in range(len(final_power_production))]
+
+            load_met = len([i for i in hybrid_power if i  >= 0])
+            self.time_load_met = 100 * load_met/N_hybrid
+
+            final_power_array = np.array(final_power_production)
+            power_met = np.where(final_power_array > schedule, schedule, final_power_array)
+            self.capacity_factor_load = np.sum(power_met) / np.sum(schedule) * 100
+
+            logger.info('Percent of time firm power requirement is met: ', np.round(self.time_load_met,2))
+            logger.info('Percent total firm power requirement is satisfied: ', np.round(self.capacity_factor_load,2))
+
+            ERS_keys = ['min_regulation_hours', 'min_regulation_power']
+            if dispatch_options is not None and dispatch_options.use_higher_hours:
+                """
+                Frequency regulation analysis for providing essential reliability services (ERS) availability operating case:
+                        Finds how many hours (in the group specified group size above the specified minimum
+                        power requirement) that the system has available to extra power that could be used to 
+                        provide ERS
+                Args:
+                    :param dispatch_options: need additional ERS arguments
+                                        'min_regulation_hours': minimum size of hours in a group to be considered for ERS (>= 1)
+                                        'min_regulation_power': minimum power available over the whole group of hours to be 
+                                                considered for ERS (> 0, in kW)
+
+                :returns: total_number_hours
+
+                """
+
+                # Performing frequency regulation analysis:
+                #    finding how many groups of hours satisfiy the ERS minimum power requirement
+                min_regulation_hours = dispatch_options.higher_hours['min_regulation_hours']
+                min_regulation_power = dispatch_options.higher_hours['min_regulation_power']
+
+                frequency_power_array = np.array(hybrid_power)
+                frequency_test = np.where(frequency_power_array > min_regulation_power, frequency_power_array, 0)
+                mask = (frequency_test!=0).astype(int)
+                padded_mask = np.pad(mask,(1,), "constant")
+                edge_mask = padded_mask[1:] - padded_mask[:-1]  # finding the difference between each array value
+
+                group_starts = np.where(edge_mask == 1)[0]
+                group_stops = np.where(edge_mask == -1)[0]
+
+                # Find groups and drop groups that are too small
+                groups = [group for group in zip(group_starts,group_stops) if ((group[1]-group[0]) >= min_regulation_hours)]
+                group_lengths = [len(final_power_production[group[0]:group[1]]) for group in groups]
+                self.total_number_hours = sum(group_lengths)
+
+                logger.info('Total number of hours available for ERS: ', np.round(self.total_number_hours,2))
         else:
-            self.generation_profile = list(total_gen)
+            self.generation_profile = total_gen
 
         self.total_gen_max_feasible_year1 = np.array(total_gen_max_feasible_year1)
         self.system_capacity_kw = hybrid_size_kw  # TODO: Should this be interconnection limit?
         self.gen_max_feasible = list(np.minimum(  # TODO: remove list() cast once parent class uses numpy 
             total_gen_max_feasible_year1, 
             self.interconnect_kw * self.site.interval / 60
         ))
```

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/hydrogen/electrolysis/PEM_H2_LT_electrolyzer.py` & `HOPP-2.2.0/hopp/simulation/technologies/hydrogen/electrolysis/PEM_H2_LT_electrolyzer.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/hydrogen/electrolysis/PEM_H2_LT_electrolyzer_Clusters.py` & `HOPP-2.2.0/hopp/simulation/technologies/hydrogen/electrolysis/PEM_H2_LT_electrolyzer_Clusters.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/hydrogen/electrolysis/PEM_costs_Singlitico_model.py` & `HOPP-2.2.0/hopp/simulation/technologies/hydrogen/electrolysis/PEM_costs_Singlitico_model.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/hydrogen/electrolysis/PEM_electrolyzer_IVcurve.py` & `HOPP-2.2.0/hopp/simulation/technologies/hydrogen/electrolysis/PEM_electrolyzer_IVcurve.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/hydrogen/electrolysis/optimization_utils_linear.py` & `HOPP-2.2.0/hopp/simulation/technologies/hydrogen/electrolysis/optimization_utils_linear.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/hydrogen/electrolysis/pem_mass_and_footprint.py` & `HOPP-2.2.0/hopp/simulation/technologies/hydrogen/electrolysis/pem_mass_and_footprint.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/hydrogen/electrolysis/run_PEM_master.py` & `HOPP-2.2.0/hopp/simulation/technologies/hydrogen/electrolysis/run_PEM_master.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/hydrogen/electrolysis/run_h2_PEM.py` & `HOPP-2.2.0/hopp/simulation/technologies/hydrogen/electrolysis/run_h2_PEM.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/hydrogen/electrolysis/run_h2_clusters.py` & `HOPP-2.2.0/hopp/simulation/technologies/hydrogen/electrolysis/run_h2_clusters.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/hydrogen/h2_storage/on_turbine/on_turbine_hydrogen_storage.py` & `HOPP-2.2.0/hopp/simulation/technologies/hydrogen/h2_storage/on_turbine/on_turbine_hydrogen_storage.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/hydrogen/h2_storage/pipe_storage/underground_pipe_storage.py` & `HOPP-2.2.0/hopp/simulation/technologies/hydrogen/h2_storage/pipe_storage/underground_pipe_storage.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/hydrogen/h2_storage/pressure_vessel/compressed_gas_storage_model_20221021/Compressed_all.py` & `HOPP-2.2.0/hopp/simulation/technologies/hydrogen/h2_storage/pressure_vessel/compressed_gas_storage_model_20221021/Compressed_all.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/hydrogen/h2_storage/pressure_vessel/compressed_gas_storage_model_20221021/Compressed_gas_function.py` & `HOPP-2.2.0/hopp/simulation/technologies/hydrogen/h2_storage/pressure_vessel/compressed_gas_storage_model_20221021/Compressed_gas_function.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/hydrogen/h2_storage/pressure_vessel/tankinator.py` & `HOPP-2.2.0/hopp/simulation/technologies/hydrogen/h2_storage/pressure_vessel/tankinator.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/hydrogen/h2_storage/pressure_vessel/von_mises.py` & `HOPP-2.2.0/hopp/simulation/technologies/hydrogen/h2_storage/pressure_vessel/von_mises.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/layout/__init__.py` & `HOPP-2.2.0/hopp/simulation/technologies/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/layout/flicker_mismatch.py` & `HOPP-2.2.0/hopp/simulation/technologies/layout/flicker_mismatch.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/layout/flicker_mismatch_grid.py` & `HOPP-2.2.0/hopp/simulation/technologies/layout/flicker_mismatch_grid.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/layout/hybrid_layout.py` & `HOPP-2.2.0/hopp/simulation/technologies/layout/hybrid_layout.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/layout/layout_tools.py` & `HOPP-2.2.0/hopp/simulation/technologies/layout/layout_tools.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/layout/pv_design_utils.py` & `HOPP-2.2.0/hopp/simulation/technologies/layout/pv_design_utils.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/layout/pv_inverter.py` & `HOPP-2.2.0/hopp/simulation/technologies/layout/pv_inverter.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/layout/pv_layout.py` & `HOPP-2.2.0/hopp/simulation/technologies/layout/pv_layout.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/layout/pv_layout_tools.py` & `HOPP-2.2.0/hopp/simulation/technologies/layout/pv_layout_tools.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/layout/pv_module.py` & `HOPP-2.2.0/hopp/simulation/technologies/layout/pv_module.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/layout/shadow_flicker.py` & `HOPP-2.2.0/hopp/simulation/technologies/layout/shadow_flicker.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/layout/simple_flicker.py` & `HOPP-2.2.0/hopp/simulation/technologies/layout/simple_flicker.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/layout/wind_layout.py` & `HOPP-2.2.0/hopp/simulation/technologies/layout/wind_layout.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/layout/wind_layout_tools.py` & `HOPP-2.2.0/hopp/simulation/technologies/layout/wind_layout_tools.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/power_source.py` & `HOPP-2.2.0/hopp/simulation/technologies/power_source.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/pv/detailed_pv_plant.py` & `HOPP-2.2.0/hopp/simulation/technologies/pv/detailed_pv_plant.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/pv/pv_plant.py` & `HOPP-2.2.0/hopp/simulation/technologies/pv/pv_plant.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/reopt.py` & `HOPP-2.2.0/hopp/simulation/technologies/reopt.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/resource/elec_prices.py` & `HOPP-2.2.0/hopp/simulation/technologies/resource/elec_prices.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/resource/resource.py` & `HOPP-2.2.0/hopp/simulation/technologies/resource/resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,14 @@
         # generic api settings
         self.interval = str(int(8760/365/24 * 60))
         self.leap_year = 'false'
         self.utc = 'false'
         self.name = 'hybrid-systems'
         self.affiliation = 'NREL'
         self.reason = 'hybrid-analysis'
-        self.email = 'nicholas.diorio@nrel.gov'
         self.mailing_list = 'true'
 
         # paths
         self.path_current = os.path.dirname(os.path.abspath(__file__))
         self.path_resource = os.path.join(self.path_current, '../..', 'resource_files')
 
         # update any passed in
```

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/resource/solar_resource.py` & `HOPP-2.2.0/hopp/simulation/technologies/resource/solar_resource.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from collections import defaultdict
 from pathlib import Path
 from typing import Union
 import numpy as np
 import csv
 from PySAM.ResourceTools import SAM_CSV_to_solar_data
 
-from hopp.utilities.keys import get_developer_nrel_gov_key
+from hopp.utilities.keys import get_developer_nrel_gov_key, get_developer_nrel_gov_email
 from hopp.utilities.log import hybrid_logger as logger
 from hopp.simulation.technologies.resource.resource import Resource
 from hopp import ROOT_DIR
 
 
 BASE_URL = "https://developer.nrel.gov/api/nsrdb/v2/solar/psm3-download.csv"
 
@@ -67,15 +67,15 @@
         self.format_data()
 
         logger.info("SolarResource: {}".format(self.filename))
 
     def download_resource(self):
         url = '{base}?wkt=POINT({lon}+{lat})&names={year}&leap_day={leap}&interval={interval}&utc={utc}&full_name={name}&email={email}&affiliation={affiliation}&mailing_list={mailing_list}&reason={reason}&api_key={api}&attributes={attr}'.format(
             base=BASE_URL, year=self.year, lat=self.latitude, lon=self.longitude, leap=self.leap_year, interval=self.interval,
-            utc=self.utc, name=self.name, email=self.email,
+            utc=self.utc, name=self.name, email=get_developer_nrel_gov_email(),
             mailing_list=self.mailing_list, affiliation=self.affiliation, reason=self.reason, api=get_developer_nrel_gov_key(),
             attr=self.solar_attributes)
 
         success = self.call_api(url, filename=self.filename)
 
         return success
```

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/resource/wave_resource.py` & `HOPP-2.2.0/hopp/simulation/technologies/resource/wave_resource.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/resource/wind_resource.py` & `HOPP-2.2.0/hopp/simulation/technologies/resource/wind_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import csv, os
 from pathlib import Path
 from typing import Union
 from PySAM.ResourceTools import SRW_to_wind_data
 
-from hopp.utilities.keys import get_developer_nrel_gov_key
+from hopp.utilities.keys import get_developer_nrel_gov_key, get_developer_nrel_gov_email
 from hopp.simulation.technologies.resource.resource import Resource
 from hopp import ROOT_DIR
 
 
 WTK_BASE_URL = "https://developer.nrel.gov/api/wind-toolkit/v2/wind/wtk-srw-download"
 TAP_BASE_URL = "https://dw-tap.nrel.gov/v2/srw"
 
@@ -117,15 +117,15 @@
         success = False
 
         for height, f in self.file_resource_heights.items():
             url = ""
 
             if self.source == "WTK":
                 url = '{base}?year={year}&lat={lat}&lon={lon}&hubheight={hubheight}&api_key={api_key}&email={email}'.format(
-                    base=WTK_BASE_URL, year=self.year, lat=self.latitude, lon=self.longitude, hubheight=height, api_key=get_developer_nrel_gov_key(), email=self.email
+                    base=WTK_BASE_URL, year=self.year, lat=self.latitude, lon=self.longitude, hubheight=height, api_key=get_developer_nrel_gov_key(), email=get_developer_nrel_gov_email()
                 )
             elif self.source == "TAP":
                 url = '{base}?height={hubheight}m&lat={lat}&lon={lon}&year={year}'.format(
                     base=TAP_BASE_URL, year=self.year, lat=self.latitude, lon=self.longitude, hubheight=height
                 )
 
             success = self.call_api(url, filename=f)
```

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/run_power_losses.py` & `HOPP-2.2.0/hopp/simulation/technologies/run_power_losses.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/sites/circular_site.py` & `HOPP-2.2.0/hopp/simulation/technologies/sites/circular_site.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/sites/flatirons_site.py` & `HOPP-2.2.0/hopp/simulation/technologies/sites/flatirons_site.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/sites/irregular_site.py` & `HOPP-2.2.0/hopp/simulation/technologies/sites/irregular_site.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/sites/site_info.py` & `HOPP-2.2.0/hopp/simulation/technologies/sites/site_info.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/utility_rate.py` & `HOPP-2.2.0/hopp/simulation/technologies/utility_rate.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/wave/mhk_wave_plant.py` & `HOPP-2.2.0/hopp/simulation/technologies/wave/mhk_wave_plant.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/wind/floris.py` & `HOPP-2.2.0/hopp/simulation/technologies/wind/floris.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/simulation/technologies/wind/wind_plant.py` & `HOPP-2.2.0/hopp/simulation/technologies/wind/wind_plant.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/tools/analysis/bos/atb_lookup.py` & `HOPP-2.2.0/hopp/tools/analysis/bos/atb_lookup.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/tools/analysis/bos/bos_lookup.py` & `HOPP-2.2.0/hopp/tools/analysis/bos/bos_lookup.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/tools/analysis/bos/bos_model.py` & `HOPP-2.2.0/hopp/tools/analysis/bos/bos_model.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/tools/analysis/bos/cost_calculator.py` & `HOPP-2.2.0/hopp/tools/analysis/bos/cost_calculator.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/tools/analysis/bos/hybrid_bosse.py` & `HOPP-2.2.0/hopp/tools/analysis/bos/hybrid_bosse.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/tools/analysis/bos/hybridbosse_client.py` & `HOPP-2.2.0/hopp/tools/analysis/bos/hybridbosse_client.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/tools/analysis/determine_curtailment.py` & `HOPP-2.2.0/hopp/tools/analysis/determine_curtailment.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/tools/dispatch/csp_pv_battery_plot.py` & `HOPP-2.2.0/hopp/tools/dispatch/csp_pv_battery_plot.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/tools/dispatch/plot_tools.py` & `HOPP-2.2.0/hopp/tools/dispatch/plot_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -299,14 +299,21 @@
     plt.bar(time, discharge, width=0.9, color=discharge_color, edgecolor='white', label='Battery Discharge')
     plt.bar(time, charge, width=0.9, color=charge_color, edgecolor='white', label='Battery Charge')
     plt.xlim([start, end])
     ax = plt.gca()
     ax.xaxis.set_ticks(list(range(start, end, hybrid.site.n_periods_per_day)))
     plt.grid()
     ax1 = plt.gca()
+
+    # Load following, if applicable
+    if hybrid.site.follow_desired_schedule:
+        desired_load = [p for p in hybrid.site.desired_schedule[time_slice]]
+        ax1.plot(time, desired_load, 'b--', label='Desired Load')
+        ax1.set_ylabel('Desired Load', fontsize=font_size)
+
     ax1.legend(fontsize=font_size-2, loc='upper left')
     ax1.set_ylabel('Power (MW)', fontsize=font_size)
 
     ax2 = ax1.twinx()
     ax2.plot(time, hybrid.battery.outputs.SOC[time_slice], 'k', label='State-of-Charge')
     ax2.plot(time, hybrid.battery.outputs.dispatch_SOC[time_slice], '.', label='Dispatch')
     ax2.set_ylabel('State-of-Charge (-)', fontsize=font_size)
@@ -331,14 +338,17 @@
     price = [p * hybrid.ppa_price[0] for p in hybrid.site.elec_prices.data[time_slice]]
     ax2.plot(time, price, color=price_color, label='Price')
     ax2.set_ylabel('Grid Price ($/kWh)', fontsize=font_size)
     ax2.legend(fontsize=font_size-2, loc='upper right')
     plt.xlabel('Time (hours)', fontsize=font_size)
     plt.title('Net Generation', fontsize=font_size)
 
+
+    plt.xlabel('Time (hours)', fontsize=font_size)
+    plt.title('Net Generation', fontsize=font_size)
     plt.tight_layout()
 
     if plot_filename is not None:
         plt.savefig(plot_filename)
         plt.close()
     else:
         plt.show()
```

### Comparing `HOPP-2.1.0/hopp/tools/layout/plot_tools.py` & `HOPP-2.2.0/hopp/tools/layout/plot_tools.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/tools/optimization/candidate_converter/candidate_converter.py` & `HOPP-2.2.0/hopp/tools/optimization/candidate_converter/candidate_converter.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/tools/optimization/candidate_converter/dict_converter.py` & `HOPP-2.2.0/hopp/tools/optimization/candidate_converter/dict_converter.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/tools/optimization/candidate_converter/object_converter.py` & `HOPP-2.2.0/hopp/tools/optimization/candidate_converter/object_converter.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/tools/optimization/candidate_converter/passthrough_converter.py` & `HOPP-2.2.0/hopp/tools/optimization/candidate_converter/passthrough_converter.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/tools/optimization/command_line_tools/config_tools.py` & `HOPP-2.2.0/hopp/tools/optimization/command_line_tools/config_tools.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/tools/optimization/command_line_tools/run_utils.py` & `HOPP-2.2.0/hopp/tools/optimization/command_line_tools/run_utils.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/tools/optimization/data_logging/JSON_lines_record_logger.py` & `HOPP-2.2.0/hopp/tools/optimization/data_logging/JSON_lines_record_logger.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/tools/optimization/data_logging/a_data_recorder.py` & `HOPP-2.2.0/hopp/tools/optimization/data_logging/a_data_recorder.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/tools/optimization/data_logging/data_recorder.py` & `HOPP-2.2.0/hopp/tools/optimization/data_logging/data_recorder.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/tools/optimization/data_logging/null_data_recorder.py` & `HOPP-2.2.0/hopp/tools/optimization/data_logging/null_data_recorder.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/tools/optimization/data_logging/record_logger.py` & `HOPP-2.2.0/hopp/tools/optimization/data_logging/record_logger.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/tools/optimization/data_logging/table_data_recorder.py` & `HOPP-2.2.0/hopp/tools/optimization/data_logging/table_data_recorder.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/tools/optimization/driver/ask_tell_driver.py` & `HOPP-2.2.0/hopp/tools/optimization/driver/ask_tell_driver.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/tools/optimization/driver/ask_tell_parallel_driver.py` & `HOPP-2.2.0/hopp/tools/optimization/driver/ask_tell_parallel_driver.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/tools/optimization/driver/ask_tell_parallel_driver_fns.py` & `HOPP-2.2.0/hopp/tools/optimization/driver/ask_tell_parallel_driver_fns.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/tools/optimization/driver/ask_tell_serial_driver.py` & `HOPP-2.2.0/hopp/tools/optimization/driver/ask_tell_serial_driver.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/tools/optimization/optimization_driver.py` & `HOPP-2.2.0/hopp/tools/optimization/optimization_driver.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/tools/optimization/optimization_problem.py` & `HOPP-2.2.0/hopp/tools/optimization/optimization_problem.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/tools/optimization/optimizer/CEM_optimizer.py` & `HOPP-2.2.0/hopp/tools/optimization/optimizer/CEM_optimizer.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/tools/optimization/optimizer/CMA_ES_optimizer.py` & `HOPP-2.2.0/hopp/tools/optimization/optimizer/CMA_ES_optimizer.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/tools/optimization/optimizer/DCEM_optimizer.py` & `HOPP-2.2.0/hopp/tools/optimization/optimizer/DCEM_optimizer.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/tools/optimization/optimizer/GA_optimizer.py` & `HOPP-2.2.0/hopp/tools/optimization/optimizer/GA_optimizer.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/tools/optimization/optimizer/IDCEM.py` & `HOPP-2.2.0/hopp/tools/optimization/optimizer/IDCEM.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/tools/optimization/optimizer/IPDCEM.py` & `HOPP-2.2.0/hopp/tools/optimization/optimizer/IPDCEM.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/tools/optimization/optimizer/IWDCEM.py` & `HOPP-2.2.0/hopp/tools/optimization/optimizer/IWDCEM.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/tools/optimization/optimizer/KFDCEM.py` & `HOPP-2.2.0/hopp/tools/optimization/optimizer/KFDCEM.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/tools/optimization/optimizer/SPSA_optimizer.py` & `HOPP-2.2.0/hopp/tools/optimization/optimizer/SPSA_optimizer.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/tools/optimization/optimizer/ask_tell_optimizer.py` & `HOPP-2.2.0/hopp/tools/optimization/optimizer/ask_tell_optimizer.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/tools/optimization/optimizer/particle_gradient_optimizer.py` & `HOPP-2.2.0/hopp/tools/optimization/optimizer/particle_gradient_optimizer.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/tools/optimization/optimizer/stationary_optimizer.py` & `HOPP-2.2.0/hopp/tools/optimization/optimizer/stationary_optimizer.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/tools/optimization/problem_parametrization.py` & `HOPP-2.2.0/hopp/tools/optimization/problem_parametrization.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/tools/resource/download_resource.py` & `HOPP-2.2.0/hopp/tools/resource/download_resource.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/tools/resource/resource_loader/resource_loader_files.py` & `HOPP-2.2.0/hopp/tools/resource/resource_loader/resource_loader_files.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/tools/resource/resource_loader/site_details_creator.py` & `HOPP-2.2.0/hopp/tools/resource/resource_loader/site_details_creator.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/tools/resource/resource_tools.py` & `HOPP-2.2.0/hopp/tools/resource/resource_tools.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/tools/utils.py` & `HOPP-2.2.0/hopp/tools/utils.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/type_dec.py` & `HOPP-2.2.0/hopp/type_dec.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/utilities/keys.py` & `HOPP-2.2.0/hopp/utilities/keys.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,48 @@
 from dotenv import load_dotenv, find_dotenv
 import os
 
 developer_nrel_gov_key = ""
+developer_nrel_gov_email = ""
 
 
 def set_developer_nrel_gov_key(key: str):
     global developer_nrel_gov_key
     developer_nrel_gov_key = key
-
+def set_developer_nrel_gov_email(email: str):
+    global developer_nrel_gov_email
+    developer_nrel_gov_email = email
 
 def get_developer_nrel_gov_key():
     global developer_nrel_gov_key
     if developer_nrel_gov_key is None or len(developer_nrel_gov_key) != 40:
         raise ValueError("Please provide NREL Developer key using `set_developer_nrel_gov_key`"
                          "(`from hopp.utilities.keys import set_developer_nrel_gov_key`) \n"
                          " Ensure your Developer key is set either as a `NREL_API_KEY` Environment Variable or"
                          " using the .env file method. For details on setting up .env, "
                          "please see Section 7 of 'Installing from Source' or "
                          "Section 2 of 'Installing from Package Repositories' in the README.md")
     return developer_nrel_gov_key
 
+def get_developer_nrel_gov_email():
+    global developer_nrel_gov_email
+    if developer_nrel_gov_email is None:
+        raise ValueError("Please provide NREL Developer email using `set_developer_nrel_gov_email`"
+                         "(`from hopp.utilities.keys import set_developer_nrel_gov_email`) \n"
+                         " Ensure your Developer email is set either as a `EMAIL` Environment Variable or"
+                         " using the .env file method. For details on setting up .env, "
+                         "please see Section 7 of 'Installing from Source' or "
+                         "Section 2 of 'Installing from Package Repositories' in the README.md")
+    return developer_nrel_gov_email
 
 def set_nrel_key_dot_env(path=None):
     if path and os.path.exists(path):
         load_dotenv(path)
     else:
         r = find_dotenv(usecwd=True)
         load_dotenv(r)
     NREL_API_KEY = os.getenv("NREL_API_KEY")
+    NREL_API_EMAIL = os.getenv("NREL_API_EMAIL")
     if NREL_API_KEY is not None:
         set_developer_nrel_gov_key(NREL_API_KEY)
+    if NREL_API_EMAIL is not None:
+        set_developer_nrel_gov_email(NREL_API_EMAIL)
```

### Comparing `HOPP-2.1.0/hopp/utilities/log.py` & `HOPP-2.2.0/hopp/utilities/log.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/utilities/utilities.py` & `HOPP-2.2.0/hopp/utilities/utilities.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/hopp/utilities/validators.py` & `HOPP-2.2.0/hopp/utilities/validators.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/setup.py` & `HOPP-2.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/tests/hopp/test_battery.py` & `HOPP-2.2.0/tests/hopp/test_battery.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/tests/hopp/test_battery_dispatch.py` & `HOPP-2.2.0/tests/hopp/test_battery_dispatch.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     'batt_bank_replacement': [0],
     'batt_replacement_option': 0,
     'batt_meter_position': 0,
     'om_fixed': [1],
     'om_production': [2],
     'om_capacity': (0,),
     'om_batt_fixed_cost': 0,
-    'om_batt_variable_cost': [0],
+    'om_batt_variable_cost': [0.75],
     'om_batt_capacity_cost': 0,
     'om_batt_replacement_cost': [0],
     'om_replacement_cost_escal': 0,
     'system_use_lifetime_output': 0,
     'inflation_rate': 2.5,
     'real_discount_rate': 6.4,
     'cp_capacity_credit_percent': [0],
```

### Comparing `HOPP-2.1.0/tests/hopp/test_battery_stateless.py` & `HOPP-2.2.0/tests/hopp/test_battery_stateless.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/tests/hopp/test_clustering.py` & `HOPP-2.2.0/tests/hopp/test_clustering.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/tests/hopp/test_cost_calculator.py` & `HOPP-2.2.0/tests/hopp/test_cost_calculator.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/tests/hopp/test_csp.py` & `HOPP-2.2.0/tests/hopp/test_csp.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/tests/hopp/test_custom_financial.py` & `HOPP-2.2.0/tests/hopp/test_custom_financial.py`

 * *Files 1% similar despite different names*

```diff
@@ -298,14 +298,15 @@
         "site": site,
         "technologies": power_sources
     }
     hi = HoppInterface(hopp_config)
     hybrid_plant = hi.system
     hybrid_plant.layout.plot()
     hybrid_plant.battery.dispatch.lifecycle_cost_per_kWh_cycle = 0.01
+    hybrid_plant.battery._financial_model.om_batt_variable_cost = [0.75]
 
     hybrid_plant.simulate()
 
     sizes = hybrid_plant.system_capacity_kw
     aeps = hybrid_plant.annual_energies
     npvs = hybrid_plant.net_present_values
     assert sizes.pv == approx(pv_kw, 1e-3)
@@ -387,14 +388,15 @@
         "site": site,
         "technologies": power_sources
     } 
     hi = HoppInterface(hopp_config)
     hybrid_plant = hi.system
     hybrid_plant.layout.plot()
     hybrid_plant.battery.dispatch.lifecycle_cost_per_kWh_cycle = 0.01
+    hybrid_plant.battery._financial_model.om_batt_variable_cost = [0.75]
 
     hybrid_plant.simulate()
 
     sizes = hybrid_plant.system_capacity_kw
     aeps = hybrid_plant.annual_energies
     npvs = hybrid_plant.net_present_values
     assert sizes.pv == approx(10000, 1e-3)
```

### Comparing `HOPP-2.1.0/tests/hopp/test_detailed_pv_plant.py` & `HOPP-2.2.0/tests/hopp/test_detailed_pv_plant.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/tests/hopp/test_dispatch.py` & `HOPP-2.2.0/tests/hopp/test_dispatch.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pytest
 import pyomo.environ as pyomo
 from pyomo.environ import units as u
 from pyomo.opt import TerminationCondition
 from pyomo.util.check_units import assert_units_consistent
 
 from hopp.simulation import HoppInterface
-from hopp.simulation.technologies.sites import SiteInfo
+from hopp.simulation.technologies.sites import SiteInfo, flatirons_site
 from hopp.simulation.technologies.financial.custom_financial_model import CustomFinancialModel
 from hopp.simulation.technologies.wind.wind_plant import WindPlant, WindConfig
 from hopp.simulation.technologies.pv.pv_plant import PVPlant, PVConfig
 from hopp.simulation.technologies.csp.tower_plant import TowerPlant, TowerConfig
 from hopp.simulation.technologies.csp.trough_plant import TroughPlant, TroughConfig
 from hopp.simulation.technologies.wave.mhk_wave_plant import MHKWavePlant, MHKConfig
 from hopp.simulation.technologies.financial.mhk_cost_model import MHKCostModelInputs
@@ -479,15 +479,15 @@
     available_resource = wind.generation_profile[0:dispatch_n_look_ahead]
     dispatch_generation = wind.dispatch.generation
     for t in model.forecast_horizon:
         assert dispatch_generation[t] * 1e3 == pytest.approx(available_resource[t], 1e-3)
 
 
 def test_simple_battery_dispatch(site):
-    expected_objective = 28957.15
+    expected_objective = 29678.62
     dispatch_n_look_ahead = 48
 
     config = BatteryConfig.from_dict(technologies['battery'])
     battery = Battery(site, config=config)
 
     model = pyomo.ConcreteModel(name='battery_only')
     model.forecast_horizon = pyomo.Set(initialize=range(dispatch_n_look_ahead))
@@ -543,15 +543,15 @@
     battery.simulate_with_dispatch(48, 0)
     for i in range(24):
         dispatch_power = battery.dispatch.power[i] * 1e3
         assert battery.outputs.P[i] == pytest.approx(dispatch_power, 1e-3 * abs(dispatch_power))
 
 
 def test_simple_battery_dispatch_lifecycle_count(site):
-    expected_objective = 23657
+    expected_objective = 24378.6
     expected_lifecycles = [0.75048, 1.50096]
 
     dispatch_n_look_ahead = 48
 
     config = BatteryConfig.from_dict(technologies['battery'])
     battery = Battery(site, config=config)
 
@@ -608,15 +608,15 @@
     assert sum(battery.dispatch.charge_power) > 0.0
     assert sum(battery.dispatch.discharge_power) > 0.0
     assert (sum(battery.dispatch.charge_power) * battery.dispatch.round_trip_efficiency / 100.0
             == pytest.approx(sum(battery.dispatch.discharge_power)))
 
 
 def test_detailed_battery_dispatch(site):
-    expected_objective = 33508
+    expected_objective = 34505.9
     expected_lifecycles =  [0.14300, 0.22169]
     # TODO: McCormick error is large enough to make objective 50% higher than
     #  the value of simple battery dispatch objective
 
     dispatch_n_look_ahead = 48
 
     config = BatteryConfig.from_dict(technologies['battery'])
@@ -678,15 +678,15 @@
     assert sum(battery.dispatch.discharge_power) > 0.0
     assert sum(battery.dispatch.charge_current) >= sum(battery.dispatch.discharge_current) - 1e-7
     # assert sum(battery.dispatch.charge_power) > sum(battery.dispatch.discharge_power)
     # TODO: model cheats too much where last test fails
 
 
 def test_pv_wind_battery_hybrid_dispatch(site):
-    expected_objective = 38777.757
+    expected_objective = 39005
 
     wind_solar_battery = {key: technologies[key] for key in ('pv', 'wind', 'battery', 'grid')}
     hopp_config = {
         "site": site,
         "technologies": wind_solar_battery,
         "config": {
             "dispatch_options": {
@@ -780,15 +780,15 @@
 
     hi.simulate(1)
 
     assert sum(hybrid_plant.battery.outputs.P) < 0.0
     
 
 def test_hybrid_solar_battery_dispatch(site):
-    expected_objective = 23474
+    expected_objective = 24029
 
     solar_battery_technologies = {k: technologies[k] for k in ('pv', 'battery', 'grid')}
     hopp_config = {
         "site": site,
         "technologies": solar_battery_technologies,
         "config": {
             "dispatch_options": {'grid_charging': False}
@@ -925,15 +925,15 @@
 
     # CSP can run
     assert sum(hybrid_plant.tower.dispatch.cycle_generation) > 0.0
     assert sum(hybrid_plant.tower.dispatch.receiver_thermal_power) > 0.0
 
 
 def test_simple_battery_dispatch_lifecycle_limit(site):
-    expected_objective = 7561
+    expected_objective = 7882
     max_lifecycle_per_day = 0.5
 
     dispatch_n_look_ahead = 48
 
     config = BatteryConfig.from_dict(technologies['battery'])
     battery = Battery(site, config=config)
 
@@ -988,7 +988,39 @@
     assert pyomo.value(battery.dispatch.lifecycles[0]) == pytest.approx(max_lifecycle_per_day, 1e-3)
     assert pyomo.value(battery.dispatch.lifecycles[1]) == pytest.approx(max_lifecycle_per_day, 1e-3)
 
     assert sum(battery.dispatch.charge_power) > 0.0
     assert sum(battery.dispatch.discharge_power) > 0.0
     assert (sum(battery.dispatch.charge_power) * battery.dispatch.round_trip_efficiency / 100.0
             == pytest.approx(sum(battery.dispatch.discharge_power)))
+
+
+def test_hybrid_dispatch_baseload_heuristic_and_analysis(site):
+
+    desired_schedule = 8760*[20]
+
+    desired_schedule_site = SiteInfo(flatirons_site,
+                                     desired_schedule=desired_schedule)
+    wind_solar_battery = {key: technologies[key] for key in ('pv', 'wind', 'battery')}
+
+    dispatch_options = {'battery_dispatch': 'load_following_heuristic',
+                        'use_higher_hours': True, 
+                        'higher_hours': {'min_regulation_hours': 4, 'min_regulation_power': 5000}}
+
+    hopp_config = {
+        "site": desired_schedule_site,
+        "technologies": wind_solar_battery,
+        "config": {
+            "dispatch_options": dispatch_options
+        }
+    }
+    hopp_config["technologies"]["grid"] = {
+        "interconnect_kw": interconnect_mw * 1000
+    }
+    hi = HoppInterface(hopp_config)
+    hi.simulate(1)
+
+    hybrid_plant = hi.system
+
+    assert hybrid_plant.grid.time_load_met == pytest.approx(91.9, 1e-2)
+    assert hybrid_plant.grid.capacity_factor_load == pytest.approx(94.45, 1e-2)
+    assert hybrid_plant.grid.total_number_hours == pytest.approx(3732, 1e-2)
```

### Comparing `HOPP-2.1.0/tests/hopp/test_flicker.py` & `HOPP-2.2.0/tests/hopp/test_flicker.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/tests/hopp/test_flicker_mismatch.py` & `HOPP-2.2.0/tests/hopp/test_flicker_mismatch.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/tests/hopp/test_grid.py` & `HOPP-2.2.0/tests/hopp/test_grid.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/tests/hopp/test_hybrid.py` & `HOPP-2.2.0/tests/hopp/test_hybrid.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,234 +4,378 @@
 from pytest import approx, fixture, raises
 import numpy as np
 import json
 
 from hopp.simulation import HoppInterface
 
 from hopp.simulation.technologies.sites import SiteInfo
-from hopp.simulation.technologies.pv.detailed_pv_plant import DetailedPVPlant, DetailedPVConfig
-from hopp.simulation.technologies.layout.pv_design_utils import size_electrical_parameters
+from hopp.simulation.technologies.pv.detailed_pv_plant import (
+    DetailedPVPlant,
+    DetailedPVConfig,
+)
+from hopp.simulation.technologies.layout.pv_design_utils import (
+    size_electrical_parameters,
+)
 from hopp.simulation.technologies.financial.mhk_cost_model import MHKCostModelInputs
 from tests.hopp.utils import create_default_site_info, DEFAULT_FIN_CONFIG
 from hopp import ROOT_DIR
 from hopp.utilities import load_yaml
 
 
 @fixture
 def hybrid_config():
     """Loads the config YAML and updates site info to use resource files."""
-    hybrid_config_path = ROOT_DIR.parent / "tests" / "hopp" / "inputs" / "hybrid_run.yaml"
+    hybrid_config_path = (
+        ROOT_DIR.parent / "tests" / "hopp" / "inputs" / "hybrid_run.yaml"
+    )
     hybrid_config = load_yaml(hybrid_config_path)
 
     return hybrid_config
 
 
 @fixture
 def site():
     return create_default_site_info()
 
-wave_resource_file = ROOT_DIR.parent / "resource_files" / "wave" / "Wave_resource_timeseries.csv"
+
+wave_resource_file = (
+    ROOT_DIR.parent / "resource_files" / "wave" / "Wave_resource_timeseries.csv"
+)
+
 
 @fixture
 def wavesite():
-    data = {
-        "lat": 44.6899,
-        "lon": 124.1346,
-        "year": 2010,
-        "tz": -7
-    }
+    data = {"lat": 44.6899, "lon": 124.1346, "year": 2010, "tz": -7}
     return SiteInfo(
-        data,
-        wave_resource_file=wave_resource_file, 
-        solar=False, 
-        wind=False, 
-        wave=True
+        data, wave_resource_file=wave_resource_file, solar=False, wind=False, wave=True
     )
 
-mhk_yaml_path = ROOT_DIR.parent / "tests" / "hopp" / "inputs" / "wave" / "wave_device.yaml"
+
+mhk_yaml_path = (
+    ROOT_DIR.parent / "tests" / "hopp" / "inputs" / "wave" / "wave_device.yaml"
+)
 mhk_config = load_yaml(mhk_yaml_path)
 
 interconnection_size_kw = 15000
 pv_kw = 5000
 wind_kw = 10000
 batt_kw = 5000
 
 detailed_pv = {
-    'tech_config': {
-        'system_capacity_kw': pv_kw
-    },
-    'layout_params': {
+    "tech_config": {"system_capacity_kw": pv_kw},
+    "layout_params": {
         "x_position": 0.5,
         "y_position": 0.5,
         "aspect_power": 0,
         "gcr": 0.5,
         "s_buffer": 2,
-        "x_buffer": 2
-    }
+        "x_buffer": 2,
+    },
 }
 # From a Cambium midcase BA10 2030 analysis (Jan 1 = 1):
-capacity_credit_hours_of_year = [4604,4605,4606,4628,4629,4630,4652,4821,5157,5253,
-                                 5254,5277,5278,5299,5300,5301,5302,5321,5323,5324,
-                                 5325,5326,5327,5347,5348,5349,5350,5369,5370,5371,
-                                 5372,5374,5395,5396,5397,5398,5419,5420,5421,5422,
-                                 5443,5444,5445,5446,5467,5468,5469,5493,5494,5517,
-                                 5539,5587,5589,5590,5661,5757,5781,5803,5804,5805,
-                                 5806,5826,5827,5830,5947,5948,5949,5995,5996,5997,
-                                 6019,6090,6091,6092,6093,6139,6140,6141,6163,6164,
-                                 6165,6166,6187,6188,6211,6212,6331,6354,6355,6356,
-                                 6572,6594,6595,6596,6597,6598,6618,6619,6620,6621]
+capacity_credit_hours_of_year = [
+    4604,
+    4605,
+    4606,
+    4628,
+    4629,
+    4630,
+    4652,
+    4821,
+    5157,
+    5253,
+    5254,
+    5277,
+    5278,
+    5299,
+    5300,
+    5301,
+    5302,
+    5321,
+    5323,
+    5324,
+    5325,
+    5326,
+    5327,
+    5347,
+    5348,
+    5349,
+    5350,
+    5369,
+    5370,
+    5371,
+    5372,
+    5374,
+    5395,
+    5396,
+    5397,
+    5398,
+    5419,
+    5420,
+    5421,
+    5422,
+    5443,
+    5444,
+    5445,
+    5446,
+    5467,
+    5468,
+    5469,
+    5493,
+    5494,
+    5517,
+    5539,
+    5587,
+    5589,
+    5590,
+    5661,
+    5757,
+    5781,
+    5803,
+    5804,
+    5805,
+    5806,
+    5826,
+    5827,
+    5830,
+    5947,
+    5948,
+    5949,
+    5995,
+    5996,
+    5997,
+    6019,
+    6090,
+    6091,
+    6092,
+    6093,
+    6139,
+    6140,
+    6141,
+    6163,
+    6164,
+    6165,
+    6166,
+    6187,
+    6188,
+    6211,
+    6212,
+    6331,
+    6354,
+    6355,
+    6356,
+    6572,
+    6594,
+    6595,
+    6596,
+    6597,
+    6598,
+    6618,
+    6619,
+    6620,
+    6621,
+]
 # List length 8760, True if the hour counts for capacity payments, False otherwise
-capacity_credit_hours = [hour in capacity_credit_hours_of_year for hour in range(1,8760+1)]
+capacity_credit_hours = [
+    hour in capacity_credit_hours_of_year for hour in range(1, 8760 + 1)
+]
+
 
 def test_hybrid_wave_only(hybrid_config, wavesite, subtests):
     hybrid_config["site"]["wave"] = True
     hybrid_config["site"]["wave_resource_file"] = wave_resource_file
     wave_only_technologies = {
-        'wave': {
-            'device_rating_kw': mhk_config['device_rating_kw'], 
-            'num_devices': 10, 
-            'wave_power_matrix': mhk_config['wave_power_matrix'],
-            'fin_model': DEFAULT_FIN_CONFIG
+        "wave": {
+            "device_rating_kw": mhk_config["device_rating_kw"],
+            "num_devices": 10,
+            "wave_power_matrix": mhk_config["wave_power_matrix"],
+            "fin_model": DEFAULT_FIN_CONFIG,
+        },
+        "grid": {
+            "interconnect_kw": interconnection_size_kw,
+            "fin_model": DEFAULT_FIN_CONFIG,
         },
-        'grid': {
-            'interconnect_kw': interconnection_size_kw,
-            'fin_model': DEFAULT_FIN_CONFIG,
-        }
     }
 
     hybrid_config["technologies"] = wave_only_technologies
-    
-    # TODO once the financial model is implemented, romove the line immediately following this comment and un-indent the rest of the test    
+
+    # TODO once the financial model is implemented, romove the line immediately following this comment and un-indent the rest of the test
     hi = HoppInterface(hybrid_config)
     hybrid_plant = hi.system
     # hybrid_plant = HybridSimulation(wave_only_technologies, wavesite)
-    cost_model_inputs = MHKCostModelInputs.from_dict({
-        'reference_model_num':3,
-        'water_depth': 100,
-        'distance_to_shore': 80,
-        'number_rows': 10,
-        'device_spacing':600,
-        'row_spacing': 600,
-        'cable_system_overbuild': 20
-	})
+    cost_model_inputs = MHKCostModelInputs.from_dict(
+        {
+            "reference_model_num": 3,
+            "water_depth": 100,
+            "distance_to_shore": 80,
+            "number_rows": 10,
+            "device_spacing": 600,
+            "row_spacing": 600,
+            "cable_system_overbuild": 20,
+        }
+    )
     assert hybrid_plant.wave is not None
     hybrid_plant.wave.create_mhk_cost_calculator(cost_model_inputs)
 
     hi.simulate()
     aeps = hybrid_plant.annual_energies
     npvs = hybrid_plant.net_present_values
     cf = hybrid_plant.capacity_factors
 
     # check that wave and grid match when only wave is in the hybrid system
     with subtests.test("financial parameters"):
-        assert hybrid_plant.wave._financial_model.FinancialParameters == approx(hybrid_plant.grid._financial_model.FinancialParameters)
+        assert hybrid_plant.wave._financial_model.FinancialParameters == approx(
+            hybrid_plant.grid._financial_model.FinancialParameters
+        )
     with subtests.test("Revenue"):
-        assert hybrid_plant.wave._financial_model.Revenue == approx(hybrid_plant.grid._financial_model.Revenue)
+        assert hybrid_plant.wave._financial_model.Revenue == approx(
+            hybrid_plant.grid._financial_model.Revenue
+        )
     with subtests.test("SystemCosts"):
-        assert hybrid_plant.wave._financial_model.SystemCosts == approx(hybrid_plant.grid._financial_model.SystemCosts)
+        assert hybrid_plant.wave._financial_model.SystemCosts == approx(
+            hybrid_plant.grid._financial_model.SystemCosts
+        )
 
     # with subtests.test("SystemOutput.__dict__"):
     #     skip(reason="this test will not be consistent until the code is more type stable. Outputs may be tuple or list")
     #     assert hybrid_plant.wave._financial_model.SystemOutput.__dict__ == hybrid_plant.grid._financial_model.SystemOutput.__dict__
     with subtests.test("SystemOutput.gen"):
-        assert hybrid_plant.wave._financial_model.SystemOutput.gen == approx(hybrid_plant.grid._financial_model.SystemOutput.gen)
+        assert hybrid_plant.wave._financial_model.SystemOutput.gen == approx(
+            hybrid_plant.grid._financial_model.SystemOutput.gen
+        )
     with subtests.test("SystemOutput.system_capacity"):
-        assert hybrid_plant.wave._financial_model.SystemOutput.system_capacity == approx(hybrid_plant.grid._financial_model.SystemOutput.system_capacity)
+        assert (
+            hybrid_plant.wave._financial_model.SystemOutput.system_capacity
+            == approx(hybrid_plant.grid._financial_model.SystemOutput.system_capacity)
+        )
     with subtests.test("SystemOutput.degradation"):
-        assert hybrid_plant.wave._financial_model.SystemOutput.degradation == approx(hybrid_plant.grid._financial_model.SystemOutput.degradation)
+        assert hybrid_plant.wave._financial_model.SystemOutput.degradation == approx(
+            hybrid_plant.grid._financial_model.SystemOutput.degradation
+        )
     with subtests.test("SystemOutput.system_pre_curtailment_kwac"):
-        assert hybrid_plant.wave._financial_model.SystemOutput.system_pre_curtailment_kwac == approx(hybrid_plant.grid._financial_model.SystemOutput.system_pre_curtailment_kwac)
+        assert (
+            hybrid_plant.wave._financial_model.SystemOutput.system_pre_curtailment_kwac
+            == approx(
+                hybrid_plant.grid._financial_model.SystemOutput.system_pre_curtailment_kwac
+            )
+        )
     with subtests.test("SystemOutput.annual_energy_pre_curtailment_ac"):
-        assert hybrid_plant.wave._financial_model.SystemOutput.annual_energy_pre_curtailment_ac == approx(hybrid_plant.grid._financial_model.SystemOutput.annual_energy_pre_curtailment_ac)
+        assert (
+            hybrid_plant.wave._financial_model.SystemOutput.annual_energy_pre_curtailment_ac
+            == approx(
+                hybrid_plant.grid._financial_model.SystemOutput.annual_energy_pre_curtailment_ac
+            )
+        )
 
     with subtests.test("Outputs"):
-        assert hybrid_plant.wave._financial_model.Outputs == approx(hybrid_plant.grid._financial_model.Outputs)
+        assert hybrid_plant.wave._financial_model.Outputs == approx(
+            hybrid_plant.grid._financial_model.Outputs
+        )
     with subtests.test("net cash flow"):
-        wave_period = hybrid_plant.wave._financial_model.value('analysis_period')
-        grid_period = hybrid_plant.grid._financial_model.value('analysis_period')
-        assert hybrid_plant.wave._financial_model.net_cash_flow(wave_period) == approx(hybrid_plant.grid._financial_model.net_cash_flow(grid_period))
-    
+        wave_period = hybrid_plant.wave._financial_model.value("analysis_period")
+        grid_period = hybrid_plant.grid._financial_model.value("analysis_period")
+        assert hybrid_plant.wave._financial_model.net_cash_flow(wave_period) == approx(
+            hybrid_plant.grid._financial_model.net_cash_flow(grid_period)
+        )
+
     with subtests.test("degradation"):
-        assert hybrid_plant.wave._financial_model.value("degradation") == approx(hybrid_plant.grid._financial_model.value("degradation"))
+        assert hybrid_plant.wave._financial_model.value("degradation") == approx(
+            hybrid_plant.grid._financial_model.value("degradation")
+        )
     with subtests.test("total_installed_cost"):
-        assert hybrid_plant.wave._financial_model.value("total_installed_cost") == approx(hybrid_plant.grid._financial_model.value("total_installed_cost"))
+        assert hybrid_plant.wave._financial_model.value(
+            "total_installed_cost"
+        ) == approx(hybrid_plant.grid._financial_model.value("total_installed_cost"))
     with subtests.test("inflation_rate"):
-        assert hybrid_plant.wave._financial_model.value("inflation_rate") == approx(hybrid_plant.grid._financial_model.value("inflation_rate"))
+        assert hybrid_plant.wave._financial_model.value("inflation_rate") == approx(
+            hybrid_plant.grid._financial_model.value("inflation_rate")
+        )
     with subtests.test("annual_energy"):
-        assert hybrid_plant.wave._financial_model.value("annual_energy") == approx(hybrid_plant.grid._financial_model.value("annual_energy"))
+        assert hybrid_plant.wave._financial_model.value("annual_energy") == approx(
+            hybrid_plant.grid._financial_model.value("annual_energy")
+        )
     with subtests.test("ppa_price_input"):
-        assert hybrid_plant.wave._financial_model.value("ppa_price_input") == approx(hybrid_plant.grid._financial_model.value("ppa_price_input"))
+        assert hybrid_plant.wave._financial_model.value("ppa_price_input") == approx(
+            hybrid_plant.grid._financial_model.value("ppa_price_input")
+        )
     with subtests.test("ppa_escalation"):
-        assert hybrid_plant.wave._financial_model.value("ppa_escalation") == approx(hybrid_plant.grid._financial_model.value("ppa_escalation"))
+        assert hybrid_plant.wave._financial_model.value("ppa_escalation") == approx(
+            hybrid_plant.grid._financial_model.value("ppa_escalation")
+        )
 
     # test hybrid outputs
     with subtests.test("wave aep"):
-        assert aeps.wave == approx(12132526.0,1e-2)
+        assert aeps.wave == approx(12132526.0, 1e-2)
     with subtests.test("hybrid wave only aep"):
         assert aeps.hybrid == approx(aeps.wave)
     with subtests.test("wave cf"):
-        assert cf.wave == approx(48.42,1e-2)
+        assert cf.wave == approx(48.42, 1e-2)
     with subtests.test("hybrid wave only cf"):
         assert cf.hybrid == approx(cf.wave)
     with subtests.test("wave npv"):
-        #TODO check/verify this test value somehow, not sure how to do it right now
+        # TODO check/verify this test value somehow, not sure how to do it right now
         assert npvs.wave == approx(-53731805.52113224)
     with subtests.test("hybrid wave only npv"):
         assert npvs.hybrid == approx(npvs.wave)
 
+
 def test_hybrid_wave_battery(hybrid_config, wavesite, subtests):
     hybrid_config["site"]["wave"] = True
     hybrid_config["site"]["wave_resource_file"] = wave_resource_file
     wave_only_technologies = {
-        'wave': {
-            'device_rating_kw': mhk_config['device_rating_kw'], 
-            'num_devices': 10, 
-            'wave_power_matrix': mhk_config['wave_power_matrix'],
-            'fin_model': DEFAULT_FIN_CONFIG
+        "wave": {
+            "device_rating_kw": mhk_config["device_rating_kw"],
+            "num_devices": 10,
+            "wave_power_matrix": mhk_config["wave_power_matrix"],
+            "fin_model": DEFAULT_FIN_CONFIG,
         },
-        'battery': {
-            'system_capacity_kwh': 20000,
-            'system_capacity_kw': 80000,
-            'fin_model': DEFAULT_FIN_CONFIG
+        "battery": {
+            "system_capacity_kwh": 20000,
+            "system_capacity_kw": 80000,
+            "fin_model": DEFAULT_FIN_CONFIG,
+        },
+        "grid": {
+            "interconnect_kw": interconnection_size_kw,
+            "fin_model": DEFAULT_FIN_CONFIG,
         },
-        'grid': {
-            'interconnect_kw': interconnection_size_kw,
-            'fin_model': DEFAULT_FIN_CONFIG,
-        }
     }
 
     hybrid_config["technologies"] = wave_only_technologies
-    
-    # TODO once the financial model is implemented, romove the line immediately following this comment and un-indent the rest of the test    
+
+    # TODO once the financial model is implemented, romove the line immediately following this comment and un-indent the rest of the test
     hi = HoppInterface(hybrid_config)
     hybrid_plant = hi.system
     # hybrid_plant = HybridSimulation(wave_only_technologies, wavesite)
-    cost_model_inputs = MHKCostModelInputs.from_dict({
-        'reference_model_num':3,
-        'water_depth': 100,
-        'distance_to_shore': 80,
-        'number_rows': 10,
-        'device_spacing':600,
-        'row_spacing': 600,
-        'cable_system_overbuild': 20
-	})
+    cost_model_inputs = MHKCostModelInputs.from_dict(
+        {
+            "reference_model_num": 3,
+            "water_depth": 100,
+            "distance_to_shore": 80,
+            "number_rows": 10,
+            "device_spacing": 600,
+            "row_spacing": 600,
+            "cable_system_overbuild": 20,
+        }
+    )
     assert hybrid_plant.wave is not None
     hybrid_plant.wave.create_mhk_cost_calculator(cost_model_inputs)
+    hybrid_plant.battery._financial_model.om_batt_variable_cost = [0.75]
 
     hi.simulate()
     aeps = hybrid_plant.annual_energies
     npvs = hybrid_plant.net_present_values
     cf = hybrid_plant.capacity_factors
 
     with subtests.test("battery aep"):
         assert aeps.battery == approx(87.84, 1e3)
 
+
 def test_hybrid_wind_only(hybrid_config):
     technologies = hybrid_config["technologies"]
-    wind_only = {key: technologies[key] for key in ('wind', 'grid')}
+    wind_only = {key: technologies[key] for key in ("wind", "grid")}
     hybrid_config["technologies"] = wind_only
     hi = HoppInterface(hybrid_config)
     hybrid_plant = hi.system
 
     hi.simulate(25)
 
     aeps = hybrid_plant.annual_energies
@@ -243,15 +387,15 @@
 
     assert npvs.wind == approx(-13692784, 1e3)
     assert npvs.hybrid == approx(-13692784, 1e3)
 
 
 def test_hybrid_pv_only(hybrid_config):
     technologies = hybrid_config["technologies"]
-    solar_only = {key: technologies[key] for key in ('pv', 'grid')}
+    solar_only = {key: technologies[key] for key in ("pv", "grid")}
     hybrid_config["technologies"] = solar_only
     hi = HoppInterface(hybrid_config)
 
     hybrid_plant = hi.system
 
     hi.simulate()
 
@@ -265,65 +409,83 @@
     assert aeps.hybrid == approx(9884106.55, 1e-3)
 
     assert npvs.pv == approx(-5121293, 1e3)
     assert npvs.hybrid == approx(-5121293, 1e3)
 
 
 def test_detailed_pv_system_capacity(hybrid_config, subtests):
-    with subtests.test("Detailed PV model (pvsamv1) using defaults except the top level system_capacity_kw parameter"):
+    with subtests.test(
+        "Detailed PV model (pvsamv1) using defaults except the top level system_capacity_kw parameter"
+    ):
         annual_energy_expected = 11128604
         npv_expected = -2436229
         technologies = hybrid_config["technologies"]
-        solar_only = deepcopy({key: technologies[key] for key in ('pv', 'grid')})   # includes system_capacity_kw parameter
-        solar_only['pv']['use_pvwatts'] = False             # specify detailed PV model but don't change any defaults
-        solar_only['grid']['interconnect_kw'] = 150e3
+        solar_only = deepcopy(
+            {key: technologies[key] for key in ("pv", "grid")}
+        )  # includes system_capacity_kw parameter
+        solar_only["pv"][
+            "use_pvwatts"
+        ] = False  # specify detailed PV model but don't change any defaults
+        solar_only["grid"]["interconnect_kw"] = 150e3
         hybrid_config["technologies"] = solar_only
         hi = HoppInterface(hybrid_config)
         hybrid_plant = hi.system
-        assert hybrid_plant.pv.value('subarray1_nstrings') == 1343
+        assert hybrid_plant.pv.value("subarray1_nstrings") == 1343
         hybrid_plant.layout.plot()
 
         hi.simulate()
 
         aeps = hybrid_plant.annual_energies
         npvs = hybrid_plant.net_present_values
         assert aeps.pv == approx(annual_energy_expected, 1e-3)
         assert aeps.hybrid == approx(annual_energy_expected, 1e-3)
         assert npvs.pv == approx(npv_expected, 1e-3)
         assert npvs.hybrid == approx(npv_expected, 1e-3)
 
-    
-    with subtests.test("Detailed PV model (pvsamv1) using parameters from file except the top level system_capacity_kw parameter"):
-        pvsamv1_defaults_file = Path(__file__).absolute().parent / "pvsamv1_basic_params.json"
-        with open(pvsamv1_defaults_file, 'r') as f:
+    with subtests.test(
+        "Detailed PV model (pvsamv1) using parameters from file except the top level system_capacity_kw parameter"
+    ):
+        pvsamv1_defaults_file = (
+            Path(__file__).absolute().parent / "pvsamv1_basic_params.json"
+        )
+        with open(pvsamv1_defaults_file, "r") as f:
             tech_config = json.load(f)
-        solar_only = deepcopy({key: technologies[key] for key in ('pv', 'grid')})   # includes system_capacity_kw parameter
-        solar_only['pv']['use_pvwatts'] = False             # specify detailed PV model
-        solar_only['pv']['tech_config'] = tech_config       # specify parameters
-        solar_only['grid']['interconnect_kw'] = 150e3
+        solar_only = deepcopy(
+            {key: technologies[key] for key in ("pv", "grid")}
+        )  # includes system_capacity_kw parameter
+        solar_only["pv"]["use_pvwatts"] = False  # specify detailed PV model
+        solar_only["pv"]["tech_config"] = tech_config  # specify parameters
+        solar_only["grid"]["interconnect_kw"] = 150e3
         hybrid_config["technologies"] = solar_only
         with raises(Exception) as context:
             hi = HoppInterface(hybrid_config)
-        assert "The specified system capacity of 5000 kW is more than 5% from the value calculated" in str(context.value)
+        assert (
+            "The specified system capacity of 5000 kW is more than 5% from the value calculated"
+            in str(context.value)
+        )
 
         # Run detailed PV model (pvsamv1) using file parameters, minus the number of strings, and the top level system_capacity_kw parameter
         annual_energy_expected = 8955045
         npv_expected = -2622684
-        pvsamv1_defaults_file = Path(__file__).absolute().parent / "pvsamv1_basic_params.json"
-        with open(pvsamv1_defaults_file, 'r') as f:
+        pvsamv1_defaults_file = (
+            Path(__file__).absolute().parent / "pvsamv1_basic_params.json"
+        )
+        with open(pvsamv1_defaults_file, "r") as f:
             tech_config = json.load(f)
-        tech_config.pop('subarray1_nstrings')
-        solar_only = deepcopy({key: technologies[key] for key in ('pv', 'grid')})   # includes system_capacity_kw parameter
-        solar_only['pv']['use_pvwatts'] = False             # specify detailed PV model
-        solar_only['pv']['tech_config'] = tech_config       # specify parameters
-        solar_only['grid']['interconnect_kw'] = 150e3
+        tech_config.pop("subarray1_nstrings")
+        solar_only = deepcopy(
+            {key: technologies[key] for key in ("pv", "grid")}
+        )  # includes system_capacity_kw parameter
+        solar_only["pv"]["use_pvwatts"] = False  # specify detailed PV model
+        solar_only["pv"]["tech_config"] = tech_config  # specify parameters
+        solar_only["grid"]["interconnect_kw"] = 150e3
         hybrid_config["technologies"] = solar_only
         hi = HoppInterface(hybrid_config)
         hybrid_plant = hi.system
-        assert hybrid_plant.pv.value('subarray1_nstrings') == 1343
+        assert hybrid_plant.pv.value("subarray1_nstrings") == 1343
         hybrid_plant.layout.plot()
 
         hi.simulate()
         aeps = hybrid_plant.annual_energies
         npvs = hybrid_plant.net_present_values
         assert aeps.pv == approx(annual_energy_expected, 1e-3)
         assert aeps.hybrid == approx(annual_energy_expected, 1e-3)
@@ -335,26 +497,27 @@
     with subtests.test("standalone detailed PV model (pvsamv1) using defaults"):
         annual_energy_expected = 11128604
         config = DetailedPVConfig.from_dict(detailed_pv)
         pv_plant = DetailedPVPlant(site=site, config=config)
         assert pv_plant.system_capacity_kw == approx(pv_kw, 1e-2)
         pv_plant.simulate_power(1, False)
         assert pv_plant.system_capacity_kw == approx(pv_kw, 1e-2)
-        assert pv_plant._system_model.Outputs.annual_energy == approx(annual_energy_expected, 1e-2)
+        assert pv_plant._system_model.Outputs.annual_energy == approx(
+            annual_energy_expected, 1e-2
+        )
         assert pv_plant._system_model.Outputs.capacity_factor == approx(25.66, 1e-2)
 
     with subtests.test("detailed PV model (pvsamv1) using defaults"):
         technologies = hybrid_config["technologies"]
         npv_expected = -2436229
-        solar_only = {
-            'pv': detailed_pv,
-            'grid': technologies['grid']
-        }
-        solar_only['pv']['use_pvwatts'] = False             # specify detailed PV model but don't change any defaults
-        solar_only['grid']['interconnect_kw'] = 150e3
+        solar_only = {"pv": detailed_pv, "grid": technologies["grid"]}
+        solar_only["pv"][
+            "use_pvwatts"
+        ] = False  # specify detailed PV model but don't change any defaults
+        solar_only["grid"]["interconnect_kw"] = 150e3
         hybrid_config["technologies"] = solar_only
         hi = HoppInterface(hybrid_config)
         hybrid_plant = hi.system
         hybrid_plant.layout.plot()
 
         hi.simulate()
 
@@ -364,22 +527,24 @@
         assert aeps.hybrid == approx(annual_energy_expected, 1e-3)
         assert npvs.pv == approx(npv_expected, 1e-3)
         assert npvs.hybrid == approx(npv_expected, 1e-3)
 
     with subtests.test("Detailed PV model (pvsamv1) using parameters from file"):
         annual_energy_expected = 102997528
         npv_expected = -25049424
-        pvsamv1_defaults_file = Path(__file__).absolute().parent / "pvsamv1_basic_params.json"
-        with open(pvsamv1_defaults_file, 'r') as f:
+        pvsamv1_defaults_file = (
+            Path(__file__).absolute().parent / "pvsamv1_basic_params.json"
+        )
+        with open(pvsamv1_defaults_file, "r") as f:
             tech_config = json.load(f)
-        solar_only = deepcopy({key: technologies[key] for key in ('pv', 'grid')})
-        solar_only['pv']['use_pvwatts'] = False             # specify detailed PV model
-        solar_only['pv']['tech_config'] = tech_config       # specify parameters
-        solar_only['grid']['interconnect_kw'] = 150e3
-        solar_only['pv']['system_capacity_kw'] = 50000      # use another system capacity
+        solar_only = deepcopy({key: technologies[key] for key in ("pv", "grid")})
+        solar_only["pv"]["use_pvwatts"] = False  # specify detailed PV model
+        solar_only["pv"]["tech_config"] = tech_config  # specify parameters
+        solar_only["grid"]["interconnect_kw"] = 150e3
+        solar_only["pv"]["system_capacity_kw"] = 50000  # use another system capacity
         hybrid_config["technologies"] = solar_only
         hi = HoppInterface(hybrid_config)
         hybrid_plant = hi.system
         hybrid_plant.layout.plot()
 
         hi.simulate()
 
@@ -406,46 +571,57 @@
     # aeps = hybrid_plant.annual_energies
     # npvs = hybrid_plant.net_present_values
     # assert aeps.pv == approx(annual_energy_expected, 1e-3)
     # assert aeps.hybrid == approx(annual_energy_expected, 1e-3)
     # assert npvs.pv == approx(npv_expected, 1e-3)
     # assert npvs.hybrid == approx(npv_expected, 1e-3)
 
-    with subtests.test("Detailed PV model using parameters from file and autosizing electrical parameters"):
+    with subtests.test(
+        "Detailed PV model using parameters from file and autosizing electrical parameters"
+    ):
         annual_energy_expected = 102319358
         npv_expected = -25110524
-        pvsamv1_defaults_file = Path(__file__).absolute().parent / "pvsamv1_basic_params.json"
-        with open(pvsamv1_defaults_file, 'r') as f:
+        pvsamv1_defaults_file = (
+            Path(__file__).absolute().parent / "pvsamv1_basic_params.json"
+        )
+        with open(pvsamv1_defaults_file, "r") as f:
             tech_config = json.load(f)
-        solar_only = deepcopy({key: technologies[key] for key in ('pv', 'grid')})
-        solar_only['pv']['use_pvwatts'] = False             # specify detailed PV model
-        solar_only['pv']['tech_config'] = tech_config       # specify parameters
-        solar_only['grid']['interconnect_kw'] = 150e3
-        solar_only['pv'].pop('system_capacity_kw')          # use default system capacity instead
+        solar_only = deepcopy({key: technologies[key] for key in ("pv", "grid")})
+        solar_only["pv"]["use_pvwatts"] = False  # specify detailed PV model
+        solar_only["pv"]["tech_config"] = tech_config  # specify parameters
+        solar_only["grid"]["interconnect_kw"] = 150e3
+        solar_only["pv"].pop(
+            "system_capacity_kw"
+        )  # use default system capacity instead
 
         # autosize number of strings, number of inverters and adjust system capacity
-        n_strings, n_combiners, n_inverters, calculated_system_capacity = size_electrical_parameters(
-            target_system_capacity=solar_only['pv']['tech_config']['system_capacity'],
-            target_dc_ac_ratio=1.34,
-            modules_per_string=solar_only['pv']['tech_config']['subarray1_modules_per_string'],
-            module_power= \
-                solar_only['pv']['tech_config']['cec_i_mp_ref'] \
-                * solar_only['pv']['tech_config']['cec_v_mp_ref'] \
+        n_strings, n_combiners, n_inverters, calculated_system_capacity = (
+            size_electrical_parameters(
+                target_system_capacity=solar_only["pv"]["tech_config"][
+                    "system_capacity"
+                ],
+                target_dc_ac_ratio=1.34,
+                modules_per_string=solar_only["pv"]["tech_config"][
+                    "subarray1_modules_per_string"
+                ],
+                module_power=solar_only["pv"]["tech_config"]["cec_i_mp_ref"]
+                * solar_only["pv"]["tech_config"]["cec_v_mp_ref"]
                 * 1e-3,
-            inverter_power=solar_only['pv']['tech_config']['inv_snl_paco'] * 1e-3,
-            n_inputs_inverter=50,
-            n_inputs_combiner=32
+                inverter_power=solar_only["pv"]["tech_config"]["inv_snl_paco"] * 1e-3,
+                n_inputs_inverter=50,
+                n_inputs_combiner=32,
+            )
         )
         assert n_strings == 13435
         assert n_combiners == 420
         assert n_inverters == 50
         assert calculated_system_capacity == approx(50002.2, 1e-3)
-        solar_only['pv']['tech_config']['subarray1_nstrings'] = n_strings
-        solar_only['pv']['tech_config']['inverter_count'] = n_inverters
-        solar_only['pv']['tech_config']['system_capacity'] = calculated_system_capacity
+        solar_only["pv"]["tech_config"]["subarray1_nstrings"] = n_strings
+        solar_only["pv"]["tech_config"]["inverter_count"] = n_inverters
+        solar_only["pv"]["tech_config"]["system_capacity"] = calculated_system_capacity
 
         hybrid_config["technologies"] = solar_only
         hi = HoppInterface(hybrid_config)
         hybrid_plant = hi.system
         hybrid_plant.layout.plot()
 
         hi.simulate()
@@ -464,96 +640,90 @@
     annual_energy_expected = 11128604
     npv_expected = -2436229
     system_capacity_kw = 5000
     system_capacity_kw_expected = 4998
     interconnect_kw = 150e3
 
     layout_params = {
-        "x_position": 0.5, 
-        "y_position": 0.5, 
-        "aspect_power": 0, 
-        "gcr": 0.5, 
-        "s_buffer": 2, 
-        "x_buffer": 2
+        "x_position": 0.5,
+        "y_position": 0.5,
+        "aspect_power": 0,
+        "gcr": 0.5,
+        "s_buffer": 2,
+        "x_buffer": 2,
     }
 
     # Run non-user-instantiated to compare against
     with subtests.test("baseline comparison"):
         solar_only = {
-            'pv': {
-                'use_pvwatts': False,
-                'tech_config': {'system_capacity_kw': system_capacity_kw},
+            "pv": {
+                "use_pvwatts": False,
+                "tech_config": {"system_capacity_kw": system_capacity_kw},
                 "layout_params": layout_params,
-                'dc_degradation': [0] * 25
+                "dc_degradation": [0] * 25,
             },
-            'grid': {
-                'interconnect_kw': interconnect_kw,
-                'ppa_price': 0.01
-            }
-        }
-        hopp_config = {
-            "site": site,
-            "technologies": solar_only
+            "grid": {"interconnect_kw": interconnect_kw, "ppa_price": 0.01},
         }
+        hopp_config = {"site": site, "technologies": solar_only}
         hi = HoppInterface(hopp_config)
         hybrid_plant = hi.system
         hybrid_plant.layout.plot()
         hybrid_plant.simulate()
         aeps = hybrid_plant.annual_energies
         npvs = hybrid_plant.net_present_values
         assert hybrid_plant.pv.system_capacity_kw == approx(system_capacity_kw, 1e-2)
         assert aeps.pv == approx(annual_energy_expected, 1e-2)
         assert aeps.hybrid == approx(annual_energy_expected, 1e-2)
         assert npvs.pv == approx(npv_expected, 1e-2)
         assert npvs.hybrid == approx(npv_expected, 1e-2)
 
-
     with subtests.test("detailed PV plant, grid and respective financial models"):
-        # Run 
+        # Run
         power_sources = {
-            'pv': {
-                'use_pvwatts': False,
-                'system_capacity_kw': system_capacity_kw,
-                'layout_params': layout_params,
-                'fin_model': 'FlatPlatePVSingleOwner',
-                'dc_degradation': [0] * 25
+            "pv": {
+                "use_pvwatts": False,
+                "system_capacity_kw": system_capacity_kw,
+                "layout_params": layout_params,
+                "fin_model": "FlatPlatePVSingleOwner",
+                "dc_degradation": [0] * 25,
+            },
+            "grid": {
+                "interconnect_kw": interconnect_kw,
+                "fin_model": "GenericSystemSingleOwner",
+                "ppa_price": 0.01,
             },
-            'grid': {
-                'interconnect_kw': interconnect_kw,
-                'fin_model': 'GenericSystemSingleOwner',
-                'ppa_price': 0.01
-            }
-        }
-        hopp_config = {
-            "site": site,
-            "technologies": power_sources
         }
+        hopp_config = {"site": site, "technologies": power_sources}
         hi = HoppInterface(hopp_config)
         hybrid_plant = hi.system
         assert hybrid_plant.pv is not None
         hybrid_plant.layout.plot()
 
         hybrid_plant.simulate()
 
         aeps = hybrid_plant.annual_energies
         npvs = hybrid_plant.net_present_values
-        assert hybrid_plant.pv._system_model.value("system_capacity") == approx(system_capacity_kw_expected, 1e-3)
-        assert hybrid_plant.pv._financial_model.value("system_capacity") == approx(system_capacity_kw_expected, 1e-3)
+        assert hybrid_plant.pv._system_model.value("system_capacity") == approx(
+            system_capacity_kw_expected, 1e-3
+        )
+        assert hybrid_plant.pv._financial_model.value("system_capacity") == approx(
+            system_capacity_kw_expected, 1e-3
+        )
         assert aeps.pv == approx(annual_energy_expected, 1e-3)
         assert aeps.hybrid == approx(annual_energy_expected, 1e-3)
         assert npvs.pv == approx(npv_expected, 1e-3)
         assert npvs.hybrid == approx(npv_expected, 1e-3)
 
 
 def test_hybrid(hybrid_config):
     """
     Performance from Wind is slightly different from wind-only case because the solar presence modified the wind layout
     """
     technologies = hybrid_config["technologies"]
-    solar_wind_hybrid = {key: technologies[key] for key in ('pv', 'wind', 'grid')}
+    solar_wind_hybrid = {key: technologies[key] for key in ("pv", "wind", "grid")}
     hybrid_config["technologies"] = solar_wind_hybrid
     hi = HoppInterface(hybrid_config)
     hybrid_plant = hi.system
 
     hi.simulate()
 
     aeps = hybrid_plant.annual_energies
@@ -566,19 +736,24 @@
     assert npvs.pv == approx(-5121293, 1e3)
     assert npvs.wind == approx(-13909363, 1e3)
     assert npvs.hybrid == approx(-19216589, 1e3)
 
 
 def test_wind_pv_with_storage_dispatch(hybrid_config):
     technologies = hybrid_config["technologies"]
-    wind_pv_battery = {key: technologies[key] for key in ('pv', 'wind', 'battery', 'grid')}
+    wind_pv_battery = {
+        key: technologies[key] for key in ("pv", "wind", "battery", "grid")
+    }
     hybrid_config["technologies"] = wind_pv_battery
     hybrid_config["technologies"]["grid"]["ppa_price"] = 0.03
     hi = HoppInterface(hybrid_config)
     hybrid_plant = hi.system
+    hybrid_plant.battery._financial_model.SystemCosts.assign(
+        {"om_batt_variable_cost": [0.75]}
+    )
 
     hi.simulate()
 
     aeps = hybrid_plant.annual_energies
     npvs = hybrid_plant.net_present_values
     taxes = hybrid_plant.federal_taxes
     apv = hybrid_plant.energy_purchases
@@ -645,148 +820,144 @@
     assert tc.battery[1] == approx(2201850, rel=5e-2)
     assert tc.hybrid[1] == approx(4338902, rel=5e-2)
 
 
 def test_tower_pv_hybrid(hybrid_config):
     interconnection_size_kw_test = 50000
     technologies_test = {
-        'tower': {
-            'cycle_capacity_kw': 50 * 1000, 
-            'solar_multiple': 2.0, 
-            'tes_hours': 12.0
+        "tower": {
+            "cycle_capacity_kw": 50 * 1000,
+            "solar_multiple": 2.0,
+            "tes_hours": 12.0,
         },
-        'pv': {'system_capacity_kw': 50 * 1000},
-        'grid': {
-            'interconnect_kw': interconnection_size_kw_test,
-            'ppa_price': 0.12
-        }
+        "pv": {"system_capacity_kw": 50 * 1000},
+        "grid": {"interconnect_kw": interconnection_size_kw_test, "ppa_price": 0.12},
     }
 
-    solar_hybrid = {key: technologies_test[key] for key in ('tower', 'pv', 'grid')}
+    solar_hybrid = {key: technologies_test[key] for key in ("tower", "pv", "grid")}
     hybrid_config["technologies"] = solar_hybrid
-    dispatch_options={'is_test_start_year': True, 'is_test_end_year': True}
+    dispatch_options = {"is_test_start_year": True, "is_test_end_year": True}
     hybrid_config["config"]["dispatch_options"] = dispatch_options
     hi = HoppInterface(hybrid_config)
     hybrid_plant = hi.system
-    hybrid_plant.tower.value('helio_width', 8.0)
-    hybrid_plant.tower.value('helio_height', 8.0)
+    hybrid_plant.tower.value("helio_width", 8.0)
+    hybrid_plant.tower.value("helio_height", 8.0)
 
     hi.simulate()
 
     aeps = hybrid_plant.annual_energies
     npvs = hybrid_plant.net_present_values
 
     assert aeps.pv == approx(104286701.28, 1e-3)
     assert aeps.tower == approx(3769716.50, 5e-2)
     assert aeps.hybrid == approx(107780622.67, 1e-2)
 
     # TODO: check npv for csp would require a full simulation
     assert npvs.pv == approx(45233832.23, 1e3)
-    #assert npvs.tower == approx(-13909363, 1e3)
-    #assert npvs.hybrid == approx(-19216589, 1e3)
+    # assert npvs.tower == approx(-13909363, 1e3)
+    # assert npvs.hybrid == approx(-19216589, 1e3)
 
 
 def test_trough_pv_hybrid(hybrid_config):
     interconnection_size_kw_test = 50000
     technologies_test = {
-        'trough': {
-            'cycle_capacity_kw': 50 * 1000, 
-            'solar_multiple': 2.0, 
-            'tes_hours': 12.0
-        },
-        'pv': {'system_capacity_kw': 50 * 1000},
-        'grid': {
-            'interconnect_kw': interconnection_size_kw_test,
-            'ppa_price': 0.12
+        "trough": {
+            "cycle_capacity_kw": 50 * 1000,
+            "solar_multiple": 2.0,
+            "tes_hours": 12.0,
         },
+        "pv": {"system_capacity_kw": 50 * 1000},
+        "grid": {"interconnect_kw": interconnection_size_kw_test, "ppa_price": 0.12},
     }
 
-    solar_hybrid = {key: technologies_test[key] for key in ('trough', 'pv', 'grid')}
+    solar_hybrid = {key: technologies_test[key] for key in ("trough", "pv", "grid")}
     hybrid_config["technologies"] = solar_hybrid
-    dispatch_options={'is_test_start_year': True, 'is_test_end_year': True}
+    dispatch_options = {"is_test_start_year": True, "is_test_end_year": True}
     hybrid_config["config"]["dispatch_options"] = dispatch_options
     hi = HoppInterface(hybrid_config)
     hybrid_plant = hi.system
 
     hi.simulate()
 
     aeps = hybrid_plant.annual_energies
     npvs = hybrid_plant.net_present_values
 
     assert aeps.pv == approx(104286701.17, 1e-3)
     assert aeps.trough == approx(1858279.58, 2e-2)
     assert aeps.hybrid == approx(106111732.52, 1e-3)
 
     assert npvs.pv == approx(80738107, 1e3)
-    #assert npvs.tower == approx(-13909363, 1e3)
-    #assert npvs.hybrid == approx(-19216589, 1e3)
+    # assert npvs.tower == approx(-13909363, 1e3)
+    # assert npvs.hybrid == approx(-19216589, 1e3)
 
 
 def test_tower_pv_battery_hybrid(hybrid_config):
     interconnection_size_kw_test = 50000
     technologies_test = {
-        'tower': {
-            'cycle_capacity_kw': 50 * 1000, 
-            'solar_multiple': 2.0, 
-            'tes_hours': 12.0
+        "tower": {
+            "cycle_capacity_kw": 50 * 1000,
+            "solar_multiple": 2.0,
+            "tes_hours": 12.0,
         },
-        'pv': {'system_capacity_kw': 50 * 1000},
-        'battery': {
-            'system_capacity_kwh': 40 * 1000,
-            'system_capacity_kw': 20 * 1000
-        },
-        'grid': {
-            'interconnect_kw': interconnection_size_kw_test,
-            'ppa_price': 0.12
-        }
+        "pv": {"system_capacity_kw": 50 * 1000},
+        "battery": {"system_capacity_kwh": 40 * 1000, "system_capacity_kw": 20 * 1000},
+        "grid": {"interconnect_kw": interconnection_size_kw_test, "ppa_price": 0.12},
     }
 
-    solar_hybrid = {key: technologies_test[key] for key in ('tower', 'pv', 'battery', 'grid')}
-    dispatch_options={'is_test_start_year': True, 'is_test_end_year': True}
+    solar_hybrid = {
+        key: technologies_test[key] for key in ("tower", "pv", "battery", "grid")
+    }
+    dispatch_options = {"is_test_start_year": True, "is_test_end_year": True}
     hybrid_config["technologies"] = solar_hybrid
     hybrid_config["config"]["dispatch_options"] = dispatch_options
     hi = HoppInterface(hybrid_config)
     hybrid_plant = hi.system
-    hybrid_plant.tower.value('helio_width', 10.0)
-    hybrid_plant.tower.value('helio_height', 10.0)
+    hybrid_plant.tower.value("helio_width", 10.0)
+    hybrid_plant.tower.value("helio_height", 10.0)
 
     hi.simulate()
 
     aeps = hybrid_plant.annual_energies
     npvs = hybrid_plant.net_present_values
 
     assert aeps.pv == approx(104286701, 1e-3)
     assert aeps.tower == approx(3783849, 5e-2)
     assert aeps.battery == approx(-9477, 2e-1)
     assert aeps.hybrid == approx(107903653, 1e-2)
 
     assert npvs.pv == approx(80738107, 1e3)
-    #assert npvs.tower == approx(-13909363, 1e3)
-    #assert npvs.hybrid == approx(-19216589, 1e3)
+    # assert npvs.tower == approx(-13909363, 1e3)
+    # assert npvs.hybrid == approx(-19216589, 1e3)
+
 
 def test_hybrid_om_costs_error(hybrid_config):
     technologies = hybrid_config["technologies"]
-    wind_pv_battery = {key: technologies[key] for key in ('pv', 'wind', 'battery', 'grid')}
-    dispatch_options={'battery_dispatch': 'one_cycle_heuristic'}
+    wind_pv_battery = {
+        key: technologies[key] for key in ("pv", "wind", "battery", "grid")
+    }
+    dispatch_options = {"battery_dispatch": "one_cycle_heuristic"}
     hybrid_config["technologies"] = wind_pv_battery
     hybrid_config["technologies"]["grid"]["ppa_price"] = 0.03
     hybrid_config["config"]["dispatch_options"] = dispatch_options
     hi = HoppInterface(hybrid_config)
     hybrid_plant = hi.system
-    hybrid_plant.battery._financial_model.value('om_production', (1,))
+    hybrid_plant.battery._financial_model.value("om_production", (1,))
 
     try:
         hi.simulate()
     except ValueError as e:
         assert e
 
+
 def test_hybrid_om_costs(hybrid_config):
     technologies = hybrid_config["technologies"]
-    wind_pv_battery = {key: technologies[key] for key in ('pv', 'wind', 'battery', 'grid')}
-    dispatch_options={'battery_dispatch': 'one_cycle_heuristic'}
+    wind_pv_battery = {
+        key: technologies[key] for key in ("pv", "wind", "battery", "grid")
+    }
+    dispatch_options = {"battery_dispatch": "one_cycle_heuristic"}
     hybrid_config["technologies"] = wind_pv_battery
     hybrid_config["technologies"]["grid"]["ppa_price"] = 0.03
     hybrid_config["config"]["dispatch_options"] = dispatch_options
     hi = HoppInterface(hybrid_config)
     hybrid_plant = hi.system
 
     # set all O&M costs to 0 to start
@@ -806,15 +977,17 @@
     hybrid_plant.battery.om_variable = 3
 
     hi.simulate()
 
     var_om_costs = hybrid_plant.om_variable_expenses
     total_om_costs = hybrid_plant.om_total_expenses
     for i in range(len(var_om_costs.hybrid)):
-        assert var_om_costs.pv[i] + var_om_costs.wind[i] + var_om_costs.battery[i] == approx(var_om_costs.hybrid[i], rel=1e-1)
+        assert var_om_costs.pv[i] + var_om_costs.wind[i] + var_om_costs.battery[
+            i
+        ] == approx(var_om_costs.hybrid[i], rel=1e-1)
         assert total_om_costs.pv[i] == approx(var_om_costs.pv[i])
         assert total_om_costs.wind[i] == approx(var_om_costs.wind[i])
         assert total_om_costs.battery[i] == approx(var_om_costs.battery[i])
         assert total_om_costs.hybrid[i] == approx(var_om_costs.hybrid[i])
     hybrid_plant.wind.om_variable = 0
     hybrid_plant.pv.om_variable = 0
     hybrid_plant.battery.om_variable = 0
@@ -823,16 +996,17 @@
     hybrid_plant.wind.om_fixed = 5
     hybrid_plant.pv.om_fixed = 2
     hybrid_plant.battery.om_fixed = 3
     hi.simulate()
     fixed_om_costs = hybrid_plant.om_fixed_expenses
     total_om_costs = hybrid_plant.om_total_expenses
     for i in range(len(fixed_om_costs.hybrid)):
-        assert fixed_om_costs.pv[i] + fixed_om_costs.wind[i] + fixed_om_costs.battery[i] \
-               == approx(fixed_om_costs.hybrid[i])
+        assert fixed_om_costs.pv[i] + fixed_om_costs.wind[i] + fixed_om_costs.battery[
+            i
+        ] == approx(fixed_om_costs.hybrid[i])
         assert total_om_costs.pv[i] == approx(fixed_om_costs.pv[i])
         assert total_om_costs.wind[i] == approx(fixed_om_costs.wind[i])
         assert total_om_costs.battery[i] == approx(fixed_om_costs.battery[i])
         assert total_om_costs.hybrid[i] == approx(fixed_om_costs.hybrid[i])
     hybrid_plant.wind.om_fixed = 0
     hybrid_plant.pv.om_fixed = 0
     hybrid_plant.battery.om_fixed = 0
@@ -841,140 +1015,195 @@
     hybrid_plant.wind.om_capacity = 5
     hybrid_plant.pv.om_capacity = 2
     hybrid_plant.battery.om_capacity = 3
     hi.simulate()
     cap_om_costs = hybrid_plant.om_capacity_expenses
     total_om_costs = hybrid_plant.om_total_expenses
     for i in range(len(cap_om_costs.hybrid)):
-        assert cap_om_costs.pv[i] + cap_om_costs.wind[i] + cap_om_costs.battery[i] \
-               == approx(cap_om_costs.hybrid[i])
+        assert cap_om_costs.pv[i] + cap_om_costs.wind[i] + cap_om_costs.battery[
+            i
+        ] == approx(cap_om_costs.hybrid[i])
         assert total_om_costs.pv[i] == approx(cap_om_costs.pv[i])
         assert total_om_costs.wind[i] == approx(cap_om_costs.wind[i])
         assert total_om_costs.battery[i] == approx(cap_om_costs.battery[i])
         assert total_om_costs.hybrid[i] == approx(cap_om_costs.hybrid[i])
     hybrid_plant.wind.om_capacity = 0
     hybrid_plant.pv.om_capacity = 0
     hybrid_plant.battery.om_capacity = 0
 
+
 def test_hybrid_tax_incentives(hybrid_config):
     technologies = hybrid_config["technologies"]
-    wind_pv_battery = {key: technologies[key] for key in ('pv', 'wind', 'battery', 'grid')}
-    dispatch_options={'battery_dispatch': 'one_cycle_heuristic'}
+    wind_pv_battery = {
+        key: technologies[key] for key in ("pv", "wind", "battery", "grid")
+    }
+    dispatch_options = {"battery_dispatch": "one_cycle_heuristic"}
     hybrid_config["technologies"] = wind_pv_battery
     hybrid_config["technologies"]["grid"]["ppa_price"] = 0.03
     hybrid_config["config"]["dispatch_options"] = dispatch_options
     hi = HoppInterface(hybrid_config)
     hybrid_plant = hi.system
 
-    hybrid_plant.pv._financial_model.value('itc_fed_percent', [0.0])
-    hybrid_plant.wind._financial_model.value('ptc_fed_amount', (1,))
-    hybrid_plant.pv._financial_model.value('ptc_fed_amount', (2,))
-    hybrid_plant.battery._financial_model.value('ptc_fed_amount', (3,))
-    hybrid_plant.wind._financial_model.value('ptc_fed_escal', 0)
-    hybrid_plant.pv._financial_model.value('ptc_fed_escal', 0)
-    hybrid_plant.battery._financial_model.value('ptc_fed_escal', 0)
+    hybrid_plant.pv._financial_model.value("itc_fed_percent", [0.0])
+    hybrid_plant.wind._financial_model.value("ptc_fed_amount", (1,))
+    hybrid_plant.pv._financial_model.value("ptc_fed_amount", (2,))
+    hybrid_plant.battery._financial_model.value("ptc_fed_amount", (3,))
+    hybrid_plant.wind._financial_model.value("ptc_fed_escal", 0)
+    hybrid_plant.pv._financial_model.value("ptc_fed_escal", 0)
+    hybrid_plant.battery._financial_model.value("ptc_fed_escal", 0)
 
     hi.simulate()
 
     ptc_wind = hybrid_plant.wind._financial_model.value("cf_ptc_fed")[1]
-    assert ptc_wind == approx(hybrid_plant.wind._financial_model.value("ptc_fed_amount")[0]*hybrid_plant.wind.annual_energy_kwh, rel=1e-3)
+    assert ptc_wind == approx(
+        hybrid_plant.wind._financial_model.value("ptc_fed_amount")[0]
+        * hybrid_plant.wind.annual_energy_kwh,
+        rel=1e-3,
+    )
 
     ptc_pv = hybrid_plant.pv._financial_model.value("cf_ptc_fed")[1]
-    assert ptc_pv == approx(hybrid_plant.pv._financial_model.value("ptc_fed_amount")[0]*hybrid_plant.pv.annual_energy_kwh, rel=1e-3)
+    assert ptc_pv == approx(
+        hybrid_plant.pv._financial_model.value("ptc_fed_amount")[0]
+        * hybrid_plant.pv.annual_energy_kwh,
+        rel=1e-3,
+    )
 
     ptc_batt = hybrid_plant.battery._financial_model.value("cf_ptc_fed")[1]
-    assert ptc_batt == approx(hybrid_plant.battery._financial_model.value("ptc_fed_amount")[0]
-           * hybrid_plant.battery._financial_model.value('batt_annual_discharge_energy')[1], rel=1e-3)
+    assert ptc_batt == approx(
+        hybrid_plant.battery._financial_model.value("ptc_fed_amount")[0]
+        * hybrid_plant.battery._financial_model.value("batt_annual_discharge_energy")[
+            1
+        ],
+        rel=1e-3,
+    )
 
     ptc_hybrid = hybrid_plant.grid._financial_model.value("cf_ptc_fed")[1]
     ptc_fed_amount = hybrid_plant.grid._financial_model.value("ptc_fed_amount")[0]
     assert ptc_fed_amount == approx(1.229, rel=1e-2)
-    assert ptc_hybrid == approx(ptc_fed_amount * hybrid_plant.grid._financial_model.value('cf_energy_net')[1], rel=1e-3)
+    assert ptc_hybrid == approx(
+        ptc_fed_amount * hybrid_plant.grid._financial_model.value("cf_energy_net")[1],
+        rel=1e-3,
+    )
 
 
 def test_capacity_credit(hybrid_config):
     technologies = hybrid_config["technologies"]
     site = create_default_site_info(capacity_hours=capacity_credit_hours)
-    wind_pv_battery = {key: technologies[key] for key in ('pv', 'wind', 'battery')}
-    wind_pv_battery['grid'] = {
-        'interconnect_kw': interconnection_size_kw,
-        'ppa_price': 0.03
+    wind_pv_battery = {key: technologies[key] for key in ("pv", "wind", "battery")}
+    wind_pv_battery["grid"] = {
+        "interconnect_kw": interconnection_size_kw,
+        "ppa_price": 0.03,
     }
     hybrid_config["technologies"] = wind_pv_battery
     hybrid_config["site"] = site
     hi = HoppInterface(hybrid_config)
     hybrid_plant = hi.system
+    hybrid_plant.battery._financial_model.SystemCosts.assign(
+        {"om_batt_variable_cost": [0.75]}
+    )
 
     assert hybrid_plant.interconnect_kw == 15e3
 
     # Backup values for resetting before tests
     gen_max_feasible_orig = hybrid_plant.battery.gen_max_feasible
     capacity_hours_orig = hybrid_plant.site.capacity_hours
     interconnect_kw_orig = hybrid_plant.interconnect_kw
+
     def reinstate_orig_values():
         hybrid_plant.battery.gen_max_feasible = gen_max_feasible_orig
         hybrid_plant.site.capacity_hours = capacity_hours_orig
         hybrid_plant.interconnect_kw = interconnect_kw_orig
 
     # Test when 0 gen_max_feasible
     reinstate_orig_values()
     hybrid_plant.battery.gen_max_feasible = [0] * 8760
-    capacity_credit_battery = hybrid_plant.battery.calc_capacity_credit_percent(hybrid_plant.interconnect_kw)
+    capacity_credit_battery = hybrid_plant.battery.calc_capacity_credit_percent(
+        hybrid_plant.interconnect_kw
+    )
     assert capacity_credit_battery == approx(0, rel=0.05)
     # Test when representative gen_max_feasible
     reinstate_orig_values()
     hybrid_plant.battery.gen_max_feasible = [2500] * 8760
-    capacity_credit_battery = hybrid_plant.battery.calc_capacity_credit_percent(hybrid_plant.interconnect_kw)
+    capacity_credit_battery = hybrid_plant.battery.calc_capacity_credit_percent(
+        hybrid_plant.interconnect_kw
+    )
     assert capacity_credit_battery == approx(50, rel=0.05)
     # Test when no capacity hours
     reinstate_orig_values()
     hybrid_plant.battery.gen_max_feasible = [2500] * 8760
     hybrid_plant.site.capacity_hours = [False] * 8760
-    capacity_credit_battery = hybrid_plant.battery.calc_capacity_credit_percent(hybrid_plant.interconnect_kw)
+    capacity_credit_battery = hybrid_plant.battery.calc_capacity_credit_percent(
+        hybrid_plant.interconnect_kw
+    )
     assert capacity_credit_battery == approx(0, rel=0.05)
     # Test when no interconnect capacity
     reinstate_orig_values()
     hybrid_plant.battery.gen_max_feasible = [2500] * 8760
     hybrid_plant.interconnect_kw = 0
-    capacity_credit_battery = hybrid_plant.battery.calc_capacity_credit_percent(hybrid_plant.interconnect_kw)
+    capacity_credit_battery = hybrid_plant.battery.calc_capacity_credit_percent(
+        hybrid_plant.interconnect_kw
+    )
     assert capacity_credit_battery == approx(0, rel=0.05)
 
     # Test integration with system simulation
     reinstate_orig_values()
     cap_payment_mw = 100000
     hybrid_plant.assign({"cp_capacity_payment_amount": [cap_payment_mw]})
 
     assert hybrid_plant.interconnect_kw == 15e3
 
     hi.simulate()
 
-    total_gen_max_feasible = np.array(hybrid_plant.pv.gen_max_feasible) \
-                           + np.array(hybrid_plant.wind.gen_max_feasible) \
-                           + np.array(hybrid_plant.battery.gen_max_feasible)
-    assert sum(hybrid_plant.grid.gen_max_feasible) == approx(sum(np.minimum(hybrid_plant.grid.interconnect_kw * hybrid_plant.site.interval / 60, \
-                                                                            total_gen_max_feasible)), rel=0.01)
-
-    total_nominal_capacity = hybrid_plant.pv.calc_nominal_capacity(hybrid_plant.interconnect_kw) \
-                           + hybrid_plant.wind.calc_nominal_capacity(hybrid_plant.interconnect_kw) \
-                           + hybrid_plant.battery.calc_nominal_capacity(hybrid_plant.interconnect_kw)
+    total_gen_max_feasible = (
+        np.array(hybrid_plant.pv.gen_max_feasible)
+        + np.array(hybrid_plant.wind.gen_max_feasible)
+        + np.array(hybrid_plant.battery.gen_max_feasible)
+    )
+    assert sum(hybrid_plant.grid.gen_max_feasible) == approx(
+        sum(
+            np.minimum(
+                hybrid_plant.grid.interconnect_kw * hybrid_plant.site.interval / 60,
+                total_gen_max_feasible,
+            )
+        ),
+        rel=0.01,
+    )
+
+    total_nominal_capacity = (
+        hybrid_plant.pv.calc_nominal_capacity(hybrid_plant.interconnect_kw)
+        + hybrid_plant.wind.calc_nominal_capacity(hybrid_plant.interconnect_kw)
+        + hybrid_plant.battery.calc_nominal_capacity(hybrid_plant.interconnect_kw)
+    )
     assert total_nominal_capacity == approx(18845.8, rel=0.01)
-    assert total_nominal_capacity == approx(hybrid_plant.grid.hybrid_nominal_capacity, rel=0.01)
-    
+    assert total_nominal_capacity == approx(
+        hybrid_plant.grid.hybrid_nominal_capacity, rel=0.01
+    )
+
     capcred = hybrid_plant.capacity_credit_percent
-    assert capcred['pv'][0] == approx(8.03, rel=0.05)
-    assert capcred['wind'][0] == approx(33.25, rel=0.10)
-    assert capcred['battery'][0] == approx(58.95, rel=0.05)
-    assert capcred['hybrid'][0] == approx(43.88, rel=0.05)
+    assert capcred["pv"][0] == approx(8.03, rel=0.05)
+    assert capcred["wind"][0] == approx(33.25, rel=0.10)
+    assert capcred["battery"][0] == approx(58.95, rel=0.05)
+    assert capcred["hybrid"][0] == approx(43.88, rel=0.05)
 
     cp_pay = hybrid_plant.capacity_payments
-    np_cap = hybrid_plant.system_nameplate_mw # This is not the same as nominal capacity...
-    assert cp_pay['pv'][1]/(np_cap['pv'])/(capcred['pv'][0]/100) == approx(cap_payment_mw, 0.05)
-    assert cp_pay['wind'][1]/(np_cap['wind'])/(capcred['wind'][0]/100) == approx(cap_payment_mw, 0.05)
-    assert cp_pay['battery'][1]/(np_cap['battery'])/(capcred['battery'][0]/100) == approx(cap_payment_mw, 0.05)
-    assert cp_pay['hybrid'][1]/(np_cap['hybrid'])/(capcred['hybrid'][0]/100) == approx(cap_payment_mw, 0.05)
+    np_cap = (
+        hybrid_plant.system_nameplate_mw
+    )  # This is not the same as nominal capacity...
+    assert cp_pay["pv"][1] / (np_cap["pv"]) / (capcred["pv"][0] / 100) == approx(
+        cap_payment_mw, 0.05
+    )
+    assert cp_pay["wind"][1] / (np_cap["wind"]) / (capcred["wind"][0] / 100) == approx(
+        cap_payment_mw, 0.05
+    )
+    assert cp_pay["battery"][1] / (np_cap["battery"]) / (
+        capcred["battery"][0] / 100
+    ) == approx(cap_payment_mw, 0.05)
+    assert cp_pay["hybrid"][1] / (np_cap["hybrid"]) / (
+        capcred["hybrid"][0] / 100
+    ) == approx(cap_payment_mw, 0.05)
 
     aeps = hybrid_plant.annual_energies
     npvs = hybrid_plant.net_present_values
     taxes = hybrid_plant.federal_taxes
     apv = hybrid_plant.energy_purchases
     debt = hybrid_plant.debt_payment
     esv = hybrid_plant.energy_sales
```

### Comparing `HOPP-2.1.0/tests/hopp/test_layout.py` & `HOPP-2.2.0/tests/hopp/test_layout.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/tests/hopp/test_pv_source.py` & `HOPP-2.2.0/tests/hopp/test_pv_source.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/tests/hopp/test_reopt.py` & `HOPP-2.2.0/tests/hopp/test_reopt.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/tests/hopp/test_resource.py` & `HOPP-2.2.0/tests/hopp/test_resource.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/tests/hopp/test_resource_download.py` & `HOPP-2.2.0/tests/hopp/test_resource_download.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/tests/hopp/test_site_info.py` & `HOPP-2.2.0/tests/hopp/test_site_info.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/tests/hopp/test_solar_wind.py` & `HOPP-2.2.0/tests/hopp/test_solar_wind.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/tests/hopp/test_tower_source.py` & `HOPP-2.2.0/tests/hopp/test_tower_source.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/tests/hopp/test_trough_source.py` & `HOPP-2.2.0/tests/hopp/test_trough_source.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/tests/hopp/test_utility_rate.py` & `HOPP-2.2.0/tests/hopp/test_utility_rate.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/tests/hopp/test_wave.py` & `HOPP-2.2.0/tests/hopp/test_wave.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/tests/hopp/test_wind.py` & `HOPP-2.2.0/tests/hopp/test_wind.py`

 * *Files identical despite different names*

### Comparing `HOPP-2.1.0/tests/hopp/utils.py` & `HOPP-2.2.0/tests/hopp/utils.py`

 * *Files identical despite different names*

