# Comparing `tmp/xenon_fuse-1.2.0.tar.gz` & `tmp/xenon_fuse-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xenon_fuse-1.2.0.tar", max compression
+gzip compressed data, was "xenon_fuse-1.2.1.tar", max compression
```

## Comparing `xenon_fuse-1.2.0.tar` & `xenon_fuse-1.2.1.tar`

### file list

```diff
@@ -1,59 +1,60 @@
--rw-r--r--   0        0        0     1536 2024-04-11 16:49:58.763337 xenon_fuse-1.2.0/LICENSE
--rw-r--r--   0        0        0     1726 2024-04-11 16:49:58.763337 xenon_fuse-1.2.0/README.md
--rw-r--r--   0        0        0      160 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/__init__.py
--rw-r--r--   0        0        0     9142 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/common.py
--rw-r--r--   0        0        0     9554 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/context.py
--rw-r--r--   0        0        0     2639 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugin.py
--rw-r--r--   0        0        0      241 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/__init__.py
--rw-r--r--   0        0        0      478 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/detector_physics/README.md
--rw-r--r--   0        0        0      593 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/detector_physics/__init__.py
--rw-r--r--   0        0        0     9196 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/detector_physics/csv_input.py
--rw-r--r--   0        0        0      615 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/detector_physics/delayed_electrons/__init__.py
--rw-r--r--   0        0        0     1055 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_drift.py
--rw-r--r--   0        0        0      803 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_extraction.py
--rw-r--r--   0        0        0     2550 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_merger.py
--rw-r--r--   0        0        0      974 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_s1photonhits.py
--rw-r--r--   0        0        0     2017 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_secondary_scintillation.py
--rw-r--r--   0        0        0      837 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_timing.py
--rw-r--r--   0        0        0     8539 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/detector_physics/delayed_electrons/photo_ionization_electrons.py
--rw-r--r--   0        0        0    14746 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/detector_physics/electron_drift.py
--rw-r--r--   0        0        0     4556 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/detector_physics/electron_extraction.py
--rw-r--r--   0        0        0     3121 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/detector_physics/electron_timing.py
--rw-r--r--   0        0        0     5471 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/detector_physics/s1_photon_hits.py
--rw-r--r--   0        0        0    13699 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/detector_physics/s1_photon_propagation.py
--rw-r--r--   0        0        0    35274 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/detector_physics/s2_photon_propagation.py
--rw-r--r--   0        0        0     9188 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/detector_physics/secondary_scintillation.py
--rw-r--r--   0        0        0      647 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/micro_physics/README.md
--rw-r--r--   0        0        0      459 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/micro_physics/__init__.py
--rw-r--r--   0        0        0    10138 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/micro_physics/detector_volumes.py
--rw-r--r--   0        0        0     2314 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/micro_physics/electric_field.py
--rw-r--r--   0        0        0     4574 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/micro_physics/find_cluster.py
--rw-r--r--   0        0        0    22316 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/micro_physics/input.py
--rw-r--r--   0        0        0     5342 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/micro_physics/merge_cluster.py
--rw-r--r--   0        0        0      456 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/micro_physics/microphysics_summary.py
--rw-r--r--   0        0        0     4295 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/micro_physics/wfsim_connection.py
--rw-r--r--   0        0        0    17709 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/micro_physics/yields.py
--rw-r--r--   0        0        0      152 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/pmt_and_daq/README.md
--rw-r--r--   0        0        0      251 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/pmt_and_daq/__init__.py
--rw-r--r--   0        0        0     9569 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/pmt_and_daq/photon_pulses.py
--rw-r--r--   0        0        0      436 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/pmt_and_daq/photon_summary.py
--rw-r--r--   0        0        0     9013 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/pmt_and_daq/pmt_afterpulses.py
--rw-r--r--   0        0        0    20113 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/pmt_and_daq/pmt_response_and_daq.py
--rw-r--r--   0        0        0      293 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/truth_information/__init__.py
--rw-r--r--   0        0        0     2789 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/truth_information/cluster_tagging.py
--rw-r--r--   0        0        0     2278 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/truth_information/event_truth.py
--rw-r--r--   0        0        0     8349 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/truth_information/peak_truth.py
--rw-r--r--   0        0        0     4754 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/truth_information/records_truth.py
--rw-r--r--   0        0        0     1543 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/plugins/truth_information/surviving_clusters.py
--rw-r--r--   0        0        0      895 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/vertical_merger_plugin.py
--rw-r--r--   0        0        0     1041 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/fuse/volume_plugin.py
--rw-r--r--   0        0        0     1169 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      823 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/tests/_utils.py
--rw-r--r--   0        0        0     1770 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/tests/test_DetectorPhysics_csv.py
--rw-r--r--   0        0        0     3299 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/tests/test_FullChain.py
--rw-r--r--   0        0        0     4900 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/tests/test_FullChain_w_DelayedElectrons.py
--rw-r--r--   0        0        0     2490 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/tests/test_MicroPhysics.py
--rw-r--r--   0        0        0     4560 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/tests/test_deterministic_seed.py
--rw-r--r--   0        0        0     7827 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/tests/test_input.py
--rw-r--r--   0        0        0     5000 2024-04-11 16:49:58.787337 xenon_fuse-1.2.0/tests/test_plugin_random_seed.py
--rw-r--r--   0        0        0     3250 1970-01-01 00:00:00.000000 xenon_fuse-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1536 2024-04-24 11:35:16.193976 xenon_fuse-1.2.1/LICENSE
+-rw-r--r--   0        0        0     1726 2024-04-24 11:35:16.193976 xenon_fuse-1.2.1/README.md
+-rw-r--r--   0        0        0      204 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/__init__.py
+-rw-r--r--   0        0        0     9142 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/common.py
+-rw-r--r--   0        0        0     9697 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/context.py
+-rw-r--r--   0        0        0     2785 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/dtypes.py
+-rw-r--r--   0        0        0     2639 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugin.py
+-rw-r--r--   0        0        0      241 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/__init__.py
+-rw-r--r--   0        0        0      478 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/detector_physics/README.md
+-rw-r--r--   0        0        0      593 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/detector_physics/__init__.py
+-rw-r--r--   0        0        0     7963 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/detector_physics/csv_input.py
+-rw-r--r--   0        0        0      615 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/detector_physics/delayed_electrons/__init__.py
+-rw-r--r--   0        0        0     1055 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_drift.py
+-rw-r--r--   0        0        0      803 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_extraction.py
+-rw-r--r--   0        0        0     2550 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_merger.py
+-rw-r--r--   0        0        0      956 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_s1photonhits.py
+-rw-r--r--   0        0        0     2017 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_secondary_scintillation.py
+-rw-r--r--   0        0        0      837 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_timing.py
+-rw-r--r--   0        0        0     8539 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/detector_physics/delayed_electrons/photo_ionization_electrons.py
+-rw-r--r--   0        0        0    14728 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/detector_physics/electron_drift.py
+-rw-r--r--   0        0        0     4537 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/detector_physics/electron_extraction.py
+-rw-r--r--   0        0        0     3103 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/detector_physics/electron_timing.py
+-rw-r--r--   0        0        0     5453 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/detector_physics/s1_photon_hits.py
+-rw-r--r--   0        0        0    13368 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/detector_physics/s1_photon_propagation.py
+-rw-r--r--   0        0        0    34895 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/detector_physics/s2_photon_propagation.py
+-rw-r--r--   0        0        0     9238 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/detector_physics/secondary_scintillation.py
+-rw-r--r--   0        0        0      647 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/micro_physics/README.md
+-rw-r--r--   0        0        0      459 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/micro_physics/__init__.py
+-rw-r--r--   0        0        0     7280 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/micro_physics/detector_volumes.py
+-rw-r--r--   0        0        0     2262 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/micro_physics/electric_field.py
+-rw-r--r--   0        0        0     4556 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/micro_physics/find_cluster.py
+-rw-r--r--   0        0        0    20236 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/micro_physics/input.py
+-rw-r--r--   0        0        0     4424 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/micro_physics/merge_cluster.py
+-rw-r--r--   0        0        0      456 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/micro_physics/microphysics_summary.py
+-rw-r--r--   0        0        0     4305 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/micro_physics/wfsim_connection.py
+-rw-r--r--   0        0        0    17364 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/micro_physics/yields.py
+-rw-r--r--   0        0        0      152 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/pmt_and_daq/README.md
+-rw-r--r--   0        0        0      251 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/pmt_and_daq/__init__.py
+-rw-r--r--   0        0        0     9569 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/pmt_and_daq/photon_pulses.py
+-rw-r--r--   0        0        0      436 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/pmt_and_daq/photon_summary.py
+-rw-r--r--   0        0        0     8682 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/pmt_and_daq/pmt_afterpulses.py
+-rw-r--r--   0        0        0    20113 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/pmt_and_daq/pmt_response_and_daq.py
+-rw-r--r--   0        0        0      293 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/truth_information/__init__.py
+-rw-r--r--   0        0        0     2771 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/truth_information/cluster_tagging.py
+-rw-r--r--   0        0        0     2260 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/truth_information/event_truth.py
+-rw-r--r--   0        0        0     8331 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/truth_information/peak_truth.py
+-rw-r--r--   0        0        0     4784 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/truth_information/records_truth.py
+-rw-r--r--   0        0        0     1543 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/truth_information/surviving_clusters.py
+-rw-r--r--   0        0        0      895 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/vertical_merger_plugin.py
+-rw-r--r--   0        0        0     1041 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/volume_plugin.py
+-rw-r--r--   0        0        0     1169 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0      823 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/tests/_utils.py
+-rw-r--r--   0        0        0     1770 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/tests/test_DetectorPhysics_csv.py
+-rw-r--r--   0        0        0     3526 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/tests/test_FullChain.py
+-rw-r--r--   0        0        0     4900 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/tests/test_FullChain_w_DelayedElectrons.py
+-rw-r--r--   0        0        0     2490 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/tests/test_MicroPhysics.py
+-rw-r--r--   0        0        0     4560 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/tests/test_deterministic_seed.py
+-rw-r--r--   0        0        0     7134 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/tests/test_input.py
+-rw-r--r--   0        0        0     5000 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/tests/test_plugin_random_seed.py
+-rw-r--r--   0        0        0     3250 1970-01-01 00:00:00.000000 xenon_fuse-1.2.1/PKG-INFO
```

### Comparing `xenon_fuse-1.2.0/LICENSE` & `xenon_fuse-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.0/README.md` & `xenon_fuse-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.0/fuse/common.py` & `xenon_fuse-1.2.1/fuse/common.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.0/fuse/context.py` & `xenon_fuse-1.2.1/fuse/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -238,26 +238,30 @@
             map_data["map"].shape[-1] == pmt_mask.shape[0]
         ), "Error! Pattern map and PMT gains must have same dimensions!"
         map_data["map"][..., ~pmt_mask] = 0.0
     return straxen.InterpolatingMap(map_data, method=method)
 
 
 @URLConfig.register("s2_aft_scaling")
-def modify_s2_pattern_map(s2_pattern_map, s2_mean_area_fraction_top, n_tpc_pmts, n_top_pmts):
+def modify_s2_pattern_map(
+    s2_pattern_map, s2_mean_area_fraction_top, n_tpc_pmts, n_top_pmts, turned_off_pmts
+):
     """Modify the S2 pattern map to match a given input AFT."""
     if s2_mean_area_fraction_top > 0:
         s2map = deepcopy(s2_pattern_map)
-        s2map_topeff_ = s2map.data["map"][..., 0:n_top_pmts].sum(axis=2)
-        s2map_toteff_ = s2map.data["map"].sum(axis=2)
-        orig_aft_ = np.mean((s2map_topeff_ / s2map_toteff_)[s2map_toteff_ > 0.0])
+        # First we need to set turned off pmts before scaling
+        s2map.data["map"][..., turned_off_pmts] = 0
+        s2map_topeff_ = s2map.data["map"][..., :n_top_pmts].sum(axis=2, keepdims=True)
+        s2map_toteff_ = s2map.data["map"].sum(axis=2, keepdims=True)
+        orig_aft_ = np.nanmean(s2map_topeff_ / s2map_toteff_)
         # Getting scales for top/bottom separately to preserve total efficiency
         scale_top_ = s2_mean_area_fraction_top / orig_aft_
         scale_bot_ = (1 - s2_mean_area_fraction_top) / (1 - orig_aft_)
-        s2map.data["map"][:, :, 0:n_top_pmts] *= scale_top_
-        s2map.data["map"][:, :, n_top_pmts:n_tpc_pmts] *= scale_bot_
+        s2map.data["map"][..., :n_top_pmts] *= scale_top_
+        s2map.data["map"][..., n_top_pmts:n_tpc_pmts] *= scale_bot_
         s2_pattern_map.__init__(s2map.data)
     return s2_pattern_map
 
 
 # Probably not needed!
 @URLConfig.register("simple_load")
 def load(data):
```

### Comparing `xenon_fuse-1.2.0/fuse/plugin.py` & `xenon_fuse-1.2.1/fuse/plugin.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.0/fuse/plugins/detector_physics/__init__.py` & `xenon_fuse-1.2.1/fuse/plugins/detector_physics/__init__.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.0/fuse/plugins/detector_physics/delayed_electrons/__init__.py` & `xenon_fuse-1.2.1/fuse/plugins/detector_physics/delayed_electrons/__init__.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.0/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_drift.py` & `xenon_fuse-1.2.1/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_drift.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.0/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_extraction.py` & `xenon_fuse-1.2.1/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_extraction.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.0/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_merger.py` & `xenon_fuse-1.2.1/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_merger.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.0/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_s1photonhits.py` & `xenon_fuse-1.2.1/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_s1photonhits.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 
     depends_on = "photo_ionization_electrons"
     provides = "delayed_s1_photons"
     data_kind = "delayed_interactions_in_roi"
 
     dtype = [
         (("Number detected S1 photons", "n_s1_photon_hits"), np.int32),
-    ]
-    dtype = dtype + strax.time_fields
+    ] + strax.time_fields
 
     def compute(self, delayed_interactions_in_roi):
         result = np.zeros(len(delayed_interactions_in_roi), dtype=self.dtype)
         result["time"] = delayed_interactions_in_roi["time"]
         result["endtime"] = delayed_interactions_in_roi["endtime"]
         return result
```

### Comparing `xenon_fuse-1.2.0/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_secondary_scintillation.py` & `xenon_fuse-1.2.1/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_secondary_scintillation.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.0/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_timing.py` & `xenon_fuse-1.2.1/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_timing.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.0/fuse/plugins/detector_physics/delayed_electrons/photo_ionization_electrons.py` & `xenon_fuse-1.2.1/fuse/plugins/detector_physics/delayed_electrons/photo_ionization_electrons.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.0/fuse/plugins/detector_physics/electron_drift.py` & `xenon_fuse-1.2.1/fuse/plugins/detector_physics/electron_drift.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,16 +39,15 @@
         ),
         (("Observed x position of the cluster at liquid-gas interface [cm]", "x_obs"), np.float32),
         (("Observed y position of the cluster at liquid-gas interface [cm]", "y_obs"), np.float32),
         (
             ("Observed z position of the cluster after field distortion correction [cm]", "z_obs"),
             np.float32,
         ),
-    ]
-    dtype = dtype + strax.time_fields
+    ] + strax.time_fields
 
     save_when = strax.SaveWhen.ALWAYS
 
     # Config options
 
     drift_velocity_liquid = straxen.URLConfig(
         default="take://resource://"
```

### Comparing `xenon_fuse-1.2.0/fuse/plugins/detector_physics/electron_extraction.py` & `xenon_fuse-1.2.1/fuse/plugins/detector_physics/electron_extraction.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,15 @@
     provides = "extracted_electrons"
     data_kind = "interactions_in_roi"
 
     save_when = strax.SaveWhen.ALWAYS
 
     dtype = [
         (("Number of electrons extracted into the gas phase", "n_electron_extracted"), np.int32),
-    ]
-
-    dtype = dtype + strax.time_fields
+    ] + strax.time_fields
 
     # Config options
     s2_secondary_sc_gain_mc = straxen.URLConfig(
         default="take://resource://"
         "SIMULATION_CONFIG_FILE.json?&fmt=json"
         "&take=s2_secondary_sc_gain",
         type=(int, float),
```

### Comparing `xenon_fuse-1.2.0/fuse/plugins/detector_physics/electron_timing.py` & `xenon_fuse-1.2.1/fuse/plugins/detector_physics/electron_timing.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,15 @@
 
     save_when = strax.SaveWhen.TARGET
 
     dtype = [
         (("x position of the electron [cm]", "x"), np.float32),
         (("y position of the electron [cm]", "y"), np.float32),
         (("ID of the cluster creating the electron", "cluster_id"), np.int32),
-    ]
-    dtype = dtype + strax.time_fields
+    ] + strax.time_fields
 
     # Config options
     electron_trapping_time = straxen.URLConfig(
         default="take://resource://"
         "SIMULATION_CONFIG_FILE.json?&fmt=json"
         "&take=electron_trapping_time",
         type=(int, float),
```

### Comparing `xenon_fuse-1.2.0/fuse/plugins/detector_physics/s1_photon_hits.py` & `xenon_fuse-1.2.1/fuse/plugins/detector_physics/s1_photon_hits.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,16 +25,15 @@
     provides = "s1_photons"
     data_kind = "interactions_in_roi"
 
     save_when = strax.SaveWhen.ALWAYS
 
     dtype = [
         (("Number detected S1 photons", "n_s1_photon_hits"), np.int32),
-    ]
-    dtype = dtype + strax.time_fields
+    ] + strax.time_fields
 
     # Config options
     pmt_circuit_load_resistor = straxen.URLConfig(
         default="take://resource://"
         "SIMULATION_CONFIG_FILE.json?&fmt=json"
         "&take=pmt_circuit_load_resistor",
         type=(int, float),
```

### Comparing `xenon_fuse-1.2.0/fuse/plugins/detector_physics/s1_photon_propagation.py` & `xenon_fuse-1.2.1/fuse/plugins/detector_physics/s1_photon_propagation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 
 import numpy as np
 import nestpy
 import strax
 import straxen
 
+from ...dtypes import propagated_photons_fields
 from ...common import pmt_gains, build_photon_propagation_output
 from ...common import (
     init_spe_scaling_factor_distributions,
     pmt_transit_time_spread,
     photon_gain_calculation,
 )
 from ...plugin import FuseBasePlugin
@@ -36,22 +37,15 @@
 
     depends_on = ("microphysics_summary", "s1_photons")
     provides = "propagated_s1_photons"
     data_kind = "s1_photons"
 
     save_when = strax.SaveWhen.TARGET
 
-    dtype = [
-        (("PMT channel of the photon", "channel"), np.int16),
-        (("Photon creates a double photo-electron emission", "dpe"), np.bool_),
-        (("Sampled PMT gain for the photon", "photon_gain"), np.int32),
-        (("ID of the cluster creating the photon", "cluster_id"), np.int32),
-        (("Type of the photon. S1 (1), S2 (2) or PMT AP (0)", "photon_type"), np.int8),
-    ]
-    dtype = dtype + strax.time_fields
+    dtype = propagated_photons_fields + strax.time_fields
 
     # Config options shared by S1 and S2 simulation
     p_double_pe_emision = straxen.URLConfig(
         default="take://resource://"
         "SIMULATION_CONFIG_FILE.json?&fmt=json"
         "&take=p_double_pe_emision",
         type=(int, float),
```

### Comparing `xenon_fuse-1.2.0/fuse/plugins/detector_physics/s2_photon_propagation.py` & `xenon_fuse-1.2.1/fuse/plugins/detector_physics/s2_photon_propagation.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import numpy as np
 import logging
 
 from numba import njit
 from scipy.stats import skewnorm
 from scipy import constants
 
+from ...dtypes import propagated_photons_fields
 from ...common import pmt_gains, build_photon_propagation_output
 from ...common import (
     init_spe_scaling_factor_distributions,
     pmt_transit_time_spread,
     photon_gain_calculation,
 )
 from ...plugin import FuseBaseDownChunkingPlugin
@@ -44,22 +45,15 @@
     )
 
     provides = "propagated_s2_photons"
     data_kind = "s2_photons"
 
     save_when = strax.SaveWhen.TARGET
 
-    dtype = [
-        (("PMT channel of the photon", "channel"), np.int16),
-        (("Photon creates a double photo-electron emission", "dpe"), np.bool_),
-        (("Sampled PMT gain for the photon", "photon_gain"), np.int32),
-        (("ID of the cluster creating the photon", "cluster_id"), np.int32),
-        (("Type of the photon. S1 (1), S2 (2) or PMT AP (0)", "photon_type"), np.int8),
-    ]
-    dtype = dtype + strax.time_fields
+    dtype = propagated_photons_fields + strax.time_fields
 
     # Config options shared by S1 and S2 simulation
     p_double_pe_emision = straxen.URLConfig(
         default="take://resource://"
         "SIMULATION_CONFIG_FILE.json?&fmt=json"
         "&take=p_double_pe_emision",
         type=(int, float),
@@ -213,15 +207,16 @@
         default="s2_aft_scaling://pattern_map://resource://simulation_config://"
         "SIMULATION_CONFIG_FILE.json?"
         "&key=s2_pattern_map"
         "&fmt=pkl"
         "&pmt_mask=plugin.pmt_mask"
         "&s2_mean_area_fraction_top=plugin.s2_mean_area_fraction_top"
         "&n_tpc_pmts=plugin.n_tpc_pmts"
-        "&n_top_pmts=plugin.n_top_pmts",
+        "&n_top_pmts=plugin.n_top_pmts"
+        "&turned_off_pmts=plugin.turned_off_pmts",
         cache=True,
         help="S2 pattern map",
     )
 
     singlet_fraction_gas = straxen.URLConfig(
         default="take://resource://"
         "SIMULATION_CONFIG_FILE.json?&fmt=json"
@@ -446,17 +441,14 @@
             pattern = self.s2_pattern_map(positions)  # [position, pmt]
 
         if pattern.shape[1] - 1 not in bottom_index:
             pattern = np.pad(
                 pattern, [[0, 0], [0, len(bottom_index)]], "constant", constant_values=1
             )
 
-        # Remove turned off pmts
-        pattern[:, np.in1d(channels, self.turned_off_pmts)] = 0
-
         sum_pat = np.sum(pattern, axis=1).reshape(-1, 1)
         pattern = np.divide(pattern, sum_pat, out=np.zeros_like(pattern), where=sum_pat != 0)
 
         assert pattern.shape[0] == len(positions)
         assert pattern.shape[1] == len(channels)
 
         _buffer_photon_channels = []
```

### Comparing `xenon_fuse-1.2.0/fuse/plugins/detector_physics/secondary_scintillation.py` & `xenon_fuse-1.2.1/fuse/plugins/detector_physics/secondary_scintillation.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,15 +156,16 @@
         default="s2_aft_scaling://pattern_map://resource://simulation_config://"
         "SIMULATION_CONFIG_FILE.json?"
         "&key=s2_pattern_map"
         "&fmt=pkl"
         "&pmt_mask=plugin.pmt_mask"
         "&s2_mean_area_fraction_top=plugin.s2_mean_area_fraction_top"
         "&n_tpc_pmts=plugin.n_tpc_pmts"
-        "&n_top_pmts=plugin.n_top_pmts",
+        "&n_top_pmts=plugin.n_top_pmts"
+        "&turned_off_pmts=plugin.turned_off_pmts",
         cache=True,
         help="S2 pattern map",
     )
 
     def setup(self):
         super().setup()
```

### Comparing `xenon_fuse-1.2.0/fuse/plugins/micro_physics/README.md` & `xenon_fuse-1.2.1/fuse/plugins/micro_physics/README.md`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.0/fuse/plugins/micro_physics/electric_field.py` & `xenon_fuse-1.2.1/fuse/plugins/micro_physics/electric_field.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import strax
 import numpy as np
 import logging
 import straxen
 
+from ...dtypes import electric_fields
 from ...plugin import FuseBasePlugin
 
 export, __all__ = strax.exporter()
 
 logging.basicConfig(handlers=[logging.StreamHandler()])
 log = logging.getLogger("fuse.micro_physics.electric_field")
 
@@ -20,18 +21,15 @@
 
     depends_on = "interactions_in_roi"
     provides = "electric_field_values"
     data_kind = "interactions_in_roi"
 
     save_when = strax.SaveWhen.TARGET
 
-    dtype = [
-        (("Electric field value at the cluster position [V/cm]", "e_field"), np.float32),
-        *strax.time_fields,
-    ]
+    dtype = electric_fields + strax.time_fields
 
     # Config options
     efield_map = straxen.URLConfig(
         default="itp_map://resource://simulation_config://"
         "SIMULATION_CONFIG_FILE.json?"
         "&key=efield_map"
         "&fmt=json.gz"
```

### Comparing `xenon_fuse-1.2.0/fuse/plugins/micro_physics/find_cluster.py` & `xenon_fuse-1.2.1/fuse/plugins/micro_physics/find_cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,16 +29,15 @@
 
     depends_on = "geant4_interactions"
 
     provides = "cluster_index"
 
     dtype = [
         (("Cluster index of the energy deposit", "cluster_ids"), np.int32),
-    ]
-    dtype = dtype + strax.time_fields
+    ] + strax.time_fields
 
     save_when = strax.SaveWhen.TARGET
 
     # Not start at 0. 0 are set per default for contributing clusters so we want to avoid that
     clusters_seen = 1
 
     # Config options
```

### Comparing `xenon_fuse-1.2.0/fuse/plugins/micro_physics/input.py` & `xenon_fuse-1.2.1/fuse/plugins/micro_physics/input.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import uproot
 import awkward as ak
 import numpy as np
 import pandas as pd
 import strax
 import straxen
 
+from ...dtypes import g4_fields, primary_positions_fields, deposit_positions_fields
 from ...common import full_array_to_numpy, reshape_awkward, dynamic_chunking
 from ...plugin import FuseBasePlugin
 
 export, __all__ = strax.exporter()
 
 logging.basicConfig(handlers=[logging.StreamHandler()])
 log = logging.getLogger("fuse.micro_physics.input")
@@ -23,40 +24,20 @@
 class ChunkInput(FuseBasePlugin):
     """Plugin to read XENONnT Geant4 root or csv files.
 
     The plugin can distribute the events in time based on a source rate
     and will create multiple chunks of data if needed.
     """
 
-    __version__ = "0.3.2"
+    __version__ = "0.3.3"
 
     depends_on: Tuple = tuple()
     provides = "geant4_interactions"
 
-    source_done = False
-
-    dtype = [
-        (("x position of the energy deposit [cm]", "x"), np.float64),
-        (("y position of the energy deposit [cm]", "y"), np.float64),
-        (("z position of the energy deposit [cm]", "z"), np.float64),
-        (("Time with respect to the start of the event [ns]", "t"), np.float64),
-        (("Energy deposit in keV", "ed"), np.float32),
-        (("Particle type", "type"), "<U18"),
-        (("Geant4 track ID", "trackid"), np.int16),
-        (("Particle type of the parent particle", "parenttype"), "<U18"),
-        (("Trackid of the parent particle", "parentid"), np.int16),
-        (("Geant4 process creating the particle", "creaproc"), "<U25"),
-        (("Geant4 process responsible for the energy deposit", "edproc"), "<U25"),
-        (("Geant4 event ID", "evtid"), np.int32),
-        (("x position of the primary particle [cm]", "x_pri"), np.float32),
-        (("y position of the primary particle [cm]", "y_pri"), np.float32),
-        (("z position of the primary particle [cm]", "z_pri"), np.float32),
-    ]
-
-    dtype = dtype + strax.time_fields
+    dtype = deposit_positions_fields + g4_fields + primary_positions_fields + strax.time_fields
 
     save_when = strax.SaveWhen.TARGET
 
     source_done = False
 
     # Config options
     path = straxen.URLConfig(
@@ -188,14 +169,15 @@
         entry_start=None,
         entry_stop=None,
         cut_by_eventid=False,
         cut_nr_only=False,
     ):
         self.directory = directory
         self.file_name = file_name
+        self.file_type = self.file_name.split(".")[-1]
         self.rng = random_number_generator
         self.separation_scale = separation_scale
         self.event_rate = event_rate / 1e9  # Conversion to ns
         self.n_interactions_per_chunk = n_interactions_per_chunk
         self.cut_delayed = cut_delayed
         self.last_chunk_length = np.int64(last_chunk_length)
         self.first_chunk_left = np.int64(first_chunk_left)
@@ -205,64 +187,36 @@
         self.entry_start = entry_start
         self.entry_stop = entry_stop
         self.cut_by_eventid = cut_by_eventid
         self.cut_nr_only = cut_nr_only
 
         self.file = os.path.join(self.directory, self.file_name)
 
-        self.column_names = [
-            "x",
-            "y",
-            "z",
-            "t",
-            "ed",
-            "type",
-            "trackid",
-            "parenttype",
-            "parentid",
-            "creaproc",
-            "edproc",
-        ]
+        self.dtype = deposit_positions_fields + g4_fields
+        self.columns = list(np.dtype(self.dtype).names)
+        # Remove eventid as it is not in the usual root or csv file
+        self.columns.remove("eventid")
+        self.dtype += primary_positions_fields + strax.time_fields
 
         # Prepare cut for root and csv case
         if self.outer_cylinder:
             self.cut_string = (
                 f'(r < {self.outer_cylinder["max_r"]}) '
                 f'& ((zp >= {self.outer_cylinder["min_z"] * 10}) '
                 f'& (zp < {self.outer_cylinder["max_z"] * 10}))'
             )
         else:
             self.cut_string = None
 
-        self.dtype = [
-            (("x position of the energy deposit [cm]", "x"), np.float64),
-            (("y position of the energy deposit [cm]", "y"), np.float64),
-            (("z position of the energy deposit [cm]", "z"), np.float64),
-            (("Time with respect to the start of the event [ns]", "t"), np.float64),
-            (("Energy deposit in keV", "ed"), np.float32),
-            (("Particle type", "type"), "<U18"),
-            (("Geant4 track ID", "trackid"), np.int16),
-            (("Particle type of the parent particle", "parenttype"), "<U18"),
-            (("Trackid of the parent particle", "parentid"), np.int16),
-            (("Geant4 process creating the particle", "creaproc"), "<U25"),
-            (("Geant4 process responsible for the energy deposit", "edproc"), "<U25"),
-            (("Geant4 event ID", "evtid"), np.int32),
-            (("x position of the primary particle", "x_pri"), np.float32),
-            (("y position of the primary particle", "y_pri"), np.float32),
-            (("z position of the primary particle", "z_pri"), np.float32),
-        ]
-
-        self.dtype = self.dtype + strax.time_fields
-
     def output_chunk(self):
-        """Function to return one chunk of data from the root file."""
+        """Function to return one chunk of data from the root or csv file."""
 
-        if self.file.endswith(".root"):
+        if self.file_type == "root":
             interactions, n_simulated_events, start, stop = self._load_root_file()
-        elif self.file.endswith(".csv"):
+        elif self.file_type == "csv":
             interactions, n_simulated_events, start, stop = self._load_csv_file()
         else:
             raise ValueError(
                 f'Cannot load events from file "{self.file}": .root or .cvs file needed.'
             )
 
         # Removing all events with zero energy deposit
@@ -293,35 +247,35 @@
         # Need to check start and stop again....
         if self.event_rate > 0:
             event_times = self.rng.uniform(
                 low=start / self.event_rate, high=stop / self.event_rate, size=stop - start
             ).astype(np.int64)
             event_times = np.sort(event_times)
 
-            structure = np.unique(inter_reshaped["evtid"], return_counts=True)[1]
+            structure = np.unique(inter_reshaped["eventid"], return_counts=True)[1]
 
             # Check again why [:len(structure)] is needed
             interaction_time = np.repeat(event_times[: len(structure)], structure)
             inter_reshaped["time"] = interaction_time + inter_reshaped["t"]
         elif self.event_rate == 0:
             log.info("Using event times from provided input file.")
-            if self.file.endswith(".root"):
+            if self.file_type == "root":
                 msg = (
                     "Using event times from root file is not recommended! "
                     "Use a source_rate > 0 instead."
                 )
                 log.warning(msg)
             inter_reshaped["time"] = inter_reshaped["t"]
         else:
             raise ValueError("Source rate cannot be negative!")
 
         # Remove interactions that happen way after the run ended
         delay_cut = inter_reshaped["t"] <= self.cut_delayed
         log.info(
-            f"Removing {np.sum(~delay_cut)} ({np.sum(~delay_cut)/len(delay_cut):.4%}) "
+            f"Removing {np.sum(~delay_cut)} ({np.sum(~delay_cut) / len(delay_cut):.4%}) "
             f"interactions later than {self.cut_delayed:.2e} ns."
         )
         inter_reshaped = inter_reshaped[delay_cut]
 
         sort_idx = np.argsort(inter_reshaped["time"])
         inter_reshaped = inter_reshaped[sort_idx]
 
@@ -453,23 +407,23 @@
             "z": "zp/10",
             "r": "sqrt(x**2 + y**2)",
             "t": "time*10**9",
         }
 
         # Read in data, convert mm to cm and perform a first cut if specified:
         interactions = ttree.arrays(
-            self.column_names,
+            self.columns,
             self.cut_string,
             aliases=alias,
             entry_start=start_index,
             entry_stop=stop_index,
         )
         eventids = ttree.arrays("eventid", entry_start=start_index, entry_stop=stop_index)
         eventids = ak.broadcast_arrays(eventids["eventid"], interactions["x"])[0]
-        interactions["evtid"] = eventids
+        interactions["eventid"] = eventids
 
         xyz_pri = ttree.arrays(
             ["x_pri", "y_pri", "z_pri"],
             aliases={"x_pri": "xp_pri/10", "y_pri": "yp_pri/10", "z_pri": "zp_pri/10"},
             entry_start=start_index,
             entry_stop=stop_index,
         )
@@ -519,38 +473,40 @@
             n_simulated_events: Total number of simulated events
             start: Index of the first loaded interaction
             stop: Index of the last loaded interaction
         """
 
         log.debug("Load instructions from a csv file!")
 
-        instr_df = pd.read_csv(self.file)
+        df = pd.read_csv(self.file)
 
         # unit conversion similar to root case
-        instr_df["x"] = instr_df["xp"] / 10
-        instr_df["y"] = instr_df["yp"] / 10
-        instr_df["z"] = instr_df["zp"] / 10
-        instr_df["x_pri"] = instr_df["xp_pri"] / 10
-        instr_df["y_pri"] = instr_df["yp_pri"] / 10
-        instr_df["z_pri"] = instr_df["zp_pri"] / 10
-        instr_df["r"] = np.sqrt(instr_df["x"] ** 2 + instr_df["y"] ** 2)
-        instr_df["t"] = instr_df["time"]
+        df["x"] = df["xp"] / 10
+        df["y"] = df["yp"] / 10
+        df["z"] = df["zp"] / 10
+        df["x_pri"] = df["xp_pri"] / 10
+        df["y_pri"] = df["yp_pri"] / 10
+        df["z_pri"] = df["zp_pri"] / 10
+        df["r"] = np.sqrt(df["x"] ** 2 + df["y"] ** 2)
+        df["t"] = df["time"]
+
+        missing_columns = set(self.columns) - set(df.columns)
 
         # Check if all needed columns are in place:
-        if not set(self.column_names).issubset(instr_df.columns):
-            log.warning("Not all needed columns provided!")
+        if missing_columns:
+            raise ValueError(f"Not all needed columns provided! {missing_columns} are missing.")
 
-        n_simulated_events = len(np.unique(instr_df.eventid))
+        n_simulated_events = len(np.unique(df.eventid))
 
         if self.outer_cylinder:
-            instr_df = instr_df.query(self.cut_string)
+            df = df.query(self.cut_string)
 
-        instr_df = instr_df[self.column_names + ["eventid", "x_pri", "y_pri", "z_pri"]]
+        df = df[self.columns + ["eventid", "x_pri", "y_pri", "z_pri"]]
 
-        interactions = self._awkwardify_df(instr_df)
+        interactions = self._awkwardify_df(df)
 
         # Use always all events in the csv file
         start = 0
         stop = n_simulated_events
 
         return interactions, n_simulated_events, start, stop
 
@@ -578,11 +534,11 @@
             "ed": reshape_awkward(df["ed"].values, evt_offsets),
             "type": reshape_awkward(np.array(df["type"], dtype=str), evt_offsets),
             "trackid": reshape_awkward(df["trackid"].values, evt_offsets),
             "parenttype": reshape_awkward(np.array(df["parenttype"], dtype=str), evt_offsets),
             "parentid": reshape_awkward(df["parentid"].values, evt_offsets),
             "creaproc": reshape_awkward(np.array(df["creaproc"], dtype=str), evt_offsets),
             "edproc": reshape_awkward(np.array(df["edproc"], dtype=str), evt_offsets),
-            "evtid": reshape_awkward(df["eventid"].values, evt_offsets),
+            "eventid": reshape_awkward(df["eventid"].values, evt_offsets),
         }
 
         return ak.Array(dictionary)
```

### Comparing `xenon_fuse-1.2.0/fuse/plugins/micro_physics/merge_cluster.py` & `xenon_fuse-1.2.1/fuse/plugins/micro_physics/merge_cluster.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 import strax
 import straxen
 import numpy as np
 import logging
 
+from ...dtypes import (
+    primary_positions_fields,
+    cluster_positions_fields,
+    cluster_id_fields,
+    cluster_misc_fields,
+)
 from ...plugin import FuseBasePlugin
 
 export, __all__ = strax.exporter()
 
 logging.basicConfig(handlers=[logging.StreamHandler()])
 log = logging.getLogger("fuse.micro_physics.merge_cluster")
 
@@ -21,48 +27,28 @@
     is calculated as the energy weighted average of the times of the
     energy deposits. The energy of the merged cluster is the sum of the
     individual energy depositions. The cluster is then classified based
     on either the first interaction in the cluster or the most energetic
     interaction.
     """
 
-    __version__ = "0.3.1"
-
+    __version__ = "0.3.2"
     depends_on = ("geant4_interactions", "cluster_index")
-
     provides = "clustered_interactions"
     data_kind = "clustered_interactions"
 
     save_when = strax.SaveWhen.TARGET
 
-    dtype = [
-        (("x position of the cluster [cm]", "x"), np.float32),
-        (("y position of the cluster [cm]", "y"), np.float32),
-        (("z position of the cluster [cm]", "z"), np.float32),
-        (("Energy of the cluster [keV]", "ed"), np.float32),
-        (("NEST interaction type", "nestid"), np.int8),
-        (("Mass number of the interacting particle", "A"), np.int8),
-        (("Charge number of the interacting particle", "Z"), np.int8),
-        (("Geant4 event ID", "evtid"), np.int32),
-        (("x position of the primary particle [cm]", "x_pri"), np.float32),
-        (("y position of the primary particle [cm]", "y_pri"), np.float32),
-        (("z position of the primary particle [cm]", "z_pri"), np.float32),
-        (("ID of the cluster", "cluster_id"), np.int32),
-        (("Xenon density at the cluster position. Will be set later", "xe_density"), np.float32),
-        (("ID of the volume in which the cluster occured. Will be set later", "vol_id"), np.int8),
-        (
-            (
-                "Flag indicating if a cluster can create a S2 signal. Will be set later",
-                "create_S2",
-            ),
-            np.bool_,
-        ),
-    ]
-
-    dtype = dtype + strax.time_fields
+    dtype = (
+        cluster_positions_fields
+        + cluster_id_fields
+        + cluster_misc_fields
+        + primary_positions_fields
+        + strax.time_fields
+    )
 
     # Config options
     tag_cluster_by = straxen.URLConfig(
         default="take://resource://SIMULATION_CONFIG_FILE.json?fmt=json&take=tag_cluster_by",
         cache=True,
         help="Decide if you tag the cluster "
         "according to first interaction (time) or most energetic (energy) one",
@@ -110,15 +96,15 @@
         result[i]["A"] = A
         result[i]["Z"] = Z
         result[i]["nestid"] = nestid
 
         result[i]["x_pri"] = cluster["x_pri"][main_interaction_index]
         result[i]["y_pri"] = cluster["y_pri"][main_interaction_index]
         result[i]["z_pri"] = cluster["z_pri"][main_interaction_index]
-        result[i]["evtid"] = cluster["evtid"][main_interaction_index]
+        result[i]["eventid"] = cluster["eventid"][main_interaction_index]
 
         # Get cluster id from and save it!
         result[i]["cluster_id"] = cluster["cluster_ids"][main_interaction_index]
 
     return result
```

### Comparing `xenon_fuse-1.2.0/fuse/plugins/micro_physics/wfsim_connection.py` & `xenon_fuse-1.2.1/fuse/plugins/micro_physics/wfsim_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,26 +68,26 @@
 
         ninteractions = len(interactions["ed"])
         res = np.zeros(2 * ninteractions, dtype=self.dtype)
 
         # TODO: Currently not supported rows with only electrons or photons due to
         # this super odd shape
         for i in range(2):
-            structure = np.unique(interactions["evtid"], return_counts=True)[1]
-            evtid = reshape_awkward(interactions["evtid"], structure)
+            structure = np.unique(interactions["eventid"], return_counts=True)[1]
+            eventid = reshape_awkward(interactions["eventid"], structure)
 
-            res["event_number"][i::2] = offset_range(ak.to_numpy(ak.num(evtid)))
+            res["event_number"][i::2] = offset_range(ak.to_numpy(ak.num(eventid)))
             res["type"][i::2] = i + 1
             res["x"][i::2] = interactions["x"]
             res["y"][i::2] = interactions["y"]
             res["z"][i::2] = interactions["z"]
             res["x_pri"][i::2] = interactions["x_pri"]
             res["y_pri"][i::2] = interactions["y_pri"]
             res["z_pri"][i::2] = interactions["z_pri"]
-            res["g4id"][i::2] = interactions["evtid"]
+            res["g4id"][i::2] = interactions["eventid"]
             res["vol_id"][i::2] = interactions["vol_id"]
             res["e_dep"][i::2] = interactions["ed"]
             if "local_field" in res.dtype.names:
                 res["local_field"][i::2] = interactions["e_field"]
 
             recoil = interactions["nestid"]
             res["recoil"][i::2] = np.where(np.isin(recoil, [0, 6, 7, 8, 11]), recoil, 8)
```

### Comparing `xenon_fuse-1.2.0/fuse/plugins/micro_physics/yields.py` & `xenon_fuse-1.2.1/fuse/plugins/micro_physics/yields.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
 import nestpy
 import strax
 import straxen
 import logging
 import pickle
 
+from ...dtypes import quanta_fields
 from ...plugin import FuseBasePlugin
 
 export, __all__ = strax.exporter()
 
 logging.basicConfig(handlers=[logging.StreamHandler()])
 log = logging.getLogger("fuse.micro_physics.yields")
 
@@ -24,21 +25,15 @@
 
     __version__ = "0.2.1"
 
     depends_on = ("interactions_in_roi", "electric_field_values")
     provides = "quanta"
     data_kind = "interactions_in_roi"
 
-    dtype = [
-        (("Number of photons at interaction position", "photons"), np.int32),
-        (("Number of electrons at interaction position", "electrons"), np.int32),
-        (("Number of excitons at interaction position", "excitons"), np.int32),
-    ]
-
-    dtype = dtype + strax.time_fields
+    dtype = quanta_fields + strax.time_fields
 
     save_when = strax.SaveWhen.TARGET
 
     def setup(self):
         super().setup()
 
         if self.deterministic_seed or (self.user_defined_random_seed is not None):
@@ -174,17 +169,15 @@
     provides = "quanta"
     data_kind = "interactions_in_roi"
 
     dtype = [
         ("photons", np.int32),
         ("electrons", np.int32),
         ("excitons", np.int32),
-    ]
-
-    dtype = dtype + strax.time_fields
+    ] + strax.time_fields
 
     # Forbid rechunking
     rechunk_on_save = False
 
     # Config options
     debug = straxen.URLConfig(
         default=False,
@@ -307,21 +300,15 @@
 
 class BBFYields(FuseBasePlugin):
     __version__ = "0.1.1"
 
     depends_on = ("interactions_in_roi", "electric_field_values")
     provides = "quanta"
 
-    dtype = [
-        ("photons", np.int32),
-        ("electrons", np.int32),
-        ("excitons", np.int32),
-    ]
-
-    dtype = dtype + strax.time_fields
+    dtype = quanta_fields + strax.time_fields
 
     def setup(self):
         super().setup()
 
         self.bbfyields = BBF_quanta_generator(self.rng)
 
     def compute(self, interactions_in_roi):
```

### Comparing `xenon_fuse-1.2.0/fuse/plugins/pmt_and_daq/photon_pulses.py` & `xenon_fuse-1.2.1/fuse/plugins/pmt_and_daq/photon_pulses.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.0/fuse/plugins/pmt_and_daq/pmt_afterpulses.py` & `xenon_fuse-1.2.1/fuse/plugins/pmt_and_daq/pmt_afterpulses.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import strax
 import numpy as np
 import straxen
 import logging
 
+from ...dtypes import propagated_photons_fields
 from ...common import pmt_gains
 from ...plugin import FuseBasePlugin
 
 export, __all__ = strax.exporter()
 
 logging.basicConfig(handlers=[logging.StreamHandler()])
 log = logging.getLogger("fuse.pmt_and_daq.pmt_afterpulses")
@@ -26,22 +27,15 @@
 
     depends_on = ("propagated_s2_photons", "propagated_s1_photons")
     provides = "pmt_afterpulses"
     data_kind = "ap_photons"
 
     save_when = strax.SaveWhen.TARGET
 
-    dtype = [
-        (("PMT channel of the photon", "channel"), np.int16),
-        (("Photon creates a double photo-electron emission", "dpe"), np.bool_),
-        (("Sampled PMT gain for the photon", "photon_gain"), np.int32),
-        (("ID of the cluster creating the photon", "cluster_id"), np.int32),
-        (("Type of the photon. S1 (1), S2 (2) or PMT AP (0)", "photon_type"), np.int8),
-    ]
-    dtype = dtype + strax.time_fields
+    dtype = propagated_photons_fields + strax.time_fields
 
     # Config options
 
     enable_pmt_afterpulses = straxen.URLConfig(
         default=True,
         type=bool,
         track=True,
```

### Comparing `xenon_fuse-1.2.0/fuse/plugins/pmt_and_daq/pmt_response_and_daq.py` & `xenon_fuse-1.2.1/fuse/plugins/pmt_and_daq/pmt_response_and_daq.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.0/fuse/plugins/truth_information/cluster_tagging.py` & `xenon_fuse-1.2.1/fuse/plugins/truth_information/cluster_tagging.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,16 +20,15 @@
         ("in_main_s2", np.bool_),
         ("in_alt_s1", np.bool_),
         ("in_alt_s2", np.bool_),
         ("photons_in_main_s1", np.int32),
         ("photons_in_main_s2", np.int32),
         ("photons_in_alt_s1", np.int32),
         ("photons_in_alt_s2", np.int32),
-    ]
-    dtype = dtype + strax.time_fields
+    ] + strax.time_fields
 
     def compute(self, interactions_in_roi, propagated_photons, peaks, events):
         peaks_in_event = strax.split_by_containment(peaks, events)
         photon_in_event = strax.split_touching_windows(propagated_photons, events)
 
         result = np.zeros(len(interactions_in_roi), dtype=self.dtype)
         result["time"] = interactions_in_roi["time"]
```

### Comparing `xenon_fuse-1.2.0/fuse/plugins/truth_information/event_truth.py` & `xenon_fuse-1.2.1/fuse/plugins/truth_information/event_truth.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,16 +14,15 @@
 
     dtype = [
         ("x_obs_truth", np.float32),
         ("y_obs_truth", np.float32),
         ("z_obs_truth", np.float32),
         ("energy_of_main_peaks_truth", np.float32),
         ("total_energy_in_event_truth", np.float32),
-    ]
-    dtype = dtype + strax.time_fields
+    ] + strax.time_fields
 
     def compute(self, interactions_in_roi, propagated_photons, peaks, events):
         peaks_in_event = strax.split_by_containment(peaks, events)
         photons_per_event = strax.split_by_containment(propagated_photons, events)
 
         n_events = len(events)
```

### Comparing `xenon_fuse-1.2.0/fuse/plugins/truth_information/peak_truth.py` & `xenon_fuse-1.2.1/fuse/plugins/truth_information/peak_truth.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,16 +34,15 @@
         ("number_of_contributing_delayed_electrons", np.int16),
         ("average_x_of_contributing_clusters", np.float32),
         ("average_y_of_contributing_clusters", np.float32),
         ("average_z_of_contributing_clusters", np.float32),
         ("average_x_obs_of_contributing_clusters", np.float32),
         ("average_y_obs_of_contributing_clusters", np.float32),
         ("average_z_obs_of_contributing_clusters", np.float32),
-    ]
-    dtype = dtype + strax.time_fields
+    ] + strax.time_fields
 
     gain_model_mc = straxen.URLConfig(
         default="cmt://to_pe_model?version=ONLINE&run_id=plugin.run_id",
         infer_type=False,
         help="PMT gain model",
     )
```

### Comparing `xenon_fuse-1.2.0/fuse/plugins/truth_information/records_truth.py` & `xenon_fuse-1.2.1/fuse/plugins/truth_information/records_truth.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 class RecordsTruth(strax.Plugin):
     """Plugin that computes the truth information for raw_records."""
 
     __version__ = "0.0.2"
 
     depends_on = ("photon_summary", "raw_records")
     provides = "records_truth"
+    data_kind = "raw_records"
 
     dtype = [
         (("Number of S1 photons in record", "s1_photons_in_record"), np.int32),
         (("Number of S2 photons in record", "s2_photons_in_record"), np.int32),
         (("Number of AP photons in record", "ap_photons_in_record"), np.int32),
         (("Sum of the photon gains", "raw_area"), np.float32),
     ]
```

### Comparing `xenon_fuse-1.2.0/fuse/plugins/truth_information/surviving_clusters.py` & `xenon_fuse-1.2.1/fuse/plugins/truth_information/surviving_clusters.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.0/fuse/vertical_merger_plugin.py` & `xenon_fuse-1.2.1/fuse/vertical_merger_plugin.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.0/fuse/volume_plugin.py` & `xenon_fuse-1.2.1/fuse/volume_plugin.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.0/pyproject.toml` & `xenon_fuse-1.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "xenon-fuse"
-version = "1.2.0"
+version = "1.2.1"
 description = "XENON Framework for Unified Simulations of Events"
 authors = [
   "Henning Schulze Eißing, <h_schu55@uni-muenster.de>",
   "Diego Ramírez García, <diego.ramirez@physik.uzh.ch>",
 ]
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `xenon_fuse-1.2.0/tests/_utils.py` & `xenon_fuse-1.2.1/tests/_utils.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.0/tests/test_DetectorPhysics_csv.py` & `xenon_fuse-1.2.1/tests/test_DetectorPhysics_csv.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.0/tests/test_FullChain.py` & `xenon_fuse-1.2.1/tests/test_FullChain.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 import straxen
 from _utils import test_root_file_name
 
 TIMEOUT = 240
 
 
 class TestFullChain(unittest.TestCase):
+    __test__ = True
+
     @classmethod
     def setUpClass(cls):
         cls.temp_dir = tempfile.TemporaryDirectory()
 
         cls.test_context = fuse.context.full_chain_context(
             output_folder=cls.temp_dir.name, run_without_proper_corrections=True
         )
@@ -83,9 +85,18 @@
         # self.test_context.make(self.run_number, "pulse_ids")
 
     @timeout_decorator.timeout(TIMEOUT, exception_message="PMTResponseAndDAQ timed out")
     def test_PMTResponseAndDAQ(self):
         self.test_context.make(self.run_number, "raw_records")
 
 
+class TestChunkedFullChain(TestFullChain):
+    __test__ = True
+
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+        cls.test_context.set_config({"n_interactions_per_chunk": 2})
+
+
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `xenon_fuse-1.2.0/tests/test_FullChain_w_DelayedElectrons.py` & `xenon_fuse-1.2.1/tests/test_FullChain_w_DelayedElectrons.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.0/tests/test_MicroPhysics.py` & `xenon_fuse-1.2.1/tests/test_MicroPhysics.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.0/tests/test_deterministic_seed.py` & `xenon_fuse-1.2.1/tests/test_deterministic_seed.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.0/tests/test_input.py` & `xenon_fuse-1.2.1/tests/test_input.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,173 +38,153 @@
         test_context.set_config(
             {
                 "path": self.temp_dir.name,
                 "file_name": test_root_file_name,
             }
         )
         g4_loaded = test_context.get_array(self.run_number, "geant4_interactions")
-        loaded_event_count = len(np.unique(g4_loaded["evtid"]))
-        assert loaded_event_count == 52, f"Expecting 52 events, but got {loaded_event_count} events"
+        loaded_event_count = len(np.unique(g4_loaded["eventid"]))
+        self.assertTrue(
+            loaded_event_count == 52, f"Expecting 52 events, but got {loaded_event_count} events"
+        )
 
     @timeout_decorator.timeout(TIMEOUT, exception_message="LoadHalf timed out")
     def test_load_half(self):
         test_context = fuse.context.microphysics_context(self.temp_dir.name)
         test_context.set_config(
             {
                 "path": self.temp_dir.name,
                 "file_name": test_root_file_name,
                 "entry_start": 0,
                 "entry_stop": 50,
             }
         )
         g4_loaded = test_context.get_array(self.run_number, "geant4_interactions")
-        loaded_event_count = len(np.unique(g4_loaded["evtid"]))
+        loaded_event_count = len(np.unique(g4_loaded["eventid"]))
 
-        assert loaded_event_count == 26, f"Expecting 26 events, but got {loaded_event_count} events"
+        self.assertTrue(
+            loaded_event_count == 26, f"Expecting 26 events, but got {loaded_event_count} events"
+        )
 
     @timeout_decorator.timeout(TIMEOUT, exception_message="LoadEventIDAll timed out")
     def test_load_eventid_all(self):
         test_context = fuse.context.microphysics_context(self.temp_dir.name)
         test_context.set_config(
             {"path": self.temp_dir.name, "file_name": test_root_file_name, "cut_by_eventid": True}
         )
         g4_loaded = test_context.get_array(self.run_number, "geant4_interactions")
-        loaded_event_count = len(np.unique(g4_loaded["evtid"]))
-        assert loaded_event_count == 52, f"Expecting 52 events, but got {loaded_event_count} events"
+        loaded_event_count = len(np.unique(g4_loaded["eventid"]))
+        self.assertTrue(
+            loaded_event_count == 52, f"Expecting 52 events, but got {loaded_event_count} events"
+        )
 
     @timeout_decorator.timeout(TIMEOUT, exception_message="LoadEventIDHalf timed out")
     def test_load_eventid_half(self):
         test_context = fuse.context.microphysics_context(self.temp_dir.name)
         test_context.set_config(
             {
                 "path": self.temp_dir.name,
                 "file_name": test_root_file_name,
                 "cut_by_eventid": True,
                 "entry_start": 0,
                 "entry_stop": 50,
             }
         )
         g4_loaded = test_context.get_array(self.run_number, "geant4_interactions")
-        loaded_event_count = len(np.unique(g4_loaded["evtid"]))
-        assert loaded_event_count == 23, f"Expecting 23 events, but got {loaded_event_count} events"
+        loaded_event_count = len(np.unique(g4_loaded["eventid"]))
+        self.assertTrue(
+            loaded_event_count == 23, f"Expecting 23 events, but got {loaded_event_count} events"
+        )
 
     @timeout_decorator.timeout(TIMEOUT, exception_message="InvalidArgs0 timed out")
     def test_invalid_args_0(self):
         test_context = fuse.context.microphysics_context(self.temp_dir.name)
         test_context.set_config(
             {
                 "path": self.temp_dir.name,
                 "file_name": test_root_file_name,
                 "cut_by_eventid": False,
                 "entry_start": 75,
                 "entry_stop": 15,
             }
         )
-        try:
+        with self.assertRaises(ValueError):
             test_context.make(self.run_number, "geant4_interactions")
-        except ValueError:
-            return
-        raise RuntimeError("entry_start >= entry_stop does not raise an exception!")
 
     @timeout_decorator.timeout(TIMEOUT, exception_message="InvalidArgs1 timed out")
     def test_invalid_args_1(self):
         test_context = fuse.context.microphysics_context(self.temp_dir.name)
         test_context.set_config(
             {
                 "path": self.temp_dir.name,
                 "file_name": test_root_file_name,
                 "cut_by_eventid": False,
                 "entry_start": 90,
                 "entry_stop": 91,
             }
         )
-        try:
+        with self.assertRaises(ValueError):
             test_context.make(self.run_number, "geant4_interactions")
-        except ValueError:
-            return
-        raise RuntimeError(
-            "An out-of-range entry_start without cut_by_eventid does not raise an exception!"
-        )
 
     @timeout_decorator.timeout(TIMEOUT, exception_message="InvalidArgs2 timed out")
     def test_invalid_args_2(self):
         test_context = fuse.context.microphysics_context(self.temp_dir.name)
         test_context.set_config(
             {
                 "path": self.temp_dir.name,
                 "file_name": test_root_file_name,
                 "cut_by_eventid": False,
                 "entry_start": -2,
                 "entry_stop": -1,
             }
         )
-        try:
+        with self.assertRaises(ValueError):
             test_context.make(self.run_number, "geant4_interactions")
-        except ValueError:
-            return
-        raise RuntimeError(
-            "An out-of-range entry_stop without cut_by_eventid does not raise an exception!"
-        )
 
     @timeout_decorator.timeout(TIMEOUT, exception_message="InvalidArgs3 timed out")
     def test_invalid_args_3(self):
         test_context = fuse.context.microphysics_context(self.temp_dir.name)
         test_context.set_config(
             {
                 "path": self.temp_dir.name,
                 "file_name": test_root_file_name,
                 "cut_by_eventid": True,
                 "entry_start": -2,
                 "entry_stop": -1,
             }
         )
-        try:
+        with self.assertRaises(ValueError):
             test_context.make(self.run_number, "geant4_interactions")
-        except ValueError:
-            return
-        raise RuntimeError(
-            "An out-of-range entry_stop with cut_by_eventid does not raise an exception!"
-        )
 
     @timeout_decorator.timeout(TIMEOUT, exception_message="InvalidArgs4 timed out")
     def test_invalid_args_4(self):
         test_context = fuse.context.microphysics_context(self.temp_dir.name)
         test_context.set_config(
             {
                 "path": self.temp_dir.name,
                 "file_name": test_root_file_name,
                 "cut_by_eventid": True,
                 "entry_start": 102,
                 "entry_stop": 103,
             }
         )
-        try:
+        with self.assertRaises(ValueError):
             test_context.make(self.run_number, "geant4_interactions")
-        except ValueError:
-            return
-        raise RuntimeError(
-            "An out-of-range entry_start with cut_by_eventid does not raise an exception!"
-        )
 
     @timeout_decorator.timeout(TIMEOUT, exception_message="InvalidArgs5 timed out")
     def test_invalid_args_5(self):
         test_context = fuse.context.microphysics_context(self.temp_dir.name)
         test_context.set_config(
             {
                 "path": self.temp_dir.name,
                 "file_name": test_root_file_name,
                 "cut_by_eventid": True,
                 "entry_start": 10,
                 "entry_stop": 11,
             }
         )
-        try:
+        with self.assertRaises(ValueError):
             test_context.make(self.run_number, "geant4_interactions")
-        except ValueError:
-            return
-        raise RuntimeError(
-            "Selecting an empty eventid range with cut_by_eventid does not raise an exception!"
-        )
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `xenon_fuse-1.2.0/tests/test_plugin_random_seed.py` & `xenon_fuse-1.2.1/tests/test_plugin_random_seed.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.0/PKG-INFO` & `xenon_fuse-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xenon-fuse
-Version: 1.2.0
+Version: 1.2.1
 Summary: XENON Framework for Unified Simulations of Events
 Home-page: https://github.com/XENONnT/fuse
 Author: Henning Schulze Eißing,
 Author-email: h_schu55@uni-muenster.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

