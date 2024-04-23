# Comparing `tmp/thoughtspot_tml-2.0.8.tar.gz` & `tmp/thoughtspot_tml-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thoughtspot_tml-2.0.8.tar", last modified: Mon Nov  6 20:26:29 2023, max compression
+gzip compressed data, was "thoughtspot_tml-2.0.9.tar", last modified: Wed Nov 15 22:28:50 2023, max compression
```

## Comparing `thoughtspot_tml-2.0.8.tar` & `thoughtspot_tml-2.0.9.tar`

### file list

```diff
@@ -1,76 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:26:29.582878 thoughtspot_tml-2.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:26:29.570878 thoughtspot_tml-2.0.8/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      983 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:26:29.570878 thoughtspot_tml-2.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      432 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      878 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      654 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      493 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    14780 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    39145 2023-11-06 20:26:29.582878 thoughtspot_tml-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22389 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:26:29.570878 thoughtspot_tml-2.0.8/_generate/
--rw-r--r--   0 runner    (1001) docker     (127)     7417 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/_generate/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4487 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/_generate/_proto_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:26:29.574878 thoughtspot_tml-2.0.8/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/examples/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     8964 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/examples/basic_input_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     5204 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/examples/common_attribute_changes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:26:29.574878 thoughtspot_tml-2.0.8/examples/worksheet-namespace-remapping/
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/examples/worksheet-namespace-remapping/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/examples/worksheet-namespace-remapping/worksheet_remapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-06 20:26:29.582878 thoughtspot_tml-2.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      241 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:26:29.570878 thoughtspot_tml-2.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:26:29.574878 thoughtspot_tml-2.0.8/src/thoughtspot_tml/
--rw-r--r--   0 runner    (1001) docker     (127)      709 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/src/thoughtspot_tml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/src/thoughtspot_tml/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    40670 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/src/thoughtspot_tml/_scriptability.py
--rw-r--r--   0 runner    (1001) docker     (127)     7409 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/src/thoughtspot_tml/_tml.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/src/thoughtspot_tml/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/src/thoughtspot_tml/_yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/src/thoughtspot_tml/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3872 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/src/thoughtspot_tml/spotapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     6775 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/src/thoughtspot_tml/tml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/src/thoughtspot_tml/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    13924 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/src/thoughtspot_tml/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:26:29.574878 thoughtspot_tml-2.0.8/src/thoughtspot_tml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    39145 2023-11-06 20:26:29.000000 thoughtspot_tml-2.0.8/src/thoughtspot_tml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2023-11-06 20:26:29.000000 thoughtspot_tml-2.0.8/src/thoughtspot_tml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-06 20:26:29.000000 thoughtspot_tml-2.0.8/src/thoughtspot_tml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      250 2023-11-06 20:26:29.000000 thoughtspot_tml-2.0.8/src/thoughtspot_tml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-11-06 20:26:29.000000 thoughtspot_tml-2.0.8/src/thoughtspot_tml.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:26:29.578878 thoughtspot_tml-2.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/tests/_const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:26:29.582878 thoughtspot_tml-2.0.8/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/tests/data/BAD_DUMMY.answer.tml
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/tests/data/DUMMY.answer.tml
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/tests/data/DUMMY.connection.tml
--rw-r--r--   0 runner    (1001) docker     (127)     6175 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/tests/data/DUMMY.liveboard.tml
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/tests/data/DUMMY.pinboard.tml
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/tests/data/DUMMY.sql_view.tml
--rw-r--r--   0 runner    (1001) docker     (127)      882 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/tests/data/DUMMY.table.tml
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/tests/data/DUMMY.view.tml
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/tests/data/DUMMY.worksheet.tml
--rw-r--r--   0 runner    (1001) docker     (127)     4025 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/tests/data/DUMMY_spot_app.zip
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/tests/data/SPECIAL_TABLE.table.tml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:26:29.582878 thoughtspot_tml-2.0.8/tests/data/_temp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/tests/data/_temp/.gitdontignore
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/tests/data/connection.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      380 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/tests/test_answer.py
--rw-r--r--   0 runner    (1001) docker     (127)    14836 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/tests/test_liveboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/tests/test_pinboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/tests/test_special.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/tests/test_spotapp.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/tests/test_sql_view.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/tests/test_tml.py
--rw-r--r--   0 runner    (1001) docker     (127)     8794 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/tests/test_view.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2023-11-06 20:26:23.000000 thoughtspot_tml-2.0.8/tests/test_worksheet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:28:50.453102 thoughtspot_tml-2.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:28:50.445102 thoughtspot_tml-2.0.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:28:50.445102 thoughtspot_tml-2.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    14780 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    39352 2023-11-15 22:28:50.453102 thoughtspot_tml-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22596 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:28:50.445102 thoughtspot_tml-2.0.9/_generate/
+-rw-r--r--   0 runner    (1001) docker     (127)     7417 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/_generate/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4487 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/_generate/_proto_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:28:50.445102 thoughtspot_tml-2.0.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8728 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/examples/basic_input_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5170 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/examples/common_attribute_changes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:28:50.445102 thoughtspot_tml-2.0.9/examples/worksheet-namespace-remapping/
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/examples/worksheet-namespace-remapping/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/examples/worksheet-namespace-remapping/worksheet_remapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4070 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-15 22:28:50.453102 thoughtspot_tml-2.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:28:50.441102 thoughtspot_tml-2.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:28:50.449102 thoughtspot_tml-2.0.9/src/thoughtspot_tml/
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/src/thoughtspot_tml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/src/thoughtspot_tml/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40670 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/src/thoughtspot_tml/_scriptability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7474 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/src/thoughtspot_tml/_tml.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/src/thoughtspot_tml/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/src/thoughtspot_tml/_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/src/thoughtspot_tml/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/src/thoughtspot_tml/spotapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6812 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/src/thoughtspot_tml/tml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/src/thoughtspot_tml/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13924 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/src/thoughtspot_tml/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:28:50.449102 thoughtspot_tml-2.0.9/src/thoughtspot_tml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    39352 2023-11-15 22:28:50.000000 thoughtspot_tml-2.0.9/src/thoughtspot_tml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2023-11-15 22:28:50.000000 thoughtspot_tml-2.0.9/src/thoughtspot_tml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-15 22:28:50.000000 thoughtspot_tml-2.0.9/src/thoughtspot_tml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2023-11-15 22:28:50.000000 thoughtspot_tml-2.0.9/src/thoughtspot_tml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2023-11-15 22:28:50.000000 thoughtspot_tml-2.0.9/src/thoughtspot_tml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:28:50.453102 thoughtspot_tml-2.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/tests/_const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:28:50.453102 thoughtspot_tml-2.0.9/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/tests/data/BAD_DUMMY.answer.tml
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/tests/data/DUMMY.answer.tml
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/tests/data/DUMMY.connection.tml
+-rw-r--r--   0 runner    (1001) docker     (127)     6175 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/tests/data/DUMMY.liveboard.tml
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/tests/data/DUMMY.pinboard.tml
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/tests/data/DUMMY.sql_view.tml
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/tests/data/DUMMY.table.tml
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/tests/data/DUMMY.view.tml
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/tests/data/DUMMY.worksheet.tml
+-rw-r--r--   0 runner    (1001) docker     (127)     4025 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/tests/data/DUMMY_spot_app.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/tests/data/SPECIAL_TABLE.table.tml
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/tests/data/SPECIAL_UNICODE_TABLE.table.tml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:28:50.453102 thoughtspot_tml-2.0.9/tests/data/_temp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/tests/data/_temp/.gitdontignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/tests/data/connection.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/tests/test_answer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14836 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/tests/test_liveboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/tests/test_pinboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/tests/test_special.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/tests/test_spotapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/tests/test_sql_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/tests/test_tml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8794 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/tests/test_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2023-11-15 22:28:43.000000 thoughtspot_tml-2.0.9/tests/test_worksheet.py
```

### Comparing `thoughtspot_tml-2.0.8/.github/CONTRIBUTING.md` & `thoughtspot_tml-2.0.9/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `thoughtspot_tml-2.0.8/.gitignore` & `thoughtspot_tml-2.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `thoughtspot_tml-2.0.8/LICENSE` & `thoughtspot_tml-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `thoughtspot_tml-2.0.8/PKG-INFO` & `thoughtspot_tml-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thoughtspot_tml
-Version: 2.0.8
+Version: 2.0.9
 Summary: Library for manipulating ThoughtSpot Modeling Language (TML) files
 Author-email: Bryant Howell <bryant.howell@thoughtspot.com>, Bill B <bill.back@thoughtspot.com>, boonhapus <nicholas.cooper@thoughtspot.com>
 Maintainer-email: Bryant Howell <bryant.howell@thoughtspot.com>, boonhapus <nicholas.cooper@thoughtspot.com>
 License: #ThoughtSpot Development Tools End User License Agreement
         
         THIS THOUGHTSPOT DEVELOPMENT TOOLS END USER LICENSE AGREEMENT (“EULA”) FORMS A BINDING AGREEMENT BETWEEN YOU INDIVIDUALLY OR THE BUSINESS ENTITY OR PUBLIC AGENCY ON WHOSE BEHALF YOU ARE ACCEPTING THIS AGREEMENT (“COMPANY”) AND THOUGHTSPOT, INC. (“THOUGHTSPOT”). THIS EULA DESCRIBES THE RIGHTS AND OBLIGATIONS OF COMPANY AND THOUGHTSPOT GOVERNING THE USE OF ANY APPLICATION PROGRAMMING INTERFACE, CONNECTOR, SOFTWARE DEVELOPMENT KIT, CODE SNIPPET, SAMPLE CODE, FREE CUSTOM USER INTERFACE OR VISUALIZATION, SAMPLE DATA, AND THE CORRESPONDING DOCUMENTATION FOR EACH, ANY UPDATES AND UPGRADES THERETO, AND ANY MODIFICATIONS, ENHANCEMENTS, OR IMPROVEMENTS, OF ANY OF THE FOREGOING, MADE AVAILABLE BY THOUGHTSPOT TOGETHER WITH THIS EULA (EACH A “TOOL” AND COLLECTIVELY “TOOLS”).
         
@@ -74,14 +74,17 @@
 Requires-Dist: coverage[toml]; extra == "dev"
 
 <div align="center">
   <h2><b>ThoughtSpot TML</b></h2>
 
   <i>a Python package for working with</i> <b>ThoughtSpot</b> <i>Modeling Language (TML) files programmatically</i>
 
+  ![Badge: Lint](https://github.com/thoughtspot/thoughtspot_tml/actions/workflows/lint.yml/badge.svg)
+  ![Badge: Test](https://github.com/thoughtspot/thoughtspot_tml/actions/workflows/test.yml/badge.svg)
+  
   <h3>
     <a href="#installation">Installation</a>
     <span> | </span>
     <a href="#a-basic-example">Example</a>
     <span> | </span>
     <a href="#migration-to-v200">Migration to v2.0.0</a>
     <span> | </span>
```

### Comparing `thoughtspot_tml-2.0.8/README.md` & `thoughtspot_tml-2.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 <div align="center">
   <h2><b>ThoughtSpot TML</b></h2>
 
   <i>a Python package for working with</i> <b>ThoughtSpot</b> <i>Modeling Language (TML) files programmatically</i>
 
+  ![Badge: Lint](https://github.com/thoughtspot/thoughtspot_tml/actions/workflows/lint.yml/badge.svg)
+  ![Badge: Test](https://github.com/thoughtspot/thoughtspot_tml/actions/workflows/test.yml/badge.svg)
+  
   <h3>
     <a href="#installation">Installation</a>
     <span> | </span>
     <a href="#a-basic-example">Example</a>
     <span> | </span>
     <a href="#migration-to-v200">Migration to v2.0.0</a>
     <span> | </span>
```

### Comparing `thoughtspot_tml-2.0.8/_generate/__main__.py` & `thoughtspot_tml-2.0.9/_generate/__main__.py`

 * *Files identical despite different names*

### Comparing `thoughtspot_tml-2.0.8/_generate/_proto_local.py` & `thoughtspot_tml-2.0.9/_generate/_proto_local.py`

 * *Files identical despite different names*

### Comparing `thoughtspot_tml-2.0.8/examples/README.md` & `thoughtspot_tml-2.0.9/examples/README.md`

 * *Files identical despite different names*

### Comparing `thoughtspot_tml-2.0.8/examples/basic_input_output.py` & `thoughtspot_tml-2.0.9/examples/basic_input_output.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from thoughtspot_tml import *
 from thoughtspot_tml.utils import *
 
 # Python request library for HTTP calls
 from requests import *
+
 # REST API library installable via pip
 from thoughtspot_rest_api_v1 import *
 
 # Examples of retrieving TML, loading into thoughtspot_tml objects, and serializing objects back into TML files
 # Other examples, showing actual transformations on the TML objects, will refer to this example
 
 # 'Publishing' a TML file to a ThoughtSpot instance uses the REST API /metadata/tml/import endpoint (V1 or V2.0)
@@ -16,207 +17,188 @@
 # After publishing, you will want to retrieve the GUIDs from the response, for any newly created objects
 # /security/metadata/share endpoint (V2.0) can be used to give access to the newly created objects
 # For example, see https://github.com/thoughtspot/thoughtspot_rest_api_v1_python/blob/main/examples_v2/share_objects_access_control.py
 
 
 # If you have TML files in a directory already:
 def retrieve_from_disk():
-
     # Read from file when you know the object type
-    tml_obj = Worksheet.load('/file/location/on/disk/something.worksheet.tml')
+    tml_obj = Worksheet.load("/file/location/on/disk/something.worksheet.tml")
 
     # Read from an unknown type TML file using determine_tml_type() helper
     tml_cls = determine_tml_type(path="/tests/data/some_type_of_file.tml")
     tml_obj = tml_cls.load(path="/tests/data/DUMMY.worksheet.tml")
     if type(tml) is Worksheet:
         # Do things specific to the worksheet
         pass
 
     return tml_obj
 
+
 def export_to_string(tml_object):
     # Each TML class has a .dumps(format_type="YAML") method to string
     tml_str = tml_object.dumps(format_type="YAML")
     print(tml_str)
     return tml_str
 
+
 def export_to_disk(tml_object):
     # Each TML class has a .dump() method to serialize and save directly to disk
 
     # Example of programmatic naming with the GUID of the TML object. Make sure not to overwrite, and you may have
     # removed the GUID as well depending on what process you are going through
     export_path = "/tests/data/{}.worksheet.tml".format(tml_object.guid)
 
     tml_object.dump(path=export_path)
     return export_path
 
+
 #
 # REST API interactions below
 # A simple implementations of REST functionality here based on thoughtspot_rest_api_v1 library (https://github.com/thoughtspot/thoughtspot_rest_api_v1_python)
 # Please use the library for building more complex actions (it will save you time and effort)
 
+
 def get_v2_api_token(session, thoughtspot_server, username, password, validity_time_in_sec=300):
     # V2.0 API needs a token
-    endpoint = 'auth/token/full'
-    url = '{}/api/rest/{}/{}'.format(thoughtspot_server, '2.0', endpoint)
-    json_post_data = {
-        'username': username,
-        'password': password,
-        'validity_time_in_sec': validity_time_in_sec
-    }
+    endpoint = "auth/token/full"
+    url = "{}/api/rest/{}/{}".format(thoughtspot_server, "2.0", endpoint)
+    json_post_data = {"username": username, "password": password, "validity_time_in_sec": validity_time_in_sec}
 
     response = session.post(url=url, json=json_post_data)
 
     response.raise_for_status()
     token_response = response.json()
-    token = token_response['token']
+    token = token_response["token"]
     return token
 
 
 def retrieve_from_api_no_library():
     # ThoughtSpot has V1 and V2 REST APIs
     # Both have a /metadata/tml/export endpoint to get TML as a string, in the 'edoc' portion of the response
     # V1 can export in YAML or JSON, V2 currently only in JSON (eventually will support YAML)
 
     # http://github.com/thoughtspot/thoughtspot_rest_api_v1_python is pre-built library to handle REST API interactions
 
-    thoughtspot_server = 'https://myinstance.thoughtspot.cloud'
-    username = 'myUsername@company.com'
-    password = 'apassword' # Find another way of storing to actually secure this
+    thoughtspot_server = "https://myinstance.thoughtspot.cloud"
+    username = "myUsername@company.com"
+    password = "apassword"  # Find another way of storing to actually secure this
 
     # Create a session object to save some header settings etc.
     requests_session = requests.Session()
-    api_headers = {'X-Requested-By': 'ThoughtSpot', 'Accept': 'application/json', 'Accept-Language': 'en_US'}
+    api_headers = {"X-Requested-By": "ThoughtSpot", "Accept": "application/json", "Accept-Language": "en_US"}
     requests_session.headers.update(api_headers)
 
-    token = get_v2_api_token(session=requests_session, thoughtspot_server=thoughtspot_server, username=username,
-                             password=password, validity_time_in_sec=300)
+    token = get_v2_api_token(
+        session=requests_session,
+        thoughtspot_server=thoughtspot_server,
+        username=username,
+        password=password,
+        validity_time_in_sec=300,
+    )
 
     # Add the token to the Session object for subsequent calls
-    api_headers['Authorization'] = 'Bearer {}'.format(token)
+    api_headers["Authorization"] = "Bearer {}".format(token)
     requests_session.headers.update(api_headers)
 
     # To find any particular object, use the 'metadata/search' endpoint
     # The request can be built with a large number of filtering and sorting options
     # See all of the fields in the V2.0 REST Playground
 
     metadata_search_request = {
-        'metadata': {
-            'type': 'Liveboard',
-            'name_pattern': "DEV_%"
-        },
-        'create_by_user_identifiers': ['admin_a', 'admin_b'],
-        'sort_options': {
-            'field_name': 'MODIFIED',
-            'order': 'DESC'
-        }
+        "metadata": {"type": "Liveboard", "name_pattern": "DEV_%"},
+        "create_by_user_identifiers": ["admin_a", "admin_b"],
+        "sort_options": {"field_name": "MODIFIED", "order": "DESC"},
     }
 
-    endpoint = 'metadata/search'
-    url = '{}/api/rest/{}/{}'.format(thoughtspot_server, '2.0', endpoint)
+    endpoint = "metadata/search"
+    url = "{}/api/rest/{}/{}".format(thoughtspot_server, "2.0", endpoint)
     response = requests_session.post(url=url, json=metadata_search_request)
 
     for item in response:
-        guid = item['metadata_identifier']
+        guid = item["metadata_identifier"]
         # even more details in
-        headers = item['metadata_header']
+        headers = item["metadata_header"]
         # headers['authorName']
         # headers['tags']
         break
 
     # Once you have a GUID, you can request the TML object
 
     # Set here manually, if you wanted to do repeated actions put in the loop above going through the search_response
-    guid_to_retrieve = ''
+    guid_to_retrieve = ""
 
     # This is the "long form". Eventually TYPE should not be required by the API when GUIDs are used (vs. names)
-    md_request = [
-        {
-            'identifier': guid_to_retrieve,
-            'type': 'LIVEBOARD'
-        }
-    ]
+    md_request = [{"identifier": guid_to_retrieve, "type": "LIVEBOARD"}]
 
-    endpoint = 'metadata/search'
-    url = '{}/api/rest/{}/{}'.format(thoughtspot_server, '2.0', endpoint)
+    endpoint = "metadata/search"
+    url = "{}/api/rest/{}/{}".format(thoughtspot_server, "2.0", endpoint)
     tml_response = requests_session.post(url=url, json=md_request)
     # if you only requested 1 item, just access that one item in the List response. Otherwise loop to handle each
-    tml_string = tml_response[0]['edoc']
-    item_info = tml_response[0]['info']  # additional metadata
+    tml_string = tml_response[0]["edoc"]
+    item_info = tml_response[0]["info"]  # additional metadata
 
     # Load from string you know the object type
     tml_obj = Worksheet.loads(tml_string)
 
     # Read from an unknown type TML file using determine_tml_type() helper
     tml_cls = determine_tml_type(info=item_info)
     tml_obj = tml_cls.loads(tml_document=tml_string)
     if type(tml) is Worksheet:
         # Do things specific to the worksheet
         pass
 
 
 # Example of the same workflow from above, using the thoughtspot_rest_api_v1 library
 def retrieve_from_api_with_library():
-    thoughtspot_server = 'https://myinstance.thoughtspot.cloud'
-    username = 'myUsername@company.com'
-    password = 'apassword' # Find another way of storing to actually secure this
+    thoughtspot_server = "https://myinstance.thoughtspot.cloud"
+    username = "myUsername@company.com"
+    password = "apassword"  # Find another way of storing to actually secure this
 
     ts: TSRestApiV2 = TSRestApiV2(server_url=thoughtspot_server)
     try:
         auth_token_response = ts.auth_token_full(username=username, password=password, validity_time_in_sec=3000)
-        ts.bearer_token = auth_token_response['token']
+        ts.bearer_token = auth_token_response["token"]
     except requests.exceptions.HTTPError as e:
         print(e)
         print(e.response.content)
         exit()
 
     metadata_search_request = {
-        'metadata': {
-            'type': 'Liveboard',
-            'name_pattern': "DEV_%"
-        },
-        'create_by_user_identifiers': ['admin_a', 'admin_b'],
-        'sort_options': {
-            'field_name': 'MODIFIED',
-            'order': 'DESC'
-        }
+        "metadata": {"type": "Liveboard", "name_pattern": "DEV_%"},
+        "create_by_user_identifiers": ["admin_a", "admin_b"],
+        "sort_options": {"field_name": "MODIFIED", "order": "DESC"},
     }
     search_response = ts.metadata_search(request=metadata_search_request)
     # Just an example of how to parse through the response for attributes. Identifier (guid) is what you need to
     # retrieve the TML response
     for item in search_response:
-        guid = item['metadata_identifier']
+        guid = item["metadata_identifier"]
         # even more details in
-        headers = item['metadata_header']
+        headers = item["metadata_header"]
         # headers['authorName']
         # headers['tags']
 
         #
         break
 
-
     # Once you have a GUID, you can request the TML object
 
     # Set here manually, if you wanted to do repeated actions put in the loop above going through the search_response
-    guid_to_retrieve = ''
+    guid_to_retrieve = ""
 
     # This is the "long form". Eventually TYPE should not be required by the API when GUIDs are used (vs. names)
-    md_request = [
-        {
-            'identifier': guid_to_retrieve,
-            'type': 'LIVEBOARD'
-        }
-    ]
+    md_request = [{"identifier": guid_to_retrieve, "type": "LIVEBOARD"}]
     tml_response = ts.metadata_tml_export(metadata_ids=[], export_fqn=True, metadata_request=md_request)
     # if you only requested 1 item, just access that one item in the List response. Otherwise loop to handle each
-    tml_string = tml_response[0]['edoc']
-    item_info = tml_response[0]['info']  # additional metadata
+    tml_string = tml_response[0]["edoc"]
+    item_info = tml_response[0]["info"]  # additional metadata
 
     # Load from string you know the object type
     tml_obj = Worksheet.loads(tml_string)
 
     # Read from an unknown type TML file using determine_tml_type() helper
     tml_cls = determine_tml_type(info=item_info)
     tml_obj = tml_cls.loads(tml_document=tml_string)
     if type(tml) is Worksheet:
         # Do things specific to the worksheet
-        pass
+        pass
```

### Comparing `thoughtspot_tml-2.0.8/examples/common_attribute_changes.py` & `thoughtspot_tml-2.0.9/examples/common_attribute_changes.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,32 +4,29 @@
 # Examples of the common attribute changes that people do on the various TML object types
 
 # Not a fully functioning script, but a set of code snippets to be used in your own scripts
 
 # Each example assumes you've created the appropriate TML object using .load() or .loads()
 # see basic_input_output.py and the README for how to get the objects loaded from TML on disk or from API
 
+
 # Modifies the Table object passed in, returns False if no changes were made
 def change_table(t: Table) -> bool:
     # All properties can be accessed based on TML spec: https://docs.thoughtspot.com/cloud/latest/tml#syntax-tables
 
     # Simple map of existing database to new:
-    db_map = {
-        'old_test_db' : 'NEW_TEST_DB',
-        'old_prod_db': 'NEW_PROD_DB'
-    }
+    db_map = {"old_test_db": "NEW_TEST_DB", "old_prod_db": "NEW_PROD_DB"}
 
     # Only process if the database is found in the map
     if t.table.db in db_map:
-
         # If you want to guarantee a newly created Table object when uploading, set the guid to None
         t.guid = None  # Comment out if you are creating an UPDATE or moving to a new ThoughtSpot instance
 
         # connection has two properties, .name and .fqn . FQN takes a GUID (from the 'id' property of the connection)
-        new_conn_guid = 'ddc6a4bc-312c-490d-912b-bd2b60b2ddd8'
+        new_conn_guid = "ddc6a4bc-312c-490d-912b-bd2b60b2ddd8"
         # If using an FQN, you can set name to None.
         t.table.connection.name = None
         t.table.connection.fqn = new_conn_guid
 
         # Alternatively, if there is an FQN present and you just want to switch using name, set fqn property to none
         # t.table.connection.name = '{New Connection Name}'
         # t.table.connection.fqn = None
@@ -42,58 +39,58 @@
         # t.table.db_table  = ''
 
         cols = t.table.columns
         for c in cols:
             # Convert all lower-case column names to upper-case
             c.db_column_name = c.db_column_name.upper()
             # Set to not index if a string
-            if c.data_type == 'VARCHAR':
-                c.index_type = 'DONT_INDEX'
+            if c.data_type == "VARCHAR":
+                c.index_type = "DONT_INDEX"
         return True
 
     else:
         return False
 
 
 def change_worksheet(w: Worksheet):
     # All properties can be accessed based on TML spec: https://docs.thoughtspot.com/cloud/latest/tml#syntax-worksheets
 
     # Most frequent worksheet change is to switch the tables it is connected to
     # The disambiguate() helper function is designed to do this switch
     table_name_to_guid_map = {
-        'table_name_1': '7fd39fdb-9dfe-4954-b5dd-9a5d846085b0',
-        'table_name_2':  '99999999-9999-4999-9999-999999999999'
+        "table_name_1": "7fd39fdb-9dfe-4954-b5dd-9a5d846085b0",
+        "table_name_2": "99999999-9999-4999-9999-999999999999",
     }
     w = disambiguate(w, guid_mapping=table_name_to_guid_map)
 
     # You can also get to any of the columns and manipulate them
     for col in w.worksheet.worksheet_columns:
-
         # If you changed the format of column names in the connected tables, you may need to adjust the ID
         # This is in format <table_path>::<column_id_1> -- table_path defined in Worksheet, but '<column_id_1>' is
         # the 'name' property of the column in the Table object itself
 
         # Here we'll assume we upper-cased the names in the Table, and now must make that update in the Worksheet as well
         col_id = col.column_id
         col_id_split = col_id.split("::")
         col.column_id = "{}::{}".format(col_id_split[0], col_id_split[1].upper())
 
         # Add synonyms
         col.properties.synonyms = col.properties.synonyms + ",new synonym,second synonym"
 
     return True
 
+
 def change_answer(a: Answer):
     # All properties can be accessed based on TML spec: https://docs.thoughtspot.com/cloud/latest/tml#syntax-answers
 
     # Most frequent answer change is to switch the worksheet it is connected to to a different one
     # The disambiguate() helper function is designed to do this switch
     ws_name_to_guid_map = {
-        'ws_name_1': '7fd39fdb-9dfe-4954-b5dd-9a5d846085b0',
-        'ws_name_2':  '99999999-9999-4999-9999-999999999999'
+        "ws_name_1": "7fd39fdb-9dfe-4954-b5dd-9a5d846085b0",
+        "ws_name_2": "99999999-9999-4999-9999-999999999999",
     }
     a = disambiguate(a, guid_mapping=ws_name_to_guid_map)
 
     return True
 
 
 def change_liveboard(lb: Liveboard):
@@ -101,24 +98,22 @@
 
     # Most frequent Liveboard change is to switch the worksheet the vizes in it are connected to
     # Each viz can be connected to different worksheets (or tables) so passing a mapping with all possibilities
     # is the safest way to make this change
 
     # The disambiguate() helper function is designed to do this switch
     ws_name_to_guid_map = {
-        'ws_name_1': '7fd39fdb-9dfe-4954-b5dd-9a5d846085b0',
-        'ws_name_2': '99999999-9999-4999-9999-999999999999'
+        "ws_name_1": "7fd39fdb-9dfe-4954-b5dd-9a5d846085b0",
+        "ws_name_2": "99999999-9999-4999-9999-999999999999",
     }
 
     # You can also make a map that swaps GUID to GUID:
-    ws_guid_to_guid_map = {
-       '7fd39fdb-9dfe-4954-b5dd-9a5d846085b0': '99999999-9999-4999-9999-999999999999'
-    }
+    ws_guid_to_guid_map = {"7fd39fdb-9dfe-4954-b5dd-9a5d846085b0": "99999999-9999-4999-9999-999999999999"}
 
     lb = disambiguate(lb, guid_mapping=ws_name_to_guid_map)
 
     lb.liveboard.description = "Updated description for the liveboard"
 
     # If you want to use to guarantee new object creation on import, delete guid property
     lb.guid = None
 
-    return True
+    return True
```

### Comparing `thoughtspot_tml-2.0.8/examples/worksheet-namespace-remapping/README.md` & `thoughtspot_tml-2.0.9/examples/worksheet-namespace-remapping/README.md`

 * *Files identical despite different names*

### Comparing `thoughtspot_tml-2.0.8/examples/worksheet-namespace-remapping/worksheet_remapping.py` & `thoughtspot_tml-2.0.9/examples/worksheet-namespace-remapping/worksheet_remapping.py`

 * *Files identical despite different names*

### Comparing `thoughtspot_tml-2.0.8/noxfile.py` & `thoughtspot_tml-2.0.9/noxfile.py`

 * *Files identical despite different names*

### Comparing `thoughtspot_tml-2.0.8/pyproject.toml` & `thoughtspot_tml-2.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,11 @@
 [build-system]
 requires = ["setuptools>=42", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
-[tool.setuptools_scm]
-
-[tool.setuptools.packages.find]
-where = ["src"]
-exclude = ["_generate*"]
-
 [project]
 name = "thoughtspot_tml"
 dynamic = ["version"]
 description = "Library for manipulating ThoughtSpot Modeling Language (TML) files"
 readme = "README.md"
 requires-python = ">=3.7 , < 3.12"
 license = {file = "LICENSE"}
@@ -70,14 +64,18 @@
     "coverage[toml]",
 ]
 
 # eventual plans for a jq-like utility for TML
 # [project.scripts]
 # tml = "thoughtspot_tml.cli.main:run"
 
+[tool.setuptools.packages.find]
+where = ["src"]
+exclude = ["_generate*"]
+
 [tool.setuptools.dynamic]
 version = {attr = "thoughtspot_tml._version.__version__"}
 
 [tool.black]
 line-length = 120
 exclude = '''
 (
```

### Comparing `thoughtspot_tml-2.0.8/src/thoughtspot_tml/__init__.py` & `thoughtspot_tml-2.0.9/src/thoughtspot_tml/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,10 +9,22 @@
 from thoughtspot_tml.tml import Connection as EmbraceConnection
 from thoughtspot_tml.tml import View as ThoughtSpotView
 from thoughtspot_tml.tml import Answer as SavedAnswer
 from thoughtspot_tml.tml import Table as SystemTable
 
 
 __all__ = (
-    "__version__", "Connection", "Table", "View", "SQLView", "Worksheet", "Answer", "Liveboard", "Pinboard", "SpotApp",
-    "EmbraceConnection", "ThoughtSpotView", "SavedAnswer", "SystemTable",
+    "__version__",
+    "Connection",
+    "Table",
+    "View",
+    "SQLView",
+    "Worksheet",
+    "Answer",
+    "Liveboard",
+    "Pinboard",
+    "SpotApp",
+    "EmbraceConnection",
+    "ThoughtSpotView",
+    "SavedAnswer",
+    "SystemTable",
 )
```

### Comparing `thoughtspot_tml-2.0.8/src/thoughtspot_tml/_compat.py` & `thoughtspot_tml-2.0.9/src/thoughtspot_tml/_compat.py`

 * *Files identical despite different names*

### Comparing `thoughtspot_tml-2.0.8/src/thoughtspot_tml/_scriptability.py` & `thoughtspot_tml-2.0.9/src/thoughtspot_tml/_scriptability.py`

 * *Files identical despite different names*

### Comparing `thoughtspot_tml-2.0.8/src/thoughtspot_tml/_tml.py` & `thoughtspot_tml-2.0.9/src/thoughtspot_tml/_tml.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,15 +87,14 @@
 def _recursive_remove_null(mapping: Dict[str, Any]) -> Dict[str, Any]:
     """
     Drop all keys with null values, they're optional.
     """
     new = {}
 
     for k, v in mapping.items():
-
         if isinstance(v, dict):
             v = _recursive_remove_null(v)
 
         if isinstance(v, list):
             v = [_recursive_remove_null(e) if isinstance(e, dict) else e for e in v if e is not None]
 
         # if v is an empty collection, discard it
@@ -175,15 +174,15 @@
         ------
         TMLDecodeError, when the document string cannot be parsed or receives extra data
         """
         if isinstance(path, str):
             path = pathlib.Path(path)
 
         try:
-            instance = cls.loads(path.read_text())
+            instance = cls.loads(path.read_text(encoding="utf-8"))
         except TMLDecodeError as e:
             e.path = path
             raise e from None
 
         return instance
 
     def to_dict(self) -> Dict[str, Any]:
@@ -224,12 +223,14 @@
           filepath to save the TML document to
         """
         if isinstance(path, str):
             path = pathlib.Path(path)
 
         if not path.name.endswith(".json") and not path.name.endswith(f"{self.tml_type_name}.tml"):
             warnings.warn(
-                f"saving to '{path}', expected {path.stem}.{self.tml_type_name}.tml", TMLExtensionWarning, stacklevel=2,
+                f"saving to '{path}', expected {path.stem}.{self.tml_type_name}.tml",
+                TMLExtensionWarning,
+                stacklevel=2,
             )
 
         document = self.dumps(format_type="JSON" if ".json" in path.suffix.lower() else "YAML")
-        path.write_text(document)
+        path.write_text(document, encoding="utf-8")
```

### Comparing `thoughtspot_tml-2.0.8/src/thoughtspot_tml/_yaml.py` & `thoughtspot_tml-2.0.9/src/thoughtspot_tml/_yaml.py`

 * *Files identical despite different names*

### Comparing `thoughtspot_tml-2.0.8/src/thoughtspot_tml/exceptions.py` & `thoughtspot_tml-2.0.9/src/thoughtspot_tml/exceptions.py`

 * *Files identical despite different names*

### Comparing `thoughtspot_tml-2.0.8/src/thoughtspot_tml/spotapp.py` & `thoughtspot_tml-2.0.9/src/thoughtspot_tml/spotapp.py`

 * *Files identical despite different names*

### Comparing `thoughtspot_tml-2.0.8/src/thoughtspot_tml/tml.py` & `thoughtspot_tml-2.0.9/src/thoughtspot_tml/tml.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 
 @dataclass
 class Connection(_tml.TML):
     """
     Representation of a ThoughtSpot System Table TML.
     """
+
     guid: Optional[GUID]
     connection: _scriptability.ConnectionDoc
 
     @property
     def name(self) -> str:
         return self.connection.name
 
@@ -52,26 +53,30 @@
 
     def to_rest_api_v1_metadata(self) -> ConnectionMetadata:
         """
         Return a mapping of configuration attributes, as well as database, schema, and table objects.
 
         The `connection/update` REST API endpoint requires a `metadata` parameter.
         """
-        data: ConnectionMetadata = {"configuration": {kv.key: kv.value for kv in self.connection.properties}, "externalDatabases": []}  # noqa: E501
+        data: ConnectionMetadata = {
+            "configuration": {kv.key: kv.value for kv in self.connection.properties},
+            "externalDatabases": [],
+        }
         this_database: ExternalDatabase = {"name": None, "isAutoCreated": False, "schemas": []}
         this_schema: ExternalSchema = {"name": None, "tables": []}
 
         # this connection has 0 tables (very popular "initial state" structure TS 9.0.0+)
         if self.connection.table is None:
             return data
 
         # external_databases are nested dict of list of dict.. database -> schema -> table -> columns
         # if we sort first, we can guarantee the insertion order with simple iteration
-        for table in sorted(self.connection.table, key=lambda t: (t.external_table.db_name, t.external_table.schema_name)):  # noqa: E501
-
+        for table in sorted(
+            self.connection.table, key=lambda t: (t.external_table.db_name, t.external_table.schema_name),
+        ):
             # if it's a new schema, append it this database's schema and reset
             if table.external_table.schema_name != this_schema["name"]:
                 if this_schema["name"] is not None:
                     this_database["schemas"].append(copy.deepcopy(this_schema))
 
                 this_schema["name"] = table.external_table.schema_name
                 this_schema["tables"] = []
@@ -116,79 +121,85 @@
 
 
 @dataclass
 class Table(_tml.TML):
     """
     Representation of a ThoughtSpot System Table TML.
     """
+
     guid: GUID
     table: _scriptability.LogicalTableEDocProto
 
     @property
     def name(self) -> str:
         return self.table.name
 
 
 @dataclass
 class View(_tml.TML):
     """
     Representation of a ThoughtSpot View TML.
     """
+
     guid: GUID
     view: _scriptability.ViewEDocProto
 
     @property
     def name(self) -> str:
         return self.view.name
 
 
 @dataclass
 class SQLView(_tml.TML):
     """
     Representation of a ThoughtSpot SQLView TML.
     """
+
     guid: GUID
     sql_view: _scriptability.SqlViewEDocProto
 
     @property
     def name(self) -> str:
         return self.sql_view.name
 
 
 @dataclass
 class Worksheet(_tml.TML):
     """
     Representation of a ThoughtSpot Worksheet TML.
     """
+
     guid: GUID
     worksheet: _scriptability.WorksheetEDocProto
 
     @property
     def name(self) -> str:
         return self.worksheet.name
 
 
 @dataclass
 class Answer(_tml.TML):
     """
     Representation of a ThoughtSpot Answer TML.
     """
+
     guid: GUID
     answer: _scriptability.AnswerEDocProto
 
     @property
     def name(self) -> str:
         return self.answer.name
 
 
 @dataclass
 class Liveboard(_tml.TML):
     """
     Representation of a ThoughtSpot Liveboard TML.
     """
+
     guid: GUID
     liveboard: _scriptability.PinboardEDocProto
 
     @property
     def name(self) -> str:
         return self.liveboard.name
 
@@ -208,14 +219,15 @@
 class Pinboard(_tml.TML):
     """
     Representation of a ThoughtSpot Pinboard TML.
 
     DEPRECATED :: https://docs.thoughtspot.com/software/latest/deprecation
       As part of the May 2022 ThoughtSpot release, we rebranded pinboards as Liveboards.
     """
+
     guid: GUID
     pinboard: _scriptability.PinboardEDocProto
 
     @property
     def name(self) -> str:
         return self.pinboard.name
```

### Comparing `thoughtspot_tml-2.0.8/src/thoughtspot_tml/types.py` & `thoughtspot_tml-2.0.9/src/thoughtspot_tml/types.py`

 * *Files identical despite different names*

### Comparing `thoughtspot_tml-2.0.8/src/thoughtspot_tml/utils.py` & `thoughtspot_tml-2.0.9/src/thoughtspot_tml/utils.py`

 * *Files identical despite different names*

### Comparing `thoughtspot_tml-2.0.8/src/thoughtspot_tml.egg-info/PKG-INFO` & `thoughtspot_tml-2.0.9/src/thoughtspot_tml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thoughtspot-tml
-Version: 2.0.8
+Version: 2.0.9
 Summary: Library for manipulating ThoughtSpot Modeling Language (TML) files
 Author-email: Bryant Howell <bryant.howell@thoughtspot.com>, Bill B <bill.back@thoughtspot.com>, boonhapus <nicholas.cooper@thoughtspot.com>
 Maintainer-email: Bryant Howell <bryant.howell@thoughtspot.com>, boonhapus <nicholas.cooper@thoughtspot.com>
 License: #ThoughtSpot Development Tools End User License Agreement
         
         THIS THOUGHTSPOT DEVELOPMENT TOOLS END USER LICENSE AGREEMENT (“EULA”) FORMS A BINDING AGREEMENT BETWEEN YOU INDIVIDUALLY OR THE BUSINESS ENTITY OR PUBLIC AGENCY ON WHOSE BEHALF YOU ARE ACCEPTING THIS AGREEMENT (“COMPANY”) AND THOUGHTSPOT, INC. (“THOUGHTSPOT”). THIS EULA DESCRIBES THE RIGHTS AND OBLIGATIONS OF COMPANY AND THOUGHTSPOT GOVERNING THE USE OF ANY APPLICATION PROGRAMMING INTERFACE, CONNECTOR, SOFTWARE DEVELOPMENT KIT, CODE SNIPPET, SAMPLE CODE, FREE CUSTOM USER INTERFACE OR VISUALIZATION, SAMPLE DATA, AND THE CORRESPONDING DOCUMENTATION FOR EACH, ANY UPDATES AND UPGRADES THERETO, AND ANY MODIFICATIONS, ENHANCEMENTS, OR IMPROVEMENTS, OF ANY OF THE FOREGOING, MADE AVAILABLE BY THOUGHTSPOT TOGETHER WITH THIS EULA (EACH A “TOOL” AND COLLECTIVELY “TOOLS”).
         
@@ -74,14 +74,17 @@
 Requires-Dist: coverage[toml]; extra == "dev"
 
 <div align="center">
   <h2><b>ThoughtSpot TML</b></h2>
 
   <i>a Python package for working with</i> <b>ThoughtSpot</b> <i>Modeling Language (TML) files programmatically</i>
 
+  ![Badge: Lint](https://github.com/thoughtspot/thoughtspot_tml/actions/workflows/lint.yml/badge.svg)
+  ![Badge: Test](https://github.com/thoughtspot/thoughtspot_tml/actions/workflows/test.yml/badge.svg)
+  
   <h3>
     <a href="#installation">Installation</a>
     <span> | </span>
     <a href="#a-basic-example">Example</a>
     <span> | </span>
     <a href="#migration-to-v200">Migration to v2.0.0</a>
     <span> | </span>
```

### Comparing `thoughtspot_tml-2.0.8/src/thoughtspot_tml.egg-info/SOURCES.txt` & `thoughtspot_tml-2.0.9/src/thoughtspot_tml.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -54,9 +54,10 @@
 tests/data/DUMMY.pinboard.tml
 tests/data/DUMMY.sql_view.tml
 tests/data/DUMMY.table.tml
 tests/data/DUMMY.view.tml
 tests/data/DUMMY.worksheet.tml
 tests/data/DUMMY_spot_app.zip
 tests/data/SPECIAL_TABLE.table.tml
+tests/data/SPECIAL_UNICODE_TABLE.table.tml
 tests/data/connection.yaml
 tests/data/_temp/.gitdontignore
```

### Comparing `thoughtspot_tml-2.0.8/tests/_const.py` & `thoughtspot_tml-2.0.9/tests/_const.py`

 * *Files identical despite different names*

### Comparing `thoughtspot_tml-2.0.8/tests/data/DUMMY.answer.tml` & `thoughtspot_tml-2.0.9/tests/data/DUMMY.answer.tml`

 * *Files identical despite different names*

### Comparing `thoughtspot_tml-2.0.8/tests/data/DUMMY.connection.tml` & `thoughtspot_tml-2.0.9/tests/data/DUMMY.connection.tml`

 * *Files identical despite different names*

### Comparing `thoughtspot_tml-2.0.8/tests/data/DUMMY.liveboard.tml` & `thoughtspot_tml-2.0.9/tests/data/DUMMY.liveboard.tml`

 * *Files identical despite different names*

### Comparing `thoughtspot_tml-2.0.8/tests/data/DUMMY.pinboard.tml` & `thoughtspot_tml-2.0.9/tests/data/DUMMY.pinboard.tml`

 * *Files identical despite different names*

### Comparing `thoughtspot_tml-2.0.8/tests/data/DUMMY.sql_view.tml` & `thoughtspot_tml-2.0.9/tests/data/DUMMY.sql_view.tml`

 * *Files identical despite different names*

### Comparing `thoughtspot_tml-2.0.8/tests/data/DUMMY.table.tml` & `thoughtspot_tml-2.0.9/tests/data/DUMMY.table.tml`

 * *Files identical despite different names*

### Comparing `thoughtspot_tml-2.0.8/tests/data/DUMMY.view.tml` & `thoughtspot_tml-2.0.9/tests/data/DUMMY.view.tml`

 * *Files identical despite different names*

### Comparing `thoughtspot_tml-2.0.8/tests/data/DUMMY.worksheet.tml` & `thoughtspot_tml-2.0.9/tests/data/DUMMY.worksheet.tml`

 * *Files identical despite different names*

### Comparing `thoughtspot_tml-2.0.8/tests/data/DUMMY_spot_app.zip` & `thoughtspot_tml-2.0.9/tests/data/DUMMY_spot_app.zip`

 * *Files identical despite different names*

### Comparing `thoughtspot_tml-2.0.8/tests/data/SPECIAL_TABLE.table.tml` & `thoughtspot_tml-2.0.9/tests/data/SPECIAL_TABLE.table.tml`

 * *Files identical despite different names*

### Comparing `thoughtspot_tml-2.0.8/tests/data/connection.yaml` & `thoughtspot_tml-2.0.9/tests/data/connection.yaml`

 * *Files identical despite different names*

### Comparing `thoughtspot_tml-2.0.8/tests/test_connection.py` & `thoughtspot_tml-2.0.9/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `thoughtspot_tml-2.0.8/tests/test_exceptions.py` & `thoughtspot_tml-2.0.9/tests/test_exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from ward import test, raises
 
 from . import _const
 
 
 @test("TMLDecodeError on text input")
 def _():
-
     with raises(TMLDecodeError) as exc:
         Answer.loads(tml_document="😅: INVALID")
 
     assert "supplied data does not produce a valid TML (Answer) document" in str(exc.raised)
 
 
 @test("TMLDecodeError on invalid file input")
```

### Comparing `thoughtspot_tml-2.0.8/tests/test_spotapp.py` & `thoughtspot_tml-2.0.9/tests/test_spotapp.py`

 * *Files identical despite different names*

### Comparing `thoughtspot_tml-2.0.8/tests/test_tml.py` & `thoughtspot_tml-2.0.9/tests/test_tml.py`

 * *Files identical despite different names*

### Comparing `thoughtspot_tml-2.0.8/tests/test_util.py` & `thoughtspot_tml-2.0.9/tests/test_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 
 from thoughtspot_tml.exceptions import TMLError
 from thoughtspot_tml.types import GUID
 from thoughtspot_tml.utils import determine_tml_type, disambiguate, EnvironmentGUIDMapper
-from thoughtspot_tml.utils import _recursive_scan #, _import_sort_order
+from thoughtspot_tml.utils import _recursive_scan  # , _import_sort_order
 from thoughtspot_tml.tml import Connection
 from thoughtspot_tml.tml import Table, View, SQLView, Worksheet
 from thoughtspot_tml.tml import Answer, Liveboard, Pinboard
 from thoughtspot_tml import _scriptability
 from ward import test, raises
 
 from . import _const
@@ -38,15 +38,14 @@
         determine_tml_type(info={"type": bad_type})
 
     assert f"could not parse TML type from 'info' or 'path', got '{bad_type}'" in str(exc.raised)
 
 
 @test("object utility requires one of: 'info' or 'path'")
 def _():
-
     with raises(TypeError) as exc:
         determine_tml_type()
 
     assert str(exc.raised) == "determine_tml_type() missing at least 1 required keyword-only argument: 'info' or 'path'"
 
 
 for method, envt in (
@@ -162,14 +161,15 @@
 
         tml = disambiguate(tml, guid_mapping={to_replace: FAKE_GUID})
 
         identities = _recursive_scan(tml, check=lambda x: isinstance(x, _scriptability.Identity))
         assert len(identities) >= n_replacements
         assert len([i for i in identities if i.fqn == FAKE_GUID]) == n_replacements
 
+
 @test("return a mapping iterator for two environements")
 def _():
     mapper = EnvironmentGUIDMapper(str.upper)
 
     guid_to_guid_mappings = {
         GUID("123e4567-e89b-12d3-a456-426655440000"): GUID("234e5678-f9ab-12d3-b456-526665550000"),
         GUID("345e6789-0abc-12d3-c456-626675560000"): GUID("456e789a-1bcd-12d3-d456-726685570000"),
@@ -182,17 +182,17 @@
     }
 
     for source_guid, dest_guid in guid_to_guid_mappings.items():
         mapper[source_guid] = ("source", source_guid)
         mapper[source_guid] = ("dest", dest_guid)
 
     mappings = mapper.generate_mapping("source", "dest")
-    assert(len(mappings) == 8)
+    assert len(mappings) == 8
     for g1, g2 in mappings.items():
-        assert(g2 == guid_to_guid_mappings[g1])
+        assert g2 == guid_to_guid_mappings[g1]
 
 
 # @test("raise on ambiguous TML input")
 # def _():
 #     tmls = [
 #         determine_tml_type(path=_const.DUMMY_TABLE).load(path=_const.DUMMY_TABLE),
 #         determine_tml_type(path=_const.DUMMY_VIEW).load(path=_const.DUMMY_VIEW),
```

### Comparing `thoughtspot_tml-2.0.8/tests/test_view.py` & `thoughtspot_tml-2.0.9/tests/test_view.py`

 * *Files identical despite different names*

### Comparing `thoughtspot_tml-2.0.8/tests/test_worksheet.py` & `thoughtspot_tml-2.0.9/tests/test_worksheet.py`

 * *Files identical despite different names*

