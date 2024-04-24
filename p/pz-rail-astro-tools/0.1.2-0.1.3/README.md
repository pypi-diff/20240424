# Comparing `tmp/pz-rail-astro-tools-0.1.2.tar.gz` & `tmp/pz_rail_astro_tools-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-rail-astro-tools-0.1.2.tar", last modified: Thu Nov 23 08:54:37 2023, max compression
+gzip compressed data, was "pz_rail_astro_tools-0.1.3.tar", last modified: Wed Apr 24 01:13:59 2024, max compression
```

## Comparing `pz-rail-astro-tools-0.1.2.tar` & `pz_rail_astro_tools-0.1.3.tar`

### file list

```diff
@@ -1,63 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 08:54:37.950391 pz-rail-astro-tools-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)      307 2023-11-23 08:54:27.000000 pz-rail-astro-tools-0.1.2/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 08:54:37.918391 pz-rail-astro-tools-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 08:54:37.918391 pz-rail-astro-tools-0.1.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2023-11-23 08:54:27.000000 pz-rail-astro-tools-0.1.2/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      661 2023-11-23 08:54:27.000000 pz-rail-astro-tools-0.1.2/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      707 2023-11-23 08:54:27.000000 pz-rail-astro-tools-0.1.2/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      783 2023-11-23 08:54:27.000000 pz-rail-astro-tools-0.1.2/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 08:54:37.918391 pz-rail-astro-tools-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2023-11-23 08:54:27.000000 pz-rail-astro-tools-0.1.2/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2023-11-23 08:54:27.000000 pz-rail-astro-tools-0.1.2/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      950 2023-11-23 08:54:27.000000 pz-rail-astro-tools-0.1.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      931 2023-11-23 08:54:27.000000 pz-rail-astro-tools-0.1.2/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2023-11-23 08:54:27.000000 pz-rail-astro-tools-0.1.2/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2023-11-23 08:54:27.000000 pz-rail-astro-tools-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2023-11-23 08:54:27.000000 pz-rail-astro-tools-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2023-11-23 08:54:27.000000 pz-rail-astro-tools-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3941 2023-11-23 08:54:37.950391 pz-rail-astro-tools-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2023-11-23 08:54:27.000000 pz-rail-astro-tools-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      163 2023-11-23 08:54:27.000000 pz-rail-astro-tools-0.1.2/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2023-11-23 08:54:27.000000 pz-rail-astro-tools-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-23 08:54:37.950391 pz-rail-astro-tools-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-11-23 08:54:27.000000 pz-rail-astro-tools-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 08:54:37.914391 pz-rail-astro-tools-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 08:54:37.950391 pz-rail-astro-tools-0.1.2/src/pz_rail_astro_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3941 2023-11-23 08:54:37.000000 pz-rail-astro-tools-0.1.2/src/pz_rail_astro_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2023-11-23 08:54:37.000000 pz-rail-astro-tools-0.1.2/src/pz_rail_astro_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-23 08:54:37.000000 pz-rail-astro-tools-0.1.2/src/pz_rail_astro_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2023-11-23 08:54:37.000000 pz-rail-astro-tools-0.1.2/src/pz_rail_astro_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-11-23 08:54:37.000000 pz-rail-astro-tools-0.1.2/src/pz_rail_astro_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 08:54:37.914391 pz-rail-astro-tools-0.1.2/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 08:54:37.922391 pz-rail-astro-tools-0.1.2/src/rail/astro_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      386 2023-11-23 08:54:27.000000 pz-rail-astro-tools-0.1.2/src/rail/astro_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-11-23 08:54:37.000000 pz-rail-astro-tools-0.1.2/src/rail/astro_tools/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 08:54:37.914391 pz-rail-astro-tools-0.1.2/src/rail/creation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 08:54:37.922391 pz-rail-astro-tools-0.1.2/src/rail/creation/degradation/
--rw-r--r--   0 runner    (1001) docker     (127)    11974 2023-11-23 08:54:27.000000 pz-rail-astro-tools-0.1.2/src/rail/creation/degradation/grid_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2023-11-23 08:54:27.000000 pz-rail-astro-tools-0.1.2/src/rail/creation/degradation/lsst_error_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    19794 2023-11-23 08:54:27.000000 pz-rail-astro-tools-0.1.2/src/rail/creation/degradation/observing_condition_degrader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4935 2023-11-23 08:54:27.000000 pz-rail-astro-tools-0.1.2/src/rail/creation/degradation/spectroscopic_degraders.py
--rw-r--r--   0 runner    (1001) docker     (127)    22251 2023-11-23 08:54:27.000000 pz-rail-astro-tools-0.1.2/src/rail/creation/degradation/spectroscopic_selections.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 08:54:37.922391 pz-rail-astro-tools-0.1.2/src/rail/creation/engines/
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2023-11-23 08:54:27.000000 pz-rail-astro-tools-0.1.2/src/rail/creation/engines/gcr_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 08:54:37.914391 pz-rail-astro-tools-0.1.2/src/rail/examples_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 08:54:37.914391 pz-rail-astro-tools-0.1.2/src/rail/examples_data/creation_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 08:54:37.922391 pz-rail-astro-tools-0.1.2/src/rail/examples_data/creation_data/data/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2023-11-23 08:54:27.000000 pz-rail-astro-tools-0.1.2/src/rail/examples_data/creation_data/data/HSC_grid_settings.pkl
--rw-r--r--   0 runner    (1001) docker     (127) 13823712 2023-11-23 08:54:27.000000 pz-rail-astro-tools-0.1.2/src/rail/examples_data/creation_data/data/hsc_ratios_and_specz.hdf5
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 08:54:37.946391 pz-rail-astro-tools-0.1.2/src/rail/examples_data/creation_data/data/survey_conditions/
--rw-r--r--   0 runner    (1001) docker     (127)  1581120 2023-11-23 08:54:27.000000 pz-rail-astro-tools-0.1.2/src/rail/examples_data/creation_data/data/survey_conditions/DC2-dr6-galcounts-i20-i25.3-nside-128.fits
--rw-r--r--   0 runner    (1001) docker     (127)  1581120 2023-11-23 08:54:27.000000 pz-rail-astro-tools-0.1.2/src/rail/examples_data/creation_data/data/survey_conditions/DC2-mask-neg-nside-128.fits
--rw-r--r--   0 runner    (1001) docker     (127)  1581120 2023-11-23 08:54:27.000000 pz-rail-astro-tools-0.1.2/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_airmass_i_and_nightlt1825_HEAL.fits
--rw-r--r--   0 runner    (1001) docker     (127)  1581120 2023-11-23 08:54:27.000000 pz-rail-astro-tools-0.1.2/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_fiveSigmaDepth_i_and_nightlt1825_HEAL.fits
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 08:54:37.946391 pz-rail-astro-tools-0.1.2/src/rail/tools/
--rw-r--r--   0 runner    (1001) docker     (127)    18365 2023-11-23 08:54:27.000000 pz-rail-astro-tools-0.1.2/src/rail/tools/util_photometry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 08:54:37.918391 pz-rail-astro-tools-0.1.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 08:54:37.950391 pz-rail-astro-tools-0.1.2/tests/astro_tools/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 08:54:37.950391 pz-rail-astro-tools-0.1.2/tests/astro_tools/gcr_test_data/
--rw-r--r--   0 runner    (1001) docker     (127)   179385 2023-11-23 08:54:27.000000 pz-rail-astro-tools-0.1.2/tests/astro_tools/gcr_test_data/schema.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    24490 2023-11-23 08:54:27.000000 pz-rail-astro-tools-0.1.2/tests/astro_tools/gcr_test_data/test_object_tract_4850.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)     7356 2023-11-23 08:54:27.000000 pz-rail-astro-tools-0.1.2/tests/astro_tools/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10578 2023-11-23 08:54:27.000000 pz-rail-astro-tools-0.1.2/tests/astro_tools/test_degraders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2023-11-23 08:54:27.000000 pz-rail-astro-tools-0.1.2/tests/astro_tools/test_gcr_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:13:59.030484 pz_rail_astro_tools-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:13:58.998484 pz_rail_astro_tools-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:13:58.998484 pz_rail_astro_tools-0.1.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:13:59.002484 pz_rail_astro_tools-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-04-24 01:13:59.030484 pz_rail_astro_tools-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 01:13:59.030484 pz_rail_astro_tools-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:13:58.994484 pz_rail_astro_tools-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:13:59.030484 pz_rail_astro_tools-0.1.3/src/pz_rail_astro_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-04-24 01:13:58.000000 pz_rail_astro_tools-0.1.3/src/pz_rail_astro_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-24 01:13:58.000000 pz_rail_astro_tools-0.1.3/src/pz_rail_astro_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 01:13:58.000000 pz_rail_astro_tools-0.1.3/src/pz_rail_astro_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-24 01:13:58.000000 pz_rail_astro_tools-0.1.3/src/pz_rail_astro_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 01:13:58.000000 pz_rail_astro_tools-0.1.3/src/pz_rail_astro_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:13:58.998484 pz_rail_astro_tools-0.1.3/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:13:59.002484 pz_rail_astro_tools-0.1.3/src/rail/astro_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/src/rail/astro_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-24 01:13:58.000000 pz_rail_astro_tools-0.1.3/src/rail/astro_tools/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:13:58.994484 pz_rail_astro_tools-0.1.3/src/rail/creation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:13:59.002484 pz_rail_astro_tools-0.1.3/src/rail/creation/degradation/
+-rw-r--r--   0 runner    (1001) docker     (127)    12432 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/src/rail/creation/degradation/grid_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/src/rail/creation/degradation/lsst_error_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19987 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/src/rail/creation/degradation/observing_condition_degrader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/src/rail/creation/degradation/photerr_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/src/rail/creation/degradation/photometric_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/src/rail/creation/degradation/spectroscopic_degraders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22176 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/src/rail/creation/degradation/spectroscopic_selections.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:13:59.002484 pz_rail_astro_tools-0.1.3/src/rail/creation/engines/
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/src/rail/creation/engines/gcr_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:13:58.998484 pz_rail_astro_tools-0.1.3/src/rail/examples_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:13:58.998484 pz_rail_astro_tools-0.1.3/src/rail/examples_data/creation_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:13:59.002484 pz_rail_astro_tools-0.1.3/src/rail/examples_data/creation_data/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/src/rail/examples_data/creation_data/data/HSC_grid_settings.pkl
+-rw-r--r--   0 runner    (1001) docker     (127) 13823712 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/src/rail/examples_data/creation_data/data/hsc_ratios_and_specz.hdf5
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:13:59.026484 pz_rail_astro_tools-0.1.3/src/rail/examples_data/creation_data/data/survey_conditions/
+-rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/src/rail/examples_data/creation_data/data/survey_conditions/DC2-dr6-galcounts-i20-i25.3-nside-128.fits
+-rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/src/rail/examples_data/creation_data/data/survey_conditions/DC2-mask-neg-nside-128.fits
+-rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_airmass_i_and_nightlt1825_HEAL.fits
+-rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_fiveSigmaDepth_i_and_nightlt1825_HEAL.fits
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:13:59.030484 pz_rail_astro_tools-0.1.3/src/rail/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)    18425 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/src/rail/tools/util_photometry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:13:58.998484 pz_rail_astro_tools-0.1.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:13:59.030484 pz_rail_astro_tools-0.1.3/tests/astro_tools/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:13:59.030484 pz_rail_astro_tools-0.1.3/tests/astro_tools/gcr_test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)   179385 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/tests/astro_tools/gcr_test_data/schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    24490 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/tests/astro_tools/gcr_test_data/test_object_tract_4850.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)     7356 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/tests/astro_tools/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13303 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/tests/astro_tools/test_degraders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/tests/astro_tools/test_gcr_engine.py
```

### Comparing `pz-rail-astro-tools-0.1.2/.github/ISSUE_TEMPLATE/1-bug_report.md` & `pz_rail_astro_tools-0.1.3/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `pz-rail-astro-tools-0.1.2/.github/ISSUE_TEMPLATE/2-feature_request.md` & `pz_rail_astro_tools-0.1.3/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `pz-rail-astro-tools-0.1.2/.github/pull_request_template.md` & `pz_rail_astro_tools-0.1.3/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pz-rail-astro-tools-0.1.2/.github/workflows/linting.yml` & `pz_rail_astro_tools-0.1.3/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-astro-tools-0.1.2/.github/workflows/publish-to-pypi.yml` & `pz_rail_astro_tools-0.1.3/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-astro-tools-0.1.2/.github/workflows/smoke-test.yml` & `pz_rail_astro_tools-0.1.3/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-astro-tools-0.1.2/.github/workflows/testing-and-coverage.yml` & `pz_rail_astro_tools-0.1.3/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-astro-tools-0.1.2/.gitignore` & `pz_rail_astro_tools-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pz-rail-astro-tools-0.1.2/.pre-commit-config.yaml` & `pz_rail_astro_tools-0.1.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-astro-tools-0.1.2/LICENSE` & `pz_rail_astro_tools-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pz-rail-astro-tools-0.1.2/PKG-INFO` & `pz_rail_astro_tools-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-astro-tools
-Version: 0.1.2
+Version: 0.1.3
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <lsst-desc-rail-admin@slac.stanford.edu>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz-rail-astro-tools-0.1.2/README.md` & `pz_rail_astro_tools-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-astro-tools-0.1.2/pyproject.toml` & `pz_rail_astro_tools-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pz-rail-astro-tools-0.1.2/src/pz_rail_astro_tools.egg-info/PKG-INFO` & `pz_rail_astro_tools-0.1.3/src/pz_rail_astro_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-astro-tools
-Version: 0.1.2
+Version: 0.1.3
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <lsst-desc-rail-admin@slac.stanford.edu>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz-rail-astro-tools-0.1.2/src/pz_rail_astro_tools.egg-info/SOURCES.txt` & `pz_rail_astro_tools-0.1.3/src/pz_rail_astro_tools.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 src/pz_rail_astro_tools.egg-info/requires.txt
 src/pz_rail_astro_tools.egg-info/top_level.txt
 src/rail/astro_tools/__init__.py
 src/rail/astro_tools/_version.py
 src/rail/creation/degradation/grid_selection.py
 src/rail/creation/degradation/lsst_error_model.py
 src/rail/creation/degradation/observing_condition_degrader.py
+src/rail/creation/degradation/photerr_demo.ipynb
+src/rail/creation/degradation/photometric_errors.py
 src/rail/creation/degradation/spectroscopic_degraders.py
 src/rail/creation/degradation/spectroscopic_selections.py
 src/rail/creation/engines/gcr_engine.py
 src/rail/examples_data/creation_data/data/HSC_grid_settings.pkl
 src/rail/examples_data/creation_data/data/hsc_ratios_and_specz.hdf5
 src/rail/examples_data/creation_data/data/survey_conditions/DC2-dr6-galcounts-i20-i25.3-nside-128.fits
 src/rail/examples_data/creation_data/data/survey_conditions/DC2-mask-neg-nside-128.fits
```

### Comparing `pz-rail-astro-tools-0.1.2/src/rail/creation/degradation/grid_selection.py` & `pz_rail_astro_tools-0.1.3/src/rail/creation/degradation/grid_selection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-"""Degraders that emulate spectroscopic effects on photometry"""
+"""Selector that emulate spectroscopic effects on photometry"""
 
 import os
 import numpy as np
 import pandas as pd
 import pickle
 import tables_io
-from rail.creation.degrader import Degrader
+from rail.creation.selector import Selector
 from rail.core.utils import find_rail_file
 from ceci.config import StageParameter as Param
 
 
-class GridSelection(Degrader):
+class GridSelection(Selector):
     """
     Uses the ratio of HSC spectroscpic galaxies to photometric galaxies to portion a sample
     into training and application samples. Option to implement a color-based redshift cut off in each pixel.
     Option of further degrading the training sample by limiting it to galaxies less than a redshift cutoff by specifying redshift_cut.
 
     Parameters
     ----------
@@ -35,40 +35,42 @@
       'x_limits': 2-element list, this is a list of the lower and upper limits of the magnitude. Default for HSC is [13, 16],
       'y_limits': 2-element list, this is a list of the lower and upper limits of the color. Default for HSC is [-2, 6]}
 
     NOTE: the default 'HSC' grid file, located in rail/examples_data/creation_data/data/hsc_ratios_and_specz.hdf5, is based on data from the
     Second HSC Data Release, details of which can be found here:
     Aihara, H., AlSayyad, Y., Ando, M., et al. 2019, PASJ, 71, 114
     doi: 10.1093/pasj/psz103
+    
+    Update(Apr 16 2024): Now inherit from selector and implement the _select() instead of run()
     """
     def_ratio_file = find_rail_file("examples_data/creation_data/data/hsc_ratios_and_specz.hdf5")
     def_set_file = find_rail_file("examples_data/creation_data/data/HSC_grid_settings.pkl" )
 
     name = 'GridSelection'
-    config_options = Degrader.config_options.copy()
+    config_options = Selector.config_options.copy()
     config_options.update(color_redshift_cut=Param(bool, True, msg='using color-based redshift cut'),
                           percentile_cut=Param(float, 99.0, msg='percentile cut-off for each pixel in color-based redshift cut off'),
                           redshift_cut=Param(float, 100.0, msg="cut redshifts above this value"),
                           ratio_file=Param(str, def_ratio_file,
                                            msg="path to ratio file"),
                           settings_file=Param(str, def_set_file,
                                               msg='path to pickled parameters file'),
                           random_seed=Param(int, 12345, msg="random seed for reproducibility"),
                           scaling_factor=Param(float, 1.588, msg="multiplicative factor for ratios to adjust number of galaxies kept"))
 
     def __init__(self, args, comm=None):
 
-        Degrader.__init__(self, args, comm=comm)
+        Selector.__init__(self, args, comm=comm)
 
         if self.config.redshift_cut < 0:
             raise ValueError("redshift cut must be positive")
         if (self.config.percentile_cut < 0) | (self.config.percentile_cut > 100):
             raise ValueError('percentile cut off must be between 0 and 100')
 
-    def run(self):
+    def _select(self):
         """
         HSC galaxies were binned in color magnitude space with i-band mag from -2 to 6 and g-z color from 13 to 26
         200 bins in each direction. The ratio of of galaxies with spectroscopic redshifts (training galaxies) to
         galaxies with only photometry in HSC wide field (application galaxies) was computed for each pixel. We divide
         the data into the same pixels and randomly select galaxies into the training sample based on the HSC ratios.
         If using a color-based redshift cut, galaxies with redshifts > the percentile cut are removed from the sample
         before making the random selection.
@@ -100,16 +102,17 @@
         # now remove galaxies that don't fall in i-mag and g-z color range of HSC data. These will always be application sample galaxies
         x_lims = settings['x_limits']
         y_lims = settings['y_limits']
         if len(x_lims) != 2:  # pragma: no cover
             raise ValueError("x limits should have two elements!")
         if len(y_lims) != 2:  # pragma: no cover
             raise ValueError("y limits should have two elements!")
-        data_hsc_like = data[(data['x_vals'] >= x_lims[0]) & (data['x_vals'] <= x_lims[1]) & (data['y_vals'] >= y_lims[0]) & (data['y_vals'] <= y_lims[1])]
-
+        # data_hsc_like = data[(data['x_vals'] >= x_lims[0]) & (data['x_vals'] <= x_lims[1]) & (data['y_vals'] >= y_lims[0]) & (data['y_vals'] <= y_lims[1])]
+        
+        data_hsc_like = data
         x_vals = data_hsc_like['x_vals'].to_numpy()
         y_vals = data_hsc_like['y_vals'].to_numpy()
 
         # Opens file with HSC ratios
         ratios = tables_io.read(self.config.ratio_file)['ratios']
 
         # Sets pixel edges to be the same as were used to calculate HSC ratios
@@ -151,17 +154,23 @@
 
         # For each galaxy in data, identifies the pixel it belongs in, and adds the ratio for that pixel to a new column in data called 'ratios'
         pixels_y = np.searchsorted(y_edges, y_vals) - 1
         pixels_x = np.searchsorted(x_edges, x_vals) - 1
 
         ratio_list = []
         max_specz_list = []
+                
         for pix_x, pix_y in zip(pixels_x, pixels_y):
-            ratio_list.append(ratios[pix_y][pix_x])
-            max_specz_list.append(max_specz[pix_y][pix_x])
+            # cover the galaxy outside the grid of ratio
+            if (pix_x in [-1,ratios.shape[0]]) or (pix_y in [-1, ratios.shape[1]]):
+                ratio_list.append(0.0)
+                max_specz_list.append(99.0)
+            else:
+                ratio_list.append(ratios[pix_y][pix_x])
+                max_specz_list.append(max_specz[pix_y][pix_x])
 
         data_hsc_like['ratios'] = ratio_list
         data_hsc_like['max_specz'] = max_specz_list
 
         # remove galaxies with redshifts higher than the color-based cutoff
         data_hsc_like_redshift_cut = data_hsc_like[data_hsc_like['redshift'] <= data_hsc_like['max_specz']]
 
@@ -200,13 +209,17 @@
             if random_num > xratio:  # pragma: no cover
                 for j in range(int(number_to_keep)):
                     keep_inds.append(indices_to_list[j])
 
             else:  # pragma: no cover
                 for j in range(int(number_to_keep) + 1):
                     keep_inds.append(indices_to_list[j])
+        
+        finalcut = data_hsc_like_redshift_cut.loc[keep_inds, :]
+        finalcut = finalcut[finalcut['redshift'] > 0]
+        
+        final_keep_inds = np.array(finalcut.index)
+        
+        total_mask = np.zeros(len(data), dtype=bool)
+        total_mask[final_keep_inds] = True
 
-        training_data = data_hsc_like_redshift_cut.loc[keep_inds, :]
-        training_data = training_data[training_data['redshift'] > 0]
-        training_data = training_data.drop(['x_vals', 'y_vals', 'ratios'], axis=1)
-
-        self.add_data('output', training_data)
+        return total_mask
```

### Comparing `pz-rail-astro-tools-0.1.2/src/rail/creation/degradation/lsst_error_model.py` & `pz_rail_astro_tools-0.1.3/src/rail/creation/degradation/lsst_error_model.py`

 * *Files identical despite different names*

### Comparing `pz-rail-astro-tools-0.1.2/src/rail/creation/degradation/observing_condition_degrader.py` & `pz_rail_astro_tools-0.1.3/src/rail/creation/degradation/observing_condition_degrader.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
 import healpy as hp
 import numpy as np
 import pandas as pd
 from ceci.config import StageParameter as Param
 from photerr import LsstErrorModel, LsstErrorParams
 
-from rail.creation.degrader import Degrader
+from rail.creation.noisifier import Noisifier
 
 
-class ObsCondition(Degrader):
+class ObsCondition(Noisifier):
     """Photometric errors based on observation conditions
 
     This degrader calculates spatially-varying photometric errors
     using input survey condition maps. The error is based on the
     LSSTErrorModel from the PhotErr python package.
 
     Parameters
@@ -56,15 +56,15 @@
         for the survey condition maps).
         If any argument is not passed, the default value in
         PhotErr's LsstErrorModel is adopted.
 
     """
 
     name = "ObsCondition"
-    config_options = Degrader.config_options.copy()
+    config_options = Noisifier.config_options.copy()
     config_options.update(
         nside=Param(
             int,
             128,
             msg="nside for the input maps in HEALPIX format.",
         ),
         mask=Param(
@@ -113,15 +113,15 @@
             "i":2.06,
             "z":1.58,
             "y":1.31,
         }
     
 
     def __init__(self, args, comm=None):
-        Degrader.__init__(self, args, comm=comm)
+        Noisifier.__init__(self, args, comm=comm)
 
         # store a list of keys relevant for
         # survey conditions;
         # a path to the survey condition
         # map or a float number should be
         # provided if these keys are provided
         self.obs_cond_keys = [
@@ -403,18 +403,25 @@
             for b in self.STANDARD_BANDS:
                 key=b
                 # update pixel_cat to the reddened magnitudes
                 pixel_cat[key] = (pixel_cat[key].copy())+ebvvec*self.BAND_A_EBV[b]
 
         return pixel_cat
 
+    
+    def _initNoiseModel(self):
+        """
+        Initialise the error model: LSSTerrorModel
+        """
+        self.default_errorModel = LsstErrorModel()
 
-    def run(self):
+        
+    def _addNoise(self):
         """
-        Run the degrader.
+        Run the noisifier.
         """
         self.rng = np.random.default_rng(seed=self.config["random_seed"])
 
         catalog = self.get_data("input", allow_missing=True)
 
         # if self.map_dict empty, call LsstErrorModel:
         if len(self.config["map_dict"]) == 0:
@@ -433,16 +440,16 @@
             
             # loop over each pixel
             pixel_cat_list = []
             for pixel, pixel_cat in catalog.groupby("pixel"):
                 
                 # first, check if pixel is -99 - these objects have default obs_conditions:
                 if pixel==-99:
-                    # creating the error model for this pixel
-                    errorModel = LsstErrorModel()
+                    # use the default error model for this pixel
+                    errorModel = self.default_errorModel
                 
                 else:            
                     # get the observing conditions for this pixel
                     obs_conditions = self.get_pixel_conditions(pixel)
 
                     # apply MW extinction if supplied, 
                     # replace the Mag column with reddened magnitudes:
```

### Comparing `pz-rail-astro-tools-0.1.2/src/rail/creation/degradation/spectroscopic_degraders.py` & `pz_rail_astro_tools-0.1.3/src/rail/creation/degradation/spectroscopic_degraders.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """Degraders that emulate spectroscopic effects on photometry"""
 
 import numpy as np
 import pandas as pd
-from rail.creation.degrader import Degrader
+from rail.creation.selector import Selector
+from rail.creation.noisifier import Noisifier
 
 
-class LineConfusion(Degrader):
+
+class LineConfusion(Noisifier):
     """Degrader that simulates emission line confusion.
 
     .. code-block:: python
 
        Example: degrader = LineConfusion(true_wavelen=3727,
                                          wrong_wavelen=5007,
                                          frac_wrong=0.05)
@@ -33,32 +35,36 @@
         for the correct emission line.
         Wavelength unit assumed to be the same as true_wavelen.
     frac_wrong : float between zero and one
         The fraction of galaxies with confused emission lines.
     """
 
     name = 'LineConfusion'
-    config_options = Degrader.config_options.copy()
+    config_options = Noisifier.config_options.copy()
     config_options.update(true_wavelen=float,
                           wrong_wavelen=float,
                           frac_wrong=float)
 
     def __init__(self, args, comm=None):
         """
         """
-        Degrader.__init__(self, args, comm=comm)
+        Noisifier.__init__(self, args, comm=comm)
         # validate parameters
         if self.config.true_wavelen < 0:
             raise ValueError("true_wavelen must be positive, not {self.config.true_wavelen}")
         if self.config.wrong_wavelen < 0:
             raise ValueError("wrong_wavelen must be positive, not {self.config.wrong_wavelen}")
         if self.config.frac_wrong < 0 or self.config.frac_wrong > 1:
             raise ValueError("frac_wrong must be between 0 and 1., not {self.config.wrong_wavelen}")
+            
+            
+    def _initNoiseModel(self):
+        self.rng = np.random.default_rng(self.config.seed)
 
-    def run(self):
+    def _addNoise(self):
         """ Run method
 
         Applies line confusion
 
         Notes
         -----
         Get the input data from the data store under this stages 'input' tag
@@ -71,16 +77,15 @@
 
         # get the minimum redshift
         # if wrong_wavelen < true_wavelen, this is minimum the redshift for
         # which the confused redshift is still positive
         zmin = self.config.wrong_wavelen / self.config.true_wavelen - 1
 
         # select the random fraction of galaxies whose lines are confused
-        rng = np.random.default_rng(self.config.seed)
-        idx = rng.choice(
+        idx = self.rng.choice(
             np.where(values[:, 0] > zmin)[0],
             size=int(self.config.frac_wrong * values.shape[0]),
             replace=False,
         )
 
         # transform these redshifts
         values[idx, 0] = (
@@ -88,40 +93,40 @@
         ) * self.config.true_wavelen / self.config.wrong_wavelen - 1
 
         # return results in a data frame
         outData = pd.DataFrame(values, columns=columns)
         self.add_data('output', outData)
 
 
-class InvRedshiftIncompleteness(Degrader):
+class InvRedshiftIncompleteness(Selector):
     """Degrader that simulates incompleteness with a selection function
     inversely proportional to redshift.
 
     The survival probability of this selection function is
     p(z) = min(1, z_p/z),
     where z_p is the pivot redshift.
 
     Parameters
     ----------
     pivot_redshift : positive float
         The redshift at which the incompleteness begins.
     """
 
     name = 'InvRedshiftIncompleteness'
-    config_options = Degrader.config_options.copy()
+    config_options = Selector.config_options.copy()
     config_options.update(pivot_redshift=float)
 
     def __init__(self, args, comm=None):
         """
         """
-        Degrader.__init__(self, args, comm=comm)
+        Selector.__init__(self, args, comm=comm)
         if self.config.pivot_redshift < 0:
             raise ValueError("pivot redshift must be positive, not {self.config.pivot_redshift}")
 
-    def run(self):
+    def _select(self):
         """ Run method
 
         Applies incompleteness
 
         Notes
         -----
         Get the input data from the data store under this stages 'input' tag
@@ -132,8 +137,8 @@
         # calculate survival probability for each galaxy
         survival_prob = np.clip(self.config.pivot_redshift / data["redshift"], 0, 1)
 
         # probabalistically drop galaxies from the data set
         rng = np.random.default_rng(self.config.seed)
         mask = rng.random(size=data.shape[0]) <= survival_prob
 
-        self.add_data('output', data[mask])
+        return mask
```

### Comparing `pz-rail-astro-tools-0.1.2/src/rail/creation/degradation/spectroscopic_selections.py` & `pz_rail_astro_tools-0.1.3/src/rail/creation/degradation/spectroscopic_selections.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,54 +1,60 @@
-""" Applying selection functions to catalog """
+"""Degrader that applies selection functions to catalog."""
 
 import os
 
 import numpy as np
 from ceci.config import StageParameter as Param
-from rail.creation.degrader import Degrader
+from rail.creation.selector import Selector
 from scipy.interpolate import interp1d
-from rail.core.utils import find_rail_file
+from rail.core.utils import RAILDIR
 
 
-class SpecSelection(Degrader):
-    """
-    The super class of spectroscopic selections.
+class SpecSelection(Selector):
+    """The super class of spectroscopic selections.
 
     Parameters
     ----------
-    N_tot: integer
-        total number of down-sampled, spec-selected galaxies.
-        If N_tot is greater than the number of spec-sepected galaxies, then
-        it will be ignored.
-    nondetect_val: value to be removed for non detects
-    downsample: bool
-        If True, then downsample the pre-selected galaxies
-        to N_tot galaxies.
-    success_rate_dir: string, the path to the success rate files.
-    percentile_cut: If using color-based redshift cut, percentile in redshifts above which redshifts will be cut from the sample. Default is 100 (no cut)
-    colnames: a dictionary that includes necessary columns
-                         (magnitudes, colors and redshift) for selection. For magnitudes, the keys are ugrizy; for colors, the keys are,
-                         for example, gr standing for g-r; for redshift, the key is 'redshift'.
-    random_seed: random seed for reproducibility.
-
+    N_tot : int
+        The total number of down-sampled, spec-selected galaxies. If N_tot is 
+        greater than the number of spec-sepected galaxies, then it will be 
+        ignored.
+    nondetect_val : float
+        The value to be removed for non detects
+    downsample : bool
+        If True, then downsample the pre-selected galaxies to N_tot galaxies.
+    success_rate_dir : string
+        The path to the success rate files
+    percentile_cut: int, default=100
+        If using color-based redshift cut, percentile in redshifts above which 
+        redshifts will be cut from the sample. Default is 100 (no cut).
+    colnames: dict
+        A dictionary that includes necessary columns (magnitudes, colors and 
+        redshift) for selection. For magnitudes, the keys are ugrizy; for 
+        colors, the keys are, for example, gr standing for g-r; for redshift, 
+        the key is 'redshift'.
+    random_seed : int
+        Random seed for reproducibility
     """
 
     name = "specselection"
-    config_options = Degrader.config_options.copy()
+    config_options = Selector.config_options.copy()
     config_options.update(
         N_tot=Param(int, 10000, msg="Number of selected sources"),
         nondetect_val=Param(float, 99.0, msg="value to be removed for non detects"),
         downsample=Param(
             bool,
             True,
             msg="If true, downsample the selected sources into a total number of N_tot",
         ),
         success_rate_dir=Param(
             str,
-            find_rail_file("examples_data/creation_data/data/success_rate_data"),
+            os.path.join(RAILDIR,
+                "rail/examples_data/creation_data/data/success_rate_data",
+            ),
             msg="The path to the directory containing success rate files.",
         ),
         percentile_cut=Param(int, 100, msg="cut redshifts above this percentile"),
         colnames=Param(
             dict,
             {
                 **{band: "mag_" + band + "_lsst" for band in "ugrizy"},
@@ -58,76 +64,73 @@
                          (magnitudes, colors and redshift) for selection. For magnitudes, the keys are ugrizy; for colors, the keys are, \
                          for example, gr standing for g-r; for redshift, the key is 'redshift'",
         ),
         random_seed=Param(int, 42, msg="random seed for reproducibility"),
     )
 
     def __init__(self, args, comm=None):
-        Degrader.__init__(self, args, comm=comm)
-        # validate the settings
+        Selector.__init__(self, args, comm=comm)
         self._validate_settings()
         self.mask = None
         self.rng = None
 
     def _validate_settings(self):
-        """
-        Validate all the settings.
-        """
-
+        """Validate all the settings."""
         if self.config.N_tot < 0:
             raise ValueError(
                 "Total number of selected sources must be a " "positive integer."
             )
         if os.path.exists(self.config.success_rate_dir) is not True:
             raise ValueError(
                 "Success rate path: "
                 + self.config.success_rate_dir
                 + " does not exist!"
             )
 
     def validate_colnames(self, data):
-        """
-        Validate the column names of data table to make sure they have necessary information
-        for each selection.
-        colnames: a list of column names.
+        """Validate the column names of data table to make sure they have 
+        necessary information for each selection.
+
+        Parameters
+        ----------
+        colnames : list of str
+            A list of column names
         """
         colnames = self.config.colnames.values()
         check = all(item in data.columns for item in colnames)
         if check is not True:
             raise ValueError(
                 "Columns in the data are not enough for the selection."
                 + "The data should contain "
                 + str(list(colnames))
                 + ". \n"
             )
 
     def selection(self, data):
-        """
-        Selection functions. This should be overwritten by the subclasses
-        corresponding to different spec selections.
+        """Selection functions. 
+        
+        This should be overwritten by the subclasses corresponding to different 
+        spec selections.
         """
 
     def invalid_cut(self, data):
-        """
-        This function removes entries in the data that have invalid magnitude values
-        (nondetect_val or NaN)
+        """Removes entries in the data that have invalid magnitude values (NaN
+        or nondetect_val).
         """
         nondetect_val = self.config.nondetect_val
         for band in "ugrizy":
             if band not in self.config.colnames.keys():
                 continue
             colname = self.config.colnames[band]
             self.mask &= (np.abs(data[colname]) < nondetect_val) & (
                 ~np.isnan(data[colname])
             )
 
     def downsampling_N_tot(self):
-        """
-        Method to randomly sample down the objects to a given
-        number of data objects.
+        """Randomly sample down the objects to a given number of data objects.
         """
         N_tot = self.config.N_tot
         N_selected = np.count_nonzero(self.mask)
         if N_tot > N_selected:
             print(
                 "Warning: N_tot is greater than the size of spec-selected "
                 + "sample ("
@@ -142,81 +145,77 @@
             # create a mask with only those entries enabled that have been
             # selected
             mask = np.zeros_like(self.mask)
             mask[idx_keep] = True
             # update the internal state
             self.mask &= mask
 
-    def run(self):
-        """
-        Run the selection
-        """
-        self.rng = np.random.default_rng(seed=self.config.seed)
+    def _select(self):
+        """Run the selection."""
+        self.rng = np.random.default_rng(seed=self.config.random_seed)
         # get the bands and bandNames present in the data
         data = self.get_data("input", allow_missing=True)
         self.validate_colnames(data)
         self.mask = np.product(~np.isnan(data.to_numpy()), axis=1)
         self.invalid_cut(data)
         self.selection(data)
         if self.config.downsample is True:
             self.downsampling_N_tot()
+        
+        return self.mask
+#         data_selected = data.iloc[np.where(self.mask == 1)[0]]
 
-        data_selected = data.iloc[np.where(self.mask == 1)[0]]
-
-        self.add_data("output", data_selected)
+#         self.add_data("output", data_selected)
 
     def __repr__(self):
         """
         Define how the model is represented and printed.
         """
 
 
 class SpecSelection_GAMA(SpecSelection):
-    """
-    The class of spectroscopic selections with GAMA.
-    The GAMA survey covers an area of 286 deg^2, with ~238000 objects
-    The necessary column is r band
-    """
+    """The class of spectroscopic selections with GAMA.
 
+    The GAMA survey covers an area of 286 deg^2, with ~238000 objects.
+    
+    The necessary column is r band.
+    """
+    
     name = "specselection_gama"
 
     def selection(self, data):
-        """
-        GAMA selection function
-        """
+        """GAMA selection function. """
         print("Applying the selection from GAMA survey...")
         self.mask *= data[self.config.colnames["r"]] < 19.87
 
     def __repr__(self):
-        """
-        Define how the model is represented and printed.
-        """
+        """Define how the model is represented and printed."""
         # start message
         printMsg = "Applying the GAMA selection."
 
         return printMsg
 
 
 class SpecSelection_BOSS(SpecSelection):
-    """
-    The class of spectroscopic selections with BOSS.
+    """The class of spectroscopic selections with BOSS.
+    
     BOSS selection function is based on
     http://www.sdss3.org/dr9/algorithms/boss_galaxy_ts.php
-    The selection has changed slightly compared to Dawson+13
+
+    The selection has changed slightly compared to Dawson+13.
+
     BOSS covers an area of 9100 deg^2 with 893,319 galaxies.
+
     For BOSS selection, the data should at least include gri bands.
     """
 
     name = "specselection_boss"
 
     def selection(self, data):
-        """
-        The BOSS selection function.
-        """
-
+        """The BOSS selection function."""
         print("Applying the selection from BOSS survey...")
         # cut quantities (unchanged)
         c_p = 0.7 * (
             data[self.config.colnames["g"]] - data[self.config.colnames["r"]]
         ) + 1.2 * (
             data[self.config.colnames["r"]] - data[self.config.colnames["i"]] - 0.18
         )
@@ -248,44 +247,43 @@
                 < 2.0
             )
         )
         # NOTE: we ignore the CMASS sparse sample
         self.mask *= low_z | cmass
 
     def __repr__(self):
-        """
-        Define how the model is represented and printed.
-        """
+        """ Define how the model is represented and printed."""
         # start message
         printMsg = "Applying the BOSS selection."
 
         return printMsg
 
 
 class SpecSelection_DEEP2(SpecSelection):
-    """
-    The class of spectroscopic selections with DEEP2.
+    """The class of spectroscopic selections with DEEP2.
+
     DEEP2 has a sky coverage of 2.8 deg^2 with ~53000 spectra.
-    For DEEP2, one needs R band magnitude, B-R/R-I colors which are not available for the time being.
-    So we use LSST gri bands now. When the conversion degrader is ready, this subclass will be updated
-    accordingly.
+
+    For DEEP2, one needs R band magnitude, B-R/R-I colors--which are not 
+    available for the time being, so we use LSST gri bands now. When the 
+    conversion degrader is ready, this subclass will be updated accordingly.
     """
 
     name = "specselection_deep2"
 
     def photometryCut(self, data):
-        """
-        Applying DEEP2 photometric cut based on Newman+13.
-        This modified selection gives the best match to the data n(z) with
-        its cut at z~0.75 and the B-R/R-I distribution (Newman+13, Fig. 12)
+        """Applies DEEP2 photometric cut based on Newman+13.
+
+        This modified selection gives the best match to the data n(z) with its 
+        cut at z~0.75 and the B-R/R-I distribution (Newman+13, Fig. 12).
 
         Notes
         -----
-        We cannot apply the surface brightness cut and do not apply the
-        Gaussian weighted sampling near the original colour cuts.
+        We cannot apply the surface brightness cut and do not apply the Gaussian
+        weighted sampling near the original colour cuts.
         """
         mask = (
             (data[self.config.colnames["r"]] > 18.5)
             & (data[self.config.colnames["r"]] < 24.1)
             & (  # 24.1
                 (
                     data[self.config.colnames["g"]] - data[self.config.colnames["r"]]
@@ -308,16 +306,15 @@
                 )
             )
         )  # 0.5
         # update the internal state
         self.mask &= mask
 
     def speczSuccess(self, data):
-        """
-        Spec-z success rate as function of r_AB for Q>=3 read of Figure 13 in
+        """Spec-z success rate as function of r_AB for Q>=3 read of Figure 13 in
         Newman+13 for DEEP2 fields 2-4. Values are binned in steps of 0.2 mag
         with the first and last bin centered on 19 and 24.
         """
         success_R_bins = np.arange(18.9, 24.1 + 0.01, 0.2)
         success_R_centers = (success_R_bins[1:] + success_R_bins[:-1]) / 2.0
         # paper has given 1 - [sucess rate] in the histogram
         success_rate_dir = self.config.success_rate_dir
@@ -334,66 +331,62 @@
         # Randomly sample objects according to their success rate
         random_draw = self.rng.random(len(data))
         mask = random_draw < p_success_R(data[self.config.colnames["r"]])
         # update the internal state
         self.mask &= mask
 
     def selection(self, data):
-        """
-        DEEP2 selection function
-        """
+        """DEEP2 selection function."""
         self.photometryCut(data)
         self.speczSuccess(data)
 
     def __repr__(self):
-        """
-        Define how the model is represented and printed.
-        """
+        """Define how the model is represented and printed."""
         # start message
         printMsg = "Applying the DEEP2 selection."
 
         return printMsg
 
 
 class SpecSelection_VVDSf02(SpecSelection):
-    """
-    The class of spectroscopic selections with VVDSf02.
+    """The class of spectroscopic selections with VVDSf02.
+
     It covers an area of 0.5 deg^2 with ~10000 sources.
+
     Necessary columns are i band magnitude and redshift.
     """
 
     name = "specselection_VVDSf02"
 
     def photometryCut(self, data):
-        """
-        Photometric cut of VVDS 2h-field based on LeFèvre+05.
+        """Photometric cut of VVDS 2h-field based on LeFèvre+05.
 
         Notes
         -----
-        The oversight of 1.0 magnitudes on the bright end misses 0.2% of galaxies.
+        The oversight of 1.0 magnitudes on the bright end misses 0.2% of 
+        galaxies.
         """
         mask = (data[self.config.colnames["i"]] > 17.5) & (
             data[self.config.colnames["i"]] < 24.0
         )
         # 17.5, 24.0
         self.mask &= mask
 
     def speczSuccess(self, data):
-        """
-        Success rate of VVDS 2h-field
+        """Success rate of VVDS 2h-field.
 
         Notes
         -----
-        We use a redshift-based and I-band based success rate
-        independently here since we do not know their correlation,
-        which makes the success rate worse than in reality.
-
-        Spec-z success rate as function of i_AB read of Figure 16 in
-        LeFevre+05 for the VVDS 2h field. Values are binned in steps of
-        0.5 mag with the first starting at 17 and the last bin ending at 24.
+        We use a redshift-based and I-band based success rate independently here
+        since we do not know their correlation, which makes the success rate 
+        worse than in reality.
+
+        Spec-z success rate as function of i_AB read of Figure 16 in LeFevre+05
+        for the VVDS 2h field. Values are binned in steps of 0.5 mag with the 
+        first starting at 17 and the last bin ending at 24.
         """
         success_I_bins = np.arange(17.0, 24.0 + 0.01, 0.5)
         success_I_centers = (success_I_bins[1:] + success_I_bins[:-1]) / 2.0
         success_rate_dir = self.config.success_rate_dir
         success_I_rate = np.loadtxt(
             os.path.join(success_rate_dir, "VVDSf02_I_success.txt")
         )
@@ -454,47 +447,46 @@
         self.mask &= mask
 
     def selection(self, data):
         self.photometryCut(data)
         self.speczSuccess(data)
 
     def __repr__(self):
-        """
-        Define how the model is represented and printed.
-        """
+        """Define how the model is represented and printed."""
         # start message
         printMsg = "Applying the VVDSf02 selection."
 
         return printMsg
 
 
 class SpecSelection_zCOSMOS(SpecSelection):
-    """
-    The class of spectroscopic selections with zCOSMOS
+    """The class of spectroscopic selections with zCOSMOS.
+
     It covers an area of 1.7 deg^2 with ~20000 galaxies.
+
     For zCOSMOS, the data should at least include i band and redshift.
     """
 
     name = "specselection_zCOSMOS"
 
     def photometryCut(self, data):
-        """
-        Photometry cut for zCOSMOS based on Lilly+09.
+        """Photometry cut for zCOSMOS based on Lilly+09.
+
+        Updates the internal state.
+
         NOTE: This only includes zCOSMOS bright.
-        update the internal state
         """
         mask = (data[self.config.colnames["i"]] > 15.0) & (
             data[self.config.colnames["i"]] < 22.5
         )
         # 15.0, 22.5
         self.mask &= mask
 
     def speczSuccess(self, data):
-        """
-        Spec-z success rate as function of redshift (x) and I_AB (y) read of
+        """Spec-z success rate as function of redshift (x) and I_AB (y) read of
         Figure 3 in Lilly+09 for zCOSMOS bright sample.
         """
         success_rate_dir = self.config.success_rate_dir
         x = np.arange(0, 1.4, 0.00587002, dtype=np.float64)
         y = np.arange(18, 22.4, 0.01464226, dtype=np.float64)
 
         pixels_y = np.searchsorted(y, data[self.config.colnames["i"]])
@@ -518,49 +510,49 @@
         self.mask &= mask
 
     def selection(self, data):
         self.photometryCut(data)
         self.speczSuccess(data)
 
     def __repr__(self):
-        """
-        Define how the model is represented and printed.
-        """
+        """Defines how the model is represented and printed."""
         # start message
         printMsg = "Applying the zCOSMOS selection."
 
         return printMsg
 
 
 class SpecSelection_HSC(SpecSelection):
-    """
-    The class of spectroscopic selections with HSC
-    or HSC, the data should at least include giz bands and redshift.
+    """The class of spectroscopic selections with HSC.
+
+    For HSC, the data should at least include giz bands and redshift.
     """
 
     name = "specselection_HSC"
 
     def photometryCut(self, data):
-        """
-        HSC galaxies were binned in color magnitude space with i-band mag from -2 to 6 and g-z color from 13 to 26.
+        """HSC galaxies were binned in color magnitude space with i-band mag
+        from -2 to 6 and g-z color from 13 to 26.
         """
         mask = (data[self.config.colnames["i"]] > 13.0) & (
             data[self.config.colnames["i"]] < 26.0
         )
         self.mask &= mask
         gz = data[self.config.colnames["g"]] - data[self.config.colnames["z"]]
         mask = (gz > -2.0) & (gz < 6.0)
         self.mask &= mask
 
     def speczSuccess(self, data):
-        """
-        HSC galaxies were binned in color magnitude space with i-band mag from -2 to 6 and g-z color from 13 to 26
-        200 bins in each direction. The ratio of of galaxies with spectroscopic redshifts (training galaxies) to
-        galaxies with only photometry in HSC wide field (application galaxies) was computed for each pixel. We divide
-        the data into the same pixels and randomly select galaxies into the training sample based on the HSC ratios
+        """HSC galaxies were binned in color magnitude space with i-band mag 
+        from -2 to 6 and g-z color from 13 to 26 (200 bins in each direction). 
+        The ratio of galaxies with spectroscopic redshifts (training galaxies) 
+        to galaxies with only photometry in HSC wide field (application 
+        galaxies) was computed for each pixel. We divide the data into the same
+        pixels and randomly select galaxies into the training sample based on 
+        the HSC ratios.
         """
         success_rate_dir = self.config.success_rate_dir
         x_edge = np.linspace(13, 26, 201, endpoint=True)
         y_edge = np.linspace(-2, 6, 201, endpoint=True)
 
         rates = np.loadtxt(os.path.join(success_rate_dir, "hsc_success.txt"))
 
@@ -604,14 +596,12 @@
         self.mask &= mask
 
     def selection(self, data):
         self.photometryCut(data)
         self.speczSuccess(data)
 
     def __repr__(self):
-        """
-        Define how the model is represented and printed.
-        """
+        """Defines how the model is represented and printed."""
         # start message
         printMsg = "Applying the HSC selection."
 
-        return printMsg
+        return printMsg
```

### Comparing `pz-rail-astro-tools-0.1.2/src/rail/creation/engines/gcr_engine.py` & `pz_rail_astro_tools-0.1.3/src/rail/creation/engines/gcr_engine.py`

 * *Files identical despite different names*

### Comparing `pz-rail-astro-tools-0.1.2/src/rail/examples_data/creation_data/data/hsc_ratios_and_specz.hdf5` & `pz_rail_astro_tools-0.1.3/src/rail/examples_data/creation_data/data/hsc_ratios_and_specz.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-astro-tools-0.1.2/src/rail/examples_data/creation_data/data/survey_conditions/DC2-dr6-galcounts-i20-i25.3-nside-128.fits` & `pz_rail_astro_tools-0.1.3/src/rail/examples_data/creation_data/data/survey_conditions/DC2-dr6-galcounts-i20-i25.3-nside-128.fits`

 * *Files identical despite different names*

### Comparing `pz-rail-astro-tools-0.1.2/src/rail/examples_data/creation_data/data/survey_conditions/DC2-mask-neg-nside-128.fits` & `pz_rail_astro_tools-0.1.3/src/rail/examples_data/creation_data/data/survey_conditions/DC2-mask-neg-nside-128.fits`

 * *Files identical despite different names*

### Comparing `pz-rail-astro-tools-0.1.2/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_airmass_i_and_nightlt1825_HEAL.fits` & `pz_rail_astro_tools-0.1.3/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_airmass_i_and_nightlt1825_HEAL.fits`

 * *Files identical despite different names*

### Comparing `pz-rail-astro-tools-0.1.2/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_fiveSigmaDepth_i_and_nightlt1825_HEAL.fits` & `pz_rail_astro_tools-0.1.3/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_fiveSigmaDepth_i_and_nightlt1825_HEAL.fits`

 * *Files identical despite different names*

### Comparing `pz-rail-astro-tools-0.1.2/src/rail/tools/util_photometry.py` & `pz_rail_astro_tools-0.1.3/src/rail/tools/util_photometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -411,26 +411,27 @@
         self.run()
         return self.get_handle('output')
 
 
 class Dereddener(RailStage):
     """Utility stage that does dereddening
     
-    Note: set copy_cols="ALL" to copy all 
-    columns in data
+    Note: set copy_all_cols=True to copy all 
+    columns in data, copy_cols will be ignored
     """
     name = 'Dereddener'
 
     config_options = RailStage.config_options.copy()
     config_options.update(bands='ugrizy')
     config_options.update(mag_name="mag_{band}_lsst")
     config_options.update(band_a_env=[4.81,3.64,2.70,2.06,1.58,1.31])
     config_options.update(dustmap_name='sfd')
     config_options.update(dustmap_dir=str)
     config_options.update(copy_cols=[])
+    config_options.update(copy_all_cols=False)
 
     inputs = [('input', Hdf5Handle)]
     outputs = [('output', Hdf5Handle)]
 
     def fetch_map(self):
         dust_map_dict = dict(sfd=dustmaps_sfd)
         try:
@@ -466,20 +467,20 @@
         ebvvec = dust_map(coords)
         band_mag_name_list=[]
         for i, band_ in enumerate(self.config.bands):
             band_mag_name = self.config.mag_name.format(band=band_)
             mag_vals = data[band_mag_name]
             out_data[band_mag_name] = mag_vals - ebvvec*self.config.band_a_env[i]
             band_mag_name_list.append(band_mag_name)
-        
-        # check if copy_cols is a list, or is set to ALL:
-        if isinstance(self.config.copy_cols, list): # pragma: no cover
+       
+        # check if copy_all_cols set to true:
+        if self.config.copy_all_cols==False: # pragma: no cover
             for col_ in self.config.copy_cols:  # pragma: no cover
                 out_data[col_] = data[col_]
-        elif self.config.copy_cols=="ALL": # pragma: no cover
+        elif self.config.copy_all_cols==True: # pragma: no cover
             for col_ in data:
                 # make sure we do not overwrite the photometry columns
                 if col_ not in band_mag_name_list:
                     out_data[col_] = data[col_]
 
         self.add_data('output', out_data)
```

### Comparing `pz-rail-astro-tools-0.1.2/tests/astro_tools/gcr_test_data/schema.yaml` & `pz_rail_astro_tools-0.1.3/tests/astro_tools/gcr_test_data/schema.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-astro-tools-0.1.2/tests/astro_tools/gcr_test_data/test_object_tract_4850.hdf5` & `pz_rail_astro_tools-0.1.3/tests/astro_tools/gcr_test_data/test_object_tract_4850.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-astro-tools-0.1.2/tests/astro_tools/test_core.py` & `pz_rail_astro_tools-0.1.3/tests/astro_tools/test_core.py`

 * *Files identical despite different names*

### Comparing `pz-rail-astro-tools-0.1.2/tests/astro_tools/test_degraders.py` & `pz_rail_astro_tools-0.1.3/tests/astro_tools/test_degraders.py`

 * *Files 25% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     """Test bad parameters that should raise ValueError"""
     with pytest.raises(errortype):
         InvRedshiftIncompleteness.make_stage(pivot_redshift=pivot_redshift)
 
 
 def test_InvRedshiftIncompleteness_returns_correct_shape(data):
     """Make sure returns same number of columns, fewer rows"""
-    degrader = InvRedshiftIncompleteness.make_stage(pivot_redshift=1.0)
+    degrader = InvRedshiftIncompleteness.make_stage(pivot_redshift=1.0, seed = 12345)
     degraded_data = degrader(data).data
     assert degraded_data.shape[0] < data.data.shape[0]
     assert degraded_data.shape[1] == data.data.shape[1]
     os.remove(degrader.get_output(degrader.get_aliased_tag("output"), final_name=True))
 
 
 @pytest.mark.parametrize(
@@ -98,21 +98,93 @@
 def test_GridSelection_bad_params(percentile_cut, redshift_cut, errortype):
     """Test bad parameters that should raise ValueError"""
     with pytest.raises(errortype):
         GridSelection.make_stage(percentile_cut=percentile_cut, redshift_cut=redshift_cut)
 
 
 def test_GridSelection_returns_correct_shape(data):
-    """Make sure returns 2 more columns, fewer rows"""
+    """Make sure returns same number of columns, fewer rows"""
     degrader = GridSelection.make_stage(pessimistic_redshift_cut=1.0)
     degraded_data = degrader(data).data
     assert degraded_data.shape[0] < data.data.shape[0]
-    assert degraded_data.shape[1] == data.data.shape[1] - 1
+    assert degraded_data.shape[1] == data.data.shape[1] 
     os.remove(degrader.get_output(degrader.get_aliased_tag("output"), final_name=True))
 
+    
+
+def test_SpecSelection(data):
+    bands = ["u", "g", "r", "i", "z", "y"]
+    band_dict = {band: f"mag_{band}_lsst" for band in bands}
+    rename_dict = {f"{band}_err": f"mag_err_{band}_lsst" for band in bands}
+    rename_dict.update({f"{band}": f"mag_{band}_lsst" for band in bands})
+    standard_colnames = [f"mag_{band}_lsst" for band in "ugrizy"]
+
+    col_remapper_test = ColumnMapper.make_stage(
+        name="col_remapper_test", hdf5_groupname="", columns=rename_dict
+    )
+    data = col_remapper_test(data)
+
+    degrader_GAMA = SpecSelection_GAMA.make_stage()
+    degrader_GAMA(data)
+    degrader_GAMA.__repr__()
+
+    os.remove(degrader_GAMA.get_output(degrader_GAMA.get_aliased_tag("output"), final_name=True))
+
+    degrader_BOSS = SpecSelection_BOSS.make_stage()
+    degrader_BOSS(data)
+    degrader_BOSS.__repr__()
+
+    os.remove(degrader_BOSS.get_output(degrader_BOSS.get_aliased_tag("output"), final_name=True))
+
+    degrader_DEEP2 = SpecSelection_DEEP2.make_stage()
+    degrader_DEEP2(data)
+    degrader_DEEP2.__repr__()
+
+    os.remove(degrader_DEEP2.get_output(degrader_DEEP2.get_aliased_tag("output"), final_name=True))
+
+    degrader_VVDSf02 = SpecSelection_VVDSf02.make_stage()
+    degrader_VVDSf02(data)
+    degrader_VVDSf02.__repr__()
+
+    degrader_zCOSMOS = SpecSelection_zCOSMOS.make_stage(colnames={"i": "mag_i_lsst", "redshift": "redshift"})
+    degrader_zCOSMOS(data)
+    degrader_zCOSMOS.__repr__()
+
+    os.remove(degrader_zCOSMOS.get_output(degrader_zCOSMOS.get_aliased_tag("output"), final_name=True))
+
+    degrader_HSC = SpecSelection_HSC.make_stage()
+    degrader_HSC(data)
+    degrader_HSC.__repr__()
+
+    os.remove(degrader_HSC.get_output(degrader_HSC.get_aliased_tag("output"), final_name=True))
+
+    degrader_HSC = SpecSelection_HSC.make_stage(percentile_cut=70)
+    degrader_HSC(data)
+    degrader_HSC.__repr__()
+
+    os.remove(degrader_HSC.get_output(degrader_HSC.get_aliased_tag("output"), final_name=True))
+
+
+def test_SpecSelection_low_N_tot(data_forspec):
+    bands = ["u", "g", "r", "i", "z", "y"]
+    band_dict = {band: f"mag_{band}_lsst" for band in bands}
+    rename_dict = {f"{band}_err": f"mag_err_{band}_lsst" for band in bands}
+    rename_dict.update({f"{band}": f"mag_{band}_lsst" for band in bands})
+    standard_colnames = [f"mag_{band}_lsst" for band in "ugrizy"]
+
+    col_remapper_test = ColumnMapper.make_stage(
+        name="col_remapper_test", hdf5_groupname="", columns=rename_dict
+    )
+    data_forspec = col_remapper_test(data_forspec)
+
+    degrader_zCOSMOS = SpecSelection_zCOSMOS.make_stage(N_tot=1)
+    degrader_zCOSMOS(data_forspec)
+
+    os.remove(degrader_zCOSMOS.get_output(degrader_zCOSMOS.get_aliased_tag("output"), final_name=True))
+
 
 @pytest.mark.parametrize("N_tot, errortype", [(-1, ValueError)])
 def test_SpecSelection_bad_params(N_tot, errortype):
     """Test bad parameters that should raise TypeError"""
     with pytest.raises(errortype):
         SpecSelection.make_stage(N_tot=N_tot)
```

### Comparing `pz-rail-astro-tools-0.1.2/tests/astro_tools/test_gcr_engine.py` & `pz_rail_astro_tools-0.1.3/tests/astro_tools/test_gcr_engine.py`

 * *Files identical despite different names*

