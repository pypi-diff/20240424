# Comparing `tmp/grid_data_models-0.1.0.tar.gz` & `tmp/grid_data_models-0.1.1.tar.gz`

## Comparing `grid_data_models-0.1.0.tar` & `grid_data_models-0.1.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/__init__.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/bus.py
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/capacitor.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/constants.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/exceptions.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/load.py
--rw-r--r--   0        0        0     4863 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/quantities.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/transformer.py
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/dataset/__init__.py
--rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/dataset/cost_model.py
--rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/dataset/dataset_system.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/__init__.py
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/curve.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/distribution_common.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/distribution_enum.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/distribution_graph.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/distribution_system.py
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/limitset.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/sequence_pair.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/components/__init__.py
--rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/components/distribution_branch.py
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/components/distribution_bus.py
--rw-r--r--   0        0        0     3199 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/components/distribution_capacitor.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/components/distribution_component.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/components/distribution_feeder.py
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/components/distribution_fuse.py
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/components/distribution_load.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/components/distribution_recloser.py
--rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/components/distribution_regulator.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/components/distribution_solar.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/components/distribution_substation.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/components/distribution_switch.py
--rw-r--r--   0        0        0     5670 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/components/distribution_transformer.py
--rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/components/distribution_vsource.py
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/components/geometry_branch.py
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/components/matrix_impedance_branch.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/components/matrix_impedance_fuse.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/components/matrix_impedance_recloser.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/components/matrix_impedance_switch.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/components/sequence_impedance_branch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/controllers/__init__.py
--rw-r--r--   0        0        0     6198 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/controllers/distribution_capacitor_controller.py
--rw-r--r--   0        0        0     3545 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/controllers/distribution_inverter_controller.py
--rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/controllers/distribution_recloser_controller.py
--rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/controllers/distribution_regulator_controller.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/controllers/distribution_switch_controller.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/equipment/__init__.py
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/equipment/bare_conductor_equipment.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/equipment/capacitor_equipment.py
--rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/equipment/concentric_cable_equipment.py
--rw-r--r--   0        0        0     8840 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/equipment/distribution_transformer_equipment.py
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/equipment/geometry_branch_equipment.py
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/equipment/inverter_equipment.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/equipment/load_equipment.py
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/equipment/matrix_impedance_branch_equipment.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/equipment/matrix_impedance_fuse_equipment.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/equipment/matrix_impedance_recloser_equipment.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/equipment/matrix_impedance_switch_equipment.py
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/equipment/phase_capacitor_equipment.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/equipment/phase_load_equipment.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/equipment/recloser_controller_equipment.py
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/equipment/sequence_impedance_branch_equipment.py
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/equipment/solar_equipment.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/transmission/transmission_branch.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/transmission/transmission_bus.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/transmission/transmission_capacitor.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/transmission/transmission_component.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/transmission/transmission_load.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/transmission/transmission_substation.py
--rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/.gitignore
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/README.md
--rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/__init__.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/bus.py
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/capacitor.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/constants.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/exceptions.py
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/load.py
+-rw-r--r--   0        0        0     4863 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/quantities.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/transformer.py
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/dataset/__init__.py
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/dataset/cost_model.py
+-rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/dataset/dataset_system.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/__init__.py
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/curve.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/distribution_common.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/distribution_enum.py
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/distribution_graph.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/distribution_system.py
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/limitset.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/sequence_pair.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/components/__init__.py
+-rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/components/distribution_branch.py
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/components/distribution_bus.py
+-rw-r--r--   0        0        0     3199 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/components/distribution_capacitor.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/components/distribution_component.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/components/distribution_feeder.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/components/distribution_fuse.py
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/components/distribution_load.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/components/distribution_recloser.py
+-rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/components/distribution_regulator.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/components/distribution_solar.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/components/distribution_substation.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/components/distribution_switch.py
+-rw-r--r--   0        0        0     5670 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/components/distribution_transformer.py
+-rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/components/distribution_vsource.py
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/components/geometry_branch.py
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/components/matrix_impedance_branch.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/components/matrix_impedance_fuse.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/components/matrix_impedance_recloser.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/components/matrix_impedance_switch.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/components/sequence_impedance_branch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/controllers/__init__.py
+-rw-r--r--   0        0        0     6198 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/controllers/distribution_capacitor_controller.py
+-rw-r--r--   0        0        0     3545 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/controllers/distribution_inverter_controller.py
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/controllers/distribution_recloser_controller.py
+-rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/controllers/distribution_regulator_controller.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/controllers/distribution_switch_controller.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/equipment/__init__.py
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/equipment/bare_conductor_equipment.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/equipment/capacitor_equipment.py
+-rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/equipment/concentric_cable_equipment.py
+-rw-r--r--   0        0        0     8840 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/equipment/distribution_transformer_equipment.py
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/equipment/geometry_branch_equipment.py
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/equipment/inverter_equipment.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/equipment/load_equipment.py
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/equipment/matrix_impedance_branch_equipment.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/equipment/matrix_impedance_fuse_equipment.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/equipment/matrix_impedance_recloser_equipment.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/equipment/matrix_impedance_switch_equipment.py
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/equipment/phase_capacitor_equipment.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/equipment/phase_load_equipment.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/equipment/recloser_controller_equipment.py
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/equipment/sequence_impedance_branch_equipment.py
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/distribution/equipment/solar_equipment.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/transmission/transmission_branch.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/transmission/transmission_bus.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/transmission/transmission_capacitor.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/transmission/transmission_component.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/transmission/transmission_load.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/src/gdm/transmission/transmission_substation.py
+-rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/README.md
+-rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 grid_data_models-0.1.1/PKG-INFO
```

### Comparing `grid_data_models-0.1.0/src/gdm/__init__.py` & `grid_data_models-0.1.1/src/gdm/__init__.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/bus.py` & `grid_data_models-0.1.1/src/gdm/bus.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/capacitor.py` & `grid_data_models-0.1.1/src/gdm/capacitor.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/load.py` & `grid_data_models-0.1.1/src/gdm/load.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/quantities.py` & `grid_data_models-0.1.1/src/gdm/quantities.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/version.py` & `grid_data_models-0.1.1/src/gdm/version.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 import subprocess
 import platform
 import sys
 
-VERSION = "0.1.0"
+VERSION = "0.1.1"
 
 
 def is_git_repo(dir: Path) -> bool:
     """Returns true if it is a git repo."""
     git_path = dir / ".git"
     return git_path.exists()
```

### Comparing `grid_data_models-0.1.0/src/gdm/dataset/cost_model.py` & `grid_data_models-0.1.1/src/gdm/dataset/cost_model.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/dataset/dataset_system.py` & `grid_data_models-0.1.1/src/gdm/dataset/dataset_system.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/distribution/curve.py` & `grid_data_models-0.1.1/src/gdm/distribution/curve.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/distribution/distribution_enum.py` & `grid_data_models-0.1.1/src/gdm/distribution/distribution_enum.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/distribution/distribution_graph.py` & `grid_data_models-0.1.1/src/gdm/distribution/distribution_graph.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """ This module contains class for creating graph representation of Distribution System."""
 
 import networkx as nx
 from infrasys import System
 
-from gdm.distribution.components.distribution_bus import DistributionBus
-from gdm.distribution.components.distribution_branch import DistributionBranch
-from gdm.distribution.components.distribution_transformer import DistributionTransformer
+from gdm import (
+    DistributionTransformer,
+    DistributionBranch,
+    DistributionBus,
+)
 
 
 def build_graph_from_system(system: System) -> nx.Graph:
     """Returns networkx instance of the system."""
 
     graph = nx.Graph()
     node: DistributionBus
@@ -17,9 +19,13 @@
         graph.add_node(node.name)
 
     edges: list[DistributionBranch | DistributionTransformer] = list(
         system.get_components(DistributionBranch)
     ) + list(system.get_components(DistributionTransformer))
 
     for edge in edges:
-        graph.add_edge(edge.buses[0].name, edge.buses[1].name)
+        graph.add_edge(
+            edge.buses[0].name,
+            edge.buses[1].name,
+            **{"name": edge.name, "type": edge.__class__.__name__},
+        )
     return graph
```

### Comparing `grid_data_models-0.1.0/src/gdm/distribution/distribution_system.py` & `grid_data_models-0.1.1/src/gdm/distribution/distribution_system.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/distribution/limitset.py` & `grid_data_models-0.1.1/src/gdm/distribution/limitset.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/distribution/components/distribution_branch.py` & `grid_data_models-0.1.1/src/gdm/distribution/components/distribution_branch.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/distribution/components/distribution_bus.py` & `grid_data_models-0.1.1/src/gdm/distribution/components/distribution_bus.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/distribution/components/distribution_capacitor.py` & `grid_data_models-0.1.1/src/gdm/distribution/components/distribution_capacitor.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/distribution/components/distribution_component.py` & `grid_data_models-0.1.1/src/gdm/distribution/components/distribution_component.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/distribution/components/distribution_load.py` & `grid_data_models-0.1.1/src/gdm/distribution/components/distribution_load.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/distribution/components/distribution_regulator.py` & `grid_data_models-0.1.1/src/gdm/distribution/components/distribution_regulator.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/distribution/components/distribution_solar.py` & `grid_data_models-0.1.1/src/gdm/distribution/components/distribution_solar.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/distribution/components/distribution_substation.py` & `grid_data_models-0.1.1/src/gdm/distribution/components/distribution_substation.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/distribution/components/distribution_transformer.py` & `grid_data_models-0.1.1/src/gdm/distribution/components/distribution_transformer.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/distribution/components/distribution_vsource.py` & `grid_data_models-0.1.1/src/gdm/distribution/components/distribution_vsource.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/distribution/components/geometry_branch.py` & `grid_data_models-0.1.1/src/gdm/distribution/components/geometry_branch.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/distribution/components/matrix_impedance_branch.py` & `grid_data_models-0.1.1/src/gdm/distribution/components/matrix_impedance_branch.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/distribution/components/matrix_impedance_fuse.py` & `grid_data_models-0.1.1/src/gdm/distribution/components/matrix_impedance_fuse.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/distribution/components/matrix_impedance_recloser.py` & `grid_data_models-0.1.1/src/gdm/distribution/components/matrix_impedance_recloser.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/distribution/components/matrix_impedance_switch.py` & `grid_data_models-0.1.1/src/gdm/distribution/components/matrix_impedance_switch.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/distribution/components/sequence_impedance_branch.py` & `grid_data_models-0.1.1/src/gdm/distribution/components/sequence_impedance_branch.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/distribution/controllers/distribution_capacitor_controller.py` & `grid_data_models-0.1.1/src/gdm/distribution/controllers/distribution_capacitor_controller.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/distribution/controllers/distribution_inverter_controller.py` & `grid_data_models-0.1.1/src/gdm/distribution/controllers/distribution_inverter_controller.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/distribution/controllers/distribution_recloser_controller.py` & `grid_data_models-0.1.1/src/gdm/distribution/controllers/distribution_recloser_controller.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/distribution/controllers/distribution_regulator_controller.py` & `grid_data_models-0.1.1/src/gdm/distribution/controllers/distribution_regulator_controller.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/distribution/controllers/distribution_switch_controller.py` & `grid_data_models-0.1.1/src/gdm/distribution/controllers/distribution_switch_controller.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/distribution/equipment/bare_conductor_equipment.py` & `grid_data_models-0.1.1/src/gdm/distribution/equipment/bare_conductor_equipment.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/distribution/equipment/capacitor_equipment.py` & `grid_data_models-0.1.1/src/gdm/distribution/equipment/capacitor_equipment.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/distribution/equipment/concentric_cable_equipment.py` & `grid_data_models-0.1.1/src/gdm/distribution/equipment/concentric_cable_equipment.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/distribution/equipment/distribution_transformer_equipment.py` & `grid_data_models-0.1.1/src/gdm/distribution/equipment/distribution_transformer_equipment.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/distribution/equipment/geometry_branch_equipment.py` & `grid_data_models-0.1.1/src/gdm/distribution/equipment/geometry_branch_equipment.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/distribution/equipment/inverter_equipment.py` & `grid_data_models-0.1.1/src/gdm/distribution/equipment/inverter_equipment.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/distribution/equipment/load_equipment.py` & `grid_data_models-0.1.1/src/gdm/distribution/equipment/load_equipment.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/distribution/equipment/matrix_impedance_branch_equipment.py` & `grid_data_models-0.1.1/src/gdm/distribution/equipment/matrix_impedance_branch_equipment.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/distribution/equipment/matrix_impedance_fuse_equipment.py` & `grid_data_models-0.1.1/src/gdm/distribution/equipment/matrix_impedance_fuse_equipment.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/distribution/equipment/matrix_impedance_recloser_equipment.py` & `grid_data_models-0.1.1/src/gdm/distribution/equipment/matrix_impedance_recloser_equipment.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/distribution/equipment/matrix_impedance_switch_equipment.py` & `grid_data_models-0.1.1/src/gdm/distribution/equipment/matrix_impedance_switch_equipment.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/distribution/equipment/phase_capacitor_equipment.py` & `grid_data_models-0.1.1/src/gdm/distribution/equipment/phase_capacitor_equipment.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/distribution/equipment/phase_load_equipment.py` & `grid_data_models-0.1.1/src/gdm/distribution/equipment/phase_load_equipment.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/distribution/equipment/sequence_impedance_branch_equipment.py` & `grid_data_models-0.1.1/src/gdm/distribution/equipment/sequence_impedance_branch_equipment.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/src/gdm/distribution/equipment/solar_equipment.py` & `grid_data_models-0.1.1/src/gdm/distribution/equipment/solar_equipment.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/.gitignore` & `grid_data_models-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/LICENSE.txt` & `grid_data_models-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/README.md` & `grid_data_models-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/pyproject.toml` & `grid_data_models-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.0/PKG-INFO` & `grid_data_models-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: grid-data-models
-Version: 0.1.0
+Version: 0.1.1
 Project-URL: Documentation, https://github.com/NREL-Distribution-Suites/grid-data-models#readme
 Project-URL: Issues, https://github.com/NREL-Distribution-Suites/grid-data-models/issues
 Project-URL: Source, https://github.com/NREL-Distribution-Suites/grid-data-models
 Author-email: Kapil Duwadi <Kapil.Duwadi@nrel.gov>, Aadil Latif <Aadil.Latif@nrel.gov>, Tarek Elgindy <tarek.elgindy@nrel.gov>
 License-Expression: BSD-3-Clause
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: BSD License
```

