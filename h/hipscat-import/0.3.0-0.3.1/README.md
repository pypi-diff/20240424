# Comparing `tmp/hipscat_import-0.3.0.tar.gz` & `tmp/hipscat_import-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hipscat_import-0.3.0.tar", last modified: Mon Apr 22 15:57:05 2024, max compression
+gzip compressed data, was "hipscat_import-0.3.1.tar", last modified: Wed Apr 24 16:22:19 2024, max compression
```

## Comparing `hipscat_import-0.3.0.tar` & `hipscat_import-0.3.1.tar`

### file list

```diff
@@ -1,283 +1,283 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:05.017361 hipscat_import-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.969360 hipscat_import-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.969360 hipscat_import-0.3.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.969360 hipscat_import-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/.github/workflows/build-documentation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/.github/workflows/pre-commit-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/.setup_dev.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5550 2024-04-22 15:57:05.017361 hipscat_import-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.973360 hipscat_import-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.973360 hipscat_import-0.3.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/docs/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.973360 hipscat_import-0.3.0/docs/catalogs/
--rw-r--r--   0 runner    (1001) docker     (127)    13620 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/docs/catalogs/arguments.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.973360 hipscat_import-0.3.0/docs/catalogs/public/
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/docs/catalogs/public/allwise.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/docs/catalogs/public/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/docs/catalogs/public/neowise.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/docs/catalogs/public/panstarrs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/docs/catalogs/public/sdss.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/docs/catalogs/public/tic.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/docs/catalogs/public/zubercal.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10736 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/docs/catalogs/temp_files.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.973360 hipscat_import-0.3.0/docs/guide/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/docs/guide/contact.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/docs/guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/docs/guide/dask_on_ray.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12082 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/docs/guide/index_table.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/docs/guide/margin_cache.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.973360 hipscat_import-0.3.0/docs/notebooks/
--rwxr-xr-x   0 runner    (1001) docker     (127)     7615 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/docs/notebooks/estimate_pixel_threshold.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/docs/notebooks/unequal_schema.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/docs/notebooks.rst
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.977360 hipscat_import-0.3.0/docs/static/
--rw-r--r--   0 runner    (1001) docker     (127)   136863 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/docs/static/allwise_schema.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/docs/static/allwise_types.csv
--rw-r--r--   0 runner    (1001) docker     (127)    66486 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/docs/static/neowise_schema.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/docs/static/neowise_types.csv
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/docs/static/ps1_detections_types.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/docs/static/ps1_otmo_types.csv
--rw-r--r--   0 runner    (1001) docker     (127)   412559 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/docs/static/sdss_wget.bash
--rw-r--r--   0 runner    (1001) docker     (127)    57050 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/docs/static/tic_schema.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/docs/static/tic_types.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 15:57:05.017361 hipscat_import-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.977360 hipscat_import-0.3.0/src/
--rw-r--r--   0 runner    (1001) docker     (127)    20810 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/src/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.977360 hipscat_import-0.3.0/src/hipscat_import/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/src/hipscat_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-22 15:57:04.000000 hipscat_import-0.3.0/src/hipscat_import/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.981361 hipscat_import-0.3.0/src/hipscat_import/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/src/hipscat_import/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8560 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/src/hipscat_import/catalog/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     9758 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/src/hipscat_import/catalog/file_readers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12329 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/src/hipscat_import/catalog/map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)    12059 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/src/hipscat_import/catalog/resume_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     7105 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/src/hipscat_import/catalog/run_import.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.981361 hipscat_import-0.3.0/src/hipscat_import/index/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/src/hipscat_import/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/src/hipscat_import/index/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/src/hipscat_import/index/map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/src/hipscat_import/index/run_index.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.981361 hipscat_import-0.3.0/src/hipscat_import/margin_cache/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/src/hipscat_import/margin_cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/src/hipscat_import/margin_cache/margin_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/src/hipscat_import/margin_cache/margin_cache_arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/src/hipscat_import/margin_cache/margin_cache_map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/src/hipscat_import/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     8004 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/src/hipscat_import/pipeline_resume_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/src/hipscat_import/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     6626 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/src/hipscat_import/runtime_arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.981361 hipscat_import-0.3.0/src/hipscat_import/soap/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/src/hipscat_import/soap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/src/hipscat_import/soap/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)    10153 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/src/hipscat_import/soap/map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     9464 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/src/hipscat_import/soap/resume_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/src/hipscat_import/soap/run_soap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.981361 hipscat_import-0.3.0/src/hipscat_import/verification/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/src/hipscat_import/verification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/src/hipscat_import/verification/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/src/hipscat_import/verification/run_verification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:05.013361 hipscat_import-0.3.0/src/hipscat_import.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5550 2024-04-22 15:57:04.000000 hipscat_import-0.3.0/src/hipscat_import.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11718 2024-04-22 15:57:04.000000 hipscat_import-0.3.0/src/hipscat_import.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 15:57:04.000000 hipscat_import-0.3.0/src/hipscat_import.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-22 15:57:04.000000 hipscat_import-0.3.0/src/hipscat_import.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-22 15:57:04.000000 hipscat_import-0.3.0/src/hipscat_import.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.981361 hipscat_import-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    20888 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.981361 hipscat_import-0.3.0/tests/hipscat_import/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.985360 hipscat_import-0.3.0/tests/hipscat_import/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/catalog/test_argument_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9441 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/catalog/test_file_readers.py
--rw-r--r--   0 runner    (1001) docker     (127)    17181 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/catalog/test_map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     8694 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/catalog/test_resume_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)    13396 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/catalog/test_run_import.py
--rw-r--r--   0 runner    (1001) docker     (127)    16174 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/catalog/test_run_round_trip.py
--rw-r--r--   0 runner    (1001) docker     (127)     9440 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.965360 hipscat_import-0.3.0/tests/hipscat_import/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.985360 hipscat_import-0.3.0/tests/hipscat_import/data/blank/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/blank/blank.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.985360 hipscat_import-0.3.0/tests/hipscat_import/data/mixed_schema/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/mixed_schema/input_01.csv
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/mixed_schema/input_02.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/mixed_schema/schema.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.965360 hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.965360 hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.965360 hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_0/dir_0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.985360 hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/
--rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_0_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_1_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_2_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_3_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_4_0.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.965360 hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.965360 hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/dir_0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.985360 hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/
--rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_0_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_1_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_2_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_3_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_4_0.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.989360 hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_0_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_1_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_2_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_3_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_4_0.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.989360 hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/
--rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_0_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_1_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_2_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_3_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_4_0.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.989360 hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_0_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_1_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_2_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_3_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_4_0.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.965360 hipscat_import-0.3.0/tests/hipscat_import/data/resume/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.965360 hipscat_import-0.3.0/tests/hipscat_import/data/resume/Norder=0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.989360 hipscat_import-0.3.0/tests/hipscat_import/data/resume/Norder=0/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)     8915 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/resume/Norder=0/Dir=0/Npix=11.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.965360 hipscat_import-0.3.0/tests/hipscat_import/data/resume/Norder=1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.989360 hipscat_import-0.3.0/tests/hipscat_import/data/resume/Norder=1/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=44.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=45.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=46.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=47.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.989360 hipscat_import-0.3.0/tests/hipscat_import/data/resume/intermediate/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/resume/intermediate/mapping_histogram.binary
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.989360 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky/
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky/catalog.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.993361 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_object_catalog/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.965360 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.993361 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/Dir=0/Npix=11.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_object_catalog/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_object_catalog/_metadata
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_object_catalog/catalog_info.json
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_object_catalog/partition_info.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_object_catalog/point_map.fits
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_object_catalog/provenance_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.993361 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_parts/
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_parts/catalog_00_of_05.csv
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_parts/catalog_01_of_05.csv
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_parts/catalog_02_of_05.csv
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_parts/catalog_03_of_05.csv
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_parts/catalog_04_of_05.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.993361 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source/
--rw-r--r--   0 runner    (1001) docker     (127)  1688789 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source/small_sky_source.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.997361 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source_catalog/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.965360 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.997361 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/Dir=0/Npix=4.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.965360 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.997361 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)   133671 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/Dir=0/Npix=47.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.965360 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:05.001361 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)    28346 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=176.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    86262 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=177.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    92634 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=178.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    99874 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=179.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    42177 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=180.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    54742 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=181.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    72960 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=182.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    67771 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=183.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    80265 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=184.parquet
--rw-r--r--   0 runner    (1001) docker     (127)   162064 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=185.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    31761 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=186.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    43705 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=187.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source_catalog/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (127)    28968 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source_catalog/_metadata
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source_catalog/catalog_info.json
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source_catalog/partition_info.csv
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source_catalog/point_map.fits
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source_catalog/provenance_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:05.005361 hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/0_4.csv
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/1_47.csv
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/2_176.csv
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/2_177.csv
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/2_178.csv
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/2_179.csv
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/2_180.csv
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/2_181.csv
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/2_182.csv
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/2_183.csv
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/2_184.csv
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/2_185.csv
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/2_186.csv
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/2_187.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.965360 hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/order_0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:04.965360 hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:05.009361 hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/
--rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_0_4.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    33062 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_1_47.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    10443 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_176.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    22870 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_177.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    24239 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_178.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    25729 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_179.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    13370 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_180.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    16010 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_181.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    19958 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_182.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    18844 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_183.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    21542 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_184.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    39137 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_185.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    11136 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_186.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    13692 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_187.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:05.009361 hipscat_import-0.3.0/tests/hipscat_import/data/test_formats/
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/test_formats/catalog.starr
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/test_formats/gaia_minimum.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/test_formats/gaia_minimum_schema.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/test_formats/headers.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/test_formats/hipscat_index.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/test_formats/hipscat_index.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/test_formats/macauff_metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/test_formats/pandasindex.parquet
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/test_formats/pipe_delimited.csv
--rw-r--r--   0 runner    (1001) docker     (127)    11520 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/data/test_formats/small_sky.fits
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:05.009361 hipscat_import-0.3.0/tests/hipscat_import/index/
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/index/test_index_argument.py
--rw-r--r--   0 runner    (1001) docker     (127)     7110 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/index/test_index_map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/index/test_run_index.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:05.013361 hipscat_import-0.3.0/tests/hipscat_import/margin_cache/
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/margin_cache/test_arguments_margin_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/margin_cache/test_margin_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/margin_cache/test_margin_cache_map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/margin_cache/test_margin_round_trip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:05.013361 hipscat_import-0.3.0/tests/hipscat_import/soap/
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/soap/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     7832 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/soap/test_run_soap.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/soap/test_soap_arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     6053 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/soap/test_soap_map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     7271 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/soap/test_soap_resume_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/test_pipeline_resume_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/test_runtime_arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:57:05.013361 hipscat_import-0.3.0/tests/hipscat_import/verification/
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/verification/test_run_verification.py
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-04-22 15:56:58.000000 hipscat_import-0.3.0/tests/hipscat_import/verification/test_verification_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.966298 hipscat_import-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.922298 hipscat_import-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.922298 hipscat_import-0.3.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.926298 hipscat_import-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/.github/workflows/build-documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/.github/workflows/pre-commit-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/.setup_dev.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-04-24 16:22:19.966298 hipscat_import-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.926298 hipscat_import-0.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.926298 hipscat_import-0.3.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.926298 hipscat_import-0.3.1/docs/catalogs/
+-rw-r--r--   0 runner    (1001) docker     (127)    13620 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/catalogs/arguments.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.926298 hipscat_import-0.3.1/docs/catalogs/public/
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/catalogs/public/allwise.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/catalogs/public/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/catalogs/public/neowise.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/catalogs/public/panstarrs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/catalogs/public/sdss.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/catalogs/public/tic.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/catalogs/public/zubercal.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10736 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/catalogs/temp_files.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.930298 hipscat_import-0.3.1/docs/guide/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/guide/contact.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/guide/dask_on_ray.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12082 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/guide/index_table.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/guide/margin_cache.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.930298 hipscat_import-0.3.1/docs/notebooks/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7615 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/notebooks/estimate_pixel_threshold.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/notebooks/unequal_schema.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/notebooks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.930298 hipscat_import-0.3.1/docs/static/
+-rw-r--r--   0 runner    (1001) docker     (127)   136863 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/static/allwise_schema.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/static/allwise_types.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    66486 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/static/neowise_schema.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/static/neowise_types.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/static/ps1_detections_types.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/static/ps1_otmo_types.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   412559 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/static/sdss_wget.bash
+-rw-r--r--   0 runner    (1001) docker     (127)    57050 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/static/tic_schema.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/static/tic_types.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 16:22:19.966298 hipscat_import-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.930298 hipscat_import-0.3.1/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    20810 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.934298 hipscat_import-0.3.1/src/hipscat_import/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-24 16:22:19.000000 hipscat_import-0.3.1/src/hipscat_import/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.934298 hipscat_import-0.3.1/src/hipscat_import/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8560 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/catalog/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9758 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/catalog/file_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12329 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/catalog/map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12059 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/catalog/resume_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/catalog/run_import.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.934298 hipscat_import-0.3.1/src/hipscat_import/index/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/index/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/index/map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/index/run_index.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.934298 hipscat_import-0.3.1/src/hipscat_import/margin_cache/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/margin_cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/margin_cache/margin_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/margin_cache/margin_cache_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/margin_cache/margin_cache_map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8004 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/pipeline_resume_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6626 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/runtime_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.938298 hipscat_import-0.3.1/src/hipscat_import/soap/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/soap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/soap/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10153 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/soap/map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9464 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/soap/resume_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/soap/run_soap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.938298 hipscat_import-0.3.1/src/hipscat_import/verification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/verification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/verification/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/verification/run_verification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.966298 hipscat_import-0.3.1/src/hipscat_import.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-04-24 16:22:19.000000 hipscat_import-0.3.1/src/hipscat_import.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11718 2024-04-24 16:22:19.000000 hipscat_import-0.3.1/src/hipscat_import.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 16:22:19.000000 hipscat_import-0.3.1/src/hipscat_import.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-24 16:22:19.000000 hipscat_import-0.3.1/src/hipscat_import.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-24 16:22:19.000000 hipscat_import-0.3.1/src/hipscat_import.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.938298 hipscat_import-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    20888 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.938298 hipscat_import-0.3.1/tests/hipscat_import/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.938298 hipscat_import-0.3.1/tests/hipscat_import/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/catalog/test_argument_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9441 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/catalog/test_file_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17181 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/catalog/test_map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8694 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/catalog/test_resume_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13396 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/catalog/test_run_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16162 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/catalog/test_run_round_trip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9441 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.922298 hipscat_import-0.3.1/tests/hipscat_import/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.938298 hipscat_import-0.3.1/tests/hipscat_import/data/blank/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/blank/blank.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.938298 hipscat_import-0.3.1/tests/hipscat_import/data/mixed_schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/mixed_schema/input_01.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/mixed_schema/input_02.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/mixed_schema/schema.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.918298 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.918298 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.918298 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_0/dir_0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.942298 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/
+-rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_0_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_1_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_2_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_3_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_4_0.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.918298 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.918298 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.942298 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/
+-rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_0_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_1_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_2_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_3_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_4_0.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.942298 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_0_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_1_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_2_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_3_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_4_0.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.942298 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/
+-rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_0_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_1_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_2_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_3_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_4_0.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.946298 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_0_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_1_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_2_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_3_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_4_0.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.918298 hipscat_import-0.3.1/tests/hipscat_import/data/resume/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.918298 hipscat_import-0.3.1/tests/hipscat_import/data/resume/Norder=0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.946298 hipscat_import-0.3.1/tests/hipscat_import/data/resume/Norder=0/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8915 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/resume/Norder=0/Dir=0/Npix=11.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.918298 hipscat_import-0.3.1/tests/hipscat_import/data/resume/Norder=1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.946298 hipscat_import-0.3.1/tests/hipscat_import/data/resume/Norder=1/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=44.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=45.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=46.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=47.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.946298 hipscat_import-0.3.1/tests/hipscat_import/data/resume/intermediate/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/resume/intermediate/mapping_histogram.binary
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.946298 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky/
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky/catalog.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.950298 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_object_catalog/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.918298 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.950298 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/Dir=0/Npix=11.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_object_catalog/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_object_catalog/_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_object_catalog/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_object_catalog/partition_info.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_object_catalog/point_map.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_object_catalog/provenance_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.950298 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_parts/
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_parts/catalog_00_of_05.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_parts/catalog_01_of_05.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_parts/catalog_02_of_05.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_parts/catalog_03_of_05.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_parts/catalog_04_of_05.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.950298 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source/
+-rw-r--r--   0 runner    (1001) docker     (127)  1688789 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source/small_sky_source.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.954298 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.918298 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.954298 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/Dir=0/Npix=4.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.918298 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.954298 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)   133671 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/Dir=0/Npix=47.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.918298 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.954298 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)    28346 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=176.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    86262 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=177.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    92634 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=178.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    99874 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=179.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    42177 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=180.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    54742 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=181.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    72960 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=182.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    67771 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=183.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    80265 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=184.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)   162064 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=185.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    31761 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=186.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    43705 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=187.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)    28968 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/partition_info.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/point_map.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/provenance_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.958298 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/0_4.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/1_47.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/2_176.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/2_177.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/2_178.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/2_179.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/2_180.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/2_181.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/2_182.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/2_183.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/2_184.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/2_185.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/2_186.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/2_187.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.918298 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.918298 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.962298 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/
+-rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_0_4.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    33062 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_1_47.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    10443 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_176.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    22870 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_177.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    24239 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_178.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    25729 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_179.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    13370 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_180.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    16010 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_181.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    19958 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_182.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    18844 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_183.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    21542 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_184.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    39137 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_185.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    11136 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_186.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    13692 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_187.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.962298 hipscat_import-0.3.1/tests/hipscat_import/data/test_formats/
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/test_formats/catalog.starr
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/test_formats/gaia_minimum.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/test_formats/gaia_minimum_schema.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/test_formats/headers.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/test_formats/hipscat_index.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/test_formats/hipscat_index.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/test_formats/macauff_metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/test_formats/pandasindex.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/test_formats/pipe_delimited.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    11520 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/test_formats/small_sky.fits
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.962298 hipscat_import-0.3.1/tests/hipscat_import/index/
+-rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/index/test_index_argument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7110 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/index/test_index_map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/index/test_run_index.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.962298 hipscat_import-0.3.1/tests/hipscat_import/margin_cache/
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/margin_cache/test_arguments_margin_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/margin_cache/test_margin_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/margin_cache/test_margin_cache_map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/margin_cache/test_margin_round_trip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.966298 hipscat_import-0.3.1/tests/hipscat_import/soap/
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/soap/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7832 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/soap/test_run_soap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/soap/test_soap_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6053 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/soap/test_soap_map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7271 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/soap/test_soap_resume_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/test_pipeline_resume_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/test_runtime_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.966298 hipscat_import-0.3.1/tests/hipscat_import/verification/
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/verification/test_run_verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/verification/test_verification_arguments.py
```

### Comparing `hipscat_import-0.3.0/.copier-answers.yml` & `hipscat_import-0.3.1/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/.gitattributes` & `hipscat_import-0.3.1/.gitattributes`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/.github/ISSUE_TEMPLATE/1-bug_report.md` & `hipscat_import-0.3.1/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/.github/ISSUE_TEMPLATE/2-feature_request.md` & `hipscat_import-0.3.1/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/.github/pull_request_template.md` & `hipscat_import-0.3.1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/.github/workflows/build-documentation.yml` & `hipscat_import-0.3.1/.github/workflows/build-documentation.yml`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/.github/workflows/pre-commit-ci.yml` & `hipscat_import-0.3.1/.github/workflows/pre-commit-ci.yml`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/.github/workflows/publish-to-pypi.yml` & `hipscat_import-0.3.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/.github/workflows/smoke-test.yml` & `hipscat_import-0.3.1/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/.github/workflows/testing-and-coverage.yml` & `hipscat_import-0.3.1/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/.gitignore` & `hipscat_import-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/.pre-commit-config.yaml` & `hipscat_import-0.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/.setup_dev.sh` & `hipscat_import-0.3.1/.setup_dev.sh`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/LICENSE` & `hipscat_import-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/PKG-INFO` & `hipscat_import-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hipscat-import
-Version: 0.3.0
+Version: 0.3.1
 Author-email: LINCC Frameworks <lincc-frameworks-team@lists.lsst.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, LINCC Frameworks
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -35,16 +35,15 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: dask<=2024.2.0
-Requires-Dist: dask[distributed]
+Requires-Dist: dask[complete]>=2024.3.0
 Requires-Dist: deprecated
 Requires-Dist: healpy
 Requires-Dist: hipscat>=0.2.9
 Requires-Dist: ipykernel
 Requires-Dist: pandas
 Requires-Dist: pyarrow
 Requires-Dist: pyyaml
```

### Comparing `hipscat_import-0.3.0/README.md` & `hipscat_import-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/docs/Makefile` & `hipscat_import-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/docs/catalogs/arguments.rst` & `hipscat_import-0.3.1/docs/catalogs/arguments.rst`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/docs/catalogs/public/allwise.rst` & `hipscat_import-0.3.1/docs/catalogs/public/allwise.rst`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/docs/catalogs/public/index.rst` & `hipscat_import-0.3.1/docs/catalogs/public/index.rst`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/docs/catalogs/public/neowise.rst` & `hipscat_import-0.3.1/docs/catalogs/public/neowise.rst`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/docs/catalogs/public/panstarrs.rst` & `hipscat_import-0.3.1/docs/catalogs/public/panstarrs.rst`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/docs/catalogs/public/sdss.rst` & `hipscat_import-0.3.1/docs/catalogs/public/sdss.rst`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/docs/catalogs/public/tic.rst` & `hipscat_import-0.3.1/docs/catalogs/public/tic.rst`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/docs/catalogs/public/zubercal.rst` & `hipscat_import-0.3.1/docs/catalogs/public/zubercal.rst`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/docs/catalogs/temp_files.rst` & `hipscat_import-0.3.1/docs/catalogs/temp_files.rst`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/docs/conf.py` & `hipscat_import-0.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/docs/guide/contact.rst` & `hipscat_import-0.3.1/docs/guide/contact.rst`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/docs/guide/contributing.rst` & `hipscat_import-0.3.1/docs/guide/contributing.rst`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/docs/guide/dask_on_ray.rst` & `hipscat_import-0.3.1/docs/guide/dask_on_ray.rst`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/docs/guide/index_table.rst` & `hipscat_import-0.3.1/docs/guide/index_table.rst`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/docs/guide/margin_cache.rst` & `hipscat_import-0.3.1/docs/guide/margin_cache.rst`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/docs/index.rst` & `hipscat_import-0.3.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/docs/notebooks/estimate_pixel_threshold.ipynb` & `hipscat_import-0.3.1/docs/notebooks/estimate_pixel_threshold.ipynb`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/docs/notebooks/unequal_schema.ipynb` & `hipscat_import-0.3.1/docs/notebooks/unequal_schema.ipynb`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/docs/static/allwise_schema.parquet` & `hipscat_import-0.3.1/docs/static/allwise_schema.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/docs/static/allwise_types.csv` & `hipscat_import-0.3.1/docs/static/allwise_types.csv`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/docs/static/neowise_schema.parquet` & `hipscat_import-0.3.1/docs/static/neowise_schema.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/docs/static/neowise_types.csv` & `hipscat_import-0.3.1/docs/static/neowise_types.csv`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/docs/static/ps1_detections_types.csv` & `hipscat_import-0.3.1/docs/static/ps1_detections_types.csv`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/docs/static/ps1_otmo_types.csv` & `hipscat_import-0.3.1/docs/static/ps1_otmo_types.csv`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/docs/static/sdss_wget.bash` & `hipscat_import-0.3.1/docs/static/sdss_wget.bash`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/docs/static/tic_schema.parquet` & `hipscat_import-0.3.1/docs/static/tic_schema.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/docs/static/tic_types.csv` & `hipscat_import-0.3.1/docs/static/tic_types.csv`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/pyproject.toml` & `hipscat_import-0.3.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -11,16 +11,15 @@
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
 ]
 dynamic = ["version"]
 dependencies = [
-    "dask<=2024.2.0",
-    "dask[distributed]",
+    "dask[complete]>=2024.3.0", # Includes dask expressions.
     "deprecated",
     "healpy",
     "hipscat >= 0.2.9",
     "ipykernel", # Support for Jupyter notebooks
     "pandas",
     "pyarrow",
     "pyyaml",
```

### Comparing `hipscat_import-0.3.0/src/.pylintrc` & `hipscat_import-0.3.1/src/.pylintrc`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/src/hipscat_import/catalog/arguments.py` & `hipscat_import-0.3.1/src/hipscat_import/catalog/arguments.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/src/hipscat_import/catalog/file_readers.py` & `hipscat_import-0.3.1/src/hipscat_import/catalog/file_readers.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/src/hipscat_import/catalog/map_reduce.py` & `hipscat_import-0.3.1/src/hipscat_import/catalog/map_reduce.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/src/hipscat_import/catalog/resume_plan.py` & `hipscat_import-0.3.1/src/hipscat_import/catalog/resume_plan.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/src/hipscat_import/catalog/run_import.py` & `hipscat_import-0.3.1/src/hipscat_import/catalog/run_import.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 def _map_pixels(args, client):
     """Generate a raw histogram of object counts in each healpix pixel"""
 
     if args.resume_plan.is_mapping_done():
         return
 
-    reader_future = client.scatter(args.file_reader)
+    reader_future = client.scatter(args.file_reader, hash=False)
     futures = []
     for key, file_path in args.resume_plan.map_files:
         futures.append(
             client.submit(
                 mr.map_to_pixels,
                 input_file=file_path,
                 resume_path=args.resume_plan.tmp_path,
@@ -44,15 +44,15 @@
 
 def _split_pixels(args, alignment_future, client):
     """Generate a raw histogram of object counts in each healpix pixel"""
 
     if args.resume_plan.is_splitting_done():
         return
 
-    reader_future = client.scatter(args.file_reader)
+    reader_future = client.scatter(args.file_reader, hash=False)
     futures = []
     for key, file_path in args.resume_plan.split_keys:
         futures.append(
             client.submit(
                 mr.split_pixels,
                 input_file=file_path,
                 file_reader=reader_future,
```

### Comparing `hipscat_import-0.3.0/src/hipscat_import/index/arguments.py` & `hipscat_import-0.3.1/src/hipscat_import/index/arguments.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/src/hipscat_import/index/map_reduce.py` & `hipscat_import-0.3.1/src/hipscat_import/index/map_reduce.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/src/hipscat_import/index/run_index.py` & `hipscat_import-0.3.1/src/hipscat_import/index/run_index.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/src/hipscat_import/margin_cache/margin_cache.py` & `hipscat_import-0.3.1/src/hipscat_import/margin_cache/margin_cache.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/src/hipscat_import/margin_cache/margin_cache_arguments.py` & `hipscat_import-0.3.1/src/hipscat_import/margin_cache/margin_cache_arguments.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/src/hipscat_import/margin_cache/margin_cache_map_reduce.py` & `hipscat_import-0.3.1/src/hipscat_import/margin_cache/margin_cache_map_reduce.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/src/hipscat_import/pipeline.py` & `hipscat_import-0.3.1/src/hipscat_import/pipeline.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/src/hipscat_import/pipeline_resume_plan.py` & `hipscat_import-0.3.1/src/hipscat_import/pipeline_resume_plan.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/src/hipscat_import/runtime_arguments.py` & `hipscat_import-0.3.1/src/hipscat_import/runtime_arguments.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/src/hipscat_import/soap/arguments.py` & `hipscat_import-0.3.1/src/hipscat_import/soap/arguments.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/src/hipscat_import/soap/map_reduce.py` & `hipscat_import-0.3.1/src/hipscat_import/soap/map_reduce.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/src/hipscat_import/soap/resume_plan.py` & `hipscat_import-0.3.1/src/hipscat_import/soap/resume_plan.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/src/hipscat_import/soap/run_soap.py` & `hipscat_import-0.3.1/src/hipscat_import/soap/run_soap.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/src/hipscat_import/verification/arguments.py` & `hipscat_import-0.3.1/src/hipscat_import/verification/arguments.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/src/hipscat_import/verification/run_verification.py` & `hipscat_import-0.3.1/src/hipscat_import/verification/run_verification.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/src/hipscat_import.egg-info/PKG-INFO` & `hipscat_import-0.3.1/src/hipscat_import.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hipscat-import
-Version: 0.3.0
+Version: 0.3.1
 Author-email: LINCC Frameworks <lincc-frameworks-team@lists.lsst.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, LINCC Frameworks
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -35,16 +35,15 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: dask<=2024.2.0
-Requires-Dist: dask[distributed]
+Requires-Dist: dask[complete]>=2024.3.0
 Requires-Dist: deprecated
 Requires-Dist: healpy
 Requires-Dist: hipscat>=0.2.9
 Requires-Dist: ipykernel
 Requires-Dist: pandas
 Requires-Dist: pyarrow
 Requires-Dist: pyyaml
```

### Comparing `hipscat_import-0.3.0/src/hipscat_import.egg-info/SOURCES.txt` & `hipscat_import-0.3.1/src/hipscat_import.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/.pylintrc` & `hipscat_import-0.3.1/tests/.pylintrc`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/conftest.py` & `hipscat_import-0.3.1/tests/conftest.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
         client = Client()
         yield client
         client.close()
 
         disable_dask_on_ray()
     else:
-        client = Client()
+        client = Client(n_workers=1, threads_per_worker=1)
         yield client
         client.close()
 
 
 def pytest_addoption(parser):
     """Add command line option to test dask unit tests on ray.
```

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/catalog/test_argument_validation.py` & `hipscat_import-0.3.1/tests/hipscat_import/catalog/test_argument_validation.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/catalog/test_file_readers.py` & `hipscat_import-0.3.1/tests/hipscat_import/catalog/test_file_readers.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/catalog/test_map_reduce.py` & `hipscat_import-0.3.1/tests/hipscat_import/catalog/test_map_reduce.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/catalog/test_resume_plan.py` & `hipscat_import-0.3.1/tests/hipscat_import/catalog/test_resume_plan.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/catalog/test_run_import.py` & `hipscat_import-0.3.1/tests/hipscat_import/catalog/test_run_import.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/catalog/test_run_round_trip.py` & `hipscat_import-0.3.1/tests/hipscat_import/catalog/test_run_round_trip.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     assert catalog.on_disk
     assert catalog.catalog_path == args.catalog_path
     assert catalog.catalog_info.ra_column == "source_ra"
     assert catalog.catalog_info.dec_column == "source_dec"
     assert len(catalog.get_healpix_pixels()) == 14
 
 
-@pytest.mark.dask(timeout=10)
+@pytest.mark.dask
 def test_import_mixed_schema_csv(
     dask_client,
     mixed_schema_csv_dir,
     mixed_schema_csv_parquet,
     assert_parquet_file_ids,
     tmp_path,
 ):
```

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/conftest.py` & `hipscat_import-0.3.1/tests/hipscat_import/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     """
     use_ray = config.getoption("--use_ray")
     skip_ray = pytest.mark.skip(reason="skipping this test under dask-on-ray")
     first_dask = True
     for item in items:
         timeout = None
         for mark in item.iter_markers(name="dask"):
-            timeout = 5
+            timeout = 10
             if "timeout" in mark.kwargs:
                 timeout = int(mark.kwargs.get("timeout"))
             if "skip_ray" in mark.kwargs and use_ray:
                 item.add_marker(skip_ray)
         if timeout:
             if first_dask:
                 ## The first test requires more time to set up the dask/ray client
```

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/mixed_schema/schema.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/mixed_schema/schema.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_0_0.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_0_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_1_0.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_1_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_2_0.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_2_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_3_0.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_3_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_4_0.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_4_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_0_0.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_0_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_1_0.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_1_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_2_0.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_2_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_3_0.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_3_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_4_0.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_4_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_0_0.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_0_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_1_0.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_1_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_2_0.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_2_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_3_0.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_3_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_4_0.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_4_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_0_0.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_0_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_1_0.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_1_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_2_0.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_2_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_3_0.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_3_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_4_0.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_4_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_0_0.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_0_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_1_0.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_1_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_2_0.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_2_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_3_0.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_3_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_4_0.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_4_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/resume/Norder=0/Dir=0/Npix=11.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/resume/Norder=0/Dir=0/Npix=11.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=44.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=44.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=45.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=45.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=46.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=46.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=47.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=47.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/small_sky/catalog.csv` & `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky/catalog.csv`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/Dir=0/Npix=11.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/Dir=0/Npix=11.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_object_catalog/_common_metadata` & `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_object_catalog/_common_metadata`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_object_catalog/_metadata` & `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_object_catalog/_metadata`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_object_catalog/point_map.fits` & `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_object_catalog/point_map.fits`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_object_catalog/provenance_info.json` & `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_object_catalog/provenance_info.json`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_parts/catalog_00_of_05.csv` & `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_parts/catalog_00_of_05.csv`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_parts/catalog_01_of_05.csv` & `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_parts/catalog_01_of_05.csv`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_parts/catalog_02_of_05.csv` & `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_parts/catalog_02_of_05.csv`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_parts/catalog_03_of_05.csv` & `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_parts/catalog_03_of_05.csv`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_parts/catalog_04_of_05.csv` & `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_parts/catalog_04_of_05.csv`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source/small_sky_source.csv` & `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source/small_sky_source.csv`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/Dir=0/Npix=4.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/Dir=0/Npix=4.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/Dir=0/Npix=47.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/Dir=0/Npix=47.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=176.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=176.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=177.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=177.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=178.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=178.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=179.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=179.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=180.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=180.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=181.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=181.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=182.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=182.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=183.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=183.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=184.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=184.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=185.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=185.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=186.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=186.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=187.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=187.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source_catalog/_common_metadata` & `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/_common_metadata`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source_catalog/_metadata` & `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/_metadata`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source_catalog/point_map.fits` & `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/point_map.fits`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/small_sky_source_catalog/provenance_info.json` & `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/provenance_info.json`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_0_4.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_0_4.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_1_47.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_1_47.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_176.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_176.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_177.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_177.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_178.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_178.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_179.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_179.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_180.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_180.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_181.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_181.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_182.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_182.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_183.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_183.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_184.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_184.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_185.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_185.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_186.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_186.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_187.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_187.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/test_formats/catalog.starr` & `hipscat_import-0.3.1/tests/hipscat_import/data/test_formats/catalog.starr`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/test_formats/gaia_minimum.csv` & `hipscat_import-0.3.1/tests/hipscat_import/data/test_formats/gaia_minimum.csv`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/test_formats/gaia_minimum_schema.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/test_formats/gaia_minimum_schema.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/test_formats/hipscat_index.csv` & `hipscat_import-0.3.1/tests/hipscat_import/data/test_formats/hipscat_index.csv`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/test_formats/hipscat_index.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/test_formats/hipscat_index.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/test_formats/pandasindex.parquet` & `hipscat_import-0.3.1/tests/hipscat_import/data/test_formats/pandasindex.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/data/test_formats/small_sky.fits` & `hipscat_import-0.3.1/tests/hipscat_import/data/test_formats/small_sky.fits`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/index/test_index_argument.py` & `hipscat_import-0.3.1/tests/hipscat_import/index/test_index_argument.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/index/test_index_map_reduce.py` & `hipscat_import-0.3.1/tests/hipscat_import/index/test_index_map_reduce.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/index/test_run_index.py` & `hipscat_import-0.3.1/tests/hipscat_import/index/test_run_index.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/margin_cache/test_arguments_margin_cache.py` & `hipscat_import-0.3.1/tests/hipscat_import/margin_cache/test_arguments_margin_cache.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/margin_cache/test_margin_cache.py` & `hipscat_import-0.3.1/tests/hipscat_import/margin_cache/test_margin_cache.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/margin_cache/test_margin_cache_map_reduce.py` & `hipscat_import-0.3.1/tests/hipscat_import/margin_cache/test_margin_cache_map_reduce.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/margin_cache/test_margin_round_trip.py` & `hipscat_import-0.3.1/tests/hipscat_import/margin_cache/test_margin_round_trip.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/soap/conftest.py` & `hipscat_import-0.3.1/tests/hipscat_import/soap/conftest.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/soap/test_run_soap.py` & `hipscat_import-0.3.1/tests/hipscat_import/soap/test_run_soap.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/soap/test_soap_arguments.py` & `hipscat_import-0.3.1/tests/hipscat_import/soap/test_soap_arguments.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/soap/test_soap_map_reduce.py` & `hipscat_import-0.3.1/tests/hipscat_import/soap/test_soap_map_reduce.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/soap/test_soap_resume_plan.py` & `hipscat_import-0.3.1/tests/hipscat_import/soap/test_soap_resume_plan.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/test_pipeline_resume_plan.py` & `hipscat_import-0.3.1/tests/hipscat_import/test_pipeline_resume_plan.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/test_runtime_arguments.py` & `hipscat_import-0.3.1/tests/hipscat_import/test_runtime_arguments.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/verification/test_run_verification.py` & `hipscat_import-0.3.1/tests/hipscat_import/verification/test_run_verification.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.0/tests/hipscat_import/verification/test_verification_arguments.py` & `hipscat_import-0.3.1/tests/hipscat_import/verification/test_verification_arguments.py`

 * *Files identical despite different names*

