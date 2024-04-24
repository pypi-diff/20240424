# Comparing `tmp/OpenFisca-Survey-Manager-2.2.0.tar.gz` & `tmp/openfisca_survey_manager-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenFisca-Survey-Manager-2.2.0.tar", last modified: Tue Apr  9 14:59:17 2024, max compression
+gzip compressed data, was "openfisca_survey_manager-2.2.1.tar", last modified: Wed Apr 24 09:37:23 2024, max compression
```

## Comparing `OpenFisca-Survey-Manager-2.2.0.tar` & `openfisca_survey_manager-2.2.1.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:59:17.325349 OpenFisca-Survey-Manager-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    24130 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    34499 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/LICENSE.AGPL.txt
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:59:17.321349 OpenFisca-Survey-Manager-2.2.0/OpenFisca_Survey_Manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16709 2024-04-09 14:59:17.000000 OpenFisca-Survey-Manager-2.2.0/OpenFisca_Survey_Manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-09 14:59:17.000000 OpenFisca-Survey-Manager-2.2.0/OpenFisca_Survey_Manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:59:17.000000 OpenFisca-Survey-Manager-2.2.0/OpenFisca_Survey_Manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-09 14:59:17.000000 OpenFisca-Survey-Manager-2.2.0/OpenFisca_Survey_Manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:59:17.000000 OpenFisca-Survey-Manager-2.2.0/OpenFisca_Survey_Manager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-09 14:59:17.000000 OpenFisca-Survey-Manager-2.2.0/OpenFisca_Survey_Manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-09 14:59:17.000000 OpenFisca-Survey-Manager-2.2.0/OpenFisca_Survey_Manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16709 2024-04-09 14:59:17.321349 OpenFisca-Survey-Manager-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14209 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:59:17.313350 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18199 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/aggregates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:59:17.317350 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/assets/
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_classes.csv
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_divisions.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_groupes.csv
--rw-r--r--   0 runner    (1001) docker     (127)    12096 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_postes.csv
--rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_sous_classes.csv
--rw-r--r--   0 runner    (1001) docker     (127)    11420 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)     9710 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/calmar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/coicop.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:59:17.317350 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/config_files_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/config_files_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/config_files_templates/config_template.ini
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/config_files_templates/raw_data_template.ini
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/google_colab.py
--rw-r--r--   0 runner    (1001) docker     (127)    14200 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/input_dataframe_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/read_dbf.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/read_sas.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/read_spss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:59:17.317350 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/scenarios/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/scenarios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32942 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/scenarios/abstract_scenario.py
--rw-r--r--   0 runner    (1001) docker     (127)    10858 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/scenarios/reform_scenario.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:59:17.317350 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11374 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/scripts/build_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    11813 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/simulation_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    63511 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/simulations.py
--rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/statshelpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/survey_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)    17265 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/surveys.py
--rw-r--r--   0 runner    (1001) docker     (127)    12258 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/temporary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:59:17.317350 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:59:17.321349 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/data_files/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/data_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/data_files/config_template.ini
--rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_add_survey_to_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_aggregates.py
--rw-r--r--   0 runner    (1001) docker     (127)     5221 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_calmar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_compute_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_compute_pivot_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_compute_winners_loosers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_create_data_frame_by_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_legislation_inflator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_marginal_tax_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)    10781 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_parquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_quantile.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_read_sas.py
--rw-r--r--   0 runner    (1001) docker     (127)    16428 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_scenario.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_summarize_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_surveys.py
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_tax_benefit_system_asof.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_top_bottom_share.py
--rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_write_parquet.py
--rw-r--r--   0 runner    (1001) docker     (127)    12269 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-09 14:59:17.325349 OpenFisca-Survey-Manager-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:37:23.403802 openfisca_survey_manager-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    24438 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    34499 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/LICENSE.AGPL.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:37:23.399802 openfisca_survey_manager-2.2.1/OpenFisca_Survey_Manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16709 2024-04-24 09:37:23.000000 openfisca_survey_manager-2.2.1/OpenFisca_Survey_Manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-24 09:37:23.000000 openfisca_survey_manager-2.2.1/OpenFisca_Survey_Manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 09:37:23.000000 openfisca_survey_manager-2.2.1/OpenFisca_Survey_Manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-24 09:37:23.000000 openfisca_survey_manager-2.2.1/OpenFisca_Survey_Manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 09:37:23.000000 openfisca_survey_manager-2.2.1/OpenFisca_Survey_Manager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-24 09:37:23.000000 openfisca_survey_manager-2.2.1/OpenFisca_Survey_Manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 09:37:23.000000 openfisca_survey_manager-2.2.1/OpenFisca_Survey_Manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16709 2024-04-24 09:37:23.403802 openfisca_survey_manager-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14209 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:37:23.395802 openfisca_survey_manager-2.2.1/openfisca_survey_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18199 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/aggregates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:37:23.395802 openfisca_survey_manager-2.2.1/openfisca_survey_manager/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/assets/nomenclature_coicop_source_by_classes.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/assets/nomenclature_coicop_source_by_divisions.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/assets/nomenclature_coicop_source_by_groupes.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    12096 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/assets/nomenclature_coicop_source_by_postes.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/assets/nomenclature_coicop_source_by_sous_classes.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    11420 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9710 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/calmar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/coicop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:37:23.395802 openfisca_survey_manager-2.2.1/openfisca_survey_manager/config_files_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/config_files_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/config_files_templates/config_template.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/config_files_templates/raw_data_template.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/google_colab.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14200 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/input_dataframe_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/read_dbf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/read_sas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/read_spss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:37:23.395802 openfisca_survey_manager-2.2.1/openfisca_survey_manager/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/scenarios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32942 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/scenarios/abstract_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10858 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/scenarios/reform_scenario.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:37:23.395802 openfisca_survey_manager-2.2.1/openfisca_survey_manager/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11374 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/scripts/build_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11813 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/simulation_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63623 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/simulations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/statshelpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/survey_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17265 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/surveys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12258 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/temporary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:37:23.399802 openfisca_survey_manager-2.2.1/openfisca_survey_manager/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:37:23.399802 openfisca_survey_manager-2.2.1/openfisca_survey_manager/tests/data_files/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/tests/data_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/tests/data_files/config_template.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/tests/test_add_survey_to_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/tests/test_aggregates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5221 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/tests/test_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/tests/test_calmar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/tests/test_compute_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/tests/test_compute_pivot_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/tests/test_compute_winners_loosers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/tests/test_create_data_frame_by_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/tests/test_legislation_inflator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/tests/test_marginal_tax_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/tests/test_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10781 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/tests/test_parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/tests/test_quantile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/tests/test_read_sas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16428 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/tests/test_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/tests/test_summarize_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/tests/test_surveys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/tests/test_tax_benefit_system_asof.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/tests/test_top_bottom_share.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/tests/test_write_parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12269 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/openfisca_survey_manager/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-24 09:37:23.407802 openfisca_survey_manager-2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-24 09:37:06.000000 openfisca_survey_manager-2.2.1/setup.py
```

### Comparing `OpenFisca-Survey-Manager-2.2.0/CHANGELOG.md` & `openfisca_survey_manager-2.2.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 ﻿# Changelog
 
+## 2.2.1 [#298](https://github.com/openfisca/openfisca-survey-manager/pull/298)
+
+* For `compute_aggregate`, replace the warning by an assert when `weighted = True` (the default) and no weight is defined for the variable. Before, a warning was displayed and the aggregate was computed using uniform weights.
+
 ## 2.2.0 [#295](https://github.com/openfisca/openfisca-survey-manager/pull/295)
 
 * Improve support for parquet file format :
       - If a parquet file is provided to build-collection it will be cleaned an added to the collection as a parquet file.
       - If the option `keep_original_parquet_file` is passed the parquet file is kept and added to the collection as is as is.
 
 ## 2.1.0 [#277](https://github.com/openfisca/openfisca-survey-manager/pull/277)
```

### Comparing `OpenFisca-Survey-Manager-2.2.0/LICENSE.AGPL.txt` & `openfisca_survey_manager-2.2.1/LICENSE.AGPL.txt`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/OpenFisca_Survey_Manager.egg-info/PKG-INFO` & `openfisca_survey_manager-2.2.1/OpenFisca_Survey_Manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenFisca-Survey-Manager
-Version: 2.2.0
+Version: 2.2.1
 Summary: A tool for managing survey/administrative data.
 Home-page: https://github.com/openfisca/openfisca-survey-manager
 Author: OpenFisca Team
 Author-email: contact@openfisca.fr
 License: http://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: survey data
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `OpenFisca-Survey-Manager-2.2.0/OpenFisca_Survey_Manager.egg-info/SOURCES.txt` & `openfisca_survey_manager-2.2.1/OpenFisca_Survey_Manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/OpenFisca_Survey_Manager.egg-info/requires.txt` & `openfisca_survey_manager-2.2.1/OpenFisca_Survey_Manager.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/PKG-INFO` & `openfisca_survey_manager-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenFisca-Survey-Manager
-Version: 2.2.0
+Version: 2.2.1
 Summary: A tool for managing survey/administrative data.
 Home-page: https://github.com/openfisca/openfisca-survey-manager
 Author: OpenFisca Team
 Author-email: contact@openfisca.fr
 License: http://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: survey data
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `OpenFisca-Survey-Manager-2.2.0/README.md` & `openfisca_survey_manager-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/__init__.py` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/aggregates.py` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/aggregates.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_classes.csv` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/assets/nomenclature_coicop_source_by_classes.csv`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_groupes.csv` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/assets/nomenclature_coicop_source_by_groupes.csv`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_postes.csv` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/assets/nomenclature_coicop_source_by_postes.csv`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_sous_classes.csv` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/assets/nomenclature_coicop_source_by_sous_classes.csv`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/calibration.py` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/calibration.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/calmar.py` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/calmar.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/coicop.py` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/coicop.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/config.py` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/config.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/google_colab.py` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/google_colab.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/input_dataframe_generator.py` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/input_dataframe_generator.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/matching.py` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/matching.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/read_dbf.py` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/read_dbf.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/read_sas.py` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/read_sas.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/scenarios/abstract_scenario.py` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/scenarios/abstract_scenario.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/scenarios/reform_scenario.py` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/scenarios/reform_scenario.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/scripts/build_collection.py` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/scripts/build_collection.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/simulation_builder.py` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/simulation_builder.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/simulations.py` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/simulations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Monkey-patch openfisca_core.simulations.Simulation to work with pandas."""
 
 import logging
 import numpy as np
+from numpy import logical_or as or_
 import pandas as pd
 import re
 from typing import Callable, Dict, List, Optional, Union
 
 
 import humanize
 import warnings
@@ -161,30 +162,26 @@
             assert filter_entity_key == entity_key
     else:
         filter_dummy = np.array(1.0)
 
     uniform_weight = np.array(1.0)
     weight_variable = None
     if weighted:
+        assert or_(alternative_weights, weight_variable_by_entity), "The weighted option is set at True but there is no weight variable for entity {} nor alternative weights. Either define a weight variable or switch to unweighted".format(entity_key)
         if alternative_weights:
             if isinstance(alternative_weights, str):
                 assert alternative_weights in tax_benefit_system.variables, \
                     f"{alternative_weights} is not a valid variable of the tax benefit system"
                 weight_variable = alternative_weights
 
             elif (type(alternative_weights) is int) or (type(alternative_weights) is float):
                 weight_variable = None
                 uniform_weight = float(alternative_weights)
-
-        else:
-            if weight_variable_by_entity:
-                weight_variable = weight_variable_by_entity[entity_key]
-
-            else:
-                log.warn('There is no weight variable for entity {} nor alternative weights. Switch to unweighted'.format(entity_key))
+        elif weight_variable_by_entity:
+            weight_variable = weight_variable_by_entity[entity_key]
 
     if variable in simulation.tax_benefit_system.variables:
         value = simulation.adaptative_calculate_variable(variable = variable, period = period)
     else:
         log.debug("Variable {} not found. Assigning {}".format(variable, missing_variable_default_value))
         return missing_variable_default_value
```

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/statshelpers.py` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/statshelpers.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/survey_collections.py` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/survey_collections.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/surveys.py` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/surveys.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tables.py` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/tables.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/temporary.py` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/temporary.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/__init__.py` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_add_survey_to_collection.py` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/tests/test_add_survey_to_collection.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_aggregates.py` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/tests/test_aggregates.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_calibration.py` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/tests/test_calibration.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_calmar.py` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/tests/test_calmar.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_compute_aggregate.py` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/tests/test_compute_aggregate.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,8 +29,9 @@
 
     del survey_scenario.weight_variable_by_entity
     survey_scenario.set_weight_variable_by_entity()
     assert 576 == survey_scenario.compute_aggregate(
         "social_security_contribution",
         period = period,
         filter_by = "3000 < salary < 10000",
+        weighted = False,
         ).astype(int)
```

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_compute_pivot_table.py` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/tests/test_compute_pivot_table.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_compute_winners_loosers.py` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/tests/test_compute_winners_loosers.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_create_data_frame_by_entity.py` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/tests/test_create_data_frame_by_entity.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_legislation_inflator.py` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/tests/test_legislation_inflator.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_marginal_tax_rate.py` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/tests/test_marginal_tax_rate.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_matching.py` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/tests/test_matching.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_parquet.py` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/tests/test_parquet.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_quantile.py` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/tests/test_quantile.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_read_sas.py` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/tests/test_read_sas.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_scenario.py` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/tests/test_scenario.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_summarize_variables.py` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/tests/test_summarize_variables.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_surveys.py` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/tests/test_surveys.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_tax_benefit_system_asof.py` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/tests/test_tax_benefit_system_asof.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_write_parquet.py` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/tests/test_write_parquet.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/utils.py` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/utils.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/variables.py` & `openfisca_survey_manager-2.2.1/openfisca_survey_manager/variables.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/setup.cfg` & `openfisca_survey_manager-2.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.2.0/setup.py` & `openfisca_survey_manager-2.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 """
 
 doc_lines = __doc__.split('\n')
 
 
 setup(
     name = 'OpenFisca-Survey-Manager',
-    version = '2.2.0',
+    version = '2.2.1',
     author = 'OpenFisca Team',
     author_email = 'contact@openfisca.fr',
     classifiers = [classifier for classifier in classifiers.split('\n') if classifier],
     description = doc_lines[0],
     keywords = 'survey data',
     license = 'http://www.fsf.org/licensing/licenses/agpl-3.0.html',
     license_files = ("LICENSE.AGPL.txt",),
```

