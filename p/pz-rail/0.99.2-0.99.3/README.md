# Comparing `tmp/pz-rail-0.99.2.tar.gz` & `tmp/pz_rail-0.99.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-rail-0.99.2.tar", last modified: Fri Nov  3 00:14:45 2023, max compression
+gzip compressed data, was "pz_rail-0.99.3.tar", last modified: Wed Apr 24 01:18:43 2024, max compression
```

## Comparing `pz-rail-0.99.2.tar` & `pz_rail-0.99.3.tar`

### file list

```diff
@@ -1,114 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 00:14:45.065309 pz-rail-0.99.2/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2023-11-03 00:14:17.000000 pz-rail-0.99.2/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (127)      123 2023-11-03 00:14:17.000000 pz-rail-0.99.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 00:14:45.041308 pz-rail-0.99.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 00:14:45.045308 pz-rail-0.99.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2023-11-03 00:14:17.000000 pz-rail-0.99.2/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      661 2023-11-03 00:14:17.000000 pz-rail-0.99.2/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      707 2023-11-03 00:14:17.000000 pz-rail-0.99.2/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      783 2023-11-03 00:14:17.000000 pz-rail-0.99.2/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 00:14:45.045308 pz-rail-0.99.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2023-11-03 00:14:17.000000 pz-rail-0.99.2/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (127)      914 2023-11-03 00:14:17.000000 pz-rail-0.99.2/.github/workflows/build_documentation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2023-11-03 00:14:17.000000 pz-rail-0.99.2/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      950 2023-11-03 00:14:17.000000 pz-rail-0.99.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2023-11-03 00:14:17.000000 pz-rail-0.99.2/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2023-11-03 00:14:17.000000 pz-rail-0.99.2/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2023-11-03 00:14:17.000000 pz-rail-0.99.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2023-11-03 00:14:17.000000 pz-rail-0.99.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      689 2023-11-03 00:14:17.000000 pz-rail-0.99.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2023-11-03 00:14:17.000000 pz-rail-0.99.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6049 2023-11-03 00:14:45.065309 pz-rail-0.99.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2023-11-03 00:14:17.000000 pz-rail-0.99.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-11-03 00:14:17.000000 pz-rail-0.99.2/conda-reqs.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 00:14:45.045308 pz-rail-0.99.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      655 2023-11-03 00:14:17.000000 pz-rail-0.99.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 00:14:45.033308 pz-rail-0.99.2/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 00:14:45.045308 pz-rail-0.99.2/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2023-11-03 00:14:17.000000 pz-rail-0.99.2/docs/_static/css/notebooks.css
--rw-r--r--   0 runner    (1001) docker     (127)     6431 2023-11-03 00:14:17.000000 pz-rail-0.99.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2023-11-03 00:14:17.000000 pz-rail-0.99.2/docs/demos.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2023-11-03 00:14:17.000000 pz-rail-0.99.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-11-03 00:14:17.000000 pz-rail-0.99.2/docs/nbconvert-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-11-03 00:14:17.000000 pz-rail-0.99.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 00:14:45.045308 pz-rail-0.99.2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2023-11-03 00:14:17.000000 pz-rail-0.99.2/docs/source/citing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7751 2023-11-03 00:14:17.000000 pz-rail-0.99.2/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4902 2023-11-03 00:14:17.000000 pz-rail-0.99.2/docs/source/demonstrations.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2023-11-03 00:14:17.000000 pz-rail-0.99.2/docs/source/fix_an_issue.rst
--rw-r--r--   0 runner    (1001) docker     (127)    16094 2023-11-03 00:14:17.000000 pz-rail-0.99.2/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2023-11-03 00:14:17.000000 pz-rail-0.99.2/docs/source/new_algorithm.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6138 2023-11-03 00:14:17.000000 pz-rail-0.99.2/docs/source/new_rail_stage.rst
--rw-r--r--   0 runner    (1001) docker     (127)    13974 2023-11-03 00:14:17.000000 pz-rail-0.99.2/docs/source/overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3363 2023-11-03 00:14:17.000000 pz-rail-0.99.2/docs/source/sharing_pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (127)      247 2023-11-03 00:14:17.000000 pz-rail-0.99.2/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 00:14:45.049309 pz-rail-0.99.2/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-11-03 00:14:17.000000 pz-rail-0.99.2/examples/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 00:14:45.053309 pz-rail-0.99.2/examples/core_examples/
--rw-r--r--   0 runner    (1001) docker     (127)    10879 2023-11-03 00:14:17.000000 pz-rail-0.99.2/examples/core_examples/Build_Save_Load_Run_Pipeline.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    14986 2023-11-03 00:14:17.000000 pz-rail-0.99.2/examples/core_examples/FileIO_DataStore.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6359 2023-11-03 00:14:17.000000 pz-rail-0.99.2/examples/core_examples/FluxtoMag_and_Deredden_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5252 2023-11-03 00:14:17.000000 pz-rail-0.99.2/examples/core_examples/Iterate_Tabular_Data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2023-11-03 00:14:17.000000 pz-rail-0.99.2/examples/core_examples/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2023-11-03 00:14:17.000000 pz-rail-0.99.2/examples/core_examples/Run_Saved_Pipeline.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    13836 2023-11-03 00:14:17.000000 pz-rail-0.99.2/examples/core_examples/Useful_Utilities.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      275 2023-11-03 00:14:17.000000 pz-rail-0.99.2/examples/core_examples/cleanup.sh
--rw-r--r--   0 runner    (1001) docker     (127)     8447 2023-11-03 00:14:17.000000 pz-rail-0.99.2/examples/core_examples/hyperbolic_magnitude_test.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      610 2023-11-03 00:14:17.000000 pz-rail-0.99.2/examples/core_examples/pipe_example.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2023-11-03 00:14:17.000000 pz-rail-0.99.2/examples/core_examples/pipe_example_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 00:14:45.057309 pz-rail-0.99.2/examples/creation_examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2023-11-03 00:14:17.000000 pz-rail-0.99.2/examples/creation_examples/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      227 2023-11-03 00:14:17.000000 pz-rail-0.99.2/examples/creation_examples/cleanup.sh
--rw-r--r--   0 runner    (1001) docker     (127)    18074 2023-11-03 00:14:17.000000 pz-rail-0.99.2/examples/creation_examples/degradation-demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    17118 2023-11-03 00:14:17.000000 pz-rail-0.99.2/examples/creation_examples/dsps_sed_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11809 2023-11-03 00:14:17.000000 pz-rail-0.99.2/examples/creation_examples/example_GridSelection_for_HSC.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    14843 2023-11-03 00:14:17.000000 pz-rail-0.99.2/examples/creation_examples/example_ObsConditions.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9426 2023-11-03 00:14:17.000000 pz-rail-0.99.2/examples/creation_examples/example_SpecSelection_for_zCOSMOS.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11833 2023-11-03 00:14:17.000000 pz-rail-0.99.2/examples/creation_examples/photometric_realization_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    66554 2023-11-03 00:14:17.000000 pz-rail-0.99.2/examples/creation_examples/plotting_interface_skysim_cosmoDC2_COSMOS2020_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    19565 2023-11-03 00:14:17.000000 pz-rail-0.99.2/examples/creation_examples/posterior-demo.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 00:14:45.061309 pz-rail-0.99.2/examples/estimation_examples/
--rw-r--r--   0 runner    (1001) docker     (127)    16779 2023-11-03 00:14:17.000000 pz-rail-0.99.2/examples/estimation_examples/CMNN_Demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12434 2023-11-03 00:14:17.000000 pz-rail-0.99.2/examples/estimation_examples/Fzboost_PDF_Representation_Comparison.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8664 2023-11-03 00:14:17.000000 pz-rail-0.99.2/examples/estimation_examples/GPz_estimation_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    19353 2023-11-03 00:14:17.000000 pz-rail-0.99.2/examples/estimation_examples/NZDir.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    26158 2023-11-03 00:14:17.000000 pz-rail-0.99.2/examples/estimation_examples/RAIL_estimation_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      871 2023-11-03 00:14:17.000000 pz-rail-0.99.2/examples/estimation_examples/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    28442 2023-11-03 00:14:17.000000 pz-rail-0.99.2/examples/estimation_examples/SimpleSOM_demo.ipynb.fixme
--rw-r--r--   0 runner    (1001) docker     (127)      459 2023-11-03 00:14:17.000000 pz-rail-0.99.2/examples/estimation_examples/cleanup.sh
--rw-r--r--   0 runner    (1001) docker     (127)     5249 2023-11-03 00:14:17.000000 pz-rail-0.99.2/examples/estimation_examples/nzdir_as_pipeline.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    30493 2023-11-03 00:14:17.000000 pz-rail-0.99.2/examples/estimation_examples/somocluSOM_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    36863 2023-11-03 00:14:17.000000 pz-rail-0.99.2/examples/estimation_examples/somocluSOMcluster_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    20949 2023-11-03 00:14:17.000000 pz-rail-0.99.2/examples/estimation_examples/test_sampled_summarizers.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 00:14:45.061309 pz-rail-0.99.2/examples/evaluation_examples/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-11-03 00:14:17.000000 pz-rail-0.99.2/examples/evaluation_examples/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      340 2023-11-03 00:14:17.000000 pz-rail-0.99.2/examples/evaluation_examples/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      142 2023-11-03 00:14:17.000000 pz-rail-0.99.2/examples/evaluation_examples/cleanup.sh
--rw-r--r--   0 runner    (1001) docker     (127)    18347 2023-11-03 00:14:17.000000 pz-rail-0.99.2/examples/evaluation_examples/demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    19193 2023-11-03 00:14:17.000000 pz-rail-0.99.2/examples/evaluation_examples/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 00:14:45.061309 pz-rail-0.99.2/examples/goldenspike_examples/
--rw-r--r--   0 runner    (1001) docker     (127)      714 2023-11-03 00:14:17.000000 pz-rail-0.99.2/examples/goldenspike_examples/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2023-11-03 00:14:17.000000 pz-rail-0.99.2/examples/goldenspike_examples/cleanup.sh
--rw-r--r--   0 runner    (1001) docker     (127)      310 2023-11-03 00:14:17.000000 pz-rail-0.99.2/examples/goldenspike_examples/cleanup_pipeline.sh
--rw-r--r--   0 runner    (1001) docker     (127)    25671 2023-11-03 00:14:17.000000 pz-rail-0.99.2/examples/goldenspike_examples/goldenspike.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2023-11-03 00:14:17.000000 pz-rail-0.99.2/examples/goldenspike_examples/goldenspike.yml
--rw-r--r--   0 runner    (1001) docker     (127)     9222 2023-11-03 00:14:17.000000 pz-rail-0.99.2/examples/goldenspike_examples/goldenspike_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2023-11-03 00:14:17.000000 pz-rail-0.99.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      364 2023-11-03 00:14:17.000000 pz-rail-0.99.2/rail_packages.yml
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-11-03 00:14:17.000000 pz-rail-0.99.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-03 00:14:45.065309 pz-rail-0.99.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-11-03 00:14:17.000000 pz-rail-0.99.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 00:14:45.037309 pz-rail-0.99.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 00:14:45.061309 pz-rail-0.99.2/src/pz_rail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6049 2023-11-03 00:14:44.000000 pz-rail-0.99.2/src/pz_rail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2023-11-03 00:14:45.000000 pz-rail-0.99.2/src/pz_rail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-03 00:14:44.000000 pz-rail-0.99.2/src/pz_rail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      303 2023-11-03 00:14:44.000000 pz-rail-0.99.2/src/pz_rail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-11-03 00:14:44.000000 pz-rail-0.99.2/src/pz_rail.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 00:14:45.037309 pz-rail-0.99.2/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 00:14:45.061309 pz-rail-0.99.2/src/rail/hub/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-11-03 00:14:17.000000 pz-rail-0.99.2/src/rail/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2023-11-03 00:14:44.000000 pz-rail-0.99.2/src/rail/hub/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 00:14:45.037309 pz-rail-0.99.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 00:14:45.061309 pz-rail-0.99.2/tests/hub/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-11-03 00:14:17.000000 pz-rail-0.99.2/tests/hub/test_import.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:18:43.493364 pz_rail-0.99.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-24 01:18:33.000000 pz_rail-0.99.3/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-24 01:18:33.000000 pz_rail-0.99.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:18:43.477364 pz_rail-0.99.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:18:43.477364 pz_rail-0.99.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-24 01:18:33.000000 pz_rail-0.99.3/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-24 01:18:33.000000 pz_rail-0.99.3/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-24 01:18:33.000000 pz_rail-0.99.3/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-24 01:18:33.000000 pz_rail-0.99.3/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:18:43.477364 pz_rail-0.99.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-24 01:18:33.000000 pz_rail-0.99.3/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-24 01:18:33.000000 pz_rail-0.99.3/.github/workflows/build_documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-24 01:18:33.000000 pz_rail-0.99.3/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-24 01:18:33.000000 pz_rail-0.99.3/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-04-24 01:18:33.000000 pz_rail-0.99.3/.github/workflows/smoke-test-head.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-24 01:18:33.000000 pz_rail-0.99.3/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-24 01:18:33.000000 pz_rail-0.99.3/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-24 01:18:33.000000 pz_rail-0.99.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-24 01:18:33.000000 pz_rail-0.99.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-24 01:18:33.000000 pz_rail-0.99.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-24 01:18:33.000000 pz_rail-0.99.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-04-24 01:18:43.493364 pz_rail-0.99.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-04-24 01:18:33.000000 pz_rail-0.99.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-24 01:18:33.000000 pz_rail-0.99.3/conda-reqs.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:18:43.477364 pz_rail-0.99.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-24 01:18:33.000000 pz_rail-0.99.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:18:43.473364 pz_rail-0.99.3/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:18:43.477364 pz_rail-0.99.3/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-24 01:18:33.000000 pz_rail-0.99.3/docs/_static/css/notebooks.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-04-24 01:18:33.000000 pz_rail-0.99.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-24 01:18:33.000000 pz_rail-0.99.3/docs/demos.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-24 01:18:33.000000 pz_rail-0.99.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-24 01:18:33.000000 pz_rail-0.99.3/docs/nbconvert-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-24 01:18:33.000000 pz_rail-0.99.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:18:43.481364 pz_rail-0.99.3/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-24 01:18:33.000000 pz_rail-0.99.3/docs/source/citing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-04-24 01:18:33.000000 pz_rail-0.99.3/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-04-24 01:18:33.000000 pz_rail-0.99.3/docs/source/demonstrations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-24 01:18:33.000000 pz_rail-0.99.3/docs/source/fix_an_issue.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    17570 2024-04-24 01:18:33.000000 pz_rail-0.99.3/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-24 01:18:33.000000 pz_rail-0.99.3/docs/source/new_algorithm.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-04-24 01:18:33.000000 pz_rail-0.99.3/docs/source/new_rail_stage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    13974 2024-04-24 01:18:33.000000 pz_rail-0.99.3/docs/source/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-04-24 01:18:33.000000 pz_rail-0.99.3/docs/source/sharing_pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-24 01:18:33.000000 pz_rail-0.99.3/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:18:43.481364 pz_rail-0.99.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:18:43.481364 pz_rail-0.99.3/examples/core_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    11369 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/core_examples/Build_Save_Load_Run_Pipeline.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    14986 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/core_examples/FileIO_DataStore.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6359 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/core_examples/FluxtoMag_and_Deredden_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/core_examples/Iterate_Tabular_Data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/core_examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/core_examples/Run_Saved_Pipeline.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    13855 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/core_examples/Useful_Utilities.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/core_examples/cleanup.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     8447 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/core_examples/hyperbolic_magnitude_test.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/core_examples/pipe_example.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/core_examples/pipe_example_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:18:43.485364 pz_rail-0.99.3/examples/creation_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/creation_examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/creation_examples/cleanup.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    18074 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/creation_examples/degradation-demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    17118 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/creation_examples/dsps_sed_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11809 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/creation_examples/example_GridSelection_for_HSC.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    14843 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/creation_examples/example_ObsConditions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9426 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/creation_examples/example_SpecSelection_for_zCOSMOS.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    21721 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/creation_examples/fsps_sed_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11833 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/creation_examples/photometric_realization_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    66554 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/creation_examples/plotting_interface_skysim_cosmoDC2_COSMOS2020_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    19565 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/creation_examples/posterior-demo.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:18:43.485364 pz_rail-0.99.3/examples/estimation_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    34096 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/estimation_examples/BPZ_lite_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    22684 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/estimation_examples/BPZ_lite_with_custom_SEDs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    16877 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/estimation_examples/CMNN_Demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12320 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/estimation_examples/Fzboost_PDF_Representation_Comparison.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8664 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/estimation_examples/GPz_estimation_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    19361 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/estimation_examples/NZDir.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    25938 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/estimation_examples/RAIL_estimation_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/estimation_examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    28442 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/estimation_examples/SimpleSOM_demo.ipynb.fixme
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/estimation_examples/cleanup.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/estimation_examples/nzdir_as_pipeline.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    30501 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/estimation_examples/somocluSOM_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    36871 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/estimation_examples/somocluSOMcluster_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    20794 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/estimation_examples/test_sampled_summarizers.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:18:43.489364 pz_rail-0.99.3/examples/evaluation_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/evaluation_examples/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    18248 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/evaluation_examples/Evaluation_Demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    29795 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/evaluation_examples/Evaluation_by_type.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/evaluation_examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/evaluation_examples/cleanup.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    19193 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/evaluation_examples/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:18:43.489364 pz_rail-0.99.3/examples/goldenspike_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/goldenspike_examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/goldenspike_examples/cleanup.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/goldenspike_examples/cleanup_pipeline.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    25361 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/goldenspike_examples/goldenspike.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/goldenspike_examples/goldenspike.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     9222 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/goldenspike_examples/goldenspike_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-24 01:18:33.000000 pz_rail-0.99.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-24 01:18:33.000000 pz_rail-0.99.3/rail_packages.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-24 01:18:33.000000 pz_rail-0.99.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 01:18:43.493364 pz_rail-0.99.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 01:18:33.000000 pz_rail-0.99.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:18:43.473364 pz_rail-0.99.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:18:43.489364 pz_rail-0.99.3/src/pz_rail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-04-24 01:18:43.000000 pz_rail-0.99.3/src/pz_rail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-04-24 01:18:43.000000 pz_rail-0.99.3/src/pz_rail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 01:18:43.000000 pz_rail-0.99.3/src/pz_rail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-24 01:18:43.000000 pz_rail-0.99.3/src/pz_rail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 01:18:43.000000 pz_rail-0.99.3/src/pz_rail.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:18:43.473364 pz_rail-0.99.3/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:18:43.489364 pz_rail-0.99.3/src/rail/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-24 01:18:33.000000 pz_rail-0.99.3/src/rail/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-24 01:18:43.000000 pz_rail-0.99.3/src/rail/hub/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:18:43.473364 pz_rail-0.99.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:18:43.489364 pz_rail-0.99.3/tests/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-24 01:18:33.000000 pz_rail-0.99.3/tests/hub/test_import.py
```

### Comparing `pz-rail-0.99.2/.github/ISSUE_TEMPLATE/1-bug_report.md` & `pz_rail-0.99.3/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/.github/ISSUE_TEMPLATE/2-feature_request.md` & `pz_rail-0.99.3/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/.github/pull_request_template.md` & `pz_rail-0.99.3/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/.github/workflows/build_documentation.yml` & `pz_rail-0.99.3/.github/workflows/build_documentation.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/.github/workflows/linting.yml` & `pz_rail-0.99.3/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/.github/workflows/publish-to-pypi.yml` & `pz_rail-0.99.3/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/.github/workflows/smoke-test.yml` & `pz_rail-0.99.3/.github/workflows/smoke-test.yml`

 * *Files 8% similar despite different names*

```diff
@@ -31,19 +31,23 @@
         pip install wheel numpy
         pip install .
         pip install .[dev]
         if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
     - name: Run unit tests with pytest
       run: |
         python -m pytest tests
+    - name: Set up fsps
+      run: |
+        git clone "https://github.com/cconroy20/fsps.git" "/opt/hostedtoolcache/Python/fsps"
+        echo "SPS_HOME=/opt/hostedtoolcache/Python/fsps" >> $GITHUB_ENV
     - name: Run notebooks
       run: |
         rail render-nb --skip examples/creation_examples/plotting_interface_skysim_cosmoDC2_COSMOS2020_demo.ipynb examples/${{ matrix.notebook-dir }}_examples/*.ipynb
     - name: Send status to Slack app (RAIL CI Reporter)
-      if: ${{ failure() }}
+      if: ${{ failure() && github.event_name != 'workflow_dispatch' }}
       id: slack
       uses: slackapi/slack-github-action@v1.24.0
       with:
         # For posting a rich message using Block Kit
         payload: |
           {
             "blocks": [
```

### Comparing `pz-rail-0.99.2/.github/workflows/testing-and-coverage.yml` & `pz_rail-0.99.3/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/.gitignore` & `pz_rail-0.99.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/.pre-commit-config.yaml` & `pz_rail-0.99.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/.readthedocs.yaml` & `pz_rail-0.99.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/LICENSE` & `pz_rail-0.99.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/PKG-INFO` & `pz_rail-0.99.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail
-Version: 0.99.2
+Version: 0.99.3
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -31,21 +31,31 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pz-rail-base
 Provides-Extra: algos
-Requires-Dist: pz-rail-pipelines[full]; extra == "algos"
+Requires-Dist: pz-rail-astro-tools; extra == "algos"
+Requires-Dist: pz-rail-bpz; extra == "algos"
+Requires-Dist: pz-rail-cmnn; extra == "algos"
+Requires-Dist: pz-rail-dsps; extra == "algos"
+Requires-Dist: pz-rail-flexzboost; extra == "algos"
+Requires-Dist: pz-rail-fsps; extra == "algos"
+Requires-Dist: pz-rail-gpz-v1; extra == "algos"
+Requires-Dist: pz-rail-pzflow; extra == "algos"
+Requires-Dist: pz-rail-sklearn; extra == "algos"
+Requires-Dist: pz-rail-som; extra == "algos"
+Requires-Dist: qp-prob[full]; extra == "algos"
 Provides-Extra: nb
-Requires-Dist: pz-rail-pipelines[full]; extra == "nb"
+Requires-Dist: pz-rail[algos]; extra == "nb"
 Requires-Dist: jupyter; extra == "nb"
 Requires-Dist: seaborn; extra == "nb"
 Provides-Extra: dev
-Requires-Dist: pz-rail-pipelines[full]; extra == "dev"
+Requires-Dist: pz-rail[algos]; extra == "dev"
 Requires-Dist: jupyter; extra == "dev"
 Requires-Dist: seaborn; extra == "dev"
 Requires-Dist: corner; extra == "dev"
 Requires-Dist: pandas; extra == "dev"
 Requires-Dist: h5py; extra == "dev"
 Requires-Dist: matplotlib; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
```

### Comparing `pz-rail-0.99.2/README.md` & `pz_rail-0.99.3/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/docs/Makefile` & `pz_rail-0.99.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/docs/_static/css/notebooks.css` & `pz_rail-0.99.3/docs/_static/css/notebooks.css`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/docs/conf.py` & `pz_rail-0.99.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/docs/demos.rst` & `pz_rail-0.99.3/docs/demos.rst`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/docs/index.rst` & `pz_rail-0.99.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/docs/source/citing.rst` & `pz_rail-0.99.3/docs/source/citing.rst`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/docs/source/contributing.rst` & `pz_rail-0.99.3/docs/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/docs/source/demonstrations.rst` & `pz_rail-0.99.3/docs/source/demonstrations.rst`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/docs/source/fix_an_issue.rst` & `pz_rail-0.99.3/docs/source/fix_an_issue.rst`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/docs/source/installation.rst` & `pz_rail-0.99.3/docs/source/installation.rst`

 * *Files 18% similar despite different names*

```diff
@@ -14,39 +14,64 @@
 
 1. `Exploration Installation`_: install all of the RAIL algorithms and explore RAIL using a series of demonstration jupyter notebooks.
 2. `Production Installation`_: install all of the RAIL algorithms in an existing conda environment.
 3. `Algorithm Installation`_  install a single RAIL algorithm in an existing conda environment.
 4. `Developer Installation`_: install all of RAIL algorithms from source in "editable" mode.
 
 
+.. note::
+    In the following instructions you will see the use of both ``pip`` and ``conda``.
+    We have found that ``conda`` is particularly good at creating virtual environments
+    and installing packages that have compiled libraries. Thus we prefer it over
+    ``pip`` and ``venv`` for those purposes.
+
+    Additionally, we use ``pip`` to build and install RAIL code from source because
+    ``conda`` does not provide that functionality.
+
+.. tip::
+
+    Throughout the installation documentation we make reference to ``conda`` as
+    a tool to create a RAIL virtual environment and install compiled dependencies
+    we acknowledge that it can be potentially very slow. Using ``mamba`` can be
+    significantly faster, but it is not as widely adopted in the community.
+
+    If you would like to experiment with ``mamba`` it can be installed with
+    ``conda install mamba -n base -c conda-forge``. The ``mamba`` documentation
+    is `here <https://mamba.readthedocs.io/>`_.
+
 Exploration Installation
 ------------------------
 
-Here we will be installing the source code from `rail <https://github.com/LSSTDESC/rail>`_ to access all of the demonstration notebooks, and using that to install all of the other alo
+Here we will be installing the source code from `rail <https://github.com/LSSTDESC/rail>`_
+to access all of the demonstration notebooks, and use that to install all of the other algorithms.
 
-We have included an `environment.yml` that makes it easy to create a conda environment named "[env]" that uses conda to install some packages that have compiled libraries we have found that it is easier to install with conda.
+We have included an ``environment.yml`` that makes it easy to create a virtual
+environment named "[env]" that uses conda to install some packages that have
+compiled libraries.
 
 .. tabs::
 
    .. group-tab:: General
 
       .. code-block:: bash
 
           git clone https://github.com/LSSTDESC/rail.git
           cd rail
           conda env create -f environment.yml -n [env]  # or mamba env create, which is much faster
           conda activate [env]
-          pip install .[dev]
+          pip install -e .[dev]
 
 
-      If for some reason the `pip install .[dev]` fails (e.g.,because of a problem in building the dependencies for one of the algorithms) you can run a more fault-tolerant installation using a rail script:
+      If for some reason the ``pip install .[dev]`` fails (e.g.,because of a problem
+      in building the dependencies for one of the algorithms) you can run a more
+      fault-tolerant installation using a rail script:
 
       .. code-block:: bash
             
-          pip install .
+          pip install -e .
           rail install --package-file rail_packages.yml
 
 
       At that point you should be able to run the demonstration notebooks, e.g.;
 
       .. code-block:: bash
 
@@ -57,51 +82,57 @@
 
       .. code-block:: bash
 
           git clone https://github.com/LSSTDESC/rail.git
           cd rail
           conda env create -f environment.yml -n [env]  # or mamba env create, which is much faster
           conda activate [env]
-          pip install '.[dev]'
+          pip install -e '.[dev]'
 
 
-      If for some reason the `pip install '.[dev]'` fails (e.g.,because of a problem in building the dependencies for one of the algorithms) you can run a more fault-tolerant installation using a rail script:
+      If for some reason the ``pip install '.[dev]'`` fails (e.g.,because of a
+      problem in building the dependencies for one of the algorithms) you can run
+      a more fault-tolerant installation using a rail script:
 
       .. code-block:: bash
             
-          pip install .
+          pip install -e .
           rail install --package-file rail_packages.yml
 
-                
+
       At that point you should be able to run the demonstration notebooks, e.g.;
 
       .. code-block:: bash
 
           jupyter-notebook examples/estimation_examples/RAIL_estimation_demo.ipynb
 
 
 Production Installation
 -----------------------   
 
-Here we will be installing all of the RAIL algorithms into an existing conda environment "[env]".  To do this we recommend that you install `rail` from source, to be sure to get the latest version of the `conda-reqs.txt` file
+Here we will be installing all of the RAIL algorithms into an existing virtual
+environment "[env]". To do this we recommend that you install ``rail`` from source,
+to be sure to get the latest version of the ``conda-reqs.txt`` file.
 
 .. tabs::
 
    .. group-tab:: General
 
       .. code-block:: bash
   
           git clone https://github.com/LSSTDESC/rail.git
           cd rail
           conda activate [env]
           conda install -n [env] -c conda-forge --file conda-reqs.txt  # or mamba install, which is much faster
           pip install .[algos]
 
 
-      Again, if for some reason the `pip install .[algos]` fails (e.g.,because of a problem in building the dependencies for one of the algorithms) you can run a more fault-tolerant installation using a rail script:
+      Again, if for some reason the ``pip install .[algos]`` fails (e.g.,because
+      of a problem in building the dependencies for one of the algorithms) you
+      can run a more fault-tolerant installation using a rail script:
 
       .. code-block:: bash
             
           pip install .
           rail install --package-file rail_packages.yml
 
 
@@ -112,71 +143,86 @@
           git clone https://github.com/LSSTDESC/rail.git
           cd rail
           conda activate [env]
           conda install -n [env] -c conda-forge --file conda-reqs.txt  # or mamba install, which is much faster
           pip install '.[algos]'
 
 
-      Again, if for some reason the `pip install '.[algos]'` fails (e.g.,because of a problem in building the dependencies for one of the algorithms) you can run a more fault-tolerant installation using a rail script:
+      Again, if for some reason the `pip install '.[algos]'` fails (e.g.,because
+      of a problem in building the dependencies for one of the algorithms) you
+      can run a more fault-tolerant installation using a rail script:
 
       .. code-block:: bash
             
           pip install .
           rail install --package-file rail_packages.yml
 
 
 Algorithm Installation
-----------------------   
+----------------------
 
-Here we will be a single RAIL algorithm (e.g., rail_som) into an existing conda environment "[env]".
+Here we will be installing a single RAIL algorithm (e.g., ``rail_som``) into an
+existing virtual environment "[env]".
 
 .. tabs::
 
    .. group-tab:: General
 
       .. code-block:: bash
 
           conda activate [env]
           pip install pz-rail-som  # (note the name change)
 
 
-      Again, if for some reason that fails because of conflicting dependencies, then adding the dependencies with compiled libraries via conda might fix the issue.  We have included `conda-reqs.txt` file in each RAIL algorithm's repository to specify the dependencies of that algorithm that might best be installed using conda.
+      Again, if for some reason that fails because of conflicting dependencies,
+      then adding the dependencies with compiled libraries via conda might fix
+      the issue.  We have included ``conda-reqs.txt`` file in each RAIL algorithm's
+      repository to specify the dependencies of that algorithm that might best
+      be installed using conda.
 
       .. code-block:: bash
 
           git clone https://github.com/LSSTDESC/rail_som.git
-          cd rail_som    
+          cd rail_som
           conda install -n [env] -c conda-forge --file conda-reqs.txt
-          pip install .		
+          pip install -e .
 
 
    .. group-tab:: zsh (e.g., Mac M1+ default)
 
       .. code-block:: bash
 
           conda activate [env]
           pip install pz-rail-som  # (note the name change)
 
 
-      Again, if for some reason that fails because of conflicting dependencies, then adding the dependencies with compiled libraries via conda might fix the issue.  We have included `conda-reqs.txt` file in each RAIL algorithm's repository to specify the dependencies of that algorithm that might best be installed using conda.
+      Again, if for some reason that fails because of conflicting dependencies,
+      then adding the dependencies with compiled libraries via conda might fix
+      the issue. We have included ``conda-reqs.txt`` file in each RAIL algorithm's
+      repository to specify the dependencies of that algorithm that might best
+      be installed using conda.
 
       .. code-block:: bash
 
           git clone https://github.com/LSSTDESC/rail_som.git
-          cd rail_som    
+          cd rail_som
           conda install -n [env] -c conda-forge --file conda-reqs.txt
-          pip install .		
+          pip install -e .
+
 
-    
 Developer Installation
 ----------------------   
 
-Here we will be installing the source code from `rail <https://github.com/LSSTDESC/rail>`_ to access all of the demonstration notebooks, and using that to install all of the other alo
-
-We have included an `environment.yml` that makes it easy to create a conda environment named "[env]" that uses conda to install some packages that have compiled libraries we have found that it is easier to install with conda.
+Here we will be installing the source code from `rail <https://github.com/LSSTDESC/rail>`_
+to access all of the demonstration notebooks, and using that to install all of the other
+algorithms.
+
+We have included an ``environment.yml`` that makes it easy to create a virtual
+environment named "[env]" that uses conda to install some packages that have
+compiled libraries.
 
 .. tabs::
 
    .. group-tab:: General
 
       .. code-block:: bash
 
@@ -197,22 +243,31 @@
           cd rail
           conda env create -f environment.yml -n [env]  # or mamba env create, which is much faster
           conda activate [env]
           pip install -e .
           rail clone-source --package-file rail_packages.yml
           rail install --package-file rail_packages.yml --from-source 
 
-To update all your rail packages, use the command line tool in the [env]:
 
-```
-rail update-source --package-file rail_packages.yml
-```
-from the root of rail. 
+RAIL Command Line Utility
+=========================
+
+RAIL provides a command line utility to help with installation and maintenance of RAIL.
+The command line utility is called ``rail``.
+You can see the available commands by running ``rail --help``.
+
+The most useful commands are:
+
+- ``rail install``: install RAIL packages from pypi or from source.
+- ``rail update-source``: update RAIL packages from source.
+
+.. tip::
+    To update all your rail packages, in the current environment, use:
+    ``rail update-source --package-file rail_packages.yml`` from the root of rail.
 
-    
 
 RAIL packages
 =============
 
 Depending on how you want to use RAIL you will be installing one or more RAIL packages.  So, first let's clarify the
 RAIL packages structure.
 
@@ -263,15 +318,21 @@
 .. code-block:: bash
 
     git clone https://github.com/LSSTDESC/RAIL.git  # (or whichever packages you need)
     cd RAIL
     pip install -e .[all] # (or pip install -e '.[all]' if you are using zsh, note the single quotes). 
 
 
-If you only want to install the dependencies for a specific piece of RAIL, you can change the install option. E.g. to install only the dependencies for the Creation Module or the Estimation Module, run `pip install .[creation]` or `pip install .[estimation]` respectively. For other install options, look at the keys for the `extras_require` dictionary at the top of `setup.py`.
+If you only want to install the dependencies for a specific piece of RAIL, you
+can change the install option. E.g. to install only the dependencies for the
+Creation Module or the Estimation Module, run ``pip install .[creation]`` or
+``pip install .[estimation]`` respectively.
+
+For other install options, look at the keys for the ``extras_require`` dictionary
+at the top of ``setup.py``.
 
 
 
 Algorithm / architecture specific issues
 ========================================
 
 
@@ -293,67 +354,81 @@
 
       For Delight you should be able to just do:
 
       .. code-block:: bash
 
           pip install pz-rail-delight
 
-      However, the particular estimator `Delight` is built with `Cython` and uses `openmp`.  Mac has dropped native support for `openmp`, which will likely cause problems when trying to run the `DelightEstimator` estimation code in RAIL.  See the notes below for instructions on installing Delight if you wish to use this particular estimator.
+      However, the particular estimator ``Delight`` is built with ``Cython`` and uses ``openmp``.  Mac has dropped native support for ``openmp``, which will likely cause problems when trying to run the ``DelightEstimator`` estimation code in RAIL.  See the notes below for instructions on installing Delight if you wish to use this particular estimator.
 
-      If you are installing RAIL on a Mac, as noted above the `DelightEstimator` estimator requires that your machine's `gcc` be set up to work with `openmp`. If you are installing on a Mac and do not plan on using `DelightEstimator`, then you can simply install RAIL with `pip install .[base]` rather than `pip install .[all]`, which will skip the Delight package.  If you are on a Mac and *do* expect to run `DelightEstimator`, then follow the instructions `here <https://github.com/LSSTDESC/Delight/blob/master/Mac_installation.md>`_ to install Delight before running `pip install .[all]`.
+      If you are installing RAIL on a Mac, as noted above the ``DelightEstimator`` estimator requires that your machine's ``gcc`` be set up to work with ``openmp``. If you are installing on a Mac and do not plan on using ``DelightEstimator``, then you can simply install RAIL with ``pip install .[base]`` rather than ``pip install .[all]``, which will skip the Delight package.  If you are on a Mac and *do* expect to run ``DelightEstimator``, then follow the instructions `here <https://github.com/LSSTDESC/Delight/blob/master/Mac_installation.md>`_ to install Delight before running ``pip install .[all]``.
 
     
 Installing FlexZBoost
 ---------------------
 
 For FlexZBoost, you should be able to just do
 
 .. code-block:: bash
 
     pip install pz-rail-flexzboost
 
 But if you run into problems you might need to:
 
-- install `xgboost` with the command `pip install xgboost==0.90.0`
-- install FlexCode with `pip install FlexCode[all]`
+- install ``xgboost`` with the command ``pip install xgboost==0.90.0``
+- install FlexCode with ``pip install FlexCode[all]``
 
 
 Installing bpz_lite
 -------------------
 
 For bpz_lite, you should be able to just do
 
 .. code-block:: bash
 
     pip install pz-rail-bpz
 
 But if you run into problems you might need to:
 
-- cd to a directory where you wish to clone the DESC_BPZ package and run `git clone https://github.com/LSSTDESC/DESC_BPZ.git`
-- cd to the DESC_BPZ directory and run `python setup.py install` (add `--user` if you are on a shared system such as NERSC)
-- try `pip install pz-rail-bpz` again.
+- cd to a directory where you wish to clone the DESC_BPZ package and run ``git clone https://github.com/LSSTDESC/DESC_BPZ.git``
+- cd to the DESC_BPZ directory and run ``python setup.py install`` (add ``--user`` if you are on a shared system such as NERSC)
+- try ``pip install pz-rail-bpz`` again.
 
 
 Using GPU-optimization for pzflow
 ---------------------------------
 
 Note that the Creation Module depends on pzflow, which has an optional GPU-compatible installation.
 For instructions, see the `pzflow Github repo <https://github.com/jfcrenshaw/pzflow/>`_.
 
-On some systems that are slightly out of date, e.g. an older version of python's `setuptools`, there can be some problems installing packages hosted on GitHub rather than PyPi.  We recommend that you update your system; however, some users have still reported problems with installation of subpackages necessary for `flexzboost` and `bpz_lite`.  If this occurs, try the following procedure:
-
-Once you have installed RAIL, you can import the package (via `import rail`) in any of your scripts and notebooks.
-For examples demonstrating how to use the different pieces, see the notebooks in the `examples/` directory.
+On some systems that are slightly out of date, e.g. an older version of python's
+``setuptools``, there can be some problems installing packages hosted on GitHub
+rather than PyPi.
+We recommend that you update your system; however, some users have still reported
+problems with installation of subpackages necessary for ``flexzboost`` and ``bpz_lite``.
+If this occurs, try the following procedure:
+
+Once you have installed RAIL, you can import the package (via ``import rail``) 
+in any of your scripts and notebooks.
+For examples demonstrating how to use the different pieces, see the notebooks in
+the ``examples/`` directory.
 
 
 Adding your kernel to jupyter
 =============================
-If you want to use the kernel that you have just created to run RAIL example demos, then you may need to explicitly add an ipython kernel.  You may need to first install ipykernel with `conda install ipykernel`.  You can do then add your kernel with the following command, making sure that you have the conda environment that you wish to add activated.  From your environment, execute the command:
-`python -m ipykernel install --user --name [nametocallnewkernel]`
-(you may or may not need to prepend `sudo` depending on your permissions).  When you next start up Jupyter you should see a kernel with your new name as an option, including using the Jupyter interface at NERSC.
+If you want to use the kernel that you have just created to run RAIL example demos,
+then you may need to explicitly add an ipython kernel.
+You may need to first install ipykernel with ``conda install ipykernel``.
+You can then add your kernel with the following command, making sure that you
+have the conda environment that you wish to add activated.
+From your environment, execute the command:
+``python -m ipykernel install --user --name [name_to_call_new_kernel]``
+(you may or may not need to prepend ``sudo`` depending on your permissions).
+When you next start up Jupyter you should see a kernel with your new name as an
+option, including using the Jupyter interface at NERSC.
 
 
 ..  LocalWords:  jupyter environment.yml rail_packages.yml pypi numpy
 ..  LocalWords:  conda-reqs.txt conda-forge pz-rail-som pz-rail-base
 ..  LocalWords:  scipy rail_bpz rail_flexzboost pz-rail alogrithm bpz
 ..  LocalWords:  setup.py pz-rail-delight Cython openmp openmp pzflow
 ..  LocalWords:  pz-rail-flexzboost xgboost xgboost bpz_lite ipython
```

### Comparing `pz-rail-0.99.2/docs/source/new_algorithm.rst` & `pz_rail-0.99.3/docs/source/new_algorithm.rst`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/docs/source/new_rail_stage.rst` & `pz_rail-0.99.3/docs/source/new_rail_stage.rst`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/docs/source/overview.rst` & `pz_rail-0.99.3/docs/source/overview.rst`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/docs/source/sharing_pipeline.rst` & `pz_rail-0.99.3/docs/source/sharing_pipeline.rst`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/examples/core_examples/Build_Save_Load_Run_Pipeline.ipynb` & `pz_rail-0.99.3/examples/core_examples/Build_Save_Load_Run_Pipeline.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9897363005768178%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(4, '**Last Run Successfully:** December 22, 2023')], "*

 * *            "delete: [4]}}, 2: {'source': {insert: [(11, 'from rail.core.util_stages import "*

 * *            "ColumnMapper, TableConverter')], delete: [11]}}, 4: {'source': {insert: [(1, "*

 * *            "'DS.__class__.allow_overwrite = True')], delete: [1]}}, 6: {'source': {insert: [(6, "*

 * *            "'post_grid = [float(x) for x in np.linspace(0.0, 5, 21)]')], delete: [6]}}, 8: "*

 * *            "{'source': {insert: [(18,  […]*

```diff
@@ -4,15 +4,15 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Build, Save, Load, and Run a Pipeline\n",
                 "\n",
                 "**Author:** Eric Charles\n",
                 "\n",
-                "**Last Run Successfully:** August 2, 2023"
+                "**Last Run Successfully:** December 22, 2023"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "This notebook shows how to:\n",
@@ -39,15 +39,15 @@
                 "from rail.core.stage import RailStage\n",
                 "from rail.creation.degradation.spectroscopic_degraders import LineConfusion\n",
                 "from rail.creation.degradation.quantityCut import QuantityCut\n",
                 "from rail.creation.degradation.lsst_error_model import LSSTErrorModel\n",
                 "from rail.creation.engines.flowEngine import FlowCreator, FlowPosterior\n",
                 "from rail.core.data import TableHandle\n",
                 "from rail.core.stage import RailStage\n",
-                "from rail.core.util_stages import ColumnMapper, TableConverter\n"
+                "from rail.core.util_stages import ColumnMapper, TableConverter"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We'll start by setting up the RAIL data store. RAIL uses [ceci](https://github.com/LSSTDESC/ceci), which is designed for pipelines rather than interactive notebooks; the data store will work around that and enable us to use data interactively.\n",
@@ -60,15 +60,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "DS = RailStage.data_store\n",
-                "DS.__class__.allow_overwrite = True\n"
+                "DS.__class__.allow_overwrite = True"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Build the pipeline\n",
@@ -96,15 +96,15 @@
             "source": [
                 "from rail.core.utils import find_rail_file\n",
                 "\n",
                 "flow_file = find_rail_file(\"examples_data/goldenspike_data/data/pretrained_flow.pkl\")\n",
                 "bands = [\"u\", \"g\", \"r\", \"i\", \"z\", \"y\"]\n",
                 "band_dict = {band: f\"mag_{band}_lsst\" for band in bands}\n",
                 "rename_dict = {f\"mag_{band}_lsst_err\": f\"mag_err_{band}_lsst\" for band in bands}\n",
-                "post_grid = [float(x) for x in np.linspace(0.0, 5, 21)]\n"
+                "post_grid = [float(x) for x in np.linspace(0.0, 5, 21)]"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Define the pipeline stages\n",
@@ -143,24 +143,24 @@
                 "\n",
                 "flow_post_test = FlowPosterior.make_stage(\n",
                 "    name=\"flow_post_test\", column=\"redshift\", flow=flow_file, grid=post_grid\n",
                 ")\n",
                 "\n",
                 "table_conv_test = TableConverter.make_stage(\n",
                 "    name=\"table_conv_test\", output_format=\"numpyDict\", seed=12345\n",
-                ")\n"
+                ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "flow_engine_test.sample(6, seed=0).data\n"
+                "flow_engine_test.sample(6, seed=0).data"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Make the pipeline and add the stages\n",
@@ -173,15 +173,15 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "pipe = ceci.Pipeline.interactive()\n",
                 "stages = [flow_engine_test, lsst_error_model_test, col_remapper_test, table_conv_test]\n",
                 "for stage in stages:\n",
-                "    pipe.add_stage(stage)\n"
+                "    pipe.add_stage(stage)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Interactive introspection\n",
@@ -194,47 +194,47 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Get the names of the stages\n",
-                "pipe.stage_names\n"
+                "pipe.stage_names"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Get the configuration of a particular stage\n",
-                "pipe.flow_engine_test.config\n"
+                "pipe.flow_engine_test.config"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Get the list of outputs 'tags'\n",
                 "# These are how the stage thinks of the outputs, as a list names associated to DataHandle types.\n",
-                "pipe.flow_engine_test.outputs\n"
+                "pipe.flow_engine_test.outputs"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Get the list of outputs 'aliased tags'\n",
                 "# These are how the pipeline things of the outputs, as a unique key that points to a particular file\n",
-                "pipe.flow_engine_test._outputs\n"
+                "pipe.flow_engine_test._outputs"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Connect up the pipeline stages\n",
@@ -248,15 +248,15 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "lsst_error_model_test.connect_input(flow_engine_test)\n",
                 "col_remapper_test.connect_input(lsst_error_model_test)\n",
                 "# flow_post_test.connect_input(col_remapper_test, inputTag='input')\n",
-                "table_conv_test.connect_input(col_remapper_test)\n"
+                "table_conv_test.connect_input(col_remapper_test)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Initialize the pipeline\n",
@@ -274,15 +274,15 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "pipe.initialize(\n",
                 "    dict(model=flow_file), dict(output_dir=\".\", log_dir=\".\", resume=False), None\n",
-                ")\n"
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Save the pipeline\n",
@@ -296,15 +296,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "pipe.save(\"pipe_saved.yml\")\n"
+                "pipe.save(\"pipe_saved.yml\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Read the saved pipeline"
@@ -312,15 +312,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "pr = ceci.Pipeline.read(\"pipe_saved.yml\")\n"
+                "pr = ceci.Pipeline.read(\"pipe_saved.yml\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Run the newly read pipeline\n",
@@ -330,24 +330,32 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "pr.run()\n"
+                "pr.run()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Running saved pipelines from the command line\n",
+                "Once you've saved a pipeline and have the `pipeline_name.yml` and `pipeline_name_config.yml` file pair, you can go ahead and run the pipeline from the command line instead, if you prefer. With [ceci](https://github.com/LSSTDESC/ceci) installed in your environment, just run `ceci path/to/the/pipeline.yml`. Running the pipeline we've just made would look like:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "pwd\n"
+                "! ceci pipe_saved.yml"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
@@ -359,15 +367,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.4"
+            "version": "3.11.6"
         },
         "vscode": {
             "interpreter": {
                 "hash": "1cc5b75da6b94fd59f6c7b0992047078a9372d2242c3f23a554e39af5a039534"
             }
         }
     },
```

### Comparing `pz-rail-0.99.2/examples/core_examples/FileIO_DataStore.ipynb` & `pz_rail-0.99.3/examples/core_examples/FileIO_DataStore.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/examples/core_examples/FluxtoMag_and_Deredden_example.ipynb` & `pz_rail-0.99.3/examples/core_examples/FluxtoMag_and_Deredden_example.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/examples/core_examples/Iterate_Tabular_Data.ipynb` & `pz_rail-0.99.3/examples/core_examples/Iterate_Tabular_Data.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/examples/core_examples/README.md` & `pz_rail-0.99.3/examples/core_examples/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/examples/core_examples/Run_Saved_Pipeline.ipynb` & `pz_rail-0.99.3/examples/core_examples/Run_Saved_Pipeline.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/examples/core_examples/Useful_Utilities.ipynb` & `pz_rail-0.99.3/examples/core_examples/Useful_Utilities.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999640804597701%*

 * *Differences: {"'cells'": "{22: {'source': {insert: [(0, 'import os\\n')]}}}"}*

```diff
@@ -223,14 +223,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "import os\n",
                 "from rail.core.utils import RAILDIR\n",
                 "\n",
                 "flow_file = os.path.join(\n",
                 "    RAILDIR, \"rail/examples_data/goldenspike_data/data/pretrained_flow.pkl\"\n",
                 ")"
             ]
         },
```

### Comparing `pz-rail-0.99.2/examples/core_examples/hyperbolic_magnitude_test.ipynb` & `pz_rail-0.99.3/examples/core_examples/hyperbolic_magnitude_test.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/examples/core_examples/pipe_example.yml` & `pz_rail-0.99.3/examples/core_examples/pipe_example.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/examples/core_examples/pipe_example_config.yml` & `pz_rail-0.99.3/examples/core_examples/pipe_example_config.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/examples/creation_examples/README.md` & `pz_rail-0.99.3/examples/creation_examples/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/examples/creation_examples/degradation-demo.ipynb` & `pz_rail-0.99.3/examples/creation_examples/degradation-demo.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/examples/creation_examples/dsps_sed_demo.ipynb` & `pz_rail-0.99.3/examples/creation_examples/dsps_sed_demo.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/examples/creation_examples/example_GridSelection_for_HSC.ipynb` & `pz_rail-0.99.3/examples/creation_examples/example_GridSelection_for_HSC.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/examples/creation_examples/example_ObsConditions.ipynb` & `pz_rail-0.99.3/examples/creation_examples/example_ObsConditions.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/examples/creation_examples/example_SpecSelection_for_zCOSMOS.ipynb` & `pz_rail-0.99.3/examples/creation_examples/example_SpecSelection_for_zCOSMOS.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/examples/creation_examples/photometric_realization_demo.ipynb` & `pz_rail-0.99.3/examples/creation_examples/photometric_realization_demo.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/examples/creation_examples/plotting_interface_skysim_cosmoDC2_COSMOS2020_demo.ipynb` & `pz_rail-0.99.3/examples/creation_examples/plotting_interface_skysim_cosmoDC2_COSMOS2020_demo.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/examples/creation_examples/posterior-demo.ipynb` & `pz_rail-0.99.3/examples/creation_examples/posterior-demo.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8730980904472283%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(4, 'last run successfully: March 7, 2024')], delete: [4]}}, "*

 * *            "18: {'source': {insert: [(2, 'n_samples = 50\\n')], delete: [2]}}, 29: {'source': "*

 * *            "{insert: [(0, 'Based on this histogram, I will marginalize over u band values from 25 "*

 * *            'to 31. Like how I tested different numbers of error samples above, here I will test '*

 * *            "different resolutions for the u band grid.\\n')], delete: [0]}}, 30: {'source': "*

 * *            '{inser […]*

```diff
@@ -4,15 +4,15 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Using a Creator to Calculate True Posteriors for a Galaxy Sample\n",
                 "\n",
                 "author: John Franklin Crenshaw, Sam Schmidt, Eric Charles, others...\n",
                 "\n",
-                "last run successfully: August 2, 2023"
+                "last run successfully: March 7, 2024"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "This notebook demonstrates how to use a RAIL Engine to calculate true posteriors for galaxy samples drawn from the same Engine. Note that this notebook assumes you have already read through `degradation-demo.ipynb`.\n",
@@ -224,15 +224,15 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# set up the error model\n",
                 "\n",
-                "n_samples = 30\n",
+                "n_samples = 50\n",
                 "# create the FlowEngine\n",
                 "flowEngine_degr = FlowCreator.make_stage(\n",
                 "    name=\"degraded\", flow_file=flow_file, n_samples=n_samples\n",
                 ")\n",
                 "# draw a few samples\n",
                 "samples_degr = flowEngine_degr.sample(n_samples, seed=0)\n",
                 "errorModel = LSSTErrorModel.make_stage(name=\"lsst_errors\", input=\"xx\", sigLim=5)\n",
@@ -440,15 +440,15 @@
                 "plt.show()\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Based on this histogram, I will marginalize over u band values from 27 to 31. Like how I tested different numbers of error samples above, here I will test different resolutions for the u band grid.\n",
+                "Based on this histogram, I will marginalize over u band values from 25 to 31. Like how I tested different numbers of error samples above, here I will test different resolutions for the u band grid.\n",
                 "\n",
                 "I will provide our new u band grid in the `marg_rules` dictionary, which will also include `\"flag\"` which tells `FlowEngine` what my flag for non-detections is.\n",
                 "In this simple example, we are using a fixed grid for the u band, but notice that the u band rule takes the form of a function - this is because the grid over which to marginalize can be a function of any of the other variables in the row. \n",
                 "If I wanted to marginalize over any other bands, I would need to include corresponding rules in `marg_rules` too.\n",
                 "\n",
                 "For this example, I will only calculate pdfs for galaxy 3, which is the galaxy with a non-detection in the u band. Also, similarly to how I tested the error convolution with a variable number of samples, I will test the marginalization with varying resolutions for the marginalized grid."
             ]
@@ -472,15 +472,15 @@
                 ")\n",
                 "\n",
                 "# iterate over variable grid resolution\n",
                 "for nbins in [10, 20, 50, 100]:\n",
                 "    # set up the marginalization rules for this grid resolution\n",
                 "    marg_rules = {\n",
                 "        \"flag\": errorModel.config[\"ndFlag\"],\n",
-                "        \"u\": lambda row: np.linspace(27, 31, nbins),\n",
+                "        \"u\": lambda row: np.linspace(25, 31, nbins),\n",
                 "    }\n",
                 "\n",
                 "    # calculate the posterior by marginalizing over u and sampling\n",
                 "    # from the error distributions of the other galaxies\n",
                 "    pdfs_u_marginalized[nbins] = get_degr_post(\n",
                 "        f\"degr_post_nbins_{nbins}\",\n",
                 "        row3_degraded,\n",
@@ -526,18 +526,18 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.4"
+            "version": "3.10.13"
         },
         "vscode": {
             "interpreter": {
                 "hash": "1cc5b75da6b94fd59f6c7b0992047078a9372d2242c3f23a554e39af5a039534"
             }
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 2
+    "nbformat_minor": 4
 }
```

### Comparing `pz-rail-0.99.2/examples/estimation_examples/CMNN_Demo.ipynb` & `pz_rail-0.99.3/examples/estimation_examples/CMNN_Demo.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9937213827838828%*

 * *Differences: {"'cells'": "{1: {'source': {delete: [5, 4, 3, 2, 1, 0]}}, 11: {'source': {insert: [(0, 'from "*

 * *            'rail.core.utils import RAILDIR\\n\'), (1, "trainFile = os.path.join(RAILDIR, '*

 * *            '\'rail/examples_data/testdata/test_dc2_training_9816.hdf5\')\\n"), (2, "testFile = '*

 * *            'os.path.join(RAILDIR, '*

 * *            '\'rail/examples_data/testdata/test_dc2_validation_9816.hdf5\')\\n")], delete: [2, 1, '*

 * *            "0]}}, insert: [(0, OrderedDict([('cell_type', 'markdown'), ('metadata', "*

 * *   […]*

```diff
@@ -1,19 +1,24 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# CMNN Demo\n",
+                "# RAIL CMNN Tutorial Notebook\n",
                 "\n",
                 "**Author:** Sam Schmidt\n",
                 "\n",
-                "**Last Successfully Run:** September 26, 2023\n",
-                "\n",
+                "**Last Successfully Run:** September 26, 2023"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "This is a notebook demonstrating some of the features of the LSSTDESC `RAIL` version of the CMNN estimator, see **[Graham et al. (2018)](https://ui.adsabs.harvard.edu/abs/2018AJ....155....1G/abstract)** for more details on the algorithm.<br>\n",
                 "\n",
                 "CMNN stands for color-matched nearest-neighbor, and as this name implies, the method works by finding the Mahalanobis distance between each test galaxy and the training galaxies, and selecting one of those \"nearby\" in color space as the redshift estimate.  The algorithm also estimates the \"width\" of the resulting PDF based on the standard deviation of this nearby set and returns a single Gaussian with a mean and width defined as such.<br>\n",
                 "\n",
                 "The current version of the code consists of a training stage, `CMNNInformer`, that computes colors for a set of training data and an estimation stage `CMNNEstimator` that calculates the Mahalanobis distance to each training galaxy for each test galaxy and returns a single Guassian PDF for each galaxy.   The mean value of this Gaussian PDF can be estimated in one of three ways (see selection mode below), and the width is determined by the standard deviation of training galaxy redshifts within the threshold Mahalanobis distance. Future implementation improvements may change the output format to include multiple Gaussians.\n",
                 "\n",
                 "For the color calculation, there is an option for how to treat the \"non-detections\" in a band: the default choice is to ignore any colors that contain a non-detect magnitude and adjust the number of degrees of freedom in the Mahalanobis distance accordingly (this is how the CMNN algorithm was originally implemented).  Or, if the configuration parameter `nondetect_replace` is set to `True` in `CMNNInformer`, the non-detected magnitudes will be replaced with the 1-sigma limiting magnitude in each band as supplied by the user via the `mag_limits` configuration parameter (or by the default 1-sigma limits if the user does not supply specific numbers).  We have not done any exploration of the relative performance of these two choices, but note that there is not a significant performance difference in terms of runtime between the two methods.<br>\n",
@@ -131,17 +136,17 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from rail.core.utils import find_rail_file\n",
-                "trainFile = find_rail_file('examples_data/testdata/test_dc2_training_9816.hdf5')\n",
-                "testFile = find_rail_file('examples_data/testdata/test_dc2_validation_9816.hdf5')\n",
+                "from rail.core.utils import RAILDIR\n",
+                "trainFile = os.path.join(RAILDIR, 'rail/examples_data/testdata/test_dc2_training_9816.hdf5')\n",
+                "testFile = os.path.join(RAILDIR, 'rail/examples_data/testdata/test_dc2_validation_9816.hdf5')\n",
                 "training_data = DS.read_file(\"training_data\", TableHandle, trainFile)\n",
                 "test_data = DS.read_file(\"test_data\", TableHandle, testFile)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -375,13 +380,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.4"
+            "version": "3.11.6"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `pz-rail-0.99.2/examples/estimation_examples/Fzboost_PDF_Representation_Comparison.ipynb` & `pz_rail-0.99.3/examples/estimation_examples/Fzboost_PDF_Representation_Comparison.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9952224310776943%*

 * *Differences: {"'cells'": '{delete: [37]}', "'metadata'": "{'language_info': {'version': '3.11.6'}}"}*

```diff
@@ -404,21 +404,14 @@
                 "    pass\n",
                 "\n",
                 "try:\n",
                 "    os.unlink(interp_file_name)\n",
                 "except FileNotFoundError:\n",
                 "    pass"
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
@@ -429,15 +422,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.4"
+            "version": "3.11.6"
         },
         "vscode": {
             "interpreter": {
                 "hash": "47c0d775efeae3192041035019ca2d946443ef986557562adbc143cc5fa38455"
             }
         }
     },
```

### Comparing `pz-rail-0.99.2/examples/estimation_examples/GPz_estimation_example.ipynb` & `pz_rail-0.99.3/examples/estimation_examples/GPz_estimation_example.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/examples/estimation_examples/NZDir.ipynb` & `pz_rail-0.99.3/examples/estimation_examples/NZDir.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997710622710623%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, '**Author:** Sam Schmidt\\n'), (4, '**Last successfully "*

 * *            "run:** April 26, 2023')], delete: [4, 2]}}}"}*

```diff
@@ -3,17 +3,17 @@
         {
             "cell_type": "markdown",
             "id": "2859224e-4ef2-44c8-940c-b911c5568f89",
             "metadata": {},
             "source": [
                 "# The NZDir estimator\n",
                 "\n",
-                "Author: Sam Schmidt\n",
+                "**Author:** Sam Schmidt\n",
                 "\n",
-                "Last successfully run: April 26, 2023"
+                "**Last successfully run:** April 26, 2023"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "aed15c9e",
             "metadata": {},
             "source": [
```

### Comparing `pz-rail-0.99.2/examples/estimation_examples/RAIL_estimation_demo.ipynb` & `pz_rail-0.99.3/examples/estimation_examples/RAIL_estimation_demo.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9922470238095238%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# RAIL Estimation Tutorial Notebook\\n'), (2, "*

 * *            "'**Authors:** Sam Schmidt, Eric Charles, Alex Malz, others...\\n'), (4, '**Last run "*

 * *            "successfully:** August 15, 2023')], delete: [4, 2, 0]}}, 6: {'source': {insert: [(0, "*

 * *            "'## Importing all available estimators\\n')], delete: [0]}}, delete: [49, 48]}",*

 * * "'metadata'": "{'language_info': {'version': '3.11.6'}}"}*

```diff
@@ -1,18 +1,18 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# RAIL/Estimation Tutorial Notebook\n",
+                "# RAIL Estimation Tutorial Notebook\n",
                 "\n",
-                "author: Sam Schmidt, Eric Charles, Alex Malz, others...\n",
+                "**Authors:** Sam Schmidt, Eric Charles, Alex Malz, others...\n",
                 "\n",
-                "last run successfully: August 15, 2023"
+                "**Last run successfully:** August 15, 2023"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "This is a notebook demonstrating some of the `estimation` features of the LSST-DESC `RAIL`-iverse packages.  \n",
@@ -63,15 +63,15 @@
                 "DS.__class__.allow_overwrite = True"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Importing all available estimators\n",
+                "## Importing all available estimators\n",
                 "\n",
                 "There is some handy functionality in `rail.stages` to import all available stages that are installed in your environment.  `RailStage` knows about all of the sub-types of stages.  By looping through the values in  the `RailStage.pipeline_stages` dictionary, we can isolate those that are sub-classes of `rail.estimation.estimator.CatEstimator`, which operate on catalog-like inputs.  Let's run this `import_and_attach_all()` command, and then print out the subclasses that are now available for use (though in this demo we only take advantage of two specific estimators):"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -514,28 +514,14 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The results look very good! FlexZBoost is a mature algorithm, and with representative training data we see a very tight correlation with true redshift and few outliers due to physical degeneracies.<br>"
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": []
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
@@ -546,13 +532,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.4"
+            "version": "3.11.6"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `pz-rail-0.99.2/examples/estimation_examples/README.md` & `pz_rail-0.99.3/examples/estimation_examples/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/examples/estimation_examples/SimpleSOM_demo.ipynb.fixme` & `pz_rail-0.99.3/examples/estimation_examples/SimpleSOM_demo.ipynb.fixme`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/examples/estimation_examples/nzdir_as_pipeline.ipynb` & `pz_rail-0.99.3/examples/estimation_examples/nzdir_as_pipeline.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9852430555555556%*

 * *Differences: {"'cells'": "{0: {'source': ['# NZDir as a Pipeline\\n', '\\n', '**Author:** Sam Schmidt\\n', "*

 * *            "'\\n', '**Last successfully run:** April 26, 2023']}, delete: [17, 1]}"}*

```diff
@@ -1,24 +1,19 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "id": "c1005cfd",
             "metadata": {},
             "source": [
-                "# NZDir as a Pipeline"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "113cdd0f",
-            "metadata": {},
-            "source": [
-                "Author: Sam Schmidt<br>\n",
-                "Last successfully run: April 26, 2023<br>"
+                "# NZDir as a Pipeline\n",
+                "\n",
+                "**Author:** Sam Schmidt\n",
+                "\n",
+                "**Last successfully run:** April 26, 2023"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "e324bb13",
             "metadata": {},
@@ -186,22 +181,14 @@
                 "fig, axs = plt.subplots(figsize=(10,8))\n",
                 "nzdir_nz[0].plot_native(axes=axs, fc = [0, 0, 1, 0.01])\n",
                 "nzd_ens[1].plot_native(axes=axs, fc = [0, 1, 0, 0.01])\n",
                 "nzd_ens[4].plot_native(axes=axs, fc = [1, 0, 0, 0.01])\n",
                 "axs.set_xlim(0,3)\n",
                 "axs.legend()"
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "3c9d353a-a054-4a5b-9ae7-8ac40d9f61bc",
-            "metadata": {},
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
```

### Comparing `pz-rail-0.99.2/examples/estimation_examples/somocluSOM_demo.ipynb` & `pz_rail-0.99.3/examples/estimation_examples/somocluSOM_demo.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997209821428572%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, '**Author:** Ziang Yan, Sam Schmidt\\n'), (4, '**Last "*

 * *            "successfully run:** June 16, 2023')], delete: [4, 2]}}, 51: {'source': {insert: [(0, "*

 * *            "'## Quantitative metrics\\n')], delete: [0]}}}"}*

```diff
@@ -3,17 +3,17 @@
         {
             "cell_type": "markdown",
             "id": "56bf073d",
             "metadata": {},
             "source": [
                 "# Somoclu SOM Summarizer Demo\n",
                 "\n",
-                "Author: Ziang Yan, Sam Schmidt\n",
+                "**Author:** Ziang Yan, Sam Schmidt\n",
                 "\n",
-                "Last successfully run: June 16, 2023"
+                "**Last successfully run:** June 16, 2023"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "f40c36ff",
             "metadata": {},
             "source": [
@@ -620,15 +620,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "3b32f0d8",
             "metadata": {},
             "source": [
-                "## quantitative metrics\n",
+                "## Quantitative metrics\n",
                 "\n",
                 "Let's look at how we've done at estimating the mean redshift and \"width\" (via standard deviation) of our tomographic bin compared to the true redshift and \"width\" for both our \"full\" sample and \"bright\" i<23.5 samples.  We will plot the mean and std dev for the full and bright distributions compared to the true mean and width, and show the Gaussian uncertainty approximation given the scatter in the bootstraps for the mean:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
```

### Comparing `pz-rail-0.99.2/examples/estimation_examples/somocluSOMcluster_demo.ipynb` & `pz_rail-0.99.3/examples/estimation_examples/somocluSOMcluster_demo.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997384207589286%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, '**Author:** Ziang Yan, Sam Schmidt\\n'), (4, '**Last "*

 * *            "successfully run:** June 16, 2023')], delete: [4, 2]}}, 55: {'source': {insert: [(0, "*

 * *            "'## Quantitative metrics\\n')], delete: [0]}}}"}*

```diff
@@ -3,17 +3,17 @@
         {
             "cell_type": "markdown",
             "id": "211657f5",
             "metadata": {},
             "source": [
                 "# Somoclu SOM Summarizer Cluster Demo\n",
                 "\n",
-                "Author: Ziang Yan, Sam Schmidt\n",
+                "**Author:** Ziang Yan, Sam Schmidt\n",
                 "\n",
-                "Last successfully run: June 16, 2023"
+                "**Last successfully run:** June 16, 2023"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "17cd4514",
             "metadata": {},
             "source": [
@@ -740,15 +740,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "526c2f84",
             "metadata": {},
             "source": [
-                "## quantitative metrics\n",
+                "## Quantitative metrics\n",
                 "\n",
                 "Let's look at how we've done at estimating the mean redshift and \"width\" (via standard deviation) of our tomographic bin compared to the true redshift and \"width\" for both our \"full\" sample and \"bright\" i<23.5 samples.  We will plot the mean and std dev for the full and bright distributions compared to the true mean and width, and show the Gaussian uncertainty approximation given the scatter in the bootstraps for the mean:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
```

### Comparing `pz-rail-0.99.2/examples/estimation_examples/test_sampled_summarizers.ipynb` & `pz_rail-0.99.3/examples/estimation_examples/test_sampled_summarizers.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9978398617511521%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, '**Author:** Sam Schmidt\\n'), (4, '**Last successfully "*

 * *            "run:** April 26, 2023')], delete: [4, 2]}}, delete: [61]}"}*

```diff
@@ -3,17 +3,17 @@
         {
             "cell_type": "markdown",
             "id": "c697f8c4",
             "metadata": {},
             "source": [
                 "# Test Sampled Summarizers\n",
                 "\n",
-                "Author: Sam Schmidt\n",
+                "**Author:** Sam Schmidt\n",
                 "\n",
-                "Last successfully run: April 26, 2023"
+                "**Last successfully run:** April 26, 2023"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "042969c1-911f-4c35-a1dd-f90befe099dc",
             "metadata": {},
             "source": [
@@ -651,22 +651,14 @@
         {
             "cell_type": "markdown",
             "id": "7c0b6442-68ce-4a7f-b7be-8727a364deec",
             "metadata": {},
             "source": [
                 "Again, not a huge spread in predicted mean redshifts based solely on bootstraps, even with only ~20,000 galaxies."
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "b206103c-31bd-4e7a-bacf-d35268d52dcb",
-            "metadata": {},
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
```

### Comparing `pz-rail-0.99.2/examples/evaluation_examples/demo.ipynb` & `pz_rail-0.99.3/examples/evaluation_examples/Evaluation_Demo.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.997245670995671%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, '**Authors:** Sam Schmidt, Alex Malz, Julia Gschwend, "*

 * *            "others...\\n'), (4, '**Last run successfully:** June 16, 2023 (with qp-prob >= "*

 * *            "0.8.2)')], delete: [4, 2]}}, 2: {'source': {insert: [(2, 'from "*

 * *            "rail.evaluation.evaluator import OldEvaluator\\n')], delete: [2]}}, 16: {'source': "*

 * *            '["FZB_eval = OldEvaluator.make_stage(name=\'FZB_eval\', truth=truth)"]}, delete: '*

 * *            '[54]}'}*

```diff
@@ -2,17 +2,17 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Demo: RAIL Evaluation \n",
                 "\n",
-                "Author: Sam Schmidt, Alex Malz, Julia Gschwend, others...\n",
+                "**Authors:** Sam Schmidt, Alex Malz, Julia Gschwend, others...\n",
                 "\n",
-                "last run successfully: June 16, 2023 (with qp-prob >= 0.8.2)"
+                "**Last run successfully:** June 16, 2023 (with qp-prob >= 0.8.2)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The purpose of this notebook is to demonstrate the application of the metrics scripts to be used on the photo-z PDF catalogs produced by the PZ working group. The first implementation of the _evaluation_ module is based on the refactoring of the code used in [Schmidt et al. 2020](https://arxiv.org/pdf/2001.03621.pdf), available on Github repository [PZDC1paper](https://github.com/LSSTDESC/PZDC1paper). \n",
@@ -24,15 +24,15 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import rail\n",
                 "from rail.evaluation.metrics.cdeloss import *\n",
-                "from rail.evaluation.evaluator import Evaluator\n",
+                "from rail.evaluation.evaluator import OldEvaluator\n",
                 "from rail.core.data import QPHandle, TableHandle\n",
                 "from rail.core.stage import RailStage\n",
                 "from utils import plot_pit_qq, ks_plot\n",
                 "import qp \n",
                 "import os\n",
                 "%matplotlib inline\n",
                 "%reload_ext autoreload\n",
@@ -170,15 +170,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "FZB_eval = Evaluator.make_stage(name='FZB_eval', truth=truth)"
+                "FZB_eval = OldEvaluator.make_stage(name='FZB_eval', truth=truth)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -542,21 +542,14 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We note that all of the quantities as run individually are identical to the quantities in our summary table - a nice check that things have run properly."
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
```

### Comparing `pz-rail-0.99.2/examples/evaluation_examples/utils.py` & `pz_rail-0.99.3/examples/evaluation_examples/utils.py`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/examples/goldenspike_examples/README.md` & `pz_rail-0.99.3/examples/goldenspike_examples/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/examples/goldenspike_examples/cleanup.sh` & `pz_rail-0.99.3/examples/goldenspike_examples/cleanup.sh`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/examples/goldenspike_examples/goldenspike.ipynb` & `pz_rail-0.99.3/examples/goldenspike_examples/goldenspike.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.995123528814935%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# Goldenspike: an example of an end-to-end analysis "*

 * *            "using RAIL\\n'), (2, '**Authors:** Sam Schmidt, Eric Charles, Alex Malz, John "*

 * *            "Franklin Crenshaw, others...\\n'), (4, '**Last run successfully:** Oct 23, 2023')], "*

 * *            "delete: [4, 2, 0]}}, 4: {'source': {insert: [(20, 'from rail.evaluation.evaluator "*

 * *            "import OldEvaluator\\n')], delete: [20]}}, 34: {'source': {insert: [(5, '    the_eval "*

 * *            '= OldEvaluat […]*

```diff
@@ -1,19 +1,19 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "id": "c8fb0b8d",
             "metadata": {},
             "source": [
-                "# Goldenspike, an example of an end-to-end analysis using RAIL\n",
+                "# Goldenspike: an example of an end-to-end analysis using RAIL\n",
                 "\n",
-                "author: Sam Schmidt, Eric Charles, Alex Malz, John Franklin Crenshaw, others...\n",
+                "**Authors:** Sam Schmidt, Eric Charles, Alex Malz, John Franklin Crenshaw, others...\n",
                 "\n",
-                "last run successfully: Oct 23, 2023"
+                "**Last run successfully:** Oct 23, 2023"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "minute-lender",
             "metadata": {},
             "source": [
@@ -87,15 +87,15 @@
                 "from rail.estimation.algos.bpz_lite import BPZliteInformer, BPZliteEstimator\n",
                 "from rail.estimation.algos.k_nearneigh import KNearNeighInformer, KNearNeighEstimator\n",
                 "from rail.estimation.algos.flexzboost import FlexZBoostInformer, FlexZBoostEstimator\n",
                 "\n",
                 "from rail.estimation.algos.naive_stack import NaiveStackSummarizer\n",
                 "from rail.estimation.algos.point_est_hist import PointEstHistSummarizer\n",
                 "\n",
-                "from rail.evaluation.evaluator import Evaluator\n"
+                "from rail.evaluation.evaluator import OldEvaluator\n"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "scheduled-chamber",
             "metadata": {},
             "source": [
@@ -484,22 +484,14 @@
             "source": [
                 "inform_bpz.inform(train_data)\n",
                 "inform_knn.inform(train_data)\n",
                 "inform_fzboost.inform(train_data)\n"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "7869451a-f1c5-4c6a-85d3-70022f8cc1e6",
-            "metadata": {},
-            "outputs": [],
-            "source": []
-        },
-        {
             "cell_type": "markdown",
             "id": "colonial-trailer",
             "metadata": {},
             "source": [
                 "## Estimate photo-z posteriors\n",
                 "\n",
                 "More detail on the specific estimators used here is available in the `rail/examples/estimation_examples/RAIL_estimation_demo.ipynb` notebook, but here is a very brief summary of the three estimators used in this notebook:\n",
@@ -572,15 +564,15 @@
             "outputs": [],
             "source": [
                 "eval_dict = dict(bpz=bpz_estimated, fzboost=fzboost_estimated, knn=knn_estimated)\n",
                 "truth = test_data_orig\n",
                 "\n",
                 "result_dict = {}\n",
                 "for key, val in eval_dict.items():\n",
-                "    the_eval = Evaluator.make_stage(name=f\"{key}_eval\", truth=truth)\n",
+                "    the_eval = OldEvaluator.make_stage(name=f\"{key}_eval\", truth=truth)\n",
                 "    result_dict[key] = the_eval.evaluate(val, truth)\n"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "danish-miller",
             "metadata": {},
@@ -789,36 +781,28 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "informational-performer",
             "metadata": {},
             "source": [
-                "# Clean up:\n",
+                "## Clean up:\n",
                 "\n",
                 "Finally, you'll notice that we've written a large number of temporary files in the course of running this demo, to delete these and clean up the directory just run the `cleanup.sh` script in this directory to delete the data files."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "racial-stocks",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# TODO fix and add clean up scripts\n"
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "4f1b54da-4e39-4f74-86e4-466e310f5a60",
-            "metadata": {},
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
```

### Comparing `pz-rail-0.99.2/examples/goldenspike_examples/goldenspike.yml` & `pz_rail-0.99.3/examples/goldenspike_examples/goldenspike.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/examples/goldenspike_examples/goldenspike_config.yml` & `pz_rail-0.99.3/examples/goldenspike_examples/goldenspike_config.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.2/pyproject.toml` & `pz_rail-0.99.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -19,25 +19,35 @@
 dependencies = [
     "pz-rail-base",
 ]
 
 # On a mac, install optional dependencies with `pip install '.[dev]'` (include the single quotes)
 [project.optional-dependencies]
 algos = [
-    "pz-rail-pipelines[full]",
+    "pz-rail-astro-tools",
+    "pz-rail-bpz",
+    "pz-rail-cmnn",
+    "pz-rail-dsps",
+    "pz-rail-flexzboost",
+    "pz-rail-fsps",
+    "pz-rail-gpz-v1",
+    "pz-rail-pzflow",
+    "pz-rail-sklearn",
+    "pz-rail-som",
+    "qp-prob[full]",
 ]
 
 nb = [
-    "pz-rail-pipelines[full]",
+    "pz-rail[algos]",
     "jupyter",
     "seaborn",
 ]
 
 dev = [
-    "pz-rail-pipelines[full]",
+    "pz-rail[algos]",
     "jupyter",
     "seaborn",
     "corner",
     "pandas",
     "h5py",
     "matplotlib",
     "coverage",
```

### Comparing `pz-rail-0.99.2/src/pz_rail.egg-info/PKG-INFO` & `pz_rail-0.99.3/src/pz_rail.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail
-Version: 0.99.2
+Version: 0.99.3
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -31,21 +31,31 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pz-rail-base
 Provides-Extra: algos
-Requires-Dist: pz-rail-pipelines[full]; extra == "algos"
+Requires-Dist: pz-rail-astro-tools; extra == "algos"
+Requires-Dist: pz-rail-bpz; extra == "algos"
+Requires-Dist: pz-rail-cmnn; extra == "algos"
+Requires-Dist: pz-rail-dsps; extra == "algos"
+Requires-Dist: pz-rail-flexzboost; extra == "algos"
+Requires-Dist: pz-rail-fsps; extra == "algos"
+Requires-Dist: pz-rail-gpz-v1; extra == "algos"
+Requires-Dist: pz-rail-pzflow; extra == "algos"
+Requires-Dist: pz-rail-sklearn; extra == "algos"
+Requires-Dist: pz-rail-som; extra == "algos"
+Requires-Dist: qp-prob[full]; extra == "algos"
 Provides-Extra: nb
-Requires-Dist: pz-rail-pipelines[full]; extra == "nb"
+Requires-Dist: pz-rail[algos]; extra == "nb"
 Requires-Dist: jupyter; extra == "nb"
 Requires-Dist: seaborn; extra == "nb"
 Provides-Extra: dev
-Requires-Dist: pz-rail-pipelines[full]; extra == "dev"
+Requires-Dist: pz-rail[algos]; extra == "dev"
 Requires-Dist: jupyter; extra == "dev"
 Requires-Dist: seaborn; extra == "dev"
 Requires-Dist: corner; extra == "dev"
 Requires-Dist: pandas; extra == "dev"
 Requires-Dist: h5py; extra == "dev"
 Requires-Dist: matplotlib; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
```

### Comparing `pz-rail-0.99.2/src/pz_rail.egg-info/SOURCES.txt` & `pz_rail-0.99.3/src/pz_rail.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 .github/ISSUE_TEMPLATE/0-general_issue.md
 .github/ISSUE_TEMPLATE/1-bug_report.md
 .github/ISSUE_TEMPLATE/2-feature_request.md
 .github/workflows/add-issue-to-project-tracker.yml
 .github/workflows/build_documentation.yml
 .github/workflows/linting.yml
 .github/workflows/publish-to-pypi.yml
+.github/workflows/smoke-test-head.yml
 .github/workflows/smoke-test.yml
 .github/workflows/testing-and-coverage.yml
 docs/Makefile
 docs/conf.py
 docs/demos.rst
 docs/index.rst
 docs/nbconvert-requirements.txt
@@ -52,33 +53,37 @@
 examples/creation_examples/README.md
 examples/creation_examples/cleanup.sh
 examples/creation_examples/degradation-demo.ipynb
 examples/creation_examples/dsps_sed_demo.ipynb
 examples/creation_examples/example_GridSelection_for_HSC.ipynb
 examples/creation_examples/example_ObsConditions.ipynb
 examples/creation_examples/example_SpecSelection_for_zCOSMOS.ipynb
+examples/creation_examples/fsps_sed_demo.ipynb
 examples/creation_examples/photometric_realization_demo.ipynb
 examples/creation_examples/plotting_interface_skysim_cosmoDC2_COSMOS2020_demo.ipynb
 examples/creation_examples/posterior-demo.ipynb
+examples/estimation_examples/BPZ_lite_demo.ipynb
+examples/estimation_examples/BPZ_lite_with_custom_SEDs.ipynb
 examples/estimation_examples/CMNN_Demo.ipynb
 examples/estimation_examples/Fzboost_PDF_Representation_Comparison.ipynb
 examples/estimation_examples/GPz_estimation_example.ipynb
 examples/estimation_examples/NZDir.ipynb
 examples/estimation_examples/RAIL_estimation_demo.ipynb
 examples/estimation_examples/README.md
 examples/estimation_examples/SimpleSOM_demo.ipynb.fixme
 examples/estimation_examples/cleanup.sh
 examples/estimation_examples/nzdir_as_pipeline.ipynb
 examples/estimation_examples/somocluSOM_demo.ipynb
 examples/estimation_examples/somocluSOMcluster_demo.ipynb
 examples/estimation_examples/test_sampled_summarizers.ipynb
 examples/evaluation_examples/.gitignore
+examples/evaluation_examples/Evaluation_Demo.ipynb
+examples/evaluation_examples/Evaluation_by_type.ipynb
 examples/evaluation_examples/README.md
 examples/evaluation_examples/cleanup.sh
-examples/evaluation_examples/demo.ipynb
 examples/evaluation_examples/utils.py
 examples/goldenspike_examples/README.md
 examples/goldenspike_examples/cleanup.sh
 examples/goldenspike_examples/cleanup_pipeline.sh
 examples/goldenspike_examples/goldenspike.ipynb
 examples/goldenspike_examples/goldenspike.yml
 examples/goldenspike_examples/goldenspike_config.yml
```

