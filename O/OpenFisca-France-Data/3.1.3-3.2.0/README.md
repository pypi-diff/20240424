# Comparing `tmp/openfisca_france_data-3.1.3.tar.gz` & `tmp/openfisca_france_data-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openfisca_france_data-3.1.3.tar", last modified: Tue Apr 16 14:44:17 2024, max compression
+gzip compressed data, was "openfisca_france_data-3.2.0.tar", last modified: Wed Apr 24 16:18:12 2024, max compression
```

## Comparing `openfisca_france_data-3.1.3.tar` & `openfisca_france_data-3.2.0.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:44:17.383345 openfisca_france_data-3.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    15241 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    34519 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:44:17.379345 openfisca_france_data-3.1.3/OpenFisca_France_Data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12351 2024-04-16 14:44:17.000000 openfisca_france_data-3.1.3/OpenFisca_France_Data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-04-16 14:44:17.000000 openfisca_france_data-3.1.3/OpenFisca_France_Data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 14:44:17.000000 openfisca_france_data-3.1.3/OpenFisca_France_Data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-16 14:44:17.000000 openfisca_france_data-3.1.3/OpenFisca_France_Data.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-16 14:44:17.000000 openfisca_france_data-3.1.3/OpenFisca_France_Data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-16 14:44:17.000000 openfisca_france_data-3.1.3/OpenFisca_France_Data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12351 2024-04-16 14:44:17.383345 openfisca_france_data-3.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10702 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:44:17.367345 openfisca_france_data-3.1.3/openfisca_france_data/
--rw-r--r--   0 runner    (1001) docker     (127)     7936 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6005 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/aggregates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:44:17.367345 openfisca_france_data-3.1.3/openfisca_france_data/assets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/assets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:44:17.363345 openfisca_france_data-3.1.3/openfisca_france_data/assets/aggregats/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:44:17.367345 openfisca_france_data-3.1.3/openfisca_france_data/assets/aggregats/france_entiere/
--rw-r--r--   0 runner    (1001) docker     (127)     9989 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2019.json
--rw-r--r--   0 runner    (1001) docker     (127)    10514 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2020.json
--rw-r--r--   0 runner    (1001) docker     (127)     9998 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2021.json
--rw-r--r--   0 runner    (1001) docker     (127)     9346 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2022.json
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2023.json
--rw-r--r--   0 runner    (1001) docker     (127)     4722 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_template.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:44:17.367345 openfisca_france_data-3.1.3/openfisca_france_data/assets/aggregats/ines/
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/assets/aggregats/ines/ines_2019.json
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/assets/aggregats/ines/ines_2020.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:44:17.367345 openfisca_france_data-3.1.3/openfisca_france_data/assets/aggregats/taxipp/
--rw-r--r--   0 runner    (1001) docker     (127)    12991 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/assets/aggregats/taxipp/agregats_tests_taxipp_2_0.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:44:17.367345 openfisca_france_data-3.1.3/openfisca_france_data/assets/zone_apl_data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/assets/zone_apl_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/assets/zone_apl_data/codeAplReader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:44:17.367345 openfisca_france_data-3.1.3/openfisca_france_data/assets/zone_apl_data/zone_apl/
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/assets/zone_apl_data/zone_apl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/assets/zone_apl_data/zone_apl/zone_apl_imputation_data_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/base_survey.py
--rw-r--r--   0 runner    (1001) docker     (127)    21046 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    24951 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/comparator.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:44:17.363345 openfisca_france_data-3.1.3/openfisca_france_data/dads/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:44:17.371345 openfisca_france_data-3.1.3/openfisca_france_data/dads/input_data_builder/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/dads/input_data_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/dads/input_data_builder/create_variables_individuelles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:44:17.371345 openfisca_france_data-3.1.3/openfisca_france_data/erfs/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/erfs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:44:17.371345 openfisca_france_data-3.1.3/openfisca_france_data/erfs/input_data_builder/
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/erfs/input_data_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/erfs/input_data_builder/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/erfs/input_data_builder/run_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/erfs/input_data_builder/step_01_pre_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    21783 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/erfs/input_data_builder/step_02_imputation_loyer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11919 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/erfs/input_data_builder/step_03_fip.py
--rw-r--r--   0 runner    (1001) docker     (127)    26165 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/erfs/input_data_builder/step_04_famille.py
--rw-r--r--   0 runner    (1001) docker     (127)    13995 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/erfs/input_data_builder/step_05_foyer.py
--rw-r--r--   0 runner    (1001) docker     (127)    36615 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/erfs/input_data_builder/step_06_rebuild.py
--rw-r--r--   0 runner    (1001) docker     (127)     8399 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/erfs/input_data_builder/step_07_invalides.py
--rw-r--r--   0 runner    (1001) docker     (127)    13155 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/erfs/input_data_builder/step_08_final.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/erfs/input_data_builder/step_10_check_final2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:44:17.371345 openfisca_france_data-3.1.3/openfisca_france_data/erfs/old/
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/erfs/old/aggregates.py
--rw-r--r--   0 runner    (1001) docker     (127)    19168 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/erfs/old/datatable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/erfs/scenario.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:44:17.371345 openfisca_france_data-3.1.3/openfisca_france_data/erfs_fpr/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/erfs_fpr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/erfs_fpr/comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     7324 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/erfs_fpr/get_survey_scenario.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:44:17.375345 openfisca_france_data-3.1.3/openfisca_france_data/erfs_fpr/input_data_builder/
--rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/erfs_fpr/input_data_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15394 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/erfs_fpr/input_data_builder/step_01_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    25444 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/erfs_fpr/input_data_builder/step_02_imputation_loyer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/erfs_fpr/input_data_builder/step_02_menage.py
--rw-r--r--   0 runner    (1001) docker     (127)    45059 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/erfs_fpr/input_data_builder/step_03_variables_individuelles.py
--rw-r--r--   0 runner    (1001) docker     (127)    35145 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/erfs_fpr/input_data_builder/step_04_famille.py
--rw-r--r--   0 runner    (1001) docker     (127)    10755 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/erfs_fpr/input_data_builder/step_06_final.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/erfs_fpr/scenario.py
--rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/erfs_fpr/test_case_creation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:44:17.363345 openfisca_france_data-3.1.3/openfisca_france_data/felin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:44:17.375345 openfisca_france_data-3.1.3/openfisca_france_data/felin/input_data_builder/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/felin/input_data_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/felin/input_data_builder/create_variables_individuelles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:44:17.375345 openfisca_france_data-3.1.3/openfisca_france_data/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/model/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8882 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/model/calage.py
--rw-r--r--   0 runner    (1001) docker     (127)    12121 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/model/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/model/id_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/model/survey_variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:44:17.375345 openfisca_france_data-3.1.3/openfisca_france_data/reforms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/reforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12440 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/reforms/inversion_directe_salaires.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:44:17.375345 openfisca_france_data-3.1.3/openfisca_france_data/reforms/old_openfisca_france_reforms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/reforms/old_openfisca_france_reforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/reforms/old_openfisca_france_reforms/allocations_familiales_imposables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/reforms/old_openfisca_france_reforms/cesthra_invalidee.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/reforms/old_openfisca_france_reforms/de_net_a_brut.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:44:17.375345 openfisca_france_data-3.1.3/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/allocations_familiales_imposables.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/cesthra_invalidite.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/landais_piketty_saez.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/plf2015.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/plf2016.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/plfr2014.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/plfrss2014.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/trannoy_wasmer.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/reforms/old_openfisca_france_reforms/plf2015.py
--rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/reforms/old_openfisca_france_reforms/plf2016_ayrault_muet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/reforms/old_openfisca_france_reforms/plfr2014.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/reforms/old_openfisca_france_reforms/trannoy_wasmer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:44:17.375345 openfisca_france_data-3.1.3/openfisca_france_data/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/scripts/build_input_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6701 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/smic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7140 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/surveys.py
--rw-r--r--   0 runner    (1001) docker     (127)    15051 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/openfisca_france_data/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-16 14:44:17.383345 openfisca_france_data-3.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:44:17.379345 openfisca_france_data-3.1.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:44:17.363345 openfisca_france_data-3.1.3/tests/erfs_fpr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:44:17.379345 openfisca_france_data-3.1.3/tests/erfs_fpr/integration/
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/tests/erfs_fpr/integration/test_af.py
--rw-r--r--   0 runner    (1001) docker     (127)     8730 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/tests/erfs_fpr/integration/test_aggregates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/tests/erfs_fpr/integration/test_al.py
--rw-r--r--   0 runner    (1001) docker     (127)    10685 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/tests/erfs_fpr/integration/test_create_salaire_de_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/tests/erfs_fpr/integration/test_impot_revenu.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/tests/erfs_fpr/integration/test_inflation.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/tests/erfs_fpr/integration/test_input_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/tests/erfs_fpr/integration/test_pivot_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/tests/erfs_fpr/integration/test_rebuild_input_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/tests/erfs_fpr/integration/test_rsa.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/tests/erfs_fpr/integration/test_salaire_imposable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:44:17.379345 openfisca_france_data-3.1.3/tests/erfs_fpr/unit/
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/tests/erfs_fpr/unit/test_get_survey_scenario.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/tests/erfs_fpr/unit/test_scenario.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/tests/test_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/tests/test_calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)     7910 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/tests/test_fake_survey_simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/tests/test_get_baremes_salarie.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-16 14:44:02.000000 openfisca_france_data-3.1.3/tests/test_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.585731 openfisca_france_data-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    15626 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    34519 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.581731 openfisca_france_data-3.2.0/OpenFisca_France_Data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12351 2024-04-24 16:18:12.000000 openfisca_france_data-3.2.0/OpenFisca_France_Data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-04-24 16:18:12.000000 openfisca_france_data-3.2.0/OpenFisca_France_Data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 16:18:12.000000 openfisca_france_data-3.2.0/OpenFisca_France_Data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-24 16:18:12.000000 openfisca_france_data-3.2.0/OpenFisca_France_Data.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-24 16:18:12.000000 openfisca_france_data-3.2.0/OpenFisca_France_Data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-24 16:18:12.000000 openfisca_france_data-3.2.0/OpenFisca_France_Data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12351 2024-04-24 16:18:12.585731 openfisca_france_data-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10702 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.569731 openfisca_france_data-3.2.0/openfisca_france_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     7936 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6005 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/aggregates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.569731 openfisca_france_data-3.2.0/openfisca_france_data/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/assets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.561731 openfisca_france_data-3.2.0/openfisca_france_data/assets/aggregats/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.569731 openfisca_france_data-3.2.0/openfisca_france_data/assets/aggregats/france_entiere/
+-rw-r--r--   0 runner    (1001) docker     (127)     9989 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2019.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10514 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2020.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9998 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2021.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9346 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2022.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2023.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4722 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_template.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.569731 openfisca_france_data-3.2.0/openfisca_france_data/assets/aggregats/ines/
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/assets/aggregats/ines/ines_2019.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/assets/aggregats/ines/ines_2020.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.569731 openfisca_france_data-3.2.0/openfisca_france_data/assets/aggregats/taxipp/
+-rw-r--r--   0 runner    (1001) docker     (127)    12991 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/assets/aggregats/taxipp/agregats_tests_taxipp_2_0.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.569731 openfisca_france_data-3.2.0/openfisca_france_data/assets/zone_apl_data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/assets/zone_apl_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/assets/zone_apl_data/codeAplReader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.569731 openfisca_france_data-3.2.0/openfisca_france_data/assets/zone_apl_data/zone_apl/
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/assets/zone_apl_data/zone_apl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/assets/zone_apl_data/zone_apl/zone_apl_imputation_data_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/base_survey.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21046 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24951 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/comparator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.561731 openfisca_france_data-3.2.0/openfisca_france_data/dads/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.569731 openfisca_france_data-3.2.0/openfisca_france_data/dads/input_data_builder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/dads/input_data_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/dads/input_data_builder/create_variables_individuelles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.569731 openfisca_france_data-3.2.0/openfisca_france_data/erfs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.573731 openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/run_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/step_01_pre_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21783 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/step_02_imputation_loyer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11919 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/step_03_fip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26165 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/step_04_famille.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13995 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/step_05_foyer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36615 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/step_06_rebuild.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8399 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/step_07_invalides.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13155 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/step_08_final.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/step_10_check_final2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.573731 openfisca_france_data-3.2.0/openfisca_france_data/erfs/old/
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs/old/aggregates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19168 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs/old/datatable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs/scenario.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.573731 openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7324 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/get_survey_scenario.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.573731 openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/input_data_builder/
+-rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/input_data_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15394 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_01_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25444 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_02_imputation_loyer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_02_menage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51170 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_03_variables_individuelles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35145 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_04_famille.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10755 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_06_final.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/test_case_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.561731 openfisca_france_data-3.2.0/openfisca_france_data/felin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.577731 openfisca_france_data-3.2.0/openfisca_france_data/felin/input_data_builder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/felin/input_data_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/felin/input_data_builder/create_variables_individuelles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.577731 openfisca_france_data-3.2.0/openfisca_france_data/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8882 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/model/calage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12121 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/model/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/model/id_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/model/survey_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.577731 openfisca_france_data-3.2.0/openfisca_france_data/reforms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/reforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12440 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/reforms/inversion_directe_salaires.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.577731 openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/allocations_familiales_imposables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/cesthra_invalidee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/de_net_a_brut.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.577731 openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/allocations_familiales_imposables.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/cesthra_invalidite.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/landais_piketty_saez.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/plf2015.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/plf2016.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/plfr2014.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/plfrss2014.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/trannoy_wasmer.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/plf2015.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/plf2016_ayrault_muet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/plfr2014.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/trannoy_wasmer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.581731 openfisca_france_data-3.2.0/openfisca_france_data/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/scripts/build_input_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6701 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/smic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7140 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/surveys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15051 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-24 16:18:12.585731 openfisca_france_data-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.581731 openfisca_france_data-3.2.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.565731 openfisca_france_data-3.2.0/tests/erfs_fpr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.581731 openfisca_france_data-3.2.0/tests/erfs_fpr/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/tests/erfs_fpr/integration/test_af.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8730 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/tests/erfs_fpr/integration/test_aggregates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/tests/erfs_fpr/integration/test_al.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10685 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/tests/erfs_fpr/integration/test_create_salaire_de_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/tests/erfs_fpr/integration/test_impot_revenu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/tests/erfs_fpr/integration/test_inflation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/tests/erfs_fpr/integration/test_input_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/tests/erfs_fpr/integration/test_pivot_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/tests/erfs_fpr/integration/test_rebuild_input_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/tests/erfs_fpr/integration/test_rsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/tests/erfs_fpr/integration/test_salaire_imposable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.581731 openfisca_france_data-3.2.0/tests/erfs_fpr/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/tests/erfs_fpr/unit/test_get_survey_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/tests/erfs_fpr/unit/test_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/tests/test_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/tests/test_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7910 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/tests/test_fake_survey_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/tests/test_get_baremes_salarie.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/tests/test_misc.py
```

### Comparing `openfisca_france_data-3.1.3/CHANGELOG.md` & `openfisca_france_data-3.2.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Changelog
 
+### 3.2.0 [#255](https://github.com/openfisca/openfisca-france-data/pull/255)
+
+* New features
+  - Améliore la construction des variables `contrat_de_travail` et `heures_remunerees_volumes` avec l'erfs_fpr
+    - Utilisations des variables `sp00` à `sp12` qui décrivent le statut d'activité sur les douze derniers mois pour prendre en compte la part de travail connue dans l'année
+
 ### 3.1.3 [#254](https://github.com/openfisca/openfisca-france-data/pull/254)
 
 * Technical changes
   - Met à jour la version d'openfisca france dans les dépendances
 
 ### 3.1.2 [#250](https://github.com/openfisca/openfisca-france-data/pull/250)
```

### Comparing `openfisca_france_data-3.1.3/CONTRIBUTING.md` & `openfisca_france_data-3.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/LICENSE` & `openfisca_france_data-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/OpenFisca_France_Data.egg-info/PKG-INFO` & `openfisca_france_data-3.2.0/OpenFisca_France_Data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenFisca-France-Data
-Version: 3.1.3
+Version: 3.2.0
 Summary: OpenFisca-France-Data module to work with French survey data
 Home-page: https://github.com/openfisca/openfisca-france-data
 Author: OpenFisca Team
 Author-email: contact@openfisca.fr
 License: http://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: tax benefit social survey data microsimulation
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `openfisca_france_data-3.1.3/OpenFisca_France_Data.egg-info/SOURCES.txt` & `openfisca_france_data-3.2.0/OpenFisca_France_Data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/PKG-INFO` & `openfisca_france_data-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenFisca-France-Data
-Version: 3.1.3
+Version: 3.2.0
 Summary: OpenFisca-France-Data module to work with French survey data
 Home-page: https://github.com/openfisca/openfisca-france-data
 Author: OpenFisca Team
 Author-email: contact@openfisca.fr
 License: http://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: tax benefit social survey data microsimulation
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `openfisca_france_data-3.1.3/README.md` & `openfisca_france_data-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/__init__.py` & `openfisca_france_data-3.2.0/openfisca_france_data/__init__.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/aggregates.py` & `openfisca_france_data-3.2.0/openfisca_france_data/aggregates.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2019.json` & `openfisca_france_data-3.2.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2019.json`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2020.json` & `openfisca_france_data-3.2.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2020.json`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2021.json` & `openfisca_france_data-3.2.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2021.json`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2022.json` & `openfisca_france_data-3.2.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2022.json`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2023.json` & `openfisca_france_data-3.2.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2023.json`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_template.json` & `openfisca_france_data-3.2.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_template.json`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/assets/aggregats/ines/ines_2019.json` & `openfisca_france_data-3.2.0/openfisca_france_data/assets/aggregats/ines/ines_2019.json`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/assets/aggregats/ines/ines_2020.json` & `openfisca_france_data-3.2.0/openfisca_france_data/assets/aggregats/ines/ines_2020.json`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/assets/aggregats/taxipp/agregats_tests_taxipp_2_0.xlsx` & `openfisca_france_data-3.2.0/openfisca_france_data/assets/aggregats/taxipp/agregats_tests_taxipp_2_0.xlsx`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/assets/zone_apl_data/zone_apl/zone_apl_imputation_data_reader.py` & `openfisca_france_data-3.2.0/openfisca_france_data/assets/zone_apl_data/zone_apl/zone_apl_imputation_data_reader.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/base_survey.py` & `openfisca_france_data-3.2.0/openfisca_france_data/base_survey.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/common.py` & `openfisca_france_data-3.2.0/openfisca_france_data/common.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/comparator.py` & `openfisca_france_data-3.2.0/openfisca_france_data/comparator.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/config.py` & `openfisca_france_data-3.2.0/openfisca_france_data/config.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/dads/input_data_builder/create_variables_individuelles.py` & `openfisca_france_data-3.2.0/openfisca_france_data/dads/input_data_builder/create_variables_individuelles.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/erfs/__init__.py` & `openfisca_france_data-3.2.0/openfisca_france_data/erfs/__init__.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/erfs/input_data_builder/__init__.py` & `openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/erfs/input_data_builder/base.py` & `openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/base.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/erfs/input_data_builder/run_all.py` & `openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/run_all.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/erfs/input_data_builder/step_01_pre_processing.py` & `openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/step_01_pre_processing.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/erfs/input_data_builder/step_02_imputation_loyer.py` & `openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/step_02_imputation_loyer.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/erfs/input_data_builder/step_03_fip.py` & `openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/step_03_fip.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/erfs/input_data_builder/step_04_famille.py` & `openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/step_04_famille.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/erfs/input_data_builder/step_05_foyer.py` & `openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/step_05_foyer.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/erfs/input_data_builder/step_06_rebuild.py` & `openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/step_06_rebuild.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/erfs/input_data_builder/step_07_invalides.py` & `openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/step_07_invalides.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/erfs/input_data_builder/step_08_final.py` & `openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/step_08_final.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/erfs/input_data_builder/step_10_check_final2.py` & `openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/step_10_check_final2.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/erfs/old/aggregates.py` & `openfisca_france_data-3.2.0/openfisca_france_data/erfs/old/aggregates.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/erfs/old/datatable.py` & `openfisca_france_data-3.2.0/openfisca_france_data/erfs/old/datatable.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/erfs/scenario.py` & `openfisca_france_data-3.2.0/openfisca_france_data/erfs/scenario.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/erfs_fpr/comparison.py` & `openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/comparison.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/erfs_fpr/get_survey_scenario.py` & `openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/get_survey_scenario.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/erfs_fpr/input_data_builder/__init__.py` & `openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/input_data_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/erfs_fpr/input_data_builder/step_01_preprocessing.py` & `openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_01_preprocessing.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/erfs_fpr/input_data_builder/step_02_imputation_loyer.py` & `openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_02_imputation_loyer.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/erfs_fpr/input_data_builder/step_02_menage.py` & `openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_02_menage.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/erfs_fpr/input_data_builder/step_03_variables_individuelles.py` & `openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_03_variables_individuelles.py`

 * *Files 11% similar despite different names*

```diff
@@ -503,15 +503,15 @@
         'categorie_non_salarie'
         ] = 3
     #fix un peu crade : cstot ne semble pas recouvrir tout le champ des personnes qui ont du rpns
     # on met par défaut ces gens là en chef d'entreprise
     individus.loc[
         ((individus['rpns_imposables'] != 0) & (individus['categorie_non_salarie'] == 0)),
         'categorie_non_salarie'
-        ] = 2  
+        ] = 2
 
 
 def create_contrat_de_travail(individus, period, salaire_type = 'imposable'):
     """Création de la variable contrat_de_travail et heure_remunerees_volume.
 
     Ses modliatés sont:
         0 - temps_plein
@@ -575,14 +575,37 @@
         log.debug('Salaire retenu: {}'.format('salaire_imposable'))
         individus['salaire'] = individus.salaire_imposable.copy()
         smic = smic_annuel_imposable_by_year[period.start.year]
 
     if period.unit == 'month':
         smic = period.size * smic / 12
 
+    # Etape préliminaire : construction d'une variable pour avoir une estimation de la part de l'année connue en emploi.
+    # l'idée est d'utiliser les variables sp00-sp12 qui décrivent la situation principale pour chaque mois, du mois de l'enquête (sp00) à 12 mois en arrièvre (sp12).
+    # Cela permet de compenser le fait que sinon on ne regarde la situation de l'emploi que pour la semaine de référence alors qu'on a des revenus annuels.
+
+    # d abord on recupere le mois de l'enquete
+    individus['mois_enquete'] = [int(str(i)[4:6]) for i in individus.datdeb]
+    assert (individus.mois_enquete.isin(range(9, 13))).all()
+
+    # # on ne prend que les mois de l'année en cours donc on n'a pas le même nombre de mois connus selon le mois de l'enquête
+
+    individus['nb_mois_salariat_annee'] = 0
+    for i in ["00", "01", "02", "03", "04", "05", "06", "07", "08", "09", "10", "11"]:
+        individus['nb_mois_salariat_annee'] = individus.nb_mois_salariat_annee + np.where(int(i) < individus['mois_enquete'], np.where((individus[f"sp{i}"] == 1), 1, 0), 0)
+        individus['nb_mois_salariat_annee'] = individus.nb_mois_salariat_annee + np.where(int(i) < individus['mois_enquete'], np.where((individus[f"sp{i}"] == 2), 1, 0), 0)
+
+    # # normalement sp == 2 c'est de l'emploi non salarié mais possible que ce soit des statuts micro ou autre imposé dans assimilé salaire donc qu'on voit en salaire
+    # # si sp est nan un mois donnée, le mois est considéré comme non travaillé
+
+    individus['part_salariat_annee_connue'] = individus['nb_mois_salariat_annee'] / individus['mois_enquete']
+    individus['part_salariat_annee_connue'] = np.where(individus['part_salariat_annee_connue'] == 0, 1, individus['part_salariat_annee_connue'])
+    # s'il n'y a aucun mois travaillé dans l'année on met à 1 comme ça on ne l'utilise pas
+
+
     # 0 On élimine les individus avec un salaire_net nul des salariés
     # 1. utilisation de tppred et durhab
     # 1.1  temps_plein
     individus.query('tppred == 1').duhab.value_counts(dropna = False)
     assert (individus.query('tppred == 1').duhab >= 4).all()
     individus.loc[
         (individus.salaire > 0) & (
@@ -595,152 +618,214 @@
     assert (individus.query('tppred == 2').duhab.isin([1, 2, 3, 9])).all()
     individus.loc[
         (individus.salaire > 0) & (
             (individus.tppred == 2) | (individus.duhab.isin(range(1, 4)))
             ),
         'contrat_de_travail'
         ] = 1
+
+    # on met à temps partiel les personnes qui se déclarent en temps plein au moment de l'enquète mais qui ont des périodes d'inactivité dans l'année
+    passage_temps_plein_temps_partiel = (
+        (individus.contrat_de_travail == 0) &
+        (individus.salaire > 0) &
+        (individus.part_salariat_annee_connue < 1)
+    )
+    individus.loc[passage_temps_plein_temps_partiel, 'contrat_de_travail'] = 1
     assert (individus.query('salaire == 0').contrat_de_travail == 6).all()
+    assert (individus.query('contrat_de_travail == 0').part_salariat_annee_connue == 1).all()
     # 2. On traite les salaires horaires inféreurs au SMIC
     # 2.1 temps plein
     temps_plein = individus.query('(contrat_de_travail == 0) & (salaire > 0)')
     # (temps_plein.salaire > smic).value_counts()
     # temps_plein.query('salaire < 15000').salaire.hist()
     individus['heures_remunerees_volume'] = 0
     # On bascule à temps partiel et on réajuste les heures des temps plein qui ne touche pas le smic
     temps_plein_sous_smic = (
         (individus.contrat_de_travail == 0) &
         (individus.salaire > 0) &
         (individus.salaire < smic)
         )
+
+    assert (individus.loc[temps_plein_sous_smic].part_salariat_annee_connue == 1).all()
+    # il n'y a bien que des individus qu'on a pas pu mettre à temps partiel du fait de la part salariat dans l'année connue
+
     individus.loc[
         temps_plein_sous_smic,
         'contrat_de_travail'] = 1
     individus.loc[
         temps_plein_sous_smic,
         'heures_remunerees_volume'] = individus.loc[
             temps_plein_sous_smic,
             'salaire'
             ] / smic * 35
     assert (individus.loc[temps_plein_sous_smic, 'heures_remunerees_volume'] < 35).all()
     assert (individus.loc[temps_plein_sous_smic, 'heures_remunerees_volume'] > 0).all()
     assert (individus.query('salaire == 0').contrat_de_travail == 6).all()
     del temps_plein, temps_plein_sous_smic
+
     # 2.2 Pour les temps partiel on prends les heures hhc
+    individus.loc[(individus.hhc > 35) & (individus.hhc.notnull()) & (individus.contrat_de_travail == 1),'hhc'] = 35
+    individus.loc[(passage_temps_plein_temps_partiel) & (individus.hhc.isnull()), 'hhc'] = 35
+    del passage_temps_plein_temps_partiel
+    # on met 35h aux individus qui étaient à temps plein et qu'on a basculé en temps partiel pour la part salarié dans l'année
+
     # On vérfie que celles qu'on a créées jusqu'ici sont correctes
     assert (individus.query('salaire == 0').contrat_de_travail == 6).all()
     assert (individus.query('(contrat_de_travail == 1) & (salaire > 0)').heures_remunerees_volume < 35).all()
-    #
+
     axes = (individus.query('(contrat_de_travail == 1) & (salaire > 0)').hhc).hist(bins=100)
     axes.set_title("Heures (hhc)")
     # individus.query('(contrat_de_travail == 1) & (salaire > 0)').hhc.isnull().sum() = 489
     # 2.2.1 On abaisse le nombre d'heures pour que les gens touchent au moins le smic horaire
     temps_partiel = (individus.contrat_de_travail == 1) & (individus.salaire > 0)
     moins_que_smic_horaire_hhc = (
-        ((individus.salaire / individus.hhc) < (smic / 35)) &
-        individus.hhc.notnull()
+        ((individus.salaire / (individus.hhc * individus.part_salariat_annee_connue)) < (smic / 35)) # on adapte le nombre d'heure en fonction de la part travaillée observée dans l'année
         )
+    hhc_positif = (individus.hhc.notnull() & (individus.hhc > 0))
     # Si on dispose de la variable hhc on l'utilise
+    # Si moins que le SMIC on met au SMIC
     individus.loc[
-        temps_partiel & moins_que_smic_horaire_hhc,
+        temps_partiel & moins_que_smic_horaire_hhc & hhc_positif,
         'heures_remunerees_volume'
         ] = individus.loc[
-            temps_partiel & moins_que_smic_horaire_hhc,
+            temps_partiel & moins_que_smic_horaire_hhc & hhc_positif,
             'salaire'
             ] / smic * 35
+    # Sinon on met le nombre d'heures renseignées au proratat du temps de travail dans l'année
     individus.loc[
-        temps_partiel & (~moins_que_smic_horaire_hhc) & individus.hhc.notnull(),
+        temps_partiel & (~moins_que_smic_horaire_hhc) & hhc_positif,
         'heures_remunerees_volume'
         ] = individus.loc[
-            temps_partiel & (~moins_que_smic_horaire_hhc) & individus.hhc.notnull(),
+            temps_partiel & (~moins_que_smic_horaire_hhc) & hhc_positif,
             'hhc'
-            ]
+            ] * individus.loc[
+            temps_partiel & (~moins_que_smic_horaire_hhc) & hhc_positif,
+            'part_salariat_annee_connue'
+            ] # on adapte le nombre d'heure en fonction de la part travaillée observée dans l'année
+
+    assert (individus.loc[temps_partiel & moins_que_smic_horaire_hhc & hhc_positif, 'heures_remunerees_volume'] < 35).all()
+    assert (individus.loc[temps_partiel & moins_que_smic_horaire_hhc & hhc_positif, 'heures_remunerees_volume'] > 0).all()
+    assert (individus.loc[temps_partiel & (~moins_que_smic_horaire_hhc) & hhc_positif, 'heures_remunerees_volume'] <= 35).all()
+    assert (individus.loc[temps_partiel & (~moins_que_smic_horaire_hhc) & hhc_positif, 'heures_remunerees_volume'] > 0).all()
+
+    individus.loc[temps_partiel & (~moins_que_smic_horaire_hhc) & hhc_positif & (individus.heures_remunerees_volume == 35),'contrat_de_travail'] = 0
+    individus.loc[temps_partiel & (~moins_que_smic_horaire_hhc) & hhc_positif & (individus.heures_remunerees_volume == 35),'heures_remunerees_volume'] = 0
+
     axes = (
         individus
         .loc[temps_partiel]
         .query('(contrat_de_travail == 1) & (salaire > 0)')
         .heures_remunerees_volume
         .hist(bins=100)
         )
     axes.set_title("Heures (heures_remunerees_volume)")
     # 2.2.2 Il reste à ajuster le nombre d'heures pour les salariés à temps partiel qui n'ont pas de hhc
     # et qui disposent de moins que le smic_horaire ou de les basculer en temps plein sinon
-    moins_que_smic_horaire_sans_hhc = (individus.salaire < smic) & individus.hhc.isnull()
+    moins_que_smic_horaire_sans_hhc = (individus.salaire < smic * (individus.part_salariat_annee_connue)) & individus.hhc.isnull()
     individus.loc[
         temps_partiel & moins_que_smic_horaire_sans_hhc,
         'heures_remunerees_volume'
         ] = individus.loc[
             temps_partiel & moins_que_smic_horaire_sans_hhc,
             'salaire'
             ] / smic * 35
-    plus_que_smic_horaire_sans_hhc = (
-        (individus.salaire >= smic) &
-        individus.hhc.isnull()
+
+    plus_que_smic_horaire_sans_hhc_temps_plein = (
+        (individus.salaire >= smic * (individus.part_salariat_annee_connue)) &
+        individus.hhc.isnull() &
+        (individus.part_salariat_annee_connue == 1)
         )
     individus.loc[
-        temps_partiel & plus_que_smic_horaire_sans_hhc,
+        temps_partiel & plus_que_smic_horaire_sans_hhc_temps_plein,
         'contrat_de_travail'
         ] = 0
     individus.loc[
-        temps_partiel & plus_que_smic_horaire_sans_hhc,
+        temps_partiel & plus_que_smic_horaire_sans_hhc_temps_plein,
         'heures_remunerees_volume'
         ] = 0
+
+    plus_que_smic_horaire_sans_hhc_temps_partiel = (
+        (individus.salaire >= smic * (individus.part_salariat_annee_connue)) &
+        individus.hhc.isnull() &
+        (individus.part_salariat_annee_connue < 1)
+        )
+    individus.loc[
+        temps_partiel & plus_que_smic_horaire_sans_hhc_temps_partiel,
+        'heures_remunerees_volume'
+        ] = 35 * individus.part_salariat_annee_connue
+
     # 2.2.3 On repasse en temps plein ceux qui ont plus de 35 heures par semaine
     temps_partiel_bascule_temps_plein = (
         temps_partiel &
         (individus.heures_remunerees_volume >= 35)
         )
     individus.loc[
         temps_partiel_bascule_temps_plein,
         'contrat_de_travail',
         ] = 0
     individus.loc[
         temps_partiel_bascule_temps_plein,
         'heures_remunerees_volume',
         ] = 0
-    del temps_partiel, temps_partiel_bascule_temps_plein, moins_que_smic_horaire_hhc, moins_que_smic_horaire_sans_hhc
+    del temps_partiel, temps_partiel_bascule_temps_plein, moins_que_smic_horaire_hhc#, moins_que_smic_horaire_sans_hhc
     assert (individus.query('contrat_de_travail == 0').heures_remunerees_volume == 0).all()
     assert (individus.query('contrat_de_travail == 1').heures_remunerees_volume < 35).all()
     assert (individus.query('salaire == 0').contrat_de_travail == 6).all()
     assert (individus.query('contrat_de_travail == 6').heures_remunerees_volume == 0).all()
     # 2.3 On traite ceux qui ont un salaire mais pas de contrat de travail renseigné
     # (temps plein ou temps complet)
     salarie_sans_contrat_de_travail = (
         (individus.salaire > 0) &
         ~individus.contrat_de_travail.isin([0, 1])
         )
-    # 2.3.1 On passe à temps plein ceux qui ont un salaire supérieur au SMIC annuel
+    # 2.3.1 On passe à temps plein ceux qui ont un salaire supérieur au SMIC annuel et qui ont travaillé toute l'année jusqu'à l'enquête
     individus.loc[
         salarie_sans_contrat_de_travail &
-        (individus.salaire >= smic),
+        (individus.salaire >= smic) &
+        (individus.part_salariat_annee_connue == 1),
         'contrat_de_travail'
         ] = 0
     assert (individus.loc[
         salarie_sans_contrat_de_travail &
         (individus.salaire >= smic),
         'heures_remunerees_volume'
         ] == 0).all()
+    # on passe à temps partiel ceux qui sont supérieur au smic mais qui ont une part travaillée inférieur à 1.
+    # On leur attribut un nombre d'heure au proratat de la durée travaillée
+    individus.loc[
+        salarie_sans_contrat_de_travail &
+        (individus.salaire >= smic * individus.part_salariat_annee_connue) &
+        (individus.part_salariat_annee_connue < 1),
+        'contrat_de_travail'
+        ] = 1
+    individus.loc[
+        salarie_sans_contrat_de_travail &
+        (individus.salaire >= smic * individus.part_salariat_annee_connue) &
+        (individus.part_salariat_annee_connue < 1),
+        'heures_remunerees_volume'
+        ] = 35 * individus.part_salariat_annee_connue
     # 2.3.2 On passe à temps partiel ceux qui ont un salaire inférieur au SMIC annuel
     individus.loc[
         salarie_sans_contrat_de_travail &
-        (individus.salaire < smic),
+        (individus.salaire < smic * individus.part_salariat_annee_connue),
         'contrat_de_travail'
         ] = 1
     individus.loc[
         salarie_sans_contrat_de_travail &
-        (individus.salaire < smic),
+        (individus.salaire < smic * individus.part_salariat_annee_connue),
         'heures_remunerees_volume'
         ] = individus.loc[
             salarie_sans_contrat_de_travail &
-            (individus.salaire < smic),
+            (individus.salaire < smic * individus.part_salariat_annee_connue),
             'salaire'
             ] / smic * 35
     # 2.3.3 On attribue des heures rémunérées aux individus à temps partiel qui ont un
     # salaire strictement positif mais un nombre d'heures travaillées nul
     salaire_sans_heures = (individus.contrat_de_travail == 1) & ~(individus.heures_remunerees_volume > 0)
+
     assert (individus.loc[salaire_sans_heures, 'salaire'] > 0).all()
     assert (individus.loc[salaire_sans_heures, 'duhab'] == 1).all()
     # Cela concerne peu de personnes qui ont par ailleurs duhab = 1 et un salaire supérieur au smic.
     # On leur attribue donc un nombre d'heures travaillées égal à 15.
     individus.loc[
         salaire_sans_heures &
         (individus.salaire > smic),
@@ -748,14 +833,15 @@
     #
     individus.query('salaire > 0').contrat_de_travail.value_counts(dropna = False)
     individus.query('salaire == 0').contrat_de_travail.value_counts(dropna = False)
 
     individus.loc[salarie_sans_contrat_de_travail, 'salaire'].min()
     individus.loc[salarie_sans_contrat_de_travail, 'salaire'].hist(bins = 1000)
     del salarie_sans_contrat_de_travail
+
     # On vérifie que l'on n'a pas fait d'erreurs
     assert (individus.salaire >= 0).all(), "Des salaires sont negatifs: {}".format(
             individus.loc[~(individus.salaire >= 0), 'salaire']
             )
     assert individus.contrat_de_travail.isin([0, 1, 6]).all()
     assert (individus.query('salaire > 0').contrat_de_travail.isin([0, 1])).all()
     assert (individus.query('salaire == 0').contrat_de_travail == 6).all()
@@ -783,14 +869,17 @@
         else:
             log.error('Wrong period {}. Should be month or year'.format(period))
             raise
     else:
         log.error('Wrong period {}. Should be month or year'.format(period))
         raise
 
+     # On arrondit les heures supplémentaires à l'entier inférieur, et mon met 1 si en dessous de 1
+    individus.loc[individus.contrat_de_travail == 1, 'heures_remunerees_volume'] = np.maximum(1,np.round(individus.loc[individus.contrat_de_travail == 1, 'heures_remunerees_volume']))
+
     del individus['salaire']
 
     return
 
 
 def create_date_naissance(individus, age_variable = 'age', annee_naissance_variable = None, mois_naissance = None,
          year = None):
```

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/erfs_fpr/input_data_builder/step_04_famille.py` & `openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_04_famille.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/erfs_fpr/input_data_builder/step_06_final.py` & `openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_06_final.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/erfs_fpr/scenario.py` & `openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/scenario.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/erfs_fpr/test_case_creation.py` & `openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/test_case_creation.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/felin/input_data_builder/create_variables_individuelles.py` & `openfisca_france_data-3.2.0/openfisca_france_data/felin/input_data_builder/create_variables_individuelles.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/model/base.py` & `openfisca_france_data-3.2.0/openfisca_france_data/model/base.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/model/calage.py` & `openfisca_france_data-3.2.0/openfisca_france_data/model/calage.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/model/common.py` & `openfisca_france_data-3.2.0/openfisca_france_data/model/common.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/model/id_variables.py` & `openfisca_france_data-3.2.0/openfisca_france_data/model/id_variables.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/model/survey_variables.py` & `openfisca_france_data-3.2.0/openfisca_france_data/model/survey_variables.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/reforms/inversion_directe_salaires.py` & `openfisca_france_data-3.2.0/openfisca_france_data/reforms/inversion_directe_salaires.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/reforms/old_openfisca_france_reforms/allocations_familiales_imposables.py` & `openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/allocations_familiales_imposables.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/reforms/old_openfisca_france_reforms/cesthra_invalidee.py` & `openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/cesthra_invalidee.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/reforms/old_openfisca_france_reforms/de_net_a_brut.py` & `openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/de_net_a_brut.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/landais_piketty_saez.yaml` & `openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/landais_piketty_saez.yaml`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/plfr2014.yaml` & `openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/plfr2014.yaml`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/plfrss2014.yaml` & `openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/plfrss2014.yaml`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/reforms/old_openfisca_france_reforms/plf2015.py` & `openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/plf2015.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/reforms/old_openfisca_france_reforms/plf2016_ayrault_muet.py` & `openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/plf2016_ayrault_muet.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/reforms/old_openfisca_france_reforms/plfr2014.py` & `openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/plfr2014.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/reforms/old_openfisca_france_reforms/trannoy_wasmer.py` & `openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/trannoy_wasmer.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/scripts/build_input_data.py` & `openfisca_france_data-3.2.0/openfisca_france_data/scripts/build_input_data.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/smic.py` & `openfisca_france_data-3.2.0/openfisca_france_data/smic.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/surveys.py` & `openfisca_france_data-3.2.0/openfisca_france_data/surveys.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/openfisca_france_data/utils.py` & `openfisca_france_data-3.2.0/openfisca_france_data/utils.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/setup.cfg` & `openfisca_france_data-3.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/setup.py` & `openfisca_france_data-3.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md') as file:
     long_description = file.read()
 
 setup(
     name = "OpenFisca-France-Data",
-    version = "3.1.3",
+    version = "3.2.0",
     description = "OpenFisca-France-Data module to work with French survey data",
     long_description = long_description,
     long_description_content_type="text/markdown",
     author = "OpenFisca Team",
     author_email = "contact@openfisca.fr",
     url = "https://github.com/openfisca/openfisca-france-data",
     license = "http://www.fsf.org/licensing/licenses/agpl-3.0.html",
```

### Comparing `openfisca_france_data-3.1.3/tests/erfs_fpr/integration/test_af.py` & `openfisca_france_data-3.2.0/tests/erfs_fpr/integration/test_af.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/tests/erfs_fpr/integration/test_aggregates.py` & `openfisca_france_data-3.2.0/tests/erfs_fpr/integration/test_aggregates.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/tests/erfs_fpr/integration/test_al.py` & `openfisca_france_data-3.2.0/tests/erfs_fpr/integration/test_al.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/tests/erfs_fpr/integration/test_create_salaire_de_base.py` & `openfisca_france_data-3.2.0/tests/erfs_fpr/integration/test_create_salaire_de_base.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/tests/erfs_fpr/integration/test_impot_revenu.py` & `openfisca_france_data-3.2.0/tests/erfs_fpr/integration/test_impot_revenu.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/tests/erfs_fpr/integration/test_inflation.py` & `openfisca_france_data-3.2.0/tests/erfs_fpr/integration/test_inflation.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/tests/erfs_fpr/integration/test_input_variables.py` & `openfisca_france_data-3.2.0/tests/erfs_fpr/integration/test_input_variables.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/tests/erfs_fpr/integration/test_pivot_table.py` & `openfisca_france_data-3.2.0/tests/erfs_fpr/integration/test_pivot_table.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/tests/erfs_fpr/integration/test_rebuild_input_data.py` & `openfisca_france_data-3.2.0/tests/erfs_fpr/integration/test_rebuild_input_data.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/tests/erfs_fpr/integration/test_rsa.py` & `openfisca_france_data-3.2.0/tests/erfs_fpr/integration/test_rsa.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/tests/erfs_fpr/integration/test_salaire_imposable.py` & `openfisca_france_data-3.2.0/tests/erfs_fpr/integration/test_salaire_imposable.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/tests/erfs_fpr/unit/test_get_survey_scenario.py` & `openfisca_france_data-3.2.0/tests/erfs_fpr/unit/test_get_survey_scenario.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/tests/test_aggregate.py` & `openfisca_france_data-3.2.0/tests/test_aggregate.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/tests/test_calibration.py` & `openfisca_france_data-3.2.0/tests/test_calibration.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/tests/test_fake_survey_simulation.py` & `openfisca_france_data-3.2.0/tests/test_fake_survey_simulation.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/tests/test_get_baremes_salarie.py` & `openfisca_france_data-3.2.0/tests/test_get_baremes_salarie.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.1.3/tests/test_misc.py` & `openfisca_france_data-3.2.0/tests/test_misc.py`

 * *Files identical despite different names*

