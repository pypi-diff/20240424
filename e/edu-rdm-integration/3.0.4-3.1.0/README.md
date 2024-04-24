# Comparing `tmp/edu-rdm-integration-3.0.4.tar.gz` & `tmp/edu-rdm-integration-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edu-rdm-integration-3.0.4.tar", last modified: Wed Apr 17 09:27:08 2024, max compression
+gzip compressed data, was "edu-rdm-integration-3.1.0.tar", last modified: Wed Apr 24 07:06:14 2024, max compression
```

## Comparing `edu-rdm-integration-3.0.4.tar` & `edu-rdm-integration-3.1.0.tar`

### file list

```diff
@@ -1,216 +1,216 @@
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-17 09:27:08.840003 edu-rdm-integration-3.0.4/
--rw-r--r--   0 toor      (1000) toor      (1000)    42155 2024-04-17 09:27:03.000000 edu-rdm-integration-3.0.4/CHANGELOG.md
--rwxr-xr-x   0 toor      (1000) toor      (1000)     5358 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/CONDUCT.md
--rw-r--r--   0 toor      (1000) toor      (1000)     3458 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/LICENSE
--rw-r--r--   0 toor      (1000) toor      (1000)      206 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/MANIFEST.in
--rw-r--r--   0 toor      (1000) toor      (1000)    61229 2024-04-17 09:27:08.840003 edu-rdm-integration-3.0.4/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)    17793 2024-03-07 13:08:26.000000 edu-rdm-integration-3.0.4/README.md
--rw-r--r--   0 toor      (1000) toor      (1000)      171 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/pyproject.toml
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-17 09:27:08.705003 edu-rdm-integration-3.0.4/requirements/
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-17 09:27:08.710003 edu-rdm-integration-3.0.4/requirements/dependencies/
--rw-r--r--   0 toor      (1000) toor      (1000)       89 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/requirements/dependencies/development_packages.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       52 2024-03-18 08:19:35.000000 edu-rdm-integration-3.0.4/requirements/dependencies/external_packages.txt
--rw-r--r--   0 toor      (1000) toor      (1000)      122 2024-03-18 08:19:35.000000 edu-rdm-integration-3.0.4/requirements/dependencies/internal_packages.txt
--rw-r--r--   0 toor      (1000) toor      (1000)      372 2024-03-18 08:19:35.000000 edu-rdm-integration-3.0.4/requirements/dependencies/internal_sources.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       49 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/requirements/dependencies/production_packages.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       78 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/requirements/dependencies/system_packages.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/requirements/dependencies/testing_packages.txt
--rw-r--r--   0 toor      (1000) toor      (1000)      188 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/requirements/development.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       75 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/requirements/production.txt
--rw-r--r--   0 toor      (1000) toor      (1000)      189 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/requirements/stage.txt
--rw-r--r--   0 toor      (1000) toor      (1000)      471 2024-04-17 09:27:08.841003 edu-rdm-integration-3.0.4/setup.cfg
--rw-r--r--   0 toor      (1000) toor      (1000)     2956 2024-04-17 09:27:03.000000 edu-rdm-integration-3.0.4/setup.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-17 09:27:08.696003 edu-rdm-integration-3.0.4/src/
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-17 09:27:08.723003 edu-rdm-integration-3.0.4/src/edu_rdm_integration/
--rw-r--r--   0 toor      (1000) toor      (1000)       72 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-17 09:27:08.739003 edu-rdm-integration-3.0.4/src/edu_rdm_integration/adapters/
--rw-r--r--   0 toor      (1000) toor      (1000)       83 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/adapters/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      363 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/adapters/apps.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1505 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/adapters/caches.py
--rw-r--r--   0 toor      (1000) toor      (1000)       66 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/adapters/consts.py
--rw-r--r--   0 toor      (1000) toor      (1000)       93 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/adapters/enums.py
--rw-r--r--   0 toor      (1000) toor      (1000)      255 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/adapters/errors.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2076 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/adapters/functions.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1106 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/adapters/helpers.py
--rw-r--r--   0 toor      (1000) toor      (1000)      590 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/adapters/managers.py
--rw-r--r--   0 toor      (1000) toor      (1000)      327 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/adapters/presenters.py
--rw-r--r--   0 toor      (1000) toor      (1000)      598 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/adapters/receivers.py
--rw-r--r--   0 toor      (1000) toor      (1000)      515 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/adapters/results.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2664 2024-02-20 14:08:27.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/adapters/runners.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5505 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/adapters/strategies.py
--rw-r--r--   0 toor      (1000) toor      (1000)      181 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/adapters/strings.py
--rw-r--r--   0 toor      (1000) toor      (1000)       59 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/adapters/tests.py
--rw-r--r--   0 toor      (1000) toor      (1000)      496 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/adapters/validators.py
--rw-r--r--   0 toor      (1000) toor      (1000)      337 2024-01-15 06:45:08.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/app_meta.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2056 2024-03-07 13:08:26.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/app_settings.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3571 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/apps.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1341 2023-12-15 06:35:54.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/base.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-17 09:27:08.744003 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_and_export_data/
--rw-r--r--   0 toor      (1000) toor      (1000)       82 2024-03-26 10:01:36.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_and_export_data/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      160 2024-03-26 10:01:36.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_and_export_data/apps.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-17 09:27:08.745003 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_and_export_data/migrations/
--rw-r--r--   0 toor      (1000) toor      (1000)     4714 2024-03-26 10:01:36.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_and_export_data/migrations/0001_initial.py
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-03-26 10:01:36.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_and_export_data/migrations/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2038 2024-03-29 11:36:54.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_and_export_data/models.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3546 2024-04-17 09:27:03.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_and_export_data/utils.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-17 09:27:08.750003 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-17 09:27:08.756003 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/base/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/base/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2170 2024-02-20 14:08:27.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/base/caches.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2998 2024-02-20 14:08:27.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/base/functions.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1017 2023-12-13 13:36:37.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/base/helpers.py
--rw-r--r--   0 toor      (1000) toor      (1000)     6172 2024-02-20 14:08:27.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/base/managers.py
--rw-r--r--   0 toor      (1000) toor      (1000)     8521 2024-02-20 14:08:27.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/base/mixins.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1565 2024-03-14 19:45:32.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/base/runners.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-17 09:27:08.757003 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/calculated/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/calculated/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-17 09:27:08.768003 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/calculated/base/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/calculated/base/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2838 2024-02-20 14:08:27.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/calculated/base/caches.py
--rw-r--r--   0 toor      (1000) toor      (1000)       84 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/calculated/base/consts.py
--rw-r--r--   0 toor      (1000) toor      (1000)       93 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/calculated/base/enums.py
--rw-r--r--   0 toor      (1000) toor      (1000)      326 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/calculated/base/errors.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1670 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/calculated/base/functions.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1547 2023-12-13 13:36:37.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/calculated/base/helpers.py
--rw-r--r--   0 toor      (1000) toor      (1000)      838 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/calculated/base/managers.py
--rw-r--r--   0 toor      (1000) toor      (1000)      438 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/calculated/base/presenters.py
--rw-r--r--   0 toor      (1000) toor      (1000)      708 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/calculated/base/results.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1626 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/calculated/base/runners.py
--rw-r--r--   0 toor      (1000) toor      (1000)      181 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/calculated/base/strings.py
--rw-r--r--   0 toor      (1000) toor      (1000)       59 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/calculated/base/tests.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1057 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/calculated/base/validators.py
--rw-r--r--   0 toor      (1000) toor      (1000)     7629 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/calculated/strategies.py
--rw-r--r--   0 toor      (1000) toor      (1000)    14543 2024-03-06 15:50:06.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/collect.py
--rw-r--r--   0 toor      (1000) toor      (1000)     9075 2024-03-06 15:50:06.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/generators.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2995 2024-03-18 08:19:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/helpers.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-17 09:27:08.769003 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/non_calculated/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/non_calculated/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-17 09:27:08.780003 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/non_calculated/base/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/non_calculated/base/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     6589 2024-02-20 14:08:27.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/non_calculated/base/caches.py
--rw-r--r--   0 toor      (1000) toor      (1000)       66 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/non_calculated/base/consts.py
--rw-r--r--   0 toor      (1000) toor      (1000)       93 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/non_calculated/base/enums.py
--rw-r--r--   0 toor      (1000) toor      (1000)      297 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/non_calculated/base/errors.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1563 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/non_calculated/base/functions.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1433 2023-12-13 13:36:37.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/non_calculated/base/helpers.py
--rw-r--r--   0 toor      (1000) toor      (1000)      783 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/non_calculated/base/managers.py
--rw-r--r--   0 toor      (1000) toor      (1000)      409 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/non_calculated/base/presenters.py
--rw-r--r--   0 toor      (1000) toor      (1000)      674 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/non_calculated/base/results.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1519 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/non_calculated/base/runners.py
--rw-r--r--   0 toor      (1000) toor      (1000)      181 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/non_calculated/base/strings.py
--rw-r--r--   0 toor      (1000) toor      (1000)       59 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/non_calculated/base/tests.py
--rw-r--r--   0 toor      (1000) toor      (1000)      973 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/non_calculated/base/validators.py
--rw-r--r--   0 toor      (1000) toor      (1000)     7431 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/non_calculated/strategies.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5367 2024-03-18 08:19:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/tests.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1104 2023-12-13 13:36:37.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/consts.py
--rw-r--r--   0 toor      (1000) toor      (1000)    14552 2024-04-17 09:27:03.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/entities.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-17 09:27:08.783003 edu-rdm-integration-3.0.4/src/edu_rdm_integration/enum_register/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/enum_register/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4021 2024-03-18 08:19:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/enum_register/mixins.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2218 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/enum_register/register.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4246 2024-03-26 10:01:36.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/enums.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-17 09:27:08.788003 edu-rdm-integration-3.0.4/src/edu_rdm_integration/export_data/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/export_data/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-17 09:27:08.799003 edu-rdm-integration-3.0.4/src/edu_rdm_integration/export_data/base/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/export_data/base/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1541 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/export_data/base/caches.py
--rw-r--r--   0 toor      (1000) toor      (1000)      519 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/export_data/base/consts.py
--rw-r--r--   0 toor      (1000) toor      (1000)       93 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/export_data/base/enums.py
--rw-r--r--   0 toor      (1000) toor      (1000)      291 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/export_data/base/errors.py
--rw-r--r--   0 toor      (1000) toor      (1000)    12784 2024-04-17 09:27:03.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/export_data/base/functions.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4609 2024-04-03 12:03:40.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/export_data/base/helpers.py
--rw-r--r--   0 toor      (1000) toor      (1000)     6075 2024-02-20 14:08:27.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/export_data/base/managers.py
--rw-r--r--   0 toor      (1000) toor      (1000)      403 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/export_data/base/presenters.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2576 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/export_data/base/requests.py
--rw-r--r--   0 toor      (1000) toor      (1000)      662 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/export_data/base/results.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2521 2024-02-20 14:08:27.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/export_data/base/runners.py
--rw-r--r--   0 toor      (1000) toor      (1000)      181 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/export_data/base/strings.py
--rw-r--r--   0 toor      (1000) toor      (1000)       59 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/export_data/base/tests.py
--rw-r--r--   0 toor      (1000) toor      (1000)      961 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/export_data/base/validators.py
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/export_data/consts.py
--rw-r--r--   0 toor      (1000) toor      (1000)    17231 2024-03-07 13:08:27.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/export_data/export.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4020 2023-12-15 06:35:54.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/export_data/generators.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2933 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/export_data/helpers.py
--rw-r--r--   0 toor      (1000) toor      (1000)     6725 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/export_data/strategies.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-17 09:27:08.801003 edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-17 09:27:08.811003 edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_collect_data_template/
--rw-r--r--   0 toor      (1000) toor      (1000)      107 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_collect_data_template/__init__.py-tpl
--rw-r--r--   0 toor      (1000) toor      (1000)      319 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_collect_data_template/apps.py-tpl
--rw-r--r--   0 toor      (1000) toor      (1000)      963 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_collect_data_template/caches.py-tpl
--rw-r--r--   0 toor      (1000) toor      (1000)       66 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_collect_data_template/consts.py-tpl
--rw-r--r--   0 toor      (1000) toor      (1000)       93 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_collect_data_template/enums.py-tpl
--rw-r--r--   0 toor      (1000) toor      (1000)      247 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_collect_data_template/errors.py-tpl
--rw-r--r--   0 toor      (1000) toor      (1000)     5349 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_collect_data_template/functions.py-tpl
--rw-r--r--   0 toor      (1000) toor      (1000)     1254 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_collect_data_template/helpers.py-tpl
--rw-r--r--   0 toor      (1000) toor      (1000)     1731 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_collect_data_template/managers.py-tpl
--rw-r--r--   0 toor      (1000) toor      (1000)      316 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_collect_data_template/presenters.py-tpl
--rw-r--r--   0 toor      (1000) toor      (1000)      589 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_collect_data_template/results.py-tpl
--rw-r--r--   0 toor      (1000) toor      (1000)     2937 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_collect_data_template/runners.py-tpl
--rw-r--r--   0 toor      (1000) toor      (1000)      181 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_collect_data_template/strings.py-tpl
--rw-r--r--   0 toor      (1000) toor      (1000)      838 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_collect_data_template/tests.py-tpl
--rw-r--r--   0 toor      (1000) toor      (1000)      587 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_collect_data_template/validators.py-tpl
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-17 09:27:08.822003 edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_export_data_template/
--rw-r--r--   0 toor      (1000) toor      (1000)      107 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_export_data_template/__init__.py-tpl
--rw-r--r--   0 toor      (1000) toor      (1000)      319 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_export_data_template/apps.py-tpl
--rw-r--r--   0 toor      (1000) toor      (1000)     1054 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_export_data_template/caches.py-tpl
--rw-r--r--   0 toor      (1000) toor      (1000)       66 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_export_data_template/consts.py-tpl
--rw-r--r--   0 toor      (1000) toor      (1000)       93 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_export_data_template/enums.py-tpl
--rw-r--r--   0 toor      (1000) toor      (1000)      247 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_export_data_template/errors.py-tpl
--rw-r--r--   0 toor      (1000) toor      (1000)     2882 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_export_data_template/functions.py-tpl
--rw-r--r--   0 toor      (1000) toor      (1000)     1272 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_export_data_template/helpers.py-tpl
--rw-r--r--   0 toor      (1000) toor      (1000)     2671 2023-12-07 10:11:59.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_export_data_template/managers.py-tpl
--rw-r--r--   0 toor      (1000) toor      (1000)      316 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_export_data_template/presenters.py-tpl
--rw-r--r--   0 toor      (1000) toor      (1000)      589 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_export_data_template/results.py-tpl
--rw-r--r--   0 toor      (1000) toor      (1000)     3653 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_export_data_template/runners.py-tpl
--rw-r--r--   0 toor      (1000) toor      (1000)      181 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_export_data_template/strings.py-tpl
--rw-r--r--   0 toor      (1000) toor      (1000)       59 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_export_data_template/tests.py-tpl
--rw-r--r--   0 toor      (1000) toor      (1000)      587 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_export_data_template/validators.py-tpl
--rw-r--r--   0 toor      (1000) toor      (1000)    10997 2024-03-26 10:01:36.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/helpers.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-17 09:27:08.823003 edu-rdm-integration-3.0.4/src/edu_rdm_integration/management/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/management/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-17 09:27:08.830003 edu-rdm-integration-3.0.4/src/edu_rdm_integration/management/commands/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/management/commands/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3843 2024-01-11 11:42:02.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/management/commands/check_upload_status.py
--rw-r--r--   0 toor      (1000) toor      (1000)      750 2024-01-11 11:42:02.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/management/commands/collect_latest_models_data.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1022 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/management/commands/collect_models_data.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1211 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/management/commands/datamart_status.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1487 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/management/commands/datamart_upload.py
--rw-r--r--   0 toor      (1000) toor      (1000)      920 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/management/commands/export_entities_data.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1146 2024-01-11 11:42:02.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/management/commands/export_latest_entities_data.py
--rw-r--r--   0 toor      (1000) toor      (1000)    13439 2024-03-06 15:50:06.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/management/general.py
--rw-r--r--   0 toor      (1000) toor      (1000)      473 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/mapping.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-17 09:27:08.836003 edu-rdm-integration-3.0.4/src/edu_rdm_integration/migrations/
--rw-r--r--   0 toor      (1000) toor      (1000)    18719 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/migrations/0001_initial.py
--rw-r--r--   0 toor      (1000) toor      (1000)      737 2023-12-08 11:59:51.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/migrations/0002_init_data_uploadstatus.py
--rw-r--r--   0 toor      (1000) toor      (1000)      735 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/migrations/0003_create_index_file_upload_status.py
--rw-r--r--   0 toor      (1000) toor      (1000)      626 2023-12-08 11:41:16.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/migrations/0004_uploaderclientlog.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1782 2023-12-08 11:59:51.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/migrations/0005_auto_20231204_1224.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3448 2023-12-08 11:59:51.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/migrations/0006_request_status_data.py
--rw-r--r--   0 toor      (1000) toor      (1000)      457 2023-12-08 11:59:51.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/migrations/0007_delete_upload_status.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1427 2024-01-15 06:45:08.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/migrations/0008_transferredentity.py
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/migrations/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)    29327 2024-01-15 06:45:08.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/models.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-17 09:27:08.836003 edu-rdm-integration-3.0.4/src/edu_rdm_integration/registry/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-01-15 06:45:08.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/registry/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4146 2024-01-15 06:45:08.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/registry/actions.py
--rw-r--r--   0 toor      (1000) toor      (1000)       73 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/signals.py
--rw-r--r--   0 toor      (1000) toor      (1000)     6807 2023-12-04 16:17:35.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/storages.py
--rw-r--r--   0 toor      (1000) toor      (1000)    13716 2024-03-26 10:01:36.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/tasks.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-17 09:27:08.839003 edu-rdm-integration-3.0.4/src/edu_rdm_integration/uploader_log/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-12-08 11:41:16.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/uploader_log/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     6755 2023-12-13 08:36:13.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/uploader_log/actions.py
--rw-r--r--   0 toor      (1000) toor      (1000)      265 2023-12-08 11:41:16.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/uploader_log/apps.py
--rw-r--r--   0 toor      (1000) toor      (1000)      266 2023-12-08 11:41:16.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/uploader_log/enums.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3203 2023-12-11 20:05:53.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/uploader_log/managers.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2110 2023-12-13 08:36:13.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/uploader_log/ui.py
--rw-r--r--   0 toor      (1000) toor      (1000)    10369 2024-03-26 10:01:36.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration/utils.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-17 09:27:08.727003 edu-rdm-integration-3.0.4/src/edu_rdm_integration.egg-info/
--rw-r--r--   0 toor      (1000) toor      (1000)    61229 2024-04-17 09:27:08.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration.egg-info/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)    10685 2024-04-17 09:27:08.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration.egg-info/SOURCES.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2024-04-17 09:27:08.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration.egg-info/dependency_links.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2024-04-17 09:27:08.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration.egg-info/namespace_packages.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-12-04 16:17:43.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration.egg-info/not-zip-safe
--rw-r--r--   0 toor      (1000) toor      (1000)      253 2024-04-17 09:27:08.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration.egg-info/requires.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       20 2024-04-17 09:27:08.000000 edu-rdm-integration-3.0.4/src/edu_rdm_integration.egg-info/top_level.txt
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-24 07:06:14.281293 edu-rdm-integration-3.1.0/
+-rw-r--r--   0 toor      (1000) toor      (1000)    42526 2024-04-24 07:06:08.000000 edu-rdm-integration-3.1.0/CHANGELOG.md
+-rwxr-xr-x   0 toor      (1000) toor      (1000)     5358 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/CONDUCT.md
+-rw-r--r--   0 toor      (1000) toor      (1000)     3458 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/LICENSE
+-rw-r--r--   0 toor      (1000) toor      (1000)      206 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/MANIFEST.in
+-rw-r--r--   0 toor      (1000) toor      (1000)    61600 2024-04-24 07:06:14.281293 edu-rdm-integration-3.1.0/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)    17793 2024-03-07 13:08:26.000000 edu-rdm-integration-3.1.0/README.md
+-rw-r--r--   0 toor      (1000) toor      (1000)      175 2024-04-24 07:06:08.000000 edu-rdm-integration-3.1.0/pyproject.toml
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-24 07:06:14.234293 edu-rdm-integration-3.1.0/requirements/
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-24 07:06:14.235293 edu-rdm-integration-3.1.0/requirements/dependencies/
+-rw-r--r--   0 toor      (1000) toor      (1000)       89 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/requirements/dependencies/development_packages.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       52 2024-03-18 08:19:35.000000 edu-rdm-integration-3.1.0/requirements/dependencies/external_packages.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)      122 2024-03-18 08:19:35.000000 edu-rdm-integration-3.1.0/requirements/dependencies/internal_packages.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)      372 2024-03-18 08:19:35.000000 edu-rdm-integration-3.1.0/requirements/dependencies/internal_sources.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       49 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/requirements/dependencies/production_packages.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       78 2024-04-24 07:06:08.000000 edu-rdm-integration-3.1.0/requirements/dependencies/system_packages.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/requirements/dependencies/testing_packages.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)      188 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/requirements/development.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       75 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/requirements/production.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)      189 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/requirements/stage.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)      471 2024-04-24 07:06:14.282293 edu-rdm-integration-3.1.0/setup.cfg
+-rw-r--r--   0 toor      (1000) toor      (1000)     2956 2024-04-24 07:06:08.000000 edu-rdm-integration-3.1.0/setup.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-24 07:06:14.227293 edu-rdm-integration-3.1.0/src/
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-24 07:06:14.239293 edu-rdm-integration-3.1.0/src/edu_rdm_integration/
+-rw-r--r--   0 toor      (1000) toor      (1000)       72 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-24 07:06:14.245293 edu-rdm-integration-3.1.0/src/edu_rdm_integration/adapters/
+-rw-r--r--   0 toor      (1000) toor      (1000)       83 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/adapters/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      363 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/adapters/apps.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1505 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/adapters/caches.py
+-rw-r--r--   0 toor      (1000) toor      (1000)       66 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/adapters/consts.py
+-rw-r--r--   0 toor      (1000) toor      (1000)       93 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/adapters/enums.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      255 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/adapters/errors.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2076 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/adapters/functions.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1106 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/adapters/helpers.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      590 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/adapters/managers.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      327 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/adapters/presenters.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      598 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/adapters/receivers.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      515 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/adapters/results.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2664 2024-02-20 14:08:27.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/adapters/runners.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5505 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/adapters/strategies.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      181 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/adapters/strings.py
+-rw-r--r--   0 toor      (1000) toor      (1000)       59 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/adapters/tests.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      496 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/adapters/validators.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      337 2024-01-15 06:45:08.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/app_meta.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2056 2024-03-07 13:08:26.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/app_settings.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3571 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/apps.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1341 2023-12-15 06:35:54.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/base.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-24 07:06:14.246293 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_and_export_data/
+-rw-r--r--   0 toor      (1000) toor      (1000)       82 2024-03-26 10:01:36.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_and_export_data/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      160 2024-03-26 10:01:36.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_and_export_data/apps.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-24 07:06:14.247293 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_and_export_data/migrations/
+-rw-r--r--   0 toor      (1000) toor      (1000)     4714 2024-03-26 10:01:36.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_and_export_data/migrations/0001_initial.py
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-03-26 10:01:36.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_and_export_data/migrations/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2038 2024-03-29 11:36:54.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_and_export_data/models.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3546 2024-04-24 07:06:08.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_and_export_data/utils.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-24 07:06:14.248293 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-24 07:06:14.250293 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/base/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/base/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2170 2024-02-20 14:08:27.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/base/caches.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2998 2024-02-20 14:08:27.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/base/functions.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1017 2023-12-13 13:36:37.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/base/helpers.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6172 2024-02-20 14:08:27.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/base/managers.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     8521 2024-02-20 14:08:27.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/base/mixins.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1565 2024-03-14 19:45:32.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/base/runners.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-24 07:06:14.251293 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/calculated/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/calculated/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-24 07:06:14.254293 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/calculated/base/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/calculated/base/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2838 2024-02-20 14:08:27.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/calculated/base/caches.py
+-rw-r--r--   0 toor      (1000) toor      (1000)       84 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/calculated/base/consts.py
+-rw-r--r--   0 toor      (1000) toor      (1000)       93 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/calculated/base/enums.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      326 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/calculated/base/errors.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1670 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/calculated/base/functions.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1547 2023-12-13 13:36:37.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/calculated/base/helpers.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      838 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/calculated/base/managers.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      438 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/calculated/base/presenters.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      708 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/calculated/base/results.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1626 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/calculated/base/runners.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      181 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/calculated/base/strings.py
+-rw-r--r--   0 toor      (1000) toor      (1000)       59 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/calculated/base/tests.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1057 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/calculated/base/validators.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     7629 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/calculated/strategies.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    14543 2024-03-06 15:50:06.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/collect.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     9075 2024-03-06 15:50:06.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/generators.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2995 2024-03-18 08:19:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/helpers.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-24 07:06:14.255293 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/non_calculated/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/non_calculated/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-24 07:06:14.259293 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/non_calculated/base/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/non_calculated/base/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6589 2024-02-20 14:08:27.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/non_calculated/base/caches.py
+-rw-r--r--   0 toor      (1000) toor      (1000)       66 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/non_calculated/base/consts.py
+-rw-r--r--   0 toor      (1000) toor      (1000)       93 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/non_calculated/base/enums.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      297 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/non_calculated/base/errors.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1563 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/non_calculated/base/functions.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1433 2023-12-13 13:36:37.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/non_calculated/base/helpers.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      783 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/non_calculated/base/managers.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      409 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/non_calculated/base/presenters.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      674 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/non_calculated/base/results.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1519 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/non_calculated/base/runners.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      181 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/non_calculated/base/strings.py
+-rw-r--r--   0 toor      (1000) toor      (1000)       59 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/non_calculated/base/tests.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      973 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/non_calculated/base/validators.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     7431 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/non_calculated/strategies.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5367 2024-03-18 08:19:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/tests.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1104 2023-12-13 13:36:37.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/consts.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    14552 2024-04-24 07:06:08.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/entities.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-24 07:06:14.259293 edu-rdm-integration-3.1.0/src/edu_rdm_integration/enum_register/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/enum_register/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4021 2024-03-18 08:19:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/enum_register/mixins.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2218 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/enum_register/register.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4246 2024-03-26 10:01:36.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/enums.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-24 07:06:14.261293 edu-rdm-integration-3.1.0/src/edu_rdm_integration/export_data/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/export_data/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-24 07:06:14.264293 edu-rdm-integration-3.1.0/src/edu_rdm_integration/export_data/base/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/export_data/base/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1541 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/export_data/base/caches.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      519 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/export_data/base/consts.py
+-rw-r--r--   0 toor      (1000) toor      (1000)       93 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/export_data/base/enums.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      291 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/export_data/base/errors.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    12784 2024-04-24 07:06:08.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/export_data/base/functions.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4609 2024-04-03 12:03:40.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/export_data/base/helpers.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6075 2024-02-20 14:08:27.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/export_data/base/managers.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      403 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/export_data/base/presenters.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2576 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/export_data/base/requests.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      662 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/export_data/base/results.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2521 2024-02-20 14:08:27.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/export_data/base/runners.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      181 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/export_data/base/strings.py
+-rw-r--r--   0 toor      (1000) toor      (1000)       59 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/export_data/base/tests.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      961 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/export_data/base/validators.py
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/export_data/consts.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    17231 2024-03-07 13:08:27.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/export_data/export.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4020 2023-12-15 06:35:54.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/export_data/generators.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2933 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/export_data/helpers.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6725 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/export_data/strategies.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-24 07:06:14.265293 edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-24 07:06:14.269293 edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_collect_data_template/
+-rw-r--r--   0 toor      (1000) toor      (1000)      107 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_collect_data_template/__init__.py-tpl
+-rw-r--r--   0 toor      (1000) toor      (1000)      319 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_collect_data_template/apps.py-tpl
+-rw-r--r--   0 toor      (1000) toor      (1000)      963 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_collect_data_template/caches.py-tpl
+-rw-r--r--   0 toor      (1000) toor      (1000)       66 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_collect_data_template/consts.py-tpl
+-rw-r--r--   0 toor      (1000) toor      (1000)       93 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_collect_data_template/enums.py-tpl
+-rw-r--r--   0 toor      (1000) toor      (1000)      247 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_collect_data_template/errors.py-tpl
+-rw-r--r--   0 toor      (1000) toor      (1000)     5349 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_collect_data_template/functions.py-tpl
+-rw-r--r--   0 toor      (1000) toor      (1000)     1254 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_collect_data_template/helpers.py-tpl
+-rw-r--r--   0 toor      (1000) toor      (1000)     1731 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_collect_data_template/managers.py-tpl
+-rw-r--r--   0 toor      (1000) toor      (1000)      316 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_collect_data_template/presenters.py-tpl
+-rw-r--r--   0 toor      (1000) toor      (1000)      589 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_collect_data_template/results.py-tpl
+-rw-r--r--   0 toor      (1000) toor      (1000)     2937 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_collect_data_template/runners.py-tpl
+-rw-r--r--   0 toor      (1000) toor      (1000)      181 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_collect_data_template/strings.py-tpl
+-rw-r--r--   0 toor      (1000) toor      (1000)      838 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_collect_data_template/tests.py-tpl
+-rw-r--r--   0 toor      (1000) toor      (1000)      587 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_collect_data_template/validators.py-tpl
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-24 07:06:14.273293 edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_export_data_template/
+-rw-r--r--   0 toor      (1000) toor      (1000)      107 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_export_data_template/__init__.py-tpl
+-rw-r--r--   0 toor      (1000) toor      (1000)      319 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_export_data_template/apps.py-tpl
+-rw-r--r--   0 toor      (1000) toor      (1000)     1054 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_export_data_template/caches.py-tpl
+-rw-r--r--   0 toor      (1000) toor      (1000)       66 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_export_data_template/consts.py-tpl
+-rw-r--r--   0 toor      (1000) toor      (1000)       93 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_export_data_template/enums.py-tpl
+-rw-r--r--   0 toor      (1000) toor      (1000)      247 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_export_data_template/errors.py-tpl
+-rw-r--r--   0 toor      (1000) toor      (1000)     2882 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_export_data_template/functions.py-tpl
+-rw-r--r--   0 toor      (1000) toor      (1000)     1272 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_export_data_template/helpers.py-tpl
+-rw-r--r--   0 toor      (1000) toor      (1000)     2671 2023-12-07 10:11:59.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_export_data_template/managers.py-tpl
+-rw-r--r--   0 toor      (1000) toor      (1000)      316 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_export_data_template/presenters.py-tpl
+-rw-r--r--   0 toor      (1000) toor      (1000)      589 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_export_data_template/results.py-tpl
+-rw-r--r--   0 toor      (1000) toor      (1000)     3653 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_export_data_template/runners.py-tpl
+-rw-r--r--   0 toor      (1000) toor      (1000)      181 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_export_data_template/strings.py-tpl
+-rw-r--r--   0 toor      (1000) toor      (1000)       59 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_export_data_template/tests.py-tpl
+-rw-r--r--   0 toor      (1000) toor      (1000)      587 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_export_data_template/validators.py-tpl
+-rw-r--r--   0 toor      (1000) toor      (1000)    10997 2024-03-26 10:01:36.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/helpers.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-24 07:06:14.274293 edu-rdm-integration-3.1.0/src/edu_rdm_integration/management/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/management/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-24 07:06:14.276293 edu-rdm-integration-3.1.0/src/edu_rdm_integration/management/commands/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/management/commands/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3843 2024-01-11 11:42:02.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/management/commands/check_upload_status.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      750 2024-01-11 11:42:02.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/management/commands/collect_latest_models_data.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1022 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/management/commands/collect_models_data.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1211 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/management/commands/datamart_status.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1487 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/management/commands/datamart_upload.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      920 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/management/commands/export_entities_data.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1146 2024-01-11 11:42:02.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/management/commands/export_latest_entities_data.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    13439 2024-03-06 15:50:06.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/management/general.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      473 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/mapping.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-24 07:06:14.278293 edu-rdm-integration-3.1.0/src/edu_rdm_integration/migrations/
+-rw-r--r--   0 toor      (1000) toor      (1000)    18719 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/migrations/0001_initial.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      737 2023-12-08 11:59:51.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/migrations/0002_init_data_uploadstatus.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      735 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/migrations/0003_create_index_file_upload_status.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      626 2023-12-08 11:41:16.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/migrations/0004_uploaderclientlog.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1782 2023-12-08 11:59:51.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/migrations/0005_auto_20231204_1224.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3448 2023-12-08 11:59:51.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/migrations/0006_request_status_data.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      457 2023-12-08 11:59:51.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/migrations/0007_delete_upload_status.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1427 2024-01-15 06:45:08.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/migrations/0008_transferredentity.py
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/migrations/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    29327 2024-01-15 06:45:08.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/models.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-24 07:06:14.279293 edu-rdm-integration-3.1.0/src/edu_rdm_integration/registry/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-01-15 06:45:08.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/registry/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4146 2024-01-15 06:45:08.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/registry/actions.py
+-rw-r--r--   0 toor      (1000) toor      (1000)       73 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/signals.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6807 2023-12-04 16:17:35.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/storages.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    13716 2024-03-26 10:01:36.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/tasks.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-24 07:06:14.280293 edu-rdm-integration-3.1.0/src/edu_rdm_integration/uploader_log/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-12-08 11:41:16.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/uploader_log/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6755 2023-12-13 08:36:13.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/uploader_log/actions.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      265 2023-12-08 11:41:16.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/uploader_log/apps.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      266 2023-12-08 11:41:16.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/uploader_log/enums.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3203 2023-12-11 20:05:53.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/uploader_log/managers.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2110 2023-12-13 08:36:13.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/uploader_log/ui.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    10369 2024-03-26 10:01:36.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration/utils.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-24 07:06:14.280293 edu-rdm-integration-3.1.0/src/edu_rdm_integration.egg-info/
+-rw-r--r--   0 toor      (1000) toor      (1000)    61600 2024-04-24 07:06:14.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration.egg-info/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)    10685 2024-04-24 07:06:14.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration.egg-info/SOURCES.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2024-04-24 07:06:14.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration.egg-info/dependency_links.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2024-04-24 07:06:14.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration.egg-info/namespace_packages.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-12-04 16:17:43.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration.egg-info/not-zip-safe
+-rw-r--r--   0 toor      (1000) toor      (1000)      253 2024-04-24 07:06:14.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration.egg-info/requires.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       20 2024-04-24 07:06:14.000000 edu-rdm-integration-3.1.0/src/edu_rdm_integration.egg-info/top_level.txt
```

### Comparing `edu-rdm-integration-3.0.4/CHANGELOG.md` & `edu-rdm-integration-3.1.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,23 @@
 ### Изменено
 
 ### Исправлено
 
 ### Удалено
 
 
+## 3.1.0 - 2024-04-23
+Добавлена поддержка setuptools 69.*.
+Поднята минимальная версия пакета pip 23.2.1
+
+### Изменено
+- [EDUSCHL-21761](https://jira.bars.group/browse/EDUSCHL-21761)
+  MINOR Добавлена поддержка setuptools 69.*. Поднять минимальную версию pip до 23.2.1.
+
+
 ## 3.0.4 - 2024-04-17
 Возвращено проставление подэтапа выгрузки всем записям модели.
 
 ### Изменено
 - [EDUSCHL-21761](https://jira.bars.group/browse/EDUSCHL-21761)
   PATCH Возвращено проставление подэтапа выгрузки всем записям модели.
```

### Comparing `edu-rdm-integration-3.0.4/CONDUCT.md` & `edu-rdm-integration-3.1.0/CONDUCT.md`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/LICENSE` & `edu-rdm-integration-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/PKG-INFO` & `edu-rdm-integration-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edu-rdm-integration
-Version: 3.0.4
+Version: 3.1.0
 Summary: Интеграция с Региональной витриной данных
 Home-page: 
 Download-URL: 
 Author: BARS Group
 Author-email: bars@bars.group
 Platform: Any
 Classifier: Development Status :: 3 - Alpha
@@ -18,16 +18,16 @@
 Classifier: Environment :: Console
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: packaging<24,>=21.3
-Requires-Dist: pip<24,>=20.1.1
-Requires-Dist: setuptools<69,>=47.3.1
+Requires-Dist: pip<24,>=23.2.1
+Requires-Dist: setuptools<70,>=47.3.1
 Requires-Dist: wheel<0.42,>=0.37.1
 Requires-Dist: transliterate<2
 Requires-Dist: Django<3.2,>=2.2
 Requires-Dist: celery<5.3,>=4.4.7
 Requires-Dist: educommon<4,>=3.9.3
 Requires-Dist: function-tools<1,>=0.9.0
 Requires-Dist: m3-db-utils<1,>=0.3.10
@@ -290,14 +290,23 @@
 ### Изменено
 
 ### Исправлено
 
 ### Удалено
 
 
+## 3.1.0 - 2024-04-23
+Добавлена поддержка setuptools 69.*.
+Поднята минимальная версия пакета pip 23.2.1
+
+### Изменено
+- [EDUSCHL-21761](https://jira.bars.group/browse/EDUSCHL-21761)
+  MINOR Добавлена поддержка setuptools 69.*. Поднять минимальную версию pip до 23.2.1.
+
+
 ## 3.0.4 - 2024-04-17
 Возвращено проставление подэтапа выгрузки всем записям модели.
 
 ### Изменено
 - [EDUSCHL-21761](https://jira.bars.group/browse/EDUSCHL-21761)
   PATCH Возвращено проставление подэтапа выгрузки всем записям модели.
```

### Comparing `edu-rdm-integration-3.0.4/README.md` & `edu-rdm-integration-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/setup.py` & `edu-rdm-integration-3.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     find_packages,
     setup,
 )
 
 
 PROJECT = 'edu_rdm_integration'
 
-VERSION = '3.0.4'
+VERSION = '3.1.0'
 
 current_dir_path = Path().resolve()
 
 
 #  Получение полного описания
 with open(str(current_dir_path / 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
```

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/adapters/caches.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/adapters/caches.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/adapters/functions.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/adapters/functions.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/adapters/helpers.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/adapters/helpers.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/adapters/managers.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/adapters/managers.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/adapters/receivers.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/adapters/receivers.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/adapters/results.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/adapters/results.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/adapters/runners.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/adapters/runners.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/adapters/strategies.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/adapters/strategies.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/app_settings.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/app_settings.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/apps.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/apps.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/base.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/base.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_and_export_data/migrations/0001_initial.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_and_export_data/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_and_export_data/models.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_and_export_data/models.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_and_export_data/utils.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_and_export_data/utils.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/base/caches.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/base/caches.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/base/functions.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/base/functions.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/base/helpers.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/base/helpers.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/base/managers.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/base/managers.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/base/mixins.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/base/mixins.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/base/runners.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/base/runners.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/calculated/base/caches.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/calculated/base/caches.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/calculated/base/functions.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/calculated/base/functions.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/calculated/base/helpers.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/calculated/base/helpers.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/calculated/base/managers.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/calculated/base/managers.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/calculated/base/results.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/calculated/base/results.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/calculated/base/runners.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/calculated/base/runners.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/calculated/base/validators.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/calculated/base/validators.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/calculated/strategies.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/calculated/strategies.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/collect.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/collect.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/generators.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/generators.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/helpers.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/helpers.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/non_calculated/base/caches.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/non_calculated/base/caches.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/non_calculated/base/functions.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/non_calculated/base/functions.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/non_calculated/base/helpers.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/non_calculated/base/helpers.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/non_calculated/base/managers.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/non_calculated/base/managers.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/non_calculated/base/results.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/non_calculated/base/results.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/non_calculated/base/runners.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/non_calculated/base/runners.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/non_calculated/base/validators.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/non_calculated/base/validators.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/non_calculated/strategies.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/non_calculated/strategies.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/collect_data/tests.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/collect_data/tests.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/consts.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/consts.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/entities.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/entities.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/enum_register/mixins.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/enum_register/mixins.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/enum_register/register.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/enum_register/register.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/enums.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/enums.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/export_data/base/caches.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/export_data/base/caches.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/export_data/base/consts.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/export_data/base/consts.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/export_data/base/functions.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/export_data/base/functions.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/export_data/base/helpers.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/export_data/base/helpers.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/export_data/base/managers.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/export_data/base/managers.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/export_data/base/requests.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/export_data/base/requests.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/export_data/base/results.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/export_data/base/results.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/export_data/base/runners.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/export_data/base/runners.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/export_data/base/validators.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/export_data/base/validators.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/export_data/export.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/export_data/export.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/export_data/generators.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/export_data/generators.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/export_data/helpers.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/export_data/helpers.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/export_data/strategies.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/export_data/strategies.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_collect_data_template/caches.py-tpl` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_collect_data_template/caches.py-tpl`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_collect_data_template/functions.py-tpl` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_collect_data_template/functions.py-tpl`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_collect_data_template/helpers.py-tpl` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_collect_data_template/helpers.py-tpl`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_collect_data_template/managers.py-tpl` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_collect_data_template/managers.py-tpl`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_collect_data_template/results.py-tpl` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_collect_data_template/results.py-tpl`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_collect_data_template/runners.py-tpl` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_collect_data_template/runners.py-tpl`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_collect_data_template/tests.py-tpl` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_collect_data_template/tests.py-tpl`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_collect_data_template/validators.py-tpl` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_collect_data_template/validators.py-tpl`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_export_data_template/caches.py-tpl` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_export_data_template/caches.py-tpl`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_export_data_template/functions.py-tpl` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_export_data_template/functions.py-tpl`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_export_data_template/helpers.py-tpl` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_export_data_template/helpers.py-tpl`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_export_data_template/managers.py-tpl` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_export_data_template/managers.py-tpl`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_export_data_template/results.py-tpl` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_export_data_template/results.py-tpl`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_export_data_template/runners.py-tpl` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_export_data_template/runners.py-tpl`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/function_templates/function_export_data_template/validators.py-tpl` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/function_templates/function_export_data_template/validators.py-tpl`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/helpers.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/helpers.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/management/commands/check_upload_status.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/management/commands/check_upload_status.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/management/commands/collect_latest_models_data.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/management/commands/collect_latest_models_data.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/management/commands/collect_models_data.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/management/commands/collect_models_data.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/management/commands/datamart_status.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/management/commands/datamart_status.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/management/commands/datamart_upload.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/management/commands/datamart_upload.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/management/commands/export_entities_data.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/management/commands/export_entities_data.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/management/commands/export_latest_entities_data.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/management/commands/export_latest_entities_data.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/management/general.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/management/general.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/migrations/0001_initial.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/migrations/0002_init_data_uploadstatus.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/migrations/0002_init_data_uploadstatus.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/migrations/0003_create_index_file_upload_status.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/migrations/0003_create_index_file_upload_status.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/migrations/0004_uploaderclientlog.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/migrations/0004_uploaderclientlog.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/migrations/0005_auto_20231204_1224.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/migrations/0005_auto_20231204_1224.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/migrations/0006_request_status_data.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/migrations/0006_request_status_data.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/migrations/0008_transferredentity.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/migrations/0008_transferredentity.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/models.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/models.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/registry/actions.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/registry/actions.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/storages.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/storages.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/tasks.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/tasks.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/uploader_log/actions.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/uploader_log/actions.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/uploader_log/managers.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/uploader_log/managers.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/uploader_log/ui.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/uploader_log/ui.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration/utils.py` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration/utils.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration.egg-info/PKG-INFO` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edu-rdm-integration
-Version: 3.0.4
+Version: 3.1.0
 Summary: Интеграция с Региональной витриной данных
 Home-page: 
 Download-URL: 
 Author: BARS Group
 Author-email: bars@bars.group
 Platform: Any
 Classifier: Development Status :: 3 - Alpha
@@ -18,16 +18,16 @@
 Classifier: Environment :: Console
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: packaging<24,>=21.3
-Requires-Dist: pip<24,>=20.1.1
-Requires-Dist: setuptools<69,>=47.3.1
+Requires-Dist: pip<24,>=23.2.1
+Requires-Dist: setuptools<70,>=47.3.1
 Requires-Dist: wheel<0.42,>=0.37.1
 Requires-Dist: transliterate<2
 Requires-Dist: Django<3.2,>=2.2
 Requires-Dist: celery<5.3,>=4.4.7
 Requires-Dist: educommon<4,>=3.9.3
 Requires-Dist: function-tools<1,>=0.9.0
 Requires-Dist: m3-db-utils<1,>=0.3.10
@@ -290,14 +290,23 @@
 ### Изменено
 
 ### Исправлено
 
 ### Удалено
 
 
+## 3.1.0 - 2024-04-23
+Добавлена поддержка setuptools 69.*.
+Поднята минимальная версия пакета pip 23.2.1
+
+### Изменено
+- [EDUSCHL-21761](https://jira.bars.group/browse/EDUSCHL-21761)
+  MINOR Добавлена поддержка setuptools 69.*. Поднять минимальную версию pip до 23.2.1.
+
+
 ## 3.0.4 - 2024-04-17
 Возвращено проставление подэтапа выгрузки всем записям модели.
 
 ### Изменено
 - [EDUSCHL-21761](https://jira.bars.group/browse/EDUSCHL-21761)
   PATCH Возвращено проставление подэтапа выгрузки всем записям модели.
```

### Comparing `edu-rdm-integration-3.0.4/src/edu_rdm_integration.egg-info/SOURCES.txt` & `edu-rdm-integration-3.1.0/src/edu_rdm_integration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

