# Comparing `tmp/dftbplus_step-2024.1.18.tar.gz` & `tmp/dftbplus_step-2024.4.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dftbplus_step-2024.1.18.tar", last modified: Fri Jan 19 00:20:23 2024, max compression
+gzip compressed data, was "dftbplus_step-2024.4.24.tar", last modified: Wed Apr 24 21:58:50 2024, max compression
```

## Comparing `dftbplus_step-2024.1.18.tar` & `dftbplus_step-2024.4.24.tar`

### file list

```diff
@@ -1,116 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 00:20:23.493545 dftbplus_step-2024.1.18/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10727 2024-01-19 00:20:23.493545 dftbplus_step-2024.1.18/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 00:20:23.493545 dftbplus_step-2024.1.18/dftbplus_step/
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/dftbplus_step/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      429 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/dftbplus_step/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-01-19 00:20:23.493545 dftbplus_step-2024.1.18/dftbplus_step/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     8852 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/dftbplus_step/band_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/dftbplus_step/band_structure_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/dftbplus_step/band_structure_step.py
--rw-r--r--   0 runner    (1001) docker     (127)    28893 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/dftbplus_step/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8994 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/dftbplus_step/choose_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/dftbplus_step/choose_parameters_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/dftbplus_step/choose_parameters_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/dftbplus_step/computational_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 00:20:23.477545 dftbplus_step-2024.1.18/dftbplus_step/data/
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/dftbplus_step/data/configuration.txt
--rw-r--r--   0 runner    (1001) docker     (127)   648880 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/dftbplus_step/data/metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/dftbplus_step/data/properties.csv
--rw-r--r--   0 runner    (1001) docker     (127)     7170 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/dftbplus_step/data/references.bib
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/dftbplus_step/data/seamm-dftbplus.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/dftbplus_step/data/spin-constants.json
--rw-r--r--   0 runner    (1001) docker     (127)    14279 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/dftbplus_step/dftbplus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/dftbplus_step/dftbplus_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/dftbplus_step/dftbplus_step.py
--rw-r--r--   0 runner    (1001) docker     (127)    10126 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/dftbplus_step/dos.py
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/dftbplus_step/dos_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/dftbplus_step/dos_step.py
--rw-r--r--   0 runner    (1001) docker     (127)    42556 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/dftbplus_step/energy.py
--rw-r--r--   0 runner    (1001) docker     (127)    14521 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/dftbplus_step/energy_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/dftbplus_step/energy_step.py
--rw-r--r--   0 runner    (1001) docker     (127)    16089 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/dftbplus_step/installer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/dftbplus_step/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/dftbplus_step/optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)     7442 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/dftbplus_step/optimization_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/dftbplus_step/optimization_step.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24108 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/dftbplus_step/slako.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/dftbplus_step/tk_band_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)    10716 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/dftbplus_step/tk_choose_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     6529 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/dftbplus_step/tk_dftbplus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/dftbplus_step/tk_dos.py
--rw-r--r--   0 runner    (1001) docker     (127)     8166 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/dftbplus_step/tk_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/dftbplus_step/tk_optimization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 00:20:23.493545 dftbplus_step-2024.1.18/dftbplus_step.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10727 2024-01-19 00:20:23.000000 dftbplus_step-2024.1.18/dftbplus_step.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-01-19 00:20:23.000000 dftbplus_step-2024.1.18/dftbplus_step.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-19 00:20:23.000000 dftbplus_step-2024.1.18/dftbplus_step.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-01-19 00:20:23.000000 dftbplus_step-2024.1.18/dftbplus_step.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-01-19 00:20:23.000000 dftbplus_step-2024.1.18/dftbplus_step.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-01-19 00:20:23.000000 dftbplus_step-2024.1.18/dftbplus_step.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-19 00:20:08.000000 dftbplus_step-2024.1.18/dftbplus_step.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 00:20:23.481545 dftbplus_step-2024.1.18/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 00:20:23.481545 dftbplus_step-2024.1.18/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    20790 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/docs/_static/SEAMM inverted.png
--rw-r--r--   0 runner    (1001) docker     (127)    17802 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/docs/_static/SEAMM logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    79373 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/docs/_static/molssi_main_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    68255 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/docs/_static/molssi_main_logo_inverted_white.png
--rw-r--r--   0 runner    (1001) docker     (127)    63967 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/docs/_static/molssi_square.png
--rw-r--r--   0 runner    (1001) docker     (127)    32355 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/docs/_static/nsf.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 00:20:23.481545 dftbplus_step-2024.1.18/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     9620 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 00:20:23.481545 dftbplus_step-2024.1.18/docs/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/docs/developer_guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/docs/developer_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/docs/developer_guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/docs/developer_guide/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/docs/developer_guide/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 00:20:23.481545 dftbplus_step-2024.1.18/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/docs/getting_started/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6473 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 00:20:23.481545 dftbplus_step-2024.1.18/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/docs/user_guide/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 00:20:23.481545 dftbplus_step-2024.1.18/docs/user_guide/recipes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 00:20:23.493545 dftbplus_step-2024.1.18/docs/user_guide/recipes/images/
--rw-r--r--   0 runner    (1001) docker     (127)    78707 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/docs/user_guide/recipes/images/recipe_1_extended_from_smiles.png
--rw-r--r--   0 runner    (1001) docker     (127)   237359 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/docs/user_guide/recipes/images/recipe_1_extended_parameters.png
--rw-r--r--   0 runner    (1001) docker     (127)   160565 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/docs/user_guide/recipes/images/recipe_1_extended_submit.png
--rw-r--r--   0 runner    (1001) docker     (127)   191198 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/docs/user_guide/recipes/images/recipe_1_extended_zenodo.png
--rw-r--r--   0 runner    (1001) docker     (127)   322411 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/docs/user_guide/recipes/images/recipe_1_flowchart.png
--rw-r--r--   0 runner    (1001) docker     (127)   215412 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/docs/user_guide/recipes/images/recipe_1_job_page.png
--rw-r--r--   0 runner    (1001) docker     (127)    42596 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/docs/user_guide/recipes/images/recipe_1_jobs.png
--rw-r--r--   0 runner    (1001) docker     (127)   312511 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/docs/user_guide/recipes/images/recipe_1_optimization.png
--rw-r--r--   0 runner    (1001) docker     (127)   552118 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/docs/user_guide/recipes/images/recipe_1_parameters.png
--rw-r--r--   0 runner    (1001) docker     (127)   105143 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/docs/user_guide/recipes/images/recipe_1_run.png
--rw-r--r--   0 runner    (1001) docker     (127)   242410 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/docs/user_guide/recipes/images/recipe_1_water.png
--rw-r--r--   0 runner    (1001) docker     (127)   392560 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/docs/user_guide/recipes/images/recipe_2_bandstructure.png
--rw-r--r--   0 runner    (1001) docker     (127)   255981 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/docs/user_guide/recipes/images/recipe_2_bandstructure_zoomed.png
--rw-r--r--   0 runner    (1001) docker     (127)   248214 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/docs/user_guide/recipes/images/recipe_2_choose.png
--rw-r--r--   0 runner    (1001) docker     (127)   149017 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/docs/user_guide/recipes/images/recipe_2_dftb+_flow.png
--rw-r--r--   0 runner    (1001) docker     (127)    89447 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/docs/user_guide/recipes/images/recipe_2_flowchart.png
--rw-r--r--   0 runner    (1001) docker     (127)    51779 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/docs/user_guide/recipes/images/recipe_2_parameters.png
--rw-r--r--   0 runner    (1001) docker     (127)   244713 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/docs/user_guide/recipes/images/recipe_2_parameters_dialog.png
--rw-r--r--   0 runner    (1001) docker     (127)   148388 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/docs/user_guide/recipes/images/recipe_2_read.png
--rw-r--r--   0 runner    (1001) docker     (127)   193878 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/docs/user_guide/recipes/images/recipe_2_submit.png
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/docs/user_guide/recipes/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    13258 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/docs/user_guide/recipes/recipe_1.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6266 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/docs/user_guide/recipes/recipe_1_extended.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9635 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/docs/user_guide/recipes/recipe_2.rst
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-01-19 00:20:23.493545 dftbplus_step-2024.1.18/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 00:20:23.493545 dftbplus_step-2024.1.18/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/tests/test_dftbplus_step.py
--rw-r--r--   0 runner    (1001) docker     (127)    68611 2024-01-19 00:20:03.000000 dftbplus_step-2024.1.18/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:58:50.851204 dftbplus_step-2024.4.24/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10998 2024-04-24 21:58:50.851204 dftbplus_step-2024.4.24/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:58:50.851204 dftbplus_step-2024.4.24/dftbplus_step/
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/dftbplus_step/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      429 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/dftbplus_step/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-24 21:58:50.851204 dftbplus_step-2024.4.24/dftbplus_step/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8852 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/dftbplus_step/band_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/dftbplus_step/band_structure_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/dftbplus_step/band_structure_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27343 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/dftbplus_step/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8990 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/dftbplus_step/choose_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/dftbplus_step/choose_parameters_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/dftbplus_step/choose_parameters_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/dftbplus_step/computational_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:58:50.839204 dftbplus_step-2024.4.24/dftbplus_step/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/dftbplus_step/data/configuration.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/dftbplus_step/data/dftbplus.ini
+-rw-r--r--   0 runner    (1001) docker     (127)   648880 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/dftbplus_step/data/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/dftbplus_step/data/properties.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     7170 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/dftbplus_step/data/references.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/dftbplus_step/data/seamm-dftbplus.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/dftbplus_step/data/spin-constants.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16220 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/dftbplus_step/dftbplus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/dftbplus_step/dftbplus_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/dftbplus_step/dftbplus_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10122 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/dftbplus_step/dos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/dftbplus_step/dos_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/dftbplus_step/dos_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42548 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/dftbplus_step/energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14521 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/dftbplus_step/energy_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/dftbplus_step/energy_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16387 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/dftbplus_step/installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/dftbplus_step/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/dftbplus_step/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7442 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/dftbplus_step/optimization_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/dftbplus_step/optimization_step.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24108 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/dftbplus_step/slako.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/dftbplus_step/tk_band_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10716 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/dftbplus_step/tk_choose_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6529 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/dftbplus_step/tk_dftbplus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/dftbplus_step/tk_dos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8166 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/dftbplus_step/tk_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/dftbplus_step/tk_optimization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:58:50.851204 dftbplus_step-2024.4.24/dftbplus_step.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10998 2024-04-24 21:58:50.000000 dftbplus_step-2024.4.24/dftbplus_step.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-04-24 21:58:50.000000 dftbplus_step-2024.4.24/dftbplus_step.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 21:58:50.000000 dftbplus_step-2024.4.24/dftbplus_step.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-24 21:58:50.000000 dftbplus_step-2024.4.24/dftbplus_step.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-24 21:58:50.000000 dftbplus_step-2024.4.24/dftbplus_step.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-24 21:58:50.000000 dftbplus_step-2024.4.24/dftbplus_step.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 21:58:40.000000 dftbplus_step-2024.4.24/dftbplus_step.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:58:50.839204 dftbplus_step-2024.4.24/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:58:50.839204 dftbplus_step-2024.4.24/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    20790 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/docs/_static/SEAMM inverted.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17802 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/docs/_static/SEAMM logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    79373 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/docs/_static/molssi_main_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    68255 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/docs/_static/molssi_main_logo_inverted_white.png
+-rw-r--r--   0 runner    (1001) docker     (127)    63967 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/docs/_static/molssi_square.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32355 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/docs/_static/nsf.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:58:50.839204 dftbplus_step-2024.4.24/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9620 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:58:50.843204 dftbplus_step-2024.4.24/docs/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/docs/developer_guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/docs/developer_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/docs/developer_guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/docs/developer_guide/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/docs/developer_guide/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:58:50.843204 dftbplus_step-2024.4.24/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/docs/getting_started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6473 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:58:50.843204 dftbplus_step-2024.4.24/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/docs/user_guide/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:58:50.843204 dftbplus_step-2024.4.24/docs/user_guide/recipes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:58:50.851204 dftbplus_step-2024.4.24/docs/user_guide/recipes/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    78707 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/docs/user_guide/recipes/images/recipe_1_extended_from_smiles.png
+-rw-r--r--   0 runner    (1001) docker     (127)   237359 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/docs/user_guide/recipes/images/recipe_1_extended_parameters.png
+-rw-r--r--   0 runner    (1001) docker     (127)   160565 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/docs/user_guide/recipes/images/recipe_1_extended_submit.png
+-rw-r--r--   0 runner    (1001) docker     (127)   191198 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/docs/user_guide/recipes/images/recipe_1_extended_zenodo.png
+-rw-r--r--   0 runner    (1001) docker     (127)   322411 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/docs/user_guide/recipes/images/recipe_1_flowchart.png
+-rw-r--r--   0 runner    (1001) docker     (127)   215412 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/docs/user_guide/recipes/images/recipe_1_job_page.png
+-rw-r--r--   0 runner    (1001) docker     (127)    42596 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/docs/user_guide/recipes/images/recipe_1_jobs.png
+-rw-r--r--   0 runner    (1001) docker     (127)   312511 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/docs/user_guide/recipes/images/recipe_1_optimization.png
+-rw-r--r--   0 runner    (1001) docker     (127)   552118 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/docs/user_guide/recipes/images/recipe_1_parameters.png
+-rw-r--r--   0 runner    (1001) docker     (127)   105143 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/docs/user_guide/recipes/images/recipe_1_run.png
+-rw-r--r--   0 runner    (1001) docker     (127)   242410 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/docs/user_guide/recipes/images/recipe_1_water.png
+-rw-r--r--   0 runner    (1001) docker     (127)   392560 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/docs/user_guide/recipes/images/recipe_2_bandstructure.png
+-rw-r--r--   0 runner    (1001) docker     (127)   255981 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/docs/user_guide/recipes/images/recipe_2_bandstructure_zoomed.png
+-rw-r--r--   0 runner    (1001) docker     (127)   248214 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/docs/user_guide/recipes/images/recipe_2_choose.png
+-rw-r--r--   0 runner    (1001) docker     (127)   149017 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/docs/user_guide/recipes/images/recipe_2_dftb+_flow.png
+-rw-r--r--   0 runner    (1001) docker     (127)    89447 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/docs/user_guide/recipes/images/recipe_2_flowchart.png
+-rw-r--r--   0 runner    (1001) docker     (127)    51779 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/docs/user_guide/recipes/images/recipe_2_parameters.png
+-rw-r--r--   0 runner    (1001) docker     (127)   244713 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/docs/user_guide/recipes/images/recipe_2_parameters_dialog.png
+-rw-r--r--   0 runner    (1001) docker     (127)   148388 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/docs/user_guide/recipes/images/recipe_2_read.png
+-rw-r--r--   0 runner    (1001) docker     (127)   193878 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/docs/user_guide/recipes/images/recipe_2_submit.png
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/docs/user_guide/recipes/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    13258 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/docs/user_guide/recipes/recipe_1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6266 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/docs/user_guide/recipes/recipe_1_extended.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9635 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/docs/user_guide/recipes/recipe_2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-24 21:58:50.851204 dftbplus_step-2024.4.24/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:58:50.851204 dftbplus_step-2024.4.24/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/tests/test_dftbplus_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68610 2024-04-24 21:58:37.000000 dftbplus_step-2024.4.24/versioneer.py
```

### Comparing `dftbplus_step-2024.1.18/CONTRIBUTING.rst` & `dftbplus_step-2024.4.24/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/HISTORY.rst` & `dftbplus_step-2024.4.24/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 =======
 History
 =======
+2024.4.24 -- Finalized support for Docker containers
+    * Fixed issues and tested running in containers.
+    * Add CI to make a Docker image for DFTB+
+    * Fixed issue with changes in input for DFTB+: CalculateGradients has become
+      PrintGradients it seems.
+      
 2024.1.18 -- Support for running in containers and writing input only.
     * Added new property: scaled dipole.
     * Added option to write the input file and not run DFTB+
 
 2023.11.10 -- Standard structure handling and cleaned up output
     * Switched to standard structure handling and naming, giving consistent options
       across SEAMM.
```

### Comparing `dftbplus_step-2024.1.18/LICENSE` & `dftbplus_step-2024.4.24/LICENSE`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/PKG-INFO` & `dftbplus_step-2024.4.24/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dftbplus_step
-Version: 2024.1.18
+Version: 2024.4.24
 Summary: A SEAMM plug-in for DFTB+, a fast quantum mechanical simulation code.
 Home-page: https://github.com/molssi-seamm/dftbplus_step
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,plug-in,flowchart,quantum,simulation,atomistic,DFTB+,DFTBplus,tight-binding,DFT
 Platform: Linux
@@ -106,14 +106,20 @@
 .. _`molssi-seamm/cookiecutter-seamm-plugin`: https://github.com/molssi-seamm/cookiecutter-seamm-plugin
 .. _MolSSI: https://molssi.org
 
 
 =======
 History
 =======
+2024.4.24 -- Finalized support for Docker containers
+    * Fixed issues and tested running in containers.
+    * Add CI to make a Docker image for DFTB+
+    * Fixed issue with changes in input for DFTB+: CalculateGradients has become
+      PrintGradients it seems.
+      
 2024.1.18 -- Support for running in containers and writing input only.
     * Added new property: scaled dipole.
     * Added option to write the input file and not run DFTB+
 
 2023.11.10 -- Standard structure handling and cleaned up output
     * Switched to standard structure handling and naming, giving consistent options
       across SEAMM.
```

### Comparing `dftbplus_step-2024.1.18/README.rst` & `dftbplus_step-2024.4.24/README.rst`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/dftbplus_step/__init__.py` & `dftbplus_step-2024.4.24/dftbplus_step/__init__.py`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/dftbplus_step/band_structure.py` & `dftbplus_step-2024.4.24/dftbplus_step/band_structure.py`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/dftbplus_step/band_structure_parameters.py` & `dftbplus_step-2024.4.24/dftbplus_step/band_structure_parameters.py`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/dftbplus_step/band_structure_step.py` & `dftbplus_step-2024.4.24/dftbplus_step/band_structure_step.py`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/dftbplus_step/base.py` & `dftbplus_step-2024.4.24/dftbplus_step/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -103,14 +103,19 @@
         """The model (chemistry) used to obtain results."""
         return self.parent.model
 
     @model.setter
     def model(self, value):
         self.parent.model = value
 
+    @property
+    def exe_config(self):
+        """The configuration for the DFTB+ executable."""
+        return self.parent.exe_config
+
     def band_structure(
         self, input_path, sym_points, sym_names, Efermi=[0.0, 0.0], DOS=None
     ):
         """Prepare the graph for the band structure.
 
         Parameters
         ----------
@@ -154,30 +159,23 @@
 
         # Read configuration file for DFTB+
         ini_dir = Path(seamm_options["root"]).expanduser()
         full_config = configparser.ConfigParser()
         full_config.read(ini_dir / "dftbplus.ini")
 
         executor = self.parent.flowchart.executor
-        executor_type = executor.name
-        if executor_type not in full_config:
-            raise RuntimeError(
-                f"No section for '{executor_type}' in DFTB+ ini file "
-                f"({ini_dir / 'dftbplus.ini'})"
-            )
-        config = dict(full_config.items(executor_type))
 
         if spin_polarized:
             cmd = ["dp_bands", "-s", input_path, "band"]
         else:
             cmd = ["dp_bands", input_path, "band"]
 
         result = executor.run(
             cmd=cmd,
-            config=config,
+            config=self.exe_config,
             directory=self.directory,
             files={},
             return_files=["*"],
             in_situ=True,
             shell=True,
         )
 
@@ -267,42 +265,24 @@
         if spin_polarized and Efermi[0] != Efermi[1]:
             raise NotImplementedError(
                 f"Cannot handle different Fermi energies yet: {Efermi}"
             )
 
         logger.info("Preparing DOS")
 
-        seamm_options = self.parent.global_options
-
         # Total DOS
         executor = self.parent.flowchart.executor
 
-        # Read configuration file for DFTB+
-        ini_dir = Path(seamm_options["root"]).expanduser()
-        full_config = configparser.ConfigParser()
-        full_config.read(ini_dir / "dftbplus.ini")
-        executor_type = executor.name
-        if executor_type not in full_config:
-            raise RuntimeError(
-                f"No section for '{executor_type}' in DFTB+ ini file "
-                f"({ini_dir / 'dftbplus.ini'})"
-            )
-        config = dict(full_config.items(executor_type))
-
         result = executor.run(
             cmd=[
                 "dp_dos",
                 str(input_path),
                 "dos_total.dat",
-                ">",
-                "DOS.out",
-                "2>",
-                "dos_stderr.txt",
             ],
-            config=config,
+            config=self.exe_config,
             directory=self.directory,
             files={},
             return_files=["*"],
             in_situ=True,
             shell=True,
         )
 
@@ -365,20 +345,16 @@
 
                 result = executor.run(
                     cmd=[
                         "dp_dos",
                         "-w",
                         str(path),
                         str(out),
-                        ">",
-                        "DOS.out",
-                        "2>",
-                        "dos_stderr.txt",
                     ],
-                    config=config,
+                    config=self.exe_config,
                     directory=self.directory,
                     files={},
                     return_files=["*"],
                     in_situ=True,
                     shell=True,
                 )
 
@@ -784,43 +760,31 @@
                     "dftb_pin.hsd",
                     "geom.out.*",
                     "output",
                     "pdos*",
                     "results.tag",
                     "*.xml",
                     "eigenvec.bin",
-                ]  # yapf: disable
+                ]
 
                 # Run the calculation
                 executor = self.parent.flowchart.executor
 
-                # Read configuration file for DFTB+
-                ini_dir = Path(seamm_options["root"]).expanduser()
-                full_config = configparser.ConfigParser()
-                full_config.read(ini_dir / "dftbplus.ini")
-                executor_type = executor.name
-                if executor_type not in full_config:
-                    raise RuntimeError(
-                        f"No section for '{executor_type}' in DFTB+ ini file "
-                        f"({ini_dir / 'dftbplus.ini'})"
-                    )
-                config = dict(full_config.items(executor_type))
-
                 result = executor.run(
                     cmd=["{code}", ">", "DFTB+.out", "2>", "stderr.txt"],
-                    config=config,
+                    config=self.exe_config,
                     directory=self.directory,
                     files=files,
                     return_files=return_files,
                     in_situ=True,
                     shell=True,
                     env=env,
                 )
 
-                if result is None:
+                if not result:
                     logger.error("There was an error running DFTB+")
                     return None
 
                 logger.debug("\n" + pprint.pformat(result))
 
         if not P["input only"]:
             # Parse the results.tag file
```

### Comparing `dftbplus_step-2024.1.18/dftbplus_step/choose_parameters.py` & `dftbplus_step-2024.4.24/dftbplus_step/choose_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         return self.header + "\n" + __(text, indent=4 * " ").__str__()
 
     def get_input(self):
         """Get the input for the Slater-Koster parameters for DFTB+"""
 
         # Get the metadata for the Slater-Koster parameters
         metadata = self.parent._metadata
-        slako_dir = Path(self.parent.options["slako_dir"]).expanduser()
+        slako_dir = Path(self.exe_config["slako-dir"]).expanduser()
 
         # Create the directory
         directory = Path(self.directory)
         directory.mkdir(parents=True, exist_ok=True)
 
         P = self.parameters.current_values_to_dict(
             context=seamm.flowchart_variables._data
```

### Comparing `dftbplus_step-2024.1.18/dftbplus_step/choose_parameters_parameters.py` & `dftbplus_step-2024.4.24/dftbplus_step/choose_parameters_parameters.py`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/dftbplus_step/choose_parameters_step.py` & `dftbplus_step-2024.4.24/dftbplus_step/choose_parameters_step.py`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/dftbplus_step/computational_models.py` & `dftbplus_step-2024.4.24/dftbplus_step/computational_models.py`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/dftbplus_step/data/metadata.json` & `dftbplus_step-2024.4.24/dftbplus_step/data/metadata.json`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/dftbplus_step/data/references.bib` & `dftbplus_step-2024.4.24/dftbplus_step/data/references.bib`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/dftbplus_step/data/spin-constants.json` & `dftbplus_step-2024.4.24/dftbplus_step/data/spin-constants.json`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/dftbplus_step/dftbplus.py` & `dftbplus_step-2024.4.24/dftbplus_step/dftbplus.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 # -*- coding: utf-8 -*-
 
 """Non-graphical part of the DFTB+ step in a SEAMM flowchart
 """
 
 import collections.abc
-
-try:
-    import importlib.metadata as implib
-except Exception:
-    import importlib_metadata as implib
+import configparser
+import importlib
 import json
 import logging
 from pathlib import Path
-import pkg_resources
 import pprint  # noqa: F401
+import shutil
 import sys
 
 import molsystem
 import dftbplus_step
 import seamm
 import seamm_util
 import seamm_util.printing as printing
@@ -32,16 +29,16 @@
 # directory, and is used for all normal output from this step.
 
 logger = logging.getLogger(__name__)
 job = printing.getPrinter()
 printer = printing.getPrinter("DFTB+")
 
 # Add DFTB+'s properties to the standard properties
-path = Path(pkg_resources.resource_filename(__name__, "data/"))
-csv_file = path / "properties.csv"
+resources = importlib.resources.files("dftbplus_step") / "data"
+csv_file = resources / "properties.csv"
 molsystem.add_properties_from_file(csv_file)
 
 
 def deep_merge(d, u):
     """Do a deep merge of one dict into another.
 
     This will update d with values in u, but will not delete keys in d
@@ -234,22 +231,23 @@
             module=__name__,
             logger=logger,
         )
 
         self.parameters = dftbplus_step.DftbplusParameters()
 
         # Get the metadata for the Slater-Koster parameters
-        package = self.__module__.split(".")[0]
-        files = [p for p in implib.files(package) if p.name == "metadata.json"]
-        if len(files) != 1:
+        resources = importlib.resources.files("dftbplus_step") / "data"
+        path = resources / "metadata.json"
+        if not path.exists():
             raise RuntimeError("Can't find Slater-Koster metadata.json file")
-        data = files[0].read_text()
+        data = path.read_text()
         self._metadata = json.loads(data)
 
         # Data to pass between substeps
+        self._exe_config = None
         self._dataset = None  # SLAKO dataset used
         self._subset = None  # SLAKO modifier dataset applied to dataset
         self._reference_energies = None  # Reference energies per element.
         self._reference_energy = None  # for calculating energy of formation
         self._steps = None  # The nodes for the steps run so far.
 
     @property
@@ -258,14 +256,20 @@
         return dftbplus_step.__version__
 
     @property
     def git_revision(self):
         """The git version of this module."""
         return dftbplus_step.__git_revision__
 
+    @property
+    def exe_config(self):
+        if self._exe_config is None:
+            self.get_exe_config()
+        return self._exe_config
+
     def create_parser(self):
         """Setup the command-line / config file parser"""
         # parser_name = 'dftbplus-step'
         parser_name = self.step_type
         parser = seamm_util.getParser(name="SEAMM")
 
         # Remember if the parser exists ... this type of step may have been
@@ -472,7 +476,52 @@
             for value in node.description:
                 printer.important(value)
                 printer.important(" ")
 
             node.analyze(data=data)
 
             node = node.next()
+
+    def get_exe_config(self):
+        """Read the `dftbplus.ini` file, creating if necessary."""
+        executor = self.flowchart.executor
+
+        # Read configuration file for DFTB+ if it exists
+        executor_type = executor.name
+        full_config = configparser.ConfigParser()
+        ini_dir = Path(self.global_options["root"]).expanduser()
+        path = ini_dir / "dftbplus.ini"
+
+        if path.exists():
+            full_config.read(ini_dir / "dftbplus.ini")
+
+        # If the section we need doesn't exists, get the default
+        if not path.exists() or executor_type not in full_config:
+            resources = importlib.resources.files("dftbplus_step") / "data"
+            ini_text = (resources / "dftbplus.ini").read_text()
+            full_config.read_string(ini_text)
+
+        # Getting desperate! Look for an executable in the path
+        if executor_type not in full_config:
+            path = shutil.which("dftbplus")
+            if path is None:
+                raise RuntimeError(
+                    f"No section for '{executor_type}' in DFTB+ ini file "
+                    f"({ini_dir / 'dftbplus.ini'}), nor in the defaults, nor "
+                    "in the path!"
+                )
+            else:
+                full_config[executor_type] = {
+                    "installation": "local",
+                    "code": str(path),
+                }
+
+        # If the ini file does not exist, write it out!
+        if not path.exists():
+            with path.open("w") as fd:
+                full_config.write(fd)
+            printer.normal(f"Wrote the DFTB+ configuration file to {path}")
+            printer.normal("")
+
+        self._exe_config = dict(full_config.items(executor_type))
+        # Use the matching version of the seamm-dftbplus image by default.
+        self._exe_config["version"] = self.version
```

### Comparing `dftbplus_step-2024.1.18/dftbplus_step/dftbplus_parameters.py` & `dftbplus_step-2024.4.24/dftbplus_step/dftbplus_parameters.py`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/dftbplus_step/dftbplus_step.py` & `dftbplus_step-2024.4.24/dftbplus_step/dftbplus_step.py`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/dftbplus_step/dos.py` & `dftbplus_step-2024.4.24/dftbplus_step/dos.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,15 +163,15 @@
         if "InitialCharges" in dftb:
             del dftb["InitialCharges"]
 
         # Set up for atom based DOS
         if "Analysis" not in energy_in:
             energy_in["Analysis"] = {}
         analysis = energy_in["Analysis"]
-        analysis["CalculateForces"] = "No"
+        analysis["PrintForces"] = "No"
 
         elements = set(configuration.atoms.symbols)
         elements = sorted([*elements])
         dos = {}
         n = 0
         for element in elements:
             n += 1
```

### Comparing `dftbplus_step-2024.1.18/dftbplus_step/dos_parameters.py` & `dftbplus_step-2024.4.24/dftbplus_step/dos_parameters.py`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/dftbplus_step/dos_step.py` & `dftbplus_step-2024.4.24/dftbplus_step/dos_step.py`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/dftbplus_step/energy.py` & `dftbplus_step-2024.4.24/dftbplus_step/energy.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,23 +205,23 @@
         model, parameter_set_name = parameter_set.split("/", 1)
 
         # Main control of the Hamiltonian
         if model == "DFTB":
             # template
             result = {
                 "Analysis": {
-                    "CalculateForces": "Yes",
+                    "PrintForces": "Yes",
                 },
                 "Hamiltonian": {"DFTB": {}},
             }
             hamiltonian = result["Hamiltonian"]["DFTB"]
         else:
             result = {
                 "Analysis": {
-                    "CalculateForces": "Yes",
+                    "PrintForces": "Yes",
                 },
                 "Hamiltonian": {"xTB": {}},
             }
             hamiltonian = result["Hamiltonian"]["xTB"]
 
         # Basic parameters
         hamiltonian["SCC"] = P["SCC"]
```

### Comparing `dftbplus_step-2024.1.18/dftbplus_step/energy_parameters.py` & `dftbplus_step-2024.4.24/dftbplus_step/energy_parameters.py`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/dftbplus_step/energy_step.py` & `dftbplus_step-2024.4.24/dftbplus_step/energy_step.py`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/dftbplus_step/installer.py` & `dftbplus_step-2024.4.24/dftbplus_step/installer.py`

 * *Files 26% similar despite different names*

```diff
@@ -23,66 +23,58 @@
 
 class Installer(seamm_installer.InstallerBase):
     """Handle further installation needed after installing dftbplus-step.
 
     The Python package `dftbplus-step` should already be installed, using `pip`,
     `conda`, or similar. This plug-in-specific installer then checks for the
     Dftbplus executable, installing it if needed, and registers its
-    location in seamm.ini.
+    location in ~/SEAMM/dftbplus.ini.
 
     There are a number of ways to determine which are the correct Dftbplus
     executables to use. The aim of this installer is to help the user locate
     the executables. There are a number of possibilities:
 
     1. The correct executables are already available.
 
-        1. If they are already registered in `seamm.ini` there is nothing else
+        1. If they are already registered in `dftbplus.ini` there is nothing else
            to do.
         2. They may be in the current path, in which case they need to be added
-           to `seamm.ini`.
+           to `dftbplus.ini`.
         3. If a module system is in use, a module may need to be loaded to give
            access to Dftbplus.
         4. They cannot be found automatically, so the user needs to locate the
            executables for the installer.
 
     2. Dftbplus is not installed on the machine. In this case they can be
        installed in a Conda environment. There is one choice:
 
         1. They can be installed in a separate environment, `seamm-dftbplus` by
            default.
 
     The Slater-Koster potentials also need to be installed if not present. They are
-    placed in ~/SEAMM/Parameters/slako by default.
+    placed in ~/SEAMM/Parameters/slako or, in containers, ~/Parameters/slako by default.
+    The code uses those in ~/Parameters before those in ~/SEAMM/Parameters.
     """
 
     def __init__(self, logger=logger):
         # Call the base class initialization, which sets up the commandline
         # parser, amongst other things.
         super().__init__(logger=logger)
 
         logger.debug("Initializing the Dftbplus installer object.")
 
         self.section = "dftbplus-step"
-        self.path_name = "dftbplus-path"
         self.executables = ["dftb+"]
         self.resource_path = Path(pkg_resources.resource_filename(__name__, "data/"))
 
         self.slako_url = "https://dftb.org/fileadmin/DFTB/public/slako-unpacked.tar.xz"
 
-        # What Conda environment is the default?
-        data = self.configuration.get_values(self.section)
-        if "conda-environment" in data and data["conda-environment"] != "":
-            self.environment = data["conda-environment"]
-        else:
-            self.environment = "seamm-dftbplus"
-
         # The environment.yaml file for Conda installations.
-        path = Path(pkg_resources.resource_filename(__name__, "data/"))
-        logger.debug(f"data directory: {path}")
-        self.environment_file = path / "seamm-dftbplus.yml"
+        logger.debug(f"data directory: {self.resource_path}")
+        self.environment_file = self.resource_path / "seamm-dftbplus.yml"
 
     def check(self):
         """Check the installation and fix errors if requested.
 
         If the option `yes` is present and True, this method will attempt to
         correct any errors in the configuration file. Use `--yes` on the
         command line to enable this.
@@ -106,29 +98,48 @@
 
         Returns
         -------
         bool
             True if everything is OK, False otherwise. If `yes` is given as an
             option, the return value is after fixing the configuration.
         """
+        print("Checking the DFTB+ installation.")
+
+        # What Conda environment is the default?
+        path = self.configuration.path.parent / "dftbplus.ini"
+        if not path.exists():
+            text = (self.resource_path / "dftbplus.ini").read_text()
+            path.write_text(text)
+            print(f"    The dftbplus.ini file did not exist. Created {path}")
+
+        self.exe_config.path = path
+
+        # Get the current values
+        data = self.exe_config.get_values("local")
+
+        if "conda-environment" in data and data["conda-environment"] != "":
+            self.environment = data["conda-environment"]
+        else:
+            self.environment = "seamm-dftbplus"
+
         # Check the DFTB+ executable
         result = super().check()
 
         # And the Slater-Koster parameter files.
-        self.logger.debug("Checking the Slater-Koster parameters.")
+        print("    Checking the Slater-Koster parameters.")
 
         # First read in the configuration file in the normal fashion
         # to get the root directory (~/SEAMM usually), which may be needed.
         parser = seamm_util.seamm_parser()
         parser.parse_args([])
         options = parser.get_options("SEAMM")
         root = Path(options["root"]).expanduser().resolve()
 
         # Get the values from the configuration
-        data = self.configuration.get_values(self.section)
+        data = self.exe_config.get_values("local")
         if "slako-dir" in data and data["slako-dir"] != "":
             tmp = data["slako-dir"].replace("${root:SEAMM}", str(root))
             slako_dir = Path(tmp).expanduser().resolve()
             have_key = True
         else:
             slako_dir = root / "Parameters" / "slako"
             have_key = False
@@ -161,31 +172,29 @@
             if not have_key:
                 if self.options.yes or self.ask_yes_no(
                     f"The location of the Slater-Koster files, '{slako_dir}', is not "
                     "registered in the configuration file.\nDo you want to correct "
                     "this?",
                     default="yes",
                 ):
-                    self.configuration.set_value(
-                        self.section, "slako-dir", str(slako_dir)
-                    )
-                    self.configuration.save()
+                    self.exe_config.set_value("local", "slako-dir", str(slako_dir))
+                    self.exe_config.save()
 
         if install == "check contents":
             # How do we do this? Check files, versions, what?
             print(
                 "At this time, this install is not able  to check the individual files"
                 "\nto see if they are up-to-date or not. Updating currently forces an "
                 "update."
             )
         elif install == "full":
             self.install_files(slako_dir)
-            self.configuration.set_value(self.section, "slako-dir", str(slako_dir))
-            self.configuration.save()
-            print("Done!\n")
+            self.exe_config.set_value("local", "slako-dir", str(slako_dir))
+            self.exe_config.save()
+            print("    Done!\n")
         else:
             result = False
 
         return result
 
     def exe_version(self, path):
         """Get the version of the Dftbplus executable.
@@ -277,27 +286,27 @@
         # to get the root directory (~/SEAMM usually), which may be needed.
         parser = seamm_util.seamm_parser()
         parser.parse_args([])
         options = parser.get_options("SEAMM")
         root = Path(options["root"]).expanduser().resolve()
 
         # Get the values from the configuration
-        data = self.configuration.get_values(self.section)
+        data = self.exe_config.get_values("local")
         if "slako-dir" in data and data["slako-dir"] != "":
             tmp = data["slako-dir"].replace("${root:SEAMM}", str(root))
             slako_dir = Path(tmp).expanduser().resolve()
         else:
             slako_dir = root / "Parameters" / "slako"
 
         print(f"Installing the Slater-Koster files to {slako_dir}.")
         slako_dir.parent.mkdir(parents=True, exist_ok=True)
         self.install_files(slako_dir)
 
-        self.configuration.set_value(self.section, "slako-dir", str(slako_dir))
-        self.configuration.save()
+        self.exe_config.set_value("local", "slako-dir", str(slako_dir))
+        self.exe_config.save()
 
         print("Done!\n")
 
     def uninstall(self):
         """Uninstall DFTB+ and the Slater-Koster files
 
         The base class handles the DFTB+ executable, ensuring that the following
@@ -320,15 +329,15 @@
         # Uninstall the DFTB+ executable
         super().uninstall()
 
         # And the Slater-Koster parameter files.
         self.logger.debug("Uninstalling the Slater-Koster parameters.")
 
         # Get the values from the configuration
-        data = self.configuration.get_values(self.section)
+        data = self.exe_config.get_values("local")
         if "slako-dir" in data and data["slako-dir"] != "":
             # First read in the configuration file in the normal fashion
             # to get the root directory (~/SEAMM usually), which may be needed.
             parser = seamm_util.seamm_parser()
             parser.parse_args([])
             options = parser.get_options("SEAMM")
             root = Path(options["root"]).expanduser().resolve()
@@ -337,16 +346,16 @@
             slako_dir = Path(tmp).expanduser().resolve()
 
             print(f"Deleting the Slater-Koster files in {slako_dir}.")
             print(f"{data['slako-dir']=}")
 
             shutil.rmtree(slako_dir, ignore_errors=True)
 
-            self.configuration.set_value(self.section, "slako-dir", "")
-            self.configuration.save()
+            self.exe_config.set_value("local", "slako-dir", "")
+            self.exe_config.save()
             print("Done!\n")
         else:
             print("The Slater-Koster files were not installed, so nothing to do.")
 
     def update(self):
         """Update DFTB+ and the Slater-Koster files
 
@@ -369,15 +378,15 @@
         # Update the DFTB+ executable
         super().update()
 
         # And the Slater-Koster parameter files.
         self.logger.debug("Updating the Slater-Koster parameters.")
 
         # Get the values from the configuration
-        data = self.configuration.get_values(self.section)
+        data = self.exe_config.get_values("local")
         if "slako-dir" in data and data["slako-dir"] != "":
             # First read in the configuration file in the normal fashion
             # to get the root directory (~/SEAMM usually), which may be needed.
             parser = seamm_util.seamm_parser()
             parser.parse_args([])
             options = parser.get_options("SEAMM")
             root = Path(options["root"]).expanduser().resolve()
@@ -387,16 +396,16 @@
 
             if not slako_dir.exists():
                 print(
                     f"The Slater-Koster files are not installed at {slako_dir}, "
                     "\nwhere the configuration file indicates they should be."
                     "\nFixing the configuration file."
                 )
-                self.configuration.set_value(self.section, "slako-dir", "")
-                self.configuration.save()
+                self.exe_config.set_value("local", "slako-dir", "")
+                self.exe_config.save()
             else:
                 print(f"Updating the Slater-Koster files in {slako_dir}.")
                 slako_dir.parent.mkdir(parents=True, exist_ok=True)
                 self.install_files(slako_dir)
 
             print("Done!\n")
         else:
```

### Comparing `dftbplus_step-2024.1.18/dftbplus_step/metadata.py` & `dftbplus_step-2024.4.24/dftbplus_step/metadata.py`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/dftbplus_step/optimization.py` & `dftbplus_step-2024.4.24/dftbplus_step/optimization.py`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/dftbplus_step/optimization_parameters.py` & `dftbplus_step-2024.4.24/dftbplus_step/optimization_parameters.py`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/dftbplus_step/optimization_step.py` & `dftbplus_step-2024.4.24/dftbplus_step/optimization_step.py`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/dftbplus_step/slako.py` & `dftbplus_step-2024.4.24/dftbplus_step/slako.py`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/dftbplus_step/tk_band_structure.py` & `dftbplus_step-2024.4.24/dftbplus_step/tk_band_structure.py`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/dftbplus_step/tk_choose_parameters.py` & `dftbplus_step-2024.4.24/dftbplus_step/tk_choose_parameters.py`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/dftbplus_step/tk_dftbplus.py` & `dftbplus_step-2024.4.24/dftbplus_step/tk_dftbplus.py`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/dftbplus_step/tk_dos.py` & `dftbplus_step-2024.4.24/dftbplus_step/tk_dos.py`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/dftbplus_step/tk_energy.py` & `dftbplus_step-2024.4.24/dftbplus_step/tk_energy.py`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/dftbplus_step/tk_optimization.py` & `dftbplus_step-2024.4.24/dftbplus_step/tk_optimization.py`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/dftbplus_step.egg-info/PKG-INFO` & `dftbplus_step-2024.4.24/dftbplus_step.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dftbplus_step
-Version: 2024.1.18
+Version: 2024.4.24
 Summary: A SEAMM plug-in for DFTB+, a fast quantum mechanical simulation code.
 Home-page: https://github.com/molssi-seamm/dftbplus_step
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,plug-in,flowchart,quantum,simulation,atomistic,DFTB+,DFTBplus,tight-binding,DFT
 Platform: Linux
@@ -106,14 +106,20 @@
 .. _`molssi-seamm/cookiecutter-seamm-plugin`: https://github.com/molssi-seamm/cookiecutter-seamm-plugin
 .. _MolSSI: https://molssi.org
 
 
 =======
 History
 =======
+2024.4.24 -- Finalized support for Docker containers
+    * Fixed issues and tested running in containers.
+    * Add CI to make a Docker image for DFTB+
+    * Fixed issue with changes in input for DFTB+: CalculateGradients has become
+      PrintGradients it seems.
+      
 2024.1.18 -- Support for running in containers and writing input only.
     * Added new property: scaled dipole.
     * Added option to write the input file and not run DFTB+
 
 2023.11.10 -- Standard structure handling and cleaned up output
     * Switched to standard structure handling and naming, giving consistent options
       across SEAMM.
```

### Comparing `dftbplus_step-2024.1.18/dftbplus_step.egg-info/SOURCES.txt` & `dftbplus_step-2024.4.24/dftbplus_step.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 dftbplus_step.egg-info/SOURCES.txt
 dftbplus_step.egg-info/dependency_links.txt
 dftbplus_step.egg-info/entry_points.txt
 dftbplus_step.egg-info/requires.txt
 dftbplus_step.egg-info/top_level.txt
 dftbplus_step.egg-info/zip-safe
 dftbplus_step/data/configuration.txt
+dftbplus_step/data/dftbplus.ini
 dftbplus_step/data/metadata.json
 dftbplus_step/data/properties.csv
 dftbplus_step/data/references.bib
 dftbplus_step/data/seamm-dftbplus.yml
 dftbplus_step/data/spin-constants.json
 docs/Makefile
 docs/authors.rst
```

### Comparing `dftbplus_step-2024.1.18/dftbplus_step.egg-info/entry_points.txt` & `dftbplus_step-2024.4.24/dftbplus_step.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/docs/Makefile` & `dftbplus_step-2024.4.24/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/docs/_static/SEAMM inverted.png` & `dftbplus_step-2024.4.24/docs/_static/SEAMM inverted.png`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/docs/_static/SEAMM logo.png` & `dftbplus_step-2024.4.24/docs/_static/SEAMM logo.png`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/docs/_static/molssi_main_logo.png` & `dftbplus_step-2024.4.24/docs/_static/molssi_main_logo.png`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/docs/_static/molssi_main_logo_inverted_white.png` & `dftbplus_step-2024.4.24/docs/_static/molssi_main_logo_inverted_white.png`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/docs/_static/molssi_square.png` & `dftbplus_step-2024.4.24/docs/_static/molssi_square.png`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/docs/_static/nsf.png` & `dftbplus_step-2024.4.24/docs/_static/nsf.png`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/docs/conf.py` & `dftbplus_step-2024.4.24/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/docs/developer_guide/installation.rst` & `dftbplus_step-2024.4.24/docs/developer_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/docs/getting_started/index.rst` & `dftbplus_step-2024.4.24/docs/getting_started/index.rst`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/docs/index.rst` & `dftbplus_step-2024.4.24/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/docs/make.bat` & `dftbplus_step-2024.4.24/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/docs/user_guide/index.rst` & `dftbplus_step-2024.4.24/docs/user_guide/index.rst`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/docs/user_guide/recipes/images/recipe_1_extended_from_smiles.png` & `dftbplus_step-2024.4.24/docs/user_guide/recipes/images/recipe_1_extended_from_smiles.png`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/docs/user_guide/recipes/images/recipe_1_extended_parameters.png` & `dftbplus_step-2024.4.24/docs/user_guide/recipes/images/recipe_1_extended_parameters.png`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/docs/user_guide/recipes/images/recipe_1_extended_submit.png` & `dftbplus_step-2024.4.24/docs/user_guide/recipes/images/recipe_1_extended_submit.png`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/docs/user_guide/recipes/images/recipe_1_extended_zenodo.png` & `dftbplus_step-2024.4.24/docs/user_guide/recipes/images/recipe_1_extended_zenodo.png`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/docs/user_guide/recipes/images/recipe_1_flowchart.png` & `dftbplus_step-2024.4.24/docs/user_guide/recipes/images/recipe_1_flowchart.png`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/docs/user_guide/recipes/images/recipe_1_job_page.png` & `dftbplus_step-2024.4.24/docs/user_guide/recipes/images/recipe_1_job_page.png`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/docs/user_guide/recipes/images/recipe_1_jobs.png` & `dftbplus_step-2024.4.24/docs/user_guide/recipes/images/recipe_1_jobs.png`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/docs/user_guide/recipes/images/recipe_1_optimization.png` & `dftbplus_step-2024.4.24/docs/user_guide/recipes/images/recipe_1_optimization.png`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/docs/user_guide/recipes/images/recipe_1_parameters.png` & `dftbplus_step-2024.4.24/docs/user_guide/recipes/images/recipe_1_parameters.png`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/docs/user_guide/recipes/images/recipe_1_run.png` & `dftbplus_step-2024.4.24/docs/user_guide/recipes/images/recipe_1_run.png`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/docs/user_guide/recipes/images/recipe_1_water.png` & `dftbplus_step-2024.4.24/docs/user_guide/recipes/images/recipe_1_water.png`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/docs/user_guide/recipes/images/recipe_2_bandstructure.png` & `dftbplus_step-2024.4.24/docs/user_guide/recipes/images/recipe_2_bandstructure.png`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/docs/user_guide/recipes/images/recipe_2_bandstructure_zoomed.png` & `dftbplus_step-2024.4.24/docs/user_guide/recipes/images/recipe_2_bandstructure_zoomed.png`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/docs/user_guide/recipes/images/recipe_2_choose.png` & `dftbplus_step-2024.4.24/docs/user_guide/recipes/images/recipe_2_choose.png`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/docs/user_guide/recipes/images/recipe_2_dftb+_flow.png` & `dftbplus_step-2024.4.24/docs/user_guide/recipes/images/recipe_2_dftb+_flow.png`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/docs/user_guide/recipes/images/recipe_2_flowchart.png` & `dftbplus_step-2024.4.24/docs/user_guide/recipes/images/recipe_2_flowchart.png`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/docs/user_guide/recipes/images/recipe_2_parameters.png` & `dftbplus_step-2024.4.24/docs/user_guide/recipes/images/recipe_2_parameters.png`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/docs/user_guide/recipes/images/recipe_2_parameters_dialog.png` & `dftbplus_step-2024.4.24/docs/user_guide/recipes/images/recipe_2_parameters_dialog.png`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/docs/user_guide/recipes/images/recipe_2_read.png` & `dftbplus_step-2024.4.24/docs/user_guide/recipes/images/recipe_2_read.png`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/docs/user_guide/recipes/images/recipe_2_submit.png` & `dftbplus_step-2024.4.24/docs/user_guide/recipes/images/recipe_2_submit.png`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/docs/user_guide/recipes/recipe_1.rst` & `dftbplus_step-2024.4.24/docs/user_guide/recipes/recipe_1.rst`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/docs/user_guide/recipes/recipe_1_extended.rst` & `dftbplus_step-2024.4.24/docs/user_guide/recipes/recipe_1_extended.rst`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/docs/user_guide/recipes/recipe_2.rst` & `dftbplus_step-2024.4.24/docs/user_guide/recipes/recipe_2.rst`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/setup.py` & `dftbplus_step-2024.4.24/setup.py`

 * *Files identical despite different names*

### Comparing `dftbplus_step-2024.1.18/versioneer.py` & `dftbplus_step-2024.4.24/versioneer.py`

 * *Files 0% similar despite different names*

```diff
@@ -335,17 +335,17 @@
 def get_config_from_root(root):
     """Read the project setup.cfg file to determine Versioneer config."""
     # This might raise EnvironmentError (if setup.cfg is missing), or
     # configparser.NoSectionError (if it lacks a [versioneer] section), or
     # configparser.NoOptionError (if it lacks "VCS="). See the docstring at
     # the top of versioneer.py for instructions on writing your setup.cfg .
     setup_cfg = os.path.join(root, "setup.cfg")
-    parser = configparser.SafeConfigParser()
+    parser = configparser.ConfigParser()
     with open(setup_cfg, "r") as f:
-        parser.readfp(f)
+        parser.read_file(f)
     VCS = parser.get("versioneer", "VCS")  # mandatory
 
     def get(parser, name):
         if parser.has_option("versioneer", name):
             return parser.get("versioneer", name)
         return None
     cfg = VersioneerConfig()
```

