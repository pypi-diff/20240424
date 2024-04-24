# Comparing `tmp/antspymm-1.3.1.tar.gz` & `tmp/antspymm-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antspymm-1.3.1.tar", last modified: Fri Apr 19 12:27:53 2024, max compression
+gzip compressed data, was "antspymm-1.3.3.tar", last modified: Wed Apr 24 14:45:06 2024, max compression
```

## Comparing `antspymm-1.3.1.tar` & `antspymm-1.3.3.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:27:53.949706 antspymm-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-19 12:27:45.000000 antspymm-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-19 12:27:45.000000 antspymm-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14586 2024-04-19 12:27:53.949706 antspymm-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13954 2024-04-19 12:27:45.000000 antspymm-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:27:53.925706 antspymm-1.3.1/antspymm/
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-04-19 12:27:45.000000 antspymm-1.3.1/antspymm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   476486 2024-04-19 12:27:45.000000 antspymm-1.3.1/antspymm/mm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:27:53.949706 antspymm-1.3.1/antspymm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14586 2024-04-19 12:27:53.000000 antspymm-1.3.1/antspymm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-19 12:27:53.000000 antspymm-1.3.1/antspymm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 12:27:53.000000 antspymm-1.3.1/antspymm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 12:27:53.000000 antspymm-1.3.1/antspymm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-19 12:27:53.000000 antspymm-1.3.1/antspymm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 12:27:53.000000 antspymm-1.3.1/antspymm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:27:53.945706 antspymm-1.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-19 12:27:45.000000 antspymm-1.3.1/docs/adni_rsfmri_2_nrg_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)   594290 2024-04-19 12:27:45.000000 antspymm-1.3.1/docs/antspymm_data_dictionary.csv
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-19 12:27:45.000000 antspymm-1.3.1/docs/bids_cohort_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-19 12:27:45.000000 antspymm-1.3.1/docs/blind_qc.Rmd
--rw-r--r--   0 runner    (1001) docker     (127)  1055592 2024-04-19 12:27:45.000000 antspymm-1.3.1/docs/blind_qc.html
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-19 12:27:45.000000 antspymm-1.3.1/docs/convert_adni_dti_to_nrg.R
--rw-r--r--   0 runner    (1001) docker     (127)   450556 2024-04-19 12:27:45.000000 antspymm-1.3.1/docs/deepnbm.jpg
--rw-r--r--   0 runner    (1001) docker     (127)   525580 2024-04-19 12:27:45.000000 antspymm-1.3.1/docs/example_antspymm_output.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-19 12:27:45.000000 antspymm-1.3.1/docs/example_run_from_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)    28375 2024-04-19 12:27:45.000000 antspymm-1.3.1/docs/make_dict_table.Rmd
--rw-r--r--   0 runner    (1001) docker     (127)  9773579 2024-04-19 12:27:45.000000 antspymm-1.3.1/docs/make_dict_table.html
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-19 12:27:45.000000 antspymm-1.3.1/docs/nrg_cohort_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-19 12:27:45.000000 antspymm-1.3.1/docs/outlierness.py
--rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-04-19 12:27:45.000000 antspymm-1.3.1/docs/ptbp_nrg.py
--rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-04-19 12:27:45.000000 antspymm-1.3.1/docs/roi_visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-19 12:27:45.000000 antspymm-1.3.1/docs/roi_visualization_ppmi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-04-19 12:27:45.000000 antspymm-1.3.1/docs/ukbb_to_nrg_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-19 12:27:45.000000 antspymm-1.3.1/docs/ukbb_to_nrg_processing2.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 12:27:53.953706 antspymm-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-19 12:27:45.000000 antspymm-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:27:53.949706 antspymm-1.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-19 12:27:45.000000 antspymm-1.3.1/tests/blind_qc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5589 2024-04-19 12:27:45.000000 antspymm-1.3.1/tests/mm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-19 12:27:45.000000 antspymm-1.3.1/tests/mm_nrg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-19 12:27:45.000000 antspymm-1.3.1/tests/outlierness.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-19 12:27:45.000000 antspymm-1.3.1/tests/parallel_study_aggregation_example.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-19 12:27:45.000000 antspymm-1.3.1/tests/test_bids_2_nrg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-19 12:27:45.000000 antspymm-1.3.1/tests/test_deformation_gradient_reo.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-19 12:27:45.000000 antspymm-1.3.1/tests/test_dti_recon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-19 12:27:45.000000 antspymm-1.3.1/tests/test_dti_reg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-19 12:27:45.000000 antspymm-1.3.1/tests/test_dwi_rebasing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-19 12:27:45.000000 antspymm-1.3.1/tests/test_dwi_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-19 12:27:45.000000 antspymm-1.3.1/tests/test_dwi_run_ptbp_scrub.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-19 12:27:45.000000 antspymm-1.3.1/tests/test_flair_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-19 12:27:45.000000 antspymm-1.3.1/tests/test_joint_dti_recon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-19 12:27:45.000000 antspymm-1.3.1/tests/test_mm_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-19 12:27:45.000000 antspymm-1.3.1/tests/test_nrg_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-19 12:27:45.000000 antspymm-1.3.1/tests/test_perfusion_ptbp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-19 12:27:45.000000 antspymm-1.3.1/tests/test_perfusion_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-19 12:27:45.000000 antspymm-1.3.1/tests/test_rsfmri_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-19 12:27:45.000000 antspymm-1.3.1/tests/test_rsfmri_run_minimal.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-19 12:27:45.000000 antspymm-1.3.1/tests/test_ukbb_rsfmri.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-19 12:27:45.000000 antspymm-1.3.1/tests/testsr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-19 12:27:45.000000 antspymm-1.3.1/tests/visualize_tractogram.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:45:06.978081 antspymm-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 14:44:55.000000 antspymm-1.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-24 14:44:55.000000 antspymm-1.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14586 2024-04-24 14:45:06.978081 antspymm-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13954 2024-04-24 14:44:55.000000 antspymm-1.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:45:06.954081 antspymm-1.3.3/antspymm/
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-04-24 14:44:55.000000 antspymm-1.3.3/antspymm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   476733 2024-04-24 14:44:55.000000 antspymm-1.3.3/antspymm/mm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:45:06.978081 antspymm-1.3.3/antspymm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14586 2024-04-24 14:45:06.000000 antspymm-1.3.3/antspymm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-24 14:45:06.000000 antspymm-1.3.3/antspymm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 14:45:06.000000 antspymm-1.3.3/antspymm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 14:45:06.000000 antspymm-1.3.3/antspymm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-24 14:45:06.000000 antspymm-1.3.3/antspymm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 14:45:06.000000 antspymm-1.3.3/antspymm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:45:06.974081 antspymm-1.3.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-24 14:44:55.000000 antspymm-1.3.3/docs/adni_rsfmri_2_nrg_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)   594290 2024-04-24 14:44:55.000000 antspymm-1.3.3/docs/antspymm_data_dictionary.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-24 14:44:55.000000 antspymm-1.3.3/docs/bids_cohort_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-24 14:44:55.000000 antspymm-1.3.3/docs/blind_qc.Rmd
+-rw-r--r--   0 runner    (1001) docker     (127)  1055592 2024-04-24 14:44:55.000000 antspymm-1.3.3/docs/blind_qc.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-24 14:44:55.000000 antspymm-1.3.3/docs/convert_adni_dti_to_nrg.R
+-rw-r--r--   0 runner    (1001) docker     (127)   450556 2024-04-24 14:44:55.000000 antspymm-1.3.3/docs/deepnbm.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   525580 2024-04-24 14:44:55.000000 antspymm-1.3.3/docs/example_antspymm_output.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-24 14:44:55.000000 antspymm-1.3.3/docs/example_run_from_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28375 2024-04-24 14:44:55.000000 antspymm-1.3.3/docs/make_dict_table.Rmd
+-rw-r--r--   0 runner    (1001) docker     (127)  9773579 2024-04-24 14:44:55.000000 antspymm-1.3.3/docs/make_dict_table.html
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-24 14:44:55.000000 antspymm-1.3.3/docs/nrg_cohort_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-24 14:44:55.000000 antspymm-1.3.3/docs/outlierness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-04-24 14:44:55.000000 antspymm-1.3.3/docs/ptbp_nrg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-04-24 14:44:55.000000 antspymm-1.3.3/docs/roi_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-24 14:44:55.000000 antspymm-1.3.3/docs/roi_visualization_ppmi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-04-24 14:44:55.000000 antspymm-1.3.3/docs/ukbb_to_nrg_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-24 14:44:55.000000 antspymm-1.3.3/docs/ukbb_to_nrg_processing2.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 14:45:06.978081 antspymm-1.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-24 14:44:55.000000 antspymm-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:45:06.978081 antspymm-1.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-24 14:44:55.000000 antspymm-1.3.3/tests/blind_qc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5589 2024-04-24 14:44:55.000000 antspymm-1.3.3/tests/mm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-24 14:44:55.000000 antspymm-1.3.3/tests/mm_nrg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-24 14:44:55.000000 antspymm-1.3.3/tests/outlierness.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-24 14:44:55.000000 antspymm-1.3.3/tests/parallel_study_aggregation_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-24 14:44:55.000000 antspymm-1.3.3/tests/test_bids_2_nrg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-24 14:44:55.000000 antspymm-1.3.3/tests/test_deformation_gradient_reo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-24 14:44:55.000000 antspymm-1.3.3/tests/test_dti_recon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-24 14:44:55.000000 antspymm-1.3.3/tests/test_dti_reg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-24 14:44:55.000000 antspymm-1.3.3/tests/test_dwi_rebasing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-24 14:44:55.000000 antspymm-1.3.3/tests/test_dwi_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-24 14:44:55.000000 antspymm-1.3.3/tests/test_dwi_run_ptbp_scrub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-24 14:44:55.000000 antspymm-1.3.3/tests/test_flair_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-24 14:44:55.000000 antspymm-1.3.3/tests/test_joint_dti_recon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-24 14:44:55.000000 antspymm-1.3.3/tests/test_mm_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-24 14:44:55.000000 antspymm-1.3.3/tests/test_nrg_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-24 14:44:55.000000 antspymm-1.3.3/tests/test_perfusion_ptbp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-24 14:44:55.000000 antspymm-1.3.3/tests/test_perfusion_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-24 14:44:55.000000 antspymm-1.3.3/tests/test_rsfmri_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-24 14:44:55.000000 antspymm-1.3.3/tests/test_rsfmri_run_minimal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-24 14:44:55.000000 antspymm-1.3.3/tests/test_ukbb_rsfmri.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-24 14:44:55.000000 antspymm-1.3.3/tests/testsr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-24 14:44:55.000000 antspymm-1.3.3/tests/visualize_tractogram.py
```

### Comparing `antspymm-1.3.1/LICENSE` & `antspymm-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `antspymm-1.3.1/PKG-INFO` & `antspymm-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antspymm
-Version: 1.3.1
+Version: 1.3.3
 Summary: multi-channel/time-series medical image processing with antspyx
 Home-page: https://github.com/stnava/ANTsPyMM
 Author: Avants, Gosselin, Tustison, Reardon
 Author-email: stnava@gmail.com
 License: Apache 2.0
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE
```

### Comparing `antspymm-1.3.1/README.md` & `antspymm-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `antspymm-1.3.1/antspymm/__init__.py` & `antspymm-1.3.3/antspymm/__init__.py`

 * *Files identical despite different names*

### Comparing `antspymm-1.3.1/antspymm/mm.py` & `antspymm-1.3.3/antspymm/mm.py`

 * *Files 0% similar despite different names*

```diff
@@ -26950,2832 +26950,2847 @@
 00069450: 6963 7469 6f6e 6172 795f 7061 7468 290a  ictionary_path).
 00069460: 2020 2020 6d79 6469 6374 203d 206d 7964      mydict = myd
 00069470: 6963 745b 7e6d 7964 6963 745b 274d 6561  ict[~mydict['Mea
 00069480: 7375 7265 6d65 6e74 275d 2e73 7472 2e63  surement'].str.c
 00069490: 6f6e 7461 696e 7328 2274 7261 6374 6f67  ontains("tractog
 000694a0: 7261 7068 792d 6261 7365 6420 636f 6e6e  raphy-based conn
 000694b0: 6563 7469 7669 7479 222c 206e 613d 4661  ectivity", na=Fa
-000694c0: 6c73 6529 5d0a 0a20 2020 2023 204c 6f61  lse)]..    # Loa
-000694d0: 6420 696d 6167 6520 616e 6420 7072 6f63  d image and proc
-000694e0: 6573 7320 6974 0a20 2020 2065 6467 6569  ess it.    edgei
-000694f0: 6d67 203d 2061 6e74 732e 694d 6174 6828  mg = ants.iMath(
-00069500: 6272 6169 6e5f 696d 6167 652c 224e 6f72  brain_image,"Nor
-00069510: 6d61 6c69 7a65 2229 0a20 2020 2069 6620  malize").    if 
-00069520: 6564 6765 5f69 6d61 6765 5f64 696c 6174  edge_image_dilat
-00069530: 696f 6e20 3e20 303a 0a20 2020 2020 2020  ion > 0:.       
-00069540: 2065 6467 6569 6d67 203d 2061 6e74 732e   edgeimg = ants.
-00069550: 694d 6174 6828 2065 6467 6569 6d67 2c20  iMath( edgeimg, 
-00069560: 224d 4422 2c20 6564 6765 5f69 6d61 6765  "MD", edge_image
-00069570: 5f64 696c 6174 696f 6e29 0a0a 2020 2020  _dilation)..    
-00069580: 2320 4465 6669 6e65 206c 6973 7473 2061  # Define lists a
-00069590: 6e64 2064 6174 6120 6672 616d 6573 0a20  nd data frames. 
-000695a0: 2020 2070 6f73 7466 6978 203d 205b 2762     postfix = ['b
-000695b0: 6627 2c20 2763 6974 3136 386c 6162 272c  f', 'cit168lab',
-000695c0: 2027 6d74 6c27 2c20 2763 6572 6562 656c   'mtl', 'cerebel
-000695d0: 6c75 6d27 2c20 2764 6b74 5f63 6f72 7465  lum', 'dkt_corte
-000695e0: 7827 2c27 6272 6169 6e73 7465 6d27 2c27  x','brainstem','
-000695f0: 4a48 555f 776d 272c 2779 656f 275d 0a20  JHU_wm','yeo']. 
-00069600: 2020 2061 746c 6173 203d 205b 2742 4627     atlas = ['BF'
-00069610: 2c20 2743 4954 3136 3827 2c20 274d 544c  , 'CIT168', 'MTL
-00069620: 272c 2027 5475 7374 6973 6f6e 436f 6272  ', 'TustisonCobr
-00069630: 6127 2c20 2764 6573 696b 616e 2d6b 696c  a', 'desikan-kil
-00069640: 6c69 616e 792d 746f 7572 7669 6c6c 6527  liany-tourville'
-00069650: 2c27 6272 6169 6e73 7465 6d27 2c27 4a48  ,'brainstem','JH
-00069660: 555f 776d 272c 2779 656f 275d 0a20 2020  U_wm','yeo'].   
-00069670: 2070 6f73 7464 6573 6320 3d20 5b27 6e62   postdesc = ['nb
-00069680: 6d33 4348 3133 272c 2027 4349 5431 3638  m3CH13', 'CIT168
-00069690: 5f52 6569 6e66 5f4c 6561 726e 5f76 315f  _Reinf_Learn_v1_
-000696a0: 6c61 6265 6c5f 6465 7363 7269 7074 696f  label_descriptio
-000696b0: 6e73 5f70 6164 272c 2027 6d74 6c5f 6465  ns_pad', 'mtl_de
-000696c0: 7363 7269 7074 696f 6e27 2c20 2763 6572  scription', 'cer
-000696d0: 6562 656c 6c75 6d27 2c20 2764 6b74 272c  ebellum', 'dkt',
-000696e0: 2743 4954 3136 385f 5431 775f 3730 3075  'CIT168_T1w_700u
-000696f0: 6d5f 7061 645f 6164 6e69 5f62 7261 696e  m_pad_adni_brain
-00069700: 7374 656d 272c 2746 415f 4a48 555f 6c61  stem','FA_JHU_la
-00069710: 6265 6c73 5f65 6469 7465 6427 2c27 7070  bels_edited','pp
-00069720: 6d69 5f74 656d 706c 6174 655f 3530 3050  mi_template_500P
-00069730: 6172 6365 6c73 5f59 656f 3230 3131 5f31  arcels_Yeo2011_1
-00069740: 374e 6574 776f 726b 735f 3230 3233 5f68  7Networks_2023_h
-00069750: 6f6d 6f74 6f70 6963 275d 0a20 2020 2073  omotopic'].    s
-00069760: 7461 7464 6620 3d20 7064 2e44 6174 6146  tatdf = pd.DataF
-00069770: 7261 6d65 287b 2769 6d67 273a 2070 6f73  rame({'img': pos
-00069780: 7466 6978 2c20 2761 746c 6173 273a 2061  tfix, 'atlas': a
-00069790: 746c 6173 2c20 2763 7376 6465 7363 7269  tlas, 'csvdescri
-000697a0: 7074 273a 2070 6f73 7464 6573 637d 290a  pt': postdesc}).
-000697b0: 2020 2020 7465 6d70 6c61 7465 7072 6566      templatepref
-000697c0: 6978 203d 2027 7e2f 2e61 6e74 7370 796d  ix = '~/.antspym
-000697d0: 6d2f 5050 4d49 5f74 656d 706c 6174 6530  m/PPMI_template0
-000697e0: 5f27 0a20 2020 2023 2049 7465 7261 7465  _'.    # Iterate
-000697f0: 2074 6872 6f75 6768 2063 6f6c 756d 6e73   through columns
-00069800: 2061 6e64 2063 7265 6174 6520 6669 6775   and create figu
-00069810: 7265 730a 2020 2020 636f 6c32 7669 7a20  res.    col2viz 
-00069820: 3d20 2776 616c 7565 7327 0a20 2020 2069  = 'values'.    i
-00069830: 6620 5472 7565 3a0a 2020 2020 2020 2020  f True:.        
-00069840: 616e 6174 746f 7368 6f77 203d 207a 7a5b  anattoshow = zz[
-00069850: 2761 6e61 7427 5d2e 756e 6971 7565 2829  'anat'].unique()
-00069860: 0a20 2020 2020 2020 2069 6620 7665 7262  .        if verb
-00069870: 6f73 653a 0a20 2020 2020 2020 2020 2020  ose:.           
-00069880: 2070 7269 6e74 2863 6f6c 3276 697a 290a   print(col2viz).
-00069890: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-000698a0: 7428 616e 6174 746f 7368 6f77 290a 2020  t(anattoshow).  
-000698b0: 2020 2020 2020 2320 5265 7374 206f 6620        # Rest of 
-000698c0: 796f 7572 2063 6f64 6520 666f 7220 6669  your code for fi
-000698d0: 6775 7265 2063 7265 6174 696f 6e20 676f  gure creation go
-000698e0: 6573 2068 6572 652e 2e2e 0a20 2020 2020  es here....     
-000698f0: 2020 2061 6464 656d 203d 2065 6467 6569     addem = edgei
-00069900: 6d67 202a 2030 0a20 2020 2020 2020 2066  mg * 0.        f
-00069910: 6f72 206b 2069 6e20 7261 6e67 6528 6c65  or k in range(le
-00069920: 6e28 616e 6174 746f 7368 6f77 2929 3a0a  n(anattoshow)):.
-00069930: 2020 2020 2020 2020 2020 2020 6966 2076              if v
-00069940: 6572 626f 7365 3a0a 2020 2020 2020 2020  erbose:.        
-00069950: 2020 2020 2020 2020 7072 696e 7428 7374          print(st
-00069960: 7228 6b29 202b 2020 2220 2220 2b20 616e  r(k) +  " " + an
-00069970: 6174 746f 7368 6f77 5b6b 5d20 2029 0a20  attoshow[k]  ). 
-00069980: 2020 2020 2020 2020 2020 206d 7973 7562             mysub
-00069990: 203d 207a 7a5b 7a7a 5b27 616e 6174 275d   = zz[zz['anat']
-000699a0: 2e73 7472 2e63 6f6e 7461 696e 7328 616e  .str.contains(an
-000699b0: 6174 746f 7368 6f77 5b6b 5d29 5d0a 2020  attoshow[k])].  
-000699c0: 2020 2020 2020 2020 2020 616e 6174 7365            anatse
-000699d0: 6172 3d72 652e 7375 6228 2264 7469 2e66  ar=re.sub("dti.f
-000699e0: 6122 2c22 222c 616e 6174 746f 7368 6f77  a","",anattoshow
-000699f0: 5b6b 5d29 0a20 2020 2020 2020 2020 2020  [k]).           
-00069a00: 2061 6e61 7473 6561 723d 7265 2e73 7562   anatsear=re.sub
-00069a10: 2822 7431 2e76 6f6c 6173 796d 222c 2222  ("t1.volasym",""
-00069a20: 2c61 6e61 7473 6561 7229 0a20 2020 2020  ,anatsear).     
-00069a30: 2020 2020 2020 2061 6e61 7473 6561 723d         anatsear=
-00069a40: 7265 2e73 7562 2822 7431 2e74 686b 6173  re.sub("t1.thkas
-00069a50: 796d 222c 2222 2c61 6e61 7473 6561 7229  ym","",anatsear)
-00069a60: 0a20 2020 2020 2020 2020 2020 2061 6e61  .            ana
-00069a70: 7473 6561 723d 7265 2e73 7562 2822 7431  tsear=re.sub("t1
-00069a80: 2e61 7265 6161 7379 6d22 2c22 222c 616e  .areaasym","",an
-00069a90: 6174 7365 6172 290a 2020 2020 2020 2020  atsear).        
-00069aa0: 2020 2020 616e 6174 7365 6172 3d72 652e      anatsear=re.
-00069ab0: 7375 6228 2274 312e 766f 6c2e 222c 2222  sub("t1.vol.",""
-00069ac0: 2c61 6e61 7473 6561 7229 0a20 2020 2020  ,anatsear).     
-00069ad0: 2020 2020 2020 2061 6e61 7473 6561 723d         anatsear=
-00069ae0: 7265 2e73 7562 2822 7431 2e74 686b 2e22  re.sub("t1.thk."
-00069af0: 2c22 222c 616e 6174 7365 6172 290a 2020  ,"",anatsear).  
-00069b00: 2020 2020 2020 2020 2020 616e 6174 7365            anatse
-00069b10: 6172 3d72 652e 7375 6228 2274 312e 6172  ar=re.sub("t1.ar
-00069b20: 6561 2e22 2c22 222c 616e 6174 7365 6172  ea.","",anatsear
-00069b30: 290a 2020 2020 2020 2020 2020 2020 616e  ).            an
-00069b40: 6174 7365 6172 3d72 652e 7375 6228 2261  atsear=re.sub("a
-00069b50: 7379 6d64 702e 222c 2222 2c61 6e61 7473  symdp.","",anats
-00069b60: 6561 7229 0a20 2020 2020 2020 2020 2020  ear).           
-00069b70: 2061 6e61 7473 6561 723d 7265 2e73 7562   anatsear=re.sub
-00069b80: 2822 6173 796d 2e22 2c22 222c 616e 6174  ("asym.","",anat
-00069b90: 7365 6172 290a 2020 2020 2020 2020 2020  sear).          
-00069ba0: 2020 616e 6174 7365 6172 3d72 652e 7375    anatsear=re.su
-00069bb0: 6228 2264 7469 2e6d 642e 222c 2222 2c61  b("dti.md.","",a
-00069bc0: 6e61 7473 6561 7229 0a20 2020 2020 2020  natsear).       
-00069bd0: 2020 2020 2061 6e61 7473 6561 723d 7265       anatsear=re
-00069be0: 2e73 7562 2822 6474 692e 6661 2e22 2c22  .sub("dti.fa.","
-00069bf0: 222c 616e 6174 7365 6172 290a 2020 2020  ",anatsear).    
-00069c00: 2020 2020 2020 2020 616e 6174 7365 6172          anatsear
-00069c10: 3d72 652e 7375 6228 2264 7469 2e6d 6422  =re.sub("dti.md"
-00069c20: 2c22 222c 616e 6174 7365 6172 290a 2020  ,"",anatsear).  
-00069c30: 2020 2020 2020 2020 2020 616e 6174 7365            anatse
-00069c40: 6172 3d72 652e 7375 6228 2264 7469 2e6d  ar=re.sub("dti.m
-00069c50: 6561 6e2e 6d64 2e22 2c22 222c 616e 6174  ean.md.","",anat
-00069c60: 7365 6172 290a 2020 2020 2020 2020 2020  sear).          
-00069c70: 2020 616e 6174 7365 6172 3d72 652e 7375    anatsear=re.su
-00069c80: 6228 2264 7469 2e6d 6561 6e2e 6661 2e22  b("dti.mean.fa."
-00069c90: 2c22 222c 616e 6174 7365 6172 290a 2020  ,"",anatsear).  
-00069ca0: 2020 2020 2020 2020 2020 616e 6174 7365            anatse
-00069cb0: 6172 3d72 652e 7375 6228 226c 7261 7667  ar=re.sub("lravg
-00069cc0: 222c 2222 2c61 6e61 7473 6561 7229 0a20  ","",anatsear). 
-00069cd0: 2020 2020 2020 2020 2020 2061 746c 6173             atlas
-00069ce0: 7365 6172 6368 203d 206d 7964 6963 745b  search = mydict[
-00069cf0: 2774 6964 796e 616d 6573 275d 2e73 7472  'tidynames'].str
-00069d00: 2e63 6f6e 7461 696e 7328 616e 6174 7365  .contains(anatse
-00069d10: 6172 290a 2020 2020 2020 2020 2020 2020  ar).            
-00069d20: 6966 2061 746c 6173 7365 6172 6368 2e73  if atlassearch.s
-00069d30: 756d 2829 203e 2030 3a0a 2020 2020 2020  um() > 0:.      
-00069d40: 2020 2020 2020 2020 2020 7768 6963 6861            whicha
-00069d50: 746c 6173 203d 206d 7964 6963 745b 6174  tlas = mydict[at
-00069d60: 6c61 7373 6561 7263 685d 5b27 4174 6c61  lassearch]['Atla
-00069d70: 7327 5d2e 696c 6f63 5b30 5d0a 2020 2020  s'].iloc[0].    
-00069d80: 2020 2020 2020 2020 2020 2020 6f67 6c61              ogla
-00069d90: 6265 6c6e 616d 6520 3d20 6d79 6469 6374  belname = mydict
-00069da0: 5b61 746c 6173 7365 6172 6368 5d5b 274c  [atlassearch]['L
-00069db0: 6162 656c 275d 2e69 6c6f 635b 305d 0a20  abel'].iloc[0]. 
-00069dc0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00069dd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00069de0: 2070 7269 6e74 2861 6e61 7473 6561 7229   print(anatsear)
-00069df0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00069e00: 206f 676c 6162 656c 6e61 6d65 3d27 756e   oglabelname='un
-00069e10: 6b6e 6f77 6e27 0a20 2020 2020 2020 2020  known'.         
-00069e20: 2020 2020 2020 2077 6869 6368 6174 6c61         whichatla
-00069e30: 733d 4e6f 6e65 0a20 2020 2020 2020 2020  s=None.         
-00069e40: 2020 2069 6620 7665 7262 6f73 653a 0a20     if verbose:. 
-00069e50: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00069e60: 7269 6e74 2822 6f67 6c61 6265 6c6e 616d  rint("oglabelnam
-00069e70: 6520 2220 2b20 6f67 6c61 6265 6c6e 616d  e " + oglabelnam
-00069e80: 6520 290a 2020 2020 2020 2020 2020 2020  e ).            
-00069e90: 7661 6c73 3276 697a 203d 206d 7973 7562  vals2viz = mysub
-00069ea0: 5b63 6f6c 3276 697a 5d2e 6167 6728 5b27  [col2viz].agg(['
-00069eb0: 6d69 6e27 2c20 276d 6178 275d 290a 2020  min', 'max']).  
-00069ec0: 2020 2020 2020 2020 2020 7661 6c73 3276            vals2v
-00069ed0: 697a 203d 2076 616c 7332 7669 7a5b 6162  iz = vals2viz[ab
-00069ee0: 7328 7661 6c73 3276 697a 292e 6964 786d  s(vals2viz).idxm
-00069ef0: 6178 2829 5d0a 2020 2020 2020 2020 2020  ax()].          
-00069f00: 2020 6d79 6578 7420 3d20 4e6f 6e65 0a20    myext = None. 
-00069f10: 2020 2020 2020 2020 2020 2069 6620 2764             if 'd
-00069f20: 6b74 636f 7274 6578 2720 696e 2061 6e61  ktcortex' in ana
-00069f30: 7474 6f73 686f 775b 6b5d 3a0a 2020 2020  ttoshow[k]:.    
-00069f40: 2020 2020 2020 2020 2020 2020 6d79 6578              myex
-00069f50: 7420 3d20 2764 6b74 5f63 6f72 7465 7827  t = 'dkt_cortex'
-00069f60: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
-00069f70: 6620 2763 6974 3136 3827 2069 6e20 616e  f 'cit168' in an
-00069f80: 6174 746f 7368 6f77 5b6b 5d3a 0a20 2020  attoshow[k]:.   
-00069f90: 2020 2020 2020 2020 2020 2020 206d 7965               mye
-00069fa0: 7874 203d 2027 6369 7431 3638 6c61 6227  xt = 'cit168lab'
-00069fb0: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
-00069fc0: 6620 276d 746c 2720 696e 2061 6e61 7474  f 'mtl' in anatt
-00069fd0: 6f73 686f 775b 6b5d 3a0a 2020 2020 2020  oshow[k]:.      
-00069fe0: 2020 2020 2020 2020 2020 6d79 6578 7420            myext 
-00069ff0: 3d20 276d 746c 270a 2020 2020 2020 2020  = 'mtl'.        
-0006a000: 2020 2020 2020 2020 6f67 6c61 6265 6c6e          oglabeln
-0006a010: 616d 653d 7265 2e73 7562 2827 6d74 6c27  ame=re.sub('mtl'
-0006a020: 2c20 2727 2c61 6e61 7473 6561 7229 0a20  , '',anatsear). 
-0006a030: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-0006a040: 2763 6572 6562 656c 6c75 6d27 2069 6e20  'cerebellum' in 
-0006a050: 616e 6174 746f 7368 6f77 5b6b 5d3a 0a20  anattoshow[k]:. 
-0006a060: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-0006a070: 7965 7874 203d 2027 6365 7265 6265 6c6c  yext = 'cerebell
-0006a080: 756d 270a 2020 2020 2020 2020 2020 2020  um'.            
-0006a090: 2020 2020 6f67 6c61 6265 6c6e 616d 653d      oglabelname=
-0006a0a0: 7265 2e73 7562 2827 6365 7265 6265 6c6c  re.sub('cerebell
-0006a0b0: 756d 272c 2027 272c 616e 6174 7365 6172  um', '',anatsear
-0006a0c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0006a0d0: 2020 2320 6f67 6c61 6265 6c6e 616d 653d    # oglabelname=
-0006a0e0: 6f67 6c61 6265 6c6e 616d 655b 323a 5d0a  oglabelname[2:].
-0006a0f0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-0006a100: 2027 6272 6169 6e73 7465 6d27 2069 6e20   'brainstem' in 
-0006a110: 616e 6174 746f 7368 6f77 5b6b 5d3a 0a20  anattoshow[k]:. 
-0006a120: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-0006a130: 7965 7874 203d 2027 6272 6169 6e73 7465  yext = 'brainste
-0006a140: 6d27 0a20 2020 2020 2020 2020 2020 2065  m'.            e
-0006a150: 6c69 6620 616e 7928 6974 656d 2069 6e20  lif any(item in 
-0006a160: 616e 6174 746f 7368 6f77 5b6b 5d20 666f  anattoshow[k] fo
-0006a170: 7220 6974 656d 2069 6e20 5b27 6e62 6d27  r item in ['nbm'
-0006a180: 2c20 2762 6627 5d29 3a0a 2020 2020 2020  , 'bf']):.      
-0006a190: 2020 2020 2020 2020 2020 6d79 6578 7420            myext 
-0006a1a0: 3d20 2762 6627 0a20 2020 2020 2020 2020  = 'bf'.         
-0006a1b0: 2020 2020 2020 206f 676c 6162 656c 6e61         oglabelna
-0006a1c0: 6d65 3d72 652e 7375 6228 7227 5c2e 272c  me=re.sub(r'\.',
-0006a1d0: 2027 5f27 2c61 6e61 7473 6561 7229 0a20   '_',anatsear). 
-0006a1e0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-0006a1f0: 7768 6963 6861 746c 6173 203d 3d20 276a  whichatlas == 'j
-0006a200: 6f68 6e73 2068 6f70 6b69 6e73 2077 6869  ohns hopkins whi
-0006a210: 7465 206d 6174 7465 7227 3a0a 2020 2020  te matter':.    
-0006a220: 2020 2020 2020 2020 2020 2020 6d79 6578              myex
-0006a230: 7420 3d20 274a 4855 5f77 6d27 0a20 2020  t = 'JHU_wm'.   
-0006a240: 2020 2020 2020 2020 2065 6c69 6620 7768           elif wh
-0006a250: 6963 6861 746c 6173 203d 3d20 2764 6573  ichatlas == 'des
-0006a260: 696b 616e 2d6b 696c 6c69 616e 792d 746f  ikan-killiany-to
-0006a270: 7572 7669 6c6c 6527 3a0a 2020 2020 2020  urville':.      
-0006a280: 2020 2020 2020 2020 2020 6d79 6578 7420            myext 
-0006a290: 3d20 2764 6b74 5f63 6f72 7465 7827 0a20  = 'dkt_cortex'. 
-0006a2a0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-0006a2b0: 7768 6963 6861 746c 6173 203d 3d20 2743  whichatlas == 'C
-0006a2c0: 4954 3136 3827 3a0a 2020 2020 2020 2020  IT168':.        
-0006a2d0: 2020 2020 2020 2020 6d79 6578 7420 3d20          myext = 
-0006a2e0: 2763 6974 3136 386c 6162 270a 2020 2020  'cit168lab'.    
-0006a2f0: 2020 2020 2020 2020 656c 6966 2077 6869          elif whi
-0006a300: 6368 6174 6c61 7320 3d3d 2027 4246 273a  chatlas == 'BF':
-0006a310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0006a320: 206d 7965 7874 203d 2027 6266 270a 2020   myext = 'bf'.  
-0006a330: 2020 2020 2020 2020 2020 2020 2020 6f67                og
-0006a340: 6c61 6265 6c6e 616d 653d 7265 2e73 7562  labelname=re.sub
-0006a350: 2827 6266 272c 2027 272c 6f67 6c61 6265  ('bf', '',oglabe
-0006a360: 6c6e 616d 6529 0a20 2020 2020 2020 2020  lname).         
-0006a370: 2020 2065 6c69 6620 7768 6963 6861 746c     elif whichatl
-0006a380: 6173 203d 3d20 2779 656f 5f68 6f6d 6f74  as == 'yeo_homot
-0006a390: 6f70 6963 273a 0a20 2020 2020 2020 2020  opic':.         
-0006a3a0: 2020 2020 2020 206d 7965 7874 203d 2027         myext = '
-0006a3b0: 7965 6f27 0a20 2020 2020 2020 2020 2020  yeo'.           
-0006a3c0: 2069 6620 6d79 6578 7420 6973 204e 6f6e   if myext is Non
-0006a3d0: 6520 616e 6420 7665 7262 6f73 653a 0a20  e and verbose:. 
-0006a3e0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0006a3f0: 7269 6e74 2820 224d 5945 5854 2022 202b  rint( "MYEXT " +
-0006a400: 2061 6e61 7474 6f73 686f 775b 6b5d 202b   anattoshow[k] +
-0006a410: 2027 2075 6e66 6f75 6e64 2027 202b 2077   ' unfound ' + w
-0006a420: 6869 6368 6174 6c61 7320 290a 2020 2020  hichatlas ).    
-0006a430: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0006a440: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0006a450: 2076 6572 626f 7365 3a0a 2020 2020 2020   verbose:.      
-0006a460: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-0006a470: 696e 7428 2022 4d59 4558 5420 2220 2b20  int( "MYEXT " + 
-0006a480: 6d79 6578 7420 290a 0a20 2020 2020 2020  myext )..       
-0006a490: 2020 2020 2069 6620 6d79 6578 7420 3d3d       if myext ==
-0006a4a0: 2027 6369 7431 3638 6c61 6227 3a0a 2020   'cit168lab':.  
-0006a4b0: 2020 2020 2020 2020 2020 2020 2020 6f67                og
-0006a4c0: 6c61 6265 6c6e 616d 653d 7265 2e73 7562  labelname=re.sub
-0006a4d0: 2822 6369 7431 3638 222c 2222 2c6f 676c  ("cit168","",ogl
-0006a4e0: 6162 656c 6e61 6d65 290a 2020 2020 2020  abelname).      
-0006a4f0: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
-0006a500: 2020 2066 6f72 206a 2069 6e20 706f 7374     for j in post
-0006a510: 6669 783a 0a20 2020 2020 2020 2020 2020  fix:.           
-0006a520: 2020 2020 2069 6620 6a20 3d3d 2022 646b       if j == "dk
-0006a530: 745f 636f 7274 6578 223a 0a20 2020 2020  t_cortex":.     
-0006a540: 2020 2020 2020 2020 2020 2020 2020 206a                 j
-0006a550: 203d 2027 646b 7463 6f72 7465 7827 0a20   = 'dktcortex'. 
-0006a560: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0006a570: 6620 6a20 3d3d 2022 6465 6570 5f63 6974  f j == "deep_cit
-0006a580: 3136 386c 6162 223a 0a20 2020 2020 2020  168lab":.       
-0006a590: 2020 2020 2020 2020 2020 2020 206a 203d               j =
-0006a5a0: 2027 6465 6570 5f63 6974 3136 3827 0a20   'deep_cit168'. 
-0006a5b0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0006a5c0: 6e61 7474 6f73 686f 775b 6b5d 203d 2061  nattoshow[k] = a
-0006a5d0: 6e61 7474 6f73 686f 775b 6b5d 2e72 6570  nattoshow[k].rep
-0006a5e0: 6c61 6365 286a 2c20 2222 290a 2020 2020  lace(j, "").    
-0006a5f0: 2020 2020 2020 2020 6966 2076 6572 626f          if verbo
-0006a600: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0006a610: 2020 2020 7072 696e 7428 2061 6e61 7474      print( anatt
-0006a620: 6f73 686f 775b 6b5d 202b 2022 2022 202b  oshow[k] + " " +
-0006a630: 2073 7472 2820 7661 6c73 3276 697a 2029   str( vals2viz )
-0006a640: 2029 0a20 2020 2020 2020 2020 2020 206d   ).            m
-0006a650: 7961 746c 6173 203d 2061 746c 6173 5b70  yatlas = atlas[p
-0006a660: 6f73 7466 6978 2e69 6e64 6578 286d 7965  ostfix.index(mye
-0006a670: 7874 295d 0a20 2020 2020 2020 2020 2020  xt)].           
-0006a680: 2063 6f72 7265 6374 6465 7363 7269 7074   correctdescript
-0006a690: 203d 2070 6f73 7464 6573 635b 706f 7374   = postdesc[post
-0006a6a0: 6669 782e 696e 6465 7828 6d79 6578 7429  fix.index(myext)
-0006a6b0: 5d0a 2020 2020 2020 2020 2020 2020 6c6f  ].            lo
-0006a6c0: 6366 696c 656e 616d 6520 3d20 2074 656d  cfilename =  tem
-0006a6d0: 706c 6174 6570 7265 6669 7820 2b20 6d79  plateprefix + my
-0006a6e0: 6578 7420 2b20 272e 6e69 692e 677a 270a  ext + '.nii.gz'.
-0006a6f0: 2020 2020 2020 2020 2020 2020 6966 2076              if v
-0006a700: 6572 626f 7365 3a0a 2020 2020 2020 2020  erbose:.        
-0006a710: 2020 2020 2020 2020 7072 696e 7428 206c          print( l
-0006a720: 6f63 6669 6c65 6e61 6d65 2029 0a20 2020  ocfilename ).   
-0006a730: 2020 2020 2020 2020 2069 6620 6d79 6578           if myex
-0006a740: 7420 3d3d 2027 7965 6f27 3a0a 2020 2020  t == 'yeo':.    
-0006a750: 2020 2020 2020 2020 2020 2020 6f67 6c61              ogla
-0006a760: 6265 6c6e 616d 653d 6f67 6c61 6265 6c6e  belname=oglabeln
-0006a770: 616d 652e 6c6f 7765 7228 290a 2020 2020  ame.lower().    
-0006a780: 2020 2020 2020 2020 2020 2020 6f67 6c61              ogla
-0006a790: 6265 6c6e 616d 653d 7265 2e73 7562 2822  belname=re.sub("
-0006a7a0: 7273 666d 7269 5f66 636e 7870 726f 3132  rsfmri_fcnxpro12
-0006a7b0: 325f 222c 2222 2c6f 676c 6162 656c 6e61  2_","",oglabelna
-0006a7c0: 6d65 290a 2020 2020 2020 2020 2020 2020  me).            
-0006a7d0: 2020 2020 6f67 6c61 6265 6c6e 616d 653d      oglabelname=
-0006a7e0: 7265 2e73 7562 2822 7273 666d 7269 5f66  re.sub("rsfmri_f
-0006a7f0: 636e 7870 726f 3132 395f 222c 2222 2c6f  cnxpro129_","",o
-0006a800: 676c 6162 656c 6e61 6d65 290a 2020 2020  glabelname).    
-0006a810: 2020 2020 2020 2020 2020 2020 6f67 6c61              ogla
-0006a820: 6265 6c6e 616d 653d 7265 2e73 7562 2822  belname=re.sub("
-0006a830: 7273 666d 7269 5f66 636e 7870 726f 3133  rsfmri_fcnxpro13
-0006a840: 345f 222c 2222 2c6f 676c 6162 656c 6e61  4_","",oglabelna
-0006a850: 6d65 290a 2020 2020 2020 2020 2020 2020  me).            
-0006a860: 2020 2020 6c6f 6366 696c 656e 616d 6520      locfilename 
-0006a870: 3d20 227e 2f2e 616e 7473 7079 6d6d 2f70  = "~/.antspymm/p
-0006a880: 706d 695f 7465 6d70 6c61 7465 5f35 3030  pmi_template_500
-0006a890: 5061 7263 656c 735f 5965 6f32 3031 315f  Parcels_Yeo2011_
-0006a8a0: 3137 4e65 7477 6f72 6b73 5f32 3032 335f  17Networks_2023_
-0006a8b0: 686f 6d6f 746f 7069 632e 6e69 692e 677a  homotopic.nii.gz
-0006a8c0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-0006a8d0: 2020 6174 6c61 7344 6573 6372 6970 7420    atlasDescript 
-0006a8e0: 3d20 7064 2e72 6561 645f 6373 7628 6622  = pd.read_csv(f"
-0006a8f0: 7e2f 2e61 6e74 7370 796d 6d2f 7b63 6f72  ~/.antspymm/{cor
-0006a900: 7265 6374 6465 7363 7269 7074 7d2e 6373  rectdescript}.cs
-0006a910: 7622 290a 2020 2020 2020 2020 2020 2020  v").            
-0006a920: 2020 2020 6174 6c61 7344 6573 6372 6970      atlasDescrip
-0006a930: 742e 7265 6e61 6d65 2863 6f6c 756d 6e73  t.rename(columns
-0006a940: 3d7b 2753 7973 7465 6d4e 616d 6527 3a20  ={'SystemName': 
-0006a950: 2744 6573 6372 6970 7469 6f6e 277d 2c20  'Description'}, 
-0006a960: 696e 706c 6163 653d 5472 7565 290a 2020  inplace=True).  
-0006a970: 2020 2020 2020 2020 2020 2020 2020 6174                at
-0006a980: 6c61 7344 6573 6372 6970 742e 7265 6e61  lasDescript.rena
-0006a990: 6d65 2863 6f6c 756d 6e73 3d7b 2752 4f49  me(columns={'ROI
-0006a9a0: 273a 2027 4c61 6265 6c27 7d2c 2069 6e70  ': 'Label'}, inp
-0006a9b0: 6c61 6365 3d54 7275 6529 0a20 2020 2020  lace=True).     
-0006a9c0: 2020 2020 2020 2020 2020 2061 746c 6173             atlas
-0006a9d0: 4465 7363 7269 7074 5b27 4465 7363 7269  Descript['Descri
-0006a9e0: 7074 696f 6e27 5d20 3d20 6174 6c61 7344  ption'] = atlasD
-0006a9f0: 6573 6372 6970 745b 2744 6573 6372 6970  escript['Descrip
-0006aa00: 7469 6f6e 275d 2e73 7472 2e6c 6f77 6572  tion'].str.lower
-0006aa10: 2829 0a20 2020 2020 2020 2020 2020 2065  ().            e
-0006aa20: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0006aa30: 2020 2020 2061 746c 6173 4465 7363 7269       atlasDescri
-0006aa40: 7074 203d 2070 642e 7265 6164 5f63 7376  pt = pd.read_csv
-0006aa50: 2866 227e 2f2e 616e 7473 7079 7431 772f  (f"~/.antspyt1w/
-0006aa60: 7b63 6f72 7265 6374 6465 7363 7269 7074  {correctdescript
-0006aa70: 7d2e 6373 7622 290a 2020 2020 2020 2020  }.csv").        
-0006aa80: 2020 2020 2020 2020 6174 6c61 7344 6573          atlasDes
-0006aa90: 6372 6970 745b 2744 6573 6372 6970 7469  cript['Descripti
-0006aaa0: 6f6e 275d 203d 2061 746c 6173 4465 7363  on'] = atlasDesc
-0006aab0: 7269 7074 5b27 4465 7363 7269 7074 696f  ript['Descriptio
-0006aac0: 6e27 5d2e 7374 722e 6c6f 7765 7228 290a  n'].str.lower().
-0006aad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0006aae0: 6174 6c61 7344 6573 6372 6970 745b 2744  atlasDescript['D
-0006aaf0: 6573 6372 6970 7469 6f6e 275d 203d 2061  escription'] = a
-0006ab00: 746c 6173 4465 7363 7269 7074 5b27 4465  tlasDescript['De
-0006ab10: 7363 7269 7074 696f 6e27 5d2e 7374 722e  scription'].str.
-0006ab20: 7265 706c 6163 6528 2220 222c 2022 5f22  replace(" ", "_"
-0006ab30: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0006ab40: 2020 6174 6c61 7344 6573 6372 6970 745b    atlasDescript[
-0006ab50: 2744 6573 6372 6970 7469 6f6e 275d 203d  'Description'] =
-0006ab60: 2061 746c 6173 4465 7363 7269 7074 5b27   atlasDescript['
-0006ab70: 4465 7363 7269 7074 696f 6e27 5d2e 7374  Description'].st
-0006ab80: 722e 7265 706c 6163 6528 225f 6c65 6674  r.replace("_left
-0006ab90: 5f22 2c20 225f 2229 0a20 2020 2020 2020  _", "_").       
-0006aba0: 2020 2020 2020 2020 2061 746c 6173 4465           atlasDe
-0006abb0: 7363 7269 7074 5b27 4465 7363 7269 7074  script['Descript
-0006abc0: 696f 6e27 5d20 3d20 6174 6c61 7344 6573  ion'] = atlasDes
-0006abd0: 6372 6970 745b 2744 6573 6372 6970 7469  cript['Descripti
-0006abe0: 6f6e 275d 2e73 7472 2e72 6570 6c61 6365  on'].str.replace
-0006abf0: 2822 5f72 6967 6874 5f22 2c20 225f 2229  ("_right_", "_")
-0006ac00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0006ac10: 2061 746c 6173 4465 7363 7269 7074 5b27   atlasDescript['
-0006ac20: 4465 7363 7269 7074 696f 6e27 5d20 3d20  Description'] = 
-0006ac30: 6174 6c61 7344 6573 6372 6970 745b 2744  atlasDescript['D
-0006ac40: 6573 6372 6970 7469 6f6e 275d 2e73 7472  escription'].str
-0006ac50: 2e72 6570 6c61 6365 2822 5f6c 6566 7422  .replace("_left"
-0006ac60: 2c20 2222 290a 2020 2020 2020 2020 2020  , "").          
-0006ac70: 2020 2020 2020 6174 6c61 7344 6573 6372        atlasDescr
-0006ac80: 6970 745b 2744 6573 6372 6970 7469 6f6e  ipt['Description
-0006ac90: 275d 203d 2061 746c 6173 4465 7363 7269  '] = atlasDescri
-0006aca0: 7074 5b27 4465 7363 7269 7074 696f 6e27  pt['Description'
-0006acb0: 5d2e 7374 722e 7265 706c 6163 6528 225f  ].str.replace("_
-0006acc0: 7269 6768 7422 2c20 2222 290a 2020 2020  right", "").    
-0006acd0: 2020 2020 2020 2020 2020 2020 6174 6c61              atla
-0006ace0: 7344 6573 6372 6970 745b 2744 6573 6372  sDescript['Descr
-0006acf0: 6970 7469 6f6e 275d 203d 2061 746c 6173  iption'] = atlas
-0006ad00: 4465 7363 7269 7074 5b27 4465 7363 7269  Descript['Descri
-0006ad10: 7074 696f 6e27 5d2e 7374 722e 7265 706c  ption'].str.repl
-0006ad20: 6163 6528 226c 6566 745f 222c 2022 2229  ace("left_", "")
-0006ad30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0006ad40: 2061 746c 6173 4465 7363 7269 7074 5b27   atlasDescript['
-0006ad50: 4465 7363 7269 7074 696f 6e27 5d20 3d20  Description'] = 
-0006ad60: 6174 6c61 7344 6573 6372 6970 745b 2744  atlasDescript['D
-0006ad70: 6573 6372 6970 7469 6f6e 275d 2e73 7472  escription'].str
-0006ad80: 2e72 6570 6c61 6365 2822 7269 6768 745f  .replace("right_
-0006ad90: 222c 2022 2229 0a20 2020 2020 2020 2020  ", "").         
-0006ada0: 2020 2020 2020 2061 746c 6173 4465 7363         atlasDesc
-0006adb0: 7269 7074 5b27 4465 7363 7269 7074 696f  ript['Descriptio
-0006adc0: 6e27 5d20 3d20 6174 6c61 7344 6573 6372  n'] = atlasDescr
-0006add0: 6970 745b 2744 6573 6372 6970 7469 6f6e  ipt['Description
-0006ade0: 275d 2e73 7472 2e72 6570 6c61 6365 2822  '].str.replace("
-0006adf0: 2f22 2c22 2e22 290a 2020 2020 2020 2020  /",".").        
-0006ae00: 2020 2020 2020 2020 6966 206d 7965 7874          if myext
-0006ae10: 203d 3d20 274a 4855 5f77 6d27 3a0a 2020   == 'JHU_wm':.  
-0006ae20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0006ae30: 2020 6174 6c61 7344 6573 6372 6970 745b    atlasDescript[
-0006ae40: 2744 6573 6372 6970 7469 6f6e 275d 203d  'Description'] =
-0006ae50: 2061 746c 6173 4465 7363 7269 7074 5b27   atlasDescript['
-0006ae60: 4465 7363 7269 7074 696f 6e27 5d2e 7374  Description'].st
-0006ae70: 722e 7265 706c 6163 6528 2266 612d 222c  r.replace("fa-",
-0006ae80: 2022 2229 0a20 2020 2020 2020 2020 2020   "").           
-0006ae90: 2020 2020 2020 2020 2061 746c 6173 4465           atlasDe
-0006aea0: 7363 7269 7074 5b27 4465 7363 7269 7074  script['Descript
-0006aeb0: 696f 6e27 5d20 3d20 6174 6c61 7344 6573  ion'] = atlasDes
-0006aec0: 6372 6970 745b 2744 6573 6372 6970 7469  cript['Descripti
-0006aed0: 6f6e 275d 2e73 7472 2e72 6570 6c61 6365  on'].str.replace
-0006aee0: 2822 2d6c 6566 742d 222c 2022 2229 0a20  ("-left-", ""). 
-0006aef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0006af00: 2020 2061 746c 6173 4465 7363 7269 7074     atlasDescript
-0006af10: 5b27 4465 7363 7269 7074 696f 6e27 5d20  ['Description'] 
-0006af20: 3d20 6174 6c61 7344 6573 6372 6970 745b  = atlasDescript[
-0006af30: 2744 6573 6372 6970 7469 6f6e 275d 2e73  'Description'].s
-0006af40: 7472 2e72 6570 6c61 6365 2822 2d72 6967  tr.replace("-rig
-0006af50: 6874 2d22 2c20 2222 290a 2020 2020 2020  ht-", "").      
-0006af60: 2020 2020 2020 2020 2020 6966 206d 7965            if mye
-0006af70: 7874 203d 3d20 2763 6572 6562 656c 6c75  xt == 'cerebellu
-0006af80: 6d27 3a0a 2020 2020 2020 2020 2020 2020  m':.            
-0006af90: 2020 2020 2020 2020 6174 6c61 7344 6573          atlasDes
-0006afa0: 6372 6970 745b 2744 6573 6372 6970 7469  cript['Descripti
-0006afb0: 6f6e 275d 203d 2061 746c 6173 4465 7363  on'] = atlasDesc
-0006afc0: 7269 7074 5b27 4465 7363 7269 7074 696f  ript['Descriptio
-0006afd0: 6e27 5d2e 7374 722e 7265 706c 6163 6528  n'].str.replace(
-0006afe0: 226c 5f22 2c20 2222 290a 2020 2020 2020  "l_", "").      
-0006aff0: 2020 2020 2020 2020 2020 2020 2020 6174                at
-0006b000: 6c61 7344 6573 6372 6970 745b 2744 6573  lasDescript['Des
-0006b010: 6372 6970 7469 6f6e 275d 203d 2061 746c  cription'] = atl
-0006b020: 6173 4465 7363 7269 7074 5b27 4465 7363  asDescript['Desc
-0006b030: 7269 7074 696f 6e27 5d2e 7374 722e 7265  ription'].str.re
-0006b040: 706c 6163 6528 2272 5f22 2c20 2222 290a  place("r_", "").
-0006b050: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0006b060: 7665 7262 6f73 653a 0a20 2020 2020 2020  verbose:.       
-0006b070: 2020 2020 2020 2020 2070 7269 6e74 2820           print( 
-0006b080: 6174 6c61 7344 6573 6372 6970 7420 290a  atlasDescript ).
-0006b090: 2020 2020 2020 2020 2020 2020 6f67 6c61              ogla
-0006b0a0: 6265 6c6e 616d 6520 3d20 6f67 6c61 6265  belname = oglabe
-0006b0b0: 6c6e 616d 652e 6c6f 7765 7228 290a 2020  lname.lower().  
-0006b0c0: 2020 2020 2020 2020 2020 6f67 6c61 6265            oglabe
-0006b0d0: 6c6e 616d 6520 3d20 7265 2e73 7562 2822  lname = re.sub("
-0006b0e0: 2022 2c20 225f 222c 6f67 6c61 6265 6c6e   ", "_",oglabeln
-0006b0f0: 616d 6529 0a20 2020 2020 2020 2020 2020  ame).           
-0006b100: 206f 676c 6162 656c 6e61 6d65 203d 2072   oglabelname = r
-0006b110: 652e 7375 6228 225f 6c65 6674 5f22 2c20  e.sub("_left_", 
-0006b120: 225f 222c 6f67 6c61 6265 6c6e 616d 6529  "_",oglabelname)
-0006b130: 0a20 2020 2020 2020 2020 2020 206f 676c  .            ogl
-0006b140: 6162 656c 6e61 6d65 203d 2072 652e 7375  abelname = re.su
-0006b150: 6228 225f 7269 6768 745f 222c 2022 5f22  b("_right_", "_"
-0006b160: 2c6f 676c 6162 656c 6e61 6d65 290a 2020  ,oglabelname).  
-0006b170: 2020 2020 2020 2020 2020 6f67 6c61 6265            oglabe
-0006b180: 6c6e 616d 6520 3d20 7265 2e73 7562 2822  lname = re.sub("
-0006b190: 5f6c 6566 7422 2c20 2222 2c6f 676c 6162  _left", "",oglab
-0006b1a0: 656c 6e61 6d65 290a 2020 2020 2020 2020  elname).        
-0006b1b0: 2020 2020 6f67 6c61 6265 6c6e 616d 6520      oglabelname 
-0006b1c0: 3d20 7265 2e73 7562 2822 5f72 6967 6874  = re.sub("_right
-0006b1d0: 222c 2022 222c 6f67 6c61 6265 6c6e 616d  ", "",oglabelnam
-0006b1e0: 6529 0a20 2020 2020 2020 2020 2020 206f  e).            o
-0006b1f0: 676c 6162 656c 6e61 6d65 203d 2072 652e  glabelname = re.
-0006b200: 7375 6228 2274 3168 6965 725f 766f 6c5f  sub("t1hier_vol_
-0006b210: 222c 2022 222c 6f67 6c61 6265 6c6e 616d  ", "",oglabelnam
-0006b220: 6529 0a20 2020 2020 2020 2020 2020 206f  e).            o
-0006b230: 676c 6162 656c 6e61 6d65 203d 2072 652e  glabelname = re.
-0006b240: 7375 6228 2274 3168 6965 725f 6172 6561  sub("t1hier_area
-0006b250: 5f22 2c20 2222 2c6f 676c 6162 656c 6e61  _", "",oglabelna
-0006b260: 6d65 290a 2020 2020 2020 2020 2020 2020  me).            
-0006b270: 6f67 6c61 6265 6c6e 616d 6520 3d20 7265  oglabelname = re
-0006b280: 2e73 7562 2822 7431 6869 6572 5f74 686b  .sub("t1hier_thk
-0006b290: 5f22 2c20 2222 2c6f 676c 6162 656c 6e61  _", "",oglabelna
-0006b2a0: 6d65 290a 2020 2020 2020 2020 2020 2020  me).            
-0006b2b0: 6f67 6c61 6265 6c6e 616d 6520 3d20 7265  oglabelname = re
-0006b2c0: 2e73 7562 2822 646b 7472 6567 696f 6e73  .sub("dktregions
-0006b2d0: 222c 2022 222c 6f67 6c61 6265 6c6e 616d  ", "",oglabelnam
-0006b2e0: 6529 0a20 2020 2020 2020 2020 2020 206f  e).            o
-0006b2f0: 676c 6162 656c 6e61 6d65 203d 2072 652e  glabelname = re.
-0006b300: 7375 6228 2264 6b74 636f 7274 6578 222c  sub("dktcortex",
-0006b310: 2022 222c 6f67 6c61 6265 6c6e 616d 6529   "",oglabelname)
-0006b320: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0006b330: 6d79 6578 7420 3d3d 2027 4a48 555f 776d  myext == 'JHU_wm
-0006b340: 273a 0a20 2020 2020 2020 2020 2020 2020  ':.             
-0006b350: 2020 206f 676c 6162 656c 6e61 6d65 203d     oglabelname =
-0006b360: 2072 652e 7375 6228 2264 7469 5f6d 6561   re.sub("dti_mea
-0006b370: 6e5f 6661 2e22 2c20 2222 2c6f 676c 6162  n_fa.", "",oglab
-0006b380: 656c 6e61 6d65 290a 2020 2020 2020 2020  elname).        
-0006b390: 2020 2020 2020 2020 6f67 6c61 6265 6c6e          oglabeln
-0006b3a0: 616d 6520 3d20 7265 2e73 7562 2822 6474  ame = re.sub("dt
-0006b3b0: 695f 6d65 616e 5f6d 642e 222c 2022 222c  i_mean_md.", "",
-0006b3c0: 6f67 6c61 6265 6c6e 616d 6529 0a20 2020  oglabelname).   
-0006b3d0: 2020 2020 2020 2020 2020 2020 206f 676c               ogl
-0006b3e0: 6162 656c 6e61 6d65 203d 2072 652e 7375  abelname = re.su
-0006b3f0: 6228 222e 6c65 6674 2e22 2c20 2222 2c6f  b(".left.", "",o
-0006b400: 676c 6162 656c 6e61 6d65 290a 2020 2020  glabelname).    
-0006b410: 2020 2020 2020 2020 2020 2020 6f67 6c61              ogla
-0006b420: 6265 6c6e 616d 6520 3d20 7265 2e73 7562  belname = re.sub
-0006b430: 2822 2e72 6967 6874 2e22 2c20 2222 2c6f  (".right.", "",o
-0006b440: 676c 6162 656c 6e61 6d65 290a 2020 2020  glabelname).    
-0006b450: 2020 2020 2020 2020 2020 2020 6f67 6c61              ogla
-0006b460: 6265 6c6e 616d 6520 3d20 7265 2e73 7562  belname = re.sub
-0006b470: 2822 2e6c 7261 7667 2e22 2c20 2222 2c6f  (".lravg.", "",o
-0006b480: 676c 6162 656c 6e61 6d65 290a 2020 2020  glabelname).    
-0006b490: 2020 2020 2020 2020 2020 2020 6f67 6c61              ogla
-0006b4a0: 6265 6c6e 616d 6520 3d20 7265 2e73 7562  belname = re.sub
-0006b4b0: 2822 2e61 7379 6d2e 222c 2022 222c 6f67  (".asym.", "",og
-0006b4c0: 6c61 6265 6c6e 616d 6529 0a0a 2020 2020  labelname)..    
-0006b4d0: 2020 2020 2020 2020 6966 2076 6572 626f          if verbo
-0006b4e0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0006b4f0: 2020 2020 7072 696e 7428 226f 676c 6162      print("oglab
-0006b500: 656c 6e61 6d65 2022 202b 206f 676c 6162  elname " + oglab
-0006b510: 656c 6e61 6d65 2029 0a0a 2020 2020 2020  elname )..      
-0006b520: 2020 2020 2020 6966 206d 7965 7874 203d        if myext =
-0006b530: 3d20 2763 6572 6562 656c 6c75 6d27 3a0a  = 'cerebellum':.
-0006b540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0006b550: 6174 6c61 7344 6573 6372 6970 745b 2744  atlasDescript['D
-0006b560: 6573 6372 6970 7469 6f6e 275d 203d 2061  escription'] = a
-0006b570: 746c 6173 4465 7363 7269 7074 5b27 4465  tlasDescript['De
-0006b580: 7363 7269 7074 696f 6e27 5d2e 7374 722e  scription'].str.
-0006b590: 7265 706c 6163 6528 226c 5f22 2c20 2222  replace("l_", ""
-0006b5a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0006b5b0: 2020 6174 6c61 7344 6573 6372 6970 745b    atlasDescript[
-0006b5c0: 2744 6573 6372 6970 7469 6f6e 275d 203d  'Description'] =
-0006b5d0: 2061 746c 6173 4465 7363 7269 7074 5b27   atlasDescript['
-0006b5e0: 4465 7363 7269 7074 696f 6e27 5d2e 7374  Description'].st
-0006b5f0: 722e 7265 706c 6163 6528 2272 5f22 2c20  r.replace("r_", 
-0006b600: 2222 290a 2020 2020 2020 2020 2020 2020  "").            
-0006b610: 2020 2020 7768 6963 6869 6e64 6578 203d      whichindex =
-0006b620: 2061 746c 6173 4465 7363 7269 7074 2e69   atlasDescript.i
-0006b630: 6e64 6578 5b61 746c 6173 4465 7363 7269  ndex[atlasDescri
-0006b640: 7074 5b27 4465 7363 7269 7074 696f 6e27  pt['Description'
-0006b650: 5d20 3d3d 206f 676c 6162 656c 6e61 6d65  ] == oglabelname
-0006b660: 5d2e 7661 6c75 6573 5b30 5d0a 2020 2020  ].values[0].    
-0006b670: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0006b680: 2020 2020 2020 2020 2020 2020 2020 7768                wh
-0006b690: 6963 6869 6e64 6578 203d 2061 746c 6173  ichindex = atlas
-0006b6a0: 4465 7363 7269 7074 2e69 6e64 6578 5b61  Descript.index[a
-0006b6b0: 746c 6173 4465 7363 7269 7074 5b27 4465  tlasDescript['De
-0006b6c0: 7363 7269 7074 696f 6e27 5d2e 7374 722e  scription'].str.
-0006b6d0: 636f 6e74 6169 6e73 286f 676c 6162 656c  contains(oglabel
-0006b6e0: 6e61 6d65 295d 0a0a 2020 2020 2020 2020  name)]..        
-0006b6f0: 2020 2020 6966 2074 7970 6528 7768 6963      if type(whic
-0006b700: 6869 6e64 6578 2920 6973 206e 702e 696e  hindex) is np.in
-0006b710: 7436 343a 0a20 2020 2020 2020 2020 2020  t64:.           
-0006b720: 2020 2020 206c 6162 656c 6e75 6d73 203d       labelnums =
-0006b730: 2061 746c 6173 4465 7363 7269 7074 2e6c   atlasDescript.l
-0006b740: 6f63 5b77 6869 6368 696e 6465 782c 2027  oc[whichindex, '
-0006b750: 4c61 6265 6c27 5d0a 2020 2020 2020 2020  Label'].        
-0006b760: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0006b770: 2020 2020 2020 2020 2020 6c61 6265 6c6e            labeln
-0006b780: 756d 7320 3d20 6c69 7374 2861 746c 6173  ums = list(atlas
-0006b790: 4465 7363 7269 7074 2e6c 6f63 5b77 6869  Descript.loc[whi
-0006b7a0: 6368 696e 6465 782c 2027 4c61 6265 6c27  chindex, 'Label'
-0006b7b0: 5d29 0a0a 2020 2020 2020 2020 2020 2020  ])..            
-0006b7c0: 6966 206d 7965 7874 203d 3d20 2779 656f  if myext == 'yeo
-0006b7d0: 273a 0a20 2020 2020 2020 2020 2020 2020  ':.             
-0006b7e0: 2020 2070 6172 7473 203d 2072 652e 6669     parts = re.fi
-0006b7f0: 6e64 616c 6c28 7227 5c44 2b27 2c20 6f67  ndall(r'\D+', og
-0006b800: 6c61 6265 6c6e 616d 6529 0a20 2020 2020  labelname).     
-0006b810: 2020 2020 2020 2020 2020 206f 676c 6162             oglab
-0006b820: 656c 6e61 6d65 203d 205b 7061 7274 2e72  elname = [part.r
-0006b830: 6570 6c61 6365 2827 5f27 2c20 2727 2920  eplace('_', '') 
-0006b840: 666f 7220 7061 7274 2069 6e20 7061 7274  for part in part
-0006b850: 7320 6966 2070 6172 742e 7265 706c 6163  s if part.replac
-0006b860: 6528 275f 272c 2027 2729 5d0a 2020 2020  e('_', '')].    
-0006b870: 2020 2020 2020 2020 2020 2020 6669 6c74              filt
-0006b880: 6572 6564 5f64 6620 3d20 6174 6c61 7344  ered_df = atlasD
-0006b890: 6573 6372 6970 745b 6174 6c61 7344 6573  escript[atlasDes
-0006b8a0: 6372 6970 745b 2744 6573 6372 6970 7469  cript['Descripti
-0006b8b0: 6f6e 275d 2e69 7369 6e28 6f67 6c61 6265  on'].isin(oglabe
-0006b8c0: 6c6e 616d 6529 5d0a 2020 2020 2020 2020  lname)].        
-0006b8d0: 2020 2020 2020 2020 6c61 6265 6c6e 756d          labelnum
-0006b8e0: 7320 3d20 6669 6c74 6572 6564 5f64 665b  s = filtered_df[
-0006b8f0: 274c 6162 656c 275d 2e74 6f6c 6973 7428  'Label'].tolist(
-0006b900: 290a 0a20 2020 2020 2020 2020 2020 2069  )..            i
-0006b910: 6620 6e6f 7420 6973 696e 7374 616e 6365  f not isinstance
-0006b920: 286c 6162 656c 6e75 6d73 2c20 6c69 7374  (labelnums, list
-0006b930: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0006b940: 2020 206c 6162 656c 6e75 6d73 3d5b 6c61     labelnums=[la
-0006b950: 6265 6c6e 756d 735d 0a20 2020 2020 2020  belnums].       
-0006b960: 2020 2020 2061 6464 656d 6973 7a65 726f       addemiszero
-0006b970: 203d 2061 6e74 732e 7468 7265 7368 6f6c   = ants.threshol
-0006b980: 645f 696d 6167 6528 6164 6465 6d2c 2030  d_image(addem, 0
-0006b990: 2c20 3029 0a20 2020 2020 2020 2020 2020  , 0).           
-0006b9a0: 2074 656d 7020 3d20 616e 7473 2e69 6d61   temp = ants.ima
-0006b9b0: 6765 5f72 6561 6428 6c6f 6366 696c 656e  ge_read(locfilen
-0006b9c0: 616d 6529 0a20 2020 2020 2020 2020 2020  ame).           
-0006b9d0: 2074 656d 7020 3d20 616e 7473 2e6d 6173   temp = ants.mas
-0006b9e0: 6b5f 696d 6167 6528 7465 6d70 2c20 7465  k_image(temp, te
-0006b9f0: 6d70 2c20 6c65 7665 6c3d 6c61 6265 6c6e  mp, level=labeln
-0006ba00: 756d 732c 2062 696e 6172 697a 653d 5472  ums, binarize=Tr
-0006ba10: 7565 290a 2020 2020 2020 2020 2020 2020  ue).            
-0006ba20: 6966 2076 6572 626f 7365 3a0a 2020 2020  if verbose:.    
-0006ba30: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-0006ba40: 7428 2244 4542 5547 2229 0a20 2020 2020  t("DEBUG").     
-0006ba50: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-0006ba60: 2820 2074 656d 702e 7375 6d28 2920 2920  (  temp.sum() ) 
-0006ba70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0006ba80: 2070 7269 6e74 2820 6c61 6265 6c6e 756d   print( labelnum
-0006ba90: 7320 290a 2020 2020 2020 2020 2020 2020  s ).            
-0006baa0: 7465 6d70 5b74 656d 7020 3d3d 2031 5d20  temp[temp == 1] 
-0006bab0: 3d20 2876 616c 7332 7669 7a29 0a20 2020  = (vals2viz).   
-0006bac0: 2020 2020 2020 2020 2074 656d 705b 6164           temp[ad
-0006bad0: 6465 6d69 737a 6572 6f20 3d3d 2030 5d20  demiszero == 0] 
-0006bae0: 3d20 300a 2020 2020 2020 2020 2020 2020  = 0.            
-0006baf0: 6164 6465 6d20 3d20 6164 6465 6d20 2b20  addem = addem + 
-0006bb00: 7465 6d70 0a0a 2020 2020 2020 2020 6966  temp..        if
-0006bb10: 2076 6572 626f 7365 3a0a 2020 2020 2020   verbose:.      
-0006bb20: 2020 2020 2020 7072 696e 7428 2744 6f6e        print('Don
-0006bb30: 6520 4164 6469 6e67 2729 0a20 2020 2020  e Adding').     
-0006bb40: 2020 2066 6f72 2061 7878 2069 6e20 6178     for axx in ax
-0006bb50: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
-0006bb60: 6669 6766 6e3d 6f75 7470 7574 5f70 7265  figfn=output_pre
-0006bb70: 6669 782b 6622 6669 677b 636f 6c32 7669  fix+f"fig{col2vi
-0006bb80: 7a7d 6178 7b61 7878 7d5f 7079 2e6a 7067  z}ax{axx}_py.jpg
-0006bb90: 220a 2020 2020 2020 2020 2020 2020 6966  ".            if
-0006bba0: 2063 726f 7020 3e20 303a 0a20 2020 2020   crop > 0:.     
-0006bbb0: 2020 2020 2020 2020 2020 2063 6d61 736b             cmask
-0006bbc0: 203d 2061 6e74 732e 7468 7265 7368 6f6c   = ants.threshol
-0006bbd0: 645f 696d 6167 6528 2061 6464 656d 2c31  d_image( addem,1
-0006bbe0: 652d 352c 2031 6539 2029 2e69 4d61 7468  e-5, 1e9 ).iMath
-0006bbf0: 2822 4d44 222c 6372 6f70 2920 2b20 616e  ("MD",crop) + an
-0006bc00: 7473 2e74 6872 6573 686f 6c64 5f69 6d61  ts.threshold_ima
-0006bc10: 6765 2820 6164 6465 6d2c 2d31 6539 2c20  ge( addem,-1e9, 
-0006bc20: 2d31 652d 3520 292e 694d 6174 6828 224d  -1e-5 ).iMath("M
-0006bc30: 4422 2c63 726f 7029 0a20 2020 2020 2020  D",crop).       
-0006bc40: 2020 2020 2020 2020 2061 6464 656d 4320           addemC 
-0006bc50: 3d20 616e 7473 2e63 726f 705f 696d 6167  = ants.crop_imag
-0006bc60: 6528 2061 6464 656d 2c20 636d 6173 6b20  e( addem, cmask 
-0006bc70: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0006bc80: 2020 6564 6765 696d 6743 203d 2061 6e74    edgeimgC = ant
-0006bc90: 732e 6372 6f70 5f69 6d61 6765 2820 6564  s.crop_image( ed
-0006bca0: 6765 696d 672c 2063 6d61 736b 2029 0a20  geimg, cmask ). 
-0006bcb0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0006bcc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0006bcd0: 2061 6464 656d 4320 3d20 6164 6465 6d0a   addemC = addem.
-0006bce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0006bcf0: 6564 6765 696d 6743 203d 2065 6467 6569  edgeimgC = edgei
-0006bd00: 6d67 0a20 2020 2020 2020 2020 2020 2069  mg.            i
-0006bd10: 6620 6669 7865 645f 6f76 6572 6c61 795f  f fixed_overlay_
-0006bd20: 7261 6e67 6520 6973 206e 6f74 204e 6f6e  range is not Non
-0006bd30: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0006bd40: 2020 2061 6464 656d 435b 303a 332c 303a     addemC[0:3,0:
-0006bd50: 332c 303a 335d 3d66 6978 6564 5f6f 7665  3,0:3]=fixed_ove
-0006bd60: 726c 6179 5f72 616e 6765 5b30 5d0a 2020  rlay_range[0].  
-0006bd70: 2020 2020 2020 2020 2020 2020 2020 6164                ad
-0006bd80: 6465 6d43 5b34 3a37 2c34 3a37 2c34 3a37  demC[4:7,4:7,4:7
-0006bd90: 5d3d 6669 7865 645f 6f76 6572 6c61 795f  ]=fixed_overlay_
-0006bda0: 7261 6e67 655b 315d 0a20 2020 2020 2020  range[1].       
-0006bdb0: 2020 2020 2020 2020 2061 6464 656d 435b           addemC[
-0006bdc0: 2061 6464 656d 4320 3c20 6669 7865 645f   addemC < fixed_
-0006bdd0: 6f76 6572 6c61 795f 7261 6e67 655b 305d  overlay_range[0]
-0006bde0: 205d 203d 2066 6978 6564 5f6f 7665 726c   ] = fixed_overl
-0006bdf0: 6179 5f72 616e 6765 5b30 5d0a 2020 2020  ay_range[0].    
-0006be00: 2020 2020 2020 2020 2020 2020 6164 6465              adde
-0006be10: 6d43 5b20 6164 6465 6d43 203e 2066 6978  mC[ addemC > fix
-0006be20: 6564 5f6f 7665 726c 6179 5f72 616e 6765  ed_overlay_range
-0006be30: 5b31 5d20 5d20 3d20 6669 7865 645f 6f76  [1] ] = fixed_ov
-0006be40: 6572 6c61 795f 7261 6e67 655b 315d 0a20  erlay_range[1]. 
-0006be50: 2020 2020 2020 2020 2020 2061 6e74 732e             ants.
-0006be60: 706c 6f74 2865 6467 6569 6d67 432c 2061  plot(edgeimgC, a
-0006be70: 6464 656d 432c 2061 7869 733d 6178 782c  ddemC, axis=axx,
-0006be80: 206e 736c 6963 6573 3d6e 736c 6963 6573   nslices=nslices
-0006be90: 2c20 6e63 6f6c 3d6e 636f 6c2c 2020 2020  , ncol=ncol,    
-0006bea0: 2020 200a 2020 2020 2020 2020 2020 2020     .            
-0006beb0: 2020 2020 6f76 6572 6c61 795f 636d 6170      overlay_cmap
-0006bec0: 3d6f 7665 726c 6179 5f63 6d61 702c 2072  =overlay_cmap, r
-0006bed0: 6573 616d 706c 653d 4661 6c73 652c 0a20  esample=False,. 
-0006bee0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0006bef0: 696c 656e 616d 653d 6669 6766 6e2c 2063  ilename=figfn, c
-0006bf00: 6261 723d 6178 783d 3d61 7865 735b 305d  bar=axx==axes[0]
-0006bf10: 2c20 6372 6f70 3d54 7275 652c 2062 6c61  , crop=True, bla
-0006bf20: 636b 5f62 673d 626c 6163 6b5f 6267 2029  ck_bg=black_bg )
-0006bf30: 0a20 2020 2020 2020 2069 6620 7665 7262  .        if verb
-0006bf40: 6f73 653a 0a20 2020 2020 2020 2020 2020  ose:.           
-0006bf50: 2070 7269 6e74 2866 227b 636f 6c32 7669   print(f"{col2vi
-0006bf60: 7a7d 2064 6f6e 6522 290a 2020 2020 6966  z} done").    if
-0006bf70: 2076 6572 626f 7365 3a0a 2020 2020 2020   verbose:.      
-0006bf80: 2020 7072 696e 7428 2244 4f4e 4520 6272    print("DONE br
-0006bf90: 6169 6e20 6d61 7020 6669 6775 7265 7322  ain map figures"
-0006bfa0: 290a 2020 2020 7265 7475 726e 2061 6464  ).    return add
-0006bfb0: 656d 0a0a 6465 6620 6669 6c74 6572 5f64  em..def filter_d
-0006bfc0: 6628 696e 6466 2c20 6d79 7072 6566 6978  f(indf, myprefix
-0006bfd0: 293a 0a20 2020 2022 2222 0a20 2020 2050  ):.    """.    P
-0006bfe0: 726f 6365 7373 2061 6e64 2066 696c 7465  rocess and filte
-0006bff0: 7220 6120 7061 6e64 6173 2044 6174 6146  r a pandas DataF
-0006c000: 7261 6d65 2c20 7265 6d6f 7669 6e67 2063  rame, removing c
-0006c010: 6572 7461 696e 2063 6f6c 756d 6e73 2c20  ertain columns, 
-0006c020: 0a20 2020 2066 696c 7465 7269 6e67 2062  .    filtering b
-0006c030: 6173 6564 206f 6e20 6461 7461 2074 7970  ased on data typ
-0006c040: 6573 2c20 636f 6d70 7574 696e 6720 7468  es, computing th
-0006c050: 6520 6d65 616e 206f 6620 6e75 6d65 7269  e mean of numeri
-0006c060: 6320 636f 6c75 6d6e 732c 200a 2020 2020  c columns, .    
-0006c070: 616e 6420 6164 6469 6e67 2061 2070 7265  and adding a pre
-0006c080: 6669 7820 746f 2063 6f6c 756d 6e20 6e61  fix to column na
-0006c090: 6d65 732e 0a0a 2020 2020 5061 7261 6d65  mes...    Parame
-0006c0a0: 7465 7273 3a0a 2020 2020 696e 6466 2028  ters:.    indf (
-0006c0b0: 7061 6e64 6173 2e44 6174 6146 7261 6d65  pandas.DataFrame
-0006c0c0: 293a 2054 6865 2069 6e70 7574 2044 6174  ): The input Dat
-0006c0d0: 6146 7261 6d65 2074 6f20 6265 2070 726f  aFrame to be pro
-0006c0e0: 6365 7373 6564 2e0a 2020 2020 6d79 7072  cessed..    mypr
-0006c0f0: 6566 6978 2028 7374 7229 3a20 4120 7374  efix (str): A st
-0006c100: 7269 6e67 2070 7265 6669 7820 746f 2062  ring prefix to b
-0006c110: 6520 6164 6465 6420 746f 2074 6865 2063  e added to the c
-0006c120: 6f6c 756d 6e20 6e61 6d65 7320 0a20 2020  olumn names .   
-0006c130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0006c140: 206f 6620 7468 6520 7072 6f63 6573 7365   of the processe
-0006c150: 6420 4461 7461 4672 616d 652e 0a0a 2020  d DataFrame...  
-0006c160: 2020 5374 6570 733a 0a20 2020 2031 2e20    Steps:.    1. 
-0006c170: 5265 6d6f 7665 7320 636f 6c75 6d6e 7320  Removes columns 
-0006c180: 7769 7468 206e 616d 6573 2063 6f6e 7461  with names conta
-0006c190: 696e 696e 6720 2755 6e6e 616d 6564 272e  ining 'Unnamed'.
-0006c1a0: 0a20 2020 2032 2e20 4966 2074 6865 2044  .    2. If the D
-0006c1b0: 6174 6146 7261 6d65 2068 6173 206e 6f20  ataFrame has no 
-0006c1c0: 726f 7773 2c20 6974 2072 6574 7572 6e73  rows, it returns
-0006c1d0: 2074 6865 2065 6d70 7479 2044 6174 6146   the empty DataF
-0006c1e0: 7261 6d65 2e0a 2020 2020 332e 2046 696c  rame..    3. Fil
-0006c1f0: 7465 7273 206f 7574 2063 6f6c 756d 6e73  ters out columns
-0006c200: 2062 6173 6564 206f 6e20 7468 6520 7479   based on the ty
-0006c210: 7065 206f 6620 7468 6520 6669 7273 7420  pe of the first 
-0006c220: 656c 656d 656e 742c 200a 2020 2020 2020  element, .      
-0006c230: 206b 6565 7069 6e67 2074 686f 7365 2074   keeping those t
-0006c240: 6861 7420 6172 6520 6f66 2074 7970 6520  hat are of type 
-0006c250: 606f 626a 6563 7460 2c20 6069 6e74 602c  `object`, `int`,
-0006c260: 206f 7220 6066 6c6f 6174 602e 0a20 2020   or `float`..   
-0006c270: 2034 2e20 5265 6d6f 7665 7320 636f 6c75   4. Removes colu
-0006c280: 6d6e 7320 7468 6174 2061 7265 206f 6620  mns that are of 
-0006c290: 606f 626a 6563 7460 2064 7479 7065 2e0a  `object` dtype..
-0006c2a0: 2020 2020 352e 2043 616c 6375 6c61 7465      5. Calculate
-0006c2b0: 7320 7468 6520 6d65 616e 206f 6620 7468  s the mean of th
-0006c2c0: 6520 7265 6d61 696e 696e 6720 636f 6c75  e remaining colu
-0006c2d0: 6d6e 732c 2073 6b69 7070 696e 6720 4e61  mns, skipping Na
-0006c2e0: 4e20 7661 6c75 6573 2e0a 2020 2020 362e  N values..    6.
-0006c2f0: 2041 6464 7320 7468 6520 7370 6563 6966   Adds the specif
-0006c300: 6965 6420 606d 7970 7265 6669 7860 2074  ied `myprefix` t
-0006c310: 6f20 7468 6520 636f 6c75 6d6e 206e 616d  o the column nam
-0006c320: 6573 2e0a 0a20 2020 2052 6574 7572 6e73  es...    Returns
-0006c330: 3a0a 2020 2020 7061 6e64 6173 2e44 6174  :.    pandas.Dat
-0006c340: 6146 7261 6d65 3a20 4120 7472 616e 7366  aFrame: A transf
-0006c350: 6f72 6d65 6420 4461 7461 4672 616d 6520  ormed DataFrame 
-0006c360: 7769 7468 2061 2073 696e 676c 6520 726f  with a single ro
-0006c370: 7720 636f 6e74 6169 6e69 6e67 200a 2020  w containing .  
-0006c380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0006c390: 2020 2020 7468 6520 6d65 616e 2076 616c      the mean val
-0006c3a0: 7565 7320 6f66 2074 6865 2066 696c 7465  ues of the filte
-0006c3b0: 7265 6420 636f 6c75 6d6e 732c 2061 6e64  red columns, and
-0006c3c0: 2077 6974 6820 0a20 2020 2020 2020 2020   with .         
-0006c3d0: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
-0006c3e0: 756d 6e20 6e61 6d65 7320 7072 6566 6978  umn names prefix
-0006c3f0: 6564 2061 7320 7370 6563 6966 6965 642e  ed as specified.
-0006c400: 0a20 2020 2022 2222 0a20 2020 2069 6e64  .    """.    ind
-0006c410: 6620 3d20 696e 6466 2e6c 6f63 5b3a 2c20  f = indf.loc[:, 
-0006c420: 7e69 6e64 662e 636f 6c75 6d6e 732e 7374  ~indf.columns.st
-0006c430: 722e 636f 6e74 6169 6e73 2827 556e 6e61  r.contains('Unna
-0006c440: 6d65 642a 272c 206e 613d 4661 6c73 652c  med*', na=False,
-0006c450: 2072 6567 6578 3d54 7275 6529 5d0a 2020   regex=True)].  
-0006c460: 2020 6966 2069 6e64 662e 7368 6170 655b    if indf.shape[
-0006c470: 305d 203d 3d20 303a 0a20 2020 2020 2020  0] == 0:.       
-0006c480: 2072 6574 7572 6e20 696e 6466 0a20 2020   return indf.   
-0006c490: 206e 756d 7320 3d20 5b69 7369 6e73 7461   nums = [isinsta
-0006c4a0: 6e63 6528 696e 6466 5b63 6f6c 5d2e 696c  nce(indf[col].il
-0006c4b0: 6f63 5b30 5d2c 2028 6f62 6a65 6374 2c20  oc[0], (object, 
-0006c4c0: 696e 742c 2066 6c6f 6174 2929 2066 6f72  int, float)) for
-0006c4d0: 2063 6f6c 2069 6e20 696e 6466 2e63 6f6c   col in indf.col
-0006c4e0: 756d 6e73 5d0a 2020 2020 696e 6466 203d  umns].    indf =
-0006c4f0: 2069 6e64 662e 6c6f 635b 3a2c 206e 756d   indf.loc[:, num
-0006c500: 735d 0a20 2020 2069 6e64 6620 3d20 696e  s].    indf = in
-0006c510: 6466 2e6c 6f63 5b3a 2c20 696e 6466 2e64  df.loc[:, indf.d
-0006c520: 7479 7065 7320 213d 2027 6f62 6a65 6374  types != 'object
-0006c530: 275d 0a20 2020 2069 6e64 6620 3d20 7064  '].    indf = pd
-0006c540: 2e44 6174 6146 7261 6d65 2869 6e64 662e  .DataFrame(indf.
-0006c550: 6d65 616e 2861 7869 733d 302c 2073 6b69  mean(axis=0, ski
-0006c560: 706e 613d 5472 7565 2929 2e54 0a20 2020  pna=True)).T.   
-0006c570: 2069 6e64 6620 3d20 696e 6466 2e61 6464   indf = indf.add
-0006c580: 5f70 7265 6669 7828 6d79 7072 6566 6978  _prefix(myprefix
-0006c590: 290a 2020 2020 7265 7475 726e 2069 6e64  ).    return ind
-0006c5a0: 660a 0a0a 6465 6620 6167 6772 6567 6174  f...def aggregat
-0006c5b0: 655f 616e 7473 7079 6d6d 5f72 6573 756c  e_antspymm_resul
-0006c5c0: 7473 2869 6e70 7574 5f63 7376 2c20 7375  ts(input_csv, su
-0006c5d0: 626a 6563 745f 636f 6c3d 2773 7562 6a65  bject_col='subje
-0006c5e0: 6374 4944 272c 2064 6174 655f 636f 6c3d  ctID', date_col=
-0006c5f0: 2764 6174 6527 2c20 696d 6167 655f 636f  'date', image_co
-0006c600: 6c3d 2769 6d61 6765 4944 272c 2064 6174  l='imageID', dat
-0006c610: 655f 636f 6c75 6d6e 3d27 7365 732d 3127  e_column='ses-1'
-0006c620: 2c20 6261 7365 5f70 6174 683d 222e 2f50  , base_path="./P
-0006c630: 726f 6365 7373 6564 2f41 4e54 7345 7870  rocessed/ANTsExp
-0006c640: 4172 742f 222c 2068 6965 7276 6172 6961  Art/", hiervaria
-0006c650: 626c 653d 2754 3177 4869 6572 6172 6368  ble='T1wHierarch
-0006c660: 6963 616c 272c 2076 616c 6964 5f6d 6f64  ical', valid_mod
-0006c670: 616c 6974 6965 733d 4e6f 6e65 2c20 7665  alities=None, ve
-0006c680: 7262 6f73 653d 4661 6c73 6520 293a 0a20  rbose=False ):. 
-0006c690: 2020 2022 2222 0a20 2020 2041 6767 7265     """.    Aggre
-0006c6a0: 6761 7465 2041 4e54 7350 794d 4d20 7265  gate ANTsPyMM re
-0006c6b0: 7375 6c74 7320 6672 6f6d 2074 6865 2073  sults from the s
-0006c6c0: 7065 6369 6669 6564 2043 5356 2066 696c  pecified CSV fil
-0006c6d0: 6520 616e 6420 7361 7665 2074 6865 2061  e and save the a
-0006c6e0: 6767 7265 6761 7465 6420 7265 7375 6c74  ggregated result
-0006c6f0: 7320 746f 2061 206e 6577 2043 5356 2066  s to a new CSV f
-0006c700: 696c 652e 0a0a 2020 2020 5061 7261 6d65  ile...    Parame
-0006c710: 7465 7273 3a0a 2020 2020 2d20 696e 7075  ters:.    - inpu
-0006c720: 745f 6373 7620 2873 7472 293a 2046 696c  t_csv (str): Fil
-0006c730: 6520 7061 7468 206f 6620 7468 6520 696e  e path of the in
-0006c740: 7075 7420 4353 5620 6669 6c65 2063 6f6e  put CSV file con
-0006c750: 7461 696e 696e 6720 414e 5473 5079 4d4d  taining ANTsPyMM
-0006c760: 2051 4320 7265 7375 6c74 7320 6176 6572   QC results aver
-0006c770: 6167 6564 2061 6e64 2077 6974 6820 6f75  aged and with ou
-0006c780: 746c 6965 7220 6d65 6173 7572 656d 656e  tlier measuremen
-0006c790: 7473 2e0a 2020 2020 2d20 7375 626a 6563  ts..    - subjec
-0006c7a0: 745f 636f 6c20 2873 7472 293a 204e 616d  t_col (str): Nam
-0006c7b0: 6520 6f66 2074 6865 2063 6f6c 756d 6e20  e of the column 
-0006c7c0: 746f 2073 746f 7265 2073 7562 6a65 6374  to store subject
-0006c7d0: 2049 4473 2e0a 2020 2020 2d20 6461 7465   IDs..    - date
-0006c7e0: 5f63 6f6c 2028 7374 7229 3a20 4e61 6d65  _col (str): Name
-0006c7f0: 206f 6620 7468 6520 636f 6c75 6d6e 2074   of the column t
-0006c800: 6f20 7374 6f72 6520 6461 7465 2069 6e66  o store date inf
-0006c810: 6f72 6d61 7469 6f6e 2e0a 2020 2020 2d20  ormation..    - 
-0006c820: 696d 6167 655f 636f 6c20 2873 7472 293a  image_col (str):
-0006c830: 204e 616d 6520 6f66 2074 6865 2063 6f6c   Name of the col
-0006c840: 756d 6e20 746f 2073 746f 7265 2069 6d61  umn to store ima
-0006c850: 6765 2049 4473 2e0a 2020 2020 2d20 6461  ge IDs..    - da
-0006c860: 7465 5f63 6f6c 756d 6e20 2873 7472 293a  te_column (str):
-0006c870: 204e 616d 6520 6f66 2074 6865 2063 6f6c   Name of the col
-0006c880: 756d 6e20 7265 7072 6573 656e 7469 6e67  umn representing
-0006c890: 2074 6865 2064 6174 6520 696e 666f 726d   the date inform
-0006c8a0: 6174 696f 6e2e 0a20 2020 202d 2062 6173  ation..    - bas
-0006c8b0: 655f 7061 7468 2028 7374 7229 3a20 4261  e_path (str): Ba
-0006c8c0: 7365 2070 6174 6820 666f 7220 7365 6172  se path for sear
-0006c8d0: 6368 2070 6174 6873 2e20 4465 6661 756c  ch paths. Defaul
-0006c8e0: 7473 2074 6f20 222e 2f50 726f 6365 7373  ts to "./Process
-0006c8f0: 6564 2f41 4e54 7345 7870 4172 742f 222e  ed/ANTsExpArt/".
-0006c900: 0a20 2020 202d 2068 6965 7276 6172 6961  .    - hiervaria
-0006c910: 626c 6520 2873 7472 2920 3a20 7468 6520  ble (str) : the 
-0006c920: 7374 7269 6e67 2076 6172 6961 626c 6520  string variable 
-0006c930: 6465 6e6f 7469 6e67 2074 6865 2048 6965  denoting the Hie
-0006c940: 7261 7263 6869 6361 6c20 6f75 7470 7574  rarchical output
-0006c950: 0a20 2020 202d 2076 616c 6964 5f6d 6f64  .    - valid_mod
-0006c960: 616c 6974 6965 7320 2873 7472 2061 7272  alities (str arr
-0006c970: 6179 2920 3a20 6964 656e 7469 6669 6573  ay) : identifies
-0006c980: 2066 6f72 2065 6163 6820 6d6f 6461 6c69   for each modali
-0006c990: 7479 3b20 6966 204e 6f6e 6520 7769 6c6c  ty; if None will
-0006c9a0: 2062 6520 7265 706c 6163 6564 2062 7920   be replaced by 
-0006c9b0: 6765 745f 7661 6c69 645f 6d6f 6461 6c69  get_valid_modali
-0006c9c0: 7469 6573 286c 6f6e 673d 5472 7565 290a  ties(long=True).
-0006c9d0: 2020 2020 2d20 7665 7262 6f73 6520 3a20      - verbose : 
-0006c9e0: 626f 6f6c 6561 6e0a 0a20 2020 204e 6f74  boolean..    Not
-0006c9f0: 653a 0a20 2020 2054 6869 7320 6675 6e63  e:.    This func
-0006ca00: 7469 6f6e 2069 7320 7465 7374 6564 2075  tion is tested u
-0006ca10: 6e64 6572 206c 696d 6974 6564 2063 6972  nder limited cir
-0006ca20: 6375 6d73 7461 6e63 6573 2e20 5573 6520  cumstances. Use 
-0006ca30: 7769 7468 2063 6175 7469 6f6e 2e0a 0a20  with caution... 
-0006ca40: 2020 2045 7861 6d70 6c65 2075 7361 6765     Example usage
-0006ca50: 3a0a 2020 2020 6167 675f 6466 203d 2061  :.    agg_df = a
-0006ca60: 6767 7265 6761 7465 5f61 6e74 7370 796d  ggregate_antspym
-0006ca70: 6d5f 7265 7375 6c74 7328 2271 6364 6661  m_results("qcdfa
-0006ca80: 6f6c 2e63 7376 222c 2073 7562 6a65 6374  ol.csv", subject
-0006ca90: 5f63 6f6c 3d27 7375 626a 6563 7449 4427  _col='subjectID'
-0006caa0: 2c20 6461 7465 5f63 6f6c 3d27 6461 7465  , date_col='date
-0006cab0: 272c 2069 6d61 6765 5f63 6f6c 3d27 696d  ', image_col='im
-0006cac0: 6167 6549 4427 2c20 6461 7465 5f63 6f6c  ageID', date_col
-0006cad0: 756d 6e3d 2773 6573 2d31 272c 2062 6173  umn='ses-1', bas
-0006cae0: 655f 7061 7468 3d22 2e2f 596f 7572 2f43  e_path="./Your/C
-0006caf0: 7573 746f 6d2f 5061 7468 2f22 290a 0a20  ustom/Path/").. 
-0006cb00: 2020 2041 7574 686f 723a 0a20 2020 2041     Author:.    A
-0006cb10: 7661 6e74 7320 616e 6420 4368 6174 4750  vants and ChatGP
-0006cb20: 540a 2020 2020 2222 220a 2020 2020 696d  T.    """.    im
-0006cb30: 706f 7274 2070 616e 6461 7320 6173 2070  port pandas as p
-0006cb40: 640a 2020 2020 696d 706f 7274 206e 756d  d.    import num
-0006cb50: 7079 2061 7320 6e70 0a20 2020 2066 726f  py as np.    fro
-0006cb60: 6d20 676c 6f62 2069 6d70 6f72 7420 676c  m glob import gl
-0006cb70: 6f62 0a0a 2020 2020 6465 6620 6d79 7265  ob..    def myre
-0006cb80: 6164 5f63 7376 2878 2c20 636e 6d73 293a  ad_csv(x, cnms):
-0006cb90: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0006cba0: 2020 2020 2052 6561 6473 2061 2043 5356       Reads a CSV
-0006cbb0: 2066 696c 6520 616e 6420 7265 7475 726e   file and return
-0006cbc0: 7320 6120 4461 7461 4672 616d 6520 6578  s a DataFrame ex
-0006cbd0: 636c 7564 696e 6720 7370 6563 6966 6965  cluding specifie
-0006cbe0: 6420 636f 6c75 6d6e 732e 0a0a 2020 2020  d columns...    
-0006cbf0: 2020 2020 5061 7261 6d65 7465 7273 3a0a      Parameters:.
-0006cc00: 2020 2020 2020 2020 2d20 7820 2873 7472          - x (str
-0006cc10: 293a 2046 696c 6520 7061 7468 206f 6620  ): File path of 
-0006cc20: 7468 6520 696e 7075 7420 4353 5620 6669  the input CSV fi
-0006cc30: 6c65 2064 6573 6372 6962 696e 6720 7468  le describing th
-0006cc40: 6520 626c 696e 6420 5143 206f 7574 7075  e blind QC outpu
-0006cc50: 740a 2020 2020 2020 2020 2d20 636e 6d73  t.        - cnms
-0006cc60: 2028 6c69 7374 293a 204c 6973 7420 6f66   (list): List of
-0006cc70: 2063 6f6c 756d 6e20 6e61 6d65 7320 746f   column names to
-0006cc80: 2065 7863 6c75 6465 2066 726f 6d20 7468   exclude from th
-0006cc90: 6520 4461 7461 4672 616d 652e 0a0a 2020  e DataFrame...  
-0006cca0: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
-0006ccb0: 2020 2020 2020 2070 642e 4461 7461 4672         pd.DataFr
-0006ccc0: 616d 653a 2044 6174 6146 7261 6d65 2077  ame: DataFrame w
-0006ccd0: 6974 6820 7370 6563 6966 6965 6420 636f  ith specified co
-0006cce0: 6c75 6d6e 7320 6578 636c 7564 6564 2e0a  lumns excluded..
-0006ccf0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0006cd00: 2020 2020 6466 203d 2070 642e 7265 6164      df = pd.read
-0006cd10: 5f63 7376 2878 290a 2020 2020 2020 2020  _csv(x).        
-0006cd20: 7265 7475 726e 2064 662e 6c6f 635b 3a2c  return df.loc[:,
-0006cd30: 207e 6466 2e63 6f6c 756d 6e73 2e69 7369   ~df.columns.isi
-0006cd40: 6e28 636e 6d73 295d 0a0a 2020 2020 696d  n(cnms)]..    im
-0006cd50: 706f 7274 2077 6172 6e69 6e67 730a 2020  port warnings.  
-0006cd60: 2020 2320 5761 726e 696e 6720 6d65 7373    # Warning mess
-0006cd70: 6167 6520 666f 7220 756e 7465 7374 6564  age for untested
-0006cd80: 2066 756e 6374 696f 6e0a 2020 2020 7761   function.    wa
-0006cd90: 726e 696e 6773 2e77 6172 6e28 2257 6172  rnings.warn("War
-0006cda0: 6e69 6e67 3a20 5468 6973 2066 756e 6374  ning: This funct
-0006cdb0: 696f 6e20 6973 206e 6f74 2077 656c 6c20  ion is not well 
-0006cdc0: 7465 7374 6564 2e20 5573 6520 7769 7468  tested. Use with
-0006cdd0: 2063 6175 7469 6f6e 2e22 290a 0a20 2020   caution.")..   
-0006cde0: 2069 6620 7661 6c69 645f 6d6f 6461 6c69   if valid_modali
-0006cdf0: 7469 6573 2069 7320 4e6f 6e65 3a0a 2020  ties is None:.  
-0006ce00: 2020 2020 2020 7661 6c69 645f 6d6f 6461        valid_moda
-0006ce10: 6c69 7469 6573 203d 2067 6574 5f76 616c  lities = get_val
-0006ce20: 6964 5f6d 6f64 616c 6974 6965 7328 276c  id_modalities('l
-0006ce30: 6f6e 6727 290a 0a20 2020 2023 2052 6561  ong')..    # Rea
-0006ce40: 6420 7468 6520 696e 7075 7420 4353 5620  d the input CSV 
-0006ce50: 6669 6c65 0a20 2020 2064 6620 3d20 7064  file.    df = pd
-0006ce60: 2e72 6561 645f 6373 7628 696e 7075 745f  .read_csv(input_
-0006ce70: 6373 7629 0a0a 2020 2020 2320 4669 6c74  csv)..    # Filt
-0006ce80: 6572 2072 6f77 7320 7768 6572 6520 6d6f  er rows where mo
-0006ce90: 6461 6c69 7479 2069 7320 2754 3177 270a  dality is 'T1w'.
-0006cea0: 2020 2020 6466 203d 2064 665b 6466 5b27      df = df[df['
-0006ceb0: 6d6f 6461 6c69 7479 275d 203d 3d20 2754  modality'] == 'T
-0006cec0: 3177 275d 0a20 2020 2062 6164 6e61 6d65  1w'].    badname
-0006ced0: 7320 3d20 6765 745f 6e61 6d65 735f 6672  s = get_names_fr
-0006cee0: 6f6d 5f64 6174 615f 6672 616d 6528 205b  om_data_frame( [
-0006cef0: 2755 6e6e 616d 6564 275d 2c20 6466 2029  'Unnamed'], df )
-0006cf00: 0a20 2020 2064 663d 6466 2e64 726f 7028  .    df=df.drop(
-0006cf10: 6261 646e 616d 6573 2c20 6178 6973 3d31  badnames, axis=1
-0006cf20: 290a 0a20 2020 2023 2041 6464 206e 6577  )..    # Add new
-0006cf30: 2063 6f6c 756d 6e73 2066 6f72 2073 7562   columns for sub
-0006cf40: 6a65 6374 2049 442c 2064 6174 652c 2061  ject ID, date, a
-0006cf50: 6e64 2069 6d61 6765 2049 440a 2020 2020  nd image ID.    
-0006cf60: 6466 5b73 7562 6a65 6374 5f63 6f6c 5d20  df[subject_col] 
-0006cf70: 3d20 6e70 2e6e 616e 0a20 2020 2064 665b  = np.nan.    df[
-0006cf80: 6461 7465 5f63 6f6c 5d20 3d20 6461 7465  date_col] = date
-0006cf90: 5f63 6f6c 756d 6e0a 2020 2020 6466 5b69  _column.    df[i
-0006cfa0: 6d61 6765 5f63 6f6c 5d20 3d20 6e70 2e6e  mage_col] = np.n
-0006cfb0: 616e 0a20 2020 2064 6620 3d20 6466 2e61  an.    df = df.a
-0006cfc0: 7374 7970 6528 7b73 7562 6a65 6374 5f63  stype({subject_c
-0006cfd0: 6f6c 3a20 7374 722c 2064 6174 655f 636f  ol: str, date_co
-0006cfe0: 6c3a 2073 7472 2c20 696d 6167 655f 636f  l: str, image_co
-0006cff0: 6c3a 2073 7472 207d 290a 0a23 2020 2020  l: str })..#    
-0006d000: 6966 2076 6572 626f 7365 3a0a 2320 2020  if verbose:.#   
-0006d010: 2020 2020 2070 7269 6e74 2820 6466 2e73       print( df.s
-0006d020: 6861 7065 2029 0a23 2020 2020 2020 2020  hape ).#        
-0006d030: 7072 696e 7428 2064 662e 6474 7970 6573  print( df.dtypes
-0006d040: 2029 0a0a 2020 2020 2320 7072 6566 696c   )..    # prefil
-0006d050: 7465 7220 6466 2066 6f72 2064 6174 6120  ter df for data 
-0006d060: 7468 6174 2065 7869 7374 730a 2020 2020  that exists.    
-0006d070: 6b65 6570 203d 206e 702e 7469 6c65 2820  keep = np.tile( 
-0006d080: 4661 6c73 652c 2064 662e 7368 6170 655b  False, df.shape[
-0006d090: 305d 2029 0a20 2020 2066 6f72 2078 2069  0] ).    for x i
-0006d0a0: 6e20 7261 6e67 6528 6466 2e73 6861 7065  n range(df.shape
-0006d0b0: 5b30 5d29 3a0a 2020 2020 2020 2020 7465  [0]):.        te
-0006d0c0: 6d70 203d 2064 665b 2766 696c 656e 616d  mp = df['filenam
-0006d0d0: 6527 5d2e 696c 6f63 5b78 5d2e 7370 6c69  e'].iloc[x].spli
-0006d0e0: 7428 225f 2229 0a20 2020 2020 2020 2023  t("_").        #
-0006d0f0: 2047 656e 6572 616c 697a 6564 2073 6561   Generalized sea
-0006d100: 7263 6820 7061 7468 730a 2020 2020 2020  rch paths.      
-0006d110: 2020 7061 7468 5f74 656d 706c 6174 6520    path_template 
-0006d120: 3d20 6622 7b62 6173 655f 7061 7468 7d7b  = f"{base_path}{
-0006d130: 7465 6d70 5b30 5d7d 2f7b 6461 7465 5f63  temp[0]}/{date_c
-0006d140: 6f6c 756d 6e7d 2f2a 2f2a 2f2a 220a 2020  olumn}/*/*/*".  
-0006d150: 2020 2020 2020 6869 6572 666e 203d 2073        hierfn = s
-0006d160: 6f72 7465 6428 676c 6f62 2820 7061 7468  orted(glob( path
-0006d170: 5f74 656d 706c 6174 6520 2b20 222d 2220  _template + "-" 
-0006d180: 2b20 6869 6572 7661 7269 6162 6c65 202b  + hiervariable +
-0006d190: 2022 2d2a 7769 6465 2e63 7376 2220 2920   "-*wide.csv" ) 
-0006d1a0: 290a 2020 2020 2020 2020 6966 206c 656e  ).        if len
-0006d1b0: 2820 6869 6572 666e 2029 203e 2030 3a0a  ( hierfn ) > 0:.
-0006d1c0: 2020 2020 2020 2020 2020 2020 6b65 6570              keep
-0006d1d0: 5b78 5d3d 5472 7565 0a0a 2020 2020 0a20  [x]=True..    . 
-0006d1e0: 2020 2064 663d 6466 5b6b 6565 705d 0a20     df=df[keep]. 
-0006d1f0: 2020 200a 2020 2020 6966 2076 6572 626f     .    if verbo
-0006d200: 7365 3a0a 2020 2020 2020 2020 7072 696e  se:.        prin
-0006d210: 7428 2022 6f72 6967 696e 616c 2069 6e70  t( "original inp
-0006d220: 7574 2068 6164 2073 6861 7065 2022 202b  ut had shape " +
-0006d230: 2073 7472 2820 6466 2e73 6861 7065 5b30   str( df.shape[0
-0006d240: 5d20 2920 2b20 2220 2854 3120 6f6e 6c79  ] ) + " (T1 only
-0006d250: 2920 616e 6420 7765 2066 696e 6420 2220  ) and we find " 
-0006d260: 2b20 7374 7228 2028 6b65 6570 292e 7375  + str( (keep).su
-0006d270: 6d28 2920 2920 2b20 2220 7769 7468 2068  m() ) + " with h
-0006d280: 6965 7261 7263 6869 6361 6c20 6f75 7470  ierarchical outp
-0006d290: 7574 2064 6566 696e 6564 2062 7920 7661  ut defined by va
-0006d2a0: 7269 6162 6c65 3a20 2220 2b20 6869 6572  riable: " + hier
-0006d2b0: 7661 7269 6162 6c65 2029 0a20 2020 2020  variable ).     
-0006d2c0: 2020 2070 7269 6e74 2820 6466 2e73 6861     print( df.sha
-0006d2d0: 7065 2029 0a0a 2020 2020 6d79 6374 203d  pe )..    myct =
-0006d2e0: 2030 0a20 2020 2066 6f72 2078 2069 6e20   0.    for x in 
-0006d2f0: 7261 6e67 6528 2064 662e 7368 6170 655b  range( df.shape[
-0006d300: 305d 293a 0a20 2020 2020 2020 2069 6620  0]):.        if 
-0006d310: 7665 7262 6f73 653a 0a20 2020 2020 2020  verbose:.       
-0006d320: 2020 2020 2070 7269 6e74 2866 227b 787d       print(f"{x}
-0006d330: 2e2e 2e22 290a 2020 2020 2020 2020 6c6f  ...").        lo
-0006d340: 6369 6e64 203d 2064 662e 696e 6465 785b  cind = df.index[
-0006d350: 785d 0a20 2020 2020 2020 2074 656d 7020  x].        temp 
-0006d360: 3d20 6466 5b27 6669 6c65 6e61 6d65 275d  = df['filename']
-0006d370: 2e69 6c6f 635b 785d 2e73 706c 6974 2822  .iloc[x].split("
-0006d380: 5f22 290a 2020 2020 2020 2020 6966 2076  _").        if v
-0006d390: 6572 626f 7365 3a0a 2020 2020 2020 2020  erbose:.        
-0006d3a0: 2020 2020 7072 696e 7428 2074 656d 7020      print( temp 
-0006d3b0: 290a 2020 2020 2020 2020 6466 5b73 7562  ).        df[sub
-0006d3c0: 6a65 6374 5f63 6f6c 5d2e 696c 6f63 5b78  ject_col].iloc[x
-0006d3d0: 5d3d 7465 6d70 5b30 5d0a 2020 2020 2020  ]=temp[0].      
-0006d3e0: 2020 6466 5b64 6174 655f 636f 6c5d 2e69    df[date_col].i
-0006d3f0: 6c6f 635b 785d 3d64 6174 655f 636f 6c75  loc[x]=date_colu
-0006d400: 6d6e 0a20 2020 2020 2020 2064 665b 696d  mn.        df[im
-0006d410: 6167 655f 636f 6c5d 2e69 6c6f 635b 785d  age_col].iloc[x]
-0006d420: 3d74 656d 705b 315d 0a0a 2020 2020 2020  =temp[1]..      
-0006d430: 2020 2320 4765 6e65 7261 6c69 7a65 6420    # Generalized 
-0006d440: 7365 6172 6368 2070 6174 6873 0a20 2020  search paths.   
-0006d450: 2020 2020 2070 6174 685f 7465 6d70 6c61       path_templa
-0006d460: 7465 203d 2066 227b 6261 7365 5f70 6174  te = f"{base_pat
-0006d470: 687d 7b74 656d 705b 305d 7d2f 7b64 6174  h}{temp[0]}/{dat
-0006d480: 655f 636f 6c75 6d6e 7d2f 2a2f 2a2f 2a22  e_column}/*/*/*"
-0006d490: 0a20 2020 2020 2020 2069 6620 7665 7262  .        if verb
-0006d4a0: 6f73 653a 0a20 2020 2020 2020 2020 2020  ose:.           
-0006d4b0: 2070 7269 6e74 2870 6174 685f 7465 6d70   print(path_temp
-0006d4c0: 6c61 7465 290a 2020 2020 2020 2020 6869  late).        hi
-0006d4d0: 6572 666e 203d 2073 6f72 7465 6428 676c  erfn = sorted(gl
-0006d4e0: 6f62 2820 7061 7468 5f74 656d 706c 6174  ob( path_templat
-0006d4f0: 6520 2b20 222d 2220 2b20 6869 6572 7661  e + "-" + hierva
-0006d500: 7269 6162 6c65 202b 2022 2d2a 7769 6465  riable + "-*wide
-0006d510: 2e63 7376 2220 2920 290a 2020 2020 2020  .csv" ) ).      
-0006d520: 2020 6966 206c 656e 2820 6869 6572 666e    if len( hierfn
-0006d530: 2029 203e 2030 3a0a 2020 2020 2020 2020   ) > 0:.        
-0006d540: 2020 2020 6864 663d 7431 6466 3d64 7464      hdf=t1df=dtd
-0006d550: 663d 7273 6466 3d70 6572 6664 663d 6e6d  f=rsdf=perfdf=nm
-0006d560: 6466 3d66 6c61 6972 6466 3d4e 6f6e 650a  df=flairdf=None.
-0006d570: 2020 2020 2020 2020 2020 2020 6966 2076              if v
-0006d580: 6572 626f 7365 3a0a 2020 2020 2020 2020  erbose:.        
-0006d590: 2020 2020 2020 2020 7072 696e 7428 6869          print(hi
-0006d5a0: 6572 666e 290a 2020 2020 2020 2020 2020  erfn).          
-0006d5b0: 2020 6864 6620 3d20 7064 2e72 6561 645f    hdf = pd.read_
-0006d5c0: 6373 7628 6869 6572 666e 5b30 5d29 0a20  csv(hierfn[0]). 
-0006d5d0: 2020 2020 2020 2020 2020 2062 6164 6e61             badna
-0006d5e0: 6d65 7320 3d20 6765 745f 6e61 6d65 735f  mes = get_names_
-0006d5f0: 6672 6f6d 5f64 6174 615f 6672 616d 6528  from_data_frame(
-0006d600: 205b 2755 6e6e 616d 6564 275d 2c20 6864   ['Unnamed'], hd
-0006d610: 6620 290a 2020 2020 2020 2020 2020 2020  f ).            
-0006d620: 6864 663d 6864 662e 6472 6f70 2862 6164  hdf=hdf.drop(bad
-0006d630: 6e61 6d65 732c 2061 7869 733d 3129 0a20  names, axis=1). 
-0006d640: 2020 2020 2020 2020 2020 206e 756d 7320             nums 
-0006d650: 3d20 5b69 7369 6e73 7461 6e63 6528 6864  = [isinstance(hd
-0006d660: 665b 636f 6c5d 2e69 6c6f 635b 305d 2c20  f[col].iloc[0], 
-0006d670: 2869 6e74 2c20 666c 6f61 7429 2920 666f  (int, float)) fo
-0006d680: 7220 636f 6c20 696e 2068 6466 2e63 6f6c  r col in hdf.col
-0006d690: 756d 6e73 5d0a 2020 2020 2020 2020 2020  umns].          
-0006d6a0: 2020 636f 7265 6e61 6d65 7320 3d20 6c69    corenames = li
-0006d6b0: 7374 286e 702e 6172 7261 7928 6864 662e  st(np.array(hdf.
-0006d6c0: 636f 6c75 6d6e 7329 5b6e 756d 735d 290a  columns)[nums]).
-0006d6d0: 2020 2020 2020 2020 2020 2020 6864 662e              hdf.
-0006d6e0: 6c6f 635b 3a2c 206e 756d 735d 203d 2068  loc[:, nums] = h
-0006d6f0: 6466 2e6c 6f63 5b3a 2c20 6e75 6d73 5d2e  df.loc[:, nums].
-0006d700: 6164 645f 7072 6566 6978 2822 5431 4869  add_prefix("T1Hi
-0006d710: 6572 5f22 290a 2020 2020 2020 2020 2020  er_").          
-0006d720: 2020 6d79 6374 203d 206d 7963 7420 2b20    myct = myct + 
-0006d730: 310a 2020 2020 2020 2020 2020 2020 6466  1.            df
-0006d740: 6c69 7374 203d 205b 6864 665d 0a0a 2020  list = [hdf]..  
-0006d750: 2020 2020 2020 2020 2020 666f 7220 6d79            for my
-0006d760: 6d6f 6420 696e 2076 616c 6964 5f6d 6f64  mod in valid_mod
-0006d770: 616c 6974 6965 733a 0a20 2020 2020 2020  alities:.       
-0006d780: 2020 2020 2020 2020 2074 3177 666e 203d           t1wfn =
-0006d790: 2073 6f72 7465 6428 676c 6f62 2820 7061   sorted(glob( pa
-0006d7a0: 7468 5f74 656d 706c 6174 652b 2022 2d22  th_template+ "-"
-0006d7b0: 202b 206d 796d 6f64 202b 2022 2d2a 7769   + mymod + "-*wi
-0006d7c0: 6465 2e63 7376 2220 2920 290a 2020 2020  de.csv" ) ).    
-0006d7d0: 2020 2020 2020 2020 2020 2020 6966 206c              if l
-0006d7e0: 656e 2820 7431 7766 6e20 2920 3e20 3020  en( t1wfn ) > 0 
-0006d7f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0006d800: 2020 2020 2020 6966 2076 6572 626f 7365        if verbose
-0006d810: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0006d820: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-0006d830: 7431 7766 6e29 0a20 2020 2020 2020 2020  t1wfn).         
-0006d840: 2020 2020 2020 2020 2020 2074 3164 6620             t1df 
-0006d850: 3d20 6d79 7265 6164 5f63 7376 2874 3177  = myread_csv(t1w
-0006d860: 666e 5b30 5d2c 2063 6f72 656e 616d 6573  fn[0], corenames
-0006d870: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0006d880: 2020 2020 2020 7431 6466 203d 2066 696c        t1df = fil
-0006d890: 7465 725f 6466 2820 7431 6466 2c20 6d79  ter_df( t1df, my
-0006d8a0: 6d6f 642b 275f 2729 0a20 2020 2020 2020  mod+'_').       
-0006d8b0: 2020 2020 2020 2020 2020 2020 2064 666c               dfl
-0006d8c0: 6973 7420 3d20 6466 6c69 7374 202b 205b  ist = dflist + [
-0006d8d0: 7431 6466 5d0a 2020 2020 2020 2020 2020  t1df].          
-0006d8e0: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
-0006d8f0: 2020 2068 6466 203d 2070 642e 636f 6e63     hdf = pd.conc
-0006d900: 6174 2820 6466 6c69 7374 2c20 6178 6973  at( dflist, axis
-0006d910: 3d31 2c20 6967 6e6f 7265 5f69 6e64 6578  =1, ignore_index
-0006d920: 3d46 616c 7365 2029 0a20 2020 2020 2020  =False ).       
-0006d930: 2020 2020 2069 6620 7665 7262 6f73 653a       if verbose:
-0006d940: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0006d950: 2070 7269 6e74 2820 6466 2e6c 6f63 5b6c   print( df.loc[l
-0006d960: 6f63 696e 642c 2766 696c 656e 616d 6527  ocind,'filename'
-0006d970: 5d20 290a 2020 2020 2020 2020 2020 2020  ] ).            
-0006d980: 6966 206d 7963 7420 3d3d 2031 3a0a 2020  if myct == 1:.  
-0006d990: 2020 2020 2020 2020 2020 2020 2020 7375                su
-0006d9a0: 6264 6620 3d20 6466 2e69 6c6f 635b 5b78  bdf = df.iloc[[x
-0006d9b0: 5d5d 0a20 2020 2020 2020 2020 2020 2020  ]].             
-0006d9c0: 2020 2068 6466 2e69 6e64 6578 203d 2073     hdf.index = s
-0006d9d0: 7562 6466 2e69 6e64 6578 2e63 6f70 7928  ubdf.index.copy(
-0006d9e0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0006d9f0: 2020 6466 203d 2070 642e 636f 6e63 6174    df = pd.concat
-0006da00: 2820 5b64 662c 6864 665d 2c20 6178 6973  ( [df,hdf], axis
-0006da10: 3d31 2c20 6967 6e6f 7265 5f69 6e64 6578  =1, ignore_index
-0006da20: 3d46 616c 7365 2029 0a20 2020 2020 2020  =False ).       
-0006da30: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0006da40: 2020 2020 2020 2020 2020 2063 6f6d 6d63             commc
-0006da50: 6f6c 7320 3d20 6c69 7374 2873 6574 2868  ols = list(set(h
-0006da60: 6466 2e63 6f6c 756d 6e73 292e 696e 7465  df.columns).inte
-0006da70: 7273 6563 7469 6f6e 2864 662e 636f 6c75  rsection(df.colu
-0006da80: 6d6e 7329 290a 2020 2020 2020 2020 2020  mns)).          
-0006da90: 2020 2020 2020 6466 2e6c 6f63 5b6c 6f63        df.loc[loc
-0006daa0: 696e 642c 2063 6f6d 6d63 6f6c 735d 203d  ind, commcols] =
-0006dab0: 2068 6466 2e6c 6f63 5b30 2c20 636f 6d6d   hdf.loc[0, comm
-0006dac0: 636f 6c73 5d0a 2020 2020 6261 646e 616d  cols].    badnam
-0006dad0: 6573 203d 2067 6574 5f6e 616d 6573 5f66  es = get_names_f
-0006dae0: 726f 6d5f 6461 7461 5f66 7261 6d65 2820  rom_data_frame( 
-0006daf0: 5b27 556e 6e61 6d65 6427 5d2c 2064 6620  ['Unnamed'], df 
-0006db00: 290a 2020 2020 6466 3d64 662e 6472 6f70  ).    df=df.drop
-0006db10: 2862 6164 6e61 6d65 732c 2061 7869 733d  (badnames, axis=
-0006db20: 3129 0a20 2020 2072 6574 7572 6e28 2064  1).    return( d
-0006db30: 6620 290a 0a64 6566 2066 696e 645f 6d6f  f )..def find_mo
-0006db40: 7374 5f72 6563 656e 745f 6669 6c65 2866  st_recent_file(f
-0006db50: 696c 655f 6c69 7374 293a 0a20 2020 2022  ile_list):.    "
-0006db60: 2222 0a20 2020 2046 696e 6473 2061 6e64  "".    Finds and
-0006db70: 2072 6574 7572 6e73 2074 6865 206d 6f73   returns the mos
-0006db80: 7420 7265 6365 6e74 6c79 206d 6f64 6966  t recently modif
-0006db90: 6965 6420 6669 6c65 2066 726f 6d20 6120  ied file from a 
-0006dba0: 6c69 7374 206f 6620 6669 6c65 2070 6174  list of file pat
-0006dbb0: 6873 2e0a 2020 2020 0a20 2020 2050 6172  hs..    .    Par
-0006dbc0: 616d 6574 6572 733a 0a20 2020 202d 2066  ameters:.    - f
-0006dbd0: 696c 655f 6c69 7374 3a20 4120 6c69 7374  ile_list: A list
-0006dbe0: 206f 6620 7374 7269 6e67 732c 2077 6865   of strings, whe
-0006dbf0: 7265 2065 6163 6820 7374 7269 6e67 2069  re each string i
-0006dc00: 7320 6120 7061 7468 2074 6f20 6120 6669  s a path to a fi
-0006dc10: 6c65 2e0a 2020 2020 0a20 2020 2052 6574  le..    .    Ret
-0006dc20: 7572 6e73 3a0a 2020 2020 2d20 5468 6520  urns:.    - The 
-0006dc30: 7061 7468 2074 6f20 7468 6520 6d6f 7374  path to the most
-0006dc40: 2072 6563 656e 746c 7920 6d6f 6469 6669   recently modifi
-0006dc50: 6564 2066 696c 6520 696e 2074 6865 206c  ed file in the l
-0006dc60: 6973 742c 206f 7220 4e6f 6e65 2069 6620  ist, or None if 
-0006dc70: 7468 6520 6c69 7374 2069 7320 656d 7074  the list is empt
-0006dc80: 7920 6f72 2063 6f6e 7461 696e 7320 6e6f  y or contains no
-0006dc90: 2076 616c 6964 2066 696c 6573 2e0a 2020   valid files..  
-0006dca0: 2020 2222 220a 2020 2020 2320 4669 6c74    """.    # Filt
-0006dcb0: 6572 206f 7574 2069 7465 6d73 2074 6861  er out items tha
-0006dcc0: 7420 6172 6520 6e6f 7420 6669 6c65 7320  t are not files 
-0006dcd0: 6f72 2064 6f20 6e6f 7420 6578 6973 740a  or do not exist.
-0006dce0: 2020 2020 7661 6c69 645f 6669 6c65 7320      valid_files 
-0006dcf0: 3d20 5b66 2066 6f72 2066 2069 6e20 6669  = [f for f in fi
-0006dd00: 6c65 5f6c 6973 7420 6966 206f 732e 7061  le_list if os.pa
-0006dd10: 7468 2e69 7366 696c 6528 6629 5d0a 2020  th.isfile(f)].  
-0006dd20: 2020 0a20 2020 2023 2043 6865 636b 2069    .    # Check i
-0006dd30: 6620 7468 6520 6669 6c74 6572 6564 206c  f the filtered l
-0006dd40: 6973 7420 6973 206e 6f74 2065 6d70 7479  ist is not empty
-0006dd50: 0a20 2020 2069 6620 7661 6c69 645f 6669  .    if valid_fi
-0006dd60: 6c65 733a 0a20 2020 2020 2020 2023 2046  les:.        # F
-0006dd70: 696e 6420 7468 6520 6669 6c65 2077 6974  ind the file wit
-0006dd80: 6820 7468 6520 6c61 7465 7374 206d 6f64  h the latest mod
-0006dd90: 6966 6963 6174 696f 6e20 7469 6d65 0a20  ification time. 
-0006dda0: 2020 2020 2020 206d 6f73 745f 7265 6365         most_rece
-0006ddb0: 6e74 5f66 696c 6520 3d20 6d61 7828 7661  nt_file = max(va
-0006ddc0: 6c69 645f 6669 6c65 732c 206b 6579 3d6f  lid_files, key=o
-0006ddd0: 732e 7061 7468 2e67 6574 6d74 696d 6529  s.path.getmtime)
-0006dde0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0006ddf0: 5b6d 6f73 745f 7265 6365 6e74 5f66 696c  [most_recent_fil
-0006de00: 655d 0a20 2020 2065 6c73 653a 0a20 2020  e].    else:.   
-0006de10: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
-0006de20: 0a20 2020 200a 6465 6620 6167 6772 6567  .    .def aggreg
-0006de30: 6174 655f 616e 7473 7079 6d6d 5f72 6573  ate_antspymm_res
-0006de40: 756c 7473 5f73 6466 280a 2020 2020 7374  ults_sdf(.    st
-0006de50: 7564 795f 6466 2c20 0a20 2020 2070 726f  udy_df, .    pro
-0006de60: 6a65 6374 5f63 6f6c 3d27 7072 6f6a 6563  ject_col='projec
-0006de70: 7449 4427 2c0a 2020 2020 7375 626a 6563  tID',.    subjec
-0006de80: 745f 636f 6c3d 2773 7562 6a65 6374 4944  t_col='subjectID
-0006de90: 272c 200a 2020 2020 6461 7465 5f63 6f6c  ', .    date_col
-0006dea0: 3d27 6461 7465 272c 200a 2020 2020 696d  ='date', .    im
-0006deb0: 6167 655f 636f 6c3d 2769 6d61 6765 4944  age_col='imageID
-0006dec0: 272c 200a 2020 2020 6261 7365 5f70 6174  ', .    base_pat
-0006ded0: 683d 222e 2f22 2c20 0a20 2020 2068 6965  h="./", .    hie
-0006dee0: 7276 6172 6961 626c 653d 2754 3177 4869  rvariable='T1wHi
-0006def0: 6572 6172 6368 6963 616c 272c 200a 2020  erarchical', .  
-0006df00: 2020 7370 6c69 7473 6570 3d27 2d27 2c0a    splitsep='-',.
-0006df10: 2020 2020 6964 7365 703d 272d 272c 0a20      idsep='-',. 
-0006df20: 2020 2077 696c 645f 6361 7264 5f6d 6f64     wild_card_mod
-0006df30: 616c 6974 795f 6964 3d46 616c 7365 2c0a  ality_id=False,.
-0006df40: 2020 2020 7665 7262 6f73 653d 4661 6c73      verbose=Fals
-0006df50: 6520 293a 0a20 2020 2022 2222 0a20 2020  e ):.    """.   
-0006df60: 2041 6767 7265 6761 7465 2041 4e54 7350   Aggregate ANTsP
-0006df70: 794d 4d20 7265 7375 6c74 7320 6672 6f6d  yMM results from
-0006df80: 2074 6865 2073 7065 6369 6669 6564 2073   the specified s
-0006df90: 7475 6479 2064 6174 6120 6672 616d 6520  tudy data frame 
-0006dfa0: 616e 6420 7374 6f72 6520 7468 6520 6167  and store the ag
-0006dfb0: 6772 6567 6174 6564 2072 6573 756c 7473  gregated results
-0006dfc0: 2069 6e20 6120 6e65 7720 6461 7461 2066   in a new data f
-0006dfd0: 7261 6d65 2e20 2054 6869 7320 6173 7375  rame.  This assu
-0006dfe0: 6d65 7320 6461 7461 2069 7320 6f72 6761  mes data is orga
-0006dff0: 6e69 7a65 6420 6f6e 2064 6973 6b20 0a20  nized on disk . 
-0006e000: 2020 2061 7320 666f 6c6c 6f77 733a 2020     as follows:  
-0006e010: 726f 6f74 6469 722f 7072 6f6a 6563 7449  rootdir/projectI
-0006e020: 442f 7375 626a 6563 7449 442f 6461 7465  D/subjectID/date
-0006e030: 2f6f 7574 7075 7469 642f 696d 6167 6569  /outputid/imagei
-0006e040: 642f 2077 6865 7265 200a 2020 2020 6f75  d/ where .    ou
-0006e050: 7470 7574 6964 2069 7320 6d6f 6461 6c69  tputid is modali
-0006e060: 7479 2d73 7065 6369 6669 6320 616e 6420  ty-specific and 
-0006e070: 6372 6561 7465 6420 6279 2041 4e54 7350  created by ANTsP
-0006e080: 794d 4d20 7072 6f63 6573 7369 6e67 2e0a  yMM processing..
-0006e090: 0a20 2020 2050 6172 616d 6574 6572 733a  .    Parameters:
-0006e0a0: 0a20 2020 202d 2073 7475 6479 5f64 6620  .    - study_df 
-0006e0b0: 2870 616e 6461 7320 6466 293a 2070 616e  (pandas df): pan
-0006e0c0: 6461 7320 6461 7461 2066 7261 6d65 2c20  das data frame, 
-0006e0d0: 6f75 7470 7574 206f 6620 6765 6e65 7261  output of genera
-0006e0e0: 7465 5f6d 6d5f 6461 7461 6672 616d 652e  te_mm_dataframe.
-0006e0f0: 0a20 2020 202d 2070 726f 6a65 6374 5f63  .    - project_c
-0006e100: 6f6c 2028 7374 7229 3a20 4e61 6d65 206f  ol (str): Name o
-0006e110: 6620 7468 6520 636f 6c75 6d6e 2074 6861  f the column tha
-0006e120: 7420 7374 6f72 6573 2074 6865 2070 726f  t stores the pro
-0006e130: 6a65 6374 2049 440a 2020 2020 2d20 7375  ject ID.    - su
-0006e140: 626a 6563 745f 636f 6c20 2873 7472 293a  bject_col (str):
-0006e150: 204e 616d 6520 6f66 2074 6865 2063 6f6c   Name of the col
-0006e160: 756d 6e20 746f 2073 746f 7265 2073 7562  umn to store sub
-0006e170: 6a65 6374 2049 4473 2e0a 2020 2020 2d20  ject IDs..    - 
-0006e180: 6461 7465 5f63 6f6c 2028 7374 7229 3a20  date_col (str): 
-0006e190: 4e61 6d65 206f 6620 7468 6520 636f 6c75  Name of the colu
-0006e1a0: 6d6e 2074 6f20 7374 6f72 6520 6461 7465  mn to store date
-0006e1b0: 2069 6e66 6f72 6d61 7469 6f6e 2e0a 2020   information..  
-0006e1c0: 2020 2d20 696d 6167 655f 636f 6c20 2873    - image_col (s
-0006e1d0: 7472 293a 204e 616d 6520 6f66 2074 6865  tr): Name of the
-0006e1e0: 2063 6f6c 756d 6e20 746f 2073 746f 7265   column to store
-0006e1f0: 2069 6d61 6765 2049 4473 2e0a 2020 2020   image IDs..    
-0006e200: 2d20 6261 7365 5f70 6174 6820 2873 7472  - base_path (str
-0006e210: 293a 2042 6173 6520 7061 7468 2066 6f72  ): Base path for
-0006e220: 2073 6561 7263 6869 6e67 2066 6f72 2070   searching for p
-0006e230: 726f 6365 7373 696e 6720 6f75 7470 7574  rocessing output
-0006e240: 7320 6f66 2041 4e54 7350 794d 4d2e 0a20  s of ANTsPyMM.. 
-0006e250: 2020 202d 2068 6965 7276 6172 6961 626c     - hiervariabl
-0006e260: 6520 2873 7472 2920 3a20 7468 6520 7374  e (str) : the st
-0006e270: 7269 6e67 2076 6172 6961 626c 6520 6465  ring variable de
-0006e280: 6e6f 7469 6e67 2074 6865 2048 6965 7261  noting the Hiera
-0006e290: 7263 6869 6361 6c20 6f75 7470 7574 0a20  rchical output. 
-0006e2a0: 2020 202d 2073 706c 6974 7365 7020 2873     - splitsep (s
-0006e2b0: 7472 293a 2020 7468 6520 7365 7061 7261  tr):  the separa
-0006e2c0: 746f 7220 7573 6564 2074 6f20 7370 6c69  tor used to spli
-0006e2d0: 7420 7468 6520 6669 6c65 6e61 6d65 0a20  t the filename. 
-0006e2e0: 2020 202d 2069 6473 6570 2028 7374 7229     - idsep (str)
-0006e2f0: 3a20 7468 6520 7365 7061 7261 746f 7220  : the separator 
-0006e300: 7573 6564 2074 6f20 7061 7274 6974 696f  used to partitio
-0006e310: 6e20 7375 626a 6563 7469 6420 6461 7465  n subjectid date
-0006e320: 2061 6e64 2069 6d61 6765 6964 200a 2020   and imageid .  
-0006e330: 2020 2020 2020 666f 7220 6578 616d 706c        for exampl
-0006e340: 652c 2069 6620 6964 7365 7020 6973 202d  e, if idsep is -
-0006e350: 2074 6865 6e20 7765 2068 6176 6520 7375   then we have su
-0006e360: 626a 6563 7469 642d 6461 7465 2d69 6d61  bjectid-date-ima
-0006e370: 6765 6964 0a20 2020 202d 2077 696c 645f  geid.    - wild_
-0006e380: 6361 7264 5f6d 6f64 616c 6974 795f 6964  card_modality_id
-0006e390: 2028 626f 6f6c 293a 206b 6565 7020 6966   (bool): keep if
-0006e3a0: 2046 616c 7365 2066 6f72 2073 6166 6572   False for safer
-0006e3b0: 2065 7865 6375 7469 6f6e 0a20 2020 202d   execution.    -
-0006e3c0: 2076 6572 626f 7365 203a 2062 6f6f 6c65   verbose : boole
-0006e3d0: 616e 0a0a 2020 2020 4e6f 7465 3a0a 2020  an..    Note:.  
-0006e3e0: 2020 5468 6973 2066 756e 6374 696f 6e20    This function 
-0006e3f0: 6973 2074 6573 7465 6420 756e 6465 7220  is tested under 
-0006e400: 6c69 6d69 7465 6420 6369 7263 756d 7374  limited circumst
-0006e410: 616e 6365 732e 2055 7365 2077 6974 6820  ances. Use with 
-0006e420: 6361 7574 696f 6e2e 0a20 2020 204f 6e65  caution..    One
-0006e430: 2070 6172 7469 6375 6c61 7220 676f 7463   particular gotc
-0006e440: 6861 2069 7320 6966 2074 6865 2069 6d61  ha is if the ima
-0006e450: 6765 4944 2069 7320 7374 6f72 6564 2061  geID is stored a
-0006e460: 7320 6120 6e75 6d65 7269 6320 7661 6c75  s a numeric valu
-0006e470: 6520 696e 2074 6865 2064 6174 6166 7261  e in the datafra
-0006e480: 6d65 200a 2020 2020 6275 7420 6973 206d  me .    but is m
-0006e490: 6561 6e74 2074 6f20 6265 2061 2073 7472  eant to be a str
-0006e4a0: 696e 672e 2020 452e 672e 2027 3030 3027  ing.  E.g. '000'
-0006e4b0: 2028 7374 7269 6e67 2920 776f 756c 6420   (string) would 
-0006e4c0: 6265 2069 6e74 6572 7072 6574 6564 2061  be interpreted a
-0006e4d0: 7320 3020 696e 2074 6865 200a 2020 2020  s 0 in the .    
-0006e4e0: 6669 6c65 206e 616d 6520 676c 6f62 2e20  file name glob. 
-0006e4f0: 2054 6869 7320 776f 756c 6420 6d69 7373   This would miss
-0006e500: 2074 6865 2065 7874 616e 7420 286f 6e20   the extant (on 
-0006e510: 6469 736b 2920 6373 762e 0a0a 2020 2020  disk) csv...    
-0006e520: 4578 616d 706c 6520 7573 6167 653a 0a20  Example usage:. 
-0006e530: 2020 2061 6767 5f64 6620 3d20 6167 6772     agg_df = aggr
-0006e540: 6567 6174 655f 616e 7473 7079 6d6d 5f72  egate_antspymm_r
-0006e550: 6573 756c 7473 5f73 6466 2820 7374 7564  esults_sdf( stud
-0006e560: 7964 662c 2073 7562 6a65 6374 5f63 6f6c  ydf, subject_col
-0006e570: 3d27 7375 626a 6563 7449 4427 2c20 6461  ='subjectID', da
-0006e580: 7465 5f63 6f6c 3d27 6461 7465 272c 2069  te_col='date', i
-0006e590: 6d61 6765 5f63 6f6c 3d27 696d 6167 6549  mage_col='imageI
-0006e5a0: 4427 2c20 6261 7365 5f70 6174 683d 222e  D', base_path=".
-0006e5b0: 2f59 6f75 722f 4375 7374 6f6d 2f50 6174  /Your/Custom/Pat
-0006e5c0: 682f 2229 0a0a 2020 2020 4175 7468 6f72  h/")..    Author
-0006e5d0: 3a0a 2020 2020 4176 616e 7473 2061 6e64  :.    Avants and
-0006e5e0: 2043 6861 7447 5054 0a20 2020 2022 2222   ChatGPT.    """
-0006e5f0: 0a20 2020 2069 6d70 6f72 7420 7061 6e64  .    import pand
-0006e600: 6173 2061 7320 7064 0a20 2020 2069 6d70  as as pd.    imp
-0006e610: 6f72 7420 6e75 6d70 7920 6173 206e 700a  ort numpy as np.
-0006e620: 2020 2020 6672 6f6d 2067 6c6f 6220 696d      from glob im
-0006e630: 706f 7274 2067 6c6f 620a 0a20 2020 2064  port glob..    d
-0006e640: 6566 2070 726f 6772 6573 735f 7265 706f  ef progress_repo
-0006e650: 7274 6572 2863 7572 7265 6e74 5f73 7465  rter(current_ste
-0006e660: 702c 2074 6f74 616c 5f73 7465 7073 2c20  p, total_steps, 
-0006e670: 7769 6474 683d 3530 293a 0a20 2020 2020  width=50):.     
-0006e680: 2020 2023 2043 616c 6375 6c61 7465 2074     # Calculate t
-0006e690: 6865 2070 726f 706f 7274 696f 6e20 6f66  he proportion of
-0006e6a0: 2070 726f 6772 6573 730a 2020 2020 2020   progress.      
-0006e6b0: 2020 7072 6f67 7265 7373 203d 2063 7572    progress = cur
-0006e6c0: 7265 6e74 5f73 7465 7020 2f20 746f 7461  rent_step / tota
-0006e6d0: 6c5f 7374 6570 730a 2020 2020 2020 2020  l_steps.        
-0006e6e0: 2320 4361 6c63 756c 6174 6520 7468 6520  # Calculate the 
-0006e6f0: 6e75 6d62 6572 206f 6620 2766 696c 6c65  number of 'fille
-0006e700: 6427 2063 6861 7261 6374 6572 7320 696e  d' characters in
-0006e710: 2074 6865 2070 726f 6772 6573 7320 6261   the progress ba
-0006e720: 720a 2020 2020 2020 2020 6669 6c6c 6564  r.        filled
-0006e730: 5f6c 656e 6774 6820 3d20 696e 7428 7769  _length = int(wi
-0006e740: 6474 6820 2a20 7072 6f67 7265 7373 290a  dth * progress).
-0006e750: 2020 2020 2020 2020 2320 4372 6561 7465          # Create
-0006e760: 2074 6865 2070 726f 6772 6573 7320 6261   the progress ba
-0006e770: 7220 7374 7269 6e67 0a20 2020 2020 2020  r string.       
-0006e780: 2062 6172 203d 2027 e296 8827 202a 2066   bar = '...' * f
-0006e790: 696c 6c65 645f 6c65 6e67 7468 202b 2027  illed_length + '
-0006e7a0: 2d27 202a 2028 7769 6474 6820 2d20 6669  -' * (width - fi
-0006e7b0: 6c6c 6564 5f6c 656e 6774 6829 0a20 2020  lled_length).   
-0006e7c0: 2020 2020 2023 2050 7269 6e74 2074 6865       # Print the
-0006e7d0: 2070 726f 6772 6573 7320 6261 7220 7769   progress bar wi
-0006e7e0: 7468 2070 6572 6365 6e74 6167 650a 2020  th percentage.  
-0006e7f0: 2020 2020 2020 7072 696e 7428 6627 5c72        print(f'\r
-0006e800: 5072 6f67 7265 7373 3a20 7c7b 6261 727d  Progress: |{bar}
-0006e810: 7c20 7b69 6e74 2831 3030 202a 2070 726f  | {int(100 * pro
-0006e820: 6772 6573 7329 7d25 272c 2065 6e64 3d27  gress)}%', end='
-0006e830: 5c72 2729 0a20 2020 2020 2020 2023 2050  \r').        # P
-0006e840: 7269 6e74 2061 206e 6577 206c 696e 6520  rint a new line 
-0006e850: 7768 656e 2074 6865 2070 726f 6772 6573  when the progres
-0006e860: 7320 6973 2063 6f6d 706c 6574 650a 2020  s is complete.  
-0006e870: 2020 2020 2020 6966 2063 7572 7265 6e74        if current
-0006e880: 5f73 7465 7020 3d3d 2074 6f74 616c 5f73  _step == total_s
-0006e890: 7465 7073 3a0a 2020 2020 2020 2020 2020  teps:.          
-0006e8a0: 2020 7072 696e 7428 290a 0a20 2020 2064    print()..    d
-0006e8b0: 6566 206d 7972 6561 645f 6373 7628 782c  ef myread_csv(x,
-0006e8c0: 2063 6e6d 7329 3a0a 2020 2020 2020 2020   cnms):.        
-0006e8d0: 2222 220a 2020 2020 2020 2020 5265 6164  """.        Read
-0006e8e0: 7320 6120 4353 5620 6669 6c65 2061 6e64  s a CSV file and
-0006e8f0: 2072 6574 7572 6e73 2061 2044 6174 6146   returns a DataF
-0006e900: 7261 6d65 2065 7863 6c75 6469 6e67 2073  rame excluding s
-0006e910: 7065 6369 6669 6564 2063 6f6c 756d 6e73  pecified columns
-0006e920: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
-0006e930: 6574 6572 733a 0a20 2020 2020 2020 202d  eters:.        -
-0006e940: 2078 2028 7374 7229 3a20 4669 6c65 2070   x (str): File p
-0006e950: 6174 6820 6f66 2074 6865 2069 6e70 7574  ath of the input
-0006e960: 2043 5356 2066 696c 6520 6465 7363 7269   CSV file descri
-0006e970: 6269 6e67 2074 6865 2062 6c69 6e64 2051  bing the blind Q
-0006e980: 4320 6f75 7470 7574 0a20 2020 2020 2020  C output.       
-0006e990: 202d 2063 6e6d 7320 286c 6973 7429 3a20   - cnms (list): 
-0006e9a0: 4c69 7374 206f 6620 636f 6c75 6d6e 206e  List of column n
-0006e9b0: 616d 6573 2074 6f20 6578 636c 7564 6520  ames to exclude 
-0006e9c0: 6672 6f6d 2074 6865 2044 6174 6146 7261  from the DataFra
-0006e9d0: 6d65 2e0a 0a20 2020 2020 2020 2052 6574  me...        Ret
-0006e9e0: 7572 6e73 3a0a 2020 2020 2020 2020 7064  urns:.        pd
-0006e9f0: 2e44 6174 6146 7261 6d65 3a20 4461 7461  .DataFrame: Data
-0006ea00: 4672 616d 6520 7769 7468 2073 7065 6369  Frame with speci
-0006ea10: 6669 6564 2063 6f6c 756d 6e73 2065 7863  fied columns exc
-0006ea20: 6c75 6465 642e 0a20 2020 2020 2020 2022  luded..        "
-0006ea30: 2222 0a20 2020 2020 2020 2064 6620 3d20  "".        df = 
-0006ea40: 7064 2e72 6561 645f 6373 7628 7829 0a20  pd.read_csv(x). 
-0006ea50: 2020 2020 2020 2072 6574 7572 6e20 6466         return df
-0006ea60: 2e6c 6f63 5b3a 2c20 7e64 662e 636f 6c75  .loc[:, ~df.colu
-0006ea70: 6d6e 732e 6973 696e 2863 6e6d 7329 5d0a  mns.isin(cnms)].
-0006ea80: 0a20 2020 2069 6d70 6f72 7420 7761 726e  .    import warn
-0006ea90: 696e 6773 0a20 2020 2023 2057 6172 6e69  ings.    # Warni
-0006eaa0: 6e67 206d 6573 7361 6765 2066 6f72 2075  ng message for u
-0006eab0: 6e74 6573 7465 6420 6675 6e63 7469 6f6e  ntested function
-0006eac0: 0a20 2020 2077 6172 6e69 6e67 732e 7761  .    warnings.wa
-0006ead0: 726e 2822 5761 726e 696e 673a 2054 6869  rn("Warning: Thi
-0006eae0: 7320 6675 6e63 7469 6f6e 2069 7320 6e6f  s function is no
-0006eaf0: 7420 7765 6c6c 2074 6573 7465 642e 2055  t well tested. U
-0006eb00: 7365 2077 6974 6820 6361 7574 696f 6e2e  se with caution.
-0006eb10: 2229 0a0a 2020 2020 766d 6f64 6469 6374  ")..    vmoddict
-0006eb20: 203d 207b 7d0a 2020 2020 2320 4164 6420   = {}.    # Add 
-0006eb30: 6b65 792d 7661 6c75 6520 7061 6972 730a  key-value pairs.
-0006eb40: 2020 2020 766d 6f64 6469 6374 5b27 696d      vmoddict['im
-0006eb50: 6167 6549 4427 5d20 3d20 2754 3177 270a  ageID'] = 'T1w'.
-0006eb60: 2020 2020 766d 6f64 6469 6374 5b27 666c      vmoddict['fl
-0006eb70: 6169 7269 6427 5d20 3d20 2754 3246 6c61  airid'] = 'T2Fla
-0006eb80: 6972 270a 2020 2020 766d 6f64 6469 6374  ir'.    vmoddict
-0006eb90: 5b27 7065 7266 6964 275d 203d 2027 7065  ['perfid'] = 'pe
-0006eba0: 7266 270a 2020 2020 766d 6f64 6469 6374  rf'.    vmoddict
-0006ebb0: 5b27 7273 6669 6431 275d 203d 2027 7273  ['rsfid1'] = 'rs
-0006ebc0: 664d 5249 270a 2320 2020 2076 6d6f 6464  fMRI'.#    vmodd
-0006ebd0: 6963 745b 2772 7366 6964 3227 5d20 3d20  ict['rsfid2'] = 
-0006ebe0: 2772 7366 4d52 4927 0a20 2020 2076 6d6f  'rsfMRI'.    vmo
-0006ebf0: 6464 6963 745b 2764 7469 6431 275d 203d  ddict['dtid1'] =
-0006ec00: 2027 4454 4927 0a23 2020 2020 766d 6f64   'DTI'.#    vmod
-0006ec10: 6469 6374 5b27 6474 6964 3227 5d20 3d20  dict['dtid2'] = 
-0006ec20: 2744 5449 270a 2020 2020 766d 6f64 6469  'DTI'.    vmoddi
-0006ec30: 6374 5b27 6e6d 6964 3127 5d20 3d20 274e  ct['nmid1'] = 'N
-0006ec40: 4d32 444d 5427 0a23 2020 2020 766d 6f64  M2DMT'.#    vmod
-0006ec50: 6469 6374 5b27 6e6d 6964 3227 5d20 3d20  dict['nmid2'] = 
-0006ec60: 274e 4d32 444d 5427 0a0a 2020 2020 2320  'NM2DMT'..    # 
-0006ec70: 4669 6c74 6572 2072 6f77 7320 7768 6572  Filter rows wher
-0006ec80: 6520 6d6f 6461 6c69 7479 2069 7320 2754  e modality is 'T
-0006ec90: 3177 270a 2020 2020 6466 203d 2073 7475  1w'.    df = stu
-0006eca0: 6479 5f64 665b 2073 7475 6479 5f64 665b  dy_df[ study_df[
-0006ecb0: 276d 6f64 616c 6974 7927 5d20 3d3d 2027  'modality'] == '
-0006ecc0: 5431 7727 5d0a 2020 2020 6261 646e 616d  T1w'].    badnam
-0006ecd0: 6573 203d 2067 6574 5f6e 616d 6573 5f66  es = get_names_f
-0006ece0: 726f 6d5f 6461 7461 5f66 7261 6d65 2820  rom_data_frame( 
-0006ecf0: 5b27 556e 6e61 6d65 6427 5d2c 2064 6620  ['Unnamed'], df 
-0006ed00: 290a 2020 2020 6466 3d64 662e 6472 6f70  ).    df=df.drop
-0006ed10: 2862 6164 6e61 6d65 732c 2061 7869 733d  (badnames, axis=
-0006ed20: 3129 0a20 2020 2023 2070 7265 6669 6c74  1).    # prefilt
-0006ed30: 6572 2064 6620 666f 7220 6461 7461 2074  er df for data t
-0006ed40: 6861 7420 6578 6973 7473 0a20 2020 206b  hat exists.    k
-0006ed50: 6565 7020 3d20 6e70 2e74 696c 6528 2046  eep = np.tile( F
-0006ed60: 616c 7365 2c20 6466 2e73 6861 7065 5b30  alse, df.shape[0
-0006ed70: 5d20 290a 2020 2020 666f 7220 7820 696e  ] ).    for x in
-0006ed80: 2072 616e 6765 2864 662e 7368 6170 655b   range(df.shape[
-0006ed90: 305d 293a 0a20 2020 2020 2020 206d 7966  0]):.        myf
-0006eda0: 6e20 3d20 6f73 2e70 6174 682e 6261 7365  n = os.path.base
-0006edb0: 6e61 6d65 2820 6466 5b27 6669 6c65 6e61  name( df['filena
-0006edc0: 6d65 275d 2e69 6c6f 635b 785d 2029 0a20  me'].iloc[x] ). 
-0006edd0: 2020 2020 2020 2074 656d 7020 3d20 6d79         temp = my
-0006ede0: 666e 2e73 706c 6974 2820 7370 6c69 7473  fn.split( splits
-0006edf0: 6570 2029 0a20 2020 2020 2020 2023 2047  ep ).        # G
-0006ee00: 656e 6572 616c 697a 6564 2073 6561 7263  eneralized searc
-0006ee10: 6820 7061 7468 730a 2020 2020 2020 2020  h paths.        
-0006ee20: 7369 6430 203d 2073 7472 2820 7465 6d70  sid0 = str( temp
-0006ee30: 5b30 5d20 290a 2020 2020 2020 2020 7369  [0] ).        si
-0006ee40: 6420 3d20 7374 7228 2064 665b 7375 626a  d = str( df[subj
-0006ee50: 6563 745f 636f 6c5d 2e69 6c6f 635b 785d  ect_col].iloc[x]
-0006ee60: 2029 0a20 2020 2020 2020 2069 6620 7369   ).        if si
-0006ee70: 6430 2021 3d20 7369 643a 0a20 2020 2020  d0 != sid:.     
-0006ee80: 2020 2020 2020 2077 6172 6e69 6e67 732e         warnings.
-0006ee90: 7761 726e 2822 4f55 5445 523a 2074 6865  warn("OUTER: the
-0006eea0: 2069 6420 6465 7269 7665 6420 6672 6f6d   id derived from
-0006eeb0: 2074 6865 2066 696c 656e 616d 6520 2220   the filename " 
-0006eec0: 2b20 7369 6420 2b20 2220 646f 6573 206e  + sid + " does n
-0006eed0: 6f74 206d 6174 6368 2074 6865 2069 6420  ot match the id 
-0006eee0: 7374 6f72 6564 2069 6e20 7468 6520 6461  stored in the da
-0006eef0: 7461 2066 7261 6d65 2022 202b 2073 6964  ta frame " + sid
-0006ef00: 2029 0a20 2020 2020 2020 2020 2020 2077   ).            w
-0006ef10: 6172 6e69 6e67 732e 7761 726e 2820 2266  arnings.warn( "f
-0006ef20: 696c 656e 616d 6520 6973 203a 2022 202b  ilename is : " +
-0006ef30: 2020 6d79 666e 2029 0a20 2020 2020 2020    myfn ).       
-0006ef40: 2020 2020 2077 6172 6e69 6e67 732e 7761       warnings.wa
-0006ef50: 726e 2820 2273 6964 2069 7320 3a20 2220  rn( "sid is : " 
-0006ef60: 2b20 7369 6420 290a 2020 2020 2020 2020  + sid ).        
-0006ef70: 2020 2020 7761 726e 696e 6773 2e77 6172      warnings.war
-0006ef80: 6e28 2022 7820 6973 203a 2022 202b 2073  n( "x is : " + s
-0006ef90: 7472 2878 2920 290a 2020 2020 2020 2020  tr(x) ).        
-0006efa0: 6d79 7072 6f6a 203d 2073 7472 2864 665b  myproj = str(df[
-0006efb0: 7072 6f6a 6563 745f 636f 6c5d 2e69 6c6f  project_col].ilo
-0006efc0: 635b 785d 290a 2020 2020 2020 2020 6d79  c[x]).        my
-0006efd0: 6461 7465 203d 2073 7472 2864 665b 6461  date = str(df[da
-0006efe0: 7465 5f63 6f6c 5d2e 696c 6f63 5b78 5d29  te_col].iloc[x])
-0006eff0: 0a20 2020 2020 2020 206d 7969 6420 3d20  .        myid = 
-0006f000: 7374 7228 6466 5b69 6d61 6765 5f63 6f6c  str(df[image_col
-0006f010: 5d2e 696c 6f63 5b78 5d29 0a20 2020 2020  ].iloc[x]).     
-0006f020: 2020 2070 6174 685f 7465 6d70 6c61 7465     path_template
-0006f030: 203d 2062 6173 655f 7061 7468 202b 2022   = base_path + "
-0006f040: 2f22 202b 206d 7970 726f 6a20 2b20 2022  /" + myproj +  "
-0006f050: 2f22 202b 2073 6964 202b 2022 2f22 202b  /" + sid + "/" +
-0006f060: 206d 7964 6174 6520 2b20 272f 2720 2b20   mydate + '/' + 
-0006f070: 6869 6572 7661 7269 6162 6c65 202b 2027  hiervariable + '
-0006f080: 2f27 202b 2073 7472 286d 7969 6429 202b  /' + str(myid) +
-0006f090: 2022 2f22 0a20 2020 2020 2020 2068 6965   "/".        hie
-0006f0a0: 7266 6e20 3d20 736f 7274 6564 2867 6c6f  rfn = sorted(glo
-0006f0b0: 6228 2070 6174 685f 7465 6d70 6c61 7465  b( path_template
-0006f0c0: 202b 2022 2a22 202b 2068 6965 7276 6172   + "*" + hiervar
-0006f0d0: 6961 626c 6520 2b20 222a 7769 6465 2e63  iable + "*wide.c
-0006f0e0: 7376 2220 2920 290a 2020 2020 2020 2020  sv" ) ).        
-0006f0f0: 6966 206c 656e 2820 6869 6572 666e 2029  if len( hierfn )
-0006f100: 203e 2030 3a0a 2020 2020 2020 2020 2020   > 0:.          
-0006f110: 2020 6b65 6570 5b78 5d3d 5472 7565 0a0a    keep[x]=True..
-0006f120: 2020 2020 6466 3d64 665b 6b65 6570 5d0a      df=df[keep].
-0006f130: 0a20 2020 2069 6620 6e6f 7420 6466 2e69  .    if not df.i
-0006f140: 6e64 6578 2e69 735f 756e 6971 7565 3a0a  ndex.is_unique:.
-0006f150: 2020 2020 2020 2020 7761 726e 696e 6773          warnings
-0006f160: 2e77 6172 6e28 2264 6174 6120 6672 616d  .warn("data fram
-0006f170: 6520 646f 6573 206e 6f74 2068 6176 6520  e does not have 
-0006f180: 756e 6971 7565 2069 6e64 6963 6573 2e20  unique indices. 
-0006f190: 2077 6520 7468 6572 6566 6f72 6520 7265   we therefore re
-0006f1a0: 7365 7420 7468 6520 696e 6465 7820 746f  set the index to
-0006f1b0: 2061 6c6c 6f77 2074 6865 2066 756e 6374   allow the funct
-0006f1c0: 696f 6e20 746f 2063 6f6e 7469 6e75 6520  ion to continue 
-0006f1d0: 6f6e 2e22 2029 0a20 2020 2020 2020 2064  on." ).        d
-0006f1e0: 6620 3d20 6466 2e72 6573 6574 5f69 6e64  f = df.reset_ind
-0006f1f0: 6578 2829 0a0a 2020 2020 0a20 2020 2069  ex()..    .    i
-0006f200: 6620 7665 7262 6f73 653a 0a20 2020 2020  f verbose:.     
-0006f210: 2020 2070 7269 6e74 2820 226f 7269 6769     print( "origi
-0006f220: 6e61 6c20 696e 7075 7420 6861 6420 7368  nal input had sh
-0006f230: 6170 6520 2220 2b20 7374 7228 2064 662e  ape " + str( df.
-0006f240: 7368 6170 655b 305d 2029 202b 2022 2028  shape[0] ) + " (
-0006f250: 5431 206f 6e6c 7929 2061 6e64 2077 6520  T1 only) and we 
-0006f260: 6669 6e64 2022 202b 2073 7472 2820 286b  find " + str( (k
-0006f270: 6565 7029 2e73 756d 2829 2029 202b 2022  eep).sum() ) + "
-0006f280: 2077 6974 6820 6869 6572 6172 6368 6963   with hierarchic
-0006f290: 616c 206f 7574 7075 7420 6465 6669 6e65  al output define
-0006f2a0: 6420 6279 2076 6172 6961 626c 653a 2022  d by variable: "
-0006f2b0: 202b 2068 6965 7276 6172 6961 626c 6520   + hiervariable 
-0006f2c0: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
-0006f2d0: 2064 662e 7368 6170 6520 290a 0a20 2020   df.shape )..   
-0006f2e0: 2064 666f 7574 203d 2070 642e 4461 7461   dfout = pd.Data
-0006f2f0: 4672 616d 6528 290a 2020 2020 6d79 6374  Frame().    myct
-0006f300: 203d 2030 0a20 2020 2066 6f72 2078 2069   = 0.    for x i
-0006f310: 6e20 7261 6e67 6528 2064 662e 7368 6170  n range( df.shap
-0006f320: 655b 305d 293a 0a20 2020 2020 2020 2069  e[0]):.        i
-0006f330: 6620 7665 7262 6f73 653a 0a20 2020 2020  f verbose:.     
-0006f340: 2020 2020 2020 2070 7269 6e74 2822 5c6e         print("\n
-0006f350: 5c6e 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  \n--------------
-0006f360: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0006f370: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0006f380: 2d2d 2d22 290a 2020 2020 2020 2020 2020  ---").          
-0006f390: 2020 7072 696e 7428 6622 7b78 7d2e 2e2e    print(f"{x}...
-0006f3a0: 2229 0a20 2020 2020 2020 2065 6c73 653a  ").        else:
-0006f3b0: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
-0006f3c0: 6772 6573 735f 7265 706f 7274 6572 2878  gress_reporter(x
-0006f3d0: 2c20 6466 2e73 6861 7065 5b30 5d2c 2077  , df.shape[0], w
-0006f3e0: 6964 7468 3d35 3030 290a 2020 2020 2020  idth=500).      
-0006f3f0: 2020 6c6f 6369 6e64 203d 2064 662e 696e    locind = df.in
-0006f400: 6465 785b 785d 0a20 2020 2020 2020 206d  dex[x].        m
-0006f410: 7966 6e20 3d20 6f73 2e70 6174 682e 6261  yfn = os.path.ba
-0006f420: 7365 6e61 6d65 2820 6466 5b27 6669 6c65  sename( df['file
-0006f430: 6e61 6d65 275d 2e69 6c6f 635b 785d 2029  name'].iloc[x] )
-0006f440: 0a20 2020 2020 2020 2073 6964 203d 2073  .        sid = s
-0006f450: 7472 2820 6466 5b73 7562 6a65 6374 5f63  tr( df[subject_c
-0006f460: 6f6c 5d2e 696c 6f63 5b78 5d20 290a 2020  ol].iloc[x] ).  
-0006f470: 2020 2020 2020 7465 6d70 4220 3d20 6d79        tempB = my
-0006f480: 666e 2e73 706c 6974 2820 7370 6c69 7473  fn.split( splits
-0006f490: 6570 2029 0a20 2020 2020 2020 2073 6964  ep ).        sid
-0006f4a0: 3020 3d20 7374 7228 7465 6d70 425b 315d  0 = str(tempB[1]
-0006f4b0: 290a 2020 2020 2020 2020 6966 2073 6964  ).        if sid
-0006f4c0: 3020 213d 2073 6964 2061 6e64 2076 6572  0 != sid and ver
-0006f4d0: 626f 7365 3a0a 2020 2020 2020 2020 2020  bose:.          
-0006f4e0: 2020 7761 726e 696e 6773 2e77 6172 6e28    warnings.warn(
-0006f4f0: 2249 4e4e 4552 3a20 7468 6520 6964 2064  "INNER: the id d
-0006f500: 6572 6976 6564 2066 726f 6d20 7468 6520  erived from the 
-0006f510: 6669 6c65 6e61 6d65 2022 202b 2073 7472  filename " + str
-0006f520: 2873 6964 2920 2b20 2220 646f 6573 206e  (sid) + " does n
-0006f530: 6f74 206d 6174 6368 2074 6865 2069 6420  ot match the id 
-0006f540: 7374 6f72 6564 2069 6e20 7468 6520 6461  stored in the da
-0006f550: 7461 2066 7261 6d65 2022 202b 2073 7472  ta frame " + str
-0006f560: 2873 6964 3029 2029 0a20 2020 2020 2020  (sid0) ).       
-0006f570: 2020 2020 2077 6172 6e69 6e67 732e 7761       warnings.wa
-0006f580: 726e 2820 2266 696c 656e 616d 6520 6973  rn( "filename is
-0006f590: 203a 2022 202b 2020 7374 7228 6d79 666e   : " +  str(myfn
-0006f5a0: 2920 290a 2020 2020 2020 2020 2020 2020  ) ).            
-0006f5b0: 7761 726e 696e 6773 2e77 6172 6e28 2022  warnings.warn( "
-0006f5c0: 7369 6420 6973 203a 2022 202b 2073 7472  sid is : " + str
-0006f5d0: 2873 6964 2920 290a 2020 2020 2020 2020  (sid) ).        
-0006f5e0: 2020 2020 7761 726e 696e 6773 2e77 6172      warnings.war
-0006f5f0: 6e28 2022 7820 6973 203a 2022 202b 2073  n( "x is : " + s
-0006f600: 7472 2878 2920 290a 2020 2020 2020 2020  tr(x) ).        
-0006f610: 2020 2020 7761 726e 696e 6773 2e77 6172      warnings.war
-0006f620: 6e28 2022 696e 6465 7820 6973 203a 2022  n( "index is : "
-0006f630: 202b 2073 7472 286c 6f63 696e 6429 2029   + str(locind) )
-0006f640: 0a20 2020 2020 2020 206d 7970 726f 6a20  .        myproj 
-0006f650: 3d20 7374 7228 6466 5b70 726f 6a65 6374  = str(df[project
-0006f660: 5f63 6f6c 5d2e 696c 6f63 5b78 5d29 0a20  _col].iloc[x]). 
-0006f670: 2020 2020 2020 206d 7964 6174 6520 3d20         mydate = 
-0006f680: 7374 7228 6466 5b64 6174 655f 636f 6c5d  str(df[date_col]
-0006f690: 2e69 6c6f 635b 785d 290a 2020 2020 2020  .iloc[x]).      
-0006f6a0: 2020 6d79 6964 203d 2073 7472 2864 665b    myid = str(df[
-0006f6b0: 696d 6167 655f 636f 6c5d 2e69 6c6f 635b  image_col].iloc[
-0006f6c0: 785d 290a 2020 2020 2020 2020 6d79 7431  x]).        myt1
-0006f6d0: 6964 203d 206d 7969 640a 2020 2020 2020  id = myid.      
-0006f6e0: 2020 6966 2076 6572 626f 7365 3a0a 2020    if verbose:.  
-0006f6f0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-0006f700: 206d 7966 6e20 290a 2020 2020 2020 2020   myfn ).        
-0006f710: 2020 2020 7072 696e 7428 2074 656d 7020      print( temp 
-0006f720: 290a 2020 2020 2020 2020 2020 2020 7072  ).            pr
-0006f730: 696e 7428 2022 6964 2022 202b 2073 6964  int( "id " + sid
-0006f740: 2020 290a 2020 2020 2020 2020 7061 7468    ).        path
-0006f750: 5f74 656d 706c 6174 6520 3d20 6261 7365  _template = base
-0006f760: 5f70 6174 6820 2b20 222f 2220 2b20 6d79  _path + "/" + my
-0006f770: 7072 6f6a 202b 2020 222f 2220 2b20 7369  proj +  "/" + si
-0006f780: 6420 2b20 222f 2220 2b20 6d79 6461 7465  d + "/" + mydate
-0006f790: 202b 2027 2f27 202b 2068 6965 7276 6172   + '/' + hiervar
-0006f7a0: 6961 626c 6520 2b20 272f 2720 2b20 7374  iable + '/' + st
-0006f7b0: 7228 6d79 6964 2920 2b20 222f 220a 2020  r(myid) + "/".  
-0006f7c0: 2020 2020 2020 7365 6172 6368 6869 6572        searchhier
-0006f7d0: 203d 2070 6174 685f 7465 6d70 6c61 7465   = path_template
-0006f7e0: 202b 2022 2a22 202b 2068 6965 7276 6172   + "*" + hiervar
-0006f7f0: 6961 626c 6520 2b20 222a 7769 6465 2e63  iable + "*wide.c
-0006f800: 7376 220a 2020 2020 2020 2020 6966 2076  sv".        if v
-0006f810: 6572 626f 7365 3a0a 2020 2020 2020 2020  erbose:.        
-0006f820: 2020 2020 7072 696e 7428 2073 6561 7263      print( searc
-0006f830: 6868 6965 7220 290a 2020 2020 2020 2020  hhier ).        
-0006f840: 6869 6572 666e 203d 2073 6f72 7465 6428  hierfn = sorted(
-0006f850: 2067 6c6f 6228 2073 6561 7263 6868 6965   glob( searchhie
-0006f860: 7220 2920 290a 2020 2020 2020 2020 6966  r ) ).        if
-0006f870: 206c 656e 2820 6869 6572 666e 2029 203e   len( hierfn ) >
-0006f880: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
-0006f890: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-0006f8a0: 2822 7468 6572 6520 6172 6520 2220 2b20  ("there are " + 
-0006f8b0: 7374 7228 206c 656e 2820 6869 6572 666e  str( len( hierfn
-0006f8c0: 2029 2029 202b 2022 206e 756d 6265 7220   ) ) + " number 
-0006f8d0: 6f66 2068 6965 7220 666e 7320 7769 7468  of hier fns with
-0006f8e0: 2073 6561 7263 6820 7061 7468 2022 202b   search path " +
-0006f8f0: 2073 6561 7263 6868 6965 7220 290a 2020   searchhier ).  
-0006f900: 2020 2020 2020 6966 206c 656e 2820 6869        if len( hi
-0006f910: 6572 666e 2029 203d 3d20 313a 0a20 2020  erfn ) == 1:.   
-0006f920: 2020 2020 2020 2020 2068 6466 3d74 3164           hdf=t1d
-0006f930: 663d 6474 6466 3d72 7364 663d 7065 7266  f=dtdf=rsdf=perf
-0006f940: 6466 3d6e 6d64 663d 666c 6169 7264 663d  df=nmdf=flairdf=
-0006f950: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
-0006f960: 2069 6620 7665 7262 6f73 653a 0a20 2020   if verbose:.   
-0006f970: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-0006f980: 6e74 2868 6965 7266 6e29 0a20 2020 2020  nt(hierfn).     
-0006f990: 2020 2020 2020 2068 6466 203d 2070 642e         hdf = pd.
-0006f9a0: 7265 6164 5f63 7376 2868 6965 7266 6e5b  read_csv(hierfn[
-0006f9b0: 305d 290a 2020 2020 2020 2020 2020 2020  0]).            
-0006f9c0: 6966 2076 6572 626f 7365 3a0a 2020 2020  if verbose:.    
-0006f9d0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-0006f9e0: 7428 2068 6466 5b27 766f 6c5f 6865 6d69  t( hdf['vol_hemi
-0006f9f0: 7370 6865 7265 5f6c 6566 7468 656d 6973  sphere_lefthemis
-0006fa00: 7068 6572 6573 275d 2029 0a20 2020 2020  pheres'] ).     
-0006fa10: 2020 2020 2020 2062 6164 6e61 6d65 7320         badnames 
-0006fa20: 3d20 6765 745f 6e61 6d65 735f 6672 6f6d  = get_names_from
-0006fa30: 5f64 6174 615f 6672 616d 6528 205b 2755  _data_frame( ['U
-0006fa40: 6e6e 616d 6564 275d 2c20 6864 6620 290a  nnamed'], hdf ).
-0006fa50: 2020 2020 2020 2020 2020 2020 6864 663d              hdf=
-0006fa60: 6864 662e 6472 6f70 2862 6164 6e61 6d65  hdf.drop(badname
-0006fa70: 732c 2061 7869 733d 3129 0a20 2020 2020  s, axis=1).     
-0006fa80: 2020 2020 2020 206e 756d 7320 3d20 5b69         nums = [i
-0006fa90: 7369 6e73 7461 6e63 6528 6864 665b 636f  sinstance(hdf[co
-0006faa0: 6c5d 2e69 6c6f 635b 305d 2c20 2869 6e74  l].iloc[0], (int
-0006fab0: 2c20 666c 6f61 7429 2920 666f 7220 636f  , float)) for co
-0006fac0: 6c20 696e 2068 6466 2e63 6f6c 756d 6e73  l in hdf.columns
-0006fad0: 5d0a 2020 2020 2020 2020 2020 2020 636f  ].            co
-0006fae0: 7265 6e61 6d65 7320 3d20 6c69 7374 286e  renames = list(n
-0006faf0: 702e 6172 7261 7928 6864 662e 636f 6c75  p.array(hdf.colu
-0006fb00: 6d6e 7329 5b6e 756d 735d 290a 2020 2020  mns)[nums]).    
-0006fb10: 2020 2020 2020 2020 2320 6864 662e 6c6f          # hdf.lo
-0006fb20: 635b 3a2c 206e 756d 735d 203d 2068 6466  c[:, nums] = hdf
-0006fb30: 2e6c 6f63 5b3a 2c20 6e75 6d73 5d2e 6164  .loc[:, nums].ad
-0006fb40: 645f 7072 6566 6978 2822 5431 4869 6572  d_prefix("T1Hier
-0006fb50: 5f22 290a 2020 2020 2020 2020 2020 2020  _").            
-0006fb60: 6864 6620 3d20 6864 662e 6164 645f 7072  hdf = hdf.add_pr
-0006fb70: 6566 6978 2822 5431 4869 6572 5f22 290a  efix("T1Hier_").
-0006fb80: 2020 2020 2020 2020 2020 2020 6d79 6374              myct
-0006fb90: 203d 206d 7963 7420 2b20 310a 2020 2020   = myct + 1.    
-0006fba0: 2020 2020 2020 2020 6466 6c69 7374 203d          dflist =
-0006fbb0: 205b 6864 665d 0a0a 2020 2020 2020 2020   [hdf]..        
-0006fbc0: 2020 2020 666f 7220 6d79 6d6f 6420 696e      for mymod in
-0006fbd0: 2076 6d6f 6464 6963 742e 6b65 7973 2829   vmoddict.keys()
-0006fbe0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0006fbf0: 2020 6966 2076 6572 626f 7365 3a0a 2020    if verbose:.  
-0006fc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0006fc10: 2020 7072 696e 7428 225c 6e5c 6e2a 2a2a    print("\n\n***
-0006fc20: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-0006fc30: 2a2a 2a2a 2a2a 2022 202b 206d 796d 6f64  ****** " + mymod
-0006fc40: 202b 2022 202a 2a2a 2a2a 2a2a 2a2a 2a2a   + " ***********
-0006fc50: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2229  **************")
-0006fc60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0006fc70: 206d 6f64 616c 6974 7963 6c61 7373 203d   modalityclass =
-0006fc80: 2076 6d6f 6464 6963 745b 206d 796d 6f64   vmoddict[ mymod
-0006fc90: 205d 0a20 2020 2020 2020 2020 2020 2020   ].             
-0006fca0: 2020 2069 6620 7769 6c64 5f63 6172 645f     if wild_card_
-0006fcb0: 6d6f 6461 6c69 7479 5f69 643a 0a20 2020  modality_id:.   
-0006fcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0006fcd0: 206d 796d 6f64 6964 203d 2027 2a27 0a20   mymodid = '*'. 
-0006fce0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0006fcf0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0006fd00: 2020 2020 2020 2020 206d 796d 6f64 6964           mymodid
-0006fd10: 203d 2073 7472 2820 6466 5b6d 796d 6f64   = str( df[mymod
-0006fd20: 5d2e 696c 6f63 5b78 5d20 290a 2020 2020  ].iloc[x] ).    
-0006fd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0006fd40: 6966 206d 796d 6f64 6964 2e6c 6f77 6572  if mymodid.lower
-0006fd50: 2829 2021 3d20 226e 616e 2220 616e 6420  () != "nan" and 
-0006fd60: 6d79 6d6f 6469 642e 6c6f 7765 7228 2920  mymodid.lower() 
-0006fd70: 213d 2022 6e61 223a 0a20 2020 2020 2020  != "na":.       
-0006fd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0006fd90: 206d 796d 6f64 6964 203d 206f 732e 7061   mymodid = os.pa
-0006fda0: 7468 2e62 6173 656e 616d 6528 206d 796d  th.basename( mym
-0006fdb0: 6f64 6964 2029 0a20 2020 2020 2020 2020  odid ).         
-0006fdc0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-0006fdd0: 796d 6f64 6964 203d 206f 732e 7061 7468  ymodid = os.path
-0006fde0: 2e73 706c 6974 6578 7428 206d 796d 6f64  .splitext( mymod
-0006fdf0: 6964 2029 5b30 5d0a 2020 2020 2020 2020  id )[0].        
-0006fe00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0006fe10: 6d79 6d6f 6469 6420 3d20 6f73 2e70 6174  mymodid = os.pat
-0006fe20: 682e 7370 6c69 7465 7874 2820 6d79 6d6f  h.splitext( mymo
-0006fe30: 6469 6420 295b 305d 0a20 2020 2020 2020  did )[0].       
-0006fe40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0006fe50: 2074 656d 7020 3d20 6d79 6d6f 6469 642e   temp = mymodid.
-0006fe60: 7370 6c69 7428 2069 6473 6570 2029 0a20  split( idsep ). 
+000694c0: 6c73 6529 5d0a 0a20 2020 2073 7461 7469  lse)]..    stati
+000694d0: 7374 6963 616c 5f64 665b 2761 6e61 7427  stical_df['anat'
+000694e0: 5d20 3d20 7374 6174 6973 7469 6361 6c5f  ] = statistical_
+000694f0: 6466 5b27 616e 6174 275d 2e73 7472 2e72  df['anat'].str.r
+00069500: 6570 6c61 6365 2822 5f22 2c20 222e 222c  eplace("_", ".",
+00069510: 2072 6567 6578 3d54 7275 6529 0a0a 2020   regex=True)..  
+00069520: 2020 2320 4c6f 6164 2069 6d61 6765 2061    # Load image a
+00069530: 6e64 2070 726f 6365 7373 2069 740a 2020  nd process it.  
+00069540: 2020 6564 6765 696d 6720 3d20 616e 7473    edgeimg = ants
+00069550: 2e69 4d61 7468 2862 7261 696e 5f69 6d61  .iMath(brain_ima
+00069560: 6765 2c22 4e6f 726d 616c 697a 6522 290a  ge,"Normalize").
+00069570: 2020 2020 6966 2065 6467 655f 696d 6167      if edge_imag
+00069580: 655f 6469 6c61 7469 6f6e 203e 2030 3a0a  e_dilation > 0:.
+00069590: 2020 2020 2020 2020 6564 6765 696d 6720          edgeimg 
+000695a0: 3d20 616e 7473 2e69 4d61 7468 2820 6564  = ants.iMath( ed
+000695b0: 6765 696d 672c 2022 4d44 222c 2065 6467  geimg, "MD", edg
+000695c0: 655f 696d 6167 655f 6469 6c61 7469 6f6e  e_image_dilation
+000695d0: 290a 0a20 2020 2023 2044 6566 696e 6520  )..    # Define 
+000695e0: 6c69 7374 7320 616e 6420 6461 7461 2066  lists and data f
+000695f0: 7261 6d65 730a 2020 2020 706f 7374 6669  rames.    postfi
+00069600: 7820 3d20 5b27 6266 272c 2027 6369 7431  x = ['bf', 'cit1
+00069610: 3638 6c61 6227 2c20 276d 746c 272c 2027  68lab', 'mtl', '
+00069620: 6365 7265 6265 6c6c 756d 272c 2027 646b  cerebellum', 'dk
+00069630: 745f 636f 7274 6578 272c 2762 7261 696e  t_cortex','brain
+00069640: 7374 656d 272c 274a 4855 5f77 6d27 2c27  stem','JHU_wm','
+00069650: 7965 6f27 5d0a 2020 2020 6174 6c61 7320  yeo'].    atlas 
+00069660: 3d20 5b27 4246 272c 2027 4349 5431 3638  = ['BF', 'CIT168
+00069670: 272c 2027 4d54 4c27 2c20 2754 7573 7469  ', 'MTL', 'Tusti
+00069680: 736f 6e43 6f62 7261 272c 2027 6465 7369  sonCobra', 'desi
+00069690: 6b61 6e2d 6b69 6c6c 6961 6e79 2d74 6f75  kan-killiany-tou
+000696a0: 7276 696c 6c65 272c 2762 7261 696e 7374  rville','brainst
+000696b0: 656d 272c 274a 4855 5f77 6d27 2c27 7965  em','JHU_wm','ye
+000696c0: 6f27 5d0a 2020 2020 706f 7374 6465 7363  o'].    postdesc
+000696d0: 203d 205b 276e 626d 3343 4831 3327 2c20   = ['nbm3CH13', 
+000696e0: 2743 4954 3136 385f 5265 696e 665f 4c65  'CIT168_Reinf_Le
+000696f0: 6172 6e5f 7631 5f6c 6162 656c 5f64 6573  arn_v1_label_des
+00069700: 6372 6970 7469 6f6e 735f 7061 6427 2c20  criptions_pad', 
+00069710: 276d 746c 5f64 6573 6372 6970 7469 6f6e  'mtl_description
+00069720: 272c 2027 6365 7265 6265 6c6c 756d 272c  ', 'cerebellum',
+00069730: 2027 646b 7427 2c27 4349 5431 3638 5f54   'dkt','CIT168_T
+00069740: 3177 5f37 3030 756d 5f70 6164 5f61 646e  1w_700um_pad_adn
+00069750: 695f 6272 6169 6e73 7465 6d27 2c27 4641  i_brainstem','FA
+00069760: 5f4a 4855 5f6c 6162 656c 735f 6564 6974  _JHU_labels_edit
+00069770: 6564 272c 2770 706d 695f 7465 6d70 6c61  ed','ppmi_templa
+00069780: 7465 5f35 3030 5061 7263 656c 735f 5965  te_500Parcels_Ye
+00069790: 6f32 3031 315f 3137 4e65 7477 6f72 6b73  o2011_17Networks
+000697a0: 5f32 3032 335f 686f 6d6f 746f 7069 6327  _2023_homotopic'
+000697b0: 5d0a 2020 2020 7374 6174 6466 203d 2070  ].    statdf = p
+000697c0: 642e 4461 7461 4672 616d 6528 7b27 696d  d.DataFrame({'im
+000697d0: 6727 3a20 706f 7374 6669 782c 2027 6174  g': postfix, 'at
+000697e0: 6c61 7327 3a20 6174 6c61 732c 2027 6373  las': atlas, 'cs
+000697f0: 7664 6573 6372 6970 7427 3a20 706f 7374  vdescript': post
+00069800: 6465 7363 7d29 0a20 2020 2074 656d 706c  desc}).    templ
+00069810: 6174 6570 7265 6669 7820 3d20 277e 2f2e  ateprefix = '~/.
+00069820: 616e 7473 7079 6d6d 2f50 504d 495f 7465  antspymm/PPMI_te
+00069830: 6d70 6c61 7465 305f 270a 2020 2020 2320  mplate0_'.    # 
+00069840: 4974 6572 6174 6520 7468 726f 7567 6820  Iterate through 
+00069850: 636f 6c75 6d6e 7320 616e 6420 6372 6561  columns and crea
+00069860: 7465 2066 6967 7572 6573 0a20 2020 2063  te figures.    c
+00069870: 6f6c 3276 697a 203d 2027 7661 6c75 6573  ol2viz = 'values
+00069880: 270a 2020 2020 6966 2054 7275 653a 0a20  '.    if True:. 
+00069890: 2020 2020 2020 2061 6e61 7474 6f73 686f         anattosho
+000698a0: 7720 3d20 7a7a 5b27 616e 6174 275d 2e75  w = zz['anat'].u
+000698b0: 6e69 7175 6528 290a 2020 2020 2020 2020  nique().        
+000698c0: 6966 2076 6572 626f 7365 3a0a 2020 2020  if verbose:.    
+000698d0: 2020 2020 2020 2020 7072 696e 7428 636f          print(co
+000698e0: 6c32 7669 7a29 0a20 2020 2020 2020 2020  l2viz).         
+000698f0: 2020 2070 7269 6e74 2861 6e61 7474 6f73     print(anattos
+00069900: 686f 7729 0a20 2020 2020 2020 2023 2052  how).        # R
+00069910: 6573 7420 6f66 2079 6f75 7220 636f 6465  est of your code
+00069920: 2066 6f72 2066 6967 7572 6520 6372 6561   for figure crea
+00069930: 7469 6f6e 2067 6f65 7320 6865 7265 2e2e  tion goes here..
+00069940: 2e0a 2020 2020 2020 2020 6164 6465 6d20  ..        addem 
+00069950: 3d20 6564 6765 696d 6720 2a20 300a 2020  = edgeimg * 0.  
+00069960: 2020 2020 2020 666f 7220 6b20 696e 2072        for k in r
+00069970: 616e 6765 286c 656e 2861 6e61 7474 6f73  ange(len(anattos
+00069980: 686f 7729 293a 0a20 2020 2020 2020 2020  how)):.         
+00069990: 2020 2069 6620 7665 7262 6f73 653a 0a20     if verbose:. 
+000699a0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000699b0: 7269 6e74 2873 7472 286b 2920 2b20 2022  rint(str(k) +  "
+000699c0: 2022 202b 2061 6e61 7474 6f73 686f 775b   " + anattoshow[
+000699d0: 6b5d 2020 290a 2020 2020 2020 2020 2020  k]  ).          
+000699e0: 2020 6d79 7375 6220 3d20 7a7a 5b7a 7a5b    mysub = zz[zz[
+000699f0: 2761 6e61 7427 5d2e 7374 722e 636f 6e74  'anat'].str.cont
+00069a00: 6169 6e73 2861 6e61 7474 6f73 686f 775b  ains(anattoshow[
+00069a10: 6b5d 295d 0a20 2020 2020 2020 2020 2020  k])].           
+00069a20: 2061 6e61 7473 6561 723d 7265 2e73 7562   anatsear=re.sub
+00069a30: 2822 6474 692e 6661 222c 2222 2c61 6e61  ("dti.fa","",ana
+00069a40: 7474 6f73 686f 775b 6b5d 290a 2020 2020  ttoshow[k]).    
+00069a50: 2020 2020 2020 2020 616e 6174 7365 6172          anatsear
+00069a60: 3d72 652e 7375 6228 2274 312e 766f 6c61  =re.sub("t1.vola
+00069a70: 7379 6d22 2c22 222c 616e 6174 7365 6172  sym","",anatsear
+00069a80: 290a 2020 2020 2020 2020 2020 2020 616e  ).            an
+00069a90: 6174 7365 6172 3d72 652e 7375 6228 2274  atsear=re.sub("t
+00069aa0: 312e 7468 6b61 7379 6d22 2c22 222c 616e  1.thkasym","",an
+00069ab0: 6174 7365 6172 290a 2020 2020 2020 2020  atsear).        
+00069ac0: 2020 2020 616e 6174 7365 6172 3d72 652e      anatsear=re.
+00069ad0: 7375 6228 2274 312e 6172 6561 6173 796d  sub("t1.areaasym
+00069ae0: 222c 2222 2c61 6e61 7473 6561 7229 0a20  ","",anatsear). 
+00069af0: 2020 2020 2020 2020 2020 2061 6e61 7473             anats
+00069b00: 6561 723d 7265 2e73 7562 2822 7431 2e76  ear=re.sub("t1.v
+00069b10: 6f6c 2e22 2c22 222c 616e 6174 7365 6172  ol.","",anatsear
+00069b20: 290a 2020 2020 2020 2020 2020 2020 616e  ).            an
+00069b30: 6174 7365 6172 3d72 652e 7375 6228 2274  atsear=re.sub("t
+00069b40: 312e 7468 6b2e 222c 2222 2c61 6e61 7473  1.thk.","",anats
+00069b50: 6561 7229 0a20 2020 2020 2020 2020 2020  ear).           
+00069b60: 2061 6e61 7473 6561 723d 7265 2e73 7562   anatsear=re.sub
+00069b70: 2822 7431 2e61 7265 612e 222c 2222 2c61  ("t1.area.","",a
+00069b80: 6e61 7473 6561 7229 0a20 2020 2020 2020  natsear).       
+00069b90: 2020 2020 2061 6e61 7473 6561 723d 7265       anatsear=re
+00069ba0: 2e73 7562 2822 6173 796d 6470 2e22 2c22  .sub("asymdp.","
+00069bb0: 222c 616e 6174 7365 6172 290a 2020 2020  ",anatsear).    
+00069bc0: 2020 2020 2020 2020 616e 6174 7365 6172          anatsear
+00069bd0: 3d72 652e 7375 6228 2261 7379 6d2e 222c  =re.sub("asym.",
+00069be0: 2222 2c61 6e61 7473 6561 7229 0a20 2020  "",anatsear).   
+00069bf0: 2020 2020 2020 2020 2061 6e61 7473 6561           anatsea
+00069c00: 723d 7265 2e73 7562 2822 6474 692e 6d64  r=re.sub("dti.md
+00069c10: 2e22 2c22 222c 616e 6174 7365 6172 290a  .","",anatsear).
+00069c20: 2020 2020 2020 2020 2020 2020 616e 6174              anat
+00069c30: 7365 6172 3d72 652e 7375 6228 2264 7469  sear=re.sub("dti
+00069c40: 2e66 612e 222c 2222 2c61 6e61 7473 6561  .fa.","",anatsea
+00069c50: 7229 0a20 2020 2020 2020 2020 2020 2061  r).            a
+00069c60: 6e61 7473 6561 723d 7265 2e73 7562 2822  natsear=re.sub("
+00069c70: 6474 692e 6d64 222c 2222 2c61 6e61 7473  dti.md","",anats
+00069c80: 6561 7229 0a20 2020 2020 2020 2020 2020  ear).           
+00069c90: 2061 6e61 7473 6561 723d 7265 2e73 7562   anatsear=re.sub
+00069ca0: 2822 6474 692e 6d65 616e 2e6d 642e 222c  ("dti.mean.md.",
+00069cb0: 2222 2c61 6e61 7473 6561 7229 0a20 2020  "",anatsear).   
+00069cc0: 2020 2020 2020 2020 2061 6e61 7473 6561           anatsea
+00069cd0: 723d 7265 2e73 7562 2822 6474 692e 6d65  r=re.sub("dti.me
+00069ce0: 616e 2e66 612e 222c 2222 2c61 6e61 7473  an.fa.","",anats
+00069cf0: 6561 7229 0a20 2020 2020 2020 2020 2020  ear).           
+00069d00: 2061 6e61 7473 6561 723d 7265 2e73 7562   anatsear=re.sub
+00069d10: 2822 6c72 6176 6722 2c22 222c 616e 6174  ("lravg","",anat
+00069d20: 7365 6172 290a 2020 2020 2020 2020 2020  sear).          
+00069d30: 2020 6174 6c61 7373 6561 7263 6820 3d20    atlassearch = 
+00069d40: 6d79 6469 6374 5b27 7469 6479 6e61 6d65  mydict['tidyname
+00069d50: 7327 5d2e 7374 722e 636f 6e74 6169 6e73  s'].str.contains
+00069d60: 2861 6e61 7473 6561 7229 0a20 2020 2020  (anatsear).     
+00069d70: 2020 2020 2020 2069 6620 6174 6c61 7373         if atlass
+00069d80: 6561 7263 682e 7375 6d28 2920 3e20 303a  earch.sum() > 0:
+00069d90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00069da0: 2077 6869 6368 6174 6c61 7320 3d20 6d79   whichatlas = my
+00069db0: 6469 6374 5b61 746c 6173 7365 6172 6368  dict[atlassearch
+00069dc0: 5d5b 2741 746c 6173 275d 2e69 6c6f 635b  ]['Atlas'].iloc[
+00069dd0: 305d 0a20 2020 2020 2020 2020 2020 2020  0].             
+00069de0: 2020 206f 676c 6162 656c 6e61 6d65 203d     oglabelname =
+00069df0: 206d 7964 6963 745b 6174 6c61 7373 6561   mydict[atlassea
+00069e00: 7263 685d 5b27 4c61 6265 6c27 5d2e 696c  rch]['Label'].il
+00069e10: 6f63 5b30 5d0a 2020 2020 2020 2020 2020  oc[0].          
+00069e20: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00069e30: 2020 2020 2020 2020 7072 696e 7428 616e          print(an
+00069e40: 6174 7365 6172 290a 2020 2020 2020 2020  atsear).        
+00069e50: 2020 2020 2020 2020 6f67 6c61 6265 6c6e          oglabeln
+00069e60: 616d 653d 2775 6e6b 6e6f 776e 270a 2020  ame='unknown'.  
+00069e70: 2020 2020 2020 2020 2020 2020 2020 7768                wh
+00069e80: 6963 6861 746c 6173 3d4e 6f6e 650a 2020  ichatlas=None.  
+00069e90: 2020 2020 2020 2020 2020 6966 2076 6572            if ver
+00069ea0: 626f 7365 3a0a 2020 2020 2020 2020 2020  bose:.          
+00069eb0: 2020 2020 2020 7072 696e 7428 226f 676c        print("ogl
+00069ec0: 6162 656c 6e61 6d65 2022 202b 206f 676c  abelname " + ogl
+00069ed0: 6162 656c 6e61 6d65 2029 0a20 2020 2020  abelname ).     
+00069ee0: 2020 2020 2020 2076 616c 7332 7669 7a20         vals2viz 
+00069ef0: 3d20 6d79 7375 625b 636f 6c32 7669 7a5d  = mysub[col2viz]
+00069f00: 2e61 6767 285b 276d 696e 272c 2027 6d61  .agg(['min', 'ma
+00069f10: 7827 5d29 0a20 2020 2020 2020 2020 2020  x']).           
+00069f20: 2076 616c 7332 7669 7a20 3d20 7661 6c73   vals2viz = vals
+00069f30: 3276 697a 5b61 6273 2876 616c 7332 7669  2viz[abs(vals2vi
+00069f40: 7a29 2e69 6478 6d61 7828 295d 0a20 2020  z).idxmax()].   
+00069f50: 2020 2020 2020 2020 206d 7965 7874 203d           myext =
+00069f60: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
+00069f70: 2020 6966 2027 646b 7463 6f72 7465 7827    if 'dktcortex'
+00069f80: 2069 6e20 616e 6174 746f 7368 6f77 5b6b   in anattoshow[k
+00069f90: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
+00069fa0: 2020 206d 7965 7874 203d 2027 646b 745f     myext = 'dkt_
+00069fb0: 636f 7274 6578 270a 2020 2020 2020 2020  cortex'.        
+00069fc0: 2020 2020 656c 6966 2027 6369 7431 3638      elif 'cit168
+00069fd0: 2720 696e 2061 6e61 7474 6f73 686f 775b  ' in anattoshow[
+00069fe0: 6b5d 3a0a 2020 2020 2020 2020 2020 2020  k]:.            
+00069ff0: 2020 2020 6d79 6578 7420 3d20 2763 6974      myext = 'cit
+0006a000: 3136 386c 6162 270a 2020 2020 2020 2020  168lab'.        
+0006a010: 2020 2020 656c 6966 2027 6d74 6c27 2069      elif 'mtl' i
+0006a020: 6e20 616e 6174 746f 7368 6f77 5b6b 5d3a  n anattoshow[k]:
+0006a030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0006a040: 206d 7965 7874 203d 2027 6d74 6c27 0a20   myext = 'mtl'. 
+0006a050: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+0006a060: 676c 6162 656c 6e61 6d65 3d72 652e 7375  glabelname=re.su
+0006a070: 6228 276d 746c 272c 2027 272c 616e 6174  b('mtl', '',anat
+0006a080: 7365 6172 290a 2020 2020 2020 2020 2020  sear).          
+0006a090: 2020 656c 6966 2027 6365 7265 6265 6c6c    elif 'cerebell
+0006a0a0: 756d 2720 696e 2061 6e61 7474 6f73 686f  um' in anattosho
+0006a0b0: 775b 6b5d 3a0a 2020 2020 2020 2020 2020  w[k]:.          
+0006a0c0: 2020 2020 2020 6d79 6578 7420 3d20 2763        myext = 'c
+0006a0d0: 6572 6562 656c 6c75 6d27 0a20 2020 2020  erebellum'.     
+0006a0e0: 2020 2020 2020 2020 2020 206f 676c 6162             oglab
+0006a0f0: 656c 6e61 6d65 3d72 652e 7375 6228 2763  elname=re.sub('c
+0006a100: 6572 6562 656c 6c75 6d27 2c20 2727 2c61  erebellum', '',a
+0006a110: 6e61 7473 6561 7229 0a20 2020 2020 2020  natsear).       
+0006a120: 2020 2020 2020 2020 2023 206f 676c 6162           # oglab
+0006a130: 656c 6e61 6d65 3d6f 676c 6162 656c 6e61  elname=oglabelna
+0006a140: 6d65 5b32 3a5d 0a20 2020 2020 2020 2020  me[2:].         
+0006a150: 2020 2065 6c69 6620 2762 7261 696e 7374     elif 'brainst
+0006a160: 656d 2720 696e 2061 6e61 7474 6f73 686f  em' in anattosho
+0006a170: 775b 6b5d 3a0a 2020 2020 2020 2020 2020  w[k]:.          
+0006a180: 2020 2020 2020 6d79 6578 7420 3d20 2762        myext = 'b
+0006a190: 7261 696e 7374 656d 270a 2020 2020 2020  rainstem'.      
+0006a1a0: 2020 2020 2020 656c 6966 2061 6e79 2869        elif any(i
+0006a1b0: 7465 6d20 696e 2061 6e61 7474 6f73 686f  tem in anattosho
+0006a1c0: 775b 6b5d 2066 6f72 2069 7465 6d20 696e  w[k] for item in
+0006a1d0: 205b 276e 626d 272c 2027 6266 275d 293a   ['nbm', 'bf']):
+0006a1e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0006a1f0: 206d 7965 7874 203d 2027 6266 270a 2020   myext = 'bf'.  
+0006a200: 2020 2020 2020 2020 2020 2020 2020 6f67                og
+0006a210: 6c61 6265 6c6e 616d 653d 7265 2e73 7562  labelname=re.sub
+0006a220: 2872 275c 2e27 2c20 275f 272c 616e 6174  (r'\.', '_',anat
+0006a230: 7365 6172 290a 2020 2020 2020 2020 2020  sear).          
+0006a240: 2020 656c 6966 2077 6869 6368 6174 6c61    elif whichatla
+0006a250: 7320 3d3d 2027 6a6f 686e 7320 686f 706b  s == 'johns hopk
+0006a260: 696e 7320 7768 6974 6520 6d61 7474 6572  ins white matter
+0006a270: 273a 0a20 2020 2020 2020 2020 2020 2020  ':.             
+0006a280: 2020 206d 7965 7874 203d 2027 4a48 555f     myext = 'JHU_
+0006a290: 776d 270a 2020 2020 2020 2020 2020 2020  wm'.            
+0006a2a0: 656c 6966 2077 6869 6368 6174 6c61 7320  elif whichatlas 
+0006a2b0: 3d3d 2027 6465 7369 6b61 6e2d 6b69 6c6c  == 'desikan-kill
+0006a2c0: 6961 6e79 2d74 6f75 7276 696c 6c65 273a  iany-tourville':
+0006a2d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0006a2e0: 206d 7965 7874 203d 2027 646b 745f 636f   myext = 'dkt_co
+0006a2f0: 7274 6578 270a 2020 2020 2020 2020 2020  rtex'.          
+0006a300: 2020 656c 6966 2077 6869 6368 6174 6c61    elif whichatla
+0006a310: 7320 3d3d 2027 4349 5431 3638 273a 0a20  s == 'CIT168':. 
+0006a320: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+0006a330: 7965 7874 203d 2027 6369 7431 3638 6c61  yext = 'cit168la
+0006a340: 6227 0a20 2020 2020 2020 2020 2020 2065  b'.            e
+0006a350: 6c69 6620 7768 6963 6861 746c 6173 203d  lif whichatlas =
+0006a360: 3d20 2742 4627 3a0a 2020 2020 2020 2020  = 'BF':.        
+0006a370: 2020 2020 2020 2020 6d79 6578 7420 3d20          myext = 
+0006a380: 2762 6627 0a20 2020 2020 2020 2020 2020  'bf'.           
+0006a390: 2020 2020 206f 676c 6162 656c 6e61 6d65       oglabelname
+0006a3a0: 3d72 652e 7375 6228 2762 6627 2c20 2727  =re.sub('bf', ''
+0006a3b0: 2c6f 676c 6162 656c 6e61 6d65 290a 2020  ,oglabelname).  
+0006a3c0: 2020 2020 2020 2020 2020 656c 6966 2077            elif w
+0006a3d0: 6869 6368 6174 6c61 7320 3d3d 2027 7965  hichatlas == 'ye
+0006a3e0: 6f5f 686f 6d6f 746f 7069 6327 3a0a 2020  o_homotopic':.  
+0006a3f0: 2020 2020 2020 2020 2020 2020 2020 6d79                my
+0006a400: 6578 7420 3d20 2779 656f 270a 2020 2020  ext = 'yeo'.    
+0006a410: 2020 2020 2020 2020 6966 206d 7965 7874          if myext
+0006a420: 2069 7320 4e6f 6e65 2061 6e64 2076 6572   is None and ver
+0006a430: 626f 7365 3a0a 2020 2020 2020 2020 2020  bose:.          
+0006a440: 2020 2020 2020 6966 2077 6869 6368 6174        if whichat
+0006a450: 6c61 7320 6973 204e 6f6e 653a 0a20 2020  las is None:.   
+0006a460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0006a470: 2077 6869 6368 6174 6c61 733d 274e 6f6e   whichatlas='Non
+0006a480: 6527 0a20 2020 2020 2020 2020 2020 2020  e'.             
+0006a490: 2020 2069 6620 616e 6174 746f 7368 6f77     if anattoshow
+0006a4a0: 5b6b 5d20 6973 204e 6f6e 653a 0a20 2020  [k] is None:.   
+0006a4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0006a4c0: 2061 6e61 7474 6f73 686f 775b 6b5d 3d27   anattoshow[k]='
+0006a4d0: 4e6f 6e65 270a 2020 2020 2020 2020 2020  None'.          
+0006a4e0: 2020 2020 2020 7072 696e 7428 2022 4d59        print( "MY
+0006a4f0: 4558 5420 2220 2b20 616e 6174 746f 7368  EXT " + anattosh
+0006a500: 6f77 5b6b 5d20 2b20 2720 756e 666f 756e  ow[k] + ' unfoun
+0006a510: 6420 2720 2b20 7768 6963 6861 746c 6173  d ' + whichatlas
+0006a520: 2029 0a20 2020 2020 2020 2020 2020 2065   ).            e
+0006a530: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0006a540: 2020 2020 2069 6620 7665 7262 6f73 653a       if verbose:
+0006a550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0006a560: 2020 2020 2070 7269 6e74 2820 224d 5945       print( "MYE
+0006a570: 5854 2022 202b 206d 7965 7874 2029 0a0a  XT " + myext )..
+0006a580: 2020 2020 2020 2020 2020 2020 6966 206d              if m
+0006a590: 7965 7874 203d 3d20 2763 6974 3136 386c  yext == 'cit168l
+0006a5a0: 6162 273a 0a20 2020 2020 2020 2020 2020  ab':.           
+0006a5b0: 2020 2020 206f 676c 6162 656c 6e61 6d65       oglabelname
+0006a5c0: 3d72 652e 7375 6228 2263 6974 3136 3822  =re.sub("cit168"
+0006a5d0: 2c22 222c 6f67 6c61 6265 6c6e 616d 6529  ,"",oglabelname)
+0006a5e0: 0a20 2020 2020 2020 2020 2020 200a 2020  .            .  
+0006a5f0: 2020 2020 2020 2020 2020 666f 7220 6a20            for j 
+0006a600: 696e 2070 6f73 7466 6978 3a0a 2020 2020  in postfix:.    
+0006a610: 2020 2020 2020 2020 2020 2020 6966 206a              if j
+0006a620: 203d 3d20 2264 6b74 5f63 6f72 7465 7822   == "dkt_cortex"
+0006a630: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0006a640: 2020 2020 2020 6a20 3d20 2764 6b74 636f        j = 'dktco
+0006a650: 7274 6578 270a 2020 2020 2020 2020 2020  rtex'.          
+0006a660: 2020 2020 2020 6966 206a 203d 3d20 2264        if j == "d
+0006a670: 6565 705f 6369 7431 3638 6c61 6222 3a0a  eep_cit168lab":.
+0006a680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0006a690: 2020 2020 6a20 3d20 2764 6565 705f 6369      j = 'deep_ci
+0006a6a0: 7431 3638 270a 2020 2020 2020 2020 2020  t168'.          
+0006a6b0: 2020 2020 2020 616e 6174 746f 7368 6f77        anattoshow
+0006a6c0: 5b6b 5d20 3d20 616e 6174 746f 7368 6f77  [k] = anattoshow
+0006a6d0: 5b6b 5d2e 7265 706c 6163 6528 6a2c 2022  [k].replace(j, "
+0006a6e0: 2229 0a20 2020 2020 2020 2020 2020 2069  ").            i
+0006a6f0: 6620 7665 7262 6f73 653a 0a20 2020 2020  f verbose:.     
+0006a700: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+0006a710: 2820 616e 6174 746f 7368 6f77 5b6b 5d20  ( anattoshow[k] 
+0006a720: 2b20 2220 2220 2b20 7374 7228 2076 616c  + " " + str( val
+0006a730: 7332 7669 7a20 2920 290a 2020 2020 2020  s2viz ) ).      
+0006a740: 2020 2020 2020 6d79 6174 6c61 7320 3d20        myatlas = 
+0006a750: 6174 6c61 735b 706f 7374 6669 782e 696e  atlas[postfix.in
+0006a760: 6465 7828 6d79 6578 7429 5d0a 2020 2020  dex(myext)].    
+0006a770: 2020 2020 2020 2020 636f 7272 6563 7464          correctd
+0006a780: 6573 6372 6970 7420 3d20 706f 7374 6465  escript = postde
+0006a790: 7363 5b70 6f73 7466 6978 2e69 6e64 6578  sc[postfix.index
+0006a7a0: 286d 7965 7874 295d 0a20 2020 2020 2020  (myext)].       
+0006a7b0: 2020 2020 206c 6f63 6669 6c65 6e61 6d65       locfilename
+0006a7c0: 203d 2020 7465 6d70 6c61 7465 7072 6566   =  templatepref
+0006a7d0: 6978 202b 206d 7965 7874 202b 2027 2e6e  ix + myext + '.n
+0006a7e0: 6969 2e67 7a27 0a20 2020 2020 2020 2020  ii.gz'.         
+0006a7f0: 2020 2069 6620 7665 7262 6f73 653a 0a20     if verbose:. 
+0006a800: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0006a810: 7269 6e74 2820 6c6f 6366 696c 656e 616d  rint( locfilenam
+0006a820: 6520 290a 2020 2020 2020 2020 2020 2020  e ).            
+0006a830: 6966 206d 7965 7874 203d 3d20 2779 656f  if myext == 'yeo
+0006a840: 273a 0a20 2020 2020 2020 2020 2020 2020  ':.             
+0006a850: 2020 206f 676c 6162 656c 6e61 6d65 3d6f     oglabelname=o
+0006a860: 676c 6162 656c 6e61 6d65 2e6c 6f77 6572  glabelname.lower
+0006a870: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+0006a880: 2020 206f 676c 6162 656c 6e61 6d65 3d72     oglabelname=r
+0006a890: 652e 7375 6228 2272 7366 6d72 695f 6663  e.sub("rsfmri_fc
+0006a8a0: 6e78 7072 6f31 3232 5f22 2c22 222c 6f67  nxpro122_","",og
+0006a8b0: 6c61 6265 6c6e 616d 6529 0a20 2020 2020  labelname).     
+0006a8c0: 2020 2020 2020 2020 2020 206f 676c 6162             oglab
+0006a8d0: 656c 6e61 6d65 3d72 652e 7375 6228 2272  elname=re.sub("r
+0006a8e0: 7366 6d72 695f 6663 6e78 7072 6f31 3239  sfmri_fcnxpro129
+0006a8f0: 5f22 2c22 222c 6f67 6c61 6265 6c6e 616d  _","",oglabelnam
+0006a900: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+0006a910: 2020 206f 676c 6162 656c 6e61 6d65 3d72     oglabelname=r
+0006a920: 652e 7375 6228 2272 7366 6d72 695f 6663  e.sub("rsfmri_fc
+0006a930: 6e78 7072 6f31 3334 5f22 2c22 222c 6f67  nxpro134_","",og
+0006a940: 6c61 6265 6c6e 616d 6529 0a20 2020 2020  labelname).     
+0006a950: 2020 2020 2020 2020 2020 206c 6f63 6669             locfi
+0006a960: 6c65 6e61 6d65 203d 2022 7e2f 2e61 6e74  lename = "~/.ant
+0006a970: 7370 796d 6d2f 7070 6d69 5f74 656d 706c  spymm/ppmi_templ
+0006a980: 6174 655f 3530 3050 6172 6365 6c73 5f59  ate_500Parcels_Y
+0006a990: 656f 3230 3131 5f31 374e 6574 776f 726b  eo2011_17Network
+0006a9a0: 735f 3230 3233 5f68 6f6d 6f74 6f70 6963  s_2023_homotopic
+0006a9b0: 2e6e 6969 2e67 7a22 0a20 2020 2020 2020  .nii.gz".       
+0006a9c0: 2020 2020 2020 2020 2061 746c 6173 4465           atlasDe
+0006a9d0: 7363 7269 7074 203d 2070 642e 7265 6164  script = pd.read
+0006a9e0: 5f63 7376 2866 227e 2f2e 616e 7473 7079  _csv(f"~/.antspy
+0006a9f0: 6d6d 2f7b 636f 7272 6563 7464 6573 6372  mm/{correctdescr
+0006aa00: 6970 747d 2e63 7376 2229 0a20 2020 2020  ipt}.csv").     
+0006aa10: 2020 2020 2020 2020 2020 2061 746c 6173             atlas
+0006aa20: 4465 7363 7269 7074 2e72 656e 616d 6528  Descript.rename(
+0006aa30: 636f 6c75 6d6e 733d 7b27 5379 7374 656d  columns={'System
+0006aa40: 4e61 6d65 273a 2027 4465 7363 7269 7074  Name': 'Descript
+0006aa50: 696f 6e27 7d2c 2069 6e70 6c61 6365 3d54  ion'}, inplace=T
+0006aa60: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
+0006aa70: 2020 2020 2061 746c 6173 4465 7363 7269       atlasDescri
+0006aa80: 7074 2e72 656e 616d 6528 636f 6c75 6d6e  pt.rename(column
+0006aa90: 733d 7b27 524f 4927 3a20 274c 6162 656c  s={'ROI': 'Label
+0006aaa0: 277d 2c20 696e 706c 6163 653d 5472 7565  '}, inplace=True
+0006aab0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0006aac0: 2020 6174 6c61 7344 6573 6372 6970 745b    atlasDescript[
+0006aad0: 2744 6573 6372 6970 7469 6f6e 275d 203d  'Description'] =
+0006aae0: 2061 746c 6173 4465 7363 7269 7074 5b27   atlasDescript['
+0006aaf0: 4465 7363 7269 7074 696f 6e27 5d2e 7374  Description'].st
+0006ab00: 722e 6c6f 7765 7228 290a 2020 2020 2020  r.lower().      
+0006ab10: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0006ab20: 2020 2020 2020 2020 2020 2020 6174 6c61              atla
+0006ab30: 7344 6573 6372 6970 7420 3d20 7064 2e72  sDescript = pd.r
+0006ab40: 6561 645f 6373 7628 6622 7e2f 2e61 6e74  ead_csv(f"~/.ant
+0006ab50: 7370 7974 3177 2f7b 636f 7272 6563 7464  spyt1w/{correctd
+0006ab60: 6573 6372 6970 747d 2e63 7376 2229 0a20  escript}.csv"). 
+0006ab70: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+0006ab80: 746c 6173 4465 7363 7269 7074 5b27 4465  tlasDescript['De
+0006ab90: 7363 7269 7074 696f 6e27 5d20 3d20 6174  scription'] = at
+0006aba0: 6c61 7344 6573 6372 6970 745b 2744 6573  lasDescript['Des
+0006abb0: 6372 6970 7469 6f6e 275d 2e73 7472 2e6c  cription'].str.l
+0006abc0: 6f77 6572 2829 0a20 2020 2020 2020 2020  ower().         
+0006abd0: 2020 2020 2020 2061 746c 6173 4465 7363         atlasDesc
+0006abe0: 7269 7074 5b27 4465 7363 7269 7074 696f  ript['Descriptio
+0006abf0: 6e27 5d20 3d20 6174 6c61 7344 6573 6372  n'] = atlasDescr
+0006ac00: 6970 745b 2744 6573 6372 6970 7469 6f6e  ipt['Description
+0006ac10: 275d 2e73 7472 2e72 6570 6c61 6365 2822  '].str.replace("
+0006ac20: 2022 2c20 225f 2229 0a20 2020 2020 2020   ", "_").       
+0006ac30: 2020 2020 2020 2020 2061 746c 6173 4465           atlasDe
+0006ac40: 7363 7269 7074 5b27 4465 7363 7269 7074  script['Descript
+0006ac50: 696f 6e27 5d20 3d20 6174 6c61 7344 6573  ion'] = atlasDes
+0006ac60: 6372 6970 745b 2744 6573 6372 6970 7469  cript['Descripti
+0006ac70: 6f6e 275d 2e73 7472 2e72 6570 6c61 6365  on'].str.replace
+0006ac80: 2822 5f6c 6566 745f 222c 2022 5f22 290a  ("_left_", "_").
+0006ac90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0006aca0: 6174 6c61 7344 6573 6372 6970 745b 2744  atlasDescript['D
+0006acb0: 6573 6372 6970 7469 6f6e 275d 203d 2061  escription'] = a
+0006acc0: 746c 6173 4465 7363 7269 7074 5b27 4465  tlasDescript['De
+0006acd0: 7363 7269 7074 696f 6e27 5d2e 7374 722e  scription'].str.
+0006ace0: 7265 706c 6163 6528 225f 7269 6768 745f  replace("_right_
+0006acf0: 222c 2022 5f22 290a 2020 2020 2020 2020  ", "_").        
+0006ad00: 2020 2020 2020 2020 6174 6c61 7344 6573          atlasDes
+0006ad10: 6372 6970 745b 2744 6573 6372 6970 7469  cript['Descripti
+0006ad20: 6f6e 275d 203d 2061 746c 6173 4465 7363  on'] = atlasDesc
+0006ad30: 7269 7074 5b27 4465 7363 7269 7074 696f  ript['Descriptio
+0006ad40: 6e27 5d2e 7374 722e 7265 706c 6163 6528  n'].str.replace(
+0006ad50: 225f 6c65 6674 222c 2022 2229 0a20 2020  "_left", "").   
+0006ad60: 2020 2020 2020 2020 2020 2020 2061 746c               atl
+0006ad70: 6173 4465 7363 7269 7074 5b27 4465 7363  asDescript['Desc
+0006ad80: 7269 7074 696f 6e27 5d20 3d20 6174 6c61  ription'] = atla
+0006ad90: 7344 6573 6372 6970 745b 2744 6573 6372  sDescript['Descr
+0006ada0: 6970 7469 6f6e 275d 2e73 7472 2e72 6570  iption'].str.rep
+0006adb0: 6c61 6365 2822 5f72 6967 6874 222c 2022  lace("_right", "
+0006adc0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+0006add0: 2020 2061 746c 6173 4465 7363 7269 7074     atlasDescript
+0006ade0: 5b27 4465 7363 7269 7074 696f 6e27 5d20  ['Description'] 
+0006adf0: 3d20 6174 6c61 7344 6573 6372 6970 745b  = atlasDescript[
+0006ae00: 2744 6573 6372 6970 7469 6f6e 275d 2e73  'Description'].s
+0006ae10: 7472 2e72 6570 6c61 6365 2822 6c65 6674  tr.replace("left
+0006ae20: 5f22 2c20 2222 290a 2020 2020 2020 2020  _", "").        
+0006ae30: 2020 2020 2020 2020 6174 6c61 7344 6573          atlasDes
+0006ae40: 6372 6970 745b 2744 6573 6372 6970 7469  cript['Descripti
+0006ae50: 6f6e 275d 203d 2061 746c 6173 4465 7363  on'] = atlasDesc
+0006ae60: 7269 7074 5b27 4465 7363 7269 7074 696f  ript['Descriptio
+0006ae70: 6e27 5d2e 7374 722e 7265 706c 6163 6528  n'].str.replace(
+0006ae80: 2272 6967 6874 5f22 2c20 2222 290a 2020  "right_", "").  
+0006ae90: 2020 2020 2020 2020 2020 2020 2020 6174                at
+0006aea0: 6c61 7344 6573 6372 6970 745b 2744 6573  lasDescript['Des
+0006aeb0: 6372 6970 7469 6f6e 275d 203d 2061 746c  cription'] = atl
+0006aec0: 6173 4465 7363 7269 7074 5b27 4465 7363  asDescript['Desc
+0006aed0: 7269 7074 696f 6e27 5d2e 7374 722e 7265  ription'].str.re
+0006aee0: 706c 6163 6528 222f 222c 222e 2229 0a20  place("/","."). 
+0006aef0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0006af00: 6620 6d79 6578 7420 3d3d 2027 4a48 555f  f myext == 'JHU_
+0006af10: 776d 273a 0a20 2020 2020 2020 2020 2020  wm':.           
+0006af20: 2020 2020 2020 2020 2061 746c 6173 4465           atlasDe
+0006af30: 7363 7269 7074 5b27 4465 7363 7269 7074  script['Descript
+0006af40: 696f 6e27 5d20 3d20 6174 6c61 7344 6573  ion'] = atlasDes
+0006af50: 6372 6970 745b 2744 6573 6372 6970 7469  cript['Descripti
+0006af60: 6f6e 275d 2e73 7472 2e72 6570 6c61 6365  on'].str.replace
+0006af70: 2822 6661 2d22 2c20 2222 290a 2020 2020  ("fa-", "").    
+0006af80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0006af90: 6174 6c61 7344 6573 6372 6970 745b 2744  atlasDescript['D
+0006afa0: 6573 6372 6970 7469 6f6e 275d 203d 2061  escription'] = a
+0006afb0: 746c 6173 4465 7363 7269 7074 5b27 4465  tlasDescript['De
+0006afc0: 7363 7269 7074 696f 6e27 5d2e 7374 722e  scription'].str.
+0006afd0: 7265 706c 6163 6528 222d 6c65 6674 2d22  replace("-left-"
+0006afe0: 2c20 2222 290a 2020 2020 2020 2020 2020  , "").          
+0006aff0: 2020 2020 2020 2020 2020 6174 6c61 7344            atlasD
+0006b000: 6573 6372 6970 745b 2744 6573 6372 6970  escript['Descrip
+0006b010: 7469 6f6e 275d 203d 2061 746c 6173 4465  tion'] = atlasDe
+0006b020: 7363 7269 7074 5b27 4465 7363 7269 7074  script['Descript
+0006b030: 696f 6e27 5d2e 7374 722e 7265 706c 6163  ion'].str.replac
+0006b040: 6528 222d 7269 6768 742d 222c 2022 2229  e("-right-", "")
+0006b050: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0006b060: 2069 6620 6d79 6578 7420 3d3d 2027 6365   if myext == 'ce
+0006b070: 7265 6265 6c6c 756d 273a 0a20 2020 2020  rebellum':.     
+0006b080: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+0006b090: 746c 6173 4465 7363 7269 7074 5b27 4465  tlasDescript['De
+0006b0a0: 7363 7269 7074 696f 6e27 5d20 3d20 6174  scription'] = at
+0006b0b0: 6c61 7344 6573 6372 6970 745b 2744 6573  lasDescript['Des
+0006b0c0: 6372 6970 7469 6f6e 275d 2e73 7472 2e72  cription'].str.r
+0006b0d0: 6570 6c61 6365 2822 6c5f 222c 2022 2229  eplace("l_", "")
+0006b0e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0006b0f0: 2020 2020 2061 746c 6173 4465 7363 7269       atlasDescri
+0006b100: 7074 5b27 4465 7363 7269 7074 696f 6e27  pt['Description'
+0006b110: 5d20 3d20 6174 6c61 7344 6573 6372 6970  ] = atlasDescrip
+0006b120: 745b 2744 6573 6372 6970 7469 6f6e 275d  t['Description']
+0006b130: 2e73 7472 2e72 6570 6c61 6365 2822 725f  .str.replace("r_
+0006b140: 222c 2022 2229 0a0a 2020 2020 2020 2020  ", "")..        
+0006b150: 2020 2020 6966 2076 6572 626f 7365 3a0a      if verbose:.
+0006b160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0006b170: 7072 696e 7428 2061 746c 6173 4465 7363  print( atlasDesc
+0006b180: 7269 7074 2029 0a20 2020 2020 2020 2020  ript ).         
+0006b190: 2020 206f 676c 6162 656c 6e61 6d65 203d     oglabelname =
+0006b1a0: 206f 676c 6162 656c 6e61 6d65 2e6c 6f77   oglabelname.low
+0006b1b0: 6572 2829 0a20 2020 2020 2020 2020 2020  er().           
+0006b1c0: 206f 676c 6162 656c 6e61 6d65 203d 2072   oglabelname = r
+0006b1d0: 652e 7375 6228 2220 222c 2022 5f22 2c6f  e.sub(" ", "_",o
+0006b1e0: 676c 6162 656c 6e61 6d65 290a 2020 2020  glabelname).    
+0006b1f0: 2020 2020 2020 2020 6f67 6c61 6265 6c6e          oglabeln
+0006b200: 616d 6520 3d20 7265 2e73 7562 2822 5f6c  ame = re.sub("_l
+0006b210: 6566 745f 222c 2022 5f22 2c6f 676c 6162  eft_", "_",oglab
+0006b220: 656c 6e61 6d65 290a 2020 2020 2020 2020  elname).        
+0006b230: 2020 2020 6f67 6c61 6265 6c6e 616d 6520      oglabelname 
+0006b240: 3d20 7265 2e73 7562 2822 5f72 6967 6874  = re.sub("_right
+0006b250: 5f22 2c20 225f 222c 6f67 6c61 6265 6c6e  _", "_",oglabeln
+0006b260: 616d 6529 0a20 2020 2020 2020 2020 2020  ame).           
+0006b270: 206f 676c 6162 656c 6e61 6d65 203d 2072   oglabelname = r
+0006b280: 652e 7375 6228 225f 6c65 6674 222c 2022  e.sub("_left", "
+0006b290: 222c 6f67 6c61 6265 6c6e 616d 6529 0a20  ",oglabelname). 
+0006b2a0: 2020 2020 2020 2020 2020 206f 676c 6162             oglab
+0006b2b0: 656c 6e61 6d65 203d 2072 652e 7375 6228  elname = re.sub(
+0006b2c0: 225f 7269 6768 7422 2c20 2222 2c6f 676c  "_right", "",ogl
+0006b2d0: 6162 656c 6e61 6d65 290a 2020 2020 2020  abelname).      
+0006b2e0: 2020 2020 2020 6f67 6c61 6265 6c6e 616d        oglabelnam
+0006b2f0: 6520 3d20 7265 2e73 7562 2822 7431 6869  e = re.sub("t1hi
+0006b300: 6572 5f76 6f6c 5f22 2c20 2222 2c6f 676c  er_vol_", "",ogl
+0006b310: 6162 656c 6e61 6d65 290a 2020 2020 2020  abelname).      
+0006b320: 2020 2020 2020 6f67 6c61 6265 6c6e 616d        oglabelnam
+0006b330: 6520 3d20 7265 2e73 7562 2822 7431 6869  e = re.sub("t1hi
+0006b340: 6572 5f61 7265 615f 222c 2022 222c 6f67  er_area_", "",og
+0006b350: 6c61 6265 6c6e 616d 6529 0a20 2020 2020  labelname).     
+0006b360: 2020 2020 2020 206f 676c 6162 656c 6e61         oglabelna
+0006b370: 6d65 203d 2072 652e 7375 6228 2274 3168  me = re.sub("t1h
+0006b380: 6965 725f 7468 6b5f 222c 2022 222c 6f67  ier_thk_", "",og
+0006b390: 6c61 6265 6c6e 616d 6529 0a20 2020 2020  labelname).     
+0006b3a0: 2020 2020 2020 206f 676c 6162 656c 6e61         oglabelna
+0006b3b0: 6d65 203d 2072 652e 7375 6228 2264 6b74  me = re.sub("dkt
+0006b3c0: 7265 6769 6f6e 7322 2c20 2222 2c6f 676c  regions", "",ogl
+0006b3d0: 6162 656c 6e61 6d65 290a 2020 2020 2020  abelname).      
+0006b3e0: 2020 2020 2020 6f67 6c61 6265 6c6e 616d        oglabelnam
+0006b3f0: 6520 3d20 7265 2e73 7562 2822 646b 7463  e = re.sub("dktc
+0006b400: 6f72 7465 7822 2c20 2222 2c6f 676c 6162  ortex", "",oglab
+0006b410: 656c 6e61 6d65 290a 2020 2020 2020 2020  elname).        
+0006b420: 2020 2020 6966 206d 7965 7874 203d 3d20      if myext == 
+0006b430: 274a 4855 5f77 6d27 3a0a 2020 2020 2020  'JHU_wm':.      
+0006b440: 2020 2020 2020 2020 2020 6f67 6c61 6265            oglabe
+0006b450: 6c6e 616d 6520 3d20 7265 2e73 7562 2822  lname = re.sub("
+0006b460: 6474 695f 6d65 616e 5f66 612e 222c 2022  dti_mean_fa.", "
+0006b470: 222c 6f67 6c61 6265 6c6e 616d 6529 0a20  ",oglabelname). 
+0006b480: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+0006b490: 676c 6162 656c 6e61 6d65 203d 2072 652e  glabelname = re.
+0006b4a0: 7375 6228 2264 7469 5f6d 6561 6e5f 6d64  sub("dti_mean_md
+0006b4b0: 2e22 2c20 2222 2c6f 676c 6162 656c 6e61  .", "",oglabelna
+0006b4c0: 6d65 290a 2020 2020 2020 2020 2020 2020  me).            
+0006b4d0: 2020 2020 6f67 6c61 6265 6c6e 616d 6520      oglabelname 
+0006b4e0: 3d20 7265 2e73 7562 2822 2e6c 6566 742e  = re.sub(".left.
+0006b4f0: 222c 2022 222c 6f67 6c61 6265 6c6e 616d  ", "",oglabelnam
+0006b500: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+0006b510: 2020 206f 676c 6162 656c 6e61 6d65 203d     oglabelname =
+0006b520: 2072 652e 7375 6228 222e 7269 6768 742e   re.sub(".right.
+0006b530: 222c 2022 222c 6f67 6c61 6265 6c6e 616d  ", "",oglabelnam
+0006b540: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+0006b550: 2020 206f 676c 6162 656c 6e61 6d65 203d     oglabelname =
+0006b560: 2072 652e 7375 6228 222e 6c72 6176 672e   re.sub(".lravg.
+0006b570: 222c 2022 222c 6f67 6c61 6265 6c6e 616d  ", "",oglabelnam
+0006b580: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+0006b590: 2020 206f 676c 6162 656c 6e61 6d65 203d     oglabelname =
+0006b5a0: 2072 652e 7375 6228 222e 6173 796d 2e22   re.sub(".asym."
+0006b5b0: 2c20 2222 2c6f 676c 6162 656c 6e61 6d65  , "",oglabelname
+0006b5c0: 290a 0a20 2020 2020 2020 2020 2020 2069  )..            i
+0006b5d0: 6620 7665 7262 6f73 653a 0a20 2020 2020  f verbose:.     
+0006b5e0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+0006b5f0: 2822 6f67 6c61 6265 6c6e 616d 6520 2220  ("oglabelname " 
+0006b600: 2b20 6f67 6c61 6265 6c6e 616d 6520 290a  + oglabelname ).
+0006b610: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0006b620: 6d79 6578 7420 3d3d 2027 6365 7265 6265  myext == 'cerebe
+0006b630: 6c6c 756d 273a 0a20 2020 2020 2020 2020  llum':.         
+0006b640: 2020 2020 2020 2061 746c 6173 4465 7363         atlasDesc
+0006b650: 7269 7074 5b27 4465 7363 7269 7074 696f  ript['Descriptio
+0006b660: 6e27 5d20 3d20 6174 6c61 7344 6573 6372  n'] = atlasDescr
+0006b670: 6970 745b 2744 6573 6372 6970 7469 6f6e  ipt['Description
+0006b680: 275d 2e73 7472 2e72 6570 6c61 6365 2822  '].str.replace("
+0006b690: 6c5f 222c 2022 2229 0a20 2020 2020 2020  l_", "").       
+0006b6a0: 2020 2020 2020 2020 2061 746c 6173 4465           atlasDe
+0006b6b0: 7363 7269 7074 5b27 4465 7363 7269 7074  script['Descript
+0006b6c0: 696f 6e27 5d20 3d20 6174 6c61 7344 6573  ion'] = atlasDes
+0006b6d0: 6372 6970 745b 2744 6573 6372 6970 7469  cript['Descripti
+0006b6e0: 6f6e 275d 2e73 7472 2e72 6570 6c61 6365  on'].str.replace
+0006b6f0: 2822 725f 222c 2022 2229 0a20 2020 2020  ("r_", "").     
+0006b700: 2020 2020 2020 2020 2020 2077 6869 6368             which
+0006b710: 696e 6465 7820 3d20 6174 6c61 7344 6573  index = atlasDes
+0006b720: 6372 6970 742e 696e 6465 785b 6174 6c61  cript.index[atla
+0006b730: 7344 6573 6372 6970 745b 2744 6573 6372  sDescript['Descr
+0006b740: 6970 7469 6f6e 275d 203d 3d20 6f67 6c61  iption'] == ogla
+0006b750: 6265 6c6e 616d 655d 2e76 616c 7565 735b  belname].values[
+0006b760: 305d 0a20 2020 2020 2020 2020 2020 2065  0].            e
+0006b770: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0006b780: 2020 2020 2077 6869 6368 696e 6465 7820       whichindex 
+0006b790: 3d20 6174 6c61 7344 6573 6372 6970 742e  = atlasDescript.
+0006b7a0: 696e 6465 785b 6174 6c61 7344 6573 6372  index[atlasDescr
+0006b7b0: 6970 745b 2744 6573 6372 6970 7469 6f6e  ipt['Description
+0006b7c0: 275d 2e73 7472 2e63 6f6e 7461 696e 7328  '].str.contains(
+0006b7d0: 6f67 6c61 6265 6c6e 616d 6529 5d0a 0a20  oglabelname)].. 
+0006b7e0: 2020 2020 2020 2020 2020 2069 6620 7479             if ty
+0006b7f0: 7065 2877 6869 6368 696e 6465 7829 2069  pe(whichindex) i
+0006b800: 7320 6e70 2e69 6e74 3634 3a0a 2020 2020  s np.int64:.    
+0006b810: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
+0006b820: 6c6e 756d 7320 3d20 6174 6c61 7344 6573  lnums = atlasDes
+0006b830: 6372 6970 742e 6c6f 635b 7768 6963 6869  cript.loc[whichi
+0006b840: 6e64 6578 2c20 274c 6162 656c 275d 0a20  ndex, 'Label']. 
+0006b850: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0006b860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0006b870: 206c 6162 656c 6e75 6d73 203d 206c 6973   labelnums = lis
+0006b880: 7428 6174 6c61 7344 6573 6372 6970 742e  t(atlasDescript.
+0006b890: 6c6f 635b 7768 6963 6869 6e64 6578 2c20  loc[whichindex, 
+0006b8a0: 274c 6162 656c 275d 290a 0a20 2020 2020  'Label'])..     
+0006b8b0: 2020 2020 2020 2069 6620 6d79 6578 7420         if myext 
+0006b8c0: 3d3d 2027 7965 6f27 3a0a 2020 2020 2020  == 'yeo':.      
+0006b8d0: 2020 2020 2020 2020 2020 7061 7274 7320            parts 
+0006b8e0: 3d20 7265 2e66 696e 6461 6c6c 2872 275c  = re.findall(r'\
+0006b8f0: 442b 272c 206f 676c 6162 656c 6e61 6d65  D+', oglabelname
+0006b900: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0006b910: 2020 6f67 6c61 6265 6c6e 616d 6520 3d20    oglabelname = 
+0006b920: 5b70 6172 742e 7265 706c 6163 6528 275f  [part.replace('_
+0006b930: 272c 2027 2729 2066 6f72 2070 6172 7420  ', '') for part 
+0006b940: 696e 2070 6172 7473 2069 6620 7061 7274  in parts if part
+0006b950: 2e72 6570 6c61 6365 2827 5f27 2c20 2727  .replace('_', ''
+0006b960: 295d 0a20 2020 2020 2020 2020 2020 2020  )].             
+0006b970: 2020 2066 696c 7465 7265 645f 6466 203d     filtered_df =
+0006b980: 2061 746c 6173 4465 7363 7269 7074 5b61   atlasDescript[a
+0006b990: 746c 6173 4465 7363 7269 7074 5b27 4465  tlasDescript['De
+0006b9a0: 7363 7269 7074 696f 6e27 5d2e 6973 696e  scription'].isin
+0006b9b0: 286f 676c 6162 656c 6e61 6d65 295d 0a20  (oglabelname)]. 
+0006b9c0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+0006b9d0: 6162 656c 6e75 6d73 203d 2066 696c 7465  abelnums = filte
+0006b9e0: 7265 645f 6466 5b27 4c61 6265 6c27 5d2e  red_df['Label'].
+0006b9f0: 746f 6c69 7374 2829 0a0a 2020 2020 2020  tolist()..      
+0006ba00: 2020 2020 2020 6966 206e 6f74 2069 7369        if not isi
+0006ba10: 6e73 7461 6e63 6528 6c61 6265 6c6e 756d  nstance(labelnum
+0006ba20: 732c 206c 6973 7429 3a0a 2020 2020 2020  s, list):.      
+0006ba30: 2020 2020 2020 2020 2020 6c61 6265 6c6e            labeln
+0006ba40: 756d 733d 5b6c 6162 656c 6e75 6d73 5d0a  ums=[labelnums].
+0006ba50: 2020 2020 2020 2020 2020 2020 6164 6465              adde
+0006ba60: 6d69 737a 6572 6f20 3d20 616e 7473 2e74  miszero = ants.t
+0006ba70: 6872 6573 686f 6c64 5f69 6d61 6765 2861  hreshold_image(a
+0006ba80: 6464 656d 2c20 302c 2030 290a 2020 2020  ddem, 0, 0).    
+0006ba90: 2020 2020 2020 2020 7465 6d70 203d 2061          temp = a
+0006baa0: 6e74 732e 696d 6167 655f 7265 6164 286c  nts.image_read(l
+0006bab0: 6f63 6669 6c65 6e61 6d65 290a 2020 2020  ocfilename).    
+0006bac0: 2020 2020 2020 2020 7465 6d70 203d 2061          temp = a
+0006bad0: 6e74 732e 6d61 736b 5f69 6d61 6765 2874  nts.mask_image(t
+0006bae0: 656d 702c 2074 656d 702c 206c 6576 656c  emp, temp, level
+0006baf0: 3d6c 6162 656c 6e75 6d73 2c20 6269 6e61  =labelnums, bina
+0006bb00: 7269 7a65 3d54 7275 6529 0a20 2020 2020  rize=True).     
+0006bb10: 2020 2020 2020 2069 6620 7665 7262 6f73         if verbos
+0006bb20: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0006bb30: 2020 2070 7269 6e74 2822 4445 4255 4722     print("DEBUG"
+0006bb40: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0006bb50: 2020 7072 696e 7428 2020 7465 6d70 2e73    print(  temp.s
+0006bb60: 756d 2829 2029 200a 2020 2020 2020 2020  um() ) .        
+0006bb70: 2020 2020 2020 2020 7072 696e 7428 206c          print( l
+0006bb80: 6162 656c 6e75 6d73 2029 0a20 2020 2020  abelnums ).     
+0006bb90: 2020 2020 2020 2074 656d 705b 7465 6d70         temp[temp
+0006bba0: 203d 3d20 315d 203d 2028 7661 6c73 3276   == 1] = (vals2v
+0006bbb0: 697a 290a 2020 2020 2020 2020 2020 2020  iz).            
+0006bbc0: 7465 6d70 5b61 6464 656d 6973 7a65 726f  temp[addemiszero
+0006bbd0: 203d 3d20 305d 203d 2030 0a20 2020 2020   == 0] = 0.     
+0006bbe0: 2020 2020 2020 2061 6464 656d 203d 2061         addem = a
+0006bbf0: 6464 656d 202b 2074 656d 700a 0a20 2020  ddem + temp..   
+0006bc00: 2020 2020 2069 6620 7665 7262 6f73 653a       if verbose:
+0006bc10: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+0006bc20: 6e74 2827 446f 6e65 2041 6464 696e 6727  nt('Done Adding'
+0006bc30: 290a 2020 2020 2020 2020 666f 7220 6178  ).        for ax
+0006bc40: 7820 696e 2061 7865 733a 0a20 2020 2020  x in axes:.     
+0006bc50: 2020 2020 2020 2066 6967 666e 3d6f 7574         figfn=out
+0006bc60: 7075 745f 7072 6566 6978 2b66 2266 6967  put_prefix+f"fig
+0006bc70: 7b63 6f6c 3276 697a 7d61 787b 6178 787d  {col2viz}ax{axx}
+0006bc80: 5f70 792e 6a70 6722 0a20 2020 2020 2020  _py.jpg".       
+0006bc90: 2020 2020 2069 6620 6372 6f70 203e 2030       if crop > 0
+0006bca0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0006bcb0: 2020 636d 6173 6b20 3d20 616e 7473 2e74    cmask = ants.t
+0006bcc0: 6872 6573 686f 6c64 5f69 6d61 6765 2820  hreshold_image( 
+0006bcd0: 6164 6465 6d2c 3165 2d35 2c20 3165 3920  addem,1e-5, 1e9 
+0006bce0: 292e 694d 6174 6828 224d 4422 2c63 726f  ).iMath("MD",cro
+0006bcf0: 7029 202b 2061 6e74 732e 7468 7265 7368  p) + ants.thresh
+0006bd00: 6f6c 645f 696d 6167 6528 2061 6464 656d  old_image( addem
+0006bd10: 2c2d 3165 392c 202d 3165 2d35 2029 2e69  ,-1e9, -1e-5 ).i
+0006bd20: 4d61 7468 2822 4d44 222c 6372 6f70 290a  Math("MD",crop).
+0006bd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0006bd40: 6164 6465 6d43 203d 2061 6e74 732e 6372  addemC = ants.cr
+0006bd50: 6f70 5f69 6d61 6765 2820 6164 6465 6d2c  op_image( addem,
+0006bd60: 2063 6d61 736b 2029 0a20 2020 2020 2020   cmask ).       
+0006bd70: 2020 2020 2020 2020 2065 6467 6569 6d67           edgeimg
+0006bd80: 4320 3d20 616e 7473 2e63 726f 705f 696d  C = ants.crop_im
+0006bd90: 6167 6528 2065 6467 6569 6d67 2c20 636d  age( edgeimg, cm
+0006bda0: 6173 6b20 290a 2020 2020 2020 2020 2020  ask ).          
+0006bdb0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0006bdc0: 2020 2020 2020 2020 6164 6465 6d43 203d          addemC =
+0006bdd0: 2061 6464 656d 0a20 2020 2020 2020 2020   addem.         
+0006bde0: 2020 2020 2020 2065 6467 6569 6d67 4320         edgeimgC 
+0006bdf0: 3d20 6564 6765 696d 670a 2020 2020 2020  = edgeimg.      
+0006be00: 2020 2020 2020 6966 2066 6978 6564 5f6f        if fixed_o
+0006be10: 7665 726c 6179 5f72 616e 6765 2069 7320  verlay_range is 
+0006be20: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0006be30: 2020 2020 2020 2020 2020 6164 6465 6d43            addemC
+0006be40: 5b30 3a33 2c30 3a33 2c30 3a33 5d3d 6669  [0:3,0:3,0:3]=fi
+0006be50: 7865 645f 6f76 6572 6c61 795f 7261 6e67  xed_overlay_rang
+0006be60: 655b 305d 0a20 2020 2020 2020 2020 2020  e[0].           
+0006be70: 2020 2020 2061 6464 656d 435b 343a 372c       addemC[4:7,
+0006be80: 343a 372c 343a 375d 3d66 6978 6564 5f6f  4:7,4:7]=fixed_o
+0006be90: 7665 726c 6179 5f72 616e 6765 5b31 5d0a  verlay_range[1].
+0006bea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0006beb0: 6164 6465 6d43 5b20 6164 6465 6d43 203c  addemC[ addemC <
+0006bec0: 2066 6978 6564 5f6f 7665 726c 6179 5f72   fixed_overlay_r
+0006bed0: 616e 6765 5b30 5d20 5d20 3d20 6669 7865  ange[0] ] = fixe
+0006bee0: 645f 6f76 6572 6c61 795f 7261 6e67 655b  d_overlay_range[
+0006bef0: 305d 0a20 2020 2020 2020 2020 2020 2020  0].             
+0006bf00: 2020 2061 6464 656d 435b 2061 6464 656d     addemC[ addem
+0006bf10: 4320 3e20 6669 7865 645f 6f76 6572 6c61  C > fixed_overla
+0006bf20: 795f 7261 6e67 655b 315d 205d 203d 2066  y_range[1] ] = f
+0006bf30: 6978 6564 5f6f 7665 726c 6179 5f72 616e  ixed_overlay_ran
+0006bf40: 6765 5b31 5d0a 2020 2020 2020 2020 2020  ge[1].          
+0006bf50: 2020 616e 7473 2e70 6c6f 7428 6564 6765    ants.plot(edge
+0006bf60: 696d 6743 2c20 6164 6465 6d43 2c20 6178  imgC, addemC, ax
+0006bf70: 6973 3d61 7878 2c20 6e73 6c69 6365 733d  is=axx, nslices=
+0006bf80: 6e73 6c69 6365 732c 206e 636f 6c3d 6e63  nslices, ncol=nc
+0006bf90: 6f6c 2c20 2020 2020 2020 0a20 2020 2020  ol,       .     
+0006bfa0: 2020 2020 2020 2020 2020 206f 7665 726c             overl
+0006bfb0: 6179 5f63 6d61 703d 6f76 6572 6c61 795f  ay_cmap=overlay_
+0006bfc0: 636d 6170 2c20 7265 7361 6d70 6c65 3d46  cmap, resample=F
+0006bfd0: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
+0006bfe0: 2020 2020 2020 6669 6c65 6e61 6d65 3d66        filename=f
+0006bff0: 6967 666e 2c20 6362 6172 3d61 7878 3d3d  igfn, cbar=axx==
+0006c000: 6178 6573 5b30 5d2c 2063 726f 703d 5472  axes[0], crop=Tr
+0006c010: 7565 2c20 626c 6163 6b5f 6267 3d62 6c61  ue, black_bg=bla
+0006c020: 636b 5f62 6720 290a 2020 2020 2020 2020  ck_bg ).        
+0006c030: 6966 2076 6572 626f 7365 3a0a 2020 2020  if verbose:.    
+0006c040: 2020 2020 2020 2020 7072 696e 7428 6622          print(f"
+0006c050: 7b63 6f6c 3276 697a 7d20 646f 6e65 2229  {col2viz} done")
+0006c060: 0a20 2020 2069 6620 7665 7262 6f73 653a  .    if verbose:
+0006c070: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
+0006c080: 444f 4e45 2062 7261 696e 206d 6170 2066  DONE brain map f
+0006c090: 6967 7572 6573 2229 0a20 2020 2072 6574  igures").    ret
+0006c0a0: 7572 6e20 6164 6465 6d0a 0a64 6566 2066  urn addem..def f
+0006c0b0: 696c 7465 725f 6466 2869 6e64 662c 206d  ilter_df(indf, m
+0006c0c0: 7970 7265 6669 7829 3a0a 2020 2020 2222  yprefix):.    ""
+0006c0d0: 220a 2020 2020 5072 6f63 6573 7320 616e  ".    Process an
+0006c0e0: 6420 6669 6c74 6572 2061 2070 616e 6461  d filter a panda
+0006c0f0: 7320 4461 7461 4672 616d 652c 2072 656d  s DataFrame, rem
+0006c100: 6f76 696e 6720 6365 7274 6169 6e20 636f  oving certain co
+0006c110: 6c75 6d6e 732c 200a 2020 2020 6669 6c74  lumns, .    filt
+0006c120: 6572 696e 6720 6261 7365 6420 6f6e 2064  ering based on d
+0006c130: 6174 6120 7479 7065 732c 2063 6f6d 7075  ata types, compu
+0006c140: 7469 6e67 2074 6865 206d 6561 6e20 6f66  ting the mean of
+0006c150: 206e 756d 6572 6963 2063 6f6c 756d 6e73   numeric columns
+0006c160: 2c20 0a20 2020 2061 6e64 2061 6464 696e  , .    and addin
+0006c170: 6720 6120 7072 6566 6978 2074 6f20 636f  g a prefix to co
+0006c180: 6c75 6d6e 206e 616d 6573 2e0a 0a20 2020  lumn names...   
+0006c190: 2050 6172 616d 6574 6572 733a 0a20 2020   Parameters:.   
+0006c1a0: 2069 6e64 6620 2870 616e 6461 732e 4461   indf (pandas.Da
+0006c1b0: 7461 4672 616d 6529 3a20 5468 6520 696e  taFrame): The in
+0006c1c0: 7075 7420 4461 7461 4672 616d 6520 746f  put DataFrame to
+0006c1d0: 2062 6520 7072 6f63 6573 7365 642e 0a20   be processed.. 
+0006c1e0: 2020 206d 7970 7265 6669 7820 2873 7472     myprefix (str
+0006c1f0: 293a 2041 2073 7472 696e 6720 7072 6566  ): A string pref
+0006c200: 6978 2074 6f20 6265 2061 6464 6564 2074  ix to be added t
+0006c210: 6f20 7468 6520 636f 6c75 6d6e 206e 616d  o the column nam
+0006c220: 6573 200a 2020 2020 2020 2020 2020 2020  es .            
+0006c230: 2020 2020 2020 2020 6f66 2074 6865 2070          of the p
+0006c240: 726f 6365 7373 6564 2044 6174 6146 7261  rocessed DataFra
+0006c250: 6d65 2e0a 0a20 2020 2053 7465 7073 3a0a  me...    Steps:.
+0006c260: 2020 2020 312e 2052 656d 6f76 6573 2063      1. Removes c
+0006c270: 6f6c 756d 6e73 2077 6974 6820 6e61 6d65  olumns with name
+0006c280: 7320 636f 6e74 6169 6e69 6e67 2027 556e  s containing 'Un
+0006c290: 6e61 6d65 6427 2e0a 2020 2020 322e 2049  named'..    2. I
+0006c2a0: 6620 7468 6520 4461 7461 4672 616d 6520  f the DataFrame 
+0006c2b0: 6861 7320 6e6f 2072 6f77 732c 2069 7420  has no rows, it 
+0006c2c0: 7265 7475 726e 7320 7468 6520 656d 7074  returns the empt
+0006c2d0: 7920 4461 7461 4672 616d 652e 0a20 2020  y DataFrame..   
+0006c2e0: 2033 2e20 4669 6c74 6572 7320 6f75 7420   3. Filters out 
+0006c2f0: 636f 6c75 6d6e 7320 6261 7365 6420 6f6e  columns based on
+0006c300: 2074 6865 2074 7970 6520 6f66 2074 6865   the type of the
+0006c310: 2066 6972 7374 2065 6c65 6d65 6e74 2c20   first element, 
+0006c320: 0a20 2020 2020 2020 6b65 6570 696e 6720  .       keeping 
+0006c330: 7468 6f73 6520 7468 6174 2061 7265 206f  those that are o
+0006c340: 6620 7479 7065 2060 6f62 6a65 6374 602c  f type `object`,
+0006c350: 2060 696e 7460 2c20 6f72 2060 666c 6f61   `int`, or `floa
+0006c360: 7460 2e0a 2020 2020 342e 2052 656d 6f76  t`..    4. Remov
+0006c370: 6573 2063 6f6c 756d 6e73 2074 6861 7420  es columns that 
+0006c380: 6172 6520 6f66 2060 6f62 6a65 6374 6020  are of `object` 
+0006c390: 6474 7970 652e 0a20 2020 2035 2e20 4361  dtype..    5. Ca
+0006c3a0: 6c63 756c 6174 6573 2074 6865 206d 6561  lculates the mea
+0006c3b0: 6e20 6f66 2074 6865 2072 656d 6169 6e69  n of the remaini
+0006c3c0: 6e67 2063 6f6c 756d 6e73 2c20 736b 6970  ng columns, skip
+0006c3d0: 7069 6e67 204e 614e 2076 616c 7565 732e  ping NaN values.
+0006c3e0: 0a20 2020 2036 2e20 4164 6473 2074 6865  .    6. Adds the
+0006c3f0: 2073 7065 6369 6669 6564 2060 6d79 7072   specified `mypr
+0006c400: 6566 6978 6020 746f 2074 6865 2063 6f6c  efix` to the col
+0006c410: 756d 6e20 6e61 6d65 732e 0a0a 2020 2020  umn names...    
+0006c420: 5265 7475 726e 733a 0a20 2020 2070 616e  Returns:.    pan
+0006c430: 6461 732e 4461 7461 4672 616d 653a 2041  das.DataFrame: A
+0006c440: 2074 7261 6e73 666f 726d 6564 2044 6174   transformed Dat
+0006c450: 6146 7261 6d65 2077 6974 6820 6120 7369  aFrame with a si
+0006c460: 6e67 6c65 2072 6f77 2063 6f6e 7461 696e  ngle row contain
+0006c470: 696e 6720 0a20 2020 2020 2020 2020 2020  ing .           
+0006c480: 2020 2020 2020 2020 2020 2074 6865 206d             the m
+0006c490: 6561 6e20 7661 6c75 6573 206f 6620 7468  ean values of th
+0006c4a0: 6520 6669 6c74 6572 6564 2063 6f6c 756d  e filtered colum
+0006c4b0: 6e73 2c20 616e 6420 7769 7468 200a 2020  ns, and with .  
+0006c4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0006c4d0: 2020 2020 636f 6c75 6d6e 206e 616d 6573      column names
+0006c4e0: 2070 7265 6669 7865 6420 6173 2073 7065   prefixed as spe
+0006c4f0: 6369 6669 6564 2e0a 2020 2020 2222 220a  cified..    """.
+0006c500: 2020 2020 696e 6466 203d 2069 6e64 662e      indf = indf.
+0006c510: 6c6f 635b 3a2c 207e 696e 6466 2e63 6f6c  loc[:, ~indf.col
+0006c520: 756d 6e73 2e73 7472 2e63 6f6e 7461 696e  umns.str.contain
+0006c530: 7328 2755 6e6e 616d 6564 2a27 2c20 6e61  s('Unnamed*', na
+0006c540: 3d46 616c 7365 2c20 7265 6765 783d 5472  =False, regex=Tr
+0006c550: 7565 295d 0a20 2020 2069 6620 696e 6466  ue)].    if indf
+0006c560: 2e73 6861 7065 5b30 5d20 3d3d 2030 3a0a  .shape[0] == 0:.
+0006c570: 2020 2020 2020 2020 7265 7475 726e 2069          return i
+0006c580: 6e64 660a 2020 2020 6e75 6d73 203d 205b  ndf.    nums = [
+0006c590: 6973 696e 7374 616e 6365 2869 6e64 665b  isinstance(indf[
+0006c5a0: 636f 6c5d 2e69 6c6f 635b 305d 2c20 286f  col].iloc[0], (o
+0006c5b0: 626a 6563 742c 2069 6e74 2c20 666c 6f61  bject, int, floa
+0006c5c0: 7429 2920 666f 7220 636f 6c20 696e 2069  t)) for col in i
+0006c5d0: 6e64 662e 636f 6c75 6d6e 735d 0a20 2020  ndf.columns].   
+0006c5e0: 2069 6e64 6620 3d20 696e 6466 2e6c 6f63   indf = indf.loc
+0006c5f0: 5b3a 2c20 6e75 6d73 5d0a 2020 2020 696e  [:, nums].    in
+0006c600: 6466 203d 2069 6e64 662e 6c6f 635b 3a2c  df = indf.loc[:,
+0006c610: 2069 6e64 662e 6474 7970 6573 2021 3d20   indf.dtypes != 
+0006c620: 276f 626a 6563 7427 5d0a 2020 2020 696e  'object'].    in
+0006c630: 6466 203d 2070 642e 4461 7461 4672 616d  df = pd.DataFram
+0006c640: 6528 696e 6466 2e6d 6561 6e28 6178 6973  e(indf.mean(axis
+0006c650: 3d30 2c20 736b 6970 6e61 3d54 7275 6529  =0, skipna=True)
+0006c660: 292e 540a 2020 2020 696e 6466 203d 2069  ).T.    indf = i
+0006c670: 6e64 662e 6164 645f 7072 6566 6978 286d  ndf.add_prefix(m
+0006c680: 7970 7265 6669 7829 0a20 2020 2072 6574  yprefix).    ret
+0006c690: 7572 6e20 696e 6466 0a0a 0a64 6566 2061  urn indf...def a
+0006c6a0: 6767 7265 6761 7465 5f61 6e74 7370 796d  ggregate_antspym
+0006c6b0: 6d5f 7265 7375 6c74 7328 696e 7075 745f  m_results(input_
+0006c6c0: 6373 762c 2073 7562 6a65 6374 5f63 6f6c  csv, subject_col
+0006c6d0: 3d27 7375 626a 6563 7449 4427 2c20 6461  ='subjectID', da
+0006c6e0: 7465 5f63 6f6c 3d27 6461 7465 272c 2069  te_col='date', i
+0006c6f0: 6d61 6765 5f63 6f6c 3d27 696d 6167 6549  mage_col='imageI
+0006c700: 4427 2c20 6461 7465 5f63 6f6c 756d 6e3d  D', date_column=
+0006c710: 2773 6573 2d31 272c 2062 6173 655f 7061  'ses-1', base_pa
+0006c720: 7468 3d22 2e2f 5072 6f63 6573 7365 642f  th="./Processed/
+0006c730: 414e 5473 4578 7041 7274 2f22 2c20 6869  ANTsExpArt/", hi
+0006c740: 6572 7661 7269 6162 6c65 3d27 5431 7748  ervariable='T1wH
+0006c750: 6965 7261 7263 6869 6361 6c27 2c20 7661  ierarchical', va
+0006c760: 6c69 645f 6d6f 6461 6c69 7469 6573 3d4e  lid_modalities=N
+0006c770: 6f6e 652c 2076 6572 626f 7365 3d46 616c  one, verbose=Fal
+0006c780: 7365 2029 3a0a 2020 2020 2222 220a 2020  se ):.    """.  
+0006c790: 2020 4167 6772 6567 6174 6520 414e 5473    Aggregate ANTs
+0006c7a0: 5079 4d4d 2072 6573 756c 7473 2066 726f  PyMM results fro
+0006c7b0: 6d20 7468 6520 7370 6563 6966 6965 6420  m the specified 
+0006c7c0: 4353 5620 6669 6c65 2061 6e64 2073 6176  CSV file and sav
+0006c7d0: 6520 7468 6520 6167 6772 6567 6174 6564  e the aggregated
+0006c7e0: 2072 6573 756c 7473 2074 6f20 6120 6e65   results to a ne
+0006c7f0: 7720 4353 5620 6669 6c65 2e0a 0a20 2020  w CSV file...   
+0006c800: 2050 6172 616d 6574 6572 733a 0a20 2020   Parameters:.   
+0006c810: 202d 2069 6e70 7574 5f63 7376 2028 7374   - input_csv (st
+0006c820: 7229 3a20 4669 6c65 2070 6174 6820 6f66  r): File path of
+0006c830: 2074 6865 2069 6e70 7574 2043 5356 2066   the input CSV f
+0006c840: 696c 6520 636f 6e74 6169 6e69 6e67 2041  ile containing A
+0006c850: 4e54 7350 794d 4d20 5143 2072 6573 756c  NTsPyMM QC resul
+0006c860: 7473 2061 7665 7261 6765 6420 616e 6420  ts averaged and 
+0006c870: 7769 7468 206f 7574 6c69 6572 206d 6561  with outlier mea
+0006c880: 7375 7265 6d65 6e74 732e 0a20 2020 202d  surements..    -
+0006c890: 2073 7562 6a65 6374 5f63 6f6c 2028 7374   subject_col (st
+0006c8a0: 7229 3a20 4e61 6d65 206f 6620 7468 6520  r): Name of the 
+0006c8b0: 636f 6c75 6d6e 2074 6f20 7374 6f72 6520  column to store 
+0006c8c0: 7375 626a 6563 7420 4944 732e 0a20 2020  subject IDs..   
+0006c8d0: 202d 2064 6174 655f 636f 6c20 2873 7472   - date_col (str
+0006c8e0: 293a 204e 616d 6520 6f66 2074 6865 2063  ): Name of the c
+0006c8f0: 6f6c 756d 6e20 746f 2073 746f 7265 2064  olumn to store d
+0006c900: 6174 6520 696e 666f 726d 6174 696f 6e2e  ate information.
+0006c910: 0a20 2020 202d 2069 6d61 6765 5f63 6f6c  .    - image_col
+0006c920: 2028 7374 7229 3a20 4e61 6d65 206f 6620   (str): Name of 
+0006c930: 7468 6520 636f 6c75 6d6e 2074 6f20 7374  the column to st
+0006c940: 6f72 6520 696d 6167 6520 4944 732e 0a20  ore image IDs.. 
+0006c950: 2020 202d 2064 6174 655f 636f 6c75 6d6e     - date_column
+0006c960: 2028 7374 7229 3a20 4e61 6d65 206f 6620   (str): Name of 
+0006c970: 7468 6520 636f 6c75 6d6e 2072 6570 7265  the column repre
+0006c980: 7365 6e74 696e 6720 7468 6520 6461 7465  senting the date
+0006c990: 2069 6e66 6f72 6d61 7469 6f6e 2e0a 2020   information..  
+0006c9a0: 2020 2d20 6261 7365 5f70 6174 6820 2873    - base_path (s
+0006c9b0: 7472 293a 2042 6173 6520 7061 7468 2066  tr): Base path f
+0006c9c0: 6f72 2073 6561 7263 6820 7061 7468 732e  or search paths.
+0006c9d0: 2044 6566 6175 6c74 7320 746f 2022 2e2f   Defaults to "./
+0006c9e0: 5072 6f63 6573 7365 642f 414e 5473 4578  Processed/ANTsEx
+0006c9f0: 7041 7274 2f22 2e0a 2020 2020 2d20 6869  pArt/"..    - hi
+0006ca00: 6572 7661 7269 6162 6c65 2028 7374 7229  ervariable (str)
+0006ca10: 203a 2074 6865 2073 7472 696e 6720 7661   : the string va
+0006ca20: 7269 6162 6c65 2064 656e 6f74 696e 6720  riable denoting 
+0006ca30: 7468 6520 4869 6572 6172 6368 6963 616c  the Hierarchical
+0006ca40: 206f 7574 7075 740a 2020 2020 2d20 7661   output.    - va
+0006ca50: 6c69 645f 6d6f 6461 6c69 7469 6573 2028  lid_modalities (
+0006ca60: 7374 7220 6172 7261 7929 203a 2069 6465  str array) : ide
+0006ca70: 6e74 6966 6965 7320 666f 7220 6561 6368  ntifies for each
+0006ca80: 206d 6f64 616c 6974 793b 2069 6620 4e6f   modality; if No
+0006ca90: 6e65 2077 696c 6c20 6265 2072 6570 6c61  ne will be repla
+0006caa0: 6365 6420 6279 2067 6574 5f76 616c 6964  ced by get_valid
+0006cab0: 5f6d 6f64 616c 6974 6965 7328 6c6f 6e67  _modalities(long
+0006cac0: 3d54 7275 6529 0a20 2020 202d 2076 6572  =True).    - ver
+0006cad0: 626f 7365 203a 2062 6f6f 6c65 616e 0a0a  bose : boolean..
+0006cae0: 2020 2020 4e6f 7465 3a0a 2020 2020 5468      Note:.    Th
+0006caf0: 6973 2066 756e 6374 696f 6e20 6973 2074  is function is t
+0006cb00: 6573 7465 6420 756e 6465 7220 6c69 6d69  ested under limi
+0006cb10: 7465 6420 6369 7263 756d 7374 616e 6365  ted circumstance
+0006cb20: 732e 2055 7365 2077 6974 6820 6361 7574  s. Use with caut
+0006cb30: 696f 6e2e 0a0a 2020 2020 4578 616d 706c  ion...    Exampl
+0006cb40: 6520 7573 6167 653a 0a20 2020 2061 6767  e usage:.    agg
+0006cb50: 5f64 6620 3d20 6167 6772 6567 6174 655f  _df = aggregate_
+0006cb60: 616e 7473 7079 6d6d 5f72 6573 756c 7473  antspymm_results
+0006cb70: 2822 7163 6466 616f 6c2e 6373 7622 2c20  ("qcdfaol.csv", 
+0006cb80: 7375 626a 6563 745f 636f 6c3d 2773 7562  subject_col='sub
+0006cb90: 6a65 6374 4944 272c 2064 6174 655f 636f  jectID', date_co
+0006cba0: 6c3d 2764 6174 6527 2c20 696d 6167 655f  l='date', image_
+0006cbb0: 636f 6c3d 2769 6d61 6765 4944 272c 2064  col='imageID', d
+0006cbc0: 6174 655f 636f 6c75 6d6e 3d27 7365 732d  ate_column='ses-
+0006cbd0: 3127 2c20 6261 7365 5f70 6174 683d 222e  1', base_path=".
+0006cbe0: 2f59 6f75 722f 4375 7374 6f6d 2f50 6174  /Your/Custom/Pat
+0006cbf0: 682f 2229 0a0a 2020 2020 4175 7468 6f72  h/")..    Author
+0006cc00: 3a0a 2020 2020 4176 616e 7473 2061 6e64  :.    Avants and
+0006cc10: 2043 6861 7447 5054 0a20 2020 2022 2222   ChatGPT.    """
+0006cc20: 0a20 2020 2069 6d70 6f72 7420 7061 6e64  .    import pand
+0006cc30: 6173 2061 7320 7064 0a20 2020 2069 6d70  as as pd.    imp
+0006cc40: 6f72 7420 6e75 6d70 7920 6173 206e 700a  ort numpy as np.
+0006cc50: 2020 2020 6672 6f6d 2067 6c6f 6220 696d      from glob im
+0006cc60: 706f 7274 2067 6c6f 620a 0a20 2020 2064  port glob..    d
+0006cc70: 6566 206d 7972 6561 645f 6373 7628 782c  ef myread_csv(x,
+0006cc80: 2063 6e6d 7329 3a0a 2020 2020 2020 2020   cnms):.        
+0006cc90: 2222 220a 2020 2020 2020 2020 5265 6164  """.        Read
+0006cca0: 7320 6120 4353 5620 6669 6c65 2061 6e64  s a CSV file and
+0006ccb0: 2072 6574 7572 6e73 2061 2044 6174 6146   returns a DataF
+0006ccc0: 7261 6d65 2065 7863 6c75 6469 6e67 2073  rame excluding s
+0006ccd0: 7065 6369 6669 6564 2063 6f6c 756d 6e73  pecified columns
+0006cce0: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+0006ccf0: 6574 6572 733a 0a20 2020 2020 2020 202d  eters:.        -
+0006cd00: 2078 2028 7374 7229 3a20 4669 6c65 2070   x (str): File p
+0006cd10: 6174 6820 6f66 2074 6865 2069 6e70 7574  ath of the input
+0006cd20: 2043 5356 2066 696c 6520 6465 7363 7269   CSV file descri
+0006cd30: 6269 6e67 2074 6865 2062 6c69 6e64 2051  bing the blind Q
+0006cd40: 4320 6f75 7470 7574 0a20 2020 2020 2020  C output.       
+0006cd50: 202d 2063 6e6d 7320 286c 6973 7429 3a20   - cnms (list): 
+0006cd60: 4c69 7374 206f 6620 636f 6c75 6d6e 206e  List of column n
+0006cd70: 616d 6573 2074 6f20 6578 636c 7564 6520  ames to exclude 
+0006cd80: 6672 6f6d 2074 6865 2044 6174 6146 7261  from the DataFra
+0006cd90: 6d65 2e0a 0a20 2020 2020 2020 2052 6574  me...        Ret
+0006cda0: 7572 6e73 3a0a 2020 2020 2020 2020 7064  urns:.        pd
+0006cdb0: 2e44 6174 6146 7261 6d65 3a20 4461 7461  .DataFrame: Data
+0006cdc0: 4672 616d 6520 7769 7468 2073 7065 6369  Frame with speci
+0006cdd0: 6669 6564 2063 6f6c 756d 6e73 2065 7863  fied columns exc
+0006cde0: 6c75 6465 642e 0a20 2020 2020 2020 2022  luded..        "
+0006cdf0: 2222 0a20 2020 2020 2020 2064 6620 3d20  "".        df = 
+0006ce00: 7064 2e72 6561 645f 6373 7628 7829 0a20  pd.read_csv(x). 
+0006ce10: 2020 2020 2020 2072 6574 7572 6e20 6466         return df
+0006ce20: 2e6c 6f63 5b3a 2c20 7e64 662e 636f 6c75  .loc[:, ~df.colu
+0006ce30: 6d6e 732e 6973 696e 2863 6e6d 7329 5d0a  mns.isin(cnms)].
+0006ce40: 0a20 2020 2069 6d70 6f72 7420 7761 726e  .    import warn
+0006ce50: 696e 6773 0a20 2020 2023 2057 6172 6e69  ings.    # Warni
+0006ce60: 6e67 206d 6573 7361 6765 2066 6f72 2075  ng message for u
+0006ce70: 6e74 6573 7465 6420 6675 6e63 7469 6f6e  ntested function
+0006ce80: 0a20 2020 2077 6172 6e69 6e67 732e 7761  .    warnings.wa
+0006ce90: 726e 2822 5761 726e 696e 673a 2054 6869  rn("Warning: Thi
+0006cea0: 7320 6675 6e63 7469 6f6e 2069 7320 6e6f  s function is no
+0006ceb0: 7420 7765 6c6c 2074 6573 7465 642e 2055  t well tested. U
+0006cec0: 7365 2077 6974 6820 6361 7574 696f 6e2e  se with caution.
+0006ced0: 2229 0a0a 2020 2020 6966 2076 616c 6964  ")..    if valid
+0006cee0: 5f6d 6f64 616c 6974 6965 7320 6973 204e  _modalities is N
+0006cef0: 6f6e 653a 0a20 2020 2020 2020 2076 616c  one:.        val
+0006cf00: 6964 5f6d 6f64 616c 6974 6965 7320 3d20  id_modalities = 
+0006cf10: 6765 745f 7661 6c69 645f 6d6f 6461 6c69  get_valid_modali
+0006cf20: 7469 6573 2827 6c6f 6e67 2729 0a0a 2020  ties('long')..  
+0006cf30: 2020 2320 5265 6164 2074 6865 2069 6e70    # Read the inp
+0006cf40: 7574 2043 5356 2066 696c 650a 2020 2020  ut CSV file.    
+0006cf50: 6466 203d 2070 642e 7265 6164 5f63 7376  df = pd.read_csv
+0006cf60: 2869 6e70 7574 5f63 7376 290a 0a20 2020  (input_csv)..   
+0006cf70: 2023 2046 696c 7465 7220 726f 7773 2077   # Filter rows w
+0006cf80: 6865 7265 206d 6f64 616c 6974 7920 6973  here modality is
+0006cf90: 2027 5431 7727 0a20 2020 2064 6620 3d20   'T1w'.    df = 
+0006cfa0: 6466 5b64 665b 276d 6f64 616c 6974 7927  df[df['modality'
+0006cfb0: 5d20 3d3d 2027 5431 7727 5d0a 2020 2020  ] == 'T1w'].    
+0006cfc0: 6261 646e 616d 6573 203d 2067 6574 5f6e  badnames = get_n
+0006cfd0: 616d 6573 5f66 726f 6d5f 6461 7461 5f66  ames_from_data_f
+0006cfe0: 7261 6d65 2820 5b27 556e 6e61 6d65 6427  rame( ['Unnamed'
+0006cff0: 5d2c 2064 6620 290a 2020 2020 6466 3d64  ], df ).    df=d
+0006d000: 662e 6472 6f70 2862 6164 6e61 6d65 732c  f.drop(badnames,
+0006d010: 2061 7869 733d 3129 0a0a 2020 2020 2320   axis=1)..    # 
+0006d020: 4164 6420 6e65 7720 636f 6c75 6d6e 7320  Add new columns 
+0006d030: 666f 7220 7375 626a 6563 7420 4944 2c20  for subject ID, 
+0006d040: 6461 7465 2c20 616e 6420 696d 6167 6520  date, and image 
+0006d050: 4944 0a20 2020 2064 665b 7375 626a 6563  ID.    df[subjec
+0006d060: 745f 636f 6c5d 203d 206e 702e 6e61 6e0a  t_col] = np.nan.
+0006d070: 2020 2020 6466 5b64 6174 655f 636f 6c5d      df[date_col]
+0006d080: 203d 2064 6174 655f 636f 6c75 6d6e 0a20   = date_column. 
+0006d090: 2020 2064 665b 696d 6167 655f 636f 6c5d     df[image_col]
+0006d0a0: 203d 206e 702e 6e61 6e0a 2020 2020 6466   = np.nan.    df
+0006d0b0: 203d 2064 662e 6173 7479 7065 287b 7375   = df.astype({su
+0006d0c0: 626a 6563 745f 636f 6c3a 2073 7472 2c20  bject_col: str, 
+0006d0d0: 6461 7465 5f63 6f6c 3a20 7374 722c 2069  date_col: str, i
+0006d0e0: 6d61 6765 5f63 6f6c 3a20 7374 7220 7d29  mage_col: str })
+0006d0f0: 0a0a 2320 2020 2069 6620 7665 7262 6f73  ..#    if verbos
+0006d100: 653a 0a23 2020 2020 2020 2020 7072 696e  e:.#        prin
+0006d110: 7428 2064 662e 7368 6170 6520 290a 2320  t( df.shape ).# 
+0006d120: 2020 2020 2020 2070 7269 6e74 2820 6466         print( df
+0006d130: 2e64 7479 7065 7320 290a 0a20 2020 2023  .dtypes )..    #
+0006d140: 2070 7265 6669 6c74 6572 2064 6620 666f   prefilter df fo
+0006d150: 7220 6461 7461 2074 6861 7420 6578 6973  r data that exis
+0006d160: 7473 0a20 2020 206b 6565 7020 3d20 6e70  ts.    keep = np
+0006d170: 2e74 696c 6528 2046 616c 7365 2c20 6466  .tile( False, df
+0006d180: 2e73 6861 7065 5b30 5d20 290a 2020 2020  .shape[0] ).    
+0006d190: 666f 7220 7820 696e 2072 616e 6765 2864  for x in range(d
+0006d1a0: 662e 7368 6170 655b 305d 293a 0a20 2020  f.shape[0]):.   
+0006d1b0: 2020 2020 2074 656d 7020 3d20 6466 5b27       temp = df['
+0006d1c0: 6669 6c65 6e61 6d65 275d 2e69 6c6f 635b  filename'].iloc[
+0006d1d0: 785d 2e73 706c 6974 2822 5f22 290a 2020  x].split("_").  
+0006d1e0: 2020 2020 2020 2320 4765 6e65 7261 6c69        # Generali
+0006d1f0: 7a65 6420 7365 6172 6368 2070 6174 6873  zed search paths
+0006d200: 0a20 2020 2020 2020 2070 6174 685f 7465  .        path_te
+0006d210: 6d70 6c61 7465 203d 2066 227b 6261 7365  mplate = f"{base
+0006d220: 5f70 6174 687d 7b74 656d 705b 305d 7d2f  _path}{temp[0]}/
+0006d230: 7b64 6174 655f 636f 6c75 6d6e 7d2f 2a2f  {date_column}/*/
+0006d240: 2a2f 2a22 0a20 2020 2020 2020 2068 6965  */*".        hie
+0006d250: 7266 6e20 3d20 736f 7274 6564 2867 6c6f  rfn = sorted(glo
+0006d260: 6228 2070 6174 685f 7465 6d70 6c61 7465  b( path_template
+0006d270: 202b 2022 2d22 202b 2068 6965 7276 6172   + "-" + hiervar
+0006d280: 6961 626c 6520 2b20 222d 2a77 6964 652e  iable + "-*wide.
+0006d290: 6373 7622 2029 2029 0a20 2020 2020 2020  csv" ) ).       
+0006d2a0: 2069 6620 6c65 6e28 2068 6965 7266 6e20   if len( hierfn 
+0006d2b0: 2920 3e20 303a 0a20 2020 2020 2020 2020  ) > 0:.         
+0006d2c0: 2020 206b 6565 705b 785d 3d54 7275 650a     keep[x]=True.
+0006d2d0: 0a20 2020 200a 2020 2020 6466 3d64 665b  .    .    df=df[
+0006d2e0: 6b65 6570 5d0a 2020 2020 0a20 2020 2069  keep].    .    i
+0006d2f0: 6620 7665 7262 6f73 653a 0a20 2020 2020  f verbose:.     
+0006d300: 2020 2070 7269 6e74 2820 226f 7269 6769     print( "origi
+0006d310: 6e61 6c20 696e 7075 7420 6861 6420 7368  nal input had sh
+0006d320: 6170 6520 2220 2b20 7374 7228 2064 662e  ape " + str( df.
+0006d330: 7368 6170 655b 305d 2029 202b 2022 2028  shape[0] ) + " (
+0006d340: 5431 206f 6e6c 7929 2061 6e64 2077 6520  T1 only) and we 
+0006d350: 6669 6e64 2022 202b 2073 7472 2820 286b  find " + str( (k
+0006d360: 6565 7029 2e73 756d 2829 2029 202b 2022  eep).sum() ) + "
+0006d370: 2077 6974 6820 6869 6572 6172 6368 6963   with hierarchic
+0006d380: 616c 206f 7574 7075 7420 6465 6669 6e65  al output define
+0006d390: 6420 6279 2076 6172 6961 626c 653a 2022  d by variable: "
+0006d3a0: 202b 2068 6965 7276 6172 6961 626c 6520   + hiervariable 
+0006d3b0: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
+0006d3c0: 2064 662e 7368 6170 6520 290a 0a20 2020   df.shape )..   
+0006d3d0: 206d 7963 7420 3d20 300a 2020 2020 666f   myct = 0.    fo
+0006d3e0: 7220 7820 696e 2072 616e 6765 2820 6466  r x in range( df
+0006d3f0: 2e73 6861 7065 5b30 5d29 3a0a 2020 2020  .shape[0]):.    
+0006d400: 2020 2020 6966 2076 6572 626f 7365 3a0a      if verbose:.
+0006d410: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+0006d420: 7428 6622 7b78 7d2e 2e2e 2229 0a20 2020  t(f"{x}...").   
+0006d430: 2020 2020 206c 6f63 696e 6420 3d20 6466       locind = df
+0006d440: 2e69 6e64 6578 5b78 5d0a 2020 2020 2020  .index[x].      
+0006d450: 2020 7465 6d70 203d 2064 665b 2766 696c    temp = df['fil
+0006d460: 656e 616d 6527 5d2e 696c 6f63 5b78 5d2e  ename'].iloc[x].
+0006d470: 7370 6c69 7428 225f 2229 0a20 2020 2020  split("_").     
+0006d480: 2020 2069 6620 7665 7262 6f73 653a 0a20     if verbose:. 
+0006d490: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+0006d4a0: 2820 7465 6d70 2029 0a20 2020 2020 2020  ( temp ).       
+0006d4b0: 2064 665b 7375 626a 6563 745f 636f 6c5d   df[subject_col]
+0006d4c0: 2e69 6c6f 635b 785d 3d74 656d 705b 305d  .iloc[x]=temp[0]
+0006d4d0: 0a20 2020 2020 2020 2064 665b 6461 7465  .        df[date
+0006d4e0: 5f63 6f6c 5d2e 696c 6f63 5b78 5d3d 6461  _col].iloc[x]=da
+0006d4f0: 7465 5f63 6f6c 756d 6e0a 2020 2020 2020  te_column.      
+0006d500: 2020 6466 5b69 6d61 6765 5f63 6f6c 5d2e    df[image_col].
+0006d510: 696c 6f63 5b78 5d3d 7465 6d70 5b31 5d0a  iloc[x]=temp[1].
+0006d520: 0a20 2020 2020 2020 2023 2047 656e 6572  .        # Gener
+0006d530: 616c 697a 6564 2073 6561 7263 6820 7061  alized search pa
+0006d540: 7468 730a 2020 2020 2020 2020 7061 7468  ths.        path
+0006d550: 5f74 656d 706c 6174 6520 3d20 6622 7b62  _template = f"{b
+0006d560: 6173 655f 7061 7468 7d7b 7465 6d70 5b30  ase_path}{temp[0
+0006d570: 5d7d 2f7b 6461 7465 5f63 6f6c 756d 6e7d  ]}/{date_column}
+0006d580: 2f2a 2f2a 2f2a 220a 2020 2020 2020 2020  /*/*/*".        
+0006d590: 6966 2076 6572 626f 7365 3a0a 2020 2020  if verbose:.    
+0006d5a0: 2020 2020 2020 2020 7072 696e 7428 7061          print(pa
+0006d5b0: 7468 5f74 656d 706c 6174 6529 0a20 2020  th_template).   
+0006d5c0: 2020 2020 2068 6965 7266 6e20 3d20 736f       hierfn = so
+0006d5d0: 7274 6564 2867 6c6f 6228 2070 6174 685f  rted(glob( path_
+0006d5e0: 7465 6d70 6c61 7465 202b 2022 2d22 202b  template + "-" +
+0006d5f0: 2068 6965 7276 6172 6961 626c 6520 2b20   hiervariable + 
+0006d600: 222d 2a77 6964 652e 6373 7622 2029 2029  "-*wide.csv" ) )
+0006d610: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
+0006d620: 2068 6965 7266 6e20 2920 3e20 303a 0a20   hierfn ) > 0:. 
+0006d630: 2020 2020 2020 2020 2020 2068 6466 3d74             hdf=t
+0006d640: 3164 663d 6474 6466 3d72 7364 663d 7065  1df=dtdf=rsdf=pe
+0006d650: 7266 6466 3d6e 6d64 663d 666c 6169 7264  rfdf=nmdf=flaird
+0006d660: 663d 4e6f 6e65 0a20 2020 2020 2020 2020  f=None.         
+0006d670: 2020 2069 6620 7665 7262 6f73 653a 0a20     if verbose:. 
+0006d680: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0006d690: 7269 6e74 2868 6965 7266 6e29 0a20 2020  rint(hierfn).   
+0006d6a0: 2020 2020 2020 2020 2068 6466 203d 2070           hdf = p
+0006d6b0: 642e 7265 6164 5f63 7376 2868 6965 7266  d.read_csv(hierf
+0006d6c0: 6e5b 305d 290a 2020 2020 2020 2020 2020  n[0]).          
+0006d6d0: 2020 6261 646e 616d 6573 203d 2067 6574    badnames = get
+0006d6e0: 5f6e 616d 6573 5f66 726f 6d5f 6461 7461  _names_from_data
+0006d6f0: 5f66 7261 6d65 2820 5b27 556e 6e61 6d65  _frame( ['Unname
+0006d700: 6427 5d2c 2068 6466 2029 0a20 2020 2020  d'], hdf ).     
+0006d710: 2020 2020 2020 2068 6466 3d68 6466 2e64         hdf=hdf.d
+0006d720: 726f 7028 6261 646e 616d 6573 2c20 6178  rop(badnames, ax
+0006d730: 6973 3d31 290a 2020 2020 2020 2020 2020  is=1).          
+0006d740: 2020 6e75 6d73 203d 205b 6973 696e 7374    nums = [isinst
+0006d750: 616e 6365 2868 6466 5b63 6f6c 5d2e 696c  ance(hdf[col].il
+0006d760: 6f63 5b30 5d2c 2028 696e 742c 2066 6c6f  oc[0], (int, flo
+0006d770: 6174 2929 2066 6f72 2063 6f6c 2069 6e20  at)) for col in 
+0006d780: 6864 662e 636f 6c75 6d6e 735d 0a20 2020  hdf.columns].   
+0006d790: 2020 2020 2020 2020 2063 6f72 656e 616d           corenam
+0006d7a0: 6573 203d 206c 6973 7428 6e70 2e61 7272  es = list(np.arr
+0006d7b0: 6179 2868 6466 2e63 6f6c 756d 6e73 295b  ay(hdf.columns)[
+0006d7c0: 6e75 6d73 5d29 0a20 2020 2020 2020 2020  nums]).         
+0006d7d0: 2020 2068 6466 2e6c 6f63 5b3a 2c20 6e75     hdf.loc[:, nu
+0006d7e0: 6d73 5d20 3d20 6864 662e 6c6f 635b 3a2c  ms] = hdf.loc[:,
+0006d7f0: 206e 756d 735d 2e61 6464 5f70 7265 6669   nums].add_prefi
+0006d800: 7828 2254 3148 6965 725f 2229 0a20 2020  x("T1Hier_").   
+0006d810: 2020 2020 2020 2020 206d 7963 7420 3d20           myct = 
+0006d820: 6d79 6374 202b 2031 0a20 2020 2020 2020  myct + 1.       
+0006d830: 2020 2020 2064 666c 6973 7420 3d20 5b68       dflist = [h
+0006d840: 6466 5d0a 0a20 2020 2020 2020 2020 2020  df]..           
+0006d850: 2066 6f72 206d 796d 6f64 2069 6e20 7661   for mymod in va
+0006d860: 6c69 645f 6d6f 6461 6c69 7469 6573 3a0a  lid_modalities:.
+0006d870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0006d880: 7431 7766 6e20 3d20 736f 7274 6564 2867  t1wfn = sorted(g
+0006d890: 6c6f 6228 2070 6174 685f 7465 6d70 6c61  lob( path_templa
+0006d8a0: 7465 2b20 222d 2220 2b20 6d79 6d6f 6420  te+ "-" + mymod 
+0006d8b0: 2b20 222d 2a77 6964 652e 6373 7622 2029  + "-*wide.csv" )
+0006d8c0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+0006d8d0: 2020 2069 6620 6c65 6e28 2074 3177 666e     if len( t1wfn
+0006d8e0: 2029 203e 2030 203a 0a20 2020 2020 2020   ) > 0 :.       
+0006d8f0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0006d900: 7665 7262 6f73 653a 0a20 2020 2020 2020  verbose:.       
+0006d910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0006d920: 2070 7269 6e74 2874 3177 666e 290a 2020   print(t1wfn).  
+0006d930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0006d940: 2020 7431 6466 203d 206d 7972 6561 645f    t1df = myread_
+0006d950: 6373 7628 7431 7766 6e5b 305d 2c20 636f  csv(t1wfn[0], co
+0006d960: 7265 6e61 6d65 7329 0a20 2020 2020 2020  renames).       
+0006d970: 2020 2020 2020 2020 2020 2020 2074 3164               t1d
+0006d980: 6620 3d20 6669 6c74 6572 5f64 6628 2074  f = filter_df( t
+0006d990: 3164 662c 206d 796d 6f64 2b27 5f27 290a  1df, mymod+'_').
+0006d9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0006d9b0: 2020 2020 6466 6c69 7374 203d 2064 666c      dflist = dfl
+0006d9c0: 6973 7420 2b20 5b74 3164 665d 0a20 2020  ist + [t1df].   
+0006d9d0: 2020 2020 2020 2020 2020 2020 200a 2020               .  
+0006d9e0: 2020 2020 2020 2020 2020 6864 6620 3d20            hdf = 
+0006d9f0: 7064 2e63 6f6e 6361 7428 2064 666c 6973  pd.concat( dflis
+0006da00: 742c 2061 7869 733d 312c 2069 676e 6f72  t, axis=1, ignor
+0006da10: 655f 696e 6465 783d 4661 6c73 6520 290a  e_index=False ).
+0006da20: 2020 2020 2020 2020 2020 2020 6966 2076              if v
+0006da30: 6572 626f 7365 3a0a 2020 2020 2020 2020  erbose:.        
+0006da40: 2020 2020 2020 2020 7072 696e 7428 2064          print( d
+0006da50: 662e 6c6f 635b 6c6f 6369 6e64 2c27 6669  f.loc[locind,'fi
+0006da60: 6c65 6e61 6d65 275d 2029 0a20 2020 2020  lename'] ).     
+0006da70: 2020 2020 2020 2069 6620 6d79 6374 203d         if myct =
+0006da80: 3d20 313a 0a20 2020 2020 2020 2020 2020  = 1:.           
+0006da90: 2020 2020 2073 7562 6466 203d 2064 662e       subdf = df.
+0006daa0: 696c 6f63 5b5b 785d 5d0a 2020 2020 2020  iloc[[x]].      
+0006dab0: 2020 2020 2020 2020 2020 6864 662e 696e            hdf.in
+0006dac0: 6465 7820 3d20 7375 6264 662e 696e 6465  dex = subdf.inde
+0006dad0: 782e 636f 7079 2829 0a20 2020 2020 2020  x.copy().       
+0006dae0: 2020 2020 2020 2020 2064 6620 3d20 7064           df = pd
+0006daf0: 2e63 6f6e 6361 7428 205b 6466 2c68 6466  .concat( [df,hdf
+0006db00: 5d2c 2061 7869 733d 312c 2069 676e 6f72  ], axis=1, ignor
+0006db10: 655f 696e 6465 783d 4661 6c73 6520 290a  e_index=False ).
+0006db20: 2020 2020 2020 2020 2020 2020 656c 7365              else
+0006db30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0006db40: 2020 636f 6d6d 636f 6c73 203d 206c 6973    commcols = lis
+0006db50: 7428 7365 7428 6864 662e 636f 6c75 6d6e  t(set(hdf.column
+0006db60: 7329 2e69 6e74 6572 7365 6374 696f 6e28  s).intersection(
+0006db70: 6466 2e63 6f6c 756d 6e73 2929 0a20 2020  df.columns)).   
+0006db80: 2020 2020 2020 2020 2020 2020 2064 662e               df.
+0006db90: 6c6f 635b 6c6f 6369 6e64 2c20 636f 6d6d  loc[locind, comm
+0006dba0: 636f 6c73 5d20 3d20 6864 662e 6c6f 635b  cols] = hdf.loc[
+0006dbb0: 302c 2063 6f6d 6d63 6f6c 735d 0a20 2020  0, commcols].   
+0006dbc0: 2062 6164 6e61 6d65 7320 3d20 6765 745f   badnames = get_
+0006dbd0: 6e61 6d65 735f 6672 6f6d 5f64 6174 615f  names_from_data_
+0006dbe0: 6672 616d 6528 205b 2755 6e6e 616d 6564  frame( ['Unnamed
+0006dbf0: 275d 2c20 6466 2029 0a20 2020 2064 663d  '], df ).    df=
+0006dc00: 6466 2e64 726f 7028 6261 646e 616d 6573  df.drop(badnames
+0006dc10: 2c20 6178 6973 3d31 290a 2020 2020 7265  , axis=1).    re
+0006dc20: 7475 726e 2820 6466 2029 0a0a 6465 6620  turn( df )..def 
+0006dc30: 6669 6e64 5f6d 6f73 745f 7265 6365 6e74  find_most_recent
+0006dc40: 5f66 696c 6528 6669 6c65 5f6c 6973 7429  _file(file_list)
+0006dc50: 3a0a 2020 2020 2222 220a 2020 2020 4669  :.    """.    Fi
+0006dc60: 6e64 7320 616e 6420 7265 7475 726e 7320  nds and returns 
+0006dc70: 7468 6520 6d6f 7374 2072 6563 656e 746c  the most recentl
+0006dc80: 7920 6d6f 6469 6669 6564 2066 696c 6520  y modified file 
+0006dc90: 6672 6f6d 2061 206c 6973 7420 6f66 2066  from a list of f
+0006dca0: 696c 6520 7061 7468 732e 0a20 2020 200a  ile paths..    .
+0006dcb0: 2020 2020 5061 7261 6d65 7465 7273 3a0a      Parameters:.
+0006dcc0: 2020 2020 2d20 6669 6c65 5f6c 6973 743a      - file_list:
+0006dcd0: 2041 206c 6973 7420 6f66 2073 7472 696e   A list of strin
+0006dce0: 6773 2c20 7768 6572 6520 6561 6368 2073  gs, where each s
+0006dcf0: 7472 696e 6720 6973 2061 2070 6174 6820  tring is a path 
+0006dd00: 746f 2061 2066 696c 652e 0a20 2020 200a  to a file..    .
+0006dd10: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+0006dd20: 202d 2054 6865 2070 6174 6820 746f 2074   - The path to t
+0006dd30: 6865 206d 6f73 7420 7265 6365 6e74 6c79  he most recently
+0006dd40: 206d 6f64 6966 6965 6420 6669 6c65 2069   modified file i
+0006dd50: 6e20 7468 6520 6c69 7374 2c20 6f72 204e  n the list, or N
+0006dd60: 6f6e 6520 6966 2074 6865 206c 6973 7420  one if the list 
+0006dd70: 6973 2065 6d70 7479 206f 7220 636f 6e74  is empty or cont
+0006dd80: 6169 6e73 206e 6f20 7661 6c69 6420 6669  ains no valid fi
+0006dd90: 6c65 732e 0a20 2020 2022 2222 0a20 2020  les..    """.   
+0006dda0: 2023 2046 696c 7465 7220 6f75 7420 6974   # Filter out it
+0006ddb0: 656d 7320 7468 6174 2061 7265 206e 6f74  ems that are not
+0006ddc0: 2066 696c 6573 206f 7220 646f 206e 6f74   files or do not
+0006ddd0: 2065 7869 7374 0a20 2020 2076 616c 6964   exist.    valid
+0006dde0: 5f66 696c 6573 203d 205b 6620 666f 7220  _files = [f for 
+0006ddf0: 6620 696e 2066 696c 655f 6c69 7374 2069  f in file_list i
+0006de00: 6620 6f73 2e70 6174 682e 6973 6669 6c65  f os.path.isfile
+0006de10: 2866 295d 0a20 2020 200a 2020 2020 2320  (f)].    .    # 
+0006de20: 4368 6563 6b20 6966 2074 6865 2066 696c  Check if the fil
+0006de30: 7465 7265 6420 6c69 7374 2069 7320 6e6f  tered list is no
+0006de40: 7420 656d 7074 790a 2020 2020 6966 2076  t empty.    if v
+0006de50: 616c 6964 5f66 696c 6573 3a0a 2020 2020  alid_files:.    
+0006de60: 2020 2020 2320 4669 6e64 2074 6865 2066      # Find the f
+0006de70: 696c 6520 7769 7468 2074 6865 206c 6174  ile with the lat
+0006de80: 6573 7420 6d6f 6469 6669 6361 7469 6f6e  est modification
+0006de90: 2074 696d 650a 2020 2020 2020 2020 6d6f   time.        mo
+0006dea0: 7374 5f72 6563 656e 745f 6669 6c65 203d  st_recent_file =
+0006deb0: 206d 6178 2876 616c 6964 5f66 696c 6573   max(valid_files
+0006dec0: 2c20 6b65 793d 6f73 2e70 6174 682e 6765  , key=os.path.ge
+0006ded0: 746d 7469 6d65 290a 2020 2020 2020 2020  tmtime).        
+0006dee0: 7265 7475 726e 205b 6d6f 7374 5f72 6563  return [most_rec
+0006def0: 656e 745f 6669 6c65 5d0a 2020 2020 656c  ent_file].    el
+0006df00: 7365 3a0a 2020 2020 2020 2020 7265 7475  se:.        retu
+0006df10: 726e 204e 6f6e 650a 2020 2020 0a64 6566  rn None.    .def
+0006df20: 2061 6767 7265 6761 7465 5f61 6e74 7370   aggregate_antsp
+0006df30: 796d 6d5f 7265 7375 6c74 735f 7364 6628  ymm_results_sdf(
+0006df40: 0a20 2020 2073 7475 6479 5f64 662c 200a  .    study_df, .
+0006df50: 2020 2020 7072 6f6a 6563 745f 636f 6c3d      project_col=
+0006df60: 2770 726f 6a65 6374 4944 272c 0a20 2020  'projectID',.   
+0006df70: 2073 7562 6a65 6374 5f63 6f6c 3d27 7375   subject_col='su
+0006df80: 626a 6563 7449 4427 2c20 0a20 2020 2064  bjectID', .    d
+0006df90: 6174 655f 636f 6c3d 2764 6174 6527 2c20  ate_col='date', 
+0006dfa0: 0a20 2020 2069 6d61 6765 5f63 6f6c 3d27  .    image_col='
+0006dfb0: 696d 6167 6549 4427 2c20 0a20 2020 2062  imageID', .    b
+0006dfc0: 6173 655f 7061 7468 3d22 2e2f 222c 200a  ase_path="./", .
+0006dfd0: 2020 2020 6869 6572 7661 7269 6162 6c65      hiervariable
+0006dfe0: 3d27 5431 7748 6965 7261 7263 6869 6361  ='T1wHierarchica
+0006dff0: 6c27 2c20 0a20 2020 2073 706c 6974 7365  l', .    splitse
+0006e000: 703d 272d 272c 0a20 2020 2069 6473 6570  p='-',.    idsep
+0006e010: 3d27 2d27 2c0a 2020 2020 7769 6c64 5f63  ='-',.    wild_c
+0006e020: 6172 645f 6d6f 6461 6c69 7479 5f69 643d  ard_modality_id=
+0006e030: 4661 6c73 652c 0a20 2020 2076 6572 626f  False,.    verbo
+0006e040: 7365 3d46 616c 7365 2029 3a0a 2020 2020  se=False ):.    
+0006e050: 2222 220a 2020 2020 4167 6772 6567 6174  """.    Aggregat
+0006e060: 6520 414e 5473 5079 4d4d 2072 6573 756c  e ANTsPyMM resul
+0006e070: 7473 2066 726f 6d20 7468 6520 7370 6563  ts from the spec
+0006e080: 6966 6965 6420 7374 7564 7920 6461 7461  ified study data
+0006e090: 2066 7261 6d65 2061 6e64 2073 746f 7265   frame and store
+0006e0a0: 2074 6865 2061 6767 7265 6761 7465 6420   the aggregated 
+0006e0b0: 7265 7375 6c74 7320 696e 2061 206e 6577  results in a new
+0006e0c0: 2064 6174 6120 6672 616d 652e 2020 5468   data frame.  Th
+0006e0d0: 6973 2061 7373 756d 6573 2064 6174 6120  is assumes data 
+0006e0e0: 6973 206f 7267 616e 697a 6564 206f 6e20  is organized on 
+0006e0f0: 6469 736b 200a 2020 2020 6173 2066 6f6c  disk .    as fol
+0006e100: 6c6f 7773 3a20 2072 6f6f 7464 6972 2f70  lows:  rootdir/p
+0006e110: 726f 6a65 6374 4944 2f73 7562 6a65 6374  rojectID/subject
+0006e120: 4944 2f64 6174 652f 6f75 7470 7574 6964  ID/date/outputid
+0006e130: 2f69 6d61 6765 6964 2f20 7768 6572 6520  /imageid/ where 
+0006e140: 0a20 2020 206f 7574 7075 7469 6420 6973  .    outputid is
+0006e150: 206d 6f64 616c 6974 792d 7370 6563 6966   modality-specif
+0006e160: 6963 2061 6e64 2063 7265 6174 6564 2062  ic and created b
+0006e170: 7920 414e 5473 5079 4d4d 2070 726f 6365  y ANTsPyMM proce
+0006e180: 7373 696e 672e 0a0a 2020 2020 5061 7261  ssing...    Para
+0006e190: 6d65 7465 7273 3a0a 2020 2020 2d20 7374  meters:.    - st
+0006e1a0: 7564 795f 6466 2028 7061 6e64 6173 2064  udy_df (pandas d
+0006e1b0: 6629 3a20 7061 6e64 6173 2064 6174 6120  f): pandas data 
+0006e1c0: 6672 616d 652c 206f 7574 7075 7420 6f66  frame, output of
+0006e1d0: 2067 656e 6572 6174 655f 6d6d 5f64 6174   generate_mm_dat
+0006e1e0: 6166 7261 6d65 2e0a 2020 2020 2d20 7072  aframe..    - pr
+0006e1f0: 6f6a 6563 745f 636f 6c20 2873 7472 293a  oject_col (str):
+0006e200: 204e 616d 6520 6f66 2074 6865 2063 6f6c   Name of the col
+0006e210: 756d 6e20 7468 6174 2073 746f 7265 7320  umn that stores 
+0006e220: 7468 6520 7072 6f6a 6563 7420 4944 0a20  the project ID. 
+0006e230: 2020 202d 2073 7562 6a65 6374 5f63 6f6c     - subject_col
+0006e240: 2028 7374 7229 3a20 4e61 6d65 206f 6620   (str): Name of 
+0006e250: 7468 6520 636f 6c75 6d6e 2074 6f20 7374  the column to st
+0006e260: 6f72 6520 7375 626a 6563 7420 4944 732e  ore subject IDs.
+0006e270: 0a20 2020 202d 2064 6174 655f 636f 6c20  .    - date_col 
+0006e280: 2873 7472 293a 204e 616d 6520 6f66 2074  (str): Name of t
+0006e290: 6865 2063 6f6c 756d 6e20 746f 2073 746f  he column to sto
+0006e2a0: 7265 2064 6174 6520 696e 666f 726d 6174  re date informat
+0006e2b0: 696f 6e2e 0a20 2020 202d 2069 6d61 6765  ion..    - image
+0006e2c0: 5f63 6f6c 2028 7374 7229 3a20 4e61 6d65  _col (str): Name
+0006e2d0: 206f 6620 7468 6520 636f 6c75 6d6e 2074   of the column t
+0006e2e0: 6f20 7374 6f72 6520 696d 6167 6520 4944  o store image ID
+0006e2f0: 732e 0a20 2020 202d 2062 6173 655f 7061  s..    - base_pa
+0006e300: 7468 2028 7374 7229 3a20 4261 7365 2070  th (str): Base p
+0006e310: 6174 6820 666f 7220 7365 6172 6368 696e  ath for searchin
+0006e320: 6720 666f 7220 7072 6f63 6573 7369 6e67  g for processing
+0006e330: 206f 7574 7075 7473 206f 6620 414e 5473   outputs of ANTs
+0006e340: 5079 4d4d 2e0a 2020 2020 2d20 6869 6572  PyMM..    - hier
+0006e350: 7661 7269 6162 6c65 2028 7374 7229 203a  variable (str) :
+0006e360: 2074 6865 2073 7472 696e 6720 7661 7269   the string vari
+0006e370: 6162 6c65 2064 656e 6f74 696e 6720 7468  able denoting th
+0006e380: 6520 4869 6572 6172 6368 6963 616c 206f  e Hierarchical o
+0006e390: 7574 7075 740a 2020 2020 2d20 7370 6c69  utput.    - spli
+0006e3a0: 7473 6570 2028 7374 7229 3a20 2074 6865  tsep (str):  the
+0006e3b0: 2073 6570 6172 6174 6f72 2075 7365 6420   separator used 
+0006e3c0: 746f 2073 706c 6974 2074 6865 2066 696c  to split the fil
+0006e3d0: 656e 616d 650a 2020 2020 2d20 6964 7365  ename.    - idse
+0006e3e0: 7020 2873 7472 293a 2074 6865 2073 6570  p (str): the sep
+0006e3f0: 6172 6174 6f72 2075 7365 6420 746f 2070  arator used to p
+0006e400: 6172 7469 7469 6f6e 2073 7562 6a65 6374  artition subject
+0006e410: 6964 2064 6174 6520 616e 6420 696d 6167  id date and imag
+0006e420: 6569 6420 0a20 2020 2020 2020 2066 6f72  eid .        for
+0006e430: 2065 7861 6d70 6c65 2c20 6966 2069 6473   example, if ids
+0006e440: 6570 2069 7320 2d20 7468 656e 2077 6520  ep is - then we 
+0006e450: 6861 7665 2073 7562 6a65 6374 6964 2d64  have subjectid-d
+0006e460: 6174 652d 696d 6167 6569 640a 2020 2020  ate-imageid.    
+0006e470: 2d20 7769 6c64 5f63 6172 645f 6d6f 6461  - wild_card_moda
+0006e480: 6c69 7479 5f69 6420 2862 6f6f 6c29 3a20  lity_id (bool): 
+0006e490: 6b65 6570 2069 6620 4661 6c73 6520 666f  keep if False fo
+0006e4a0: 7220 7361 6665 7220 6578 6563 7574 696f  r safer executio
+0006e4b0: 6e0a 2020 2020 2d20 7665 7262 6f73 6520  n.    - verbose 
+0006e4c0: 3a20 626f 6f6c 6561 6e0a 0a20 2020 204e  : boolean..    N
+0006e4d0: 6f74 653a 0a20 2020 2054 6869 7320 6675  ote:.    This fu
+0006e4e0: 6e63 7469 6f6e 2069 7320 7465 7374 6564  nction is tested
+0006e4f0: 2075 6e64 6572 206c 696d 6974 6564 2063   under limited c
+0006e500: 6972 6375 6d73 7461 6e63 6573 2e20 5573  ircumstances. Us
+0006e510: 6520 7769 7468 2063 6175 7469 6f6e 2e0a  e with caution..
+0006e520: 2020 2020 4f6e 6520 7061 7274 6963 756c      One particul
+0006e530: 6172 2067 6f74 6368 6120 6973 2069 6620  ar gotcha is if 
+0006e540: 7468 6520 696d 6167 6549 4420 6973 2073  the imageID is s
+0006e550: 746f 7265 6420 6173 2061 206e 756d 6572  tored as a numer
+0006e560: 6963 2076 616c 7565 2069 6e20 7468 6520  ic value in the 
+0006e570: 6461 7461 6672 616d 6520 0a20 2020 2062  dataframe .    b
+0006e580: 7574 2069 7320 6d65 616e 7420 746f 2062  ut is meant to b
+0006e590: 6520 6120 7374 7269 6e67 2e20 2045 2e67  e a string.  E.g
+0006e5a0: 2e20 2730 3030 2720 2873 7472 696e 6729  . '000' (string)
+0006e5b0: 2077 6f75 6c64 2062 6520 696e 7465 7270   would be interp
+0006e5c0: 7265 7465 6420 6173 2030 2069 6e20 7468  reted as 0 in th
+0006e5d0: 6520 0a20 2020 2066 696c 6520 6e61 6d65  e .    file name
+0006e5e0: 2067 6c6f 622e 2020 5468 6973 2077 6f75   glob.  This wou
+0006e5f0: 6c64 206d 6973 7320 7468 6520 6578 7461  ld miss the exta
+0006e600: 6e74 2028 6f6e 2064 6973 6b29 2063 7376  nt (on disk) csv
+0006e610: 2e0a 0a20 2020 2045 7861 6d70 6c65 2075  ...    Example u
+0006e620: 7361 6765 3a0a 2020 2020 6167 675f 6466  sage:.    agg_df
+0006e630: 203d 2061 6767 7265 6761 7465 5f61 6e74   = aggregate_ant
+0006e640: 7370 796d 6d5f 7265 7375 6c74 735f 7364  spymm_results_sd
+0006e650: 6628 2073 7475 6479 6466 2c20 7375 626a  f( studydf, subj
+0006e660: 6563 745f 636f 6c3d 2773 7562 6a65 6374  ect_col='subject
+0006e670: 4944 272c 2064 6174 655f 636f 6c3d 2764  ID', date_col='d
+0006e680: 6174 6527 2c20 696d 6167 655f 636f 6c3d  ate', image_col=
+0006e690: 2769 6d61 6765 4944 272c 2062 6173 655f  'imageID', base_
+0006e6a0: 7061 7468 3d22 2e2f 596f 7572 2f43 7573  path="./Your/Cus
+0006e6b0: 746f 6d2f 5061 7468 2f22 290a 0a20 2020  tom/Path/")..   
+0006e6c0: 2041 7574 686f 723a 0a20 2020 2041 7661   Author:.    Ava
+0006e6d0: 6e74 7320 616e 6420 4368 6174 4750 540a  nts and ChatGPT.
+0006e6e0: 2020 2020 2222 220a 2020 2020 696d 706f      """.    impo
+0006e6f0: 7274 2070 616e 6461 7320 6173 2070 640a  rt pandas as pd.
+0006e700: 2020 2020 696d 706f 7274 206e 756d 7079      import numpy
+0006e710: 2061 7320 6e70 0a20 2020 2066 726f 6d20   as np.    from 
+0006e720: 676c 6f62 2069 6d70 6f72 7420 676c 6f62  glob import glob
+0006e730: 0a0a 2020 2020 6465 6620 7072 6f67 7265  ..    def progre
+0006e740: 7373 5f72 6570 6f72 7465 7228 6375 7272  ss_reporter(curr
+0006e750: 656e 745f 7374 6570 2c20 746f 7461 6c5f  ent_step, total_
+0006e760: 7374 6570 732c 2077 6964 7468 3d35 3029  steps, width=50)
+0006e770: 3a0a 2020 2020 2020 2020 2320 4361 6c63  :.        # Calc
+0006e780: 756c 6174 6520 7468 6520 7072 6f70 6f72  ulate the propor
+0006e790: 7469 6f6e 206f 6620 7072 6f67 7265 7373  tion of progress
+0006e7a0: 0a20 2020 2020 2020 2070 726f 6772 6573  .        progres
+0006e7b0: 7320 3d20 6375 7272 656e 745f 7374 6570  s = current_step
+0006e7c0: 202f 2074 6f74 616c 5f73 7465 7073 0a20   / total_steps. 
+0006e7d0: 2020 2020 2020 2023 2043 616c 6375 6c61         # Calcula
+0006e7e0: 7465 2074 6865 206e 756d 6265 7220 6f66  te the number of
+0006e7f0: 2027 6669 6c6c 6564 2720 6368 6172 6163   'filled' charac
+0006e800: 7465 7273 2069 6e20 7468 6520 7072 6f67  ters in the prog
+0006e810: 7265 7373 2062 6172 0a20 2020 2020 2020  ress bar.       
+0006e820: 2066 696c 6c65 645f 6c65 6e67 7468 203d   filled_length =
+0006e830: 2069 6e74 2877 6964 7468 202a 2070 726f   int(width * pro
+0006e840: 6772 6573 7329 0a20 2020 2020 2020 2023  gress).        #
+0006e850: 2043 7265 6174 6520 7468 6520 7072 6f67   Create the prog
+0006e860: 7265 7373 2062 6172 2073 7472 696e 670a  ress bar string.
+0006e870: 2020 2020 2020 2020 6261 7220 3d20 27e2          bar = '.
+0006e880: 9688 2720 2a20 6669 6c6c 6564 5f6c 656e  ..' * filled_len
+0006e890: 6774 6820 2b20 272d 2720 2a20 2877 6964  gth + '-' * (wid
+0006e8a0: 7468 202d 2066 696c 6c65 645f 6c65 6e67  th - filled_leng
+0006e8b0: 7468 290a 2020 2020 2020 2020 2320 5072  th).        # Pr
+0006e8c0: 696e 7420 7468 6520 7072 6f67 7265 7373  int the progress
+0006e8d0: 2062 6172 2077 6974 6820 7065 7263 656e   bar with percen
+0006e8e0: 7461 6765 0a20 2020 2020 2020 2070 7269  tage.        pri
+0006e8f0: 6e74 2866 275c 7250 726f 6772 6573 733a  nt(f'\rProgress:
+0006e900: 207c 7b62 6172 7d7c 207b 696e 7428 3130   |{bar}| {int(10
+0006e910: 3020 2a20 7072 6f67 7265 7373 297d 2527  0 * progress)}%'
+0006e920: 2c20 656e 643d 275c 7227 290a 2020 2020  , end='\r').    
+0006e930: 2020 2020 2320 5072 696e 7420 6120 6e65      # Print a ne
+0006e940: 7720 6c69 6e65 2077 6865 6e20 7468 6520  w line when the 
+0006e950: 7072 6f67 7265 7373 2069 7320 636f 6d70  progress is comp
+0006e960: 6c65 7465 0a20 2020 2020 2020 2069 6620  lete.        if 
+0006e970: 6375 7272 656e 745f 7374 6570 203d 3d20  current_step == 
+0006e980: 746f 7461 6c5f 7374 6570 733a 0a20 2020  total_steps:.   
+0006e990: 2020 2020 2020 2020 2070 7269 6e74 2829           print()
+0006e9a0: 0a0a 2020 2020 6465 6620 6d79 7265 6164  ..    def myread
+0006e9b0: 5f63 7376 2878 2c20 636e 6d73 293a 0a20  _csv(x, cnms):. 
+0006e9c0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0006e9d0: 2020 2052 6561 6473 2061 2043 5356 2066     Reads a CSV f
+0006e9e0: 696c 6520 616e 6420 7265 7475 726e 7320  ile and returns 
+0006e9f0: 6120 4461 7461 4672 616d 6520 6578 636c  a DataFrame excl
+0006ea00: 7564 696e 6720 7370 6563 6966 6965 6420  uding specified 
+0006ea10: 636f 6c75 6d6e 732e 0a0a 2020 2020 2020  columns...      
+0006ea20: 2020 5061 7261 6d65 7465 7273 3a0a 2020    Parameters:.  
+0006ea30: 2020 2020 2020 2d20 7820 2873 7472 293a        - x (str):
+0006ea40: 2046 696c 6520 7061 7468 206f 6620 7468   File path of th
+0006ea50: 6520 696e 7075 7420 4353 5620 6669 6c65  e input CSV file
+0006ea60: 2064 6573 6372 6962 696e 6720 7468 6520   describing the 
+0006ea70: 626c 696e 6420 5143 206f 7574 7075 740a  blind QC output.
+0006ea80: 2020 2020 2020 2020 2d20 636e 6d73 2028          - cnms (
+0006ea90: 6c69 7374 293a 204c 6973 7420 6f66 2063  list): List of c
+0006eaa0: 6f6c 756d 6e20 6e61 6d65 7320 746f 2065  olumn names to e
+0006eab0: 7863 6c75 6465 2066 726f 6d20 7468 6520  xclude from the 
+0006eac0: 4461 7461 4672 616d 652e 0a0a 2020 2020  DataFrame...    
+0006ead0: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+0006eae0: 2020 2020 2070 642e 4461 7461 4672 616d       pd.DataFram
+0006eaf0: 653a 2044 6174 6146 7261 6d65 2077 6974  e: DataFrame wit
+0006eb00: 6820 7370 6563 6966 6965 6420 636f 6c75  h specified colu
+0006eb10: 6d6e 7320 6578 636c 7564 6564 2e0a 2020  mns excluded..  
+0006eb20: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0006eb30: 2020 6466 203d 2070 642e 7265 6164 5f63    df = pd.read_c
+0006eb40: 7376 2878 290a 2020 2020 2020 2020 7265  sv(x).        re
+0006eb50: 7475 726e 2064 662e 6c6f 635b 3a2c 207e  turn df.loc[:, ~
+0006eb60: 6466 2e63 6f6c 756d 6e73 2e69 7369 6e28  df.columns.isin(
+0006eb70: 636e 6d73 295d 0a0a 2020 2020 696d 706f  cnms)]..    impo
+0006eb80: 7274 2077 6172 6e69 6e67 730a 2020 2020  rt warnings.    
+0006eb90: 2320 5761 726e 696e 6720 6d65 7373 6167  # Warning messag
+0006eba0: 6520 666f 7220 756e 7465 7374 6564 2066  e for untested f
+0006ebb0: 756e 6374 696f 6e0a 2020 2020 7761 726e  unction.    warn
+0006ebc0: 696e 6773 2e77 6172 6e28 2257 6172 6e69  ings.warn("Warni
+0006ebd0: 6e67 3a20 5468 6973 2066 756e 6374 696f  ng: This functio
+0006ebe0: 6e20 6973 206e 6f74 2077 656c 6c20 7465  n is not well te
+0006ebf0: 7374 6564 2e20 5573 6520 7769 7468 2063  sted. Use with c
+0006ec00: 6175 7469 6f6e 2e22 290a 0a20 2020 2076  aution.")..    v
+0006ec10: 6d6f 6464 6963 7420 3d20 7b7d 0a20 2020  moddict = {}.   
+0006ec20: 2023 2041 6464 206b 6579 2d76 616c 7565   # Add key-value
+0006ec30: 2070 6169 7273 0a20 2020 2076 6d6f 6464   pairs.    vmodd
+0006ec40: 6963 745b 2769 6d61 6765 4944 275d 203d  ict['imageID'] =
+0006ec50: 2027 5431 7727 0a20 2020 2076 6d6f 6464   'T1w'.    vmodd
+0006ec60: 6963 745b 2766 6c61 6972 6964 275d 203d  ict['flairid'] =
+0006ec70: 2027 5432 466c 6169 7227 0a20 2020 2076   'T2Flair'.    v
+0006ec80: 6d6f 6464 6963 745b 2770 6572 6669 6427  moddict['perfid'
+0006ec90: 5d20 3d20 2770 6572 6627 0a20 2020 2076  ] = 'perf'.    v
+0006eca0: 6d6f 6464 6963 745b 2772 7366 6964 3127  moddict['rsfid1'
+0006ecb0: 5d20 3d20 2772 7366 4d52 4927 0a23 2020  ] = 'rsfMRI'.#  
+0006ecc0: 2020 766d 6f64 6469 6374 5b27 7273 6669    vmoddict['rsfi
+0006ecd0: 6432 275d 203d 2027 7273 664d 5249 270a  d2'] = 'rsfMRI'.
+0006ece0: 2020 2020 766d 6f64 6469 6374 5b27 6474      vmoddict['dt
+0006ecf0: 6964 3127 5d20 3d20 2744 5449 270a 2320  id1'] = 'DTI'.# 
+0006ed00: 2020 2076 6d6f 6464 6963 745b 2764 7469     vmoddict['dti
+0006ed10: 6432 275d 203d 2027 4454 4927 0a20 2020  d2'] = 'DTI'.   
+0006ed20: 2076 6d6f 6464 6963 745b 276e 6d69 6431   vmoddict['nmid1
+0006ed30: 275d 203d 2027 4e4d 3244 4d54 270a 2320  '] = 'NM2DMT'.# 
+0006ed40: 2020 2076 6d6f 6464 6963 745b 276e 6d69     vmoddict['nmi
+0006ed50: 6432 275d 203d 2027 4e4d 3244 4d54 270a  d2'] = 'NM2DMT'.
+0006ed60: 0a20 2020 2023 2046 696c 7465 7220 726f  .    # Filter ro
+0006ed70: 7773 2077 6865 7265 206d 6f64 616c 6974  ws where modalit
+0006ed80: 7920 6973 2027 5431 7727 0a20 2020 2064  y is 'T1w'.    d
+0006ed90: 6620 3d20 7374 7564 795f 6466 5b20 7374  f = study_df[ st
+0006eda0: 7564 795f 6466 5b27 6d6f 6461 6c69 7479  udy_df['modality
+0006edb0: 275d 203d 3d20 2754 3177 275d 0a20 2020  '] == 'T1w'].   
+0006edc0: 2062 6164 6e61 6d65 7320 3d20 6765 745f   badnames = get_
+0006edd0: 6e61 6d65 735f 6672 6f6d 5f64 6174 615f  names_from_data_
+0006ede0: 6672 616d 6528 205b 2755 6e6e 616d 6564  frame( ['Unnamed
+0006edf0: 275d 2c20 6466 2029 0a20 2020 2064 663d  '], df ).    df=
+0006ee00: 6466 2e64 726f 7028 6261 646e 616d 6573  df.drop(badnames
+0006ee10: 2c20 6178 6973 3d31 290a 2020 2020 2320  , axis=1).    # 
+0006ee20: 7072 6566 696c 7465 7220 6466 2066 6f72  prefilter df for
+0006ee30: 2064 6174 6120 7468 6174 2065 7869 7374   data that exist
+0006ee40: 730a 2020 2020 6b65 6570 203d 206e 702e  s.    keep = np.
+0006ee50: 7469 6c65 2820 4661 6c73 652c 2064 662e  tile( False, df.
+0006ee60: 7368 6170 655b 305d 2029 0a20 2020 2066  shape[0] ).    f
+0006ee70: 6f72 2078 2069 6e20 7261 6e67 6528 6466  or x in range(df
+0006ee80: 2e73 6861 7065 5b30 5d29 3a0a 2020 2020  .shape[0]):.    
+0006ee90: 2020 2020 6d79 666e 203d 206f 732e 7061      myfn = os.pa
+0006eea0: 7468 2e62 6173 656e 616d 6528 2064 665b  th.basename( df[
+0006eeb0: 2766 696c 656e 616d 6527 5d2e 696c 6f63  'filename'].iloc
+0006eec0: 5b78 5d20 290a 2020 2020 2020 2020 7465  [x] ).        te
+0006eed0: 6d70 203d 206d 7966 6e2e 7370 6c69 7428  mp = myfn.split(
+0006eee0: 2073 706c 6974 7365 7020 290a 2020 2020   splitsep ).    
+0006eef0: 2020 2020 2320 4765 6e65 7261 6c69 7a65      # Generalize
+0006ef00: 6420 7365 6172 6368 2070 6174 6873 0a20  d search paths. 
+0006ef10: 2020 2020 2020 2073 6964 3020 3d20 7374         sid0 = st
+0006ef20: 7228 2074 656d 705b 305d 2029 0a20 2020  r( temp[0] ).   
+0006ef30: 2020 2020 2073 6964 203d 2073 7472 2820       sid = str( 
+0006ef40: 6466 5b73 7562 6a65 6374 5f63 6f6c 5d2e  df[subject_col].
+0006ef50: 696c 6f63 5b78 5d20 290a 2020 2020 2020  iloc[x] ).      
+0006ef60: 2020 6966 2073 6964 3020 213d 2073 6964    if sid0 != sid
+0006ef70: 3a0a 2020 2020 2020 2020 2020 2020 7761  :.            wa
+0006ef80: 726e 696e 6773 2e77 6172 6e28 224f 5554  rnings.warn("OUT
+0006ef90: 4552 3a20 7468 6520 6964 2064 6572 6976  ER: the id deriv
+0006efa0: 6564 2066 726f 6d20 7468 6520 6669 6c65  ed from the file
+0006efb0: 6e61 6d65 2022 202b 2073 6964 202b 2022  name " + sid + "
+0006efc0: 2064 6f65 7320 6e6f 7420 6d61 7463 6820   does not match 
+0006efd0: 7468 6520 6964 2073 746f 7265 6420 696e  the id stored in
+0006efe0: 2074 6865 2064 6174 6120 6672 616d 6520   the data frame 
+0006eff0: 2220 2b20 7369 6420 290a 2020 2020 2020  " + sid ).      
+0006f000: 2020 2020 2020 7761 726e 696e 6773 2e77        warnings.w
+0006f010: 6172 6e28 2022 6669 6c65 6e61 6d65 2069  arn( "filename i
+0006f020: 7320 3a20 2220 2b20 206d 7966 6e20 290a  s : " +  myfn ).
+0006f030: 2020 2020 2020 2020 2020 2020 7761 726e              warn
+0006f040: 696e 6773 2e77 6172 6e28 2022 7369 6420  ings.warn( "sid 
+0006f050: 6973 203a 2022 202b 2073 6964 2029 0a20  is : " + sid ). 
+0006f060: 2020 2020 2020 2020 2020 2077 6172 6e69             warni
+0006f070: 6e67 732e 7761 726e 2820 2278 2069 7320  ngs.warn( "x is 
+0006f080: 3a20 2220 2b20 7374 7228 7829 2029 0a20  : " + str(x) ). 
+0006f090: 2020 2020 2020 206d 7970 726f 6a20 3d20         myproj = 
+0006f0a0: 7374 7228 6466 5b70 726f 6a65 6374 5f63  str(df[project_c
+0006f0b0: 6f6c 5d2e 696c 6f63 5b78 5d29 0a20 2020  ol].iloc[x]).   
+0006f0c0: 2020 2020 206d 7964 6174 6520 3d20 7374       mydate = st
+0006f0d0: 7228 6466 5b64 6174 655f 636f 6c5d 2e69  r(df[date_col].i
+0006f0e0: 6c6f 635b 785d 290a 2020 2020 2020 2020  loc[x]).        
+0006f0f0: 6d79 6964 203d 2073 7472 2864 665b 696d  myid = str(df[im
+0006f100: 6167 655f 636f 6c5d 2e69 6c6f 635b 785d  age_col].iloc[x]
+0006f110: 290a 2020 2020 2020 2020 7061 7468 5f74  ).        path_t
+0006f120: 656d 706c 6174 6520 3d20 6261 7365 5f70  emplate = base_p
+0006f130: 6174 6820 2b20 222f 2220 2b20 6d79 7072  ath + "/" + mypr
+0006f140: 6f6a 202b 2020 222f 2220 2b20 7369 6420  oj +  "/" + sid 
+0006f150: 2b20 222f 2220 2b20 6d79 6461 7465 202b  + "/" + mydate +
+0006f160: 2027 2f27 202b 2068 6965 7276 6172 6961   '/' + hiervaria
+0006f170: 626c 6520 2b20 272f 2720 2b20 7374 7228  ble + '/' + str(
+0006f180: 6d79 6964 2920 2b20 222f 220a 2020 2020  myid) + "/".    
+0006f190: 2020 2020 6869 6572 666e 203d 2073 6f72      hierfn = sor
+0006f1a0: 7465 6428 676c 6f62 2820 7061 7468 5f74  ted(glob( path_t
+0006f1b0: 656d 706c 6174 6520 2b20 222a 2220 2b20  emplate + "*" + 
+0006f1c0: 6869 6572 7661 7269 6162 6c65 202b 2022  hiervariable + "
+0006f1d0: 2a77 6964 652e 6373 7622 2029 2029 0a20  *wide.csv" ) ). 
+0006f1e0: 2020 2020 2020 2069 6620 6c65 6e28 2068         if len( h
+0006f1f0: 6965 7266 6e20 2920 3e20 303a 0a20 2020  ierfn ) > 0:.   
+0006f200: 2020 2020 2020 2020 206b 6565 705b 785d           keep[x]
+0006f210: 3d54 7275 650a 0a20 2020 2064 663d 6466  =True..    df=df
+0006f220: 5b6b 6565 705d 0a0a 2020 2020 6966 206e  [keep]..    if n
+0006f230: 6f74 2064 662e 696e 6465 782e 6973 5f75  ot df.index.is_u
+0006f240: 6e69 7175 653a 0a20 2020 2020 2020 2077  nique:.        w
+0006f250: 6172 6e69 6e67 732e 7761 726e 2822 6461  arnings.warn("da
+0006f260: 7461 2066 7261 6d65 2064 6f65 7320 6e6f  ta frame does no
+0006f270: 7420 6861 7665 2075 6e69 7175 6520 696e  t have unique in
+0006f280: 6469 6365 732e 2020 7765 2074 6865 7265  dices.  we there
+0006f290: 666f 7265 2072 6573 6574 2074 6865 2069  fore reset the i
+0006f2a0: 6e64 6578 2074 6f20 616c 6c6f 7720 7468  ndex to allow th
+0006f2b0: 6520 6675 6e63 7469 6f6e 2074 6f20 636f  e function to co
+0006f2c0: 6e74 696e 7565 206f 6e2e 2220 290a 2020  ntinue on." ).  
+0006f2d0: 2020 2020 2020 6466 203d 2064 662e 7265        df = df.re
+0006f2e0: 7365 745f 696e 6465 7828 290a 0a20 2020  set_index()..   
+0006f2f0: 200a 2020 2020 6966 2076 6572 626f 7365   .    if verbose
+0006f300: 3a0a 2020 2020 2020 2020 7072 696e 7428  :.        print(
+0006f310: 2022 6f72 6967 696e 616c 2069 6e70 7574   "original input
+0006f320: 2068 6164 2073 6861 7065 2022 202b 2073   had shape " + s
+0006f330: 7472 2820 6466 2e73 6861 7065 5b30 5d20  tr( df.shape[0] 
+0006f340: 2920 2b20 2220 2854 3120 6f6e 6c79 2920  ) + " (T1 only) 
+0006f350: 616e 6420 7765 2066 696e 6420 2220 2b20  and we find " + 
+0006f360: 7374 7228 2028 6b65 6570 292e 7375 6d28  str( (keep).sum(
+0006f370: 2920 2920 2b20 2220 7769 7468 2068 6965  ) ) + " with hie
+0006f380: 7261 7263 6869 6361 6c20 6f75 7470 7574  rarchical output
+0006f390: 2064 6566 696e 6564 2062 7920 7661 7269   defined by vari
+0006f3a0: 6162 6c65 3a20 2220 2b20 6869 6572 7661  able: " + hierva
+0006f3b0: 7269 6162 6c65 2029 0a20 2020 2020 2020  riable ).       
+0006f3c0: 2070 7269 6e74 2820 6466 2e73 6861 7065   print( df.shape
+0006f3d0: 2029 0a0a 2020 2020 6466 6f75 7420 3d20   )..    dfout = 
+0006f3e0: 7064 2e44 6174 6146 7261 6d65 2829 0a20  pd.DataFrame(). 
+0006f3f0: 2020 206d 7963 7420 3d20 300a 2020 2020     myct = 0.    
+0006f400: 666f 7220 7820 696e 2072 616e 6765 2820  for x in range( 
+0006f410: 6466 2e73 6861 7065 5b30 5d29 3a0a 2020  df.shape[0]):.  
+0006f420: 2020 2020 2020 6966 2076 6572 626f 7365        if verbose
+0006f430: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
+0006f440: 696e 7428 225c 6e5c 6e2d 2d2d 2d2d 2d2d  int("\n\n-------
+0006f450: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0006f460: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0006f470: 2d2d 2d2d 2d2d 2d2d 2d2d 2229 0a20 2020  ----------").   
+0006f480: 2020 2020 2020 2020 2070 7269 6e74 2866           print(f
+0006f490: 227b 787d 2e2e 2e22 290a 2020 2020 2020  "{x}...").      
+0006f4a0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0006f4b0: 2020 2020 7072 6f67 7265 7373 5f72 6570      progress_rep
+0006f4c0: 6f72 7465 7228 782c 2064 662e 7368 6170  orter(x, df.shap
+0006f4d0: 655b 305d 2c20 7769 6474 683d 3530 3029  e[0], width=500)
+0006f4e0: 0a20 2020 2020 2020 206c 6f63 696e 6420  .        locind 
+0006f4f0: 3d20 6466 2e69 6e64 6578 5b78 5d0a 2020  = df.index[x].  
+0006f500: 2020 2020 2020 6d79 666e 203d 206f 732e        myfn = os.
+0006f510: 7061 7468 2e62 6173 656e 616d 6528 2064  path.basename( d
+0006f520: 665b 2766 696c 656e 616d 6527 5d2e 696c  f['filename'].il
+0006f530: 6f63 5b78 5d20 290a 2020 2020 2020 2020  oc[x] ).        
+0006f540: 7369 6420 3d20 7374 7228 2064 665b 7375  sid = str( df[su
+0006f550: 626a 6563 745f 636f 6c5d 2e69 6c6f 635b  bject_col].iloc[
+0006f560: 785d 2029 0a20 2020 2020 2020 2074 656d  x] ).        tem
+0006f570: 7042 203d 206d 7966 6e2e 7370 6c69 7428  pB = myfn.split(
+0006f580: 2073 706c 6974 7365 7020 290a 2020 2020   splitsep ).    
+0006f590: 2020 2020 7369 6430 203d 2073 7472 2874      sid0 = str(t
+0006f5a0: 656d 7042 5b31 5d29 0a20 2020 2020 2020  empB[1]).       
+0006f5b0: 2069 6620 7369 6430 2021 3d20 7369 6420   if sid0 != sid 
+0006f5c0: 616e 6420 7665 7262 6f73 653a 0a20 2020  and verbose:.   
+0006f5d0: 2020 2020 2020 2020 2077 6172 6e69 6e67           warning
+0006f5e0: 732e 7761 726e 2822 494e 4e45 523a 2074  s.warn("INNER: t
+0006f5f0: 6865 2069 6420 6465 7269 7665 6420 6672  he id derived fr
+0006f600: 6f6d 2074 6865 2066 696c 656e 616d 6520  om the filename 
+0006f610: 2220 2b20 7374 7228 7369 6429 202b 2022  " + str(sid) + "
+0006f620: 2064 6f65 7320 6e6f 7420 6d61 7463 6820   does not match 
+0006f630: 7468 6520 6964 2073 746f 7265 6420 696e  the id stored in
+0006f640: 2074 6865 2064 6174 6120 6672 616d 6520   the data frame 
+0006f650: 2220 2b20 7374 7228 7369 6430 2920 290a  " + str(sid0) ).
+0006f660: 2020 2020 2020 2020 2020 2020 7761 726e              warn
+0006f670: 696e 6773 2e77 6172 6e28 2022 6669 6c65  ings.warn( "file
+0006f680: 6e61 6d65 2069 7320 3a20 2220 2b20 2073  name is : " +  s
+0006f690: 7472 286d 7966 6e29 2029 0a20 2020 2020  tr(myfn) ).     
+0006f6a0: 2020 2020 2020 2077 6172 6e69 6e67 732e         warnings.
+0006f6b0: 7761 726e 2820 2273 6964 2069 7320 3a20  warn( "sid is : 
+0006f6c0: 2220 2b20 7374 7228 7369 6429 2029 0a20  " + str(sid) ). 
+0006f6d0: 2020 2020 2020 2020 2020 2077 6172 6e69             warni
+0006f6e0: 6e67 732e 7761 726e 2820 2278 2069 7320  ngs.warn( "x is 
+0006f6f0: 3a20 2220 2b20 7374 7228 7829 2029 0a20  : " + str(x) ). 
+0006f700: 2020 2020 2020 2020 2020 2077 6172 6e69             warni
+0006f710: 6e67 732e 7761 726e 2820 2269 6e64 6578  ngs.warn( "index
+0006f720: 2069 7320 3a20 2220 2b20 7374 7228 6c6f   is : " + str(lo
+0006f730: 6369 6e64 2920 290a 2020 2020 2020 2020  cind) ).        
+0006f740: 6d79 7072 6f6a 203d 2073 7472 2864 665b  myproj = str(df[
+0006f750: 7072 6f6a 6563 745f 636f 6c5d 2e69 6c6f  project_col].ilo
+0006f760: 635b 785d 290a 2020 2020 2020 2020 6d79  c[x]).        my
+0006f770: 6461 7465 203d 2073 7472 2864 665b 6461  date = str(df[da
+0006f780: 7465 5f63 6f6c 5d2e 696c 6f63 5b78 5d29  te_col].iloc[x])
+0006f790: 0a20 2020 2020 2020 206d 7969 6420 3d20  .        myid = 
+0006f7a0: 7374 7228 6466 5b69 6d61 6765 5f63 6f6c  str(df[image_col
+0006f7b0: 5d2e 696c 6f63 5b78 5d29 0a20 2020 2020  ].iloc[x]).     
+0006f7c0: 2020 206d 7974 3169 6420 3d20 6d79 6964     myt1id = myid
+0006f7d0: 0a20 2020 2020 2020 2069 6620 7665 7262  .        if verb
+0006f7e0: 6f73 653a 0a20 2020 2020 2020 2020 2020  ose:.           
+0006f7f0: 2070 7269 6e74 2820 6d79 666e 2029 0a20   print( myfn ). 
+0006f800: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+0006f810: 2820 7465 6d70 2029 0a20 2020 2020 2020  ( temp ).       
+0006f820: 2020 2020 2070 7269 6e74 2820 2269 6420       print( "id 
+0006f830: 2220 2b20 7369 6420 2029 0a20 2020 2020  " + sid  ).     
+0006f840: 2020 2070 6174 685f 7465 6d70 6c61 7465     path_template
+0006f850: 203d 2062 6173 655f 7061 7468 202b 2022   = base_path + "
+0006f860: 2f22 202b 206d 7970 726f 6a20 2b20 2022  /" + myproj +  "
+0006f870: 2f22 202b 2073 6964 202b 2022 2f22 202b  /" + sid + "/" +
+0006f880: 206d 7964 6174 6520 2b20 272f 2720 2b20   mydate + '/' + 
+0006f890: 6869 6572 7661 7269 6162 6c65 202b 2027  hiervariable + '
+0006f8a0: 2f27 202b 2073 7472 286d 7969 6429 202b  /' + str(myid) +
+0006f8b0: 2022 2f22 0a20 2020 2020 2020 2073 6561   "/".        sea
+0006f8c0: 7263 6868 6965 7220 3d20 7061 7468 5f74  rchhier = path_t
+0006f8d0: 656d 706c 6174 6520 2b20 222a 2220 2b20  emplate + "*" + 
+0006f8e0: 6869 6572 7661 7269 6162 6c65 202b 2022  hiervariable + "
+0006f8f0: 2a77 6964 652e 6373 7622 0a20 2020 2020  *wide.csv".     
+0006f900: 2020 2069 6620 7665 7262 6f73 653a 0a20     if verbose:. 
+0006f910: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+0006f920: 2820 7365 6172 6368 6869 6572 2029 0a20  ( searchhier ). 
+0006f930: 2020 2020 2020 2068 6965 7266 6e20 3d20         hierfn = 
+0006f940: 736f 7274 6564 2820 676c 6f62 2820 7365  sorted( glob( se
+0006f950: 6172 6368 6869 6572 2029 2029 0a20 2020  archhier ) ).   
+0006f960: 2020 2020 2069 6620 6c65 6e28 2068 6965       if len( hie
+0006f970: 7266 6e20 2920 3e20 313a 0a20 2020 2020  rfn ) > 1:.     
+0006f980: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+0006f990: 7565 4572 726f 7228 2274 6865 7265 2061  ueError("there a
+0006f9a0: 7265 2022 202b 2073 7472 2820 6c65 6e28  re " + str( len(
+0006f9b0: 2068 6965 7266 6e20 2920 2920 2b20 2220   hierfn ) ) + " 
+0006f9c0: 6e75 6d62 6572 206f 6620 6869 6572 2066  number of hier f
+0006f9d0: 6e73 2077 6974 6820 7365 6172 6368 2070  ns with search p
+0006f9e0: 6174 6820 2220 2b20 7365 6172 6368 6869  ath " + searchhi
+0006f9f0: 6572 2029 0a20 2020 2020 2020 2069 6620  er ).        if 
+0006fa00: 6c65 6e28 2068 6965 7266 6e20 2920 3d3d  len( hierfn ) ==
+0006fa10: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
+0006fa20: 6864 663d 7431 6466 3d64 7464 663d 7273  hdf=t1df=dtdf=rs
+0006fa30: 6466 3d70 6572 6664 663d 6e6d 6466 3d66  df=perfdf=nmdf=f
+0006fa40: 6c61 6972 6466 3d4e 6f6e 650a 2020 2020  lairdf=None.    
+0006fa50: 2020 2020 2020 2020 6966 2076 6572 626f          if verbo
+0006fa60: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0006fa70: 2020 2020 7072 696e 7428 6869 6572 666e      print(hierfn
+0006fa80: 290a 2020 2020 2020 2020 2020 2020 6864  ).            hd
+0006fa90: 6620 3d20 7064 2e72 6561 645f 6373 7628  f = pd.read_csv(
+0006faa0: 6869 6572 666e 5b30 5d29 0a20 2020 2020  hierfn[0]).     
+0006fab0: 2020 2020 2020 2069 6620 7665 7262 6f73         if verbos
+0006fac0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0006fad0: 2020 2070 7269 6e74 2820 6864 665b 2776     print( hdf['v
+0006fae0: 6f6c 5f68 656d 6973 7068 6572 655f 6c65  ol_hemisphere_le
+0006faf0: 6674 6865 6d69 7370 6865 7265 7327 5d20  fthemispheres'] 
+0006fb00: 290a 2020 2020 2020 2020 2020 2020 6261  ).            ba
+0006fb10: 646e 616d 6573 203d 2067 6574 5f6e 616d  dnames = get_nam
+0006fb20: 6573 5f66 726f 6d5f 6461 7461 5f66 7261  es_from_data_fra
+0006fb30: 6d65 2820 5b27 556e 6e61 6d65 6427 5d2c  me( ['Unnamed'],
+0006fb40: 2068 6466 2029 0a20 2020 2020 2020 2020   hdf ).         
+0006fb50: 2020 2068 6466 3d68 6466 2e64 726f 7028     hdf=hdf.drop(
+0006fb60: 6261 646e 616d 6573 2c20 6178 6973 3d31  badnames, axis=1
+0006fb70: 290a 2020 2020 2020 2020 2020 2020 6e75  ).            nu
+0006fb80: 6d73 203d 205b 6973 696e 7374 616e 6365  ms = [isinstance
+0006fb90: 2868 6466 5b63 6f6c 5d2e 696c 6f63 5b30  (hdf[col].iloc[0
+0006fba0: 5d2c 2028 696e 742c 2066 6c6f 6174 2929  ], (int, float))
+0006fbb0: 2066 6f72 2063 6f6c 2069 6e20 6864 662e   for col in hdf.
+0006fbc0: 636f 6c75 6d6e 735d 0a20 2020 2020 2020  columns].       
+0006fbd0: 2020 2020 2063 6f72 656e 616d 6573 203d       corenames =
+0006fbe0: 206c 6973 7428 6e70 2e61 7272 6179 2868   list(np.array(h
+0006fbf0: 6466 2e63 6f6c 756d 6e73 295b 6e75 6d73  df.columns)[nums
+0006fc00: 5d29 0a20 2020 2020 2020 2020 2020 2023  ]).            #
+0006fc10: 2068 6466 2e6c 6f63 5b3a 2c20 6e75 6d73   hdf.loc[:, nums
+0006fc20: 5d20 3d20 6864 662e 6c6f 635b 3a2c 206e  ] = hdf.loc[:, n
+0006fc30: 756d 735d 2e61 6464 5f70 7265 6669 7828  ums].add_prefix(
+0006fc40: 2254 3148 6965 725f 2229 0a20 2020 2020  "T1Hier_").     
+0006fc50: 2020 2020 2020 2068 6466 203d 2068 6466         hdf = hdf
+0006fc60: 2e61 6464 5f70 7265 6669 7828 2254 3148  .add_prefix("T1H
+0006fc70: 6965 725f 2229 0a20 2020 2020 2020 2020  ier_").         
+0006fc80: 2020 206d 7963 7420 3d20 6d79 6374 202b     myct = myct +
+0006fc90: 2031 0a20 2020 2020 2020 2020 2020 2064   1.            d
+0006fca0: 666c 6973 7420 3d20 5b68 6466 5d0a 0a20  flist = [hdf].. 
+0006fcb0: 2020 2020 2020 2020 2020 2066 6f72 206d             for m
+0006fcc0: 796d 6f64 2069 6e20 766d 6f64 6469 6374  ymod in vmoddict
+0006fcd0: 2e6b 6579 7328 293a 0a20 2020 2020 2020  .keys():.       
+0006fce0: 2020 2020 2020 2020 2069 6620 7665 7262           if verb
+0006fcf0: 6f73 653a 0a20 2020 2020 2020 2020 2020  ose:.           
+0006fd00: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
+0006fd10: 5c6e 5c6e 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  \n\n************
+0006fd20: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a20 2220  ************* " 
+0006fd30: 2b20 6d79 6d6f 6420 2b20 2220 2a2a 2a2a  + mymod + " ****
+0006fd40: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+0006fd50: 2a2a 2a2a 2a22 290a 2020 2020 2020 2020  *****").        
+0006fd60: 2020 2020 2020 2020 6d6f 6461 6c69 7479          modality
+0006fd70: 636c 6173 7320 3d20 766d 6f64 6469 6374  class = vmoddict
+0006fd80: 5b20 6d79 6d6f 6420 5d0a 2020 2020 2020  [ mymod ].      
+0006fd90: 2020 2020 2020 2020 2020 6966 2077 696c            if wil
+0006fda0: 645f 6361 7264 5f6d 6f64 616c 6974 795f  d_card_modality_
+0006fdb0: 6964 3a0a 2020 2020 2020 2020 2020 2020  id:.            
+0006fdc0: 2020 2020 2020 2020 6d79 6d6f 6469 6420          mymodid 
+0006fdd0: 3d20 272a 270a 2020 2020 2020 2020 2020  = '*'.          
+0006fde0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0006fdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0006fe00: 6d79 6d6f 6469 6420 3d20 7374 7228 2064  mymodid = str( d
+0006fe10: 665b 6d79 6d6f 645d 2e69 6c6f 635b 785d  f[mymod].iloc[x]
+0006fe20: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+0006fe30: 2020 2020 2020 2069 6620 6d79 6d6f 6469         if mymodi
+0006fe40: 642e 6c6f 7765 7228 2920 213d 2022 6e61  d.lower() != "na
+0006fe50: 6e22 2061 6e64 206d 796d 6f64 6964 2e6c  n" and mymodid.l
+0006fe60: 6f77 6572 2829 2021 3d20 226e 6122 3a0a  ower() != "na":.
 0006fe70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0006fe80: 2020 2020 2020 206d 796d 6f64 6964 203d         mymodid =
-0006fe90: 2074 656d 705b 206c 656e 2820 7465 6d70   temp[ len( temp
-0006fea0: 2029 2d31 205d 0a20 2020 2020 2020 2020   )-1 ].         
-0006feb0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0006fec0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0006fed0: 2020 2020 2020 2020 2069 6620 7665 7262           if verb
-0006fee0: 6f73 653a 0a20 2020 2020 2020 2020 2020  ose:.           
+0006fe80: 2020 2020 2020 2020 6d79 6d6f 6469 6420          mymodid 
+0006fe90: 3d20 6f73 2e70 6174 682e 6261 7365 6e61  = os.path.basena
+0006fea0: 6d65 2820 6d79 6d6f 6469 6420 290a 2020  me( mymodid ).  
+0006feb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0006fec0: 2020 2020 2020 6d79 6d6f 6469 6420 3d20        mymodid = 
+0006fed0: 6f73 2e70 6174 682e 7370 6c69 7465 7874  os.path.splitext
+0006fee0: 2820 6d79 6d6f 6469 6420 295b 305d 0a20  ( mymodid )[0]. 
 0006fef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0006ff00: 2070 7269 6e74 2822 6d69 7373 696e 6722   print("missing"
-0006ff10: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0006ff20: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
-0006ff30: 7565 0a20 2020 2020 2020 2020 2020 2020  ue.             
-0006ff40: 2020 2069 6620 7665 7262 6f73 653a 0a20     if verbose:. 
-0006ff50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0006ff60: 2020 2070 7269 6e74 2820 226d 6f64 616c     print( "modal
-0006ff70: 6974 7920 6964 2069 7320 2220 2b20 6d79  ity id is " + my
-0006ff80: 6d6f 6469 6420 2b20 2220 666f 7220 6d6f  modid + " for mo
-0006ff90: 6461 6c69 7479 2022 202b 206d 6f64 616c  dality " + modal
-0006ffa0: 6974 7963 6c61 7373 202b 2027 206d 6f64  ityclass + ' mod
-0006ffb0: 616c 6974 7920 7370 6563 6966 6963 2073  ality specific s
-0006ffc0: 7562 6a20 2720 2b20 7369 6420 2b20 2720  ubj ' + sid + ' 
-0006ffd0: 6d6f 6461 6c69 7479 2073 7065 6369 6669  modality specifi
-0006ffe0: 6320 6964 2069 7320 2720 2b20 6d79 6964  c id is ' + myid
-0006fff0: 202b 2022 2069 7473 2064 6174 6520 2220   + " its date " 
-00070000: 2b20 206d 7964 6174 6520 290a 2020 2020  +  mydate ).    
-00070010: 2020 2020 2020 2020 2020 2020 6d6f 6461              moda
-00070020: 6c69 7479 636c 6173 7373 6561 7263 6820  lityclasssearch 
-00070030: 3d20 6d6f 6461 6c69 7479 636c 6173 730a  = modalityclass.
-00070040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00070050: 6966 206d 6f64 616c 6974 7963 6c61 7373  if modalityclass
-00070060: 2069 6e20 5b27 7273 664d 5249 272c 2744   in ['rsfMRI','D
-00070070: 5449 275d 3a0a 2020 2020 2020 2020 2020  TI']:.          
-00070080: 2020 2020 2020 2020 2020 6d6f 6461 6c69            modali
-00070090: 7479 636c 6173 7373 6561 7263 683d 6d6f  tyclasssearch=mo
-000700a0: 6461 6c69 7479 636c 6173 732b 222a 220a  dalityclass+"*".
-000700b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000700c0: 7061 7468 5f74 656d 706c 6174 655f 6d20  path_template_m 
-000700d0: 3d20 6261 7365 5f70 6174 6820 2b20 222f  = base_path + "/
-000700e0: 2220 2b20 6d79 7072 6f6a 202b 2020 222f  " + myproj +  "/
-000700f0: 2220 2b20 7369 6420 2b20 222f 2220 2b20  " + sid + "/" + 
-00070100: 6d79 6461 7465 202b 2027 2f27 202b 206d  mydate + '/' + m
-00070110: 6f64 616c 6974 7963 6c61 7373 7365 6172  odalityclasssear
-00070120: 6368 202b 2027 2f27 202b 206d 796d 6f64  ch + '/' + mymod
-00070130: 6964 202b 2022 2f22 0a20 2020 2020 2020  id + "/".       
-00070140: 2020 2020 2020 2020 206d 6f64 7365 6172           modsear
-00070150: 6368 203d 2070 6174 685f 7465 6d70 6c61  ch = path_templa
-00070160: 7465 5f6d 202b 2022 2a22 202b 206d 6f64  te_m + "*" + mod
-00070170: 616c 6974 7963 6c61 7373 7365 6172 6368  alityclasssearch
-00070180: 202b 2022 2a77 6964 652e 6373 7622 0a20   + "*wide.csv". 
-00070190: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000701a0: 6620 7665 7262 6f73 653a 0a20 2020 2020  f verbose:.     
-000701b0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-000701c0: 7269 6e74 2820 6d6f 6473 6561 7263 6820  rint( modsearch 
-000701d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000701e0: 2020 7431 7766 6e20 3d20 736f 7274 6564    t1wfn = sorted
-000701f0: 2820 676c 6f62 2820 6d6f 6473 6561 7263  ( glob( modsearc
-00070200: 6820 2920 290a 2020 2020 2020 2020 2020  h ) ).          
-00070210: 2020 2020 2020 6966 206c 656e 2820 7431        if len( t1
-00070220: 7766 6e20 2920 3e20 313a 0a20 2020 2020  wfn ) > 1:.     
-00070230: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00070240: 6c61 7267 6520 3d20 6c65 6e28 7431 7766  large = len(t1wf
-00070250: 6e29 0a20 2020 2020 2020 2020 2020 2020  n).             
-00070260: 2020 2020 2020 2074 3177 666e 203d 2066         t1wfn = f
-00070270: 696e 645f 6d6f 7374 5f72 6563 656e 745f  ind_most_recent_
-00070280: 6669 6c65 2820 7431 7766 6e20 290a 2020  file( t1wfn ).  
-00070290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000702a0: 2020 7761 726e 696e 6773 2e77 6172 6e28    warnings.warn(
-000702b0: 2274 6865 7265 2061 7265 2022 202b 2073  "there are " + s
-000702c0: 7472 2820 6e6c 6172 6765 2029 202b 2022  tr( nlarge ) + "
-000702d0: 206e 756d 6265 7220 6f66 2077 6964 6520   number of wide 
-000702e0: 666e 7320 7769 7468 2073 6561 7263 6820  fns with search 
-000702f0: 7061 7468 2022 202b 206d 6f64 7365 6172  path " + modsear
-00070300: 6368 202b 2022 2077 6520 7461 6b65 2074  ch + " we take t
-00070310: 6865 206d 6f73 7420 7265 6365 6e74 206f  he most recent o
-00070320: 6620 7468 6573 6520 2220 2b20 7431 7766  f these " + t1wf
-00070330: 6e5b 305d 2029 0a23 2020 2020 2020 2020  n[0] ).#        
-00070340: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00070350: 6520 5661 6c75 6545 7272 6f72 2822 7468  e ValueError("th
-00070360: 6572 6520 6172 6520 2220 2b20 7374 7228  ere are " + str(
-00070370: 206c 656e 2820 7431 7766 6e20 2920 2920   len( t1wfn ) ) 
-00070380: 2b20 2220 6e75 6d62 6572 206f 6620 7769  + " number of wi
-00070390: 6465 2066 6e73 2077 6974 6820 7365 6172  de fns with sear
-000703a0: 6368 2070 6174 6820 2220 2b20 6d6f 6473  ch path " + mods
-000703b0: 6561 7263 6820 290a 2020 2020 2020 2020  earch ).        
-000703c0: 2020 2020 2020 2020 6966 206c 656e 2820          if len( 
-000703d0: 7431 7766 6e20 2920 3d3d 2031 3a0a 2020  t1wfn ) == 1:.  
-000703e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000703f0: 2020 6966 2076 6572 626f 7365 3a0a 2020    if verbose:.  
-00070400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00070410: 2020 2020 2020 7072 696e 7428 7431 7766        print(t1wf
-00070420: 6e29 0a20 2020 2020 2020 2020 2020 2020  n).             
-00070430: 2020 2020 2020 2074 3164 6620 3d20 6d79         t1df = my
-00070440: 7265 6164 5f63 7376 2874 3177 666e 5b30  read_csv(t1wfn[0
-00070450: 5d2c 2063 6f72 656e 616d 6573 290a 2020  ], corenames).  
-00070460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00070470: 2020 7431 6466 203d 2066 696c 7465 725f    t1df = filter_
-00070480: 6466 2820 7431 6466 2c20 6d6f 6461 6c69  df( t1df, modali
-00070490: 7479 636c 6173 732b 275f 2729 0a20 2020  tyclass+'_').   
-000704a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000704b0: 2064 666c 6973 7420 3d20 6466 6c69 7374   dflist = dflist
-000704c0: 202b 205b 7431 6466 5d0a 2020 2020 2020   + [t1df].      
-000704d0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-000704e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000704f0: 2020 2020 6966 2076 6572 626f 7365 3a0a      if verbose:.
-00070500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00070510: 2020 2020 2020 2020 7072 696e 7428 2022          print( "
-00070520: 2063 616e 6e6f 7420 6669 6e64 2022 202b   cannot find " +
-00070530: 206d 6f64 7365 6172 6368 2029 0a20 2020   modsearch ).   
-00070540: 2020 2020 2020 2020 2020 2020 200a 2020               .  
-00070550: 2020 2020 2020 2020 2020 6864 6620 3d20            hdf = 
-00070560: 7064 2e63 6f6e 6361 7428 2064 666c 6973  pd.concat( dflis
-00070570: 742c 2061 7869 733d 312c 2069 676e 6f72  t, axis=1, ignor
-00070580: 655f 696e 6465 783d 4661 6c73 6529 0a20  e_index=False). 
-00070590: 2020 2020 2020 2020 2020 2069 6620 7665             if ve
-000705a0: 7262 6f73 653a 0a20 2020 2020 2020 2020  rbose:.         
-000705b0: 2020 2020 2020 2070 7269 6e74 2820 2263         print( "c
-000705c0: 6f75 6e74 3a20 2220 2b20 7374 7228 206d  ount: " + str( m
-000705d0: 7963 7420 2920 290a 2020 2020 2020 2020  yct ) ).        
-000705e0: 2020 2020 7375 6264 6620 3d20 6466 2e69      subdf = df.i
-000705f0: 6c6f 635b 5b78 5d5d 0a20 2020 2020 2020  loc[[x]].       
-00070600: 2020 2020 2068 6466 2e69 6e64 6578 203d       hdf.index =
-00070610: 2073 7562 6466 2e69 6e64 6578 2e63 6f70   subdf.index.cop
-00070620: 7928 290a 2020 2020 2020 2020 2020 2020  y().            
-00070630: 7375 6264 6620 3d20 7064 2e63 6f6e 6361  subdf = pd.conca
-00070640: 7428 205b 7375 6264 662c 6864 665d 2c20  t( [subdf,hdf], 
-00070650: 6178 6973 3d31 2c20 6967 6e6f 7265 5f69  axis=1, ignore_i
-00070660: 6e64 6578 3d46 616c 7365 290a 2020 2020  ndex=False).    
-00070670: 2020 2020 2020 2020 6466 6f75 7420 3d20          dfout = 
-00070680: 7064 2e63 6f6e 6361 7428 205b 6466 6f75  pd.concat( [dfou
-00070690: 742c 7375 6264 665d 2c20 6178 6973 3d30  t,subdf], axis=0
-000706a0: 2c20 6967 6e6f 7265 5f69 6e64 6578 3d46  , ignore_index=F
-000706b0: 616c 7365 2029 0a20 2020 2062 6164 6e61  alse ).    badna
-000706c0: 6d65 7320 3d20 6765 745f 6e61 6d65 735f  mes = get_names_
-000706d0: 6672 6f6d 5f64 6174 615f 6672 616d 6528  from_data_frame(
-000706e0: 205b 2755 6e6e 616d 6564 275d 2c20 6466   ['Unnamed'], df
-000706f0: 6f75 7420 290a 2020 2020 6466 6f75 743d  out ).    dfout=
-00070700: 6466 6f75 742e 6472 6f70 2862 6164 6e61  dfout.drop(badna
-00070710: 6d65 732c 2061 7869 733d 3129 0a20 2020  mes, axis=1).   
-00070720: 2072 6574 7572 6e28 2064 666f 7574 2029   return( dfout )
-00070730: 0a0a 6465 6620 656e 616e 7469 6f6d 6f72  ..def enantiomor
-00070740: 7068 6963 5f66 696c 6c69 6e67 5f77 6974  phic_filling_wit
-00070750: 686f 7574 5f6d 6173 6b28 2069 6d61 6765  hout_mask( image
-00070760: 2c20 6178 6973 3d30 2c20 696e 7465 6e73  , axis=0, intens
-00070770: 6974 793d 276c 6f77 2720 293a 0a20 2020  ity='low' ):.   
-00070780: 2022 2222 0a20 2020 2050 6572 666f 726d   """.    Perform
-00070790: 2061 6e20 656e 616e 7469 6f6d 6f72 7068   an enantiomorph
-000707a0: 6963 206c 6573 696f 6e20 6669 6c6c 696e  ic lesion fillin
-000707b0: 6720 6f6e 2061 6e20 696d 6167 6520 7769  g on an image wi
-000707c0: 7468 6f75 7420 6120 6c65 7369 6f6e 206d  thout a lesion m
-000707d0: 6173 6b2e 0a0a 2020 2020 4172 6773 3a0a  ask...    Args:.
-000707e0: 2020 2020 696d 6167 6520 2861 6e74 7349      image (antsI
-000707f0: 6d61 6765 293a 2054 6865 2061 6e74 7320  mage): The ants 
-00070800: 696d 6167 6520 746f 2066 6c69 7020 616e  image to flip an
-00070810: 6420 6669 6c6c 0a20 2020 2061 7869 7320  d fill.    axis 
-00070820: 2820 696e 7420 293a 2074 6865 2061 7869  ( int ): the axi
-00070830: 7320 616c 6f6e 6720 7768 6963 6820 746f  s along which to
-00070840: 2072 6566 6c65 6374 2074 6865 2069 6d61   reflect the ima
-00070850: 6765 0a20 2020 2069 6e74 656e 7369 7479  ge.    intensity
-00070860: 2028 2073 7472 2029 203a 206c 6f77 206f   ( str ) : low o
-00070870: 7220 6869 6768 0a0a 2020 2020 5265 7475  r high..    Retu
-00070880: 726e 733a 0a20 2020 2061 6e74 732e 414e  rns:.    ants.AN
-00070890: 5473 496d 6167 653a 2054 6865 2069 6d61  TsImage: The ima
-000708a0: 6765 2061 6674 6572 2065 6e61 6e74 696f  ge after enantio
-000708b0: 6d6f 7270 6869 6320 6669 6c6c 696e 672e  morphic filling.
-000708c0: 0a20 2020 2022 2222 0a20 2020 2069 6d61  .    """.    ima
-000708d0: 6765 6e20 3d20 616e 7473 2e69 4d61 7468  gen = ants.iMath
-000708e0: 2820 696d 6167 652c 2027 4e6f 726d 616c  ( image, 'Normal
-000708f0: 697a 6527 2029 0a20 2020 2069 6d61 6765  ize' ).    image
-00070900: 6e20 3d20 616e 7473 2e69 4d61 7468 2820  n = ants.iMath( 
-00070910: 696d 6167 656e 2c20 2254 7275 6e63 6174  imagen, "Truncat
-00070920: 6549 6e74 656e 7369 7479 222c 2031 652d  eIntensity", 1e-
-00070930: 362c 2030 2e39 3820 290a 2020 2020 696d  6, 0.98 ).    im
-00070940: 6167 656e 203d 2061 6e74 732e 694d 6174  agen = ants.iMat
-00070950: 6828 2069 6d61 6765 6e2c 2027 4e6f 726d  h( imagen, 'Norm
-00070960: 616c 697a 6527 2029 0a20 2020 2023 2043  alize' ).    # C
-00070970: 7265 6174 6520 6120 6d69 7272 6f72 2069  reate a mirror i
-00070980: 6d61 6765 2028 666c 6970 7069 6e67 206c  mage (flipping l
-00070990: 6566 7420 616e 6420 7269 6768 7429 0a20  eft and right). 
-000709a0: 2020 206d 6972 726f 725f 696d 6167 6520     mirror_image 
-000709b0: 3d20 616e 7473 2e72 6566 6c65 6374 5f69  = ants.reflect_i
-000709c0: 6d61 6765 2869 6d61 6765 6e2c 2061 7869  mage(imagen, axi
-000709d0: 733d 302c 2074 783d 2753 794e 2720 295b  s=0, tx='SyN' )[
-000709e0: 2777 6172 7065 646d 6f76 6f75 7427 5d0a  'warpedmovout'].
-000709f0: 0a20 2020 2023 2043 7265 6174 6520 6120  .    # Create a 
-00070a00: 7379 6d6d 6574 7269 6320 7665 7273 696f  symmetric versio
-00070a10: 6e20 6f66 2074 6865 2069 6d61 6765 2062  n of the image b
-00070a20: 7920 6176 6572 6167 696e 6720 7468 6520  y averaging the 
-00070a30: 6f72 6967 696e 616c 2061 6e64 2074 6865  original and the
-00070a40: 206d 6972 726f 7220 696d 6167 650a 2020   mirror image.  
-00070a50: 2020 7379 6d6d 6574 7269 635f 696d 6167    symmetric_imag
-00070a60: 6520 3d20 696d 6167 656e 202a 2030 2e35  e = imagen * 0.5
-00070a70: 202b 206d 6972 726f 725f 696d 6167 6520   + mirror_image 
-00070a80: 2a20 302e 350a 0a20 2020 2023 2049 6465  * 0.5..    # Ide
-00070a90: 6e74 6966 7920 706f 7465 6e74 6961 6c20  ntify potential 
-00070aa0: 6c65 7369 6f6e 2061 7265 6173 2062 7920  lesion areas by 
-00070ab0: 6669 6e64 696e 6720 6469 6666 6572 656e  finding differen
-00070ac0: 6365 7320 6265 7477 6565 6e20 7468 6520  ces between the 
-00070ad0: 6f72 6967 696e 616c 2061 6e64 2073 796d  original and sym
-00070ae0: 6d65 7472 6963 2069 6d61 6765 0a20 2020  metric image.   
-00070af0: 2064 6966 6665 7265 6e63 655f 696d 6167   difference_imag
-00070b00: 6520 3d20 696d 6167 6520 2d20 7379 6d6d  e = image - symm
-00070b10: 6574 7269 635f 696d 6167 650a 2020 2020  etric_image.    
-00070b20: 6469 6666 7365 6720 3d20 616e 7473 2e74  diffseg = ants.t
-00070b30: 6872 6573 686f 6c64 5f69 6d61 6765 2864  hreshold_image(d
-00070b40: 6966 6665 7265 6e63 655f 696d 6167 652c  ifference_image,
-00070b50: 2022 4f74 7375 222c 2033 2029 0a20 2020   "Otsu", 3 ).   
-00070b60: 2069 6620 696e 7465 6e73 6974 7920 3d3d   if intensity ==
-00070b70: 2027 6c6f 7727 3a0a 2020 2020 2020 2020   'low':.        
-00070b80: 6c69 6b65 6c79 5f6c 6573 696f 6e20 3d20  likely_lesion = 
-00070b90: 616e 7473 2e74 6872 6573 686f 6c64 5f69  ants.threshold_i
-00070ba0: 6d61 6765 2820 6469 6666 7365 672c 2031  mage( diffseg, 1
-00070bb0: 2c20 2031 290a 2020 2020 656c 7365 3a0a  ,  1).    else:.
-00070bc0: 2020 2020 2020 2020 6c69 6b65 6c79 5f6c          likely_l
-00070bd0: 6573 696f 6e20 3d20 616e 7473 2e74 6872  esion = ants.thr
-00070be0: 6573 686f 6c64 5f69 6d61 6765 2820 6469  eshold_image( di
-00070bf0: 6666 7365 672c 2033 2c20 2033 290a 2020  ffseg, 3,  3).  
-00070c00: 2020 6c69 6b65 6c79 5f6c 6573 696f 6e20    likely_lesion 
-00070c10: 3d20 616e 7473 2e73 6d6f 6f74 685f 696d  = ants.smooth_im
-00070c20: 6167 6528 206c 696b 656c 795f 6c65 7369  age( likely_lesi
-00070c30: 6f6e 2c20 332e 3020 292e 694d 6174 6828  on, 3.0 ).iMath(
-00070c40: 224e 6f72 6d61 6c69 7a65 2229 0a20 2020  "Normalize").   
-00070c50: 206c 6573 696f 6e6e 6567 203d 2028 2069   lesionneg = ( i
-00070c60: 6d61 6765 6e2a 302b 312e 3020 2920 2d20  magen*0+1.0 ) - 
-00070c70: 6c69 6b65 6c79 5f6c 6573 696f 6e0a 2020  likely_lesion.  
-00070c80: 2020 6669 6c6c 6564 5f69 6d61 6765 203d    filled_image =
-00070c90: 2061 6e74 732e 696d 6167 655f 636c 6f6e   ants.image_clon
-00070ca0: 6528 696d 6167 656e 2920 2020 200a 2020  e(imagen)    .  
-00070cb0: 2020 6669 6c6c 6564 5f69 6d61 6765 203d    filled_image =
-00070cc0: 2069 6d61 6765 6e20 2a20 6c65 7369 6f6e   imagen * lesion
-00070cd0: 6e65 6720 2b20 6d69 7272 6f72 5f69 6d61  neg + mirror_ima
-00070ce0: 6765 202a 206c 696b 656c 795f 6c65 7369  ge * likely_lesi
-00070cf0: 6f6e 0a0a 2020 2020 7265 7475 726e 2066  on..    return f
-00070d00: 696c 6c65 645f 696d 6167 652c 2064 6966  illed_image, dif
-00070d10: 6673 6567 0a0a 0a0a 6465 6620 6669 6c74  fseg....def filt
-00070d20: 6572 5f69 6d61 6765 5f66 696c 6573 2869  er_image_files(i
-00070d30: 6d61 6765 5f70 6174 6873 2c20 6372 6974  mage_paths, crit
-00070d40: 6572 6961 3d27 6c61 7267 6573 7427 293a  eria='largest'):
-00070d50: 0a20 2020 2022 2222 0a20 2020 2046 696c  .    """.    Fil
-00070d60: 7465 7273 2061 206c 6973 7420 6f66 2069  ters a list of i
-00070d70: 6d61 6765 2066 696c 6520 7061 7468 7320  mage file paths 
-00070d80: 6261 7365 6420 6f6e 2073 7065 6369 6669  based on specifi
-00070d90: 6564 2063 7269 7465 7269 6120 616e 6420  ed criteria and 
-00070da0: 7265 7475 726e 7320 0a20 2020 2074 6865  returns .    the
-00070db0: 2070 6174 6820 6f66 2074 6865 2069 6d61   path of the ima
-00070dc0: 6765 2074 6861 7420 6265 7374 206d 6174  ge that best mat
-00070dd0: 6368 6573 2074 6861 7420 6372 6974 6572  ches that criter
-00070de0: 6961 2028 736d 616c 6c65 7374 2c20 6c61  ia (smallest, la
-00070df0: 7267 6573 742c 206f 7220 6272 6967 6874  rgest, or bright
-00070e00: 6573 7429 2e0a 0a20 2020 2041 7267 733a  est)...    Args:
-00070e10: 0a20 2020 2069 6d61 6765 5f70 6174 6873  .    image_paths
-00070e20: 2028 6c69 7374 293a 2041 206c 6973 7420   (list): A list 
-00070e30: 6f66 2066 696c 6520 7061 7468 7320 746f  of file paths to
-00070e40: 2074 6865 2069 6d61 6765 732e 0a20 2020   the images..   
-00070e50: 2063 7269 7465 7269 6120 2873 7472 293a   criteria (str):
-00070e60: 2043 7269 7465 7269 6120 666f 7220 7365   Criteria for se
-00070e70: 6c65 6374 696e 6720 7468 6520 696d 6167  lecting the imag
-00070e80: 6520 2827 736d 616c 6c65 7374 272c 2027  e ('smallest', '
-00070e90: 6c61 7267 6573 7427 2c20 2762 7269 6768  largest', 'brigh
-00070ea0: 7465 7374 2729 2e0a 0a20 2020 2052 6574  test')...    Ret
-00070eb0: 7572 6e73 3a0a 2020 2020 7374 723a 2054  urns:.    str: T
-00070ec0: 6865 2066 696c 6520 7061 7468 206f 6620  he file path of 
-00070ed0: 7468 6520 7365 6c65 6374 6564 2069 6d61  the selected ima
-00070ee0: 6765 2c20 6f72 204e 6f6e 6520 6966 206e  ge, or None if n
-00070ef0: 6f20 7661 6c69 6420 696d 6167 6573 2061  o valid images a
-00070f00: 7265 2066 6f75 6e64 2e0a 2020 2020 2222  re found..    ""
-00070f10: 220a 2020 2020 696d 706f 7274 206e 756d  ".    import num
-00070f20: 7079 2061 7320 6e70 0a20 2020 2069 6620  py as np.    if 
-00070f30: 6e6f 7420 696d 6167 655f 7061 7468 733a  not image_paths:
-00070f40: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00070f50: 4e6f 6e65 0a0a 2020 2020 7365 6c65 6374  None..    select
-00070f60: 6564 5f69 6d61 6765 5f70 6174 6820 3d20  ed_image_path = 
-00070f70: 4e6f 6e65 0a20 2020 2069 6620 6372 6974  None.    if crit
-00070f80: 6572 6961 203d 3d20 2773 6d61 6c6c 6573  eria == 'smalles
-00070f90: 7427 206f 7220 6372 6974 6572 6961 203d  t' or criteria =
-00070fa0: 3d20 276c 6172 6765 7374 273a 0a20 2020  = 'largest':.   
-00070fb0: 2020 2020 2065 7874 7265 6d65 5f76 6f6c       extreme_vol
-00070fc0: 756d 6520 3d20 4e6f 6e65 0a0a 2020 2020  ume = None..    
-00070fd0: 2020 2020 666f 7220 7061 7468 2069 6e20      for path in 
-00070fe0: 696d 6167 655f 7061 7468 733a 0a20 2020  image_paths:.   
-00070ff0: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
-00071000: 2020 2020 2020 2020 2020 2020 2020 696d                im
-00071010: 6167 6520 3d20 616e 7473 2e69 6d61 6765  age = ants.image
-00071020: 5f72 6561 6428 7061 7468 290a 2020 2020  _read(path).    
-00071030: 2020 2020 2020 2020 2020 2020 766f 6c75              volu
-00071040: 6d65 203d 206e 702e 7072 6f64 2869 6d61  me = np.prod(ima
-00071050: 6765 2e73 6861 7065 290a 0a20 2020 2020  ge.shape)..     
-00071060: 2020 2020 2020 2020 2020 2069 6620 6372             if cr
-00071070: 6974 6572 6961 203d 3d20 276c 6172 6765  iteria == 'large
-00071080: 7374 273a 0a20 2020 2020 2020 2020 2020  st':.           
-00071090: 2020 2020 2020 2020 2069 6620 6578 7472           if extr
-000710a0: 656d 655f 766f 6c75 6d65 2069 7320 4e6f  eme_volume is No
-000710b0: 6e65 206f 7220 766f 6c75 6d65 203e 2065  ne or volume > e
-000710c0: 7874 7265 6d65 5f76 6f6c 756d 653a 0a20  xtreme_volume:. 
-000710d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000710e0: 2020 2020 2020 2065 7874 7265 6d65 5f76         extreme_v
-000710f0: 6f6c 756d 6520 3d20 766f 6c75 6d65 0a20  olume = volume. 
-00071100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00071110: 2020 2020 2020 2073 656c 6563 7465 645f         selected_
-00071120: 696d 6167 655f 7061 7468 203d 2070 6174  image_path = pat
-00071130: 680a 2020 2020 2020 2020 2020 2020 2020  h.              
-00071140: 2020 656c 6966 2063 7269 7465 7269 6120    elif criteria 
-00071150: 3d3d 2027 736d 616c 6c65 7374 273a 0a20  == 'smallest':. 
-00071160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00071170: 2020 2069 6620 6578 7472 656d 655f 766f     if extreme_vo
-00071180: 6c75 6d65 2069 7320 4e6f 6e65 206f 7220  lume is None or 
-00071190: 766f 6c75 6d65 203c 2065 7874 7265 6d65  volume < extreme
-000711a0: 5f76 6f6c 756d 653a 0a20 2020 2020 2020  _volume:.       
-000711b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000711c0: 2065 7874 7265 6d65 5f76 6f6c 756d 6520   extreme_volume 
-000711d0: 3d20 766f 6c75 6d65 0a20 2020 2020 2020  = volume.       
-000711e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000711f0: 2073 656c 6563 7465 645f 696d 6167 655f   selected_image_
-00071200: 7061 7468 203d 2070 6174 680a 0a20 2020  path = path..   
-00071210: 2020 2020 2020 2020 2065 7863 6570 7420           except 
-00071220: 4578 6365 7074 696f 6e20 6173 2065 3a0a  Exception as e:.
-00071230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00071240: 7072 696e 7428 6622 4572 726f 7220 7072  print(f"Error pr
-00071250: 6f63 6573 7369 6e67 2069 6d61 6765 207b  ocessing image {
-00071260: 7061 7468 7d3a 207b 657d 2229 0a0a 2020  path}: {e}")..  
-00071270: 2020 656c 6966 2063 7269 7465 7269 6120    elif criteria 
-00071280: 3d3d 2027 6272 6967 6874 6573 7427 3a0a  == 'brightest':.
-00071290: 2020 2020 2020 2020 6d61 785f 6272 6967          max_brig
-000712a0: 6874 6e65 7373 203d 204e 6f6e 650a 0a20  htness = None.. 
-000712b0: 2020 2020 2020 2066 6f72 2070 6174 6820         for path 
-000712c0: 696e 2069 6d61 6765 5f70 6174 6873 3a0a  in image_paths:.
-000712d0: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-000712e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000712f0: 2069 6d61 6765 203d 2061 6e74 732e 696d   image = ants.im
-00071300: 6167 655f 7265 6164 2870 6174 6829 0a20  age_read(path). 
-00071310: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-00071320: 7269 6768 746e 6573 7320 3d20 6e70 2e6d  rightness = np.m
-00071330: 6561 6e28 696d 6167 652e 6e75 6d70 7928  ean(image.numpy(
-00071340: 2929 0a0a 2020 2020 2020 2020 2020 2020  ))..            
-00071350: 2020 2020 6966 206d 6178 5f62 7269 6768      if max_brigh
-00071360: 746e 6573 7320 6973 204e 6f6e 6520 6f72  tness is None or
-00071370: 2062 7269 6768 746e 6573 7320 3e20 6d61   brightness > ma
-00071380: 785f 6272 6967 6874 6e65 7373 3a0a 2020  x_brightness:.  
-00071390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000713a0: 2020 6d61 785f 6272 6967 6874 6e65 7373    max_brightness
-000713b0: 203d 2062 7269 6768 746e 6573 730a 2020   = brightness.  
-000713c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000713d0: 2020 7365 6c65 6374 6564 5f69 6d61 6765    selected_image
-000713e0: 5f70 6174 6820 3d20 7061 7468 0a0a 2020  _path = path..  
-000713f0: 2020 2020 2020 2020 2020 6578 6365 7074            except
-00071400: 2045 7863 6570 7469 6f6e 2061 7320 653a   Exception as e:
-00071410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00071420: 2070 7269 6e74 2866 2245 7272 6f72 2070   print(f"Error p
-00071430: 726f 6365 7373 696e 6720 696d 6167 6520  rocessing image 
-00071440: 7b70 6174 687d 3a20 7b65 7d22 290a 0a20  {path}: {e}").. 
-00071450: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00071460: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-00071470: 7228 2243 7269 7465 7269 6120 6d75 7374  r("Criteria must
-00071480: 2062 6520 2773 6d61 6c6c 6573 7427 2c20   be 'smallest', 
-00071490: 276c 6172 6765 7374 272c 206f 7220 2762  'largest', or 'b
-000714a0: 7269 6768 7465 7374 272e 2229 0a0a 2020  rightest'.")..  
-000714b0: 2020 7265 7475 726e 2073 656c 6563 7465    return selecte
-000714c0: 645f 696d 6167 655f 7061 7468 0a0a 0a0a  d_image_path....
-000714d0: 6465 6620 6d6d 5f6d 6174 6368 5f62 795f  def mm_match_by_
-000714e0: 7163 5f73 636f 7269 6e67 2864 665f 612c  qc_scoring(df_a,
-000714f0: 2064 665f 622c 206d 6174 6368 5f63 6f6c   df_b, match_col
-00071500: 756d 6e2c 2063 7269 7465 7269 612c 2070  umn, criteria, p
-00071510: 7265 6669 783d 276d 6174 6368 6564 5f27  refix='matched_'
-00071520: 2c20 6578 636c 7564 655f 636f 6c75 6d6e  , exclude_column
-00071530: 733d 4e6f 6e65 293a 0a20 2020 2022 2222  s=None):.    """
-00071540: 0a20 2020 204d 6174 6368 2065 6163 6820  .    Match each 
-00071550: 726f 7720 696e 2064 665f 6120 746f 2061  row in df_a to a
-00071560: 2072 6f77 2069 6e20 6466 5f62 2062 6173   row in df_b bas
-00071570: 6564 206f 6e20 6120 6d61 7463 6869 6e67  ed on a matching
-00071580: 2063 6f6c 756d 6e20 616e 6420 6372 6974   column and crit
-00071590: 6572 6961 2066 6f72 2073 656c 6563 7469  eria for selecti
-000715a0: 6e67 2074 6865 2062 6573 7420 6d61 7463  ng the best matc
-000715b0: 682c 0a20 2020 2077 6974 6820 6f70 7469  h,.    with opti
-000715c0: 6f6e 7320 746f 2070 7265 6669 7820 636f  ons to prefix co
-000715d0: 6c75 6d6e 206e 616d 6573 2066 726f 6d20  lumn names from 
-000715e0: 6466 5f62 2061 6e64 2065 7863 6c75 6465  df_b and exclude
-000715f0: 2063 6572 7461 696e 2063 6f6c 756d 6e73   certain columns
-00071600: 2066 726f 6d20 7468 6520 6669 6e61 6c20   from the final 
-00071610: 6f75 7470 7574 2e20 4164 6469 7469 6f6e  output. Addition
-00071620: 616c 6c79 2c0a 2020 2020 7265 7475 726e  ally,.    return
-00071630: 7320 6120 4461 7461 4672 616d 6520 636f  s a DataFrame co
-00071640: 6e74 6169 6e69 6e67 2072 6f77 7320 6672  ntaining rows fr
-00071650: 6f6d 2064 665f 6220 7468 6174 2077 6572  om df_b that wer
-00071660: 6520 6e6f 7420 6d61 7463 6865 6420 746f  e not matched to
-00071670: 2061 6e79 2072 6f77 2069 6e20 6466 5f61   any row in df_a
-00071680: 2e0a 0a20 2020 2050 6172 616d 6574 6572  ...    Parameter
-00071690: 733a 0a20 2020 202d 2064 665f 613a 2044  s:.    - df_a: D
-000716a0: 6174 6146 7261 6d65 2041 2e0a 2020 2020  ataFrame A..    
-000716b0: 2d20 6466 5f62 3a20 4461 7461 4672 616d  - df_b: DataFram
-000716c0: 6520 422e 0a20 2020 202d 206d 6174 6368  e B..    - match
-000716d0: 5f63 6f6c 756d 6e3a 2054 6865 2063 6f6c  _column: The col
-000716e0: 756d 6e20 6e61 6d65 206f 6e20 7768 6963  umn name on whic
-000716f0: 6820 726f 7773 2073 686f 756c 6420 6d61  h rows should ma
-00071700: 7463 6820 6265 7477 6565 6e20 4461 7461  tch between Data
-00071710: 4672 616d 6520 4120 616e 6420 422e 0a20  Frame A and B.. 
-00071720: 2020 202d 2063 7269 7465 7269 613a 2041     - criteria: A
-00071730: 2064 6963 7469 6f6e 6172 7920 7768 6572   dictionary wher
-00071740: 6520 6b65 7973 2061 7265 2063 6f6c 756d  e keys are colum
-00071750: 6e20 6e61 6d65 7320 616e 6420 7661 6c75  n names and valu
-00071760: 6573 2061 7265 2027 6d69 6e27 206f 7220  es are 'min' or 
-00071770: 276d 6178 272c 2069 6e64 6963 6174 696e  'max', indicatin
-00071780: 6720 7768 6574 6865 720a 2020 2020 2020  g whether.      
-00071790: 2020 2020 2020 2020 2020 7468 6520 636f            the co
-000717a0: 6c75 6d6e 2073 686f 756c 6420 6265 206d  lumn should be m
-000717b0: 696e 696d 697a 6564 206f 7220 6d61 7869  inimized or maxi
-000717c0: 6d69 7a65 6420 666f 7220 7468 6520 6265  mized for the be
-000717d0: 7374 206d 6174 6368 2e0a 2020 2020 2d20  st match..    - 
-000717e0: 7072 6566 6978 3a20 4120 7374 7269 6e67  prefix: A string
-000717f0: 2070 7265 6669 7820 746f 2061 6464 2074   prefix to add t
-00071800: 6f20 636f 6c75 6d6e 206e 616d 6573 2066  o column names f
-00071810: 726f 6d20 6466 5f62 2069 6e20 7468 6520  rom df_b in the 
-00071820: 6669 6e61 6c20 6f75 7470 7574 2074 6f20  final output to 
-00071830: 6176 6f69 6420 6475 706c 6963 6174 696f  avoid duplicatio
-00071840: 6e2e 0a20 2020 202d 2065 7863 6c75 6465  n..    - exclude
-00071850: 5f63 6f6c 756d 6e73 3a20 4120 6c69 7374  _columns: A list
-00071860: 206f 6620 636f 6c75 6d6e 206e 616d 6573   of column names
-00071870: 2066 726f 6d20 6466 5f62 2074 6f20 6578   from df_b to ex
-00071880: 636c 7564 6520 6672 6f6d 2074 6865 2066  clude from the f
-00071890: 696e 616c 206f 7574 7075 742e 0a20 2020  inal output..   
-000718a0: 200a 2020 2020 5265 7475 726e 733a 0a20   .    Returns:. 
-000718b0: 2020 202d 2041 2074 7570 6c65 206f 6620     - A tuple of 
-000718c0: 7477 6f20 4461 7461 4672 616d 6573 3a20  two DataFrames: 
-000718d0: 0a20 2020 2020 2020 2031 2e20 4120 6e65  .        1. A ne
-000718e0: 7720 4461 7461 4672 616d 6520 636f 6d62  w DataFrame comb
-000718f0: 696e 696e 6720 6466 5f61 2077 6974 6820  ining df_a with 
-00071900: 6d61 7463 6865 6420 726f 7773 2066 726f  matched rows fro
-00071910: 6d20 6466 5f62 2e0a 2020 2020 2020 2020  m df_b..        
-00071920: 322e 2041 2044 6174 6146 7261 6d65 2063  2. A DataFrame c
-00071930: 6f6e 7461 696e 696e 6720 726f 7773 2066  ontaining rows f
-00071940: 726f 6d20 6466 5f62 2074 6861 7420 7765  rom df_b that we
-00071950: 7265 206e 6f74 206d 6174 6368 6564 2074  re not matched t
-00071960: 6f20 6466 5f61 2e0a 2020 2020 2222 220a  o df_a..    """.
-00071970: 2020 2020 6672 6f6d 2073 6369 7079 2e73      from scipy.s
-00071980: 7461 7473 2069 6d70 6f72 7420 7a73 636f  tats import zsco
-00071990: 7265 0a20 2020 2064 665f 6120 3d20 6466  re.    df_a = df
-000719a0: 5f61 2e6c 6f63 5b3a 2c20 7e64 665f 612e  _a.loc[:, ~df_a.
-000719b0: 636f 6c75 6d6e 732e 7374 722e 7374 6172  columns.str.star
-000719c0: 7473 7769 7468 2827 556e 6e61 6d65 643a  tswith('Unnamed:
-000719d0: 2729 5d0a 2020 2020 6466 5f62 203d 2064  ')].    df_b = d
-000719e0: 665f 622e 6c6f 635b 3a2c 207e 6466 5f62  f_b.loc[:, ~df_b
-000719f0: 2e63 6f6c 756d 6e73 2e73 7472 2e73 7461  .columns.str.sta
-00071a00: 7274 7377 6974 6828 2755 6e6e 616d 6564  rtswith('Unnamed
-00071a10: 3a27 295d 2e63 6f70 7928 290a 2020 2020  :')].copy().    
-00071a20: 0a20 2020 2023 204e 6f72 6d61 6c69 7a65  .    # Normalize
-00071a30: 2064 665f 6220 6261 7365 6420 6f6e 2063   df_b based on c
-00071a40: 7269 7465 7269 610a 2020 2020 666f 7220  riteria.    for 
-00071a50: 636f 6c2c 2063 7269 7420 696e 2063 7269  col, crit in cri
-00071a60: 7465 7269 612e 6974 656d 7328 293a 0a20  teria.items():. 
-00071a70: 2020 2020 2020 2069 6620 6372 6974 203d         if crit =
-00071a80: 3d20 276d 6178 273a 0a20 2020 2020 2020  = 'max':.       
-00071a90: 2020 2020 2064 665f 622e 6c6f 635b 6466       df_b.loc[df
-00071aa0: 5f62 2e69 6e64 6578 2c20 6627 7363 6f72  _b.index, f'scor
-00071ab0: 655f 7b63 6f6c 7d27 5d20 3d20 7a73 636f  e_{col}'] = zsco
-00071ac0: 7265 282d 6466 5f62 5b63 6f6c 5d29 0a20  re(-df_b[col]). 
-00071ad0: 2020 2020 2020 2065 6c69 6620 6372 6974         elif crit
-00071ae0: 203d 3d20 276d 696e 273a 0a20 2020 2020   == 'min':.     
-00071af0: 2020 2020 2020 2064 665f 622e 6c6f 635b         df_b.loc[
-00071b00: 6466 5f62 2e69 6e64 6578 2c20 6627 7363  df_b.index, f'sc
-00071b10: 6f72 655f 7b63 6f6c 7d27 5d20 3d20 7a73  ore_{col}'] = zs
-00071b20: 636f 7265 2864 665f 625b 636f 6c5d 290a  core(df_b[col]).
-00071b30: 0a20 2020 2023 2043 616c 6375 6c61 7465  .    # Calculate
-00071b40: 2027 6265 7374 5f73 636f 7265 2720 6279   'best_score' by
-00071b50: 2073 756d 6d69 6e67 2061 6c6c 2073 636f   summing all sco
-00071b60: 7265 2063 6f6c 756d 6e73 0a20 2020 2073  re columns.    s
-00071b70: 636f 7265 5f63 6f6c 756d 6e73 203d 205b  core_columns = [
-00071b80: 6627 7363 6f72 655f 7b63 6f6c 7d27 2066  f'score_{col}' f
-00071b90: 6f72 2063 6f6c 2069 6e20 6372 6974 6572  or col in criter
-00071ba0: 6961 2e6b 6579 7328 295d 0a20 2020 2064  ia.keys()].    d
-00071bb0: 665f 625b 2762 6573 745f 7363 6f72 6527  f_b['best_score'
-00071bc0: 5d20 3d20 6466 5f62 5b73 636f 7265 5f63  ] = df_b[score_c
-00071bd0: 6f6c 756d 6e73 5d2e 7375 6d28 6178 6973  olumns].sum(axis
-00071be0: 3d31 290a 0a20 2020 206d 6174 6368 6564  =1)..    matched
-00071bf0: 5f69 6e64 6963 6573 203d 205b 5d20 2023  _indices = []  #
-00071c00: 2054 7261 636b 2069 6e64 6963 6573 206f   Track indices o
-00071c10: 6620 6d61 7463 6865 6420 726f 7773 2069  f matched rows i
-00071c20: 6e20 6466 5f62 0a0a 2020 2020 2320 4d61  n df_b..    # Ma
-00071c30: 7463 6820 726f 7773 0a20 2020 206d 6174  tch rows.    mat
-00071c40: 6368 6564 5f72 6f77 7320 3d20 5b5d 0a20  ched_rows = []. 
-00071c50: 2020 2066 6f72 205f 2c20 726f 775f 6120     for _, row_a 
-00071c60: 696e 2064 665f 612e 6974 6572 726f 7773  in df_a.iterrows
-00071c70: 2829 3a0a 2020 2020 2020 2020 6d61 7463  ():.        matc
-00071c80: 6865 7320 3d20 6466 5f62 5b64 665f 625b  hes = df_b[df_b[
-00071c90: 6d61 7463 685f 636f 6c75 6d6e 5d20 3d3d  match_column] ==
-00071ca0: 2072 6f77 5f61 5b6d 6174 6368 5f63 6f6c   row_a[match_col
-00071cb0: 756d 6e5d 5d0a 2020 2020 2020 2020 6966  umn]].        if
-00071cc0: 206e 6f74 206d 6174 6368 6573 2e65 6d70   not matches.emp
-00071cd0: 7479 3a0a 2020 2020 2020 2020 2020 2020  ty:.            
-00071ce0: 6265 7374 5f69 6478 203d 206d 6174 6368  best_idx = match
-00071cf0: 6573 5b27 6265 7374 5f73 636f 7265 275d  es['best_score']
-00071d00: 2e69 6478 6d69 6e28 290a 2020 2020 2020  .idxmin().      
-00071d10: 2020 2020 2020 6265 7374 5f6d 6174 6368        best_match
-00071d20: 203d 206d 6174 6368 6573 2e6c 6f63 5b62   = matches.loc[b
-00071d30: 6573 745f 6964 785d 0a20 2020 2020 2020  est_idx].       
-00071d40: 2020 2020 206d 6174 6368 6564 5f69 6e64       matched_ind
-00071d50: 6963 6573 2e61 7070 656e 6428 6265 7374  ices.append(best
-00071d60: 5f69 6478 2920 2023 2054 7261 636b 2074  _idx)  # Track t
-00071d70: 6869 7320 696e 6465 7820 6173 206d 6174  his index as mat
-00071d80: 6368 6564 0a20 2020 2020 2020 2020 2020  ched.           
-00071d90: 206d 6174 6368 6564 5f72 6f77 732e 6170   matched_rows.ap
-00071da0: 7065 6e64 2862 6573 745f 6d61 7463 6829  pend(best_match)
-00071db0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00071dc0: 2020 2020 2020 2020 2020 206d 6174 6368             match
-00071dd0: 6564 5f72 6f77 732e 6170 7065 6e64 2870  ed_rows.append(p
-00071de0: 642e 5365 7269 6573 2864 7479 7065 3d27  d.Series(dtype='
-00071df0: 666c 6f61 7436 3427 2929 0a0a 2020 2020  float64'))..    
-00071e00: 2320 4372 6561 7465 2061 2044 6174 6146  # Create a DataF
-00071e10: 7261 6d65 2066 726f 6d20 6d61 7463 6865  rame from matche
-00071e20: 6420 726f 7773 0a20 2020 2064 665f 6d61  d rows.    df_ma
-00071e30: 7463 6865 6420 3d20 7064 2e44 6174 6146  tched = pd.DataF
-00071e40: 7261 6d65 286d 6174 6368 6564 5f72 6f77  rame(matched_row
-00071e50: 7329 2e72 6573 6574 5f69 6e64 6578 2864  s).reset_index(d
-00071e60: 726f 703d 5472 7565 290a 2020 2020 0a20  rop=True).    . 
-00071e70: 2020 2023 2045 7863 6c75 6465 2073 7065     # Exclude spe
-00071e80: 6369 6669 6564 2063 6f6c 756d 6e73 2061  cified columns a
-00071e90: 6e64 2061 6464 2070 7265 6669 780a 2020  nd add prefix.  
-00071ea0: 2020 6966 2065 7863 6c75 6465 5f63 6f6c    if exclude_col
-00071eb0: 756d 6e73 2069 7320 6e6f 7420 4e6f 6e65  umns is not None
-00071ec0: 3a0a 2020 2020 2020 2020 6466 5f6d 6174  :.        df_mat
-00071ed0: 6368 6564 203d 2064 665f 6d61 7463 6865  ched = df_matche
-00071ee0: 642e 6472 6f70 2863 6f6c 756d 6e73 3d65  d.drop(columns=e
-00071ef0: 7863 6c75 6465 5f63 6f6c 756d 6e73 2c20  xclude_columns, 
-00071f00: 6572 726f 7273 3d27 6967 6e6f 7265 2729  errors='ignore')
-00071f10: 0a20 2020 2064 665f 6d61 7463 6865 6420  .    df_matched 
-00071f20: 3d20 6466 5f6d 6174 6368 6564 2e72 656e  = df_matched.ren
-00071f30: 616d 6528 636f 6c75 6d6e 733d 6c61 6d62  ame(columns=lamb
-00071f40: 6461 2078 3a20 6622 7b70 7265 6669 787d  da x: f"{prefix}
-00071f50: 7b78 7d22 2069 6620 7820 213d 206d 6174  {x}" if x != mat
-00071f60: 6368 5f63 6f6c 756d 6e20 616e 6420 7820  ch_column and x 
-00071f70: 696e 2064 665f 6d61 7463 6865 642e 636f  in df_matched.co
-00071f80: 6c75 6d6e 7320 656c 7365 2078 290a 0a20  lumns else x).. 
-00071f90: 2020 2023 2043 6f6d 6269 6e65 2064 665f     # Combine df_
-00071fa0: 6120 7769 7468 206d 6174 6368 6564 2072  a with matched r
-00071fb0: 6f77 7320 6672 6f6d 2064 665f 620a 2020  ows from df_b.  
-00071fc0: 2020 7265 7375 6c74 5f64 6620 3d20 7064    result_df = pd
-00071fd0: 2e63 6f6e 6361 7428 5b64 665f 612e 7265  .concat([df_a.re
-00071fe0: 7365 745f 696e 6465 7828 6472 6f70 3d54  set_index(drop=T
-00071ff0: 7275 6529 2c20 6466 5f6d 6174 6368 6564  rue), df_matched
-00072000: 5d2c 2061 7869 733d 3129 0a20 2020 200a  ], axis=1).    .
-00072010: 2020 2020 2320 4578 7472 6163 7420 756e      # Extract un
-00072020: 6d61 7463 6865 6420 726f 7773 2066 726f  matched rows fro
-00072030: 6d20 6466 5f62 0a20 2020 2075 6e6d 6174  m df_b.    unmat
-00072040: 6368 6564 5f64 665f 6220 3d20 6466 5f62  ched_df_b = df_b
-00072050: 2e64 726f 7028 696e 6465 783d 6d61 7463  .drop(index=matc
-00072060: 6865 645f 696e 6469 6365 7329 2e72 6573  hed_indices).res
-00072070: 6574 5f69 6e64 6578 2864 726f 703d 5472  et_index(drop=Tr
-00072080: 7565 290a 0a20 2020 2072 6574 7572 6e20  ue)..    return 
-00072090: 7265 7375 6c74 5f64 662c 2075 6e6d 6174  result_df, unmat
-000720a0: 6368 6564 5f64 665f 620a 0a0a 6465 6620  ched_df_b...def 
-000720b0: 6669 785f 4c52 5f52 4c5f 7374 7566 6628  fix_LR_RL_stuff(
-000720c0: 6466 2c20 636f 6c31 2c20 636f 6c32 2c20  df, col1, col2, 
-000720d0: 7369 7a65 5f63 6f6c 312c 2073 697a 655f  size_col1, size_
-000720e0: 636f 6c32 2c20 6964 312c 2069 6432 2029  col2, id1, id2 )
-000720f0: 3a0a 2020 2020 6466 5f63 6f70 7920 3d20  :.    df_copy = 
-00072100: 6466 2e63 6f70 7928 290a 2020 2020 2320  df.copy().    # 
-00072110: 456e 7375 7265 2063 6f6c 756d 6e73 2063  Ensure columns c
-00072120: 6f6e 7461 696e 2073 7472 696e 6773 2066  ontain strings f
-00072130: 6f72 2073 7562 7374 7269 6e67 2063 6865  or substring che
-00072140: 636b 730a 2020 2020 6466 5f63 6f70 795b  cks.    df_copy[
-00072150: 636f 6c31 5d20 3d20 6466 5f63 6f70 795b  col1] = df_copy[
-00072160: 636f 6c31 5d2e 6173 7479 7065 2873 7472  col1].astype(str
-00072170: 290a 2020 2020 6466 5f63 6f70 795b 636f  ).    df_copy[co
-00072180: 6c32 5d20 3d20 6466 5f63 6f70 795b 636f  l2] = df_copy[co
-00072190: 6c32 5d2e 6173 7479 7065 2873 7472 290a  l2].astype(str).
-000721a0: 2020 2020 6466 5f63 6f70 795b 6964 315d      df_copy[id1]
-000721b0: 203d 2064 665f 636f 7079 5b69 6431 5d2e   = df_copy[id1].
-000721c0: 6173 7479 7065 2873 7472 290a 2020 2020  astype(str).    
-000721d0: 6466 5f63 6f70 795b 6964 325d 203d 2064  df_copy[id2] = d
-000721e0: 665f 636f 7079 5b69 6432 5d2e 6173 7479  f_copy[id2].asty
-000721f0: 7065 2873 7472 290a 2020 2020 0a20 2020  pe(str).    .   
-00072200: 2066 6f72 2069 6e64 6578 2c20 726f 7720   for index, row 
-00072210: 696e 2064 665f 636f 7079 2e69 7465 7272  in df_copy.iterr
-00072220: 6f77 7328 293a 0a20 2020 2020 2020 2063  ows():.        c
-00072230: 6f6c 315f 7661 6c20 3d20 726f 775b 636f  ol1_val = row[co
-00072240: 6c31 5d0a 2020 2020 2020 2020 636f 6c32  l1].        col2
-00072250: 5f76 616c 203d 2072 6f77 5b63 6f6c 325d  _val = row[col2]
-00072260: 0a20 2020 2020 2020 2073 697a 6531 203d  .        size1 =
-00072270: 2072 6f77 5b73 697a 655f 636f 6c31 5d0a   row[size_col1].
-00072280: 2020 2020 2020 2020 7369 7a65 3220 3d20          size2 = 
-00072290: 726f 775b 7369 7a65 5f63 6f6c 325d 0a20  row[size_col2]. 
-000722a0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-000722b0: 2320 4368 6563 6b20 666f 7220 2752 4c27  # Check for 'RL'
-000722c0: 206f 7220 274c 5227 2069 6e20 6561 6368   or 'LR' in each
-000722d0: 2063 6f6c 756d 6e20 616e 6420 636f 6d70   column and comp
-000722e0: 6172 6520 7369 7a65 730a 2020 2020 2020  are sizes.      
-000722f0: 2020 6966 2028 2752 4c27 2069 6e20 636f    if ('RL' in co
-00072300: 6c31 5f76 616c 206f 7220 274c 5227 2069  l1_val or 'LR' i
-00072310: 6e20 636f 6c31 5f76 616c 2920 616e 6420  n col1_val) and 
-00072320: 2827 524c 2720 696e 2063 6f6c 325f 7661  ('RL' in col2_va
-00072330: 6c20 6f72 2027 4c52 2720 696e 2063 6f6c  l or 'LR' in col
-00072340: 325f 7661 6c29 3a0a 2020 2020 2020 2020  2_val):.        
-00072350: 2020 2020 636f 6e74 696e 7565 0a20 2020      continue.   
-00072360: 2020 2020 2065 6c69 6620 2752 4c27 206e       elif 'RL' n
-00072370: 6f74 2069 6e20 636f 6c31 5f76 616c 2061  ot in col1_val a
-00072380: 6e64 2027 4c52 2720 6e6f 7420 696e 2063  nd 'LR' not in c
-00072390: 6f6c 315f 7661 6c20 616e 6420 2752 4c27  ol1_val and 'RL'
-000723a0: 206e 6f74 2069 6e20 636f 6c32 5f76 616c   not in col2_val
-000723b0: 2061 6e64 2027 4c52 2720 6e6f 7420 696e   and 'LR' not in
-000723c0: 2063 6f6c 325f 7661 6c3a 0a20 2020 2020   col2_val:.     
-000723d0: 2020 2020 2020 2069 6620 7369 7a65 3120         if size1 
-000723e0: 3c20 7369 7a65 323a 0a20 2020 2020 2020  < size2:.       
-000723f0: 2020 2020 2020 2020 2064 665f 636f 7079           df_copy
-00072400: 2e61 745b 696e 6465 782c 2063 6f6c 315d  .at[index, col1]
-00072410: 203d 2064 665f 636f 7079 2e61 745b 696e   = df_copy.at[in
-00072420: 6465 782c 2063 6f6c 325d 0a20 2020 2020  dex, col2].     
-00072430: 2020 2020 2020 2020 2020 2064 665f 636f             df_co
-00072440: 7079 2e61 745b 696e 6465 782c 2073 697a  py.at[index, siz
-00072450: 655f 636f 6c31 5d20 3d20 6466 5f63 6f70  e_col1] = df_cop
-00072460: 792e 6174 5b69 6e64 6578 2c20 7369 7a65  y.at[index, size
-00072470: 5f63 6f6c 325d 0a20 2020 2020 2020 2020  _col2].         
-00072480: 2020 2020 2020 2064 665f 636f 7079 2e61         df_copy.a
-00072490: 745b 696e 6465 782c 2069 6431 5d20 3d20  t[index, id1] = 
-000724a0: 6466 5f63 6f70 792e 6174 5b69 6e64 6578  df_copy.at[index
-000724b0: 2c20 6964 325d 0a20 2020 2020 2020 2020  , id2].         
-000724c0: 2020 2020 2020 2064 665f 636f 7079 2e61         df_copy.a
-000724d0: 745b 696e 6465 782c 2073 697a 655f 636f  t[index, size_co
-000724e0: 6c32 5d20 3d20 300a 2020 2020 2020 2020  l2] = 0.        
-000724f0: 2020 2020 2020 2020 6466 5f63 6f70 792e          df_copy.
-00072500: 6174 5b69 6e64 6578 2c20 636f 6c32 5d20  at[index, col2] 
-00072510: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
-00072520: 2020 2020 2020 2064 665f 636f 7079 2e61         df_copy.a
-00072530: 745b 696e 6465 782c 2069 6432 5d20 3d20  t[index, id2] = 
-00072540: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
-00072550: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00072560: 2020 2020 2020 2064 665f 636f 7079 2e61         df_copy.a
-00072570: 745b 696e 6465 782c 2063 6f6c 325d 203d  t[index, col2] =
-00072580: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
-00072590: 2020 2020 2020 6466 5f63 6f70 792e 6174        df_copy.at
-000725a0: 5b69 6e64 6578 2c20 7369 7a65 5f63 6f6c  [index, size_col
-000725b0: 325d 203d 2030 0a20 2020 2020 2020 2020  2] = 0.         
-000725c0: 2020 2020 2020 2064 665f 636f 7079 2e61         df_copy.a
-000725d0: 745b 696e 6465 782c 2069 6432 5d20 3d20  t[index, id2] = 
-000725e0: 4e6f 6e65 0a20 2020 2020 2020 2065 6c69  None.        eli
-000725f0: 6620 2752 4c27 2069 6e20 636f 6c31 5f76  f 'RL' in col1_v
-00072600: 616c 206f 7220 274c 5227 2069 6e20 636f  al or 'LR' in co
-00072610: 6c31 5f76 616c 3a0a 2020 2020 2020 2020  l1_val:.        
-00072620: 2020 2020 6966 2073 697a 6531 203c 2073      if size1 < s
-00072630: 697a 6532 3a0a 2020 2020 2020 2020 2020  ize2:.          
-00072640: 2020 2020 2020 6466 5f63 6f70 792e 6174        df_copy.at
-00072650: 5b69 6e64 6578 2c20 636f 6c31 5d20 3d20  [index, col1] = 
-00072660: 6466 5f63 6f70 792e 6174 5b69 6e64 6578  df_copy.at[index
-00072670: 2c20 636f 6c32 5d0a 2020 2020 2020 2020  , col2].        
-00072680: 2020 2020 2020 2020 6466 5f63 6f70 792e          df_copy.
-00072690: 6174 5b69 6e64 6578 2c20 6964 315d 203d  at[index, id1] =
-000726a0: 2064 665f 636f 7079 2e61 745b 696e 6465   df_copy.at[inde
-000726b0: 782c 2069 6432 5d0a 2020 2020 2020 2020  x, id2].        
-000726c0: 2020 2020 2020 2020 6466 5f63 6f70 792e          df_copy.
-000726d0: 6174 5b69 6e64 6578 2c20 7369 7a65 5f63  at[index, size_c
-000726e0: 6f6c 315d 203d 2064 665f 636f 7079 2e61  ol1] = df_copy.a
-000726f0: 745b 696e 6465 782c 2073 697a 655f 636f  t[index, size_co
-00072700: 6c32 5d0a 2020 2020 2020 2020 2020 2020  l2].            
-00072710: 2020 2020 6466 5f63 6f70 792e 6174 5b69      df_copy.at[i
-00072720: 6e64 6578 2c20 7369 7a65 5f63 6f6c 325d  ndex, size_col2]
-00072730: 203d 2030 0a20 2020 2020 2020 2020 2020   = 0.           
-00072740: 2020 2020 2064 665f 636f 7079 2e61 745b       df_copy.at[
-00072750: 696e 6465 782c 2063 6f6c 325d 203d 204e  index, col2] = N
-00072760: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
-00072770: 2020 2020 6466 5f63 6f70 792e 6174 5b69      df_copy.at[i
-00072780: 6e64 6578 2c20 6964 325d 203d 204e 6f6e  ndex, id2] = Non
-00072790: 650a 2020 2020 2020 2020 2020 2020 656c  e.            el
-000727a0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-000727b0: 2020 2020 6466 5f63 6f70 792e 6174 5b69      df_copy.at[i
-000727c0: 6e64 6578 2c20 636f 6c32 5d20 3d20 4e6f  ndex, col2] = No
-000727d0: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
-000727e0: 2020 2064 665f 636f 7079 2e61 745b 696e     df_copy.at[in
-000727f0: 6465 782c 2069 6432 5d20 3d20 4e6f 6e65  dex, id2] = None
-00072800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00072810: 2064 665f 636f 7079 2e61 745b 696e 6465   df_copy.at[inde
-00072820: 782c 2073 697a 655f 636f 6c32 5d20 3d20  x, size_col2] = 
-00072830: 300a 2020 2020 2020 2020 656c 6966 2027  0.        elif '
-00072840: 524c 2720 696e 2063 6f6c 325f 7661 6c20  RL' in col2_val 
-00072850: 6f72 2027 4c52 2720 696e 2063 6f6c 325f  or 'LR' in col2_
-00072860: 7661 6c3a 0a20 2020 2020 2020 2020 2020  val:.           
-00072870: 2069 6620 7369 7a65 3220 3c20 7369 7a65   if size2 < size
-00072880: 313a 0a20 2020 2020 2020 2020 2020 2020  1:.             
-00072890: 2020 2064 665f 636f 7079 2e61 745b 696e     df_copy.at[in
-000728a0: 6465 782c 2069 6432 5d20 3d20 4e6f 6e65  dex, id2] = None
-000728b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000728c0: 2064 665f 636f 7079 2e61 745b 696e 6465   df_copy.at[inde
-000728d0: 782c 2063 6f6c 325d 203d 204e 6f6e 650a  x, col2] = None.
-000728e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000728f0: 6466 5f63 6f70 792e 6174 5b69 6e64 6578  df_copy.at[index
-00072900: 2c20 7369 7a65 5f63 6f6c 325d 203d 2030  , size_col2] = 0
-00072910: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-00072920: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00072930: 2020 2064 665f 636f 7079 2e61 745b 696e     df_copy.at[in
-00072940: 6465 782c 2063 6f6c 315d 203d 2064 665f  dex, col1] = df_
-00072950: 636f 7079 2e61 745b 696e 6465 782c 2063  copy.at[index, c
-00072960: 6f6c 325d 0a20 2020 2020 2020 2020 2020  ol2].           
-00072970: 2020 2020 2064 665f 636f 7079 2e61 745b       df_copy.at[
-00072980: 696e 6465 782c 2069 6431 5d20 3d20 6466  index, id1] = df
-00072990: 5f63 6f70 792e 6174 5b69 6e64 6578 2c20  _copy.at[index, 
-000729a0: 6964 325d 0a20 2020 2020 2020 2020 2020  id2].           
-000729b0: 2020 2020 2064 665f 636f 7079 2e61 745b       df_copy.at[
-000729c0: 696e 6465 782c 2073 697a 655f 636f 6c31  index, size_col1
-000729d0: 5d20 3d20 6466 5f63 6f70 792e 6174 5b69  ] = df_copy.at[i
-000729e0: 6e64 6578 2c20 7369 7a65 5f63 6f6c 325d  ndex, size_col2]
-000729f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00072a00: 2064 665f 636f 7079 2e61 745b 696e 6465   df_copy.at[inde
-00072a10: 782c 2073 697a 655f 636f 6c32 5d20 3d20  x, size_col2] = 
-00072a20: 300a 2020 2020 2020 2020 2020 2020 2020  0.              
-00072a30: 2020 6466 5f63 6f70 792e 6174 5b69 6e64    df_copy.at[ind
-00072a40: 6578 2c20 636f 6c32 5d20 3d20 4e6f 6e65  ex, col2] = None
-00072a50: 2020 2020 0a20 2020 2020 2020 2020 2020      .           
-00072a60: 2020 2020 2064 665f 636f 7079 2e61 745b       df_copy.at[
-00072a70: 696e 6465 782c 2069 6432 5d20 3d20 4e6f  index, id2] = No
-00072a80: 6e65 2020 2020 0a20 2020 2072 6574 7572  ne    .    retur
-00072a90: 6e20 6466 5f63 6f70 790a 0a0a 6465 6620  n df_copy...def 
-00072aa0: 7265 6e61 6d65 6974 2864 662c 206f 6c64  renameit(df, old
-00072ab0: 5f63 6f6c 5f6e 616d 652c 206e 6577 5f63  _col_name, new_c
-00072ac0: 6f6c 5f6e 616d 6529 3a0a 2020 2020 2222  ol_name):.    ""
-00072ad0: 220a 2020 2020 5265 6e61 6d65 7320 6120  ".    Renames a 
-00072ae0: 636f 6c75 6d6e 2069 6e20 6120 7061 6e64  column in a pand
-00072af0: 6173 2044 6174 6146 7261 6d65 2069 6e20  as DataFrame in 
-00072b00: 706c 6163 652e 2052 6169 7365 7320 616e  place. Raises an
-00072b10: 2065 7272 6f72 2069 6620 7468 6520 7370   error if the sp
-00072b20: 6563 6966 6965 6420 6f6c 6420 636f 6c75  ecified old colu
-00072b30: 6d6e 206e 616d 6520 646f 6573 206e 6f74  mn name does not
-00072b40: 2065 7869 7374 2e0a 0a20 2020 2050 6172   exist...    Par
-00072b50: 616d 6574 6572 733a 0a20 2020 202d 2064  ameters:.    - d
-00072b60: 663a 2070 616e 6461 732e 4461 7461 4672  f: pandas.DataFr
-00072b70: 616d 650a 2020 2020 2020 2020 5468 6520  ame.        The 
-00072b80: 4461 7461 4672 616d 6520 696e 2077 6869  DataFrame in whi
-00072b90: 6368 2074 6865 2063 6f6c 756d 6e20 6973  ch the column is
-00072ba0: 2074 6f20 6265 2072 656e 616d 6564 2e0a   to be renamed..
-00072bb0: 2020 2020 2d20 6f6c 645f 636f 6c5f 6e61      - old_col_na
-00072bc0: 6d65 3a20 7374 720a 2020 2020 2020 2020  me: str.        
-00072bd0: 5468 6520 6375 7272 656e 7420 6e61 6d65  The current name
-00072be0: 206f 6620 7468 6520 636f 6c75 6d6e 2074   of the column t
-00072bf0: 6f20 6265 2072 656e 616d 6564 2e0a 2020  o be renamed..  
-00072c00: 2020 2d20 6e65 775f 636f 6c5f 6e61 6d65    - new_col_name
-00072c10: 3a20 7374 720a 2020 2020 2020 2020 5468  : str.        Th
-00072c20: 6520 6e65 7720 6e61 6d65 2066 6f72 2074  e new name for t
-00072c30: 6865 2063 6f6c 756d 6e2e 0a20 2020 200a  he column..    .
-00072c40: 2020 2020 5261 6973 6573 3a0a 2020 2020      Raises:.    
-00072c50: 2d20 5661 6c75 6545 7272 6f72 3a20 4966  - ValueError: If
-00072c60: 2074 6865 206f 6c64 2063 6f6c 756d 6e20   the old column 
-00072c70: 6e61 6d65 2064 6f65 7320 6e6f 7420 6578  name does not ex
-00072c80: 6973 7420 696e 2074 6865 2044 6174 6146  ist in the DataF
-00072c90: 7261 6d65 2e0a 2020 2020 0a20 2020 2052  rame..    .    R
-00072ca0: 6574 7572 6e73 3a0a 2020 2020 4e6f 6e65  eturns:.    None
-00072cb0: 0a20 2020 2022 2222 0a20 2020 2069 6d70  .    """.    imp
-00072cc0: 6f72 7420 7761 726e 696e 6773 0a20 2020  ort warnings.   
-00072cd0: 2023 2043 6865 636b 2069 6620 7468 6520   # Check if the 
-00072ce0: 6f6c 6420 636f 6c75 6d6e 206e 616d 6520  old column name 
-00072cf0: 6578 6973 7473 2069 6e20 7468 6520 4461  exists in the Da
-00072d00: 7461 4672 616d 650a 2020 2020 6966 206f  taFrame.    if o
-00072d10: 6c64 5f63 6f6c 5f6e 616d 6520 6e6f 7420  ld_col_name not 
-00072d20: 696e 2064 662e 636f 6c75 6d6e 733a 0a20  in df.columns:. 
-00072d30: 2020 2020 2020 2077 6172 6e69 6e67 732e         warnings.
-00072d40: 7761 726e 2866 2254 6865 2063 6f6c 756d  warn(f"The colum
-00072d50: 6e20 277b 6f6c 645f 636f 6c5f 6e61 6d65  n '{old_col_name
-00072d60: 7d27 2064 6f65 7320 6e6f 7420 6578 6973  }' does not exis
-00072d70: 7420 696e 2074 6865 2044 6174 6146 7261  t in the DataFra
-00072d80: 6d65 2e22 290a 2020 2020 2020 2020 7265  me.").        re
-00072d90: 7475 726e 0a20 2020 200a 2020 2020 2320  turn.    .    # 
-00072da0: 5072 6f63 6565 6420 7769 7468 2072 656e  Proceed with ren
-00072db0: 616d 696e 6720 7468 6520 636f 6c75 6d6e  aming the column
-00072dc0: 2069 6620 6974 2065 7869 7374 730a 2020   if it exists.  
-00072dd0: 2020 6466 2e72 656e 616d 6528 636f 6c75    df.rename(colu
-00072de0: 6d6e 733d 7b6f 6c64 5f63 6f6c 5f6e 616d  mns={old_col_nam
-00072df0: 653a 206e 6577 5f63 6f6c 5f6e 616d 657d  e: new_col_name}
-00072e00: 2c20 696e 706c 6163 653d 5472 7565 290a  , inplace=True).
-00072e10: 0a0a 6465 6620 6d6d 5f6d 6174 6368 5f62  ..def mm_match_b
-00072e20: 795f 7163 5f73 636f 7269 6e67 5f61 6c6c  y_qc_scoring_all
-00072e30: 2820 7163 5f64 6174 6166 7261 6d65 2c20  ( qc_dataframe, 
-00072e40: 6669 785f 4c52 524c 3d54 7275 652c 2076  fix_LRRL=True, v
-00072e50: 6572 626f 7365 3d54 7275 6520 293a 0a20  erbose=True ):. 
-00072e60: 2020 2022 2222 0a20 2020 2050 726f 6365     """.    Proce
-00072e70: 7373 6573 2061 2071 7561 6c69 7479 2063  sses a quality c
-00072e80: 6f6e 7472 6f6c 2028 5143 2920 4461 7461  ontrol (QC) Data
-00072e90: 4672 616d 6520 746f 2070 6572 666f 726d  Frame to perform
-00072ea0: 206d 6f64 616c 6974 792d 7370 6563 6966   modality-specif
-00072eb0: 6963 206d 6174 6368 696e 6720 616e 6420  ic matching and 
-00072ec0: 6669 6c74 6572 696e 6720 6261 7365 640a  filtering based.
-00072ed0: 2020 2020 6f6e 2070 7265 6465 6669 6e65      on predefine
-00072ee0: 6420 6372 6974 6572 6961 2c20 6f70 7469  d criteria, opti
-00072ef0: 6d69 7a69 6e67 2066 6f72 206d 696e 696d  mizing for minim
-00072f00: 616c 206f 7574 6c69 6572 7320 616e 6420  al outliers and 
-00072f10: 6e6f 6973 652c 2061 6e64 206d 6178 696d  noise, and maxim
-00072f20: 616c 2073 6967 6e61 6c2d 746f 2d6e 6f69  al signal-to-noi
-00072f30: 7365 2072 6174 696f 2028 534e 5229 2c0a  se ratio (SNR),.
-00072f40: 2020 2020 6578 7065 6374 6564 2076 616c      expected val
-00072f50: 7565 206f 6620 7261 6e64 6f6d 6e65 7373  ue of randomness
-00072f60: 2028 4556 5229 2c20 616e 6420 6469 6d65   (EVR), and dime
-00072f70: 6e73 696f 6e61 6c69 7479 2074 696d 6520  nsionality time 
-00072f80: 2864 696d 7429 2e0a 0a20 2020 2054 6869  (dimt)...    Thi
-00072f90: 7320 6675 6e63 7469 6f6e 2069 7465 7261  s function itera
-00072fa0: 7469 7665 6c79 206d 6174 6368 6573 2064  tively matches d
-00072fb0: 6174 6166 7261 6d65 7320 6465 7269 7665  ataframes derive
-00072fc0: 6420 6672 6f6d 2074 6865 2051 4320 6461  d from the QC da
-00072fd0: 7461 6672 616d 6520 666f 7220 6469 6666  taframe for diff
-00072fe0: 6572 656e 7420 696d 6167 696e 6720 6d6f  erent imaging mo
-00072ff0: 6461 6c69 7469 6573 2c0a 2020 2020 6170  dalities,.    ap
-00073000: 706c 7969 6e67 2061 2073 6572 6965 7320  plying a series 
-00073010: 6f66 2066 696c 7465 7273 2074 6f20 7365  of filters to se
-00073020: 6c65 6374 2074 6865 2062 6573 7420 6d61  lect the best ma
-00073030: 7463 6865 7320 6261 7365 6420 6f6e 2074  tches based on t
-00073040: 6865 2051 4320 6d65 7472 6963 732e 204d  he QC metrics. M
-00073050: 6174 6368 6573 2061 7265 206d 6164 6520  atches are made 
-00073060: 7769 7468 0a20 2020 2063 6f6e 7369 6465  with.    conside
-00073070: 7261 7469 6f6e 2074 6f20 6d69 6e69 6d69  ration to minimi
-00073080: 7a65 206f 7574 6c69 6572 206c 6f6f 7020  ze outlier loop 
-00073090: 616e 6420 6e6f 6973 652c 2077 6869 6c65  and noise, while
-000730a0: 206d 6178 696d 697a 696e 6720 534e 522c   maximizing SNR,
-000730b0: 2045 5652 2c20 616e 6420 6469 6d74 2066   EVR, and dimt f
-000730c0: 6f72 2065 6163 6820 6d6f 6461 6c69 7479  or each modality
-000730d0: 2e0a 0a20 2020 2050 6172 616d 6574 6572  ...    Parameter
-000730e0: 733a 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  s:.    ---------
-000730f0: 2d0a 2020 2020 7163 5f64 6174 6166 7261  -.    qc_datafra
-00073100: 6d65 203a 2070 616e 6461 732e 4461 7461  me : pandas.Data
-00073110: 4672 616d 650a 2020 2020 2020 2020 5468  Frame.        Th
-00073120: 6520 4461 7461 4672 616d 6520 636f 6e74  e DataFrame cont
-00073130: 6169 6e69 6e67 2051 4320 6d65 7472 6963  aining QC metric
-00073140: 7320 666f 7220 6469 6666 6572 656e 7420  s for different 
-00073150: 6d6f 6461 6c69 7469 6573 2061 6e64 2069  modalities and i
-00073160: 6d61 6769 6e67 2064 6174 612e 0a20 2020  maging data..   
-00073170: 2066 6978 5f4c 5252 4c20 3a20 626f 6f6c   fix_LRRL : bool
-00073180: 2c20 6f70 7469 6f6e 616c 0a0a 2020 2020  , optional..    
-00073190: 7665 7262 6f73 6520 3a20 626f 6f6c 2c20  verbose : bool, 
-000731a0: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
-000731b0: 2049 6620 5472 7565 2c20 7072 696e 7473   If True, prints
-000731c0: 2074 6865 2070 726f 6772 6573 7320 616e   the progress an
-000731d0: 6420 7468 6520 7368 6170 6520 6f66 2074  d the shape of t
-000731e0: 6865 2044 6174 6146 7261 6d65 2062 6569  he DataFrame bei
-000731f0: 6e67 2070 726f 6365 7373 6564 2069 6e20  ng processed in 
-00073200: 6561 6368 2073 7465 702e 0a0a 2020 2020  each step...    
-00073210: 5072 6f63 6573 733a 0a20 2020 202d 2d2d  Process:.    ---
-00073220: 2d2d 2d2d 0a20 2020 2031 2e20 5374 616e  ----.    1. Stan
-00073230: 6461 7264 697a 6573 206d 6f64 616c 6974  dardizes modalit
-00073240: 6965 7320 6279 206d 6572 6769 6e67 2044  ies by merging D
-00073250: 5449 2d72 656c 6174 6564 2065 6e74 7269  TI-related entri
-00073260: 6573 2e0a 2020 2020 322e 2043 6f6e 7665  es..    2. Conve
-00073270: 7274 7320 7370 6563 6966 6963 2063 6f6c  rts specific col
-00073280: 756d 6e73 2074 6f20 6170 7072 6f70 7269  umns to appropri
-00073290: 6174 6520 6461 7461 2074 7970 6573 2066  ate data types f
-000732a0: 6f72 2070 726f 6365 7373 696e 672e 0a20  or processing.. 
-000732b0: 2020 2033 2e20 5065 7266 6f72 6d73 206d     3. Performs m
-000732c0: 6f64 616c 6974 792d 7370 6563 6966 6963  odality-specific
-000732d0: 206d 6174 6368 696e 6720 616e 6420 6669   matching and fi
-000732e0: 6c74 6572 696e 6720 6261 7365 6420 6f6e  ltering based on
-000732f0: 2074 6865 206f 7574 6c69 6572 2063 6f6c   the outlier col
-00073300: 756d 6e20 616e 6420 6372 6974 6572 6961  umn and criteria
-00073310: 2066 6f72 2065 6163 6820 6d6f 6461 6c69   for each modali
-00073320: 7479 2e0a 2020 2020 342e 2049 7465 7261  ty..    4. Itera
-00073330: 7469 7665 6c79 2070 726f 6365 7373 6573  tively processes
-00073340: 2075 6e6d 6174 6368 6564 2064 6174 6120   unmatched data 
-00073350: 666f 7220 7072 6564 6566 696e 6564 206d  for predefined m
-00073360: 6f64 616c 6974 6965 7320 7769 7468 2073  odalities with s
-00073370: 7065 6369 6669 6320 7072 6566 6978 6573  pecific prefixes
-00073380: 2074 6f20 6669 6e64 2066 7572 7468 6572   to find further
-00073390: 206d 6174 6368 6573 2e0a 2020 2020 0a20   matches..    . 
-000733a0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-000733b0: 2d2d 2d2d 2d2d 2d0a 2020 2020 7061 6e64  -------.    pand
-000733c0: 6173 2e44 6174 6146 7261 6d65 0a20 2020  as.DataFrame.   
-000733d0: 2020 2020 2054 6865 206d 6174 6368 6564       The matched
-000733e0: 2061 6e64 2066 696c 7465 7265 6420 4461   and filtered Da
-000733f0: 7461 4672 616d 6520 6166 7465 7220 6170  taFrame after ap
-00073400: 706c 7969 6e67 2061 6c6c 2051 4320 7363  plying all QC sc
-00073410: 6f72 696e 6720 616e 6420 6d61 7463 6869  oring and matchi
-00073420: 6e67 206f 7065 7261 7469 6f6e 7320 6163  ng operations ac
-00073430: 726f 7373 2073 7065 6369 6669 6564 206d  ross specified m
-00073440: 6f64 616c 6974 6965 732e 0a0a 2020 2020  odalities...    
-00073450: 2222 220a 2020 2020 7163 5f64 6174 6166  """.    qc_dataf
-00073460: 7261 6d65 5b27 6d6f 6461 6c69 7479 275d  rame['modality']
-00073470: 203d 2071 635f 6461 7461 6672 616d 655b   = qc_dataframe[
-00073480: 276d 6f64 616c 6974 7927 5d2e 7265 706c  'modality'].repl
-00073490: 6163 6528 5b27 4454 4964 7769 272c 2027  ace(['DTIdwi', '
-000734a0: 4454 4962 3027 5d2c 2027 4454 4927 2c20  DTIb0'], 'DTI', 
-000734b0: 7265 6765 783d 5472 7565 290a 2020 2020  regex=True).    
-000734c0: 7163 5f64 6174 6166 7261 6d65 5b27 6669  qc_dataframe['fi
-000734d0: 6c65 6e61 6d65 275d 3d71 635f 6461 7461  lename']=qc_data
-000734e0: 6672 616d 655b 2766 696c 656e 616d 6527  frame['filename'
-000734f0: 5d2e 6173 7479 7065 2873 7472 290a 2020  ].astype(str).  
-00073500: 2020 7163 5f64 6174 6166 7261 6d65 5b27    qc_dataframe['
-00073510: 6f6c 5f6c 6f6f 7027 5d3d 7163 5f64 6174  ol_loop']=qc_dat
-00073520: 6166 7261 6d65 5b27 6f6c 5f6c 6f6f 7027  aframe['ol_loop'
-00073530: 5d2e 6173 7479 7065 2866 6c6f 6174 290a  ].astype(float).
-00073540: 2020 2020 7163 5f64 6174 6166 7261 6d65      qc_dataframe
-00073550: 5b27 6f6c 5f6c 6f66 275d 3d71 635f 6461  ['ol_lof']=qc_da
-00073560: 7461 6672 616d 655b 276f 6c5f 6c6f 6627  taframe['ol_lof'
-00073570: 5d2e 6173 7479 7065 2866 6c6f 6174 290a  ].astype(float).
-00073580: 2020 2020 7163 5f64 6174 6166 7261 6d65      qc_dataframe
-00073590: 5b27 6f6c 5f6c 6f66 5f64 6563 6973 696f  ['ol_lof_decisio
-000735a0: 6e27 5d3d 7163 5f64 6174 6166 7261 6d65  n']=qc_dataframe
-000735b0: 5b27 6f6c 5f6c 6f66 5f64 6563 6973 696f  ['ol_lof_decisio
-000735c0: 6e27 5d2e 6173 7479 7065 2866 6c6f 6174  n'].astype(float
-000735d0: 290a 2020 2020 6f75 746c 6965 725f 636f  ).    outlier_co
-000735e0: 6c75 6d6e 3d27 6f6c 5f6c 6f6f 7027 0a20  lumn='ol_loop'. 
-000735f0: 2020 206d 6d64 6630 203d 2062 6573 745f     mmdf0 = best_
-00073600: 6d6d 6d28 2071 635f 6461 7461 6672 616d  mmm( qc_datafram
-00073610: 652c 2027 5431 7727 2c20 6f75 746c 6965  e, 'T1w', outlie
-00073620: 725f 636f 6c75 6d6e 3d6f 7574 6c69 6572  r_column=outlier
-00073630: 5f63 6f6c 756d 6e20 295b 2766 696c 7427  _column )['filt'
-00073640: 5d0a 2020 2020 666c 6466 203d 2062 6573  ].    fldf = bes
-00073650: 745f 6d6d 6d28 2071 635f 6461 7461 6672  t_mmm( qc_datafr
-00073660: 616d 652c 2027 5432 466c 6169 7227 2c20  ame, 'T2Flair', 
-00073670: 6f75 746c 6965 725f 636f 6c75 6d6e 3d6f  outlier_column=o
-00073680: 7574 6c69 6572 5f63 6f6c 756d 6e20 295b  utlier_column )[
-00073690: 2766 696c 7427 5d0a 2020 2020 6e6d 6466  'filt'].    nmdf
-000736a0: 203d 2062 6573 745f 6d6d 6d28 2071 635f   = best_mmm( qc_
-000736b0: 6461 7461 6672 616d 652c 2027 4e4d 3244  dataframe, 'NM2D
-000736c0: 4d54 272c 206f 7574 6c69 6572 5f63 6f6c  MT', outlier_col
-000736d0: 756d 6e3d 6f75 746c 6965 725f 636f 6c75  umn=outlier_colu
-000736e0: 6d6e 2029 5b27 6669 6c74 275d 0a20 2020  mn )['filt'].   
-000736f0: 2072 7364 6620 3d20 6265 7374 5f6d 6d6d   rsdf = best_mmm
-00073700: 2820 7163 5f64 6174 6166 7261 6d65 2c20  ( qc_dataframe, 
-00073710: 2772 7366 4d52 4927 2c20 6f75 746c 6965  'rsfMRI', outlie
-00073720: 725f 636f 6c75 6d6e 3d6f 7574 6c69 6572  r_column=outlier
-00073730: 5f63 6f6c 756d 6e20 295b 2766 696c 7427  _column )['filt'
-00073740: 5d0a 2020 2020 6474 6466 203d 2062 6573  ].    dtdf = bes
-00073750: 745f 6d6d 6d28 2071 635f 6461 7461 6672  t_mmm( qc_datafr
-00073760: 616d 652c 2027 4454 4927 2c20 6f75 746c  ame, 'DTI', outl
-00073770: 6965 725f 636f 6c75 6d6e 3d6f 7574 6c69  ier_column=outli
-00073780: 6572 5f63 6f6c 756d 6e20 295b 2766 696c  er_column )['fil
-00073790: 7427 5d0a 0a20 2020 2063 7269 7465 7269  t']..    criteri
-000737a0: 6120 3d20 7b27 6f6c 5f6c 6f6f 7027 3a20  a = {'ol_loop': 
-000737b0: 276d 696e 272c 2027 6e6f 6973 6527 3a20  'min', 'noise': 
-000737c0: 276d 696e 272c 2027 736e 7227 3a20 276d  'min', 'snr': 'm
-000737d0: 6178 272c 2027 4556 5227 3a20 276d 6178  ax', 'EVR': 'max
-000737e0: 272c 2027 7265 666c 6563 7469 6f6e 5f65  ', 'reflection_e
-000737f0: 7272 273a 276d 696e 277d 0a20 2020 2078  rr':'min'}.    x
-00073800: 636c 203d 205b 2027 6d72 696d 6667 272c  cl = [ 'mrimfg',
-00073810: 2027 6d72 696d 6f64 656c 272c 276d 7269   'mrimodel','mri
-00073820: 4d61 676e 6574 6963 4669 656c 6453 7472  MagneticFieldStr
-00073830: 656e 6774 6827 2c20 2764 7469 5f66 6169  ength', 'dti_fai
-00073840: 6c65 6427 2c20 2772 7366 5f66 6169 6c65  led', 'rsf_faile
-00073850: 6427 2c20 2773 7562 6a65 6374 4944 272c  d', 'subjectID',
-00073860: 2027 6461 7465 272c 2027 7375 626a 6563   'date', 'subjec
-00073870: 7449 4464 6174 6527 2c27 7265 7065 6174  tIDdate','repeat
-00073880: 275d 0a20 2020 2023 2041 7373 756d 696e  '].    # Assumin
-00073890: 6720 6466 5f61 2061 6e64 2064 665f 6220  g df_a and df_b 
-000738a0: 6172 6520 616c 7265 6164 7920 6c6f 6164  are already load
-000738b0: 6564 0a20 2020 206d 6d64 662c 2075 6e64  ed.    mmdf, und
-000738c0: 6666 6c20 3d20 6d6d 5f6d 6174 6368 5f62  ffl = mm_match_b
-000738d0: 795f 7163 5f73 636f 7269 6e67 286d 6d64  y_qc_scoring(mmd
-000738e0: 6630 2c20 666c 6466 2c20 2773 7562 6a65  f0, fldf, 'subje
-000738f0: 6374 4944 6461 7465 272c 2063 7269 7465  ctIDdate', crite
-00073900: 7269 612c 200a 2020 2020 2020 2020 2020  ria, .          
-00073910: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00073920: 6566 6978 3d27 5432 466c 6169 725f 272c  efix='T2Flair_',
-00073930: 2065 7863 6c75 6465 5f63 6f6c 756d 6e73   exclude_columns
-00073940: 3d78 636c 2029 0a0a 2020 2020 7072 6566  =xcl )..    pref
-00073950: 6978 6573 203d 205b 274e 4d31 5f27 2c20  ixes = ['NM1_', 
-00073960: 274e 4d32 5f27 2c20 274e 4d33 5f27 2c20  'NM2_', 'NM3_', 
-00073970: 274e 4d34 5f27 2c20 274e 4d35 5f27 2c20  'NM4_', 'NM5_', 
-00073980: 274e 4d36 5f27 5d20 200a 2020 2020 756e  'NM6_']  .    un
-00073990: 6466 6d6f 6420 3d20 6e6d 6466 2020 2320  dfmod = nmdf  # 
-000739a0: 496e 6974 6961 6c69 7a65 2027 756e 6466  Initialize 'undf
-000739b0: 6d6f 6427 2077 6974 6820 276e 6d64 6627  mod' with 'nmdf'
-000739c0: 2066 6f72 2074 6865 2066 6972 7374 2069   for the first i
-000739d0: 7465 7261 7469 6f6e 0a20 2020 2069 6620  teration.    if 
-000739e0: 7665 7262 6f73 653a 0a20 2020 2020 2020  verbose:.       
-000739f0: 2070 7269 6e74 2827 7374 6172 7420 4e4d   print('start NM
-00073a00: 2729 0a20 2020 2020 2020 2070 7269 6e74  ').        print
-00073a10: 2820 756e 6466 6d6f 642e 7368 6170 6520  ( undfmod.shape 
-00073a20: 290a 2020 2020 666f 7220 7072 6566 6978  ).    for prefix
-00073a30: 2069 6e20 7072 6566 6978 6573 3a0a 2020   in prefixes:.  
-00073a40: 2020 2020 2020 6966 2075 6e64 666d 6f64        if undfmod
-00073a50: 2e73 6861 7065 5b30 5d20 3e20 3530 3a0a  .shape[0] > 50:.
-00073a60: 2020 2020 2020 2020 2020 2020 6d6d 6466              mmdf
-00073a70: 2c20 756e 6466 6d6f 6420 3d20 6d6d 5f6d  , undfmod = mm_m
-00073a80: 6174 6368 5f62 795f 7163 5f73 636f 7269  atch_by_qc_scori
-00073a90: 6e67 286d 6d64 662c 2075 6e64 666d 6f64  ng(mmdf, undfmod
-00073aa0: 2c20 2773 7562 6a65 6374 4944 6461 7465  , 'subjectIDdate
-00073ab0: 272c 2063 7269 7465 7269 612c 2070 7265  ', criteria, pre
-00073ac0: 6669 783d 7072 6566 6978 2c20 6578 636c  fix=prefix, excl
-00073ad0: 7564 655f 636f 6c75 6d6e 733d 7863 6c29  ude_columns=xcl)
-00073ae0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00073af0: 7665 7262 6f73 653a 0a20 2020 2020 2020  verbose:.       
-00073b00: 2020 2020 2020 2020 2070 7269 6e74 2820           print( 
-00073b10: 7072 6566 6978 2029 0a20 2020 2020 2020  prefix ).       
-00073b20: 2020 2020 2020 2020 2070 7269 6e74 2820           print( 
-00073b30: 756e 6466 6d6f 642e 7368 6170 6520 290a  undfmod.shape ).
-00073b40: 0a20 2020 2063 7269 7465 7269 6120 3d20  .    criteria = 
-00073b50: 7b27 6f6c 5f6c 6f6f 7027 3a20 276d 696e  {'ol_loop': 'min
-00073b60: 272c 2027 6e6f 6973 6527 3a20 276d 696e  ', 'noise': 'min
-00073b70: 272c 2027 736e 7227 3a20 276d 6178 272c  ', 'snr': 'max',
-00073b80: 2027 4556 5227 3a20 276d 6178 272c 2027   'EVR': 'max', '
-00073b90: 6469 6d74 273a 276d 6178 277d 0a20 2020  dimt':'max'}.   
-00073ba0: 2023 2068 6967 6865 7220 6276 616c 7565   # higher bvalue
-00073bb0: 7320 6c65 6164 2074 6f20 6d6f 7265 206e  s lead to more n
-00073bc0: 6f69 7365 202e 2e2e 0a20 2020 2063 7269  oise ....    cri
-00073bd0: 7465 7269 6120 3d20 7b27 6f6c 5f6c 6f6f  teria = {'ol_loo
-00073be0: 7027 3a20 276d 696e 272c 2027 6e6f 6973  p': 'min', 'nois
-00073bf0: 6527 3a20 276d 696e 272c 2020 2764 7469  e': 'min',  'dti
-00073c00: 5f62 7661 6c75 654d 6178 273a 276d 696e  _bvalueMax':'min
-00073c10: 272c 2020 2764 696d 7427 3a27 6d61 7827  ',  'dimt':'max'
-00073c20: 7d0a 2020 2020 7072 6566 6978 6573 203d  }.    prefixes =
-00073c30: 205b 2744 5449 315f 272c 2027 4454 4932   ['DTI1_', 'DTI2
-00073c40: 5f27 2c20 2744 5449 335f 275d 2020 2320  _', 'DTI3_']  # 
-00073c50: 4c69 7374 206f 6620 7072 6566 6978 6573  List of prefixes
-00073c60: 2066 6f72 2065 6163 6820 6d61 7463 6869   for each matchi
-00073c70: 6e67 2069 7465 7261 7469 6f6e 0a20 2020  ng iteration.   
-00073c80: 2075 6e64 666d 6f64 203d 2064 7464 660a   undfmod = dtdf.
-00073c90: 2020 2020 6966 2076 6572 626f 7365 3a0a      if verbose:.
-00073ca0: 2020 2020 2020 2020 7072 696e 7428 2773          print('s
-00073cb0: 7461 7274 2044 5427 290a 2020 2020 2020  tart DT').      
-00073cc0: 2020 7072 696e 7428 2075 6e64 666d 6f64    print( undfmod
-00073cd0: 2e73 6861 7065 2029 0a20 2020 2066 6f72  .shape ).    for
-00073ce0: 2070 7265 6669 7820 696e 2070 7265 6669   prefix in prefi
-00073cf0: 7865 733a 0a20 2020 2020 2020 2069 6620  xes:.        if 
-00073d00: 756e 6466 6d6f 642e 7368 6170 655b 305d  undfmod.shape[0]
-00073d10: 203e 2035 303a 0a20 2020 2020 2020 2020   > 50:.         
-00073d20: 2020 206d 6d64 662c 2075 6e64 666d 6f64     mmdf, undfmod
-00073d30: 203d 206d 6d5f 6d61 7463 685f 6279 5f71   = mm_match_by_q
-00073d40: 635f 7363 6f72 696e 6728 6d6d 6466 2c20  c_scoring(mmdf, 
-00073d50: 756e 6466 6d6f 642c 2027 7375 626a 6563  undfmod, 'subjec
-00073d60: 7449 4464 6174 6527 2c20 6372 6974 6572  tIDdate', criter
-00073d70: 6961 2c20 7072 6566 6978 3d70 7265 6669  ia, prefix=prefi
-00073d80: 782c 2065 7863 6c75 6465 5f63 6f6c 756d  x, exclude_colum
-00073d90: 6e73 3d78 636c 290a 2020 2020 2020 2020  ns=xcl).        
-00073da0: 2020 2020 6966 2076 6572 626f 7365 3a0a      if verbose:.
-00073db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00073dc0: 7072 696e 7428 2070 7265 6669 7820 290a  print( prefix ).
-00073dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00073de0: 7072 696e 7428 2075 6e64 666d 6f64 2e73  print( undfmod.s
-00073df0: 6861 7065 2029 0a0a 2020 2020 7072 6566  hape )..    pref
-00073e00: 6978 6573 203d 205b 2772 7366 315f 272c  ixes = ['rsf1_',
-00073e10: 2027 7273 6632 5f27 2c20 2772 7366 335f   'rsf2_', 'rsf3_
-00073e20: 275d 2020 2320 4c69 7374 206f 6620 7072  ']  # List of pr
-00073e30: 6566 6978 6573 2066 6f72 2065 6163 6820  efixes for each 
-00073e40: 6d61 7463 6869 6e67 2069 7465 7261 7469  matching iterati
-00073e50: 6f6e 0a20 2020 2075 6e64 666d 6f64 203d  on.    undfmod =
-00073e60: 2072 7364 6620 2023 2049 6e69 7469 616c   rsdf  # Initial
-00073e70: 697a 6520 2775 6e64 666d 6f64 2720 7769  ize 'undfmod' wi
-00073e80: 7468 2027 6e6d 6466 2720 666f 7220 7468  th 'nmdf' for th
-00073e90: 6520 6669 7273 7420 6974 6572 6174 696f  e first iteratio
-00073ea0: 6e0a 2020 2020 6966 2076 6572 626f 7365  n.    if verbose
-00073eb0: 3a0a 2020 2020 2020 2020 7072 696e 7428  :.        print(
-00073ec0: 2773 7461 7274 2072 7366 2729 0a20 2020  'start rsf').   
-00073ed0: 2020 2020 2070 7269 6e74 2820 756e 6466       print( undf
-00073ee0: 6d6f 642e 7368 6170 6520 290a 2020 2020  mod.shape ).    
-00073ef0: 666f 7220 7072 6566 6978 2069 6e20 7072  for prefix in pr
-00073f00: 6566 6978 6573 3a0a 2020 2020 2020 2020  efixes:.        
-00073f10: 6966 2075 6e64 666d 6f64 2e73 6861 7065  if undfmod.shape
-00073f20: 5b30 5d20 3e20 3530 3a0a 2020 2020 2020  [0] > 50:.      
-00073f30: 2020 2020 2020 6d6d 6466 2c20 756e 6466        mmdf, undf
-00073f40: 6d6f 6420 3d20 6d6d 5f6d 6174 6368 5f62  mod = mm_match_b
-00073f50: 795f 7163 5f73 636f 7269 6e67 286d 6d64  y_qc_scoring(mmd
-00073f60: 662c 2075 6e64 666d 6f64 2c20 2773 7562  f, undfmod, 'sub
-00073f70: 6a65 6374 4944 6461 7465 272c 2063 7269  jectIDdate', cri
-00073f80: 7465 7269 612c 2070 7265 6669 783d 7072  teria, prefix=pr
-00073f90: 6566 6978 2c20 6578 636c 7564 655f 636f  efix, exclude_co
-00073fa0: 6c75 6d6e 733d 7863 6c29 0a20 2020 2020  lumns=xcl).     
-00073fb0: 2020 2020 2020 2069 6620 7665 7262 6f73         if verbos
-00073fc0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00073fd0: 2020 2070 7269 6e74 2820 7072 6566 6978     print( prefix
-00073fe0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-00073ff0: 2020 2070 7269 6e74 2820 756e 6466 6d6f     print( undfmo
-00074000: 642e 7368 6170 6520 290a 2020 2020 0a20  d.shape ).    . 
-00074010: 2020 2069 6620 6669 785f 4c52 524c 3a0a     if fix_LRRL:.
-00074020: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-00074030: 206d 6d64 663d 6669 785f 4c52 5f52 4c5f   mmdf=fix_LR_RL_
-00074040: 7374 7566 6628 206d 6d64 662c 2027 4454  stuff( mmdf, 'DT
-00074050: 4931 5f66 696c 656e 616d 6527 2c20 2744  I1_filename', 'D
-00074060: 5449 325f 6669 6c65 6e61 6d65 272c 2027  TI2_filename', '
-00074070: 4454 4931 5f64 696d 7427 2c20 2744 5449  DTI1_dimt', 'DTI
-00074080: 325f 6469 6d74 2729 0a20 2020 2020 2020  2_dimt').       
-00074090: 206d 6d64 663d 6669 785f 4c52 5f52 4c5f   mmdf=fix_LR_RL_
-000740a0: 7374 7566 6628 206d 6d64 662c 2027 7273  stuff( mmdf, 'rs
-000740b0: 6631 5f66 696c 656e 616d 6527 2c20 2772  f1_filename', 'r
-000740c0: 7366 325f 6669 6c65 6e61 6d65 272c 2027  sf2_filename', '
-000740d0: 7273 6631 5f64 696d 7427 2c20 2772 7366  rsf1_dimt', 'rsf
-000740e0: 325f 6469 6d74 272c 2027 7273 6631 5f69  2_dimt', 'rsf1_i
-000740f0: 6d61 6765 4944 272c 2027 7273 6632 5f69  mageID', 'rsf2_i
-00074100: 6d61 6765 4944 2720 2029 0a20 2020 2065  mageID'  ).    e
-00074110: 6c73 653a 0a20 2020 2020 2020 2069 6d70  lse:.        imp
-00074120: 6f72 7420 7761 726e 696e 6773 0a20 2020  ort warnings.   
-00074130: 2020 2020 2077 6172 6e69 6e67 732e 7761       warnings.wa
-00074140: 726e 2822 4649 584d 453a 2073 686f 756c  rn("FIXME: shoul
-00074150: 6420 6669 7820 4c52 2061 6e64 2052 4c20  d fix LR and RL 
-00074160: 7369 7475 6174 696f 6e20 666f 7220 7468  situation for th
-00074170: 6520 4454 4920 616e 6420 7273 664d 5249  e DTI and rsfMRI
-00074180: 2229 0a0a 2020 2020 2320 6e6f 7720 646f  ")..    # now do
-00074190: 2074 6865 206e 6563 6573 7361 7279 2072   the necessary r
-000741a0: 6570 6c61 6365 6d65 6e74 730a 2020 2020  eplacements.    
-000741b0: 0a20 2020 2072 656e 616d 6569 7428 206d  .    renameit( m
-000741c0: 6d64 662c 2027 7065 7266 5f69 6d61 6765  mdf, 'perf_image
-000741d0: 4944 272c 2027 7065 7266 6964 2720 290a  ID', 'perfid' ).
-000741e0: 2020 2020 7265 6e61 6d65 6974 2820 6d6d      renameit( mm
-000741f0: 6466 2c20 2770 6572 665f 6669 6c65 6e61  df, 'perf_filena
-00074200: 6d65 272c 2027 7065 7266 666e 2720 290a  me', 'perffn' ).
-00074210: 2020 2020 7265 6e61 6d65 6974 2820 6d6d      renameit( mm
-00074220: 6466 2c20 2754 3246 6c61 6972 5f69 6d61  df, 'T2Flair_ima
-00074230: 6765 4944 272c 2027 666c 6169 7269 6427  geID', 'flairid'
-00074240: 2029 0a20 2020 2072 656e 616d 6569 7428   ).    renameit(
-00074250: 206d 6d64 662c 2027 5432 466c 6169 725f   mmdf, 'T2Flair_
-00074260: 6669 6c65 6e61 6d65 272c 2027 666c 6169  filename', 'flai
-00074270: 7266 6e27 2029 0a20 2020 2072 656e 616d  rfn' ).    renam
-00074280: 6569 7428 206d 6d64 662c 2027 7273 6631  eit( mmdf, 'rsf1
-00074290: 5f69 6d61 6765 4944 272c 2027 7273 6669  _imageID', 'rsfi
-000742a0: 6431 2720 290a 2020 2020 7265 6e61 6d65  d1' ).    rename
-000742b0: 6974 2820 6d6d 6466 2c20 2772 7366 325f  it( mmdf, 'rsf2_
-000742c0: 696d 6167 6549 4427 2c20 2772 7366 6964  imageID', 'rsfid
-000742d0: 3227 2029 0a20 2020 2072 656e 616d 6569  2' ).    renamei
-000742e0: 7428 206d 6d64 662c 2027 7273 6631 5f66  t( mmdf, 'rsf1_f
-000742f0: 696c 656e 616d 6527 2c20 2772 7366 666e  ilename', 'rsffn
-00074300: 3127 2029 0a20 2020 2072 656e 616d 6569  1' ).    renamei
-00074310: 7428 206d 6d64 662c 2027 7273 6632 5f66  t( mmdf, 'rsf2_f
-00074320: 696c 656e 616d 6527 2c20 2772 7366 666e  ilename', 'rsffn
-00074330: 3227 2029 0a20 2020 2072 656e 616d 6569  2' ).    renamei
-00074340: 7428 206d 6d64 662c 2027 4454 4931 5f69  t( mmdf, 'DTI1_i
-00074350: 6d61 6765 4944 272c 2027 6474 6964 3127  mageID', 'dtid1'
-00074360: 2029 0a20 2020 2072 656e 616d 6569 7428   ).    renameit(
-00074370: 206d 6d64 662c 2027 4454 4932 5f69 6d61   mmdf, 'DTI2_ima
-00074380: 6765 4944 272c 2027 6474 6964 3227 2029  geID', 'dtid2' )
-00074390: 0a20 2020 2072 656e 616d 6569 7428 206d  .    renameit( m
-000743a0: 6d64 662c 2027 4454 4933 5f69 6d61 6765  mdf, 'DTI3_image
-000743b0: 4944 272c 2027 6474 6964 3327 2029 0a20  ID', 'dtid3' ). 
-000743c0: 2020 2072 656e 616d 6569 7428 206d 6d64     renameit( mmd
-000743d0: 662c 2027 4454 4931 5f66 696c 656e 616d  f, 'DTI1_filenam
-000743e0: 6527 2c20 2764 7466 6e31 2720 290a 2020  e', 'dtfn1' ).  
-000743f0: 2020 7265 6e61 6d65 6974 2820 6d6d 6466    renameit( mmdf
-00074400: 2c20 2744 5449 325f 6669 6c65 6e61 6d65  , 'DTI2_filename
-00074410: 272c 2027 6474 666e 3227 2029 0a20 2020  ', 'dtfn2' ).   
-00074420: 2072 656e 616d 6569 7428 206d 6d64 662c   renameit( mmdf,
-00074430: 2027 4454 4933 5f66 696c 656e 616d 6527   'DTI3_filename'
-00074440: 2c20 2764 7466 6e33 2720 290a 2020 2020  , 'dtfn3' ).    
-00074450: 666f 7220 7820 696e 2072 616e 6765 2831  for x in range(1
-00074460: 2c36 293a 0a20 2020 2020 2020 2074 656d  ,6):.        tem
-00074470: 7030 3d22 4e4d 222b 7374 7228 7829 2b22  p0="NM"+str(x)+"
-00074480: 5f69 6d61 6765 4944 220a 2020 2020 2020  _imageID".      
-00074490: 2020 7465 6d70 313d 226e 6d69 6422 2b73    temp1="nmid"+s
-000744a0: 7472 2878 290a 2020 2020 2020 2020 7265  tr(x).        re
-000744b0: 6e61 6d65 6974 2820 6d6d 6466 2c20 7465  nameit( mmdf, te
-000744c0: 6d70 302c 2074 656d 7031 2029 0a20 2020  mp0, temp1 ).   
-000744d0: 2020 2020 2074 656d 7030 3d22 4e4d 222b       temp0="NM"+
-000744e0: 7374 7228 7829 2b22 5f66 696c 656e 616d  str(x)+"_filenam
-000744f0: 6522 0a20 2020 2020 2020 2074 656d 7031  e".        temp1
-00074500: 3d22 6e6d 666e 222b 7374 7228 7829 0a20  ="nmfn"+str(x). 
-00074510: 2020 2020 2020 2072 656e 616d 6569 7428         renameit(
-00074520: 206d 6d64 662c 2074 656d 7030 2c20 7465   mmdf, temp0, te
-00074530: 6d70 3120 290a 2020 2020 7265 7475 726e  mp1 ).    return
-00074540: 206d 6d64 660a                            mmdf.
+0006ff00: 2020 2020 2020 206d 796d 6f64 6964 203d         mymodid =
+0006ff10: 206f 732e 7061 7468 2e73 706c 6974 6578   os.path.splitex
+0006ff20: 7428 206d 796d 6f64 6964 2029 5b30 5d0a  t( mymodid )[0].
+0006ff30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0006ff40: 2020 2020 2020 2020 7465 6d70 203d 206d          temp = m
+0006ff50: 796d 6f64 6964 2e73 706c 6974 2820 6964  ymodid.split( id
+0006ff60: 7365 7020 290a 2020 2020 2020 2020 2020  sep ).          
+0006ff70: 2020 2020 2020 2020 2020 2020 2020 6d79                my
+0006ff80: 6d6f 6469 6420 3d20 7465 6d70 5b20 6c65  modid = temp[ le
+0006ff90: 6e28 2074 656d 7020 292d 3120 5d0a 2020  n( temp )-1 ].  
+0006ffa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0006ffb0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0006ffc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0006ffd0: 6966 2076 6572 626f 7365 3a0a 2020 2020  if verbose:.    
+0006ffe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0006fff0: 2020 2020 2020 2020 7072 696e 7428 226d          print("m
+00070000: 6973 7369 6e67 2229 0a20 2020 2020 2020  issing").       
+00070010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00070020: 2063 6f6e 7469 6e75 650a 2020 2020 2020   continue.      
+00070030: 2020 2020 2020 2020 2020 6966 2076 6572            if ver
+00070040: 626f 7365 3a0a 2020 2020 2020 2020 2020  bose:.          
+00070050: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00070060: 2022 6d6f 6461 6c69 7479 2069 6420 6973   "modality id is
+00070070: 2022 202b 206d 796d 6f64 6964 202b 2022   " + mymodid + "
+00070080: 2066 6f72 206d 6f64 616c 6974 7920 2220   for modality " 
+00070090: 2b20 6d6f 6461 6c69 7479 636c 6173 7320  + modalityclass 
+000700a0: 2b20 2720 6d6f 6461 6c69 7479 2073 7065  + ' modality spe
+000700b0: 6369 6669 6320 7375 626a 2027 202b 2073  cific subj ' + s
+000700c0: 6964 202b 2027 206d 6f64 616c 6974 7920  id + ' modality 
+000700d0: 7370 6563 6966 6963 2069 6420 6973 2027  specific id is '
+000700e0: 202b 206d 7969 6420 2b20 2220 6974 7320   + myid + " its 
+000700f0: 6461 7465 2022 202b 2020 6d79 6461 7465  date " +  mydate
+00070100: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+00070110: 2020 206d 6f64 616c 6974 7963 6c61 7373     modalityclass
+00070120: 7365 6172 6368 203d 206d 6f64 616c 6974  search = modalit
+00070130: 7963 6c61 7373 0a20 2020 2020 2020 2020  yclass.         
+00070140: 2020 2020 2020 2069 6620 6d6f 6461 6c69         if modali
+00070150: 7479 636c 6173 7320 696e 205b 2772 7366  tyclass in ['rsf
+00070160: 4d52 4927 2c27 4454 4927 5d3a 0a20 2020  MRI','DTI']:.   
+00070170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00070180: 206d 6f64 616c 6974 7963 6c61 7373 7365   modalityclassse
+00070190: 6172 6368 3d6d 6f64 616c 6974 7963 6c61  arch=modalitycla
+000701a0: 7373 2b22 2a22 0a20 2020 2020 2020 2020  ss+"*".         
+000701b0: 2020 2020 2020 2070 6174 685f 7465 6d70         path_temp
+000701c0: 6c61 7465 5f6d 203d 2062 6173 655f 7061  late_m = base_pa
+000701d0: 7468 202b 2022 2f22 202b 206d 7970 726f  th + "/" + mypro
+000701e0: 6a20 2b20 2022 2f22 202b 2073 6964 202b  j +  "/" + sid +
+000701f0: 2022 2f22 202b 206d 7964 6174 6520 2b20   "/" + mydate + 
+00070200: 272f 2720 2b20 6d6f 6461 6c69 7479 636c  '/' + modalitycl
+00070210: 6173 7373 6561 7263 6820 2b20 272f 2720  asssearch + '/' 
+00070220: 2b20 6d79 6d6f 6469 6420 2b20 222f 220a  + mymodid + "/".
+00070230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00070240: 6d6f 6473 6561 7263 6820 3d20 7061 7468  modsearch = path
+00070250: 5f74 656d 706c 6174 655f 6d20 2b20 222a  _template_m + "*
+00070260: 2220 2b20 6d6f 6461 6c69 7479 636c 6173  " + modalityclas
+00070270: 7373 6561 7263 6820 2b20 222a 7769 6465  ssearch + "*wide
+00070280: 2e63 7376 220a 2020 2020 2020 2020 2020  .csv".          
+00070290: 2020 2020 2020 6966 2076 6572 626f 7365        if verbose
+000702a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000702b0: 2020 2020 2020 7072 696e 7428 206d 6f64        print( mod
+000702c0: 7365 6172 6368 2029 0a20 2020 2020 2020  search ).       
+000702d0: 2020 2020 2020 2020 2074 3177 666e 203d           t1wfn =
+000702e0: 2073 6f72 7465 6428 2067 6c6f 6228 206d   sorted( glob( m
+000702f0: 6f64 7365 6172 6368 2029 2029 0a20 2020  odsearch ) ).   
+00070300: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00070310: 6c65 6e28 2074 3177 666e 2029 203e 2031  len( t1wfn ) > 1
+00070320: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00070330: 2020 2020 2020 6e6c 6172 6765 203d 206c        nlarge = l
+00070340: 656e 2874 3177 666e 290a 2020 2020 2020  en(t1wfn).      
+00070350: 2020 2020 2020 2020 2020 2020 2020 7431                t1
+00070360: 7766 6e20 3d20 6669 6e64 5f6d 6f73 745f  wfn = find_most_
+00070370: 7265 6365 6e74 5f66 696c 6528 2074 3177  recent_file( t1w
+00070380: 666e 2029 0a20 2020 2020 2020 2020 2020  fn ).           
+00070390: 2020 2020 2020 2020 2077 6172 6e69 6e67           warning
+000703a0: 732e 7761 726e 2822 7468 6572 6520 6172  s.warn("there ar
+000703b0: 6520 2220 2b20 7374 7228 206e 6c61 7267  e " + str( nlarg
+000703c0: 6520 2920 2b20 2220 6e75 6d62 6572 206f  e ) + " number o
+000703d0: 6620 7769 6465 2066 6e73 2077 6974 6820  f wide fns with 
+000703e0: 7365 6172 6368 2070 6174 6820 2220 2b20  search path " + 
+000703f0: 6d6f 6473 6561 7263 6820 2b20 2220 7765  modsearch + " we
+00070400: 2074 616b 6520 7468 6520 6d6f 7374 2072   take the most r
+00070410: 6563 656e 7420 6f66 2074 6865 7365 2022  ecent of these "
+00070420: 202b 2074 3177 666e 5b30 5d20 290a 2320   + t1wfn[0] ).# 
+00070430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00070440: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+00070450: 726f 7228 2274 6865 7265 2061 7265 2022  ror("there are "
+00070460: 202b 2073 7472 2820 6c65 6e28 2074 3177   + str( len( t1w
+00070470: 666e 2029 2029 202b 2022 206e 756d 6265  fn ) ) + " numbe
+00070480: 7220 6f66 2077 6964 6520 666e 7320 7769  r of wide fns wi
+00070490: 7468 2073 6561 7263 6820 7061 7468 2022  th search path "
+000704a0: 202b 206d 6f64 7365 6172 6368 2029 0a20   + modsearch ). 
+000704b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000704c0: 6620 6c65 6e28 2074 3177 666e 2029 203d  f len( t1wfn ) =
+000704d0: 3d20 313a 0a20 2020 2020 2020 2020 2020  = 1:.           
+000704e0: 2020 2020 2020 2020 2069 6620 7665 7262           if verb
+000704f0: 6f73 653a 0a20 2020 2020 2020 2020 2020  ose:.           
+00070500: 2020 2020 2020 2020 2020 2020 2070 7269               pri
+00070510: 6e74 2874 3177 666e 290a 2020 2020 2020  nt(t1wfn).      
+00070520: 2020 2020 2020 2020 2020 2020 2020 7431                t1
+00070530: 6466 203d 206d 7972 6561 645f 6373 7628  df = myread_csv(
+00070540: 7431 7766 6e5b 305d 2c20 636f 7265 6e61  t1wfn[0], corena
+00070550: 6d65 7329 0a20 2020 2020 2020 2020 2020  mes).           
+00070560: 2020 2020 2020 2020 2074 3164 6620 3d20           t1df = 
+00070570: 6669 6c74 6572 5f64 6628 2074 3164 662c  filter_df( t1df,
+00070580: 206d 6f64 616c 6974 7963 6c61 7373 2b27   modalityclass+'
+00070590: 5f27 290a 2020 2020 2020 2020 2020 2020  _').            
+000705a0: 2020 2020 2020 2020 6466 6c69 7374 203d          dflist =
+000705b0: 2064 666c 6973 7420 2b20 5b74 3164 665d   dflist + [t1df]
+000705c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000705d0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000705e0: 2020 2020 2020 2020 2020 2069 6620 7665             if ve
+000705f0: 7262 6f73 653a 0a20 2020 2020 2020 2020  rbose:.         
+00070600: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00070610: 7269 6e74 2820 2220 6361 6e6e 6f74 2066  rint( " cannot f
+00070620: 696e 6420 2220 2b20 6d6f 6473 6561 7263  ind " + modsearc
+00070630: 6820 290a 2020 2020 2020 2020 2020 2020  h ).            
+00070640: 2020 2020 0a20 2020 2020 2020 2020 2020      .           
+00070650: 2068 6466 203d 2070 642e 636f 6e63 6174   hdf = pd.concat
+00070660: 2820 6466 6c69 7374 2c20 6178 6973 3d31  ( dflist, axis=1
+00070670: 2c20 6967 6e6f 7265 5f69 6e64 6578 3d46  , ignore_index=F
+00070680: 616c 7365 290a 2020 2020 2020 2020 2020  alse).          
+00070690: 2020 6966 2076 6572 626f 7365 3a0a 2020    if verbose:.  
+000706a0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+000706b0: 696e 7428 2022 636f 756e 743a 2022 202b  int( "count: " +
+000706c0: 2073 7472 2820 6d79 6374 2029 2029 0a20   str( myct ) ). 
+000706d0: 2020 2020 2020 2020 2020 2073 7562 6466             subdf
+000706e0: 203d 2064 662e 696c 6f63 5b5b 785d 5d0a   = df.iloc[[x]].
+000706f0: 2020 2020 2020 2020 2020 2020 6864 662e              hdf.
+00070700: 696e 6465 7820 3d20 7375 6264 662e 696e  index = subdf.in
+00070710: 6465 782e 636f 7079 2829 0a20 2020 2020  dex.copy().     
+00070720: 2020 2020 2020 2073 7562 6466 203d 2070         subdf = p
+00070730: 642e 636f 6e63 6174 2820 5b73 7562 6466  d.concat( [subdf
+00070740: 2c68 6466 5d2c 2061 7869 733d 312c 2069  ,hdf], axis=1, i
+00070750: 676e 6f72 655f 696e 6465 783d 4661 6c73  gnore_index=Fals
+00070760: 6529 0a20 2020 2020 2020 2020 2020 2064  e).            d
+00070770: 666f 7574 203d 2070 642e 636f 6e63 6174  fout = pd.concat
+00070780: 2820 5b64 666f 7574 2c73 7562 6466 5d2c  ( [dfout,subdf],
+00070790: 2061 7869 733d 302c 2069 676e 6f72 655f   axis=0, ignore_
+000707a0: 696e 6465 783d 4661 6c73 6520 290a 2020  index=False ).  
+000707b0: 2020 6261 646e 616d 6573 203d 2067 6574    badnames = get
+000707c0: 5f6e 616d 6573 5f66 726f 6d5f 6461 7461  _names_from_data
+000707d0: 5f66 7261 6d65 2820 5b27 556e 6e61 6d65  _frame( ['Unname
+000707e0: 6427 5d2c 2064 666f 7574 2029 0a20 2020  d'], dfout ).   
+000707f0: 2064 666f 7574 3d64 666f 7574 2e64 726f   dfout=dfout.dro
+00070800: 7028 6261 646e 616d 6573 2c20 6178 6973  p(badnames, axis
+00070810: 3d31 290a 2020 2020 7265 7475 726e 2820  =1).    return( 
+00070820: 6466 6f75 7420 290a 0a64 6566 2065 6e61  dfout )..def ena
+00070830: 6e74 696f 6d6f 7270 6869 635f 6669 6c6c  ntiomorphic_fill
+00070840: 696e 675f 7769 7468 6f75 745f 6d61 736b  ing_without_mask
+00070850: 2820 696d 6167 652c 2061 7869 733d 302c  ( image, axis=0,
+00070860: 2069 6e74 656e 7369 7479 3d27 6c6f 7727   intensity='low'
+00070870: 2029 3a0a 2020 2020 2222 220a 2020 2020   ):.    """.    
+00070880: 5065 7266 6f72 6d20 616e 2065 6e61 6e74  Perform an enant
+00070890: 696f 6d6f 7270 6869 6320 6c65 7369 6f6e  iomorphic lesion
+000708a0: 2066 696c 6c69 6e67 206f 6e20 616e 2069   filling on an i
+000708b0: 6d61 6765 2077 6974 686f 7574 2061 206c  mage without a l
+000708c0: 6573 696f 6e20 6d61 736b 2e0a 0a20 2020  esion mask...   
+000708d0: 2041 7267 733a 0a20 2020 2069 6d61 6765   Args:.    image
+000708e0: 2028 616e 7473 496d 6167 6529 3a20 5468   (antsImage): Th
+000708f0: 6520 616e 7473 2069 6d61 6765 2074 6f20  e ants image to 
+00070900: 666c 6970 2061 6e64 2066 696c 6c0a 2020  flip and fill.  
+00070910: 2020 6178 6973 2028 2069 6e74 2029 3a20    axis ( int ): 
+00070920: 7468 6520 6178 6973 2061 6c6f 6e67 2077  the axis along w
+00070930: 6869 6368 2074 6f20 7265 666c 6563 7420  hich to reflect 
+00070940: 7468 6520 696d 6167 650a 2020 2020 696e  the image.    in
+00070950: 7465 6e73 6974 7920 2820 7374 7220 2920  tensity ( str ) 
+00070960: 3a20 6c6f 7720 6f72 2068 6967 680a 0a20  : low or high.. 
+00070970: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+00070980: 616e 7473 2e41 4e54 7349 6d61 6765 3a20  ants.ANTsImage: 
+00070990: 5468 6520 696d 6167 6520 6166 7465 7220  The image after 
+000709a0: 656e 616e 7469 6f6d 6f72 7068 6963 2066  enantiomorphic f
+000709b0: 696c 6c69 6e67 2e0a 2020 2020 2222 220a  illing..    """.
+000709c0: 2020 2020 696d 6167 656e 203d 2061 6e74      imagen = ant
+000709d0: 732e 694d 6174 6828 2069 6d61 6765 2c20  s.iMath( image, 
+000709e0: 274e 6f72 6d61 6c69 7a65 2720 290a 2020  'Normalize' ).  
+000709f0: 2020 696d 6167 656e 203d 2061 6e74 732e    imagen = ants.
+00070a00: 694d 6174 6828 2069 6d61 6765 6e2c 2022  iMath( imagen, "
+00070a10: 5472 756e 6361 7465 496e 7465 6e73 6974  TruncateIntensit
+00070a20: 7922 2c20 3165 2d36 2c20 302e 3938 2029  y", 1e-6, 0.98 )
+00070a30: 0a20 2020 2069 6d61 6765 6e20 3d20 616e  .    imagen = an
+00070a40: 7473 2e69 4d61 7468 2820 696d 6167 656e  ts.iMath( imagen
+00070a50: 2c20 274e 6f72 6d61 6c69 7a65 2720 290a  , 'Normalize' ).
+00070a60: 2020 2020 2320 4372 6561 7465 2061 206d      # Create a m
+00070a70: 6972 726f 7220 696d 6167 6520 2866 6c69  irror image (fli
+00070a80: 7070 696e 6720 6c65 6674 2061 6e64 2072  pping left and r
+00070a90: 6967 6874 290a 2020 2020 6d69 7272 6f72  ight).    mirror
+00070aa0: 5f69 6d61 6765 203d 2061 6e74 732e 7265  _image = ants.re
+00070ab0: 666c 6563 745f 696d 6167 6528 696d 6167  flect_image(imag
+00070ac0: 656e 2c20 6178 6973 3d30 2c20 7478 3d27  en, axis=0, tx='
+00070ad0: 5379 4e27 2029 5b27 7761 7270 6564 6d6f  SyN' )['warpedmo
+00070ae0: 766f 7574 275d 0a0a 2020 2020 2320 4372  vout']..    # Cr
+00070af0: 6561 7465 2061 2073 796d 6d65 7472 6963  eate a symmetric
+00070b00: 2076 6572 7369 6f6e 206f 6620 7468 6520   version of the 
+00070b10: 696d 6167 6520 6279 2061 7665 7261 6769  image by averagi
+00070b20: 6e67 2074 6865 206f 7269 6769 6e61 6c20  ng the original 
+00070b30: 616e 6420 7468 6520 6d69 7272 6f72 2069  and the mirror i
+00070b40: 6d61 6765 0a20 2020 2073 796d 6d65 7472  mage.    symmetr
+00070b50: 6963 5f69 6d61 6765 203d 2069 6d61 6765  ic_image = image
+00070b60: 6e20 2a20 302e 3520 2b20 6d69 7272 6f72  n * 0.5 + mirror
+00070b70: 5f69 6d61 6765 202a 2030 2e35 0a0a 2020  _image * 0.5..  
+00070b80: 2020 2320 4964 656e 7469 6679 2070 6f74    # Identify pot
+00070b90: 656e 7469 616c 206c 6573 696f 6e20 6172  ential lesion ar
+00070ba0: 6561 7320 6279 2066 696e 6469 6e67 2064  eas by finding d
+00070bb0: 6966 6665 7265 6e63 6573 2062 6574 7765  ifferences betwe
+00070bc0: 656e 2074 6865 206f 7269 6769 6e61 6c20  en the original 
+00070bd0: 616e 6420 7379 6d6d 6574 7269 6320 696d  and symmetric im
+00070be0: 6167 650a 2020 2020 6469 6666 6572 656e  age.    differen
+00070bf0: 6365 5f69 6d61 6765 203d 2069 6d61 6765  ce_image = image
+00070c00: 202d 2073 796d 6d65 7472 6963 5f69 6d61   - symmetric_ima
+00070c10: 6765 0a20 2020 2064 6966 6673 6567 203d  ge.    diffseg =
+00070c20: 2061 6e74 732e 7468 7265 7368 6f6c 645f   ants.threshold_
+00070c30: 696d 6167 6528 6469 6666 6572 656e 6365  image(difference
+00070c40: 5f69 6d61 6765 2c20 224f 7473 7522 2c20  _image, "Otsu", 
+00070c50: 3320 290a 2020 2020 6966 2069 6e74 656e  3 ).    if inten
+00070c60: 7369 7479 203d 3d20 276c 6f77 273a 0a20  sity == 'low':. 
+00070c70: 2020 2020 2020 206c 696b 656c 795f 6c65         likely_le
+00070c80: 7369 6f6e 203d 2061 6e74 732e 7468 7265  sion = ants.thre
+00070c90: 7368 6f6c 645f 696d 6167 6528 2064 6966  shold_image( dif
+00070ca0: 6673 6567 2c20 312c 2020 3129 0a20 2020  fseg, 1,  1).   
+00070cb0: 2065 6c73 653a 0a20 2020 2020 2020 206c   else:.        l
+00070cc0: 696b 656c 795f 6c65 7369 6f6e 203d 2061  ikely_lesion = a
+00070cd0: 6e74 732e 7468 7265 7368 6f6c 645f 696d  nts.threshold_im
+00070ce0: 6167 6528 2064 6966 6673 6567 2c20 332c  age( diffseg, 3,
+00070cf0: 2020 3329 0a20 2020 206c 696b 656c 795f    3).    likely_
+00070d00: 6c65 7369 6f6e 203d 2061 6e74 732e 736d  lesion = ants.sm
+00070d10: 6f6f 7468 5f69 6d61 6765 2820 6c69 6b65  ooth_image( like
+00070d20: 6c79 5f6c 6573 696f 6e2c 2033 2e30 2029  ly_lesion, 3.0 )
+00070d30: 2e69 4d61 7468 2822 4e6f 726d 616c 697a  .iMath("Normaliz
+00070d40: 6522 290a 2020 2020 6c65 7369 6f6e 6e65  e").    lesionne
+00070d50: 6720 3d20 2820 696d 6167 656e 2a30 2b31  g = ( imagen*0+1
+00070d60: 2e30 2029 202d 206c 696b 656c 795f 6c65  .0 ) - likely_le
+00070d70: 7369 6f6e 0a20 2020 2066 696c 6c65 645f  sion.    filled_
+00070d80: 696d 6167 6520 3d20 616e 7473 2e69 6d61  image = ants.ima
+00070d90: 6765 5f63 6c6f 6e65 2869 6d61 6765 6e29  ge_clone(imagen)
+00070da0: 2020 2020 0a20 2020 2066 696c 6c65 645f      .    filled_
+00070db0: 696d 6167 6520 3d20 696d 6167 656e 202a  image = imagen *
+00070dc0: 206c 6573 696f 6e6e 6567 202b 206d 6972   lesionneg + mir
+00070dd0: 726f 725f 696d 6167 6520 2a20 6c69 6b65  ror_image * like
+00070de0: 6c79 5f6c 6573 696f 6e0a 0a20 2020 2072  ly_lesion..    r
+00070df0: 6574 7572 6e20 6669 6c6c 6564 5f69 6d61  eturn filled_ima
+00070e00: 6765 2c20 6469 6666 7365 670a 0a0a 0a64  ge, diffseg....d
+00070e10: 6566 2066 696c 7465 725f 696d 6167 655f  ef filter_image_
+00070e20: 6669 6c65 7328 696d 6167 655f 7061 7468  files(image_path
+00070e30: 732c 2063 7269 7465 7269 613d 276c 6172  s, criteria='lar
+00070e40: 6765 7374 2729 3a0a 2020 2020 2222 220a  gest'):.    """.
+00070e50: 2020 2020 4669 6c74 6572 7320 6120 6c69      Filters a li
+00070e60: 7374 206f 6620 696d 6167 6520 6669 6c65  st of image file
+00070e70: 2070 6174 6873 2062 6173 6564 206f 6e20   paths based on 
+00070e80: 7370 6563 6966 6965 6420 6372 6974 6572  specified criter
+00070e90: 6961 2061 6e64 2072 6574 7572 6e73 200a  ia and returns .
+00070ea0: 2020 2020 7468 6520 7061 7468 206f 6620      the path of 
+00070eb0: 7468 6520 696d 6167 6520 7468 6174 2062  the image that b
+00070ec0: 6573 7420 6d61 7463 6865 7320 7468 6174  est matches that
+00070ed0: 2063 7269 7465 7269 6120 2873 6d61 6c6c   criteria (small
+00070ee0: 6573 742c 206c 6172 6765 7374 2c20 6f72  est, largest, or
+00070ef0: 2062 7269 6768 7465 7374 292e 0a0a 2020   brightest)...  
+00070f00: 2020 4172 6773 3a0a 2020 2020 696d 6167    Args:.    imag
+00070f10: 655f 7061 7468 7320 286c 6973 7429 3a20  e_paths (list): 
+00070f20: 4120 6c69 7374 206f 6620 6669 6c65 2070  A list of file p
+00070f30: 6174 6873 2074 6f20 7468 6520 696d 6167  aths to the imag
+00070f40: 6573 2e0a 2020 2020 6372 6974 6572 6961  es..    criteria
+00070f50: 2028 7374 7229 3a20 4372 6974 6572 6961   (str): Criteria
+00070f60: 2066 6f72 2073 656c 6563 7469 6e67 2074   for selecting t
+00070f70: 6865 2069 6d61 6765 2028 2773 6d61 6c6c  he image ('small
+00070f80: 6573 7427 2c20 276c 6172 6765 7374 272c  est', 'largest',
+00070f90: 2027 6272 6967 6874 6573 7427 292e 0a0a   'brightest')...
+00070fa0: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+00070fb0: 2073 7472 3a20 5468 6520 6669 6c65 2070   str: The file p
+00070fc0: 6174 6820 6f66 2074 6865 2073 656c 6563  ath of the selec
+00070fd0: 7465 6420 696d 6167 652c 206f 7220 4e6f  ted image, or No
+00070fe0: 6e65 2069 6620 6e6f 2076 616c 6964 2069  ne if no valid i
+00070ff0: 6d61 6765 7320 6172 6520 666f 756e 642e  mages are found.
+00071000: 0a20 2020 2022 2222 0a20 2020 2069 6d70  .    """.    imp
+00071010: 6f72 7420 6e75 6d70 7920 6173 206e 700a  ort numpy as np.
+00071020: 2020 2020 6966 206e 6f74 2069 6d61 6765      if not image
+00071030: 5f70 6174 6873 3a0a 2020 2020 2020 2020  _paths:.        
+00071040: 7265 7475 726e 204e 6f6e 650a 0a20 2020  return None..   
+00071050: 2073 656c 6563 7465 645f 696d 6167 655f   selected_image_
+00071060: 7061 7468 203d 204e 6f6e 650a 2020 2020  path = None.    
+00071070: 6966 2063 7269 7465 7269 6120 3d3d 2027  if criteria == '
+00071080: 736d 616c 6c65 7374 2720 6f72 2063 7269  smallest' or cri
+00071090: 7465 7269 6120 3d3d 2027 6c61 7267 6573  teria == 'larges
+000710a0: 7427 3a0a 2020 2020 2020 2020 6578 7472  t':.        extr
+000710b0: 656d 655f 766f 6c75 6d65 203d 204e 6f6e  eme_volume = Non
+000710c0: 650a 0a20 2020 2020 2020 2066 6f72 2070  e..        for p
+000710d0: 6174 6820 696e 2069 6d61 6765 5f70 6174  ath in image_pat
+000710e0: 6873 3a0a 2020 2020 2020 2020 2020 2020  hs:.            
+000710f0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+00071100: 2020 2020 2069 6d61 6765 203d 2061 6e74       image = ant
+00071110: 732e 696d 6167 655f 7265 6164 2870 6174  s.image_read(pat
+00071120: 6829 0a20 2020 2020 2020 2020 2020 2020  h).             
+00071130: 2020 2076 6f6c 756d 6520 3d20 6e70 2e70     volume = np.p
+00071140: 726f 6428 696d 6167 652e 7368 6170 6529  rod(image.shape)
+00071150: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00071160: 2020 6966 2063 7269 7465 7269 6120 3d3d    if criteria ==
+00071170: 2027 6c61 7267 6573 7427 3a0a 2020 2020   'largest':.    
+00071180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00071190: 6966 2065 7874 7265 6d65 5f76 6f6c 756d  if extreme_volum
+000711a0: 6520 6973 204e 6f6e 6520 6f72 2076 6f6c  e is None or vol
+000711b0: 756d 6520 3e20 6578 7472 656d 655f 766f  ume > extreme_vo
+000711c0: 6c75 6d65 3a0a 2020 2020 2020 2020 2020  lume:.          
+000711d0: 2020 2020 2020 2020 2020 2020 2020 6578                ex
+000711e0: 7472 656d 655f 766f 6c75 6d65 203d 2076  treme_volume = v
+000711f0: 6f6c 756d 650a 2020 2020 2020 2020 2020  olume.          
+00071200: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00071210: 6c65 6374 6564 5f69 6d61 6765 5f70 6174  lected_image_pat
+00071220: 6820 3d20 7061 7468 0a20 2020 2020 2020  h = path.       
+00071230: 2020 2020 2020 2020 2065 6c69 6620 6372           elif cr
+00071240: 6974 6572 6961 203d 3d20 2773 6d61 6c6c  iteria == 'small
+00071250: 6573 7427 3a0a 2020 2020 2020 2020 2020  est':.          
+00071260: 2020 2020 2020 2020 2020 6966 2065 7874            if ext
+00071270: 7265 6d65 5f76 6f6c 756d 6520 6973 204e  reme_volume is N
+00071280: 6f6e 6520 6f72 2076 6f6c 756d 6520 3c20  one or volume < 
+00071290: 6578 7472 656d 655f 766f 6c75 6d65 3a0a  extreme_volume:.
+000712a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000712b0: 2020 2020 2020 2020 6578 7472 656d 655f          extreme_
+000712c0: 766f 6c75 6d65 203d 2076 6f6c 756d 650a  volume = volume.
+000712d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000712e0: 2020 2020 2020 2020 7365 6c65 6374 6564          selected
+000712f0: 5f69 6d61 6765 5f70 6174 6820 3d20 7061  _image_path = pa
+00071300: 7468 0a0a 2020 2020 2020 2020 2020 2020  th..            
+00071310: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
+00071320: 2061 7320 653a 0a20 2020 2020 2020 2020   as e:.         
+00071330: 2020 2020 2020 2070 7269 6e74 2866 2245         print(f"E
+00071340: 7272 6f72 2070 726f 6365 7373 696e 6720  rror processing 
+00071350: 696d 6167 6520 7b70 6174 687d 3a20 7b65  image {path}: {e
+00071360: 7d22 290a 0a20 2020 2065 6c69 6620 6372  }")..    elif cr
+00071370: 6974 6572 6961 203d 3d20 2762 7269 6768  iteria == 'brigh
+00071380: 7465 7374 273a 0a20 2020 2020 2020 206d  test':.        m
+00071390: 6178 5f62 7269 6768 746e 6573 7320 3d20  ax_brightness = 
+000713a0: 4e6f 6e65 0a0a 2020 2020 2020 2020 666f  None..        fo
+000713b0: 7220 7061 7468 2069 6e20 696d 6167 655f  r path in image_
+000713c0: 7061 7468 733a 0a20 2020 2020 2020 2020  paths:.         
+000713d0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+000713e0: 2020 2020 2020 2020 696d 6167 6520 3d20          image = 
+000713f0: 616e 7473 2e69 6d61 6765 5f72 6561 6428  ants.image_read(
+00071400: 7061 7468 290a 2020 2020 2020 2020 2020  path).          
+00071410: 2020 2020 2020 6272 6967 6874 6e65 7373        brightness
+00071420: 203d 206e 702e 6d65 616e 2869 6d61 6765   = np.mean(image
+00071430: 2e6e 756d 7079 2829 290a 0a20 2020 2020  .numpy())..     
+00071440: 2020 2020 2020 2020 2020 2069 6620 6d61             if ma
+00071450: 785f 6272 6967 6874 6e65 7373 2069 7320  x_brightness is 
+00071460: 4e6f 6e65 206f 7220 6272 6967 6874 6e65  None or brightne
+00071470: 7373 203e 206d 6178 5f62 7269 6768 746e  ss > max_brightn
+00071480: 6573 733a 0a20 2020 2020 2020 2020 2020  ess:.           
+00071490: 2020 2020 2020 2020 206d 6178 5f62 7269           max_bri
+000714a0: 6768 746e 6573 7320 3d20 6272 6967 6874  ghtness = bright
+000714b0: 6e65 7373 0a20 2020 2020 2020 2020 2020  ness.           
+000714c0: 2020 2020 2020 2020 2073 656c 6563 7465           selecte
+000714d0: 645f 696d 6167 655f 7061 7468 203d 2070  d_image_path = p
+000714e0: 6174 680a 0a20 2020 2020 2020 2020 2020  ath..           
+000714f0: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+00071500: 6e20 6173 2065 3a0a 2020 2020 2020 2020  n as e:.        
+00071510: 2020 2020 2020 2020 7072 696e 7428 6622          print(f"
+00071520: 4572 726f 7220 7072 6f63 6573 7369 6e67  Error processing
+00071530: 2069 6d61 6765 207b 7061 7468 7d3a 207b   image {path}: {
+00071540: 657d 2229 0a0a 2020 2020 656c 7365 3a0a  e}")..    else:.
+00071550: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+00071560: 6c75 6545 7272 6f72 2822 4372 6974 6572  lueError("Criter
+00071570: 6961 206d 7573 7420 6265 2027 736d 616c  ia must be 'smal
+00071580: 6c65 7374 272c 2027 6c61 7267 6573 7427  lest', 'largest'
+00071590: 2c20 6f72 2027 6272 6967 6874 6573 7427  , or 'brightest'
+000715a0: 2e22 290a 0a20 2020 2072 6574 7572 6e20  .")..    return 
+000715b0: 7365 6c65 6374 6564 5f69 6d61 6765 5f70  selected_image_p
+000715c0: 6174 680a 0a0a 0a64 6566 206d 6d5f 6d61  ath....def mm_ma
+000715d0: 7463 685f 6279 5f71 635f 7363 6f72 696e  tch_by_qc_scorin
+000715e0: 6728 6466 5f61 2c20 6466 5f62 2c20 6d61  g(df_a, df_b, ma
+000715f0: 7463 685f 636f 6c75 6d6e 2c20 6372 6974  tch_column, crit
+00071600: 6572 6961 2c20 7072 6566 6978 3d27 6d61  eria, prefix='ma
+00071610: 7463 6865 645f 272c 2065 7863 6c75 6465  tched_', exclude
+00071620: 5f63 6f6c 756d 6e73 3d4e 6f6e 6529 3a0a  _columns=None):.
+00071630: 2020 2020 2222 220a 2020 2020 4d61 7463      """.    Matc
+00071640: 6820 6561 6368 2072 6f77 2069 6e20 6466  h each row in df
+00071650: 5f61 2074 6f20 6120 726f 7720 696e 2064  _a to a row in d
+00071660: 665f 6220 6261 7365 6420 6f6e 2061 206d  f_b based on a m
+00071670: 6174 6368 696e 6720 636f 6c75 6d6e 2061  atching column a
+00071680: 6e64 2063 7269 7465 7269 6120 666f 7220  nd criteria for 
+00071690: 7365 6c65 6374 696e 6720 7468 6520 6265  selecting the be
+000716a0: 7374 206d 6174 6368 2c0a 2020 2020 7769  st match,.    wi
+000716b0: 7468 206f 7074 696f 6e73 2074 6f20 7072  th options to pr
+000716c0: 6566 6978 2063 6f6c 756d 6e20 6e61 6d65  efix column name
+000716d0: 7320 6672 6f6d 2064 665f 6220 616e 6420  s from df_b and 
+000716e0: 6578 636c 7564 6520 6365 7274 6169 6e20  exclude certain 
+000716f0: 636f 6c75 6d6e 7320 6672 6f6d 2074 6865  columns from the
+00071700: 2066 696e 616c 206f 7574 7075 742e 2041   final output. A
+00071710: 6464 6974 696f 6e61 6c6c 792c 0a20 2020  dditionally,.   
+00071720: 2072 6574 7572 6e73 2061 2044 6174 6146   returns a DataF
+00071730: 7261 6d65 2063 6f6e 7461 696e 696e 6720  rame containing 
+00071740: 726f 7773 2066 726f 6d20 6466 5f62 2074  rows from df_b t
+00071750: 6861 7420 7765 7265 206e 6f74 206d 6174  hat were not mat
+00071760: 6368 6564 2074 6f20 616e 7920 726f 7720  ched to any row 
+00071770: 696e 2064 665f 612e 0a0a 2020 2020 5061  in df_a...    Pa
+00071780: 7261 6d65 7465 7273 3a0a 2020 2020 2d20  rameters:.    - 
+00071790: 6466 5f61 3a20 4461 7461 4672 616d 6520  df_a: DataFrame 
+000717a0: 412e 0a20 2020 202d 2064 665f 623a 2044  A..    - df_b: D
+000717b0: 6174 6146 7261 6d65 2042 2e0a 2020 2020  ataFrame B..    
+000717c0: 2d20 6d61 7463 685f 636f 6c75 6d6e 3a20  - match_column: 
+000717d0: 5468 6520 636f 6c75 6d6e 206e 616d 6520  The column name 
+000717e0: 6f6e 2077 6869 6368 2072 6f77 7320 7368  on which rows sh
+000717f0: 6f75 6c64 206d 6174 6368 2062 6574 7765  ould match betwe
+00071800: 656e 2044 6174 6146 7261 6d65 2041 2061  en DataFrame A a
+00071810: 6e64 2042 2e0a 2020 2020 2d20 6372 6974  nd B..    - crit
+00071820: 6572 6961 3a20 4120 6469 6374 696f 6e61  eria: A dictiona
+00071830: 7279 2077 6865 7265 206b 6579 7320 6172  ry where keys ar
+00071840: 6520 636f 6c75 6d6e 206e 616d 6573 2061  e column names a
+00071850: 6e64 2076 616c 7565 7320 6172 6520 276d  nd values are 'm
+00071860: 696e 2720 6f72 2027 6d61 7827 2c20 696e  in' or 'max', in
+00071870: 6469 6361 7469 6e67 2077 6865 7468 6572  dicating whether
+00071880: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00071890: 2074 6865 2063 6f6c 756d 6e20 7368 6f75   the column shou
+000718a0: 6c64 2062 6520 6d69 6e69 6d69 7a65 6420  ld be minimized 
+000718b0: 6f72 206d 6178 696d 697a 6564 2066 6f72  or maximized for
+000718c0: 2074 6865 2062 6573 7420 6d61 7463 682e   the best match.
+000718d0: 0a20 2020 202d 2070 7265 6669 783a 2041  .    - prefix: A
+000718e0: 2073 7472 696e 6720 7072 6566 6978 2074   string prefix t
+000718f0: 6f20 6164 6420 746f 2063 6f6c 756d 6e20  o add to column 
+00071900: 6e61 6d65 7320 6672 6f6d 2064 665f 6220  names from df_b 
+00071910: 696e 2074 6865 2066 696e 616c 206f 7574  in the final out
+00071920: 7075 7420 746f 2061 766f 6964 2064 7570  put to avoid dup
+00071930: 6c69 6361 7469 6f6e 2e0a 2020 2020 2d20  lication..    - 
+00071940: 6578 636c 7564 655f 636f 6c75 6d6e 733a  exclude_columns:
+00071950: 2041 206c 6973 7420 6f66 2063 6f6c 756d   A list of colum
+00071960: 6e20 6e61 6d65 7320 6672 6f6d 2064 665f  n names from df_
+00071970: 6220 746f 2065 7863 6c75 6465 2066 726f  b to exclude fro
+00071980: 6d20 7468 6520 6669 6e61 6c20 6f75 7470  m the final outp
+00071990: 7574 2e0a 2020 2020 0a20 2020 2052 6574  ut..    .    Ret
+000719a0: 7572 6e73 3a0a 2020 2020 2d20 4120 7475  urns:.    - A tu
+000719b0: 706c 6520 6f66 2074 776f 2044 6174 6146  ple of two DataF
+000719c0: 7261 6d65 733a 200a 2020 2020 2020 2020  rames: .        
+000719d0: 312e 2041 206e 6577 2044 6174 6146 7261  1. A new DataFra
+000719e0: 6d65 2063 6f6d 6269 6e69 6e67 2064 665f  me combining df_
+000719f0: 6120 7769 7468 206d 6174 6368 6564 2072  a with matched r
+00071a00: 6f77 7320 6672 6f6d 2064 665f 622e 0a20  ows from df_b.. 
+00071a10: 2020 2020 2020 2032 2e20 4120 4461 7461         2. A Data
+00071a20: 4672 616d 6520 636f 6e74 6169 6e69 6e67  Frame containing
+00071a30: 2072 6f77 7320 6672 6f6d 2064 665f 6220   rows from df_b 
+00071a40: 7468 6174 2077 6572 6520 6e6f 7420 6d61  that were not ma
+00071a50: 7463 6865 6420 746f 2064 665f 612e 0a20  tched to df_a.. 
+00071a60: 2020 2022 2222 0a20 2020 2066 726f 6d20     """.    from 
+00071a70: 7363 6970 792e 7374 6174 7320 696d 706f  scipy.stats impo
+00071a80: 7274 207a 7363 6f72 650a 2020 2020 6466  rt zscore.    df
+00071a90: 5f61 203d 2064 665f 612e 6c6f 635b 3a2c  _a = df_a.loc[:,
+00071aa0: 207e 6466 5f61 2e63 6f6c 756d 6e73 2e73   ~df_a.columns.s
+00071ab0: 7472 2e73 7461 7274 7377 6974 6828 2755  tr.startswith('U
+00071ac0: 6e6e 616d 6564 3a27 295d 0a20 2020 2064  nnamed:')].    d
+00071ad0: 665f 6220 3d20 6466 5f62 2e6c 6f63 5b3a  f_b = df_b.loc[:
+00071ae0: 2c20 7e64 665f 622e 636f 6c75 6d6e 732e  , ~df_b.columns.
+00071af0: 7374 722e 7374 6172 7473 7769 7468 2827  str.startswith('
+00071b00: 556e 6e61 6d65 643a 2729 5d2e 636f 7079  Unnamed:')].copy
+00071b10: 2829 0a20 2020 200a 2020 2020 2320 4e6f  ().    .    # No
+00071b20: 726d 616c 697a 6520 6466 5f62 2062 6173  rmalize df_b bas
+00071b30: 6564 206f 6e20 6372 6974 6572 6961 0a20  ed on criteria. 
+00071b40: 2020 2066 6f72 2063 6f6c 2c20 6372 6974     for col, crit
+00071b50: 2069 6e20 6372 6974 6572 6961 2e69 7465   in criteria.ite
+00071b60: 6d73 2829 3a0a 2020 2020 2020 2020 6966  ms():.        if
+00071b70: 2063 7269 7420 3d3d 2027 6d61 7827 3a0a   crit == 'max':.
+00071b80: 2020 2020 2020 2020 2020 2020 6466 5f62              df_b
+00071b90: 2e6c 6f63 5b64 665f 622e 696e 6465 782c  .loc[df_b.index,
+00071ba0: 2066 2773 636f 7265 5f7b 636f 6c7d 275d   f'score_{col}']
+00071bb0: 203d 207a 7363 6f72 6528 2d64 665f 625b   = zscore(-df_b[
+00071bc0: 636f 6c5d 290a 2020 2020 2020 2020 656c  col]).        el
+00071bd0: 6966 2063 7269 7420 3d3d 2027 6d69 6e27  if crit == 'min'
+00071be0: 3a0a 2020 2020 2020 2020 2020 2020 6466  :.            df
+00071bf0: 5f62 2e6c 6f63 5b64 665f 622e 696e 6465  _b.loc[df_b.inde
+00071c00: 782c 2066 2773 636f 7265 5f7b 636f 6c7d  x, f'score_{col}
+00071c10: 275d 203d 207a 7363 6f72 6528 6466 5f62  '] = zscore(df_b
+00071c20: 5b63 6f6c 5d29 0a0a 2020 2020 2320 4361  [col])..    # Ca
+00071c30: 6c63 756c 6174 6520 2762 6573 745f 7363  lculate 'best_sc
+00071c40: 6f72 6527 2062 7920 7375 6d6d 696e 6720  ore' by summing 
+00071c50: 616c 6c20 7363 6f72 6520 636f 6c75 6d6e  all score column
+00071c60: 730a 2020 2020 7363 6f72 655f 636f 6c75  s.    score_colu
+00071c70: 6d6e 7320 3d20 5b66 2773 636f 7265 5f7b  mns = [f'score_{
+00071c80: 636f 6c7d 2720 666f 7220 636f 6c20 696e  col}' for col in
+00071c90: 2063 7269 7465 7269 612e 6b65 7973 2829   criteria.keys()
+00071ca0: 5d0a 2020 2020 6466 5f62 5b27 6265 7374  ].    df_b['best
+00071cb0: 5f73 636f 7265 275d 203d 2064 665f 625b  _score'] = df_b[
+00071cc0: 7363 6f72 655f 636f 6c75 6d6e 735d 2e73  score_columns].s
+00071cd0: 756d 2861 7869 733d 3129 0a0a 2020 2020  um(axis=1)..    
+00071ce0: 6d61 7463 6865 645f 696e 6469 6365 7320  matched_indices 
+00071cf0: 3d20 5b5d 2020 2320 5472 6163 6b20 696e  = []  # Track in
+00071d00: 6469 6365 7320 6f66 206d 6174 6368 6564  dices of matched
+00071d10: 2072 6f77 7320 696e 2064 665f 620a 0a20   rows in df_b.. 
+00071d20: 2020 2023 204d 6174 6368 2072 6f77 730a     # Match rows.
+00071d30: 2020 2020 6d61 7463 6865 645f 726f 7773      matched_rows
+00071d40: 203d 205b 5d0a 2020 2020 666f 7220 5f2c   = [].    for _,
+00071d50: 2072 6f77 5f61 2069 6e20 6466 5f61 2e69   row_a in df_a.i
+00071d60: 7465 7272 6f77 7328 293a 0a20 2020 2020  terrows():.     
+00071d70: 2020 206d 6174 6368 6573 203d 2064 665f     matches = df_
+00071d80: 625b 6466 5f62 5b6d 6174 6368 5f63 6f6c  b[df_b[match_col
+00071d90: 756d 6e5d 203d 3d20 726f 775f 615b 6d61  umn] == row_a[ma
+00071da0: 7463 685f 636f 6c75 6d6e 5d5d 0a20 2020  tch_column]].   
+00071db0: 2020 2020 2069 6620 6e6f 7420 6d61 7463       if not matc
+00071dc0: 6865 732e 656d 7074 793a 0a20 2020 2020  hes.empty:.     
+00071dd0: 2020 2020 2020 2062 6573 745f 6964 7820         best_idx 
+00071de0: 3d20 6d61 7463 6865 735b 2762 6573 745f  = matches['best_
+00071df0: 7363 6f72 6527 5d2e 6964 786d 696e 2829  score'].idxmin()
+00071e00: 0a20 2020 2020 2020 2020 2020 2062 6573  .            bes
+00071e10: 745f 6d61 7463 6820 3d20 6d61 7463 6865  t_match = matche
+00071e20: 732e 6c6f 635b 6265 7374 5f69 6478 5d0a  s.loc[best_idx].
+00071e30: 2020 2020 2020 2020 2020 2020 6d61 7463              matc
+00071e40: 6865 645f 696e 6469 6365 732e 6170 7065  hed_indices.appe
+00071e50: 6e64 2862 6573 745f 6964 7829 2020 2320  nd(best_idx)  # 
+00071e60: 5472 6163 6b20 7468 6973 2069 6e64 6578  Track this index
+00071e70: 2061 7320 6d61 7463 6865 640a 2020 2020   as matched.    
+00071e80: 2020 2020 2020 2020 6d61 7463 6865 645f          matched_
+00071e90: 726f 7773 2e61 7070 656e 6428 6265 7374  rows.append(best
+00071ea0: 5f6d 6174 6368 290a 2020 2020 2020 2020  _match).        
+00071eb0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00071ec0: 2020 6d61 7463 6865 645f 726f 7773 2e61    matched_rows.a
+00071ed0: 7070 656e 6428 7064 2e53 6572 6965 7328  ppend(pd.Series(
+00071ee0: 6474 7970 653d 2766 6c6f 6174 3634 2729  dtype='float64')
+00071ef0: 290a 0a20 2020 2023 2043 7265 6174 6520  )..    # Create 
+00071f00: 6120 4461 7461 4672 616d 6520 6672 6f6d  a DataFrame from
+00071f10: 206d 6174 6368 6564 2072 6f77 730a 2020   matched rows.  
+00071f20: 2020 6466 5f6d 6174 6368 6564 203d 2070    df_matched = p
+00071f30: 642e 4461 7461 4672 616d 6528 6d61 7463  d.DataFrame(matc
+00071f40: 6865 645f 726f 7773 292e 7265 7365 745f  hed_rows).reset_
+00071f50: 696e 6465 7828 6472 6f70 3d54 7275 6529  index(drop=True)
+00071f60: 0a20 2020 200a 2020 2020 2320 4578 636c  .    .    # Excl
+00071f70: 7564 6520 7370 6563 6966 6965 6420 636f  ude specified co
+00071f80: 6c75 6d6e 7320 616e 6420 6164 6420 7072  lumns and add pr
+00071f90: 6566 6978 0a20 2020 2069 6620 6578 636c  efix.    if excl
+00071fa0: 7564 655f 636f 6c75 6d6e 7320 6973 206e  ude_columns is n
+00071fb0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00071fc0: 2064 665f 6d61 7463 6865 6420 3d20 6466   df_matched = df
+00071fd0: 5f6d 6174 6368 6564 2e64 726f 7028 636f  _matched.drop(co
+00071fe0: 6c75 6d6e 733d 6578 636c 7564 655f 636f  lumns=exclude_co
+00071ff0: 6c75 6d6e 732c 2065 7272 6f72 733d 2769  lumns, errors='i
+00072000: 676e 6f72 6527 290a 2020 2020 6466 5f6d  gnore').    df_m
+00072010: 6174 6368 6564 203d 2064 665f 6d61 7463  atched = df_matc
+00072020: 6865 642e 7265 6e61 6d65 2863 6f6c 756d  hed.rename(colum
+00072030: 6e73 3d6c 616d 6264 6120 783a 2066 227b  ns=lambda x: f"{
+00072040: 7072 6566 6978 7d7b 787d 2220 6966 2078  prefix}{x}" if x
+00072050: 2021 3d20 6d61 7463 685f 636f 6c75 6d6e   != match_column
+00072060: 2061 6e64 2078 2069 6e20 6466 5f6d 6174   and x in df_mat
+00072070: 6368 6564 2e63 6f6c 756d 6e73 2065 6c73  ched.columns els
+00072080: 6520 7829 0a0a 2020 2020 2320 436f 6d62  e x)..    # Comb
+00072090: 696e 6520 6466 5f61 2077 6974 6820 6d61  ine df_a with ma
+000720a0: 7463 6865 6420 726f 7773 2066 726f 6d20  tched rows from 
+000720b0: 6466 5f62 0a20 2020 2072 6573 756c 745f  df_b.    result_
+000720c0: 6466 203d 2070 642e 636f 6e63 6174 285b  df = pd.concat([
+000720d0: 6466 5f61 2e72 6573 6574 5f69 6e64 6578  df_a.reset_index
+000720e0: 2864 726f 703d 5472 7565 292c 2064 665f  (drop=True), df_
+000720f0: 6d61 7463 6865 645d 2c20 6178 6973 3d31  matched], axis=1
+00072100: 290a 2020 2020 0a20 2020 2023 2045 7874  ).    .    # Ext
+00072110: 7261 6374 2075 6e6d 6174 6368 6564 2072  ract unmatched r
+00072120: 6f77 7320 6672 6f6d 2064 665f 620a 2020  ows from df_b.  
+00072130: 2020 756e 6d61 7463 6865 645f 6466 5f62    unmatched_df_b
+00072140: 203d 2064 665f 622e 6472 6f70 2869 6e64   = df_b.drop(ind
+00072150: 6578 3d6d 6174 6368 6564 5f69 6e64 6963  ex=matched_indic
+00072160: 6573 292e 7265 7365 745f 696e 6465 7828  es).reset_index(
+00072170: 6472 6f70 3d54 7275 6529 0a0a 2020 2020  drop=True)..    
+00072180: 7265 7475 726e 2072 6573 756c 745f 6466  return result_df
+00072190: 2c20 756e 6d61 7463 6865 645f 6466 5f62  , unmatched_df_b
+000721a0: 0a0a 0a64 6566 2066 6978 5f4c 525f 524c  ...def fix_LR_RL
+000721b0: 5f73 7475 6666 2864 662c 2063 6f6c 312c  _stuff(df, col1,
+000721c0: 2063 6f6c 322c 2073 697a 655f 636f 6c31   col2, size_col1
+000721d0: 2c20 7369 7a65 5f63 6f6c 322c 2069 6431  , size_col2, id1
+000721e0: 2c20 6964 3220 293a 0a20 2020 2064 665f  , id2 ):.    df_
+000721f0: 636f 7079 203d 2064 662e 636f 7079 2829  copy = df.copy()
+00072200: 0a20 2020 2023 2045 6e73 7572 6520 636f  .    # Ensure co
+00072210: 6c75 6d6e 7320 636f 6e74 6169 6e20 7374  lumns contain st
+00072220: 7269 6e67 7320 666f 7220 7375 6273 7472  rings for substr
+00072230: 696e 6720 6368 6563 6b73 0a20 2020 2064  ing checks.    d
+00072240: 665f 636f 7079 5b63 6f6c 315d 203d 2064  f_copy[col1] = d
+00072250: 665f 636f 7079 5b63 6f6c 315d 2e61 7374  f_copy[col1].ast
+00072260: 7970 6528 7374 7229 0a20 2020 2064 665f  ype(str).    df_
+00072270: 636f 7079 5b63 6f6c 325d 203d 2064 665f  copy[col2] = df_
+00072280: 636f 7079 5b63 6f6c 325d 2e61 7374 7970  copy[col2].astyp
+00072290: 6528 7374 7229 0a20 2020 2064 665f 636f  e(str).    df_co
+000722a0: 7079 5b69 6431 5d20 3d20 6466 5f63 6f70  py[id1] = df_cop
+000722b0: 795b 6964 315d 2e61 7374 7970 6528 7374  y[id1].astype(st
+000722c0: 7229 0a20 2020 2064 665f 636f 7079 5b69  r).    df_copy[i
+000722d0: 6432 5d20 3d20 6466 5f63 6f70 795b 6964  d2] = df_copy[id
+000722e0: 325d 2e61 7374 7970 6528 7374 7229 0a20  2].astype(str). 
+000722f0: 2020 200a 2020 2020 666f 7220 696e 6465     .    for inde
+00072300: 782c 2072 6f77 2069 6e20 6466 5f63 6f70  x, row in df_cop
+00072310: 792e 6974 6572 726f 7773 2829 3a0a 2020  y.iterrows():.  
+00072320: 2020 2020 2020 636f 6c31 5f76 616c 203d        col1_val =
+00072330: 2072 6f77 5b63 6f6c 315d 0a20 2020 2020   row[col1].     
+00072340: 2020 2063 6f6c 325f 7661 6c20 3d20 726f     col2_val = ro
+00072350: 775b 636f 6c32 5d0a 2020 2020 2020 2020  w[col2].        
+00072360: 7369 7a65 3120 3d20 726f 775b 7369 7a65  size1 = row[size
+00072370: 5f63 6f6c 315d 0a20 2020 2020 2020 2073  _col1].        s
+00072380: 697a 6532 203d 2072 6f77 5b73 697a 655f  ize2 = row[size_
+00072390: 636f 6c32 5d0a 2020 2020 2020 2020 0a20  col2].        . 
+000723a0: 2020 2020 2020 2023 2043 6865 636b 2066         # Check f
+000723b0: 6f72 2027 524c 2720 6f72 2027 4c52 2720  or 'RL' or 'LR' 
+000723c0: 696e 2065 6163 6820 636f 6c75 6d6e 2061  in each column a
+000723d0: 6e64 2063 6f6d 7061 7265 2073 697a 6573  nd compare sizes
+000723e0: 0a20 2020 2020 2020 2069 6620 2827 524c  .        if ('RL
+000723f0: 2720 696e 2063 6f6c 315f 7661 6c20 6f72  ' in col1_val or
+00072400: 2027 4c52 2720 696e 2063 6f6c 315f 7661   'LR' in col1_va
+00072410: 6c29 2061 6e64 2028 2752 4c27 2069 6e20  l) and ('RL' in 
+00072420: 636f 6c32 5f76 616c 206f 7220 274c 5227  col2_val or 'LR'
+00072430: 2069 6e20 636f 6c32 5f76 616c 293a 0a20   in col2_val):. 
+00072440: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
+00072450: 6e75 650a 2020 2020 2020 2020 656c 6966  nue.        elif
+00072460: 2027 524c 2720 6e6f 7420 696e 2063 6f6c   'RL' not in col
+00072470: 315f 7661 6c20 616e 6420 274c 5227 206e  1_val and 'LR' n
+00072480: 6f74 2069 6e20 636f 6c31 5f76 616c 2061  ot in col1_val a
+00072490: 6e64 2027 524c 2720 6e6f 7420 696e 2063  nd 'RL' not in c
+000724a0: 6f6c 325f 7661 6c20 616e 6420 274c 5227  ol2_val and 'LR'
+000724b0: 206e 6f74 2069 6e20 636f 6c32 5f76 616c   not in col2_val
+000724c0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+000724d0: 2073 697a 6531 203c 2073 697a 6532 3a0a   size1 < size2:.
+000724e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000724f0: 6466 5f63 6f70 792e 6174 5b69 6e64 6578  df_copy.at[index
+00072500: 2c20 636f 6c31 5d20 3d20 6466 5f63 6f70  , col1] = df_cop
+00072510: 792e 6174 5b69 6e64 6578 2c20 636f 6c32  y.at[index, col2
+00072520: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00072530: 2020 6466 5f63 6f70 792e 6174 5b69 6e64    df_copy.at[ind
+00072540: 6578 2c20 7369 7a65 5f63 6f6c 315d 203d  ex, size_col1] =
+00072550: 2064 665f 636f 7079 2e61 745b 696e 6465   df_copy.at[inde
+00072560: 782c 2073 697a 655f 636f 6c32 5d0a 2020  x, size_col2].  
+00072570: 2020 2020 2020 2020 2020 2020 2020 6466                df
+00072580: 5f63 6f70 792e 6174 5b69 6e64 6578 2c20  _copy.at[index, 
+00072590: 6964 315d 203d 2064 665f 636f 7079 2e61  id1] = df_copy.a
+000725a0: 745b 696e 6465 782c 2069 6432 5d0a 2020  t[index, id2].  
+000725b0: 2020 2020 2020 2020 2020 2020 2020 6466                df
+000725c0: 5f63 6f70 792e 6174 5b69 6e64 6578 2c20  _copy.at[index, 
+000725d0: 7369 7a65 5f63 6f6c 325d 203d 2030 0a20  size_col2] = 0. 
+000725e0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+000725f0: 665f 636f 7079 2e61 745b 696e 6465 782c  f_copy.at[index,
+00072600: 2063 6f6c 325d 203d 204e 6f6e 650a 2020   col2] = None.  
+00072610: 2020 2020 2020 2020 2020 2020 2020 6466                df
+00072620: 5f63 6f70 792e 6174 5b69 6e64 6578 2c20  _copy.at[index, 
+00072630: 6964 325d 203d 204e 6f6e 650a 2020 2020  id2] = None.    
+00072640: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00072650: 2020 2020 2020 2020 2020 2020 2020 6466                df
+00072660: 5f63 6f70 792e 6174 5b69 6e64 6578 2c20  _copy.at[index, 
+00072670: 636f 6c32 5d20 3d20 4e6f 6e65 0a20 2020  col2] = None.   
+00072680: 2020 2020 2020 2020 2020 2020 2064 665f               df_
+00072690: 636f 7079 2e61 745b 696e 6465 782c 2073  copy.at[index, s
+000726a0: 697a 655f 636f 6c32 5d20 3d20 300a 2020  ize_col2] = 0.  
+000726b0: 2020 2020 2020 2020 2020 2020 2020 6466                df
+000726c0: 5f63 6f70 792e 6174 5b69 6e64 6578 2c20  _copy.at[index, 
+000726d0: 6964 325d 203d 204e 6f6e 650a 2020 2020  id2] = None.    
+000726e0: 2020 2020 656c 6966 2027 524c 2720 696e      elif 'RL' in
+000726f0: 2063 6f6c 315f 7661 6c20 6f72 2027 4c52   col1_val or 'LR
+00072700: 2720 696e 2063 6f6c 315f 7661 6c3a 0a20  ' in col1_val:. 
+00072710: 2020 2020 2020 2020 2020 2069 6620 7369             if si
+00072720: 7a65 3120 3c20 7369 7a65 323a 0a20 2020  ze1 < size2:.   
+00072730: 2020 2020 2020 2020 2020 2020 2064 665f               df_
+00072740: 636f 7079 2e61 745b 696e 6465 782c 2063  copy.at[index, c
+00072750: 6f6c 315d 203d 2064 665f 636f 7079 2e61  ol1] = df_copy.a
+00072760: 745b 696e 6465 782c 2063 6f6c 325d 0a20  t[index, col2]. 
+00072770: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00072780: 665f 636f 7079 2e61 745b 696e 6465 782c  f_copy.at[index,
+00072790: 2069 6431 5d20 3d20 6466 5f63 6f70 792e   id1] = df_copy.
+000727a0: 6174 5b69 6e64 6578 2c20 6964 325d 0a20  at[index, id2]. 
+000727b0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+000727c0: 665f 636f 7079 2e61 745b 696e 6465 782c  f_copy.at[index,
+000727d0: 2073 697a 655f 636f 6c31 5d20 3d20 6466   size_col1] = df
+000727e0: 5f63 6f70 792e 6174 5b69 6e64 6578 2c20  _copy.at[index, 
+000727f0: 7369 7a65 5f63 6f6c 325d 0a20 2020 2020  size_col2].     
+00072800: 2020 2020 2020 2020 2020 2064 665f 636f             df_co
+00072810: 7079 2e61 745b 696e 6465 782c 2073 697a  py.at[index, siz
+00072820: 655f 636f 6c32 5d20 3d20 300a 2020 2020  e_col2] = 0.    
+00072830: 2020 2020 2020 2020 2020 2020 6466 5f63              df_c
+00072840: 6f70 792e 6174 5b69 6e64 6578 2c20 636f  opy.at[index, co
+00072850: 6c32 5d20 3d20 4e6f 6e65 0a20 2020 2020  l2] = None.     
+00072860: 2020 2020 2020 2020 2020 2064 665f 636f             df_co
+00072870: 7079 2e61 745b 696e 6465 782c 2069 6432  py.at[index, id2
+00072880: 5d20 3d20 4e6f 6e65 0a20 2020 2020 2020  ] = None.       
+00072890: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+000728a0: 2020 2020 2020 2020 2020 2064 665f 636f             df_co
+000728b0: 7079 2e61 745b 696e 6465 782c 2063 6f6c  py.at[index, col
+000728c0: 325d 203d 204e 6f6e 650a 2020 2020 2020  2] = None.      
+000728d0: 2020 2020 2020 2020 2020 6466 5f63 6f70            df_cop
+000728e0: 792e 6174 5b69 6e64 6578 2c20 6964 325d  y.at[index, id2]
+000728f0: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+00072900: 2020 2020 2020 2020 6466 5f63 6f70 792e          df_copy.
+00072910: 6174 5b69 6e64 6578 2c20 7369 7a65 5f63  at[index, size_c
+00072920: 6f6c 325d 203d 2030 0a20 2020 2020 2020  ol2] = 0.       
+00072930: 2065 6c69 6620 2752 4c27 2069 6e20 636f   elif 'RL' in co
+00072940: 6c32 5f76 616c 206f 7220 274c 5227 2069  l2_val or 'LR' i
+00072950: 6e20 636f 6c32 5f76 616c 3a0a 2020 2020  n col2_val:.    
+00072960: 2020 2020 2020 2020 6966 2073 697a 6532          if size2
+00072970: 203c 2073 697a 6531 3a0a 2020 2020 2020   < size1:.      
+00072980: 2020 2020 2020 2020 2020 6466 5f63 6f70            df_cop
+00072990: 792e 6174 5b69 6e64 6578 2c20 6964 325d  y.at[index, id2]
+000729a0: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+000729b0: 2020 2020 2020 2020 6466 5f63 6f70 792e          df_copy.
+000729c0: 6174 5b69 6e64 6578 2c20 636f 6c32 5d20  at[index, col2] 
+000729d0: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
+000729e0: 2020 2020 2020 2064 665f 636f 7079 2e61         df_copy.a
+000729f0: 745b 696e 6465 782c 2073 697a 655f 636f  t[index, size_co
+00072a00: 6c32 5d20 3d20 300a 2020 2020 2020 2020  l2] = 0.        
+00072a10: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00072a20: 2020 2020 2020 2020 2020 6466 5f63 6f70            df_cop
+00072a30: 792e 6174 5b69 6e64 6578 2c20 636f 6c31  y.at[index, col1
+00072a40: 5d20 3d20 6466 5f63 6f70 792e 6174 5b69  ] = df_copy.at[i
+00072a50: 6e64 6578 2c20 636f 6c32 5d0a 2020 2020  ndex, col2].    
+00072a60: 2020 2020 2020 2020 2020 2020 6466 5f63              df_c
+00072a70: 6f70 792e 6174 5b69 6e64 6578 2c20 6964  opy.at[index, id
+00072a80: 315d 203d 2064 665f 636f 7079 2e61 745b  1] = df_copy.at[
+00072a90: 696e 6465 782c 2069 6432 5d0a 2020 2020  index, id2].    
+00072aa0: 2020 2020 2020 2020 2020 2020 6466 5f63              df_c
+00072ab0: 6f70 792e 6174 5b69 6e64 6578 2c20 7369  opy.at[index, si
+00072ac0: 7a65 5f63 6f6c 315d 203d 2064 665f 636f  ze_col1] = df_co
+00072ad0: 7079 2e61 745b 696e 6465 782c 2073 697a  py.at[index, siz
+00072ae0: 655f 636f 6c32 5d0a 2020 2020 2020 2020  e_col2].        
+00072af0: 2020 2020 2020 2020 6466 5f63 6f70 792e          df_copy.
+00072b00: 6174 5b69 6e64 6578 2c20 7369 7a65 5f63  at[index, size_c
+00072b10: 6f6c 325d 203d 2030 0a20 2020 2020 2020  ol2] = 0.       
+00072b20: 2020 2020 2020 2020 2064 665f 636f 7079           df_copy
+00072b30: 2e61 745b 696e 6465 782c 2063 6f6c 325d  .at[index, col2]
+00072b40: 203d 204e 6f6e 6520 2020 200a 2020 2020   = None    .    
+00072b50: 2020 2020 2020 2020 2020 2020 6466 5f63              df_c
+00072b60: 6f70 792e 6174 5b69 6e64 6578 2c20 6964  opy.at[index, id
+00072b70: 325d 203d 204e 6f6e 6520 2020 200a 2020  2] = None    .  
+00072b80: 2020 7265 7475 726e 2064 665f 636f 7079    return df_copy
+00072b90: 0a0a 0a64 6566 2072 656e 616d 6569 7428  ...def renameit(
+00072ba0: 6466 2c20 6f6c 645f 636f 6c5f 6e61 6d65  df, old_col_name
+00072bb0: 2c20 6e65 775f 636f 6c5f 6e61 6d65 293a  , new_col_name):
+00072bc0: 0a20 2020 2022 2222 0a20 2020 2052 656e  .    """.    Ren
+00072bd0: 616d 6573 2061 2063 6f6c 756d 6e20 696e  ames a column in
+00072be0: 2061 2070 616e 6461 7320 4461 7461 4672   a pandas DataFr
+00072bf0: 616d 6520 696e 2070 6c61 6365 2e20 5261  ame in place. Ra
+00072c00: 6973 6573 2061 6e20 6572 726f 7220 6966  ises an error if
+00072c10: 2074 6865 2073 7065 6369 6669 6564 206f   the specified o
+00072c20: 6c64 2063 6f6c 756d 6e20 6e61 6d65 2064  ld column name d
+00072c30: 6f65 7320 6e6f 7420 6578 6973 742e 0a0a  oes not exist...
+00072c40: 2020 2020 5061 7261 6d65 7465 7273 3a0a      Parameters:.
+00072c50: 2020 2020 2d20 6466 3a20 7061 6e64 6173      - df: pandas
+00072c60: 2e44 6174 6146 7261 6d65 0a20 2020 2020  .DataFrame.     
+00072c70: 2020 2054 6865 2044 6174 6146 7261 6d65     The DataFrame
+00072c80: 2069 6e20 7768 6963 6820 7468 6520 636f   in which the co
+00072c90: 6c75 6d6e 2069 7320 746f 2062 6520 7265  lumn is to be re
+00072ca0: 6e61 6d65 642e 0a20 2020 202d 206f 6c64  named..    - old
+00072cb0: 5f63 6f6c 5f6e 616d 653a 2073 7472 0a20  _col_name: str. 
+00072cc0: 2020 2020 2020 2054 6865 2063 7572 7265         The curre
+00072cd0: 6e74 206e 616d 6520 6f66 2074 6865 2063  nt name of the c
+00072ce0: 6f6c 756d 6e20 746f 2062 6520 7265 6e61  olumn to be rena
+00072cf0: 6d65 642e 0a20 2020 202d 206e 6577 5f63  med..    - new_c
+00072d00: 6f6c 5f6e 616d 653a 2073 7472 0a20 2020  ol_name: str.   
+00072d10: 2020 2020 2054 6865 206e 6577 206e 616d       The new nam
+00072d20: 6520 666f 7220 7468 6520 636f 6c75 6d6e  e for the column
+00072d30: 2e0a 2020 2020 0a20 2020 2052 6169 7365  ..    .    Raise
+00072d40: 733a 0a20 2020 202d 2056 616c 7565 4572  s:.    - ValueEr
+00072d50: 726f 723a 2049 6620 7468 6520 6f6c 6420  ror: If the old 
+00072d60: 636f 6c75 6d6e 206e 616d 6520 646f 6573  column name does
+00072d70: 206e 6f74 2065 7869 7374 2069 6e20 7468   not exist in th
+00072d80: 6520 4461 7461 4672 616d 652e 0a20 2020  e DataFrame..   
+00072d90: 200a 2020 2020 5265 7475 726e 733a 0a20   .    Returns:. 
+00072da0: 2020 204e 6f6e 650a 2020 2020 2222 220a     None.    """.
+00072db0: 2020 2020 696d 706f 7274 2077 6172 6e69      import warni
+00072dc0: 6e67 730a 2020 2020 2320 4368 6563 6b20  ngs.    # Check 
+00072dd0: 6966 2074 6865 206f 6c64 2063 6f6c 756d  if the old colum
+00072de0: 6e20 6e61 6d65 2065 7869 7374 7320 696e  n name exists in
+00072df0: 2074 6865 2044 6174 6146 7261 6d65 0a20   the DataFrame. 
+00072e00: 2020 2069 6620 6f6c 645f 636f 6c5f 6e61     if old_col_na
+00072e10: 6d65 206e 6f74 2069 6e20 6466 2e63 6f6c  me not in df.col
+00072e20: 756d 6e73 3a0a 2020 2020 2020 2020 7761  umns:.        wa
+00072e30: 726e 696e 6773 2e77 6172 6e28 6622 5468  rnings.warn(f"Th
+00072e40: 6520 636f 6c75 6d6e 2027 7b6f 6c64 5f63  e column '{old_c
+00072e50: 6f6c 5f6e 616d 657d 2720 646f 6573 206e  ol_name}' does n
+00072e60: 6f74 2065 7869 7374 2069 6e20 7468 6520  ot exist in the 
+00072e70: 4461 7461 4672 616d 652e 2229 0a20 2020  DataFrame.").   
+00072e80: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+00072e90: 0a20 2020 2023 2050 726f 6365 6564 2077  .    # Proceed w
+00072ea0: 6974 6820 7265 6e61 6d69 6e67 2074 6865  ith renaming the
+00072eb0: 2063 6f6c 756d 6e20 6966 2069 7420 6578   column if it ex
+00072ec0: 6973 7473 0a20 2020 2064 662e 7265 6e61  ists.    df.rena
+00072ed0: 6d65 2863 6f6c 756d 6e73 3d7b 6f6c 645f  me(columns={old_
+00072ee0: 636f 6c5f 6e61 6d65 3a20 6e65 775f 636f  col_name: new_co
+00072ef0: 6c5f 6e61 6d65 7d2c 2069 6e70 6c61 6365  l_name}, inplace
+00072f00: 3d54 7275 6529 0a0a 0a64 6566 206d 6d5f  =True)...def mm_
+00072f10: 6d61 7463 685f 6279 5f71 635f 7363 6f72  match_by_qc_scor
+00072f20: 696e 675f 616c 6c28 2071 635f 6461 7461  ing_all( qc_data
+00072f30: 6672 616d 652c 2066 6978 5f4c 5252 4c3d  frame, fix_LRRL=
+00072f40: 5472 7565 2c20 7665 7262 6f73 653d 5472  True, verbose=Tr
+00072f50: 7565 2029 3a0a 2020 2020 2222 220a 2020  ue ):.    """.  
+00072f60: 2020 5072 6f63 6573 7365 7320 6120 7175    Processes a qu
+00072f70: 616c 6974 7920 636f 6e74 726f 6c20 2851  ality control (Q
+00072f80: 4329 2044 6174 6146 7261 6d65 2074 6f20  C) DataFrame to 
+00072f90: 7065 7266 6f72 6d20 6d6f 6461 6c69 7479  perform modality
+00072fa0: 2d73 7065 6369 6669 6320 6d61 7463 6869  -specific matchi
+00072fb0: 6e67 2061 6e64 2066 696c 7465 7269 6e67  ng and filtering
+00072fc0: 2062 6173 6564 0a20 2020 206f 6e20 7072   based.    on pr
+00072fd0: 6564 6566 696e 6564 2063 7269 7465 7269  edefined criteri
+00072fe0: 612c 206f 7074 696d 697a 696e 6720 666f  a, optimizing fo
+00072ff0: 7220 6d69 6e69 6d61 6c20 6f75 746c 6965  r minimal outlie
+00073000: 7273 2061 6e64 206e 6f69 7365 2c20 616e  rs and noise, an
+00073010: 6420 6d61 7869 6d61 6c20 7369 676e 616c  d maximal signal
+00073020: 2d74 6f2d 6e6f 6973 6520 7261 7469 6f20  -to-noise ratio 
+00073030: 2853 4e52 292c 0a20 2020 2065 7870 6563  (SNR),.    expec
+00073040: 7465 6420 7661 6c75 6520 6f66 2072 616e  ted value of ran
+00073050: 646f 6d6e 6573 7320 2845 5652 292c 2061  domness (EVR), a
+00073060: 6e64 2064 696d 656e 7369 6f6e 616c 6974  nd dimensionalit
+00073070: 7920 7469 6d65 2028 6469 6d74 292e 0a0a  y time (dimt)...
+00073080: 2020 2020 5468 6973 2066 756e 6374 696f      This functio
+00073090: 6e20 6974 6572 6174 6976 656c 7920 6d61  n iteratively ma
+000730a0: 7463 6865 7320 6461 7461 6672 616d 6573  tches dataframes
+000730b0: 2064 6572 6976 6564 2066 726f 6d20 7468   derived from th
+000730c0: 6520 5143 2064 6174 6166 7261 6d65 2066  e QC dataframe f
+000730d0: 6f72 2064 6966 6665 7265 6e74 2069 6d61  or different ima
+000730e0: 6769 6e67 206d 6f64 616c 6974 6965 732c  ging modalities,
+000730f0: 0a20 2020 2061 7070 6c79 696e 6720 6120  .    applying a 
+00073100: 7365 7269 6573 206f 6620 6669 6c74 6572  series of filter
+00073110: 7320 746f 2073 656c 6563 7420 7468 6520  s to select the 
+00073120: 6265 7374 206d 6174 6368 6573 2062 6173  best matches bas
+00073130: 6564 206f 6e20 7468 6520 5143 206d 6574  ed on the QC met
+00073140: 7269 6373 2e20 4d61 7463 6865 7320 6172  rics. Matches ar
+00073150: 6520 6d61 6465 2077 6974 680a 2020 2020  e made with.    
+00073160: 636f 6e73 6964 6572 6174 696f 6e20 746f  consideration to
+00073170: 206d 696e 696d 697a 6520 6f75 746c 6965   minimize outlie
+00073180: 7220 6c6f 6f70 2061 6e64 206e 6f69 7365  r loop and noise
+00073190: 2c20 7768 696c 6520 6d61 7869 6d69 7a69  , while maximizi
+000731a0: 6e67 2053 4e52 2c20 4556 522c 2061 6e64  ng SNR, EVR, and
+000731b0: 2064 696d 7420 666f 7220 6561 6368 206d   dimt for each m
+000731c0: 6f64 616c 6974 792e 0a0a 2020 2020 5061  odality...    Pa
+000731d0: 7261 6d65 7465 7273 3a0a 2020 2020 2d2d  rameters:.    --
+000731e0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2071 635f  --------.    qc_
+000731f0: 6461 7461 6672 616d 6520 3a20 7061 6e64  dataframe : pand
+00073200: 6173 2e44 6174 6146 7261 6d65 0a20 2020  as.DataFrame.   
+00073210: 2020 2020 2054 6865 2044 6174 6146 7261       The DataFra
+00073220: 6d65 2063 6f6e 7461 696e 696e 6720 5143  me containing QC
+00073230: 206d 6574 7269 6373 2066 6f72 2064 6966   metrics for dif
+00073240: 6665 7265 6e74 206d 6f64 616c 6974 6965  ferent modalitie
+00073250: 7320 616e 6420 696d 6167 696e 6720 6461  s and imaging da
+00073260: 7461 2e0a 2020 2020 6669 785f 4c52 524c  ta..    fix_LRRL
+00073270: 203a 2062 6f6f 6c2c 206f 7074 696f 6e61   : bool, optiona
+00073280: 6c0a 0a20 2020 2076 6572 626f 7365 203a  l..    verbose :
+00073290: 2062 6f6f 6c2c 206f 7074 696f 6e61 6c0a   bool, optional.
+000732a0: 2020 2020 2020 2020 4966 2054 7275 652c          If True,
+000732b0: 2070 7269 6e74 7320 7468 6520 7072 6f67   prints the prog
+000732c0: 7265 7373 2061 6e64 2074 6865 2073 6861  ress and the sha
+000732d0: 7065 206f 6620 7468 6520 4461 7461 4672  pe of the DataFr
+000732e0: 616d 6520 6265 696e 6720 7072 6f63 6573  ame being proces
+000732f0: 7365 6420 696e 2065 6163 6820 7374 6570  sed in each step
+00073300: 2e0a 0a20 2020 2050 726f 6365 7373 3a0a  ...    Process:.
+00073310: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+00073320: 312e 2053 7461 6e64 6172 6469 7a65 7320  1. Standardizes 
+00073330: 6d6f 6461 6c69 7469 6573 2062 7920 6d65  modalities by me
+00073340: 7267 696e 6720 4454 492d 7265 6c61 7465  rging DTI-relate
+00073350: 6420 656e 7472 6965 732e 0a20 2020 2032  d entries..    2
+00073360: 2e20 436f 6e76 6572 7473 2073 7065 6369  . Converts speci
+00073370: 6669 6320 636f 6c75 6d6e 7320 746f 2061  fic columns to a
+00073380: 7070 726f 7072 6961 7465 2064 6174 6120  ppropriate data 
+00073390: 7479 7065 7320 666f 7220 7072 6f63 6573  types for proces
+000733a0: 7369 6e67 2e0a 2020 2020 332e 2050 6572  sing..    3. Per
+000733b0: 666f 726d 7320 6d6f 6461 6c69 7479 2d73  forms modality-s
+000733c0: 7065 6369 6669 6320 6d61 7463 6869 6e67  pecific matching
+000733d0: 2061 6e64 2066 696c 7465 7269 6e67 2062   and filtering b
+000733e0: 6173 6564 206f 6e20 7468 6520 6f75 746c  ased on the outl
+000733f0: 6965 7220 636f 6c75 6d6e 2061 6e64 2063  ier column and c
+00073400: 7269 7465 7269 6120 666f 7220 6561 6368  riteria for each
+00073410: 206d 6f64 616c 6974 792e 0a20 2020 2034   modality..    4
+00073420: 2e20 4974 6572 6174 6976 656c 7920 7072  . Iteratively pr
+00073430: 6f63 6573 7365 7320 756e 6d61 7463 6865  ocesses unmatche
+00073440: 6420 6461 7461 2066 6f72 2070 7265 6465  d data for prede
+00073450: 6669 6e65 6420 6d6f 6461 6c69 7469 6573  fined modalities
+00073460: 2077 6974 6820 7370 6563 6966 6963 2070   with specific p
+00073470: 7265 6669 7865 7320 746f 2066 696e 6420  refixes to find 
+00073480: 6675 7274 6865 7220 6d61 7463 6865 732e  further matches.
+00073490: 0a20 2020 200a 2020 2020 5265 7475 726e  .    .    Return
+000734a0: 733a 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  s:.    -------. 
+000734b0: 2020 2070 616e 6461 732e 4461 7461 4672     pandas.DataFr
+000734c0: 616d 650a 2020 2020 2020 2020 5468 6520  ame.        The 
+000734d0: 6d61 7463 6865 6420 616e 6420 6669 6c74  matched and filt
+000734e0: 6572 6564 2044 6174 6146 7261 6d65 2061  ered DataFrame a
+000734f0: 6674 6572 2061 7070 6c79 696e 6720 616c  fter applying al
+00073500: 6c20 5143 2073 636f 7269 6e67 2061 6e64  l QC scoring and
+00073510: 206d 6174 6368 696e 6720 6f70 6572 6174   matching operat
+00073520: 696f 6e73 2061 6372 6f73 7320 7370 6563  ions across spec
+00073530: 6966 6965 6420 6d6f 6461 6c69 7469 6573  ified modalities
+00073540: 2e0a 0a20 2020 2022 2222 0a20 2020 2071  ...    """.    q
+00073550: 635f 6461 7461 6672 616d 655b 276d 6f64  c_dataframe['mod
+00073560: 616c 6974 7927 5d20 3d20 7163 5f64 6174  ality'] = qc_dat
+00073570: 6166 7261 6d65 5b27 6d6f 6461 6c69 7479  aframe['modality
+00073580: 275d 2e72 6570 6c61 6365 285b 2744 5449  '].replace(['DTI
+00073590: 6477 6927 2c20 2744 5449 6230 275d 2c20  dwi', 'DTIb0'], 
+000735a0: 2744 5449 272c 2072 6567 6578 3d54 7275  'DTI', regex=Tru
+000735b0: 6529 0a20 2020 2071 635f 6461 7461 6672  e).    qc_datafr
+000735c0: 616d 655b 2766 696c 656e 616d 6527 5d3d  ame['filename']=
+000735d0: 7163 5f64 6174 6166 7261 6d65 5b27 6669  qc_dataframe['fi
+000735e0: 6c65 6e61 6d65 275d 2e61 7374 7970 6528  lename'].astype(
+000735f0: 7374 7229 0a20 2020 2071 635f 6461 7461  str).    qc_data
+00073600: 6672 616d 655b 276f 6c5f 6c6f 6f70 275d  frame['ol_loop']
+00073610: 3d71 635f 6461 7461 6672 616d 655b 276f  =qc_dataframe['o
+00073620: 6c5f 6c6f 6f70 275d 2e61 7374 7970 6528  l_loop'].astype(
+00073630: 666c 6f61 7429 0a20 2020 2071 635f 6461  float).    qc_da
+00073640: 7461 6672 616d 655b 276f 6c5f 6c6f 6627  taframe['ol_lof'
+00073650: 5d3d 7163 5f64 6174 6166 7261 6d65 5b27  ]=qc_dataframe['
+00073660: 6f6c 5f6c 6f66 275d 2e61 7374 7970 6528  ol_lof'].astype(
+00073670: 666c 6f61 7429 0a20 2020 2071 635f 6461  float).    qc_da
+00073680: 7461 6672 616d 655b 276f 6c5f 6c6f 665f  taframe['ol_lof_
+00073690: 6465 6369 7369 6f6e 275d 3d71 635f 6461  decision']=qc_da
+000736a0: 7461 6672 616d 655b 276f 6c5f 6c6f 665f  taframe['ol_lof_
+000736b0: 6465 6369 7369 6f6e 275d 2e61 7374 7970  decision'].astyp
+000736c0: 6528 666c 6f61 7429 0a20 2020 206f 7574  e(float).    out
+000736d0: 6c69 6572 5f63 6f6c 756d 6e3d 276f 6c5f  lier_column='ol_
+000736e0: 6c6f 6f70 270a 2020 2020 6d6d 6466 3020  loop'.    mmdf0 
+000736f0: 3d20 6265 7374 5f6d 6d6d 2820 7163 5f64  = best_mmm( qc_d
+00073700: 6174 6166 7261 6d65 2c20 2754 3177 272c  ataframe, 'T1w',
+00073710: 206f 7574 6c69 6572 5f63 6f6c 756d 6e3d   outlier_column=
+00073720: 6f75 746c 6965 725f 636f 6c75 6d6e 2029  outlier_column )
+00073730: 5b27 6669 6c74 275d 0a20 2020 2066 6c64  ['filt'].    fld
+00073740: 6620 3d20 6265 7374 5f6d 6d6d 2820 7163  f = best_mmm( qc
+00073750: 5f64 6174 6166 7261 6d65 2c20 2754 3246  _dataframe, 'T2F
+00073760: 6c61 6972 272c 206f 7574 6c69 6572 5f63  lair', outlier_c
+00073770: 6f6c 756d 6e3d 6f75 746c 6965 725f 636f  olumn=outlier_co
+00073780: 6c75 6d6e 2029 5b27 6669 6c74 275d 0a20  lumn )['filt']. 
+00073790: 2020 206e 6d64 6620 3d20 6265 7374 5f6d     nmdf = best_m
+000737a0: 6d6d 2820 7163 5f64 6174 6166 7261 6d65  mm( qc_dataframe
+000737b0: 2c20 274e 4d32 444d 5427 2c20 6f75 746c  , 'NM2DMT', outl
+000737c0: 6965 725f 636f 6c75 6d6e 3d6f 7574 6c69  ier_column=outli
+000737d0: 6572 5f63 6f6c 756d 6e20 295b 2766 696c  er_column )['fil
+000737e0: 7427 5d0a 2020 2020 7273 6466 203d 2062  t'].    rsdf = b
+000737f0: 6573 745f 6d6d 6d28 2071 635f 6461 7461  est_mmm( qc_data
+00073800: 6672 616d 652c 2027 7273 664d 5249 272c  frame, 'rsfMRI',
+00073810: 206f 7574 6c69 6572 5f63 6f6c 756d 6e3d   outlier_column=
+00073820: 6f75 746c 6965 725f 636f 6c75 6d6e 2029  outlier_column )
+00073830: 5b27 6669 6c74 275d 0a20 2020 2064 7464  ['filt'].    dtd
+00073840: 6620 3d20 6265 7374 5f6d 6d6d 2820 7163  f = best_mmm( qc
+00073850: 5f64 6174 6166 7261 6d65 2c20 2744 5449  _dataframe, 'DTI
+00073860: 272c 206f 7574 6c69 6572 5f63 6f6c 756d  ', outlier_colum
+00073870: 6e3d 6f75 746c 6965 725f 636f 6c75 6d6e  n=outlier_column
+00073880: 2029 5b27 6669 6c74 275d 0a0a 2020 2020   )['filt']..    
+00073890: 6372 6974 6572 6961 203d 207b 276f 6c5f  criteria = {'ol_
+000738a0: 6c6f 6f70 273a 2027 6d69 6e27 2c20 276e  loop': 'min', 'n
+000738b0: 6f69 7365 273a 2027 6d69 6e27 2c20 2773  oise': 'min', 's
+000738c0: 6e72 273a 2027 6d61 7827 2c20 2745 5652  nr': 'max', 'EVR
+000738d0: 273a 2027 6d61 7827 2c20 2772 6566 6c65  ': 'max', 'refle
+000738e0: 6374 696f 6e5f 6572 7227 3a27 6d69 6e27  ction_err':'min'
+000738f0: 7d0a 2020 2020 7863 6c20 3d20 5b20 276d  }.    xcl = [ 'm
+00073900: 7269 6d66 6727 2c20 276d 7269 6d6f 6465  rimfg', 'mrimode
+00073910: 6c27 2c27 6d72 694d 6167 6e65 7469 6346  l','mriMagneticF
+00073920: 6965 6c64 5374 7265 6e67 7468 272c 2027  ieldStrength', '
+00073930: 6474 695f 6661 696c 6564 272c 2027 7273  dti_failed', 'rs
+00073940: 665f 6661 696c 6564 272c 2027 7375 626a  f_failed', 'subj
+00073950: 6563 7449 4427 2c20 2764 6174 6527 2c20  ectID', 'date', 
+00073960: 2773 7562 6a65 6374 4944 6461 7465 272c  'subjectIDdate',
+00073970: 2772 6570 6561 7427 5d0a 2020 2020 2320  'repeat'].    # 
+00073980: 4173 7375 6d69 6e67 2064 665f 6120 616e  Assuming df_a an
+00073990: 6420 6466 5f62 2061 7265 2061 6c72 6561  d df_b are alrea
+000739a0: 6479 206c 6f61 6465 640a 2020 2020 6d6d  dy loaded.    mm
+000739b0: 6466 2c20 756e 6466 666c 203d 206d 6d5f  df, undffl = mm_
+000739c0: 6d61 7463 685f 6279 5f71 635f 7363 6f72  match_by_qc_scor
+000739d0: 696e 6728 6d6d 6466 302c 2066 6c64 662c  ing(mmdf0, fldf,
+000739e0: 2027 7375 626a 6563 7449 4464 6174 6527   'subjectIDdate'
+000739f0: 2c20 6372 6974 6572 6961 2c20 0a20 2020  , criteria, .   
+00073a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00073a10: 2020 2020 2070 7265 6669 783d 2754 3246       prefix='T2F
+00073a20: 6c61 6972 5f27 2c20 6578 636c 7564 655f  lair_', exclude_
+00073a30: 636f 6c75 6d6e 733d 7863 6c20 290a 0a20  columns=xcl ).. 
+00073a40: 2020 2070 7265 6669 7865 7320 3d20 5b27     prefixes = ['
+00073a50: 4e4d 315f 272c 2027 4e4d 325f 272c 2027  NM1_', 'NM2_', '
+00073a60: 4e4d 335f 272c 2027 4e4d 345f 272c 2027  NM3_', 'NM4_', '
+00073a70: 4e4d 355f 272c 2027 4e4d 365f 275d 2020  NM5_', 'NM6_']  
+00073a80: 0a20 2020 2075 6e64 666d 6f64 203d 206e  .    undfmod = n
+00073a90: 6d64 6620 2023 2049 6e69 7469 616c 697a  mdf  # Initializ
+00073aa0: 6520 2775 6e64 666d 6f64 2720 7769 7468  e 'undfmod' with
+00073ab0: 2027 6e6d 6466 2720 666f 7220 7468 6520   'nmdf' for the 
+00073ac0: 6669 7273 7420 6974 6572 6174 696f 6e0a  first iteration.
+00073ad0: 2020 2020 6966 2076 6572 626f 7365 3a0a      if verbose:.
+00073ae0: 2020 2020 2020 2020 7072 696e 7428 2773          print('s
+00073af0: 7461 7274 204e 4d27 290a 2020 2020 2020  tart NM').      
+00073b00: 2020 7072 696e 7428 2075 6e64 666d 6f64    print( undfmod
+00073b10: 2e73 6861 7065 2029 0a20 2020 2066 6f72  .shape ).    for
+00073b20: 2070 7265 6669 7820 696e 2070 7265 6669   prefix in prefi
+00073b30: 7865 733a 0a20 2020 2020 2020 2069 6620  xes:.        if 
+00073b40: 756e 6466 6d6f 642e 7368 6170 655b 305d  undfmod.shape[0]
+00073b50: 203e 2035 303a 0a20 2020 2020 2020 2020   > 50:.         
+00073b60: 2020 206d 6d64 662c 2075 6e64 666d 6f64     mmdf, undfmod
+00073b70: 203d 206d 6d5f 6d61 7463 685f 6279 5f71   = mm_match_by_q
+00073b80: 635f 7363 6f72 696e 6728 6d6d 6466 2c20  c_scoring(mmdf, 
+00073b90: 756e 6466 6d6f 642c 2027 7375 626a 6563  undfmod, 'subjec
+00073ba0: 7449 4464 6174 6527 2c20 6372 6974 6572  tIDdate', criter
+00073bb0: 6961 2c20 7072 6566 6978 3d70 7265 6669  ia, prefix=prefi
+00073bc0: 782c 2065 7863 6c75 6465 5f63 6f6c 756d  x, exclude_colum
+00073bd0: 6e73 3d78 636c 290a 2020 2020 2020 2020  ns=xcl).        
+00073be0: 2020 2020 6966 2076 6572 626f 7365 3a0a      if verbose:.
+00073bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00073c00: 7072 696e 7428 2070 7265 6669 7820 290a  print( prefix ).
+00073c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00073c20: 7072 696e 7428 2075 6e64 666d 6f64 2e73  print( undfmod.s
+00073c30: 6861 7065 2029 0a0a 2020 2020 6372 6974  hape )..    crit
+00073c40: 6572 6961 203d 207b 276f 6c5f 6c6f 6f70  eria = {'ol_loop
+00073c50: 273a 2027 6d69 6e27 2c20 276e 6f69 7365  ': 'min', 'noise
+00073c60: 273a 2027 6d69 6e27 2c20 2773 6e72 273a  ': 'min', 'snr':
+00073c70: 2027 6d61 7827 2c20 2745 5652 273a 2027   'max', 'EVR': '
+00073c80: 6d61 7827 2c20 2764 696d 7427 3a27 6d61  max', 'dimt':'ma
+00073c90: 7827 7d0a 2020 2020 2320 6869 6768 6572  x'}.    # higher
+00073ca0: 2062 7661 6c75 6573 206c 6561 6420 746f   bvalues lead to
+00073cb0: 206d 6f72 6520 6e6f 6973 6520 2e2e 2e0a   more noise ....
+00073cc0: 2020 2020 6372 6974 6572 6961 203d 207b      criteria = {
+00073cd0: 276f 6c5f 6c6f 6f70 273a 2027 6d69 6e27  'ol_loop': 'min'
+00073ce0: 2c20 276e 6f69 7365 273a 2027 6d69 6e27  , 'noise': 'min'
+00073cf0: 2c20 2027 6474 695f 6276 616c 7565 4d61  ,  'dti_bvalueMa
+00073d00: 7827 3a27 6d69 6e27 2c20 2027 6469 6d74  x':'min',  'dimt
+00073d10: 273a 276d 6178 277d 0a20 2020 2070 7265  ':'max'}.    pre
+00073d20: 6669 7865 7320 3d20 5b27 4454 4931 5f27  fixes = ['DTI1_'
+00073d30: 2c20 2744 5449 325f 272c 2027 4454 4933  , 'DTI2_', 'DTI3
+00073d40: 5f27 5d20 2023 204c 6973 7420 6f66 2070  _']  # List of p
+00073d50: 7265 6669 7865 7320 666f 7220 6561 6368  refixes for each
+00073d60: 206d 6174 6368 696e 6720 6974 6572 6174   matching iterat
+00073d70: 696f 6e0a 2020 2020 756e 6466 6d6f 6420  ion.    undfmod 
+00073d80: 3d20 6474 6466 0a20 2020 2069 6620 7665  = dtdf.    if ve
+00073d90: 7262 6f73 653a 0a20 2020 2020 2020 2070  rbose:.        p
+00073da0: 7269 6e74 2827 7374 6172 7420 4454 2729  rint('start DT')
+00073db0: 0a20 2020 2020 2020 2070 7269 6e74 2820  .        print( 
+00073dc0: 756e 6466 6d6f 642e 7368 6170 6520 290a  undfmod.shape ).
+00073dd0: 2020 2020 666f 7220 7072 6566 6978 2069      for prefix i
+00073de0: 6e20 7072 6566 6978 6573 3a0a 2020 2020  n prefixes:.    
+00073df0: 2020 2020 6966 2075 6e64 666d 6f64 2e73      if undfmod.s
+00073e00: 6861 7065 5b30 5d20 3e20 3530 3a0a 2020  hape[0] > 50:.  
+00073e10: 2020 2020 2020 2020 2020 6d6d 6466 2c20            mmdf, 
+00073e20: 756e 6466 6d6f 6420 3d20 6d6d 5f6d 6174  undfmod = mm_mat
+00073e30: 6368 5f62 795f 7163 5f73 636f 7269 6e67  ch_by_qc_scoring
+00073e40: 286d 6d64 662c 2075 6e64 666d 6f64 2c20  (mmdf, undfmod, 
+00073e50: 2773 7562 6a65 6374 4944 6461 7465 272c  'subjectIDdate',
+00073e60: 2063 7269 7465 7269 612c 2070 7265 6669   criteria, prefi
+00073e70: 783d 7072 6566 6978 2c20 6578 636c 7564  x=prefix, exclud
+00073e80: 655f 636f 6c75 6d6e 733d 7863 6c29 0a20  e_columns=xcl). 
+00073e90: 2020 2020 2020 2020 2020 2069 6620 7665             if ve
+00073ea0: 7262 6f73 653a 0a20 2020 2020 2020 2020  rbose:.         
+00073eb0: 2020 2020 2020 2070 7269 6e74 2820 7072         print( pr
+00073ec0: 6566 6978 2029 0a20 2020 2020 2020 2020  efix ).         
+00073ed0: 2020 2020 2020 2070 7269 6e74 2820 756e         print( un
+00073ee0: 6466 6d6f 642e 7368 6170 6520 290a 0a20  dfmod.shape ).. 
+00073ef0: 2020 2070 7265 6669 7865 7320 3d20 5b27     prefixes = ['
+00073f00: 7273 6631 5f27 2c20 2772 7366 325f 272c  rsf1_', 'rsf2_',
+00073f10: 2027 7273 6633 5f27 5d20 2023 204c 6973   'rsf3_']  # Lis
+00073f20: 7420 6f66 2070 7265 6669 7865 7320 666f  t of prefixes fo
+00073f30: 7220 6561 6368 206d 6174 6368 696e 6720  r each matching 
+00073f40: 6974 6572 6174 696f 6e0a 2020 2020 756e  iteration.    un
+00073f50: 6466 6d6f 6420 3d20 7273 6466 2020 2320  dfmod = rsdf  # 
+00073f60: 496e 6974 6961 6c69 7a65 2027 756e 6466  Initialize 'undf
+00073f70: 6d6f 6427 2077 6974 6820 276e 6d64 6627  mod' with 'nmdf'
+00073f80: 2066 6f72 2074 6865 2066 6972 7374 2069   for the first i
+00073f90: 7465 7261 7469 6f6e 0a20 2020 2069 6620  teration.    if 
+00073fa0: 7665 7262 6f73 653a 0a20 2020 2020 2020  verbose:.       
+00073fb0: 2070 7269 6e74 2827 7374 6172 7420 7273   print('start rs
+00073fc0: 6627 290a 2020 2020 2020 2020 7072 696e  f').        prin
+00073fd0: 7428 2075 6e64 666d 6f64 2e73 6861 7065  t( undfmod.shape
+00073fe0: 2029 0a20 2020 2066 6f72 2070 7265 6669   ).    for prefi
+00073ff0: 7820 696e 2070 7265 6669 7865 733a 0a20  x in prefixes:. 
+00074000: 2020 2020 2020 2069 6620 756e 6466 6d6f         if undfmo
+00074010: 642e 7368 6170 655b 305d 203e 2035 303a  d.shape[0] > 50:
+00074020: 0a20 2020 2020 2020 2020 2020 206d 6d64  .            mmd
+00074030: 662c 2075 6e64 666d 6f64 203d 206d 6d5f  f, undfmod = mm_
+00074040: 6d61 7463 685f 6279 5f71 635f 7363 6f72  match_by_qc_scor
+00074050: 696e 6728 6d6d 6466 2c20 756e 6466 6d6f  ing(mmdf, undfmo
+00074060: 642c 2027 7375 626a 6563 7449 4464 6174  d, 'subjectIDdat
+00074070: 6527 2c20 6372 6974 6572 6961 2c20 7072  e', criteria, pr
+00074080: 6566 6978 3d70 7265 6669 782c 2065 7863  efix=prefix, exc
+00074090: 6c75 6465 5f63 6f6c 756d 6e73 3d78 636c  lude_columns=xcl
+000740a0: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+000740b0: 2076 6572 626f 7365 3a0a 2020 2020 2020   verbose:.      
+000740c0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+000740d0: 2070 7265 6669 7820 290a 2020 2020 2020   prefix ).      
+000740e0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+000740f0: 2075 6e64 666d 6f64 2e73 6861 7065 2029   undfmod.shape )
+00074100: 0a20 2020 200a 2020 2020 6966 2066 6978  .    .    if fix
+00074110: 5f4c 5252 4c3a 0a20 2020 2020 2020 2023  _LRRL:.        #
+00074120: 2020 2020 2020 2020 6d6d 6466 3d66 6978          mmdf=fix
+00074130: 5f4c 525f 524c 5f73 7475 6666 2820 6d6d  _LR_RL_stuff( mm
+00074140: 6466 2c20 2744 5449 315f 6669 6c65 6e61  df, 'DTI1_filena
+00074150: 6d65 272c 2027 4454 4932 5f66 696c 656e  me', 'DTI2_filen
+00074160: 616d 6527 2c20 2744 5449 315f 6469 6d74  ame', 'DTI1_dimt
+00074170: 272c 2027 4454 4932 5f64 696d 7427 290a  ', 'DTI2_dimt').
+00074180: 2020 2020 2020 2020 6d6d 6466 3d66 6978          mmdf=fix
+00074190: 5f4c 525f 524c 5f73 7475 6666 2820 6d6d  _LR_RL_stuff( mm
+000741a0: 6466 2c20 2772 7366 315f 6669 6c65 6e61  df, 'rsf1_filena
+000741b0: 6d65 272c 2027 7273 6632 5f66 696c 656e  me', 'rsf2_filen
+000741c0: 616d 6527 2c20 2772 7366 315f 6469 6d74  ame', 'rsf1_dimt
+000741d0: 272c 2027 7273 6632 5f64 696d 7427 2c20  ', 'rsf2_dimt', 
+000741e0: 2772 7366 315f 696d 6167 6549 4427 2c20  'rsf1_imageID', 
+000741f0: 2772 7366 325f 696d 6167 6549 4427 2020  'rsf2_imageID'  
+00074200: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
+00074210: 2020 2020 696d 706f 7274 2077 6172 6e69      import warni
+00074220: 6e67 730a 2020 2020 2020 2020 7761 726e  ngs.        warn
+00074230: 696e 6773 2e77 6172 6e28 2246 4958 4d45  ings.warn("FIXME
+00074240: 3a20 7368 6f75 6c64 2066 6978 204c 5220  : should fix LR 
+00074250: 616e 6420 524c 2073 6974 7561 7469 6f6e  and RL situation
+00074260: 2066 6f72 2074 6865 2044 5449 2061 6e64   for the DTI and
+00074270: 2072 7366 4d52 4922 290a 0a20 2020 2023   rsfMRI")..    #
+00074280: 206e 6f77 2064 6f20 7468 6520 6e65 6365   now do the nece
+00074290: 7373 6172 7920 7265 706c 6163 656d 656e  ssary replacemen
+000742a0: 7473 0a20 2020 200a 2020 2020 7265 6e61  ts.    .    rena
+000742b0: 6d65 6974 2820 6d6d 6466 2c20 2770 6572  meit( mmdf, 'per
+000742c0: 665f 696d 6167 6549 4427 2c20 2770 6572  f_imageID', 'per
+000742d0: 6669 6427 2029 0a20 2020 2072 656e 616d  fid' ).    renam
+000742e0: 6569 7428 206d 6d64 662c 2027 7065 7266  eit( mmdf, 'perf
+000742f0: 5f66 696c 656e 616d 6527 2c20 2770 6572  _filename', 'per
+00074300: 6666 6e27 2029 0a20 2020 2072 656e 616d  ffn' ).    renam
+00074310: 6569 7428 206d 6d64 662c 2027 5432 466c  eit( mmdf, 'T2Fl
+00074320: 6169 725f 696d 6167 6549 4427 2c20 2766  air_imageID', 'f
+00074330: 6c61 6972 6964 2720 290a 2020 2020 7265  lairid' ).    re
+00074340: 6e61 6d65 6974 2820 6d6d 6466 2c20 2754  nameit( mmdf, 'T
+00074350: 3246 6c61 6972 5f66 696c 656e 616d 6527  2Flair_filename'
+00074360: 2c20 2766 6c61 6972 666e 2720 290a 2020  , 'flairfn' ).  
+00074370: 2020 7265 6e61 6d65 6974 2820 6d6d 6466    renameit( mmdf
+00074380: 2c20 2772 7366 315f 696d 6167 6549 4427  , 'rsf1_imageID'
+00074390: 2c20 2772 7366 6964 3127 2029 0a20 2020  , 'rsfid1' ).   
+000743a0: 2072 656e 616d 6569 7428 206d 6d64 662c   renameit( mmdf,
+000743b0: 2027 7273 6632 5f69 6d61 6765 4944 272c   'rsf2_imageID',
+000743c0: 2027 7273 6669 6432 2720 290a 2020 2020   'rsfid2' ).    
+000743d0: 7265 6e61 6d65 6974 2820 6d6d 6466 2c20  renameit( mmdf, 
+000743e0: 2772 7366 315f 6669 6c65 6e61 6d65 272c  'rsf1_filename',
+000743f0: 2027 7273 6666 6e31 2720 290a 2020 2020   'rsffn1' ).    
+00074400: 7265 6e61 6d65 6974 2820 6d6d 6466 2c20  renameit( mmdf, 
+00074410: 2772 7366 325f 6669 6c65 6e61 6d65 272c  'rsf2_filename',
+00074420: 2027 7273 6666 6e32 2720 290a 2020 2020   'rsffn2' ).    
+00074430: 7265 6e61 6d65 6974 2820 6d6d 6466 2c20  renameit( mmdf, 
+00074440: 2744 5449 315f 696d 6167 6549 4427 2c20  'DTI1_imageID', 
+00074450: 2764 7469 6431 2720 290a 2020 2020 7265  'dtid1' ).    re
+00074460: 6e61 6d65 6974 2820 6d6d 6466 2c20 2744  nameit( mmdf, 'D
+00074470: 5449 325f 696d 6167 6549 4427 2c20 2764  TI2_imageID', 'd
+00074480: 7469 6432 2720 290a 2020 2020 7265 6e61  tid2' ).    rena
+00074490: 6d65 6974 2820 6d6d 6466 2c20 2744 5449  meit( mmdf, 'DTI
+000744a0: 335f 696d 6167 6549 4427 2c20 2764 7469  3_imageID', 'dti
+000744b0: 6433 2720 290a 2020 2020 7265 6e61 6d65  d3' ).    rename
+000744c0: 6974 2820 6d6d 6466 2c20 2744 5449 315f  it( mmdf, 'DTI1_
+000744d0: 6669 6c65 6e61 6d65 272c 2027 6474 666e  filename', 'dtfn
+000744e0: 3127 2029 0a20 2020 2072 656e 616d 6569  1' ).    renamei
+000744f0: 7428 206d 6d64 662c 2027 4454 4932 5f66  t( mmdf, 'DTI2_f
+00074500: 696c 656e 616d 6527 2c20 2764 7466 6e32  ilename', 'dtfn2
+00074510: 2720 290a 2020 2020 7265 6e61 6d65 6974  ' ).    renameit
+00074520: 2820 6d6d 6466 2c20 2744 5449 335f 6669  ( mmdf, 'DTI3_fi
+00074530: 6c65 6e61 6d65 272c 2027 6474 666e 3327  lename', 'dtfn3'
+00074540: 2029 0a20 2020 2066 6f72 2078 2069 6e20   ).    for x in 
+00074550: 7261 6e67 6528 312c 3629 3a0a 2020 2020  range(1,6):.    
+00074560: 2020 2020 7465 6d70 303d 224e 4d22 2b73      temp0="NM"+s
+00074570: 7472 2878 292b 225f 696d 6167 6549 4422  tr(x)+"_imageID"
+00074580: 0a20 2020 2020 2020 2074 656d 7031 3d22  .        temp1="
+00074590: 6e6d 6964 222b 7374 7228 7829 0a20 2020  nmid"+str(x).   
+000745a0: 2020 2020 2072 656e 616d 6569 7428 206d       renameit( m
+000745b0: 6d64 662c 2074 656d 7030 2c20 7465 6d70  mdf, temp0, temp
+000745c0: 3120 290a 2020 2020 2020 2020 7465 6d70  1 ).        temp
+000745d0: 303d 224e 4d22 2b73 7472 2878 292b 225f  0="NM"+str(x)+"_
+000745e0: 6669 6c65 6e61 6d65 220a 2020 2020 2020  filename".      
+000745f0: 2020 7465 6d70 313d 226e 6d66 6e22 2b73    temp1="nmfn"+s
+00074600: 7472 2878 290a 2020 2020 2020 2020 7265  tr(x).        re
+00074610: 6e61 6d65 6974 2820 6d6d 6466 2c20 7465  nameit( mmdf, te
+00074620: 6d70 302c 2074 656d 7031 2029 0a20 2020  mp0, temp1 ).   
+00074630: 2072 6574 7572 6e20 6d6d 6466 0a          return mmdf.
```

### Comparing `antspymm-1.3.1/antspymm.egg-info/PKG-INFO` & `antspymm-1.3.3/antspymm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antspymm
-Version: 1.3.1
+Version: 1.3.3
 Summary: multi-channel/time-series medical image processing with antspyx
 Home-page: https://github.com/stnava/ANTsPyMM
 Author: Avants, Gosselin, Tustison, Reardon
 Author-email: stnava@gmail.com
 License: Apache 2.0
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE
```

### Comparing `antspymm-1.3.1/antspymm.egg-info/SOURCES.txt` & `antspymm-1.3.3/antspymm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `antspymm-1.3.1/docs/adni_rsfmri_2_nrg_conversion.py` & `antspymm-1.3.3/docs/adni_rsfmri_2_nrg_conversion.py`

 * *Files identical despite different names*

### Comparing `antspymm-1.3.1/docs/antspymm_data_dictionary.csv` & `antspymm-1.3.3/docs/antspymm_data_dictionary.csv`

 * *Files identical despite different names*

### Comparing `antspymm-1.3.1/docs/bids_cohort_example.py` & `antspymm-1.3.3/docs/bids_cohort_example.py`

 * *Files identical despite different names*

### Comparing `antspymm-1.3.1/docs/blind_qc.Rmd` & `antspymm-1.3.3/docs/blind_qc.Rmd`

 * *Files identical despite different names*

### Comparing `antspymm-1.3.1/docs/blind_qc.html` & `antspymm-1.3.3/docs/blind_qc.html`

 * *Files identical despite different names*

### Comparing `antspymm-1.3.1/docs/convert_adni_dti_to_nrg.R` & `antspymm-1.3.3/docs/convert_adni_dti_to_nrg.R`

 * *Files identical despite different names*

### Comparing `antspymm-1.3.1/docs/deepnbm.jpg` & `antspymm-1.3.3/docs/deepnbm.jpg`

 * *Files identical despite different names*

### Comparing `antspymm-1.3.1/docs/example_antspymm_output.csv` & `antspymm-1.3.3/docs/example_antspymm_output.csv`

 * *Files identical despite different names*

### Comparing `antspymm-1.3.1/docs/example_run_from_directory.py` & `antspymm-1.3.3/docs/example_run_from_directory.py`

 * *Files identical despite different names*

### Comparing `antspymm-1.3.1/docs/make_dict_table.Rmd` & `antspymm-1.3.3/docs/make_dict_table.Rmd`

 * *Files identical despite different names*

### Comparing `antspymm-1.3.1/docs/make_dict_table.html` & `antspymm-1.3.3/docs/make_dict_table.html`

 * *Files identical despite different names*

### Comparing `antspymm-1.3.1/docs/nrg_cohort_example.py` & `antspymm-1.3.3/docs/nrg_cohort_example.py`

 * *Files identical despite different names*

### Comparing `antspymm-1.3.1/docs/outlierness.py` & `antspymm-1.3.3/docs/outlierness.py`

 * *Files identical despite different names*

### Comparing `antspymm-1.3.1/docs/ptbp_nrg.py` & `antspymm-1.3.3/docs/ptbp_nrg.py`

 * *Files identical despite different names*

### Comparing `antspymm-1.3.1/docs/roi_visualization.py` & `antspymm-1.3.3/docs/roi_visualization.py`

 * *Files identical despite different names*

### Comparing `antspymm-1.3.1/docs/roi_visualization_ppmi.py` & `antspymm-1.3.3/docs/roi_visualization_ppmi.py`

 * *Files identical despite different names*

### Comparing `antspymm-1.3.1/docs/ukbb_to_nrg_processing.py` & `antspymm-1.3.3/docs/ukbb_to_nrg_processing.py`

 * *Files identical despite different names*

### Comparing `antspymm-1.3.1/docs/ukbb_to_nrg_processing2.py` & `antspymm-1.3.3/docs/ukbb_to_nrg_processing2.py`

 * *Files identical despite different names*

### Comparing `antspymm-1.3.1/setup.py` & `antspymm-1.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
       "dipy",
       "nibabel",
       "scipy",
       "siq",
       "scikit-learn"]
 
 setup(name='antspymm',
-      version='1.3.1',
+      version='1.3.3',
       description='multi-channel/time-series medical image processing with antspyx',
       long_description=long_description,
       long_description_content_type="text/markdown; charset=UTF-8; variant=GFM",
       url='https://github.com/stnava/ANTsPyMM',
       author='Avants, Gosselin, Tustison, Reardon',
       author_email='stnava@gmail.com',
       license='Apache 2.0',
```

### Comparing `antspymm-1.3.1/tests/blind_qc.py` & `antspymm-1.3.3/tests/blind_qc.py`

 * *Files identical despite different names*

### Comparing `antspymm-1.3.1/tests/mm.py` & `antspymm-1.3.3/tests/mm.py`

 * *Files identical despite different names*

### Comparing `antspymm-1.3.1/tests/mm_nrg.py` & `antspymm-1.3.3/tests/mm_nrg.py`

 * *Files identical despite different names*

### Comparing `antspymm-1.3.1/tests/outlierness.py` & `antspymm-1.3.3/tests/outlierness.py`

 * *Files identical despite different names*

### Comparing `antspymm-1.3.1/tests/parallel_study_aggregation_example.py` & `antspymm-1.3.3/tests/parallel_study_aggregation_example.py`

 * *Files identical despite different names*

### Comparing `antspymm-1.3.1/tests/test_deformation_gradient_reo.py` & `antspymm-1.3.3/tests/test_deformation_gradient_reo.py`

 * *Files identical despite different names*

### Comparing `antspymm-1.3.1/tests/test_dti_reg.py` & `antspymm-1.3.3/tests/test_dti_reg.py`

 * *Files identical despite different names*

### Comparing `antspymm-1.3.1/tests/test_dwi_rebasing.py` & `antspymm-1.3.3/tests/test_dwi_rebasing.py`

 * *Files identical despite different names*

### Comparing `antspymm-1.3.1/tests/test_dwi_run.py` & `antspymm-1.3.3/tests/test_dwi_run.py`

 * *Files identical despite different names*

### Comparing `antspymm-1.3.1/tests/test_dwi_run_ptbp_scrub.py` & `antspymm-1.3.3/tests/test_dwi_run_ptbp_scrub.py`

 * *Files identical despite different names*

### Comparing `antspymm-1.3.1/tests/test_joint_dti_recon.py` & `antspymm-1.3.3/tests/test_joint_dti_recon.py`

 * *Files identical despite different names*

### Comparing `antspymm-1.3.1/tests/test_mm_csv.py` & `antspymm-1.3.3/tests/test_mm_csv.py`

 * *Files identical despite different names*

### Comparing `antspymm-1.3.1/tests/test_nrg_validation.py` & `antspymm-1.3.3/tests/test_nrg_validation.py`

 * *Files identical despite different names*

### Comparing `antspymm-1.3.1/tests/test_perfusion_ptbp.py` & `antspymm-1.3.3/tests/test_perfusion_ptbp.py`

 * *Files identical despite different names*

### Comparing `antspymm-1.3.1/tests/test_perfusion_run.py` & `antspymm-1.3.3/tests/test_perfusion_run.py`

 * *Files identical despite different names*

### Comparing `antspymm-1.3.1/tests/test_rsfmri_run.py` & `antspymm-1.3.3/tests/test_rsfmri_run.py`

 * *Files identical despite different names*

### Comparing `antspymm-1.3.1/tests/test_rsfmri_run_minimal.py` & `antspymm-1.3.3/tests/test_rsfmri_run_minimal.py`

 * *Files identical despite different names*

### Comparing `antspymm-1.3.1/tests/test_ukbb_rsfmri.py` & `antspymm-1.3.3/tests/test_ukbb_rsfmri.py`

 * *Files identical despite different names*

### Comparing `antspymm-1.3.1/tests/testsr.py` & `antspymm-1.3.3/tests/testsr.py`

 * *Files identical despite different names*

### Comparing `antspymm-1.3.1/tests/visualize_tractogram.py` & `antspymm-1.3.3/tests/visualize_tractogram.py`

 * *Files identical despite different names*

