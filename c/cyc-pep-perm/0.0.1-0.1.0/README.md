# Comparing `tmp/cyc_pep_perm-0.0.1.tar.gz` & `tmp/cyc_pep_perm-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyc_pep_perm-0.0.1.tar", last modified: Tue Mar 26 15:58:43 2024, max compression
+gzip compressed data, was "cyc_pep_perm-0.1.0.tar", last modified: Wed Apr 24 12:35:47 2024, max compression
```

## Comparing `cyc_pep_perm-0.0.1.tar` & `cyc_pep_perm-0.1.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxr-x   0 rebecca   (1003) rebecca   (1003)        0 2024-03-26 15:58:43.610450 cyc_pep_perm-0.0.1/
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)     1073 2023-12-09 14:12:58.000000 cyc_pep_perm-0.0.1/LICENSE
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)      616 2024-01-04 14:43:34.000000 cyc_pep_perm-0.0.1/MANIFEST.in
--rw-r--r--   0 rebecca   (1003) rebecca   (1003)    11144 2024-03-26 15:58:43.610450 cyc_pep_perm-0.0.1/PKG-INFO
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)    20837 2023-12-09 14:12:58.000000 cyc_pep_perm-0.0.1/README.html
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)     9100 2024-03-26 15:57:58.000000 cyc_pep_perm-0.0.1/README.md
-drwxrwxr-x   0 rebecca   (1003) rebecca   (1003)        0 2024-03-26 15:58:43.590450 cyc_pep_perm-0.0.1/data/
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)     5070 2024-01-24 15:18:32.000000 cyc_pep_perm-0.0.1/data/perm_random20_test_dw.csv
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)   585387 2024-01-24 15:18:53.000000 cyc_pep_perm-0.0.1/data/perm_random20_test_mordred.csv
--rw-r--r--   0 rebecca   (1003) rebecca   (1003)     8414 2023-12-13 00:59:49.000000 cyc_pep_perm-0.0.1/data/perm_random20_test_raw.ods
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)    20845 2024-01-23 21:22:59.000000 cyc_pep_perm-0.0.1/data/perm_random80_train_dw.csv
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)  2335501 2023-12-09 14:12:58.000000 cyc_pep_perm-0.0.1/data/perm_random80_train_mordred.csv
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)    21935 2023-12-09 14:12:58.000000 cyc_pep_perm-0.0.1/data/perm_random80_train_raw.ods
-drwxrwxr-x   0 rebecca   (1003) rebecca   (1003)        0 2024-03-26 15:58:43.586450 cyc_pep_perm-0.0.1/docs/
-drwxrwxr-x   0 rebecca   (1003) rebecca   (1003)        0 2024-03-26 15:58:43.590450 cyc_pep_perm-0.0.1/docs/source/
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)      241 2023-12-09 14:12:58.000000 cyc_pep_perm-0.0.1/docs/source/cli.rst
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)     7283 2023-12-09 14:12:58.000000 cyc_pep_perm-0.0.1/docs/source/conf.py
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)     1815 2023-12-09 14:12:58.000000 cyc_pep_perm-0.0.1/docs/source/index.rst
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)      539 2023-12-09 14:12:58.000000 cyc_pep_perm-0.0.1/docs/source/installation.rst
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)       59 2023-12-09 14:12:58.000000 cyc_pep_perm-0.0.1/docs/source/usage.rst
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)      368 2024-03-12 15:02:27.000000 cyc_pep_perm-0.0.1/environment.yml
-drwxrwxr-x   0 rebecca   (1003) rebecca   (1003)        0 2024-03-26 15:58:43.602450 cyc_pep_perm-0.0.1/models/
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)  4448640 2023-12-13 00:48:39.000000 cyc_pep_perm-0.0.1/models/rf_random_dw.pkl
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)  3783213 2023-12-13 00:50:09.000000 cyc_pep_perm-0.0.1/models/rf_random_mordred.pkl
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)   297070 2023-12-13 00:53:52.000000 cyc_pep_perm-0.0.1/models/xgb_random_dw.pkl
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)   183073 2023-12-21 23:30:09.000000 cyc_pep_perm-0.0.1/models/xgb_random_mordred.pkl
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)    58332 2024-01-24 15:19:18.000000 cyc_pep_perm-0.0.1/playground.ipynb
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)      359 2023-12-09 14:12:58.000000 cyc_pep_perm-0.0.1/pyproject.toml
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)     4436 2024-01-25 19:11:51.000000 cyc_pep_perm-0.0.1/requirements.txt
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)     2265 2024-03-26 15:58:43.610450 cyc_pep_perm-0.0.1/setup.cfg
-drwxrwxr-x   0 rebecca   (1003) rebecca   (1003)        0 2024-03-26 15:58:43.586450 cyc_pep_perm-0.0.1/src/
-drwxrwxr-x   0 rebecca   (1003) rebecca   (1003)        0 2024-03-26 15:58:43.602450 cyc_pep_perm-0.0.1/src/cyc_pep_perm/
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)      185 2024-03-12 14:12:20.000000 cyc_pep_perm-0.0.1/src/cyc_pep_perm/__init__.py
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)      329 2023-12-09 14:12:58.000000 cyc_pep_perm-0.0.1/src/cyc_pep_perm/__main__.py
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)       42 2023-12-09 14:12:58.000000 cyc_pep_perm-0.0.1/src/cyc_pep_perm/api.py
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)      889 2023-12-09 14:12:58.000000 cyc_pep_perm-0.0.1/src/cyc_pep_perm/cli.py
-drwxrwxr-x   0 rebecca   (1003) rebecca   (1003)        0 2024-03-26 15:58:43.602450 cyc_pep_perm-0.0.1/src/cyc_pep_perm/data/
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)      450 2024-03-12 14:18:44.000000 cyc_pep_perm-0.0.1/src/cyc_pep_perm/data/__init__.py
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)    17789 2024-01-04 15:15:09.000000 cyc_pep_perm-0.0.1/src/cyc_pep_perm/data/descriptors.py
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)      895 2024-03-12 14:26:27.000000 cyc_pep_perm-0.0.1/src/cyc_pep_perm/data/paths.py
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)     8990 2024-03-12 14:43:31.000000 cyc_pep_perm-0.0.1/src/cyc_pep_perm/data/processing.py
-drwxrwxr-x   0 rebecca   (1003) rebecca   (1003)        0 2024-03-26 15:58:43.602450 cyc_pep_perm-0.0.1/src/cyc_pep_perm/models/
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)      133 2024-03-12 14:15:12.000000 cyc_pep_perm-0.0.1/src/cyc_pep_perm/models/__init__.py
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)     7914 2024-03-26 15:10:35.000000 cyc_pep_perm-0.0.1/src/cyc_pep_perm/models/randomforest.py
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)     8045 2024-03-26 15:21:45.000000 cyc_pep_perm-0.0.1/src/cyc_pep_perm/models/randomforest_class.py
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)     7731 2024-03-26 15:20:22.000000 cyc_pep_perm-0.0.1/src/cyc_pep_perm/models/xgboost.py
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)        1 2023-12-09 14:12:58.000000 cyc_pep_perm-0.0.1/src/cyc_pep_perm/py.typed
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)     1024 2023-12-09 14:12:58.000000 cyc_pep_perm-0.0.1/src/cyc_pep_perm/version.py
-drwxrwxr-x   0 rebecca   (1003) rebecca   (1003)        0 2024-03-26 15:58:43.610450 cyc_pep_perm-0.0.1/src/cyc_pep_perm.egg-info/
--rw-r--r--   0 rebecca   (1003) rebecca   (1003)    11144 2024-03-26 15:58:43.000000 cyc_pep_perm-0.0.1/src/cyc_pep_perm.egg-info/PKG-INFO
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)     1419 2024-03-26 15:58:43.000000 cyc_pep_perm-0.0.1/src/cyc_pep_perm.egg-info/SOURCES.txt
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)        1 2024-03-26 15:58:43.000000 cyc_pep_perm-0.0.1/src/cyc_pep_perm.egg-info/dependency_links.txt
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)       55 2024-03-26 15:58:43.000000 cyc_pep_perm-0.0.1/src/cyc_pep_perm.egg-info/entry_points.txt
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)        1 2023-12-10 14:16:37.000000 cyc_pep_perm-0.0.1/src/cyc_pep_perm.egg-info/not-zip-safe
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)      211 2024-03-26 15:58:43.000000 cyc_pep_perm-0.0.1/src/cyc_pep_perm.egg-info/requires.txt
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)       13 2024-03-26 15:58:43.000000 cyc_pep_perm-0.0.1/src/cyc_pep_perm.egg-info/top_level.txt
-drwxrwxr-x   0 rebecca   (1003) rebecca   (1003)        0 2024-03-26 15:58:43.602450 cyc_pep_perm-0.0.1/tests/
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)       62 2024-03-26 15:15:17.000000 cyc_pep_perm-0.0.1/tests/__init__.py
-drwxrwxr-x   0 rebecca   (1003) rebecca   (1003)        0 2024-03-26 15:58:43.606450 cyc_pep_perm-0.0.1/tests/test_models/
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)  3573620 2024-01-04 14:25:49.000000 cyc_pep_perm-0.0.1/tests/test_models/rf_random_dw_unittest.pkl
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)   419657 2024-03-26 15:15:08.000000 cyc_pep_perm-0.0.1/tests/test_models/rf_unittest.pkl
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)     5836 2024-03-26 15:12:56.000000 cyc_pep_perm-0.0.1/tests/test_randomforest.py
--rw-rw-r--   0 rebecca   (1003) rebecca   (1003)      406 2024-03-12 15:00:40.000000 cyc_pep_perm-0.0.1/tests/test_version.py
+drwxrwxr-x   0 rebecca   (1003) rebecca   (1003)        0 2024-04-24 12:35:47.268289 cyc_pep_perm-0.1.0/
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)     1073 2023-12-09 14:12:58.000000 cyc_pep_perm-0.1.0/LICENSE
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)      616 2024-01-04 14:43:34.000000 cyc_pep_perm-0.1.0/MANIFEST.in
+-rw-r--r--   0 rebecca   (1003) rebecca   (1003)    12161 2024-04-24 12:35:47.268289 cyc_pep_perm-0.1.0/PKG-INFO
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)    20837 2023-12-09 14:12:58.000000 cyc_pep_perm-0.1.0/README.html
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)    10117 2024-04-24 12:12:39.000000 cyc_pep_perm-0.1.0/README.md
+drwxrwxr-x   0 rebecca   (1003) rebecca   (1003)        0 2024-04-24 12:35:47.248289 cyc_pep_perm-0.1.0/data/
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)     5070 2024-01-24 15:18:32.000000 cyc_pep_perm-0.1.0/data/perm_random20_test_dw.csv
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)   585387 2024-01-24 15:18:53.000000 cyc_pep_perm-0.1.0/data/perm_random20_test_mordred.csv
+-rw-r--r--   0 rebecca   (1003) rebecca   (1003)     8414 2023-12-13 00:59:49.000000 cyc_pep_perm-0.1.0/data/perm_random20_test_raw.ods
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)    20845 2024-01-23 21:22:59.000000 cyc_pep_perm-0.1.0/data/perm_random80_train_dw.csv
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)  2335501 2023-12-09 14:12:58.000000 cyc_pep_perm-0.1.0/data/perm_random80_train_mordred.csv
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)    21935 2023-12-09 14:12:58.000000 cyc_pep_perm-0.1.0/data/perm_random80_train_raw.ods
+drwxrwxr-x   0 rebecca   (1003) rebecca   (1003)        0 2024-04-24 12:35:47.244289 cyc_pep_perm-0.1.0/docs/
+drwxrwxr-x   0 rebecca   (1003) rebecca   (1003)        0 2024-04-24 12:35:47.252289 cyc_pep_perm-0.1.0/docs/source/
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)      241 2023-12-09 14:12:58.000000 cyc_pep_perm-0.1.0/docs/source/cli.rst
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)     7279 2024-04-24 12:17:07.000000 cyc_pep_perm-0.1.0/docs/source/conf.py
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)     1815 2023-12-09 14:12:58.000000 cyc_pep_perm-0.1.0/docs/source/index.rst
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)      539 2023-12-09 14:12:58.000000 cyc_pep_perm-0.1.0/docs/source/installation.rst
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)       59 2023-12-09 14:12:58.000000 cyc_pep_perm-0.1.0/docs/source/usage.rst
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)      368 2024-03-12 15:02:27.000000 cyc_pep_perm-0.1.0/environment.yml
+drwxrwxr-x   0 rebecca   (1003) rebecca   (1003)        0 2024-04-24 12:35:47.260289 cyc_pep_perm-0.1.0/models/
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)  4448640 2023-12-13 00:48:39.000000 cyc_pep_perm-0.1.0/models/rf_random_dw.pkl
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)  3783213 2023-12-13 00:50:09.000000 cyc_pep_perm-0.1.0/models/rf_random_mordred.pkl
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)   297070 2023-12-13 00:53:52.000000 cyc_pep_perm-0.1.0/models/xgb_random_dw.pkl
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)   183073 2023-12-21 23:30:09.000000 cyc_pep_perm-0.1.0/models/xgb_random_mordred.pkl
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)    58332 2024-01-24 15:19:18.000000 cyc_pep_perm-0.1.0/playground.ipynb
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)      359 2023-12-09 14:12:58.000000 cyc_pep_perm-0.1.0/pyproject.toml
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)     4436 2024-04-24 12:09:52.000000 cyc_pep_perm-0.1.0/requirements.txt
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)     2265 2024-04-24 12:35:47.268289 cyc_pep_perm-0.1.0/setup.cfg
+drwxrwxr-x   0 rebecca   (1003) rebecca   (1003)        0 2024-04-24 12:35:47.244289 cyc_pep_perm-0.1.0/src/
+drwxrwxr-x   0 rebecca   (1003) rebecca   (1003)        0 2024-04-24 12:35:47.260289 cyc_pep_perm-0.1.0/src/cyc_pep_perm/
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)      185 2024-03-12 14:12:20.000000 cyc_pep_perm-0.1.0/src/cyc_pep_perm/__init__.py
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)      329 2023-12-09 14:12:58.000000 cyc_pep_perm-0.1.0/src/cyc_pep_perm/__main__.py
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)       42 2023-12-09 14:12:58.000000 cyc_pep_perm-0.1.0/src/cyc_pep_perm/api.py
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)      889 2023-12-09 14:12:58.000000 cyc_pep_perm-0.1.0/src/cyc_pep_perm/cli.py
+drwxrwxr-x   0 rebecca   (1003) rebecca   (1003)        0 2024-04-24 12:35:47.260289 cyc_pep_perm-0.1.0/src/cyc_pep_perm/data/
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)      450 2024-03-12 14:18:44.000000 cyc_pep_perm-0.1.0/src/cyc_pep_perm/data/__init__.py
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)    17789 2024-01-04 15:15:09.000000 cyc_pep_perm-0.1.0/src/cyc_pep_perm/data/descriptors.py
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)      896 2024-04-24 12:30:58.000000 cyc_pep_perm-0.1.0/src/cyc_pep_perm/data/paths.py
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)     9209 2024-04-24 11:22:01.000000 cyc_pep_perm-0.1.0/src/cyc_pep_perm/data/processing.py
+drwxrwxr-x   0 rebecca   (1003) rebecca   (1003)        0 2024-04-24 12:35:47.264289 cyc_pep_perm-0.1.0/src/cyc_pep_perm/models/
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)      133 2024-03-12 14:15:12.000000 cyc_pep_perm-0.1.0/src/cyc_pep_perm/models/__init__.py
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)     7848 2024-04-24 11:17:35.000000 cyc_pep_perm-0.1.0/src/cyc_pep_perm/models/randomforest.py
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)     7964 2024-04-24 10:10:23.000000 cyc_pep_perm-0.1.0/src/cyc_pep_perm/models/randomforest_class.py
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)     7662 2024-04-24 10:10:23.000000 cyc_pep_perm-0.1.0/src/cyc_pep_perm/models/xgboost.py
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)        1 2023-12-09 14:12:58.000000 cyc_pep_perm-0.1.0/src/cyc_pep_perm/py.typed
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)     1024 2024-04-24 12:17:17.000000 cyc_pep_perm-0.1.0/src/cyc_pep_perm/version.py
+drwxrwxr-x   0 rebecca   (1003) rebecca   (1003)        0 2024-04-24 12:35:47.268289 cyc_pep_perm-0.1.0/src/cyc_pep_perm.egg-info/
+-rw-r--r--   0 rebecca   (1003) rebecca   (1003)    12161 2024-04-24 12:35:47.000000 cyc_pep_perm-0.1.0/src/cyc_pep_perm.egg-info/PKG-INFO
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)     1419 2024-04-24 12:35:47.000000 cyc_pep_perm-0.1.0/src/cyc_pep_perm.egg-info/SOURCES.txt
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)        1 2024-04-24 12:35:47.000000 cyc_pep_perm-0.1.0/src/cyc_pep_perm.egg-info/dependency_links.txt
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)       55 2024-04-24 12:35:47.000000 cyc_pep_perm-0.1.0/src/cyc_pep_perm.egg-info/entry_points.txt
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)        1 2023-12-10 14:16:37.000000 cyc_pep_perm-0.1.0/src/cyc_pep_perm.egg-info/not-zip-safe
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)      211 2024-04-24 12:35:47.000000 cyc_pep_perm-0.1.0/src/cyc_pep_perm.egg-info/requires.txt
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)       13 2024-04-24 12:35:47.000000 cyc_pep_perm-0.1.0/src/cyc_pep_perm.egg-info/top_level.txt
+drwxrwxr-x   0 rebecca   (1003) rebecca   (1003)        0 2024-04-24 12:35:47.264289 cyc_pep_perm-0.1.0/tests/
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)       62 2024-03-26 15:15:17.000000 cyc_pep_perm-0.1.0/tests/__init__.py
+drwxrwxr-x   0 rebecca   (1003) rebecca   (1003)        0 2024-04-24 12:35:47.268289 cyc_pep_perm-0.1.0/tests/test_models/
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)  3573620 2024-01-04 14:25:49.000000 cyc_pep_perm-0.1.0/tests/test_models/rf_random_dw_unittest.pkl
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)    84683 2024-04-24 12:32:25.000000 cyc_pep_perm-0.1.0/tests/test_models/rf_unittest.pkl
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)     5836 2024-03-26 15:12:56.000000 cyc_pep_perm-0.1.0/tests/test_randomforest.py
+-rw-rw-r--   0 rebecca   (1003) rebecca   (1003)      406 2024-03-12 15:00:40.000000 cyc_pep_perm-0.1.0/tests/test_version.py
```

### Comparing `cyc_pep_perm-0.0.1/LICENSE` & `cyc_pep_perm-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cyc_pep_perm-0.0.1/MANIFEST.in` & `cyc_pep_perm-0.1.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `cyc_pep_perm-0.0.1/PKG-INFO` & `cyc_pep_perm-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyc_pep_perm
-Version: 0.0.1
+Version: 0.1.0
 Summary: Python package to predict membrane permeability of cyclic peptides.
 Home-page: https://github.com/schwallergroup/CycPepPerm
 Download-URL: https://github.com/schwallergroup/CycPepPerm/releases
 Author: Rebecca M Neeser
 Author-email: rebecca.neeser@epfl.ch
 Maintainer: Rebecca M Neeser
 Maintainer-email: rebecca.neeser@epfl.ch
@@ -78,19 +78,20 @@
 
 <br>
 
 Python package to predict membrane permeability of cyclic peptides.
 
 ## 👩‍💻 Installation
 
-We provide the code as a python package, so the only thing you need is to install it. We recommend creating a new conda environment for that (otherwise skip first line.
+We provide the code as a [python package](https://pypi.org/project/cyc-pep-perm/), so the only thing you need is to install it. We recommend creating a new conda environment for that, which allows simple package management for a project. Follow these [instructions](https://docs.anaconda.com/free/anaconda/install/index.html) to install Anaconda. However, the package containing our code can also be installed without creating a project-specific environment. In that case, one just skips the first two lines of the following code:
 
 ```bash
 $ conda create -n cyc-pep-perm python=3.10
-$ pip install cyc_pep_perm
+$ conda activate cyc-pep-perm
+$ pip install cyc-pep-perm==0.1.0
 ```
 
 ### 🛠️ For Developers
 <details>
   <summary>See detailed installation instructions</summary>
 The repository can be cloned from GitHub and installed with `pip` or `conda`. The code was built with Python 3.10 on Linux but other OS should work as well.
 
@@ -133,26 +134,29 @@
 ```
 </details>
 
 ## 🔥 Usage
 
 > For some more examples on how to process data, train and evaluate the alogrithms, please consult the folder `notebooks/`. This folder also contains a notebook to perform polynomial fits as described in the paper.
 
+All data paths in the following examples are taken from the hard-coded paths that work when one clones this repository. If you use the python package and download the data separately, please change the paths accordingly.
+
 ### Data preprocessing
 
-Here we showcase how to handle the data as for our use-case. Some simple reformating is done (see also the notebook `notebooks/01_data_preparation.ipynb`) starting from `.ods` file with DataWarrior output.
+Here we showcase how to handle the data as for our use-case. Some simple reformating is done (see also the notebook `notebooks/01_data_preparation.ipynb`) starting from `.ods` file with DataWarrior output (for data see [Data and Models](#data-and-models)).
 
 ```python
 import os
 
-from cyc_pep_perm.data.paths import DATA_PATH
 from cyc_pep_perm.data.processing import DataProcessing
 
+data_dir = "/path/to/data/folder" # ADAPT TO YOUR PATH!
+
 # this can also be a .csv input
-datapath = os.path.join(DATA_PATH, "perm_random80_train_raw.ods")
+datapath = os.path.join(data_dir, "perm_random80_train_raw.ods")
 
 # instantiate the class and make sure the columns match your inputed file - otherwise change arguments
 dp = DataProcessing(datapath=datapath)
 
 # make use of precomputed descriptors from DataWarrior
 df = dp.read_data(filename="perm_random80_train_dw.csv")
 
@@ -161,46 +165,59 @@
 ```
 
 ### Training
 
 Make sure to have the data ready to be used. In order to make the hyperparameter search more extensive, please look into the respective python scripts (e.g. `src/cyc_pep_perm/models/randomforest.py`) and adjust the `PARAMS` dictionary.
 
 ```python
+import os
+
 from cyc_pep_perm.models.randomforest import RF
-from cyc_pep_perm.data.paths import TRAIN_RANDOM_DW
+
+data_dir = "/path/to/data/folder" # ADAPT TO YOUR PATH!
+train_data = os.path.join(data_dir, "perm_random80_train_dw.csv")
+model_dir = "/path/to/model/folder" # ADAPT TO YOUR PATH!
+rf_model_trained = os.path.join(model_dir, "rf_random_dw.pkl")
 
 # instantiate class
 rf_regressor = RF()
 
 model = rf_regressor.train(
-    datapath = TRAIN_RANDOM_DW, # path to provided data from paper
+    datapath = train_data,
+    savepath = rf_model_trained,
 )
 
 y_pred, rmse, r2 = rf_regressor.evaluate()
 # will print training results, e.g.:
 >>> RMSE: 8.45
 >>> R2: 0.879
 ```
 
 ### Prediction
 
 ```python
+import os
+
 from cyc_pep_perm.models.randomforest import RF
-from cyc_pep_perm.data.paths import MODEL_RF_RANDOM_DW, TRAIN_RANDOM_DW
+
+data_dir = "/path/to/data/folder" # ADAPT TO YOUR PATH!
+train_data = os.path.join(data_dir, "perm_random80_train_dw.csv")
+model_dir = "/path/to/model/folder" # ADAPT TO YOUR PATH!
+rf_model_trained = os.path.join(model_dir, "rf_random_dw.pkl")
 
 # instantiate class
 rf_regressor = RF()
 
 # load trained model
 rf_regressor.load_model(
-    model_path = MODEL_RF_RANDOM_DW, # path to provided model from paper
+    modelpath = rf_model_trained,
 )
 
 # data to predict on, e.g.:
-df = pd.read_csv(TRAIN_RANDOM_DW)
+df = pd.read_csv(train_data)
 X = df.drop(columns=["SMILES"])
 
 # predict
 y_pred = rf_regressor.predict(X)
 ```
 
 ## Data and Models
```

### Comparing `cyc_pep_perm-0.0.1/README.html` & `cyc_pep_perm-0.1.0/README.html`

 * *Files identical despite different names*

### Comparing `cyc_pep_perm-0.0.1/README.md` & `cyc_pep_perm-0.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -23,19 +23,20 @@
 
 <br>
 
 Python package to predict membrane permeability of cyclic peptides.
 
 ## 👩‍💻 Installation
 
-We provide the code as a python package, so the only thing you need is to install it. We recommend creating a new conda environment for that (otherwise skip first line.
+We provide the code as a [python package](https://pypi.org/project/cyc-pep-perm/), so the only thing you need is to install it. We recommend creating a new conda environment for that, which allows simple package management for a project. Follow these [instructions](https://docs.anaconda.com/free/anaconda/install/index.html) to install Anaconda. However, the package containing our code can also be installed without creating a project-specific environment. In that case, one just skips the first two lines of the following code:
 
 ```bash
 $ conda create -n cyc-pep-perm python=3.10
-$ pip install cyc_pep_perm
+$ conda activate cyc-pep-perm
+$ pip install cyc-pep-perm==0.1.0
 ```
 
 ### 🛠️ For Developers
 <details>
   <summary>See detailed installation instructions</summary>
 The repository can be cloned from GitHub and installed with `pip` or `conda`. The code was built with Python 3.10 on Linux but other OS should work as well.
 
@@ -78,26 +79,29 @@
 ```
 </details>
 
 ## 🔥 Usage
 
 > For some more examples on how to process data, train and evaluate the alogrithms, please consult the folder `notebooks/`. This folder also contains a notebook to perform polynomial fits as described in the paper.
 
+All data paths in the following examples are taken from the hard-coded paths that work when one clones this repository. If you use the python package and download the data separately, please change the paths accordingly.
+
 ### Data preprocessing
 
-Here we showcase how to handle the data as for our use-case. Some simple reformating is done (see also the notebook `notebooks/01_data_preparation.ipynb`) starting from `.ods` file with DataWarrior output.
+Here we showcase how to handle the data as for our use-case. Some simple reformating is done (see also the notebook `notebooks/01_data_preparation.ipynb`) starting from `.ods` file with DataWarrior output (for data see [Data and Models](#data-and-models)).
 
 ```python
 import os
 
-from cyc_pep_perm.data.paths import DATA_PATH
 from cyc_pep_perm.data.processing import DataProcessing
 
+data_dir = "/path/to/data/folder" # ADAPT TO YOUR PATH!
+
 # this can also be a .csv input
-datapath = os.path.join(DATA_PATH, "perm_random80_train_raw.ods")
+datapath = os.path.join(data_dir, "perm_random80_train_raw.ods")
 
 # instantiate the class and make sure the columns match your inputed file - otherwise change arguments
 dp = DataProcessing(datapath=datapath)
 
 # make use of precomputed descriptors from DataWarrior
 df = dp.read_data(filename="perm_random80_train_dw.csv")
 
@@ -106,46 +110,59 @@
 ```
 
 ### Training
 
 Make sure to have the data ready to be used. In order to make the hyperparameter search more extensive, please look into the respective python scripts (e.g. `src/cyc_pep_perm/models/randomforest.py`) and adjust the `PARAMS` dictionary.
 
 ```python
+import os
+
 from cyc_pep_perm.models.randomforest import RF
-from cyc_pep_perm.data.paths import TRAIN_RANDOM_DW
+
+data_dir = "/path/to/data/folder" # ADAPT TO YOUR PATH!
+train_data = os.path.join(data_dir, "perm_random80_train_dw.csv")
+model_dir = "/path/to/model/folder" # ADAPT TO YOUR PATH!
+rf_model_trained = os.path.join(model_dir, "rf_random_dw.pkl")
 
 # instantiate class
 rf_regressor = RF()
 
 model = rf_regressor.train(
-    datapath = TRAIN_RANDOM_DW, # path to provided data from paper
+    datapath = train_data,
+    savepath = rf_model_trained,
 )
 
 y_pred, rmse, r2 = rf_regressor.evaluate()
 # will print training results, e.g.:
 >>> RMSE: 8.45
 >>> R2: 0.879
 ```
 
 ### Prediction
 
 ```python
+import os
+
 from cyc_pep_perm.models.randomforest import RF
-from cyc_pep_perm.data.paths import MODEL_RF_RANDOM_DW, TRAIN_RANDOM_DW
+
+data_dir = "/path/to/data/folder" # ADAPT TO YOUR PATH!
+train_data = os.path.join(data_dir, "perm_random80_train_dw.csv")
+model_dir = "/path/to/model/folder" # ADAPT TO YOUR PATH!
+rf_model_trained = os.path.join(model_dir, "rf_random_dw.pkl")
 
 # instantiate class
 rf_regressor = RF()
 
 # load trained model
 rf_regressor.load_model(
-    model_path = MODEL_RF_RANDOM_DW, # path to provided model from paper
+    modelpath = rf_model_trained,
 )
 
 # data to predict on, e.g.:
-df = pd.read_csv(TRAIN_RANDOM_DW)
+df = pd.read_csv(train_data)
 X = df.drop(columns=["SMILES"])
 
 # predict
 y_pred = rf_regressor.predict(X)
 ```
 
 ## Data and Models
```

### Comparing `cyc_pep_perm-0.0.1/data/perm_random20_test_dw.csv` & `cyc_pep_perm-0.1.0/data/perm_random20_test_dw.csv`

 * *Files identical despite different names*

### Comparing `cyc_pep_perm-0.0.1/data/perm_random20_test_mordred.csv` & `cyc_pep_perm-0.1.0/data/perm_random20_test_mordred.csv`

 * *Files identical despite different names*

### Comparing `cyc_pep_perm-0.0.1/data/perm_random20_test_raw.ods` & `cyc_pep_perm-0.1.0/data/perm_random20_test_raw.ods`

 * *Files identical despite different names*

### Comparing `cyc_pep_perm-0.0.1/data/perm_random80_train_dw.csv` & `cyc_pep_perm-0.1.0/data/perm_random80_train_dw.csv`

 * *Files identical despite different names*

### Comparing `cyc_pep_perm-0.0.1/data/perm_random80_train_mordred.csv` & `cyc_pep_perm-0.1.0/data/perm_random80_train_mordred.csv`

 * *Files identical despite different names*

### Comparing `cyc_pep_perm-0.0.1/data/perm_random80_train_raw.ods` & `cyc_pep_perm-0.1.0/data/perm_random80_train_raw.ods`

 * *Files identical despite different names*

### Comparing `cyc_pep_perm-0.0.1/docs/source/conf.py` & `cyc_pep_perm-0.1.0/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "cyc_pep_perm"
 copyright = f"{date.today().year}, Rebecca M Neeser"
 author = "Rebecca M Neeser"
 
 # The full version, including alpha/beta/rc tags.
-release = "0.0.1-dev"
+release = "0.1.0"
 
 # The short X.Y version.
 parsed_version = re.match(
     "(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?:-(?P<release>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?(?:\+(?P<build>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?",
     release,
 )
 version = parsed_version.expand("\g<major>.\g<minor>.\g<patch>")
```

### Comparing `cyc_pep_perm-0.0.1/docs/source/index.rst` & `cyc_pep_perm-0.1.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `cyc_pep_perm-0.0.1/docs/source/installation.rst` & `cyc_pep_perm-0.1.0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `cyc_pep_perm-0.0.1/models/rf_random_dw.pkl` & `cyc_pep_perm-0.1.0/models/rf_random_dw.pkl`

 * *Files identical despite different names*

### Comparing `cyc_pep_perm-0.0.1/models/rf_random_mordred.pkl` & `cyc_pep_perm-0.1.0/models/rf_random_mordred.pkl`

 * *Files identical despite different names*

### Comparing `cyc_pep_perm-0.0.1/models/xgb_random_dw.pkl` & `cyc_pep_perm-0.1.0/models/xgb_random_dw.pkl`

 * *Files identical despite different names*

### Comparing `cyc_pep_perm-0.0.1/models/xgb_random_mordred.pkl` & `cyc_pep_perm-0.1.0/models/xgb_random_mordred.pkl`

 * *Files identical despite different names*

### Comparing `cyc_pep_perm-0.0.1/playground.ipynb` & `cyc_pep_perm-0.1.0/playground.ipynb`

 * *Files identical despite different names*

### Comparing `cyc_pep_perm-0.0.1/requirements.txt` & `cyc_pep_perm-0.1.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `cyc_pep_perm-0.0.1/setup.cfg` & `cyc_pep_perm-0.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cyc_pep_perm
-version = 0.0.1
+version = 0.1.0
 description = Python package to predict membrane permeability of cyclic peptides.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/schwallergroup/CycPepPerm
 download_url = https://github.com/schwallergroup/CycPepPerm/releases
 project_urls = 
 	Tracker = https://github.com/schwallergroup/CycPepPerm/issues
```

### Comparing `cyc_pep_perm-0.0.1/src/cyc_pep_perm/cli.py` & `cyc_pep_perm-0.1.0/src/cyc_pep_perm/cli.py`

 * *Files identical despite different names*

### Comparing `cyc_pep_perm-0.0.1/src/cyc_pep_perm/data/descriptors.py` & `cyc_pep_perm-0.1.0/src/cyc_pep_perm/data/descriptors.py`

 * *Files identical despite different names*

### Comparing `cyc_pep_perm-0.0.1/src/cyc_pep_perm/data/paths.py` & `cyc_pep_perm-0.1.0/src/cyc_pep_perm/data/paths.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Paths to data and models.
 """
+
 import os
 
 ROOT_PATH = os.path.dirname(os.path.dirname(os.path.dirname(os.path.dirname(__file__))))
 
 DATA_PATH = os.path.join(ROOT_PATH, "data")
 TRAIN_RANDOM_DW = os.path.join(DATA_PATH, "perm_random80_train_dw.csv")
 TRAIN_RANDOM_MORDRED = os.path.join(DATA_PATH, "perm_random80_train_mordred.csv")
```

### Comparing `cyc_pep_perm-0.0.1/src/cyc_pep_perm/data/processing.py` & `cyc_pep_perm-0.1.0/src/cyc_pep_perm/data/processing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 import os
 import pickle
+from typing import Optional
 
 import pandas as pd
 from mordred import Calculator, descriptors
 from pandas_ods_reader import read_ods
 from rdkit import Chem
 from sklearn.preprocessing import StandardScaler
 
-from cyc_pep_perm.data import DATA_PATH, FEATURES_DW, MORDRED_DESCS
+from cyc_pep_perm.data import FEATURES_DW, MORDRED_DESCS
 
 
 class DataProcessing:
     """
     Class for processing data related to cyclic peptide membrane permeability.
     """
 
     def __init__(
         self,
-        datapath=os.path.join(
-            DATA_PATH, "Cyclic_peptide_membrane_permeability_random80percent.ods"
-        ),
-        target_label="CAPA [1 µM]",
-        smiles_label="SMILES",
+        datapath: str,
+        target_label: str = "CAPA [1 µM]",
+        smiles_label: str = "SMILES",
+        data: Optional[pd.DataFrame] = None,
+        df_mordred: Optional[pd.DataFrame] = None,
     ):
         """
         Initialize the DataProcessing object.
 
         Args:
             datapath (str): Path to the data file.
             target_label (str): Label of the target variable.
             smiles_label (str): Label of the SMILES column.
         """
         self.datapath = datapath
         assert os.path.exists(self.datapath), "File does not exist"
+        self.data_dir = os.path.dirname(self.datapath)
         self.target_label = target_label
         self.smiles_label = smiles_label
-        self.data = None
-        self.df_mordred = None
+        self.data = data
+        self.df_mordred = df_mordred
         self.calculator = Calculator(descriptors, ignore_3D=True)
         print(f"Target column: {self.target_label}")
         print(f"SMILES column: {self.smiles_label}")
 
-    def read_data(self, filename=None):
+    def read_data(self, filename: Optional[str] = None):
         """
         Read the data from the file and perform necessary preprocessing.
         """
         try:
             self.data = pd.read_csv(self.datapath)
         except Exception:
             self.data = read_ods(self.datapath, 1)
@@ -62,46 +64,47 @@
         # drop irrelevant columns for training
         if "target" in self.data.columns:
             self.data = self.data[["SMILES", "target"] + FEATURES_DW]
         else:
             self.data = self.data[["SMILES"] + FEATURES_DW]
 
         if filename:
-            new_filepath = os.path.join(DATA_PATH, filename)
+            new_filepath = os.path.join(self.data_dir, filename)
         else:
             new_filepath = os.path.join(
-                DATA_PATH, f'{self.datapath.split("/")[-1].split(".")[0]}.csv'
+                self.data_dir, f'{self.datapath.split("/")[-1].split(".")[0]}.csv'
             )
         self.data.to_csv(new_filepath, index=False)
 
         print(f"Saved data to {new_filepath}")
 
         return self.data
 
-    def calc_mordred(self, filename=None):
+    def calc_mordred(self, filename: Optional[str] = None):
         """
         Calculate Mordred descriptors for the molecules and save the results to a file.
 
         Args:
             filename (str, optional): Path to save the Mordred data. If not provided, a
             default filename will be used.
         """
         if self.data is None:
             self.read_data()
 
         self.df_mordred = self.calculator.pandas(self.mols)
         self.df_mordred = self.df_mordred[MORDRED_DESCS]
 
         self.df_mordred["SMILES"] = self.smiles
-        if "target" in self.data.columns:
-            self.df_mordred["target"] = self.data["target"]
+        if self.data is not None and isinstance(self.data, pd.DataFrame):
+            if "target" in self.data.columns:
+                self.df_mordred["target"] = self.data["target"]
 
         if not filename:
             filename = os.path.join(
-                DATA_PATH, f'{self.datapath.split("/")[-1].split(".")[0]}_mordred.csv'
+                self.data_dir, f'{self.datapath.split("/")[-1].split(".")[0]}_mordred.csv'
             )
         self.df_mordred.to_csv(filename, index=False)
 
         print(f"Saved Mordred descriptors to {filename}")
 
         return self.df_mordred
 
@@ -117,15 +120,15 @@
             the default path will be used.
         """
 
         if raw_data:
             data = pd.read_csv(raw_data)
             scaler_path = raw_data.split(".")[0] + "_scaler.pkl"
         else:
-            scaled_folder = os.path.join(DATA_PATH, "scaled")
+            scaled_folder = os.path.join(self.data_dir, "scaled")
             basename = self.datapath.split("/")[-1].split(".")[0]
             scaler_path = os.path.join(scaled_folder, basename + "_scaler.pkl")
             raw_data = os.path.join(scaled_folder, basename + ".csv")
             if mordred:
                 raw_data = raw_data.split(".")[0] + "_mordred.csv"
                 assert self.df_mordred is not None, "Mordred data not loaded"
                 data = self.df_mordred
```

### Comparing `cyc_pep_perm-0.0.1/src/cyc_pep_perm/models/randomforest.py` & `cyc_pep_perm-0.1.0/src/cyc_pep_perm/models/randomforest.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 import numpy as np
 import pandas as pd
 import shap
 from sklearn.ensemble import RandomForestRegressor
 from sklearn.metrics import mean_squared_error, r2_score
 from sklearn.model_selection import GridSearchCV, KFold
 
-from cyc_pep_perm.data import MODEL_RF_RANDOM_DW, TRAIN_RANDOM_DW
-
 PARAMS = {
     "n_estimators": [100, 200, 300, 400, 500],  # number of trees
     # "max_features": ["sqrt", "log2", 1.0],  # features to consider at every split
     # "max_depth": [5, 10, 20, 30],  # maximum depth of tree
     # "min_samples_split": [2, 5, 10, 20],  # min samples required to split a node
     # "min_samples_leaf": [1, 2, 4, 8],  # min samples required to be at a leaf node
     # "bootstrap": [True, False],  # method of selecting samples for training each tree
@@ -43,28 +41,29 @@
         self.data: pd.DataFrame = None
         self.X: pd.DataFrame = None
         self.y: pd.Series = None
         self.best_model: RandomForestRegressor = None
 
     def train(
         self,
-        datapath: Union[str, pd.DataFrame] = TRAIN_RANDOM_DW,
+        datapath: Union[str, pd.DataFrame],
+        savepath: str,
         params: Dict[str, List[Any]] = PARAMS,
-        savepath: str = MODEL_RF_RANDOM_DW,
         seed: int = 42,
         n_folds: int = 8,
     ) -> RandomForestRegressor:
         """
         Trains a random forest regressor model.
 
         Args:
-            datapath (str): The path to the training data. params (Dict[str, list]): The
-            hyperparameters for the random forest regressor model.
+            datapath (str): The path to the training data.
             savepath (str): The
             path to save the trained model.
+            params (Dict[str, list]): The
+            hyperparameters for the random forest regressor model.
 
         Returns:
             RandomForestRegressor: The best trained random forest regressor model.
 
         Raises:
             AssertionError: If the specified datapath does not exist.
         """
@@ -101,14 +100,15 @@
 
         print(f"Best parameters: {gs.best_params_}")
 
         # save best model
         os.makedirs(os.path.dirname(savepath), exist_ok=True)
         with open(savepath, "wb") as f:
             pickle.dump(self.best_model, f)
+        print(f"Best model saved to {savepath}")
 
         return self.best_model
 
     def evaluate(self, X: pd.DataFrame = None, y: pd.Series = None) -> tuple:
         """
         Evaluates the trained model on given data.
 
@@ -157,15 +157,15 @@
 
         """
 
         assert self.best_model is not None, "Best model not found - load or train model"
         y_pred = self.best_model.predict(X)
         return y_pred
 
-    def load(self, modelpath: str = MODEL_RF_RANDOM_DW) -> RandomForestRegressor:
+    def load(self, modelpath: str) -> RandomForestRegressor:
         """
         Loads a trained model from a file.
 
         Args:
             modelpath (str): The path to the trained model file.
 
         Returns:
```

### Comparing `cyc_pep_perm-0.0.1/src/cyc_pep_perm/models/randomforest_class.py` & `cyc_pep_perm-0.1.0/src/cyc_pep_perm/models/randomforest_class.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 import numpy as np
 import pandas as pd
 import shap
 from sklearn.ensemble import RandomForestClassifier
 from sklearn.metrics import accuracy_score, confusion_matrix
 from sklearn.model_selection import GridSearchCV, KFold
 
-from cyc_pep_perm.data import MODEL_RFCLASS_RANDOM_DW, TRAIN_RANDOM_DW
-
 PARAMS = {
     "n_estimators": [100, 200, 300, 400, 500],  # number of trees
     "class_weight": ["balanced_subsample"],  # class weights
     # "max_features": ["sqrt", "log2", 1.0],  # features to consider at every split
     # "max_depth": [5, 10, 20, 30],  # maximum depth of tree
     # "min_samples_split": [2, 5, 10, 20],  # min samples required to split a node
     # "min_samples_leaf": [1, 2, 4, 8],  # min samples required to be at a leaf node
@@ -44,28 +42,29 @@
         self.data: pd.DataFrame = None
         self.X: pd.DataFrame = None
         self.y: pd.Series = None
         self.best_model: RandomForestClassifier = None
 
     def train(
         self,
-        datapath: Union[str, pd.DataFrame] = TRAIN_RANDOM_DW,
+        datapath: Union[str, pd.DataFrame],
+        savepath: str,
         params: Dict[str, object] = PARAMS,
-        savepath: str = MODEL_RFCLASS_RANDOM_DW,
         seed: int = 42,
         n_folds: int = 8,
     ) -> RandomForestClassifier:
         """
         Trains a random forest classifier model.
 
         Args:
-            datapath (str): The path to the training data. params (Dict[str, list]): The
-            hyperparameters for the random forest classifier model.
+            datapath (str): The path to the training data.
             savepath (str): The
             path to save the trained model.
+            params (Dict[str, list]): The
+            hyperparameters for the random forest classifier model.
 
         Returns:
             RandomForestClassifier: The best trained random forest classifier model.
 
         Raises:
             AssertionError: If the specified datapath does not exist.
         """
@@ -103,14 +102,15 @@
 
         print(f"Best parameters: {gs.best_params_}")
 
         # save best model
         os.makedirs(os.path.dirname(savepath), exist_ok=True)
         with open(savepath, "wb") as f:
             pickle.dump(self.best_model, f)
+        print(f"Best model saved to {savepath}")
 
         return self.best_model
 
     def evaluate(self, X: pd.DataFrame = None, y: pd.Series = None) -> tuple:
         """
         Evaluates the trained model on given data.
 
@@ -159,15 +159,15 @@
 
         """
 
         assert self.best_model is not None, "Best model not found - load or train model"
         y_pred = self.best_model.predict(X)
         return y_pred
 
-    def load(self, modelpath: str = MODEL_RFCLASS_RANDOM_DW) -> RandomForestClassifier:
+    def load(self, modelpath: str) -> RandomForestClassifier:
         """
         Loads a trained model from a file.
 
         Args:
             modelpath (str): The path to the trained model file.
 
         Returns:
```

### Comparing `cyc_pep_perm-0.0.1/src/cyc_pep_perm/models/xgboost.py` & `cyc_pep_perm-0.1.0/src/cyc_pep_perm/models/xgboost.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 import numpy as np
 import pandas as pd
 import shap
 from sklearn.metrics import mean_squared_error, r2_score
 from sklearn.model_selection import GridSearchCV, KFold
 from xgboost import XGBRegressor
 
-from cyc_pep_perm.data import MODEL_XGB_RANDOM_DW, TRAIN_RANDOM_DW
-
 PARAMS = {
     # 'max_depth': [3, 4, 5, 8, 10],
     # 'learning_rate': [0.01, 0.05, 0.1, 0.15, 0.2],
     "n_estimators": [100, 200, 300, 400, 500],
     # 'reg_alpha': [0.01, 0.05, 0.1, 0.15, 0.2],
     # 'reg_lambda': [0.01, 0.05, 0.1, 0.15, 0.2],
     # 'min_child_weight': [1, 2, 5, 8, 10],
@@ -45,28 +43,29 @@
         self.data: pd.DataFrame = None
         self.X: pd.DataFrame = None
         self.y: pd.Series = None
         self.best_model: XGBRegressor = None
 
     def train(
         self,
-        datapath: Union[str, pd.DataFrame] = TRAIN_RANDOM_DW,
+        datapath: Union[str, pd.DataFrame],
+        savepath: str,
         params: Dict[str, List[Any]] = PARAMS,
-        savepath: str = MODEL_XGB_RANDOM_DW,
         seed: int = 42,
         n_folds: int = 8,
     ) -> XGBRegressor:
         """
         Trains a XGBoost regressor model.
 
         Args:
-            datapath (str): The path to the training data. params (Dict[str, list]): The
-            hyperparameters for the XGBoost regressor model.
+            datapath (str): The path to the training data.
             savepath (str): The
             path to save the trained model.
+            params (Dict[str, list]): The
+            hyperparameters for the XGBoost regressor model.
 
         Returns:
             XGBRegressor: The best trained XGBoost regressor model.
 
         Raises:
             AssertionError: If the specified datapath does not exist.
         """
@@ -103,14 +102,15 @@
 
         print(f"Best parameters: {gs.best_params_}")
 
         # save best model
         os.makedirs(os.path.dirname(savepath), exist_ok=True)
         with open(savepath, "wb") as f:
             pickle.dump(self.best_model, f)
+        print(f"Best model saved to {savepath}")
 
         return self.best_model
 
     def evaluate(self, X: pd.DataFrame = None, y: pd.Series = None) -> tuple:
         """
         Evaluates the trained model on given data.
 
@@ -159,15 +159,15 @@
 
         """
 
         assert self.best_model is not None, "Best model not found - load or train model"
         y_pred = self.best_model.predict(X)
         return y_pred
 
-    def load(self, modelpath: str = MODEL_XGB_RANDOM_DW) -> XGBRegressor:
+    def load(self, modelpath: str) -> XGBRegressor:
         """
         Loads a trained model from a file.
 
         Args:
             modelpath (str): The path to the trained model file.
 
         Returns:
```

### Comparing `cyc_pep_perm-0.0.1/src/cyc_pep_perm/version.py` & `cyc_pep_perm-0.1.0/src/cyc_pep_perm/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 __all__ = [
     "VERSION",
     "get_version",
     "get_git_hash",
 ]
 
-VERSION = "0.0.1"
+VERSION = "0.1.0"
 
 
 def get_git_hash() -> str:
     """Get the :mod:`cyc_pep_perm` git hash."""
     with open(os.devnull, "w") as devnull:
         try:
             ret = check_output(  # noqa: S603,S607
```

### Comparing `cyc_pep_perm-0.0.1/src/cyc_pep_perm.egg-info/PKG-INFO` & `cyc_pep_perm-0.1.0/src/cyc_pep_perm.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyc_pep_perm
-Version: 0.0.1
+Version: 0.1.0
 Summary: Python package to predict membrane permeability of cyclic peptides.
 Home-page: https://github.com/schwallergroup/CycPepPerm
 Download-URL: https://github.com/schwallergroup/CycPepPerm/releases
 Author: Rebecca M Neeser
 Author-email: rebecca.neeser@epfl.ch
 Maintainer: Rebecca M Neeser
 Maintainer-email: rebecca.neeser@epfl.ch
@@ -78,19 +78,20 @@
 
 <br>
 
 Python package to predict membrane permeability of cyclic peptides.
 
 ## 👩‍💻 Installation
 
-We provide the code as a python package, so the only thing you need is to install it. We recommend creating a new conda environment for that (otherwise skip first line.
+We provide the code as a [python package](https://pypi.org/project/cyc-pep-perm/), so the only thing you need is to install it. We recommend creating a new conda environment for that, which allows simple package management for a project. Follow these [instructions](https://docs.anaconda.com/free/anaconda/install/index.html) to install Anaconda. However, the package containing our code can also be installed without creating a project-specific environment. In that case, one just skips the first two lines of the following code:
 
 ```bash
 $ conda create -n cyc-pep-perm python=3.10
-$ pip install cyc_pep_perm
+$ conda activate cyc-pep-perm
+$ pip install cyc-pep-perm==0.1.0
 ```
 
 ### 🛠️ For Developers
 <details>
   <summary>See detailed installation instructions</summary>
 The repository can be cloned from GitHub and installed with `pip` or `conda`. The code was built with Python 3.10 on Linux but other OS should work as well.
 
@@ -133,26 +134,29 @@
 ```
 </details>
 
 ## 🔥 Usage
 
 > For some more examples on how to process data, train and evaluate the alogrithms, please consult the folder `notebooks/`. This folder also contains a notebook to perform polynomial fits as described in the paper.
 
+All data paths in the following examples are taken from the hard-coded paths that work when one clones this repository. If you use the python package and download the data separately, please change the paths accordingly.
+
 ### Data preprocessing
 
-Here we showcase how to handle the data as for our use-case. Some simple reformating is done (see also the notebook `notebooks/01_data_preparation.ipynb`) starting from `.ods` file with DataWarrior output.
+Here we showcase how to handle the data as for our use-case. Some simple reformating is done (see also the notebook `notebooks/01_data_preparation.ipynb`) starting from `.ods` file with DataWarrior output (for data see [Data and Models](#data-and-models)).
 
 ```python
 import os
 
-from cyc_pep_perm.data.paths import DATA_PATH
 from cyc_pep_perm.data.processing import DataProcessing
 
+data_dir = "/path/to/data/folder" # ADAPT TO YOUR PATH!
+
 # this can also be a .csv input
-datapath = os.path.join(DATA_PATH, "perm_random80_train_raw.ods")
+datapath = os.path.join(data_dir, "perm_random80_train_raw.ods")
 
 # instantiate the class and make sure the columns match your inputed file - otherwise change arguments
 dp = DataProcessing(datapath=datapath)
 
 # make use of precomputed descriptors from DataWarrior
 df = dp.read_data(filename="perm_random80_train_dw.csv")
 
@@ -161,46 +165,59 @@
 ```
 
 ### Training
 
 Make sure to have the data ready to be used. In order to make the hyperparameter search more extensive, please look into the respective python scripts (e.g. `src/cyc_pep_perm/models/randomforest.py`) and adjust the `PARAMS` dictionary.
 
 ```python
+import os
+
 from cyc_pep_perm.models.randomforest import RF
-from cyc_pep_perm.data.paths import TRAIN_RANDOM_DW
+
+data_dir = "/path/to/data/folder" # ADAPT TO YOUR PATH!
+train_data = os.path.join(data_dir, "perm_random80_train_dw.csv")
+model_dir = "/path/to/model/folder" # ADAPT TO YOUR PATH!
+rf_model_trained = os.path.join(model_dir, "rf_random_dw.pkl")
 
 # instantiate class
 rf_regressor = RF()
 
 model = rf_regressor.train(
-    datapath = TRAIN_RANDOM_DW, # path to provided data from paper
+    datapath = train_data,
+    savepath = rf_model_trained,
 )
 
 y_pred, rmse, r2 = rf_regressor.evaluate()
 # will print training results, e.g.:
 >>> RMSE: 8.45
 >>> R2: 0.879
 ```
 
 ### Prediction
 
 ```python
+import os
+
 from cyc_pep_perm.models.randomforest import RF
-from cyc_pep_perm.data.paths import MODEL_RF_RANDOM_DW, TRAIN_RANDOM_DW
+
+data_dir = "/path/to/data/folder" # ADAPT TO YOUR PATH!
+train_data = os.path.join(data_dir, "perm_random80_train_dw.csv")
+model_dir = "/path/to/model/folder" # ADAPT TO YOUR PATH!
+rf_model_trained = os.path.join(model_dir, "rf_random_dw.pkl")
 
 # instantiate class
 rf_regressor = RF()
 
 # load trained model
 rf_regressor.load_model(
-    model_path = MODEL_RF_RANDOM_DW, # path to provided model from paper
+    modelpath = rf_model_trained,
 )
 
 # data to predict on, e.g.:
-df = pd.read_csv(TRAIN_RANDOM_DW)
+df = pd.read_csv(train_data)
 X = df.drop(columns=["SMILES"])
 
 # predict
 y_pred = rf_regressor.predict(X)
 ```
 
 ## Data and Models
```

### Comparing `cyc_pep_perm-0.0.1/src/cyc_pep_perm.egg-info/SOURCES.txt` & `cyc_pep_perm-0.1.0/src/cyc_pep_perm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyc_pep_perm-0.0.1/tests/test_models/rf_random_dw_unittest.pkl` & `cyc_pep_perm-0.1.0/tests/test_models/rf_random_dw_unittest.pkl`

 * *Files identical despite different names*

### Comparing `cyc_pep_perm-0.0.1/tests/test_randomforest.py` & `cyc_pep_perm-0.1.0/tests/test_randomforest.py`

 * *Files identical despite different names*

