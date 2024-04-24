# Comparing `tmp/ugropy-2.0.0.tar.gz` & `tmp/ugropy-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ugropy-2.0.0.tar", last modified: Wed Mar  6 01:46:52 2024, max compression
+gzip compressed data, was "ugropy-2.0.5.tar", last modified: Wed Apr 24 02:30:03 2024, max compression
```

## Comparing `ugropy-2.0.0.tar` & `ugropy-2.0.5.tar`

### file list

```diff
@@ -1,65 +1,73 @@
-drwxrwxr-x   0 salvador  (1000) salvador  (1000)        0 2024-03-06 01:46:52.607929 ugropy-2.0.0/
--rw-rw-r--   0 salvador  (1000) salvador  (1000)     9390 2024-02-20 21:10:18.000000 ugropy-2.0.0/CONTRIBUTING.md
--rw-rw-r--   0 salvador  (1000) salvador  (1000)     1083 2023-09-06 01:12:42.000000 ugropy-2.0.0/LICENSE
--rw-rw-r--   0 salvador  (1000) salvador  (1000)      321 2024-03-03 19:08:50.000000 ugropy-2.0.0/MANIFEST.in
--rw-r--r--   0 salvador  (1000) salvador  (1000)     5449 2024-03-06 01:46:52.607929 ugropy-2.0.0/PKG-INFO
--rw-rw-r--   0 salvador  (1000) salvador  (1000)     4602 2024-03-06 01:11:54.000000 ugropy-2.0.0/README.md
--rw-rw-r--   0 salvador  (1000) salvador  (1000)     1199 2024-03-05 22:34:48.000000 ugropy-2.0.0/pyproject.toml
--rw-rw-r--   0 salvador  (1000) salvador  (1000)       68 2024-03-03 19:22:02.000000 ugropy-2.0.0/requirements.txt
--rw-rw-r--   0 salvador  (1000) salvador  (1000)       38 2024-03-06 01:46:52.607929 ugropy-2.0.0/setup.cfg
-drwxrwxr-x   0 salvador  (1000) salvador  (1000)        0 2024-03-06 01:46:52.601929 ugropy-2.0.0/ugropy/
--rw-rw-r--   0 salvador  (1000) salvador  (1000)      477 2024-03-03 18:37:04.000000 ugropy-2.0.0/ugropy/__init__.py
--rw-rw-r--   0 salvador  (1000) salvador  (1000)      262 2024-03-03 18:34:13.000000 ugropy-2.0.0/ugropy/constants.py
-drwxrwxr-x   0 salvador  (1000) salvador  (1000)        0 2024-03-06 01:46:52.603929 ugropy-2.0.0/ugropy/core/
--rw-rw-r--   0 salvador  (1000) salvador  (1000)      792 2024-03-05 21:40:08.000000 ugropy-2.0.0/ugropy/core/__init__.py
--rw-rw-r--   0 salvador  (1000) salvador  (1000)     7688 2024-03-04 22:39:58.000000 ugropy-2.0.0/ugropy/core/checks.py
--rw-rw-r--   0 salvador  (1000) salvador  (1000)     6683 2024-03-02 23:13:42.000000 ugropy-2.0.0/ugropy/core/composed.py
--rw-rw-r--   0 salvador  (1000) salvador  (1000)     2601 2024-02-29 00:56:02.000000 ugropy-2.0.0/ugropy/core/detect_model_groups.py
--rw-rw-r--   0 salvador  (1000) salvador  (1000)     4942 2024-03-05 23:29:09.000000 ugropy-2.0.0/ugropy/core/draw_molecule.py
--rw-rw-r--   0 salvador  (1000) salvador  (1000)     2530 2024-03-05 20:44:45.000000 ugropy-2.0.0/ugropy/core/fit_atoms_indexes.py
--rw-rw-r--   0 salvador  (1000) salvador  (1000)     2738 2024-03-05 21:52:02.000000 ugropy-2.0.0/ugropy/core/fragmentation_object.py
--rw-rw-r--   0 salvador  (1000) salvador  (1000)     5527 2024-03-04 23:24:59.000000 ugropy-2.0.0/ugropy/core/get_model_groups.py
--rw-rw-r--   0 salvador  (1000) salvador  (1000)     1652 2024-02-20 21:10:18.000000 ugropy-2.0.0/ugropy/core/get_rdkit_object.py
--rw-rw-r--   0 salvador  (1000) salvador  (1000)     2795 2024-02-20 21:10:18.000000 ugropy-2.0.0/ugropy/core/problematics.py
-drwxrwxr-x   0 salvador  (1000) salvador  (1000)        0 2024-03-06 01:46:52.603929 ugropy-2.0.0/ugropy/fragmentation_models/
--rw-rw-r--   0 salvador  (1000) salvador  (1000)      265 2024-03-03 18:19:35.000000 ugropy-2.0.0/ugropy/fragmentation_models/__init__.py
--rw-rw-r--   0 salvador  (1000) salvador  (1000)     7724 2024-03-04 22:38:37.000000 ugropy-2.0.0/ugropy/fragmentation_models/fragmentation_model.py
--rw-rw-r--   0 salvador  (1000) salvador  (1000)     5008 2024-03-03 19:53:56.000000 ugropy-2.0.0/ugropy/fragmentation_models/gibbs_model.py
--rw-rw-r--   0 salvador  (1000) salvador  (1000)     3398 2024-03-03 18:31:45.000000 ugropy-2.0.0/ugropy/fragmentation_models/models.py
--rw-rw-r--   0 salvador  (1000) salvador  (1000)     3975 2024-03-03 20:03:57.000000 ugropy-2.0.0/ugropy/fragmentation_models/prop_estimator.py
--rw-rw-r--   0 salvador  (1000) salvador  (1000)     2571 2024-03-03 20:01:07.000000 ugropy-2.0.0/ugropy/groups.py
-drwxrwxr-x   0 salvador  (1000) salvador  (1000)        0 2024-03-06 01:46:52.603929 ugropy-2.0.0/ugropy/groupscsv/
-drwxrwxr-x   0 salvador  (1000) salvador  (1000)        0 2024-03-06 01:46:52.604929 ugropy-2.0.0/ugropy/groupscsv/joback/
--rw-rw-r--   0 salvador  (1000) salvador  (1000)      441 2024-02-20 21:10:18.000000 ugropy-2.0.0/ugropy/groupscsv/joback/joback_problematics.csv
--rw-rw-r--   0 salvador  (1000) salvador  (1000)     2476 2024-03-05 20:44:45.000000 ugropy-2.0.0/ugropy/groupscsv/joback/joback_subgroups.csv
--rw-rw-r--   0 salvador  (1000) salvador  (1000)     4413 2024-02-20 21:10:18.000000 ugropy-2.0.0/ugropy/groupscsv/joback/properties_contrib.csv
--rw-rw-r--   0 salvador  (1000) salvador  (1000)     5935 2024-03-04 23:27:29.000000 ugropy-2.0.0/ugropy/groupscsv/problematic_structures.csv
-drwxrwxr-x   0 salvador  (1000) salvador  (1000)        0 2024-03-06 01:46:52.604929 ugropy-2.0.0/ugropy/groupscsv/psrk/
--rw-rw-r--   0 salvador  (1000) salvador  (1000)      387 2024-02-20 22:59:59.000000 ugropy-2.0.0/ugropy/groupscsv/psrk/hideouts.csv
--rw-rw-r--   0 salvador  (1000) salvador  (1000)     3538 2024-02-27 20:28:16.000000 ugropy-2.0.0/ugropy/groupscsv/psrk/psrk_info.csv
--rw-rw-r--   0 salvador  (1000) salvador  (1000)     2280 2024-02-20 21:10:18.000000 ugropy-2.0.0/ugropy/groupscsv/psrk/psrk_maingroups.csv
--rw-rw-r--   0 salvador  (1000) salvador  (1000)    10251 2024-03-04 23:29:44.000000 ugropy-2.0.0/ugropy/groupscsv/psrk/psrk_subgroups.csv
-drwxrwxr-x   0 salvador  (1000) salvador  (1000)        0 2024-03-06 01:46:52.605929 ugropy-2.0.0/ugropy/groupscsv/unifac/
--rw-rw-r--   0 salvador  (1000) salvador  (1000)      367 2024-02-28 00:17:27.000000 ugropy-2.0.0/ugropy/groupscsv/unifac/hideouts.csv
--rw-rw-r--   0 salvador  (1000) salvador  (1000)     2722 2024-02-27 20:23:58.000000 ugropy-2.0.0/ugropy/groupscsv/unifac/unifac_info.csv
--rw-rw-r--   0 salvador  (1000) salvador  (1000)     1596 2024-02-20 21:10:18.000000 ugropy-2.0.0/ugropy/groupscsv/unifac/unifac_maingroups.csv
--rw-rw-r--   0 salvador  (1000) salvador  (1000)     8757 2024-03-04 22:53:18.000000 ugropy-2.0.0/ugropy/groupscsv/unifac/unifac_subgroups.csv
-drwxrwxr-x   0 salvador  (1000) salvador  (1000)        0 2024-03-06 01:46:52.605929 ugropy-2.0.0/ugropy/properties/
--rw-rw-r--   0 salvador  (1000) salvador  (1000)      107 2024-03-03 17:17:19.000000 ugropy-2.0.0/ugropy/properties/__init__.py
--rw-rw-r--   0 salvador  (1000) salvador  (1000)    11318 2024-03-03 18:28:11.000000 ugropy-2.0.0/ugropy/properties/joback_properties.py
-drwxrwxr-x   0 salvador  (1000) salvador  (1000)        0 2024-03-06 01:46:52.606929 ugropy-2.0.0/ugropy/writers/
--rw-rw-r--   0 salvador  (1000) salvador  (1000)      317 2024-03-05 22:41:16.000000 ugropy-2.0.0/ugropy/writers/__init__.py
--rw-rw-r--   0 salvador  (1000) salvador  (1000)     2825 2024-03-01 01:21:50.000000 ugropy-2.0.0/ugropy/writers/clapeyron.py
-drwxrwxr-x   0 salvador  (1000) salvador  (1000)        0 2024-03-06 01:46:52.606929 ugropy-2.0.0/ugropy/writers/clapeyron_writers/
--rw-rw-r--   0 salvador  (1000) salvador  (1000)      297 2024-02-06 21:08:58.000000 ugropy-2.0.0/ugropy/writers/clapeyron_writers/__init__.py
--rw-rw-r--   0 salvador  (1000) salvador  (1000)     2529 2024-03-01 01:24:43.000000 ugropy-2.0.0/ugropy/writers/clapeyron_writers/critical.py
--rw-rw-r--   0 salvador  (1000) salvador  (1000)     3564 2024-03-01 01:25:06.000000 ugropy-2.0.0/ugropy/writers/clapeyron_writers/molar_mass.py
--rw-rw-r--   0 salvador  (1000) salvador  (1000)     1867 2024-02-06 21:08:58.000000 ugropy-2.0.0/ugropy/writers/clapeyron_writers/psrk_groups.py
--rw-rw-r--   0 salvador  (1000) salvador  (1000)     1841 2024-02-06 21:08:58.000000 ugropy-2.0.0/ugropy/writers/clapeyron_writers/unifac_groups.py
--rw-rw-r--   0 salvador  (1000) salvador  (1000)      741 2024-03-05 23:02:23.000000 ugropy-2.0.0/ugropy/writers/thermo.py
-drwxrwxr-x   0 salvador  (1000) salvador  (1000)        0 2024-03-06 01:46:52.606929 ugropy-2.0.0/ugropy.egg-info/
--rw-r--r--   0 salvador  (1000) salvador  (1000)     5449 2024-03-06 01:46:52.000000 ugropy-2.0.0/ugropy.egg-info/PKG-INFO
--rw-rw-r--   0 salvador  (1000) salvador  (1000)     1685 2024-03-06 01:46:52.000000 ugropy-2.0.0/ugropy.egg-info/SOURCES.txt
--rw-rw-r--   0 salvador  (1000) salvador  (1000)        1 2024-03-06 01:46:52.000000 ugropy-2.0.0/ugropy.egg-info/dependency_links.txt
--rw-rw-r--   0 salvador  (1000) salvador  (1000)       61 2024-03-06 01:46:52.000000 ugropy-2.0.0/ugropy.egg-info/requires.txt
--rw-rw-r--   0 salvador  (1000) salvador  (1000)        7 2024-03-06 01:46:52.000000 ugropy-2.0.0/ugropy.egg-info/top_level.txt
+drwxrwxr-x   0 salvador  (1000) salvador  (1000)        0 2024-04-24 02:30:03.276448 ugropy-2.0.5/
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)     9390 2024-02-20 21:10:18.000000 ugropy-2.0.5/CONTRIBUTING.md
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)     1083 2023-09-06 01:12:42.000000 ugropy-2.0.5/LICENSE
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)      336 2024-04-24 02:03:06.000000 ugropy-2.0.5/MANIFEST.in
+-rw-r--r--   0 salvador  (1000) salvador  (1000)     4915 2024-04-24 02:30:03.275448 ugropy-2.0.5/PKG-INFO
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)     4068 2024-04-24 01:34:06.000000 ugropy-2.0.5/README.md
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)     1271 2024-04-24 01:35:07.000000 ugropy-2.0.5/pyproject.toml
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)       68 2024-03-03 19:22:02.000000 ugropy-2.0.5/requirements.txt
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)       38 2024-04-24 02:30:03.276448 ugropy-2.0.5/setup.cfg
+drwxrwxr-x   0 salvador  (1000) salvador  (1000)        0 2024-04-24 02:30:03.268448 ugropy-2.0.5/ugropy/
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)      558 2024-04-24 00:09:19.000000 ugropy-2.0.5/ugropy/__init__.py
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)      251 2024-04-23 21:08:51.000000 ugropy-2.0.5/ugropy/constants.py
+drwxrwxr-x   0 salvador  (1000) salvador  (1000)        0 2024-04-24 02:30:03.270448 ugropy-2.0.5/ugropy/core/
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)      792 2024-03-05 21:40:08.000000 ugropy-2.0.5/ugropy/core/__init__.py
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)     7688 2024-03-04 22:39:58.000000 ugropy-2.0.5/ugropy/core/checks.py
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)     6683 2024-03-02 23:13:42.000000 ugropy-2.0.5/ugropy/core/composed.py
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)     2601 2024-02-29 00:56:02.000000 ugropy-2.0.5/ugropy/core/detect_model_groups.py
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)     4942 2024-03-05 23:29:09.000000 ugropy-2.0.5/ugropy/core/draw_molecule.py
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)     2530 2024-03-05 20:44:45.000000 ugropy-2.0.5/ugropy/core/fit_atoms_indexes.py
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)     2738 2024-03-05 21:52:02.000000 ugropy-2.0.5/ugropy/core/fragmentation_object.py
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)     5527 2024-04-17 01:34:23.000000 ugropy-2.0.5/ugropy/core/get_model_groups.py
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)     1687 2024-04-23 21:08:51.000000 ugropy-2.0.5/ugropy/core/get_rdkit_object.py
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)     2755 2024-04-23 21:08:51.000000 ugropy-2.0.5/ugropy/core/problematics.py
+drwxrwxr-x   0 salvador  (1000) salvador  (1000)        0 2024-04-24 02:30:03.271448 ugropy-2.0.5/ugropy/fragmentation_models/
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)      325 2024-04-23 21:08:51.000000 ugropy-2.0.5/ugropy/fragmentation_models/__init__.py
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)     7724 2024-03-04 22:38:37.000000 ugropy-2.0.5/ugropy/fragmentation_models/fragmentation_model.py
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)     5008 2024-03-03 19:53:56.000000 ugropy-2.0.5/ugropy/fragmentation_models/gibbs_model.py
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)     4681 2024-04-24 01:32:15.000000 ugropy-2.0.5/ugropy/fragmentation_models/models.py
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)     3975 2024-03-03 20:03:57.000000 ugropy-2.0.5/ugropy/fragmentation_models/prop_estimator.py
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)     2571 2024-04-24 01:39:11.000000 ugropy-2.0.5/ugropy/groups.py
+drwxrwxr-x   0 salvador  (1000) salvador  (1000)        0 2024-04-24 02:30:03.271448 ugropy-2.0.5/ugropy/groupscsv/
+drwxrwxr-x   0 salvador  (1000) salvador  (1000)        0 2024-04-24 02:30:03.266448 ugropy-2.0.5/ugropy/groupscsv/constantinou_gani/
+drwxrwxr-x   0 salvador  (1000) salvador  (1000)        0 2024-04-24 02:30:03.272448 ugropy-2.0.5/ugropy/groupscsv/constantinou_gani/primary/
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)     6304 2024-04-23 21:08:51.000000 ugropy-2.0.5/ugropy/groupscsv/constantinou_gani/primary/c_g_prymary_subgroups.csv
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)     3421 2024-04-23 21:08:51.000000 ugropy-2.0.5/ugropy/groupscsv/constantinou_gani/primary/cg_problematics.csv
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)      332 2024-04-23 21:08:51.000000 ugropy-2.0.5/ugropy/groupscsv/constantinou_gani/primary/hideouts.csv
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)      585 2024-04-23 21:08:51.000000 ugropy-2.0.5/ugropy/groupscsv/constantinou_gani/primary/properties_prymary_contrib.csv
+drwxrwxr-x   0 salvador  (1000) salvador  (1000)        0 2024-04-24 02:30:03.272448 ugropy-2.0.5/ugropy/groupscsv/constantinou_gani/secondary/
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)      932 2024-04-23 21:08:51.000000 ugropy-2.0.5/ugropy/groupscsv/constantinou_gani/secondary/structures.csv
+drwxrwxr-x   0 salvador  (1000) salvador  (1000)        0 2024-04-24 02:30:03.272448 ugropy-2.0.5/ugropy/groupscsv/joback/
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)      441 2024-02-20 21:10:18.000000 ugropy-2.0.5/ugropy/groupscsv/joback/joback_problematics.csv
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)     2476 2024-03-05 20:44:45.000000 ugropy-2.0.5/ugropy/groupscsv/joback/joback_subgroups.csv
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)     4413 2024-02-20 21:10:18.000000 ugropy-2.0.5/ugropy/groupscsv/joback/properties_contrib.csv
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)     5935 2024-04-17 01:31:22.000000 ugropy-2.0.5/ugropy/groupscsv/problematic_structures.csv
+drwxrwxr-x   0 salvador  (1000) salvador  (1000)        0 2024-04-24 02:30:03.273448 ugropy-2.0.5/ugropy/groupscsv/psrk/
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)      365 2024-04-23 21:08:51.000000 ugropy-2.0.5/ugropy/groupscsv/psrk/hideouts.csv
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)     3538 2024-02-27 20:28:16.000000 ugropy-2.0.5/ugropy/groupscsv/psrk/psrk_info.csv
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)     2280 2024-02-20 21:10:18.000000 ugropy-2.0.5/ugropy/groupscsv/psrk/psrk_maingroups.csv
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)    10246 2024-04-23 21:08:51.000000 ugropy-2.0.5/ugropy/groupscsv/psrk/psrk_subgroups.csv
+drwxrwxr-x   0 salvador  (1000) salvador  (1000)        0 2024-04-24 02:30:03.274448 ugropy-2.0.5/ugropy/groupscsv/unifac/
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)      345 2024-04-23 21:08:51.000000 ugropy-2.0.5/ugropy/groupscsv/unifac/hideouts.csv
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)     2722 2024-02-27 20:23:58.000000 ugropy-2.0.5/ugropy/groupscsv/unifac/unifac_info.csv
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)     1596 2024-02-20 21:10:18.000000 ugropy-2.0.5/ugropy/groupscsv/unifac/unifac_maingroups.csv
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)     8752 2024-04-23 21:08:51.000000 ugropy-2.0.5/ugropy/groupscsv/unifac/unifac_subgroups.csv
+drwxrwxr-x   0 salvador  (1000) salvador  (1000)        0 2024-04-24 02:30:03.274448 ugropy-2.0.5/ugropy/properties/
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)      107 2024-03-03 17:17:19.000000 ugropy-2.0.5/ugropy/properties/__init__.py
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)    11633 2024-04-24 01:00:11.000000 ugropy-2.0.5/ugropy/properties/joback_properties.py
+drwxrwxr-x   0 salvador  (1000) salvador  (1000)        0 2024-04-24 02:30:03.274448 ugropy-2.0.5/ugropy/writers/
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)      317 2024-03-05 22:41:16.000000 ugropy-2.0.5/ugropy/writers/__init__.py
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)     3075 2024-04-23 21:08:51.000000 ugropy-2.0.5/ugropy/writers/clapeyron.py
+drwxrwxr-x   0 salvador  (1000) salvador  (1000)        0 2024-04-24 02:30:03.275448 ugropy-2.0.5/ugropy/writers/clapeyron_writers/
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)      297 2024-02-06 21:08:58.000000 ugropy-2.0.5/ugropy/writers/clapeyron_writers/__init__.py
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)     2618 2024-04-23 21:08:51.000000 ugropy-2.0.5/ugropy/writers/clapeyron_writers/critical.py
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)     3686 2024-04-23 21:08:51.000000 ugropy-2.0.5/ugropy/writers/clapeyron_writers/molar_mass.py
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)     1895 2024-04-23 21:08:51.000000 ugropy-2.0.5/ugropy/writers/clapeyron_writers/psrk_groups.py
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)     1877 2024-04-23 21:08:51.000000 ugropy-2.0.5/ugropy/writers/clapeyron_writers/unifac_groups.py
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)      741 2024-03-05 23:02:23.000000 ugropy-2.0.5/ugropy/writers/thermo.py
+drwxrwxr-x   0 salvador  (1000) salvador  (1000)        0 2024-04-24 02:30:03.275448 ugropy-2.0.5/ugropy.egg-info/
+-rw-r--r--   0 salvador  (1000) salvador  (1000)     4915 2024-04-24 02:30:03.000000 ugropy-2.0.5/ugropy.egg-info/PKG-INFO
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)     2007 2024-04-24 02:30:03.000000 ugropy-2.0.5/ugropy.egg-info/SOURCES.txt
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)        1 2024-04-24 02:30:03.000000 ugropy-2.0.5/ugropy.egg-info/dependency_links.txt
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)       61 2024-04-24 02:30:03.000000 ugropy-2.0.5/ugropy.egg-info/requires.txt
+-rw-rw-r--   0 salvador  (1000) salvador  (1000)        7 2024-04-24 02:30:03.000000 ugropy-2.0.5/ugropy.egg-info/top_level.txt
```

### Comparing `ugropy-2.0.0/CONTRIBUTING.md` & `ugropy-2.0.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ugropy-2.0.0/LICENSE` & `ugropy-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ugropy-2.0.0/PKG-INFO` & `ugropy-2.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ugropy
-Version: 2.0.0
+Version: 2.0.5
 Summary: Get UNIFAC functional groups of PubChem compounds or SMILES representation.
 Author-email: "Brandolín, Salvador Eduardo" <salvadorebrandolin@mi.unc.edu.ar>
 License: The MIT License
 Project-URL: Homepage, https://github.com/ipqa-research/ugropy
 Keywords: UNIFAC,functional group,thermodynamics,chemical engineering
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
@@ -24,47 +24,54 @@
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ipqa-research/ugropy/main)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://tldrlegal.com/license/mit-license)
 ![Python 3.10+](https://img.shields.io/badge/Python-3.10%2B-blue)
 [![Docs](https://img.shields.io/badge/docs%20-%20green?style=flat&label=Sphinx&link=https%3A%2F%2Fipqa-research.github.io%2Fugropy%2Findex.html)](https://salvadorbrandolin.github.io/ugropy/)
 [![PyPI
 version](https://badge.fury.io/py/ugropy.svg)](https://badge.fury.io/py/ugropy)
 
-`ugropy` is a `Python` library to obtain subgroups from different
-thermodynamic group contribution models using both the name or the SMILES
-representation of a molecule. If the name is given, the library uses the
+`ugropy` is a `Python` library to obtain subgroups from different thermodynamic
+group contribution models using both the name or the SMILES representation of a
+molecule. If the name is given, the library uses the
 [PubChemPy](https://github.com/mcs07/PubChemPy) library to obtain the SMILES
 representation from PubChem. In both cases, `ugropy` uses the
 [RDKit](https://github.com/rdkit/rdkit) library to search the functional groups
 in the molecule.
 
 `ugropy` is in an early development stage, leaving issues of examples of
 molecules that `ugropy` fails solving the subgroups of a model is very helpful.
 
+`ugropy` is tested for `Python` 3.10, 3.11 and 3.12 on Linux, Windows and Mac
+OS.
+
 ## Try ugropy now
 You can try ugropy from its
 [Binder](https://mybinder.org/v2/gh/ipqa-research/ugropy/main). Open the
 binder.ipynb file to explore the basic features.
 
-## Models supported v2.0.0
+## Models supported v2.0.5
 - Classic liquid-vapor UNIFAC
 - Predictive Soave-Redlich-Kwong (PSRK)
 - Joback
 
 ## Writers
+`ugropy` allows you to convert the obtained functional groups or estimated
+properties to the input format required by the following thermodynamic
+libraries:
 
 - [Clapeyron.jl](github.com/ClapeyronThermo/Clapeyron.jl)
 - [Thermo](https://github.com/CalebBell/thermo)
 
 
 ## Example of use
 You can check the full tutorial
 [here](https://ipqa-research.github.io/ugropy/tutorial/tutorial.html).
 
 Get groups from the molecule's name:
 
+
 ```python
 from ugropy import Groups
 
 
 hexane = Groups("hexane")
 
 print(hexane.unifac.subgroups)
@@ -134,15 +141,15 @@
 
 # Write the csv files into a database directory
 writers.to_clapeyron(
     molecules_names=names,
     unifac_groups=[g.unifac.subgroups for g in grps],
     psrk_groups=[g.psrk.subgroups for g in grps],
     joback_objects=[g.joback for g in grps],
-    path="./database"
+    path="database"
 )
 ```
 Obtain the [Caleb Bell's Thermo](https://github.com/CalebBell/thermo) subgroups
 
 ```python
 from ugropy import unifac
 
@@ -157,26 +164,7 @@
 [{1: 2, 2: 4}, {1: 1, 2: 1, 18: 1}]
 ```
 
 ## Installation
 ```
 pip install ugropy
 ```
-
-## Refereces
-
-[1] http://www.ddbst.com/published-parameters-unifac.html
-
-[2] Joback, K. G., & Reid, R. C. (1987). ESTIMATION OF PURE-COMPONENT
-PROPERTIES FROM GROUP-CONTRIBUTIONS. Chemical Engineering Communications,
-57(1–6), 233–243. https://doi.org/10.1080/00986448708960487
-
-[3] Joback, K. G. (1989). Designing molecules possessing desired physical
-property values [Thesis (Ph. D.), Massachusetts Institute of Technology].
-https://dspace.mit.edu/handle/1721.1/14191
-
-[4] Bondi, A. (1966). Estimation of Heat Capacity of Liquids. Industrial &
-Engineering Chemistry Fundamentals, 5(4), 442–449.
-https://doi.org/10.1021/i160020a001
-
-[5] Rowlinson, J. S., & Swinton, F. (2013). Liquids and liquid mixtures:
-Butterworths monographs in chemistry. Butterworth-Heinemann
```

### Comparing `ugropy-2.0.0/README.md` & `ugropy-2.0.5/ugropy.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,49 +1,77 @@
+Metadata-Version: 2.1
+Name: ugropy
+Version: 2.0.5
+Summary: Get UNIFAC functional groups of PubChem compounds or SMILES representation.
+Author-email: "Brandolín, Salvador Eduardo" <salvadorebrandolin@mi.unc.edu.ar>
+License: The MIT License
+Project-URL: Homepage, https://github.com/ipqa-research/ugropy
+Keywords: UNIFAC,functional group,thermodynamics,chemical engineering
+Classifier: Development Status :: 1 - Planning
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy>=1.25.1
+Requires-Dist: pandas>=2.0.3
+Requires-Dist: pubchempy==1.0.4
+Requires-Dist: rdkit==2023.9.5
+
 ![logo](logo.svg)
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ipqa-research/ugropy/main)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://tldrlegal.com/license/mit-license)
 ![Python 3.10+](https://img.shields.io/badge/Python-3.10%2B-blue)
 [![Docs](https://img.shields.io/badge/docs%20-%20green?style=flat&label=Sphinx&link=https%3A%2F%2Fipqa-research.github.io%2Fugropy%2Findex.html)](https://salvadorbrandolin.github.io/ugropy/)
 [![PyPI
 version](https://badge.fury.io/py/ugropy.svg)](https://badge.fury.io/py/ugropy)
 
-`ugropy` is a `Python` library to obtain subgroups from different
-thermodynamic group contribution models using both the name or the SMILES
-representation of a molecule. If the name is given, the library uses the
+`ugropy` is a `Python` library to obtain subgroups from different thermodynamic
+group contribution models using both the name or the SMILES representation of a
+molecule. If the name is given, the library uses the
 [PubChemPy](https://github.com/mcs07/PubChemPy) library to obtain the SMILES
 representation from PubChem. In both cases, `ugropy` uses the
 [RDKit](https://github.com/rdkit/rdkit) library to search the functional groups
 in the molecule.
 
 `ugropy` is in an early development stage, leaving issues of examples of
 molecules that `ugropy` fails solving the subgroups of a model is very helpful.
 
+`ugropy` is tested for `Python` 3.10, 3.11 and 3.12 on Linux, Windows and Mac
+OS.
+
 ## Try ugropy now
 You can try ugropy from its
 [Binder](https://mybinder.org/v2/gh/ipqa-research/ugropy/main). Open the
 binder.ipynb file to explore the basic features.
 
-## Models supported v2.0.0
+## Models supported v2.0.5
 - Classic liquid-vapor UNIFAC
 - Predictive Soave-Redlich-Kwong (PSRK)
 - Joback
 
 ## Writers
+`ugropy` allows you to convert the obtained functional groups or estimated
+properties to the input format required by the following thermodynamic
+libraries:
 
 - [Clapeyron.jl](github.com/ClapeyronThermo/Clapeyron.jl)
 - [Thermo](https://github.com/CalebBell/thermo)
 
 
 ## Example of use
 You can check the full tutorial
 [here](https://ipqa-research.github.io/ugropy/tutorial/tutorial.html).
 
 Get groups from the molecule's name:
 
+
 ```python
 from ugropy import Groups
 
 
 hexane = Groups("hexane")
 
 print(hexane.unifac.subgroups)
@@ -113,15 +141,15 @@
 
 # Write the csv files into a database directory
 writers.to_clapeyron(
     molecules_names=names,
     unifac_groups=[g.unifac.subgroups for g in grps],
     psrk_groups=[g.psrk.subgroups for g in grps],
     joback_objects=[g.joback for g in grps],
-    path="./database"
+    path="database"
 )
 ```
 Obtain the [Caleb Bell's Thermo](https://github.com/CalebBell/thermo) subgroups
 
 ```python
 from ugropy import unifac
 
@@ -136,26 +164,7 @@
 [{1: 2, 2: 4}, {1: 1, 2: 1, 18: 1}]
 ```
 
 ## Installation
 ```
 pip install ugropy
 ```
-
-## Refereces
-
-[1] http://www.ddbst.com/published-parameters-unifac.html
-
-[2] Joback, K. G., & Reid, R. C. (1987). ESTIMATION OF PURE-COMPONENT
-PROPERTIES FROM GROUP-CONTRIBUTIONS. Chemical Engineering Communications,
-57(1–6), 233–243. https://doi.org/10.1080/00986448708960487
-
-[3] Joback, K. G. (1989). Designing molecules possessing desired physical
-property values [Thesis (Ph. D.), Massachusetts Institute of Technology].
-https://dspace.mit.edu/handle/1721.1/14191
-
-[4] Bondi, A. (1966). Estimation of Heat Capacity of Liquids. Industrial &
-Engineering Chemistry Fundamentals, 5(4), 442–449.
-https://doi.org/10.1021/i160020a001
-
-[5] Rowlinson, J. S., & Swinton, F. (2013). Liquids and liquid mixtures:
-Butterworths monographs in chemistry. Butterworth-Heinemann
```

### Comparing `ugropy-2.0.0/pyproject.toml` & `ugropy-2.0.5/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -7,20 +7,21 @@
 target-version = ["py310"]
 
 [tool.pytest.ini_options]
 markers = [
     "UNIFAC: classic UNIFAC model tests",
     "PSRK: predictive SRK model tests",
     "Joback: Joback-Reid contribution model tests",
-    "Dortmund: Dortmund-UNIFAC model tests"
+    "Dortmund: Dortmund-UNIFAC model tests",
+    "ConstantinouGani: Constantinou and Gani contribution model tests"
 ]
 
 [project]
 name = "ugropy"
-version = "2.0.0"
+version = "2.0.5"
 authors = [{name = "Brandolín, Salvador Eduardo", email = "salvadorebrandolin@mi.unc.edu.ar"}]
 license = {text = "The MIT License"}
 readme = "README.md"
 description = "Get UNIFAC functional groups of PubChem compounds or SMILES representation."
 keywords = ["UNIFAC", "functional group", "thermodynamics", "chemical engineering"]
 classifiers = [
     "Development Status :: 1 - Planning",
```

### Comparing `ugropy-2.0.0/ugropy/core/__init__.py` & `ugropy-2.0.5/ugropy/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ugropy-2.0.0/ugropy/core/checks.py` & `ugropy-2.0.5/ugropy/core/checks.py`

 * *Files identical despite different names*

### Comparing `ugropy-2.0.0/ugropy/core/composed.py` & `ugropy-2.0.5/ugropy/core/composed.py`

 * *Files identical despite different names*

### Comparing `ugropy-2.0.0/ugropy/core/detect_model_groups.py` & `ugropy-2.0.5/ugropy/core/detect_model_groups.py`

 * *Files identical despite different names*

### Comparing `ugropy-2.0.0/ugropy/core/draw_molecule.py` & `ugropy-2.0.5/ugropy/core/draw_molecule.py`

 * *Files identical despite different names*

### Comparing `ugropy-2.0.0/ugropy/core/fit_atoms_indexes.py` & `ugropy-2.0.5/ugropy/core/fit_atoms_indexes.py`

 * *Files identical despite different names*

### Comparing `ugropy-2.0.0/ugropy/core/fragmentation_object.py` & `ugropy-2.0.5/ugropy/core/fragmentation_object.py`

 * *Files identical despite different names*

### Comparing `ugropy-2.0.0/ugropy/core/get_model_groups.py` & `ugropy-2.0.5/ugropy/core/get_model_groups.py`

 * *Files identical despite different names*

### Comparing `ugropy-2.0.0/ugropy/core/get_rdkit_object.py` & `ugropy-2.0.5/ugropy/core/get_rdkit_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """get_rdkit_object module."""
 
+from functools import cache
 from typing import Union
 
 import pubchempy as pcp
 
 from rdkit import Chem
 
 
+@cache
 def instantiate_mol_object(
     identifier: Union[str, Chem.rdchem.Mol], identifier_type: str = "name"
 ) -> Chem.rdchem.Mol:
     """Instantiate a RDKit Mol object from molecule's name or SMILES.
 
     Parameters
     ----------
```

### Comparing `ugropy-2.0.0/ugropy/core/problematics.py` & `ugropy-2.0.5/ugropy/core/problematics.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,14 +63,12 @@
 
             for subgroup, contribution in problematic_dict.items():
                 corrected_subgroups[subgroup] = (
                     corrected_subgroups.get(subgroup, 0)
                     + contribution * how_many_problems
                 )
 
-        # Eliminate occurrences == 0
-        corrected_subgroups = {
-            key: value
-            for key, value in corrected_subgroups.items()
-            if value != 0
-        }
+    # Eliminate occurrences == 0
+    corrected_subgroups = {
+        key: value for key, value in corrected_subgroups.items() if value != 0
+    }
     return corrected_subgroups
```

### Comparing `ugropy-2.0.0/ugropy/fragmentation_models/fragmentation_model.py` & `ugropy-2.0.5/ugropy/fragmentation_models/fragmentation_model.py`

 * *Files identical despite different names*

### Comparing `ugropy-2.0.0/ugropy/fragmentation_models/gibbs_model.py` & `ugropy-2.0.5/ugropy/fragmentation_models/gibbs_model.py`

 * *Files identical despite different names*

### Comparing `ugropy-2.0.0/ugropy/fragmentation_models/models.py` & `ugropy-2.0.5/ugropy/fragmentation_models/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,53 @@
 """Fragmentation models implemented.
 
+All models can be imported directly with:
+
+.. code-block:: python
+
+   from ugropy import joback, psrk, unifac
+
+You can check the group list and their SMARTS representation with:
+
+.. code-block:: python
+
+   joback.subgroups psrk.subgroups unifac.subgroups
+
+In the case of a PropertiesEstimator like joback, you can check the
+contribution of each group to the properties with:
+
+.. code-block:: python
+
+    joback.properties_contributions
+
 Attributes
 ----------
 unifac : GibbsModel
-    Classic LV-UNIFAC FragmentationModel
+    Classic LV-UNIFAC FragmentationModel :cite:p:`ddbst, unifac1, unifac2,
+    unifac3, unifac4, unifac5, unifac6`
 psrk: GibbsModel
-    Predictive Soave-Redlich-Kwong FragmentationModel
+    Predictive Soave-Redlich-Kwong FragmentationModel :cite:p:`ddbst, psrk1,
+    psrk2`
 joback: PropertiesEstimator
-    Joback FragmentationModel
+    Joback FragmentationModel :cite:p:`joback1, joback2`
 """
 
 import pandas as pd
 
 from ugropy.constants import _csvs
 from ugropy.fragmentation_models.gibbs_model import GibbsModel
 from ugropy.fragmentation_models.prop_estimator import PropertiesEstimator
 
 
 def _rd(file_path: str, index_col: str = None) -> pd.DataFrame:
     """Read the models' csv.
 
     Parameters
     ----------
-    file_path : str
+    file_path : str or pathlib
         Path to csv file.
     index_col : str, optional
         Name of the index column, by default None.
 
     Returns
     -------
     pd.DataFrame
@@ -35,42 +56,42 @@
     with open(file_path, mode="r") as f:
         return pd.read_csv(f, sep="|", index_col=index_col, comment="?")
 
 
 # =============================================================================
 # LV-UNIFAC
 # =============================================================================
-_uni = f"{_csvs}/unifac"
+_uni = _csvs / "unifac"
 
-_uni_sg = _rd(f"{_uni}/unifac_subgroups.csv", "group")
-_uni_mg = _rd(f"{_uni}/unifac_maingroups.csv", "no.")
-_uni_info = _rd(f"{_uni}/unifac_info.csv", "group")
-_uni_problems = _rd(f"{_csvs}/problematic_structures.csv", "smarts")
-_uni_hide = _rd(f"{_uni}/hideouts.csv", "group")
+_uni_sg = _rd(_uni / "unifac_subgroups.csv", "group")
+_uni_mg = _rd(_uni / "unifac_maingroups.csv", "no.")
+_uni_info = _rd(_uni / "unifac_info.csv", "group")
+_uni_problems = _rd(_csvs / "problematic_structures.csv", "smarts")
+_uni_hide = _rd(_uni / "hideouts.csv", "group")
 
 unifac = GibbsModel(
     subgroups=_uni_sg,
     split_detection_smarts=["C5H4N", "C5H3N", "C4H3S", "C4H2S"],
     problematic_structures=_uni_problems,
     hideouts=_uni_hide,
     subgroups_info=_uni_info,
     main_groups=_uni_mg,
 )
 
 
 # =============================================================================
 # PSRK
 # =============================================================================
-_psrk = f"{_csvs}/psrk"
+_psrk = _csvs / "psrk"
 
-_psrk_sg = _rd(f"{_psrk}/psrk_subgroups.csv", "group")
-_psrk_mg = _rd(f"{_psrk}/psrk_maingroups.csv", "no.")
-_psrk_info = _rd(f"{_psrk}/psrk_info.csv", "group")
-_psrk_problems = _rd(f"{_csvs}/problematic_structures.csv", "smarts")
-_psrk_hide = _rd(f"{_psrk}/hideouts.csv", "group")
+_psrk_sg = _rd(_psrk / "psrk_subgroups.csv", "group")
+_psrk_mg = _rd(_psrk / "psrk_maingroups.csv", "no.")
+_psrk_info = _rd(_psrk / "psrk_info.csv", "group")
+_psrk_problems = _rd(_csvs / "problematic_structures.csv", "smarts")
+_psrk_hide = _rd(_psrk / "hideouts.csv", "group")
 
 psrk = GibbsModel(
     subgroups=_psrk_sg,
     split_detection_smarts=["C5H4N", "C5H3N", "C4H3S", "C4H2S"],
     problematic_structures=_psrk_problems,
     hideouts=_psrk_hide,
     subgroups_info=_psrk_info,
@@ -78,33 +99,49 @@
 )
 
 # =============================================================================
 # Dortmund
 # =============================================================================
 # _do = f"{_csvs}/dortmund"
 
-# _do_sg = _rd(f"{_do}/dortmund_subgroups.csv", "group")
-# _do_mg = _rd(f"{_do}/dortmund_maingroups.csv", "no.")
-# _do_problems = _rd(f"{_do}/dortmund_problematics.csv", "smarts")
-# _do_hide = _rd(f"{_do}/hideouts.csv", "group")
+# _do_sg = _rd(f"{_do}/dortmund_subgroups.csv", "group") _do_mg =
+# _rd(f"{_do}/dortmund_maingroups.csv", "no.") _do_problems =
+# _rd(f"{_do}/dortmund_problematics.csv", "smarts") _do_hide =
+# _rd(f"{_do}/hideouts.csv", "group")
 #
-# dortmund = FragmentationModel(
-#    subgroups=_do_sg,
-#    main_groups=_do_mg,
-#    problematic_structures=_do_problems,
-#    hideouts=_do_hide,
-# )
+# dortmund = FragmentationModel( subgroups=_do_sg, main_groups=_do_mg,
+#    problematic_structures=_do_problems, hideouts=_do_hide, )
 
 # =============================================================================
 # Joback
 # =============================================================================
-_jo = f"{_csvs}/joback"
+_jo = _csvs / "joback"
 
-_jo_sg = _rd(f"{_jo}/joback_subgroups.csv", "group")
-_jo_problems = _rd(f"{_jo}/joback_problematics.csv", "smarts")
-_jo_props = _rd(f"{_jo}/properties_contrib.csv", "group")
+_jo_sg = _rd(_jo / "joback_subgroups.csv", "group")
+_jo_problems = _rd(_jo / "joback_problematics.csv", "smarts")
+_jo_props = _rd(_jo / "properties_contrib.csv", "group")
 
 joback = PropertiesEstimator(
     subgroups=_jo_sg,
     problematic_structures=_jo_problems,
     properties_contributions=_jo_props,
 )
+
+
+# =============================================================================
+# Constantinou and Gani
+# =============================================================================
+# Primary structures
+_cg_p = _csvs / "constantinou_gani" / "primary"
+
+_cg_sg = _rd(_cg_p / "c_g_prymary_subgroups.csv", "group")
+_cg_problems = _rd(_cg_p / "cg_problematics.csv", "smarts")
+_cg_hide = _rd(_cg_p / "hideouts.csv", "group")
+_cg_props = _rd(_cg_p / "properties_prymary_contrib.csv", "group")
+
+constantinou_gani_primary = PropertiesEstimator(
+    subgroups=_cg_sg,
+    split_detection_smarts=["C5H4N", "C5H3N", "C4H3S", "C4H2S"],
+    problematic_structures=_cg_problems,
+    hideouts=_cg_hide,
+    properties_contributions=_cg_props,
+)
```

### Comparing `ugropy-2.0.0/ugropy/fragmentation_models/prop_estimator.py` & `ugropy-2.0.5/ugropy/fragmentation_models/prop_estimator.py`

 * *Files identical despite different names*

### Comparing `ugropy-2.0.0/ugropy/groups.py` & `ugropy-2.0.5/ugropy/groups.py`

 * *Files identical despite different names*

### Comparing `ugropy-2.0.0/ugropy/groupscsv/joback/joback_subgroups.csv` & `ugropy-2.0.5/ugropy/groupscsv/joback/joback_subgroups.csv`

 * *Files identical despite different names*

### Comparing `ugropy-2.0.0/ugropy/groupscsv/joback/properties_contrib.csv` & `ugropy-2.0.5/ugropy/groupscsv/joback/properties_contrib.csv`

 * *Files identical despite different names*

### Comparing `ugropy-2.0.0/ugropy/groupscsv/problematic_structures.csv` & `ugropy-2.0.5/ugropy/groupscsv/problematic_structures.csv`

 * *Files identical despite different names*

### Comparing `ugropy-2.0.0/ugropy/groupscsv/psrk/psrk_info.csv` & `ugropy-2.0.5/ugropy/groupscsv/psrk/psrk_info.csv`

 * *Files identical despite different names*

### Comparing `ugropy-2.0.0/ugropy/groupscsv/psrk/psrk_maingroups.csv` & `ugropy-2.0.5/ugropy/groupscsv/psrk/psrk_maingroups.csv`

 * *Files identical despite different names*

### Comparing `ugropy-2.0.0/ugropy/groupscsv/psrk/psrk_subgroups.csv` & `ugropy-2.0.5/ugropy/groupscsv/psrk/psrk_subgroups.csv`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 HCO|[CH](=O)([#6,Si])|[CH](=O)|"{""HCO"": 1}"|n|29.018
 CH3COO|[CH3][C](=O)[OH0]||"{""CH3COO"": 1, ""CH3"": -1, ""COO"": -1}"|y|59.044
 CH2COO|[CH2][C](=O)[OH0]||"{""CH2COO"": 1, ""CH2"": -1, ""COO"": -1}"|y|58.036
 HCOO|[CH](=O)[OH0]||"{""HCOO"": 1, ""COO"": -1}"|n|45.017
 CH3O|[CH3]O[$([Si,#6]);!$([CH](=O));!$(C(=O)[!O])]|[CH3][OH0]|"{""CH3O"": 1, ""CH3"": -1}"|n|31.034
 CH2O|[CH2]O[$([Si,#6]);!$([CH](=O));!$(C(=O)[!O]);!$([CH3])]|[CH2][OH0]|"{""CH2O"": 1, ""CH2"": -1}"|n|30.026
 CHO|[CH]O[$([Si,#6]);!$([CH](=O));!$(C(=O)[!O]);!$([CH3]);!$([CH2])]|[CH][OH0]|"{""CHO"": 1, ""CH"": -1}"|n|29.018
-THF|[CH2]1[CH2]O[CH2][CH2]1||"{""THF"": 1, ""CH2O"": -1, ""CH2"": -3}"|n|72.107
+THF|[C]1[CH2]O[CH2][C]1|[CH2;R][O;R]|"{""THF"": 1, ""CH2O"": -1}"|n|30.026
 CH3NH2|[CH3][NH2]||"{""CH3NH2"": 1, ""CH3"": -1}"|n|31.058
 CH2NH2|[CH2][NH2]||"{""CH2NH2"": 1, ""CH2"": -1}"|n|30.05
 CHNH2|[CH][NH2]||"{""CHNH2"": 1, ""CH"": -1}"|n|29.042
 CH3NH|[CH3][NH][#6,Si;!$([CH](=O));!$(C(=O)[!N])]|[CH3][NH]|"{""CH3NH"": 1, ""CH3"": -1}"|n|30.05
 CH2NH|[CH2][NH][$([#6,Si;!$([CH](=O));!$(C(=O)[!N])])&!$([CH3])]|[CH2][NH]|"{""CH2NH"": 1, ""CH2"": -1}"|n|29.042
 CHNH|[CH][NH][$([#6,Si;!$([CH](=O));!$(C(=O)[!N])])&!$([CH3])&!$([CH2])]|[CH][NH]|"{""CHNH"": 1, ""CH"": -1}"|n|28.034
 CH3N|[CH3][NH0]([#6,Si;!$([CH](=O));!$(C(=O)[!N])])[#6,Si;!$([CH](=O));!$(C(=O)[!N])]|[CH3][NH0]|"{""CH3N"": 1, ""CH3"": -1}"|n|29.042
```

### Comparing `ugropy-2.0.0/ugropy/groupscsv/unifac/unifac_info.csv` & `ugropy-2.0.5/ugropy/groupscsv/unifac/unifac_info.csv`

 * *Files identical despite different names*

### Comparing `ugropy-2.0.0/ugropy/groupscsv/unifac/unifac_maingroups.csv` & `ugropy-2.0.5/ugropy/groupscsv/unifac/unifac_maingroups.csv`

 * *Files identical despite different names*

### Comparing `ugropy-2.0.0/ugropy/groupscsv/unifac/unifac_subgroups.csv` & `ugropy-2.0.5/ugropy/groupscsv/unifac/unifac_subgroups.csv`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 HCO|[CH](=O)([#6,Si])|[CH](=O)|"{""HCO"": 1}"|n|29.018
 CH3COO|[CH3][C](=O)[OH0]||"{""CH3COO"": 1, ""CH3"": -1, ""COO"": -1}"|y|59.044
 CH2COO|[CH2][C](=O)[OH0]||"{""CH2COO"": 1, ""CH2"": -1, ""COO"": -1}"|y|58.036
 HCOO|[CH](=O)[OH0]||"{""HCOO"": 1, ""COO"": -1}"|n|45.017
 CH3O|[CH3]O[$([Si,#6]);!$([CH](=O));!$(C(=O)[!O])]|[CH3][OH0]|"{""CH3O"": 1, ""CH3"": -1}"|n|31.034
 CH2O|[CH2]O[$([Si,#6]);!$([CH](=O));!$(C(=O)[!O]);!$([CH3])]|[CH2][OH0]|"{""CH2O"": 1, ""CH2"": -1}"|n|30.026
 CHO|[CH]O[$([Si,#6]);!$([CH](=O));!$(C(=O)[!O]);!$([CH3]);!$([CH2])]|[CH][OH0]|"{""CHO"": 1, ""CH"": -1}"|n|29.018
-THF|[CH2]1[CH2]O[CH2][CH2]1||"{""THF"": 1, ""CH2O"": -1, ""CH2"": -3}"|n|72.107
+THF|[C]1[CH2]O[CH2][C]1|[CH2;R][O;R]|"{""THF"": 1, ""CH2O"": -1}"|n|30.026
 CH3NH2|[CH3][NH2]||"{""CH3NH2"": 1, ""CH3"": -1}"|n|31.058
 CH2NH2|[CH2][NH2]||"{""CH2NH2"": 1, ""CH2"": -1}"|n|30.05
 CHNH2|[CH][NH2]||"{""CHNH2"": 1, ""CH"": -1}"|n|29.042
 CH3NH|[CH3][NH][#6,Si;!$([CH](=O));!$(C(=O)[!N])]|[CH3][NH]|"{""CH3NH"": 1, ""CH3"": -1}"|n|30.05
 CH2NH|[CH2][NH][$([#6,Si;!$([CH](=O));!$(C(=O)[!N])])&!$([CH3])]|[CH2][NH]|"{""CH2NH"": 1, ""CH2"": -1}"|n|29.042
 CHNH|[CH][NH][$([#6,Si;!$([CH](=O));!$(C(=O)[!N])])&!$([CH3])&!$([CH2])]|[CH][NH]|"{""CHNH"": 1, ""CH"": -1}"|n|28.034
 CH3N|[CH3][NH0]([#6,Si;!$([CH](=O));!$(C(=O)[!N])])[#6,Si;!$([CH](=O));!$(C(=O)[!N])]|[CH3][NH0]|"{""CH3N"": 1, ""CH3"": -1}"|n|29.042
```

### Comparing `ugropy-2.0.0/ugropy/properties/joback_properties.py` & `ugropy-2.0.5/ugropy/properties/joback_properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,19 @@
 
 from ugropy.constants import R
 from ugropy.core.get_model_groups import get_groups
 from ugropy.fragmentation_models.models import joback
 
 
 class JobackProperties:
-    """Joback [1] group contribution properties estimator.
+    """Joback group contribution properties estimator.
+
+    The class recieves either the Joback and Reid model's :cite:p:`joback1,
+    joback2` groups, name or smiles of a molecule and estimates the its
+    properties.
 
     Parameters
     ----------
     identifier : str or rdkit.Chem.rdchem.Mol
         Identifier of a molecule (name, SMILES, groups, or Chem.rdchem.Mol).
         Example: you can use hexane, CCCCCC, {"-CH3": 2, "-CH2-": 4} for name,
         SMILES and groups respectively.
@@ -28,15 +32,15 @@
         factor, and vapor pressure instead of the estimated normal boiling
         point, by default None.
 
     Attributes
     ----------
     subgroups : dict
         Joback functional groups of the molecule.
-    exp_nbt : float
+    experimental_boiling_temperature : float
         User provided experimental normal boiling point [K].
     critical_temperature : float
         Joback estimated critical temperature [K].
     critical_pressure : float
         Joback estimated critical pressure [bar].
     critical_volume : float
         Joback estimated critical volume [cm³/mol].
@@ -59,41 +63,41 @@
     sum_na : float
         Joback n_A contribution to liquid viscosity [N/s/m²].
     sum_nb : float
         Joback n_B contribution to liquid viscosity [N/s/m²].
     molecular_weight : float
         Molecular weight from Joback's subgroups [g/mol].
     acentric_factor : float
-        Acentric factor from Lee and Kesler's equation [2].
+        Acentric factor from Lee and Kesler's equation :cite:p:`joback1`.
     vapor_pressure_params : dict
-        Vapor pressure G and k parameters for the Riedel-Plank-Miller [2]
-        equation [bar].
+        Vapor pressure G and k parameters for the Riedel-Plank-Miller
+        :cite:p:`joback1` equation [bar].
     """
 
     def __init__(
         self,
         identifier: str,
         identifier_type: str = "name",
         normal_boiling_point: float = None,
     ) -> None:
-        # Skip if instantiation from_groups is made.
+        # Skip if instantiation from groups is made.
         if identifier_type in ["name", "smiles", "mol"]:
             self.subgroups = get_groups(
                 joback, identifier, identifier_type
             ).subgroups
         elif identifier_type == "groups":
             self.subgroups = identifier
         else:
             raise ValueError(
                 f"Identifier type ''{identifier_type}'' is incorrect. Use "
                 "'name', 'smiles', 'mol' or 'groups'."
             )
 
         # experimental boiling temperature
-        self.exp_nbt = normal_boiling_point
+        self.experimental_boiling_temperature = normal_boiling_point
 
         # Original Joback properties
         self.critical_temperature = None
         self.critical_pressure = None
         self.critical_volume = None
         self.normal_boiling_point = None
         self.fusion_temperature = None
@@ -139,16 +143,16 @@
         return a + b * t + c * t**2 + d * t**3
 
     def heat_capacity_liquid(
         self, temperature: Union[float, NDArray]
     ) -> Union[float, NDArray]:
         """Calculate the liquid heat capacity [J/mol/K].
 
-        Uses the Rowlinson-Bondi [4-5] equation with the Joback estimated
-        properties.
+        Uses the Rowlinson-Bondi :cite:p:`joback1` equation with the Joback
+        estimated properties.
 
         Parameters
         ----------
         temperature : Union[float, NDArray]
             Temperature [K]
 
         Returns
@@ -197,16 +201,16 @@
         return n_l
 
     def vapor_pressure(
         self, temperature: Union[float, NDArray]
     ) -> Union[float, NDArray]:
         """Calculate the vapor pressure [bar].
 
-        Uses the Riedel-Plank-Miller [3] equation with the Joback estimated
-        properties.
+        Uses the Riedel-Plank-Miller :cite:p:`joback1` equation with the Joback
+        estimated properties.
 
         Parameters
         ----------
         temperature : Union[float, NDArray]
             Temperature [K]
 
         Returns
@@ -252,16 +256,16 @@
         # Joback normal boiling point (Tb)
         self.normal_boiling_point = 198.2 + np.dot(ocurr, tb_c)
 
         # Fusion temperature (Tf)
         self.fusion_temperature = 122.5 + np.dot(ocurr, tf_c)
 
         # Used normal boiling point for calculations
-        if self.exp_nbt is not None:
-            tb = self.exp_nbt
+        if self.experimental_boiling_temperature is not None:
+            tb = self.experimental_boiling_temperature
         else:
             tb = self.normal_boiling_point
 
         # Critical temperature (Tc) normal boiling temperature for calculations
         self.critical_temperature = tb * (
             0.584 + 0.965 * np.dot(ocurr, tc_c) - (np.dot(ocurr, tc_c)) ** 2
         ) ** (-1)
```

### Comparing `ugropy-2.0.0/ugropy/writers/clapeyron.py` & `ugropy-2.0.5/ugropy/writers/clapeyron.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """to_clapeyron module."""
 
+import pathlib
 from typing import List
 
 from ugropy.properties.joback_properties import JobackProperties
 
 from .clapeyron_writers import (
     write_critical,
     write_molar_mass,
@@ -13,15 +14,15 @@
 
 
 def to_clapeyron(
     molecules_names: List[str],
     unifac_groups: List[dict] = [],
     psrk_groups: List[dict] = [],
     joback_objects: List[JobackProperties] = [],
-    path: str = "./database",
+    path: str = "database",
     batch_name: str = "",
 ) -> None:
     """Write the .csv input files for Clapeyron.jl.
 
     The provided lists must have the same length. If one of the model lists is
     left empty, that model will not be writen in the .csv.
 
@@ -39,14 +40,17 @@
         Path to the directory to store de .csv files, by default "./database".
     batch_name : str, optional
         Name of the writing batch. For example, if you name the batch with
         "batch1", the output of the UNIFAC groups will be:
         "batch1_ogUNIFAC_groups.csv". With the default value will be
         "ogUNIFAC_groups.csv", by default "".
     """
+    # Use pathlib's Path internally
+    path_pathlib = pathlib.Path(path)
+
     # Check if all list have correct data:
     if len(molecules_names) == 0:
         raise ValueError("No names provided for the molecules.")
 
     if unifac_groups and len(unifac_groups) != len(molecules_names):
         raise ValueError(
             "UNIFAC groups list must have the same amount of elements than"
@@ -61,28 +65,34 @@
 
     if joback_objects and len(joback_objects) != len(molecules_names):
         raise ValueError(
             "Joback objects list must have the same amount of elements than"
             "the molecules name list."
         )
 
+    # Create dir if not created
+    if not path_pathlib.is_dir():
+        path_pathlib.mkdir(parents=True)
+
     # Molar mass
     write_molar_mass(
-        path,
+        path_pathlib,
         batch_name,
         molecules_names,
         unifac_groups,
         psrk_groups,
         joback_objects,
     )
 
     # LV-UNIFAC
     if unifac_groups:
-        write_unifac(path, batch_name, molecules_names, unifac_groups)
+        write_unifac(path_pathlib, batch_name, molecules_names, unifac_groups)
 
     # PSRK
     if psrk_groups:
-        write_psrk(path, batch_name, molecules_names, psrk_groups)
+        write_psrk(path_pathlib, batch_name, molecules_names, psrk_groups)
 
     # Critical
     if joback_objects:
-        write_critical(path, batch_name, molecules_names, joback_objects)
+        write_critical(
+            path_pathlib, batch_name, molecules_names, joback_objects
+        )
```

### Comparing `ugropy-2.0.0/ugropy/writers/clapeyron_writers/critical.py` & `ugropy-2.0.5/ugropy/writers/clapeyron_writers/critical.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 """Joback critical properties writer module."""
 
+import pathlib
 from io import StringIO
 from typing import List
 
 import pandas as pd
 
 from ugropy.properties.joback_properties import JobackProperties
 
 
 def write_critical(
-    path: str,
+    path: pathlib.Path,
     batch_name: str,
     molecules_names: List[str],
     joback_objects: List[JobackProperties] = [],
 ) -> None:
     """Create the DataFrame with the critical properties for Clapeyron.jl.
 
     Uses the Joback to estimate the critical properties of the molecules.
 
     Parameters
     ----------
-    path : str, optional
+    path : pathlib.Path, optional
         Path to the directory to store de .csv files, by default "./database".
     batch_name : str, optional
         Name of the writing batch. For example, if you name the batch with
         "batch1", the output of the UNIFAC groups will be:
         "batch1_ogUNIFAC_groups.csv". With the default value will be
         "ogUNIFAC_groups.csv", by default "".
     molecules_names : List[str]
@@ -38,14 +39,15 @@
         DataFrame with the molecular weights for Clapeyron.jl
     """
     data_str = (
         "Clapeyron Database File,,,,,\n"
         "Critical Single Parameters,,,,,\n"
         "species,CAS,Tc,Pc,Vc,acentricfactor\n"
     )
+    path_critical = pathlib.Path(path)
     # =========================================================================
     # Build dataframe
     # =========================================================================
     df = pd.read_csv(StringIO(data_str))
 
     for idx, name in enumerate(molecules_names):
         new_row = {
@@ -58,19 +60,19 @@
         }
         df.loc[len(df)] = new_row
 
     df.columns = ["" if "Unnamed" in col else col for col in df.columns]
 
     if batch_name == "":
         with open(
-            f"{path}/critical.csv", "w", newline="", encoding="utf-8"
+            path_critical / "critical.csv", "w", newline="", encoding="utf-8"
         ) as file:
             df.to_csv(file, index=False)
 
     else:
         with open(
-            f"{path}/{batch_name}_critical.csv",
+            path_critical / f"{batch_name}_critical.csv",
             "w",
             newline="",
             encoding="utf-8",
         ) as file:
             df.to_csv(file, index=False)
```

### Comparing `ugropy-2.0.0/ugropy/writers/clapeyron_writers/molar_mass.py` & `ugropy-2.0.5/ugropy/writers/clapeyron_writers/molar_mass.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 """Molar mass writer module."""
 
+import pathlib
 from io import StringIO
 from typing import List
 
 import numpy as np
 
 import pandas as pd
 
 from ugropy.fragmentation_models.models import psrk, unifac
 from ugropy.properties.joback_properties import JobackProperties
 
 
 def write_molar_mass(
-    path: str,
+    path: pathlib.Path,
     batch_name: str,
     molecules_names: List[str],
     unifac_groups: List[dict] = [],
     psrk_groups: List[dict] = [],
     joback_objects: List[JobackProperties] = [],
 ) -> None:
     """Create the DataFrame with the molecular weights for Clapeyron.jl.
 
     Parameters
     ----------
-    path : str, optional
+    path : pathlib.Path
         Path to the directory to store de .csv files, by default "./database".
     batch_name : str, optional
         Name of the writing batch. For example, if you name the batch with
         "batch1", the output of the UNIFAC groups will be:
         "batch1_ogUNIFAC_groups.csv". With the default value will be
         "ogUNIFAC_groups.csv", by default "".
     molecules_names : List[str]
@@ -45,14 +46,15 @@
         DataFrame with the molecular weights for Clapeyron.jl
     """
     data_str = (
         "Clapeyron Database File,,\n"
         "Molar Mases Single Params,,\n"
         "species,CAS,Mw\n"
     )
+    path_molar_mass = pathlib.Path(path)
     # =========================================================================
     # Get molecular weights
     # =========================================================================
     if joback_objects:
         molecular_weigths = [j.molecular_weight for j in joback_objects]
     elif unifac_groups:
         df = unifac.subgroups.copy()
@@ -86,19 +88,22 @@
         }
         df.loc[len(df)] = new_row
 
     df.columns = ["" if "Unnamed" in col else col for col in df.columns]
 
     if batch_name == "":
         with open(
-            f"{path}/molarmass.csv", "w", newline="", encoding="utf-8"
+            path_molar_mass / "molarmass.csv",
+            "w",
+            newline="",
+            encoding="utf-8",
         ) as file:
             df.to_csv(file, index=False)
 
     else:
         with open(
-            f"{path}/{batch_name}_molarmass.csv",
+            path_molar_mass / f"{batch_name}_molarmass.csv",
             "w",
             newline="",
             encoding="utf-8",
         ) as file:
             df.to_csv(file, index=False)
```

### Comparing `ugropy-2.0.0/ugropy/writers/clapeyron_writers/psrk_groups.py` & `ugropy-2.0.5/ugropy/writers/clapeyron_writers/psrk_groups.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """PSRK groups writer module."""
 
-import os
+import pathlib
 from typing import List
 
 
 def write_psrk(
-    path: str,
+    path: pathlib.Path,
     batch_name: str,
     molecules_names: List[str],
     psrk_groups: List[dict],
 ) -> None:
     """Create the DataFrame with the PSRK groups for Clapeyron.jl.
 
     Parameters
     ----------
-    path : str, optional
+    path : pathlib.Path
         Path to the directory to store de .csv files, by default "./database".
     batch_name : str, optional
         Name of the writing batch. For example, if you name the batch with
         "batch1", the output of the UNIFAC groups will be:
         "batch1_ogUNIFAC_groups.csv". With the default value will be
         "ogUNIFAC_groups.csv", by default "".
     molecules_names : List[str]
@@ -33,32 +33,34 @@
     """
     lines = [
         "Clapeyron Database File,\n"
         "PSRK Groups [csvtype = groups,grouptype = PSRK]\n"
         "species,groups\n"
     ]
 
+    path_psrk = path / "PSRK"
+
     for name, groups in zip(molecules_names, psrk_groups):
         groups_str = '"['
 
         for group in groups.keys():
             groups_str += f'""{group}"" => {groups[group]}, '
 
         groups_str = groups_str[: len(groups_str) - 2]
         groups_str += ']"\n'
 
         new_line = [f"{name},{groups_str}"]
 
         lines.extend(new_line)
 
     # Create folder for PSRK groups
-    if not os.path.exists(f"{path}/PSRK"):
-        os.makedirs(f"{path}/PSRK")
+    if not path_psrk.is_dir():
+        path_psrk.mkdir(parents=True)
 
     # Write .csv
     if batch_name == "":
-        write_path = f"{path}/PSRK/PSRK_groups.csv"
+        write_path = path_psrk / "PSRK_groups.csv"
     else:
-        write_path = f"{path}/PSRK/{batch_name}_PSRK_groups.csv"
+        write_path = path_psrk / f"{batch_name}_PSRK_groups.csv"
 
-    with open(f"{write_path}", "w", encoding="utf-8", newline="\n") as file:
+    with open(write_path, "w", encoding="utf-8", newline="\n") as file:
         file.writelines(lines)
```

### Comparing `ugropy-2.0.0/ugropy/writers/clapeyron_writers/unifac_groups.py` & `ugropy-2.0.5/ugropy/writers/clapeyron_writers/unifac_groups.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """UNIFAC groups writer module."""
 
-import os
+import pathlib
 from typing import List
 
 
 def write_unifac(
-    path: str,
+    path: pathlib.Path,
     batch_name: str,
     molecules_names: List[str],
     unifac_groups: List[dict],
 ) -> None:
     """Create the DataFrame with the classic LV-UNIFAC groups for Clapeyron.jl.
 
     Parameters
     ----------
-    path : str, optional
+    path : pathlib.Path
         Path to the directory to store de .csv files, by default "./database".
     batch_name : str, optional
         Name of the writing batch. For example, if you name the batch with
         "batch1", the output of the UNIFAC groups will be:
         "batch1_ogUNIFAC_groups.csv". With the default value will be
         "ogUNIFAC_groups.csv", by default "".
     molecules_names : List[str]
@@ -28,32 +28,34 @@
     """
     lines = [
         "Clapeyron Database File,\n"
         "original UNIFAC Groups,[csvtype = groups,grouptype = originalUNIFAC]\n"  # noqa
         "species,groups\n"
     ]
 
+    path_ogunifac = path / "ogUNIFAC"
+
     for name, groups in zip(molecules_names, unifac_groups):
         groups_str = '"['
 
         for group in groups.keys():
             groups_str += f'""{group}"" => {groups[group]}, '
 
         groups_str = groups_str[: len(groups_str) - 2]
         groups_str += ']"\n'
 
         new_line = [f"{name},{groups_str}"]
 
         lines.extend(new_line)
 
     # Create folder for ogUNIFAC groups
-    if not os.path.exists(f"{path}/ogUNIFAC"):
-        os.makedirs(f"{path}/ogUNIFAC")
+    if not path_ogunifac.is_dir():
+        path_ogunifac.mkdir(parents=True)
 
     # Write .csv
     if batch_name == "":
-        write_path = f"{path}/ogUNIFAC/ogUNIFAC_groups.csv"
+        write_path = path_ogunifac / "ogUNIFAC_groups.csv"
     else:
-        write_path = f"{path}/ogUNIFAC/{batch_name}_ogUNIFAC_groups.csv"
+        write_path = path_ogunifac / f"{batch_name}_ogUNIFAC_groups.csv"
 
-    with open(f"{write_path}", "w", encoding="utf-8", newline="\n") as file:
+    with open(write_path, "w", encoding="utf-8", newline="\n") as file:
         file.writelines(lines)
```

### Comparing `ugropy-2.0.0/ugropy/writers/thermo.py` & `ugropy-2.0.5/ugropy/writers/thermo.py`

 * *Files identical despite different names*

### Comparing `ugropy-2.0.0/ugropy.egg-info/PKG-INFO` & `ugropy-2.0.5/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,70 +1,56 @@
-Metadata-Version: 2.1
-Name: ugropy
-Version: 2.0.0
-Summary: Get UNIFAC functional groups of PubChem compounds or SMILES representation.
-Author-email: "Brandolín, Salvador Eduardo" <salvadorebrandolin@mi.unc.edu.ar>
-License: The MIT License
-Project-URL: Homepage, https://github.com/ipqa-research/ugropy
-Keywords: UNIFAC,functional group,thermodynamics,chemical engineering
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy>=1.25.1
-Requires-Dist: pandas>=2.0.3
-Requires-Dist: pubchempy==1.0.4
-Requires-Dist: rdkit==2023.9.5
-
 ![logo](logo.svg)
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ipqa-research/ugropy/main)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://tldrlegal.com/license/mit-license)
 ![Python 3.10+](https://img.shields.io/badge/Python-3.10%2B-blue)
 [![Docs](https://img.shields.io/badge/docs%20-%20green?style=flat&label=Sphinx&link=https%3A%2F%2Fipqa-research.github.io%2Fugropy%2Findex.html)](https://salvadorbrandolin.github.io/ugropy/)
 [![PyPI
 version](https://badge.fury.io/py/ugropy.svg)](https://badge.fury.io/py/ugropy)
 
-`ugropy` is a `Python` library to obtain subgroups from different
-thermodynamic group contribution models using both the name or the SMILES
-representation of a molecule. If the name is given, the library uses the
+`ugropy` is a `Python` library to obtain subgroups from different thermodynamic
+group contribution models using both the name or the SMILES representation of a
+molecule. If the name is given, the library uses the
 [PubChemPy](https://github.com/mcs07/PubChemPy) library to obtain the SMILES
 representation from PubChem. In both cases, `ugropy` uses the
 [RDKit](https://github.com/rdkit/rdkit) library to search the functional groups
 in the molecule.
 
 `ugropy` is in an early development stage, leaving issues of examples of
 molecules that `ugropy` fails solving the subgroups of a model is very helpful.
 
+`ugropy` is tested for `Python` 3.10, 3.11 and 3.12 on Linux, Windows and Mac
+OS.
+
 ## Try ugropy now
 You can try ugropy from its
 [Binder](https://mybinder.org/v2/gh/ipqa-research/ugropy/main). Open the
 binder.ipynb file to explore the basic features.
 
-## Models supported v2.0.0
+## Models supported v2.0.5
 - Classic liquid-vapor UNIFAC
 - Predictive Soave-Redlich-Kwong (PSRK)
 - Joback
 
 ## Writers
+`ugropy` allows you to convert the obtained functional groups or estimated
+properties to the input format required by the following thermodynamic
+libraries:
 
 - [Clapeyron.jl](github.com/ClapeyronThermo/Clapeyron.jl)
 - [Thermo](https://github.com/CalebBell/thermo)
 
 
 ## Example of use
 You can check the full tutorial
 [here](https://ipqa-research.github.io/ugropy/tutorial/tutorial.html).
 
 Get groups from the molecule's name:
 
+
 ```python
 from ugropy import Groups
 
 
 hexane = Groups("hexane")
 
 print(hexane.unifac.subgroups)
@@ -134,15 +120,15 @@
 
 # Write the csv files into a database directory
 writers.to_clapeyron(
     molecules_names=names,
     unifac_groups=[g.unifac.subgroups for g in grps],
     psrk_groups=[g.psrk.subgroups for g in grps],
     joback_objects=[g.joback for g in grps],
-    path="./database"
+    path="database"
 )
 ```
 Obtain the [Caleb Bell's Thermo](https://github.com/CalebBell/thermo) subgroups
 
 ```python
 from ugropy import unifac
 
@@ -157,26 +143,7 @@
 [{1: 2, 2: 4}, {1: 1, 2: 1, 18: 1}]
 ```
 
 ## Installation
 ```
 pip install ugropy
 ```
-
-## Refereces
-
-[1] http://www.ddbst.com/published-parameters-unifac.html
-
-[2] Joback, K. G., & Reid, R. C. (1987). ESTIMATION OF PURE-COMPONENT
-PROPERTIES FROM GROUP-CONTRIBUTIONS. Chemical Engineering Communications,
-57(1–6), 233–243. https://doi.org/10.1080/00986448708960487
-
-[3] Joback, K. G. (1989). Designing molecules possessing desired physical
-property values [Thesis (Ph. D.), Massachusetts Institute of Technology].
-https://dspace.mit.edu/handle/1721.1/14191
-
-[4] Bondi, A. (1966). Estimation of Heat Capacity of Liquids. Industrial &
-Engineering Chemistry Fundamentals, 5(4), 442–449.
-https://doi.org/10.1021/i160020a001
-
-[5] Rowlinson, J. S., & Swinton, F. (2013). Liquids and liquid mixtures:
-Butterworths monographs in chemistry. Butterworth-Heinemann
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ugropy-2.0.0/ugropy.egg-info/SOURCES.txt` & `ugropy-2.0.5/ugropy.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -24,14 +24,19 @@
 ugropy/core/problematics.py
 ugropy/fragmentation_models/__init__.py
 ugropy/fragmentation_models/fragmentation_model.py
 ugropy/fragmentation_models/gibbs_model.py
 ugropy/fragmentation_models/models.py
 ugropy/fragmentation_models/prop_estimator.py
 ugropy/groupscsv/problematic_structures.csv
+ugropy/groupscsv/constantinou_gani/primary/c_g_prymary_subgroups.csv
+ugropy/groupscsv/constantinou_gani/primary/cg_problematics.csv
+ugropy/groupscsv/constantinou_gani/primary/hideouts.csv
+ugropy/groupscsv/constantinou_gani/primary/properties_prymary_contrib.csv
+ugropy/groupscsv/constantinou_gani/secondary/structures.csv
 ugropy/groupscsv/joback/joback_problematics.csv
 ugropy/groupscsv/joback/joback_subgroups.csv
 ugropy/groupscsv/joback/properties_contrib.csv
 ugropy/groupscsv/psrk/hideouts.csv
 ugropy/groupscsv/psrk/psrk_info.csv
 ugropy/groupscsv/psrk/psrk_maingroups.csv
 ugropy/groupscsv/psrk/psrk_subgroups.csv
```

