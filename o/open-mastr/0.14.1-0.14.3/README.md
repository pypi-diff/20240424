# Comparing `tmp/open_mastr-0.14.1.tar.gz` & `tmp/open_mastr-0.14.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_mastr-0.14.1.tar", last modified: Wed Jan 17 16:16:15 2024, max compression
+gzip compressed data, was "open_mastr-0.14.3.tar", last modified: Wed Apr 24 11:28:13 2024, max compression
```

## Comparing `open_mastr-0.14.1.tar` & `open_mastr-0.14.3.tar`

### file list

```diff
@@ -1,45 +1,196 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 16:16:15.563893 open_mastr-0.14.1/
--rw-r--r--   0 runner    (1001) docker     (127)    34521 2024-01-17 16:16:08.000000 open_mastr-0.14.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     9184 2024-01-17 16:16:15.563893 open_mastr-0.14.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7128 2024-01-17 16:16:08.000000 open_mastr-0.14.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 16:16:15.555893 open_mastr-0.14.1/open_mastr/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-01-17 16:16:08.000000 open_mastr-0.14.1/open_mastr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16679 2024-01-17 16:16:08.000000 open_mastr-0.14.1/open_mastr/mastr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 16:16:15.555893 open_mastr-0.14.1/open_mastr/soap_api/
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-01-17 16:16:08.000000 open_mastr-0.14.1/open_mastr/soap_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48325 2024-01-17 16:16:08.000000 open_mastr-0.14.1/open_mastr/soap_api/download.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 16:16:15.555893 open_mastr-0.14.1/open_mastr/soap_api/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-01-17 16:16:08.000000 open_mastr-0.14.1/open_mastr/soap_api/metadata/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 16:16:08.000000 open_mastr-0.14.1/open_mastr/soap_api/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15770 2024-01-17 16:16:08.000000 open_mastr-0.14.1/open_mastr/soap_api/metadata/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     7990 2024-01-17 16:16:08.000000 open_mastr-0.14.1/open_mastr/soap_api/metadata/description.py
--rw-r--r--   0 runner    (1001) docker     (127)    41996 2024-01-17 16:16:08.000000 open_mastr-0.14.1/open_mastr/soap_api/mirror.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-01-17 16:16:08.000000 open_mastr-0.14.1/open_mastr/soap_api/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-01-17 16:16:08.000000 open_mastr-0.14.1/open_mastr/soap_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 16:16:15.559893 open_mastr-0.14.1/open_mastr/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 16:16:08.000000 open_mastr-0.14.1/open_mastr/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 16:16:15.559893 open_mastr-0.14.1/open_mastr/utils/config/
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-01-17 16:16:08.000000 open_mastr-0.14.1/open_mastr/utils/config/logging.yml
--rw-r--r--   0 runner    (1001) docker     (127)     9476 2024-01-17 16:16:08.000000 open_mastr-0.14.1/open_mastr/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    21765 2024-01-17 16:16:08.000000 open_mastr-0.14.1/open_mastr/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6749 2024-01-17 16:16:08.000000 open_mastr-0.14.1/open_mastr/utils/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-01-17 16:16:08.000000 open_mastr-0.14.1/open_mastr/utils/docs.py
--rw-r--r--   0 runner    (1001) docker     (127)    27609 2024-01-17 16:16:08.000000 open_mastr-0.14.1/open_mastr/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    36349 2024-01-17 16:16:08.000000 open_mastr-0.14.1/open_mastr/utils/orm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 16:16:15.559893 open_mastr-0.14.1/open_mastr/xml_download/
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-01-17 16:16:08.000000 open_mastr-0.14.1/open_mastr/xml_download/colums_to_replace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-01-17 16:16:08.000000 open_mastr-0.14.1/open_mastr/xml_download/utils_cleansing_bulk.py
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-01-17 16:16:08.000000 open_mastr-0.14.1/open_mastr/xml_download/utils_download_bulk.py
--rw-r--r--   0 runner    (1001) docker     (127)    12986 2024-01-17 16:16:08.000000 open_mastr-0.14.1/open_mastr/xml_download/utils_write_to_database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 16:16:15.559893 open_mastr-0.14.1/open_mastr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9184 2024-01-17 16:16:15.000000 open_mastr-0.14.1/open_mastr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-01-17 16:16:15.000000 open_mastr-0.14.1/open_mastr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-17 16:16:15.000000 open_mastr-0.14.1/open_mastr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-01-17 16:16:15.000000 open_mastr-0.14.1/open_mastr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-17 16:16:15.000000 open_mastr-0.14.1/open_mastr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-01-17 16:16:15.563893 open_mastr-0.14.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-01-17 16:16:08.000000 open_mastr-0.14.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 16:16:15.559893 open_mastr-0.14.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-01-17 16:16:08.000000 open_mastr-0.14.1/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    12579 2024-01-17 16:16:08.000000 open_mastr-0.14.1/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-01-17 16:16:08.000000 open_mastr-0.14.1/tests/test_mastr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:28:13.359331 open_mastr-0.14.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-24 11:28:06.000000 open_mastr-0.14.3/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-24 11:28:06.000000 open_mastr-0.14.3/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-24 11:28:06.000000 open_mastr-0.14.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:28:13.267331 open_mastr-0.14.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:28:13.267331 open_mastr-0.14.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-24 11:28:06.000000 open_mastr-0.14.3/.github/ISSUE_TEMPLATE/issue_template_bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-24 11:28:06.000000 open_mastr-0.14.3/.github/ISSUE_TEMPLATE/issue_template_feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-24 11:28:06.000000 open_mastr-0.14.3/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:28:13.267331 open_mastr-0.14.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-24 11:28:06.000000 open_mastr-0.14.3/.github/workflows/ci-develop.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-24 11:28:06.000000 open_mastr-0.14.3/.github/workflows/ci-production.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-24 11:28:06.000000 open_mastr-0.14.3/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-24 11:28:06.000000 open_mastr-0.14.3/.github/workflows/test-pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-24 11:28:06.000000 open_mastr-0.14.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-24 11:28:06.000000 open_mastr-0.14.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-24 11:28:06.000000 open_mastr-0.14.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    16526 2024-04-24 11:28:06.000000 open_mastr-0.14.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-24 11:28:06.000000 open_mastr-0.14.3/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     6834 2024-04-24 11:28:06.000000 open_mastr-0.14.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    34521 2024-04-24 11:28:06.000000 open_mastr-0.14.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    49323 2024-04-24 11:28:13.359331 open_mastr-0.14.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7172 2024-04-24 11:28:06.000000 open_mastr-0.14.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-04-24 11:28:06.000000 open_mastr-0.14.3/RELEASE_PROCEDURE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:28:13.271330 open_mastr-0.14.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:28:13.271330 open_mastr-0.14.3/docs/_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:28:13.271330 open_mastr-0.14.3/docs/_data/raw/
+-rw-r--r--   0 runner    (1001) docker     (127)    11186 2024-04-24 11:28:06.000000 open_mastr-0.14.3/docs/_data/raw/bnetza_mastr_biomass_raw.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    11192 2024-04-24 11:28:06.000000 open_mastr-0.14.3/docs/_data/raw/bnetza_mastr_combustion_raw.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     9643 2024-04-24 11:28:06.000000 open_mastr-0.14.3/docs/_data/raw/bnetza_mastr_gsgk_raw.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     9348 2024-04-24 11:28:06.000000 open_mastr-0.14.3/docs/_data/raw/bnetza_mastr_hydro_raw.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     7805 2024-04-24 11:28:06.000000 open_mastr-0.14.3/docs/_data/raw/bnetza_mastr_nuclear_raw.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10941 2024-04-24 11:28:06.000000 open_mastr-0.14.3/docs/_data/raw/bnetza_mastr_solar_raw.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     9760 2024-04-24 11:28:06.000000 open_mastr-0.14.3/docs/_data/raw/bnetza_mastr_storage_raw.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    11758 2024-04-24 11:28:06.000000 open_mastr-0.14.3/docs/_data/raw/bnetza_mastr_wind_raw.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-24 11:28:06.000000 open_mastr-0.14.3/docs/_data/raw_data.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:28:13.271330 open_mastr-0.14.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-24 11:28:06.000000 open_mastr-0.14.3/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)    18422 2024-04-24 11:28:06.000000 open_mastr-0.14.3/docs/advanced.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-24 11:28:06.000000 open_mastr-0.14.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-24 11:28:06.000000 open_mastr-0.14.3/docs/data-release-notes.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6014 2024-04-24 11:28:06.000000 open_mastr-0.14.3/docs/dataset.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:28:13.271330 open_mastr-0.14.3/docs/development/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-24 11:28:06.000000 open_mastr-0.14.3/docs/development/changelog_mirror.md
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-24 11:28:06.000000 open_mastr-0.14.3/docs/development/contributing_mirror.md
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-24 11:28:06.000000 open_mastr-0.14.3/docs/development/release_procedure_mirror.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-04-24 11:28:06.000000 open_mastr-0.14.3/docs/getting_started.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:28:13.275330 open_mastr-0.14.3/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    68299 2024-04-24 11:28:06.000000 open_mastr-0.14.3/docs/images/DBBrowser.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)   116772 2024-04-24 11:28:06.000000 open_mastr-0.14.3/docs/images/DetailAnlagenModellMaStR.png
+-rw-r--r--   0 runner    (1001) docker     (127)   325132 2024-04-24 11:28:06.000000 open_mastr-0.14.3/docs/images/DetailAnlagen_english.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)    53860 2024-04-24 11:28:06.000000 open_mastr-0.14.3/docs/images/MaStR_Mirror.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11951 2024-04-24 11:28:06.000000 open_mastr-0.14.3/docs/images/MaStR_downloading.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    63845 2024-04-24 11:28:06.000000 open_mastr-0.14.3/docs/images/ObjektmodellMaStR.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23940 2024-04-24 11:28:06.000000 open_mastr-0.14.3/docs/images/OpenEnergyFamily_Logo_OpenMaStR_no_name_grey.png
+-rw-r--r--   0 runner    (1001) docker     (127)    30513 2024-04-24 11:28:06.000000 open_mastr-0.14.3/docs/images/OpenEnergyFamily_Logo_OpenMaStR_no_name_white.png
+-rw-r--r--   0 runner    (1001) docker     (127)    35337 2024-04-24 11:28:06.000000 open_mastr-0.14.3/docs/images/OpenEnergyFamily_Logo_OpenMaStR_white.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-24 11:28:06.000000 open_mastr-0.14.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)   161194 2024-04-24 11:28:06.000000 open_mastr-0.14.3/docs/mastr_structure.graphml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:28:13.275330 open_mastr-0.14.3/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-24 11:28:06.000000 open_mastr-0.14.3/docs/reference/advanced.md
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-24 11:28:06.000000 open_mastr-0.14.3/docs/reference/basic.md
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-24 11:28:06.000000 open_mastr-0.14.3/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-24 11:28:06.000000 open_mastr-0.14.3/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-24 11:28:06.000000 open_mastr-0.14.3/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-24 11:28:06.000000 open_mastr-0.14.3/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:28:13.275330 open_mastr-0.14.3/open_mastr/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-24 11:28:06.000000 open_mastr-0.14.3/open_mastr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16683 2024-04-24 11:28:06.000000 open_mastr-0.14.3/open_mastr/mastr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:28:13.275330 open_mastr-0.14.3/open_mastr/soap_api/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-24 11:28:06.000000 open_mastr-0.14.3/open_mastr/soap_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49168 2024-04-24 11:28:06.000000 open_mastr-0.14.3/open_mastr/soap_api/download.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:28:13.279330 open_mastr-0.14.3/open_mastr/soap_api/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-24 11:28:06.000000 open_mastr-0.14.3/open_mastr/soap_api/metadata/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 11:28:06.000000 open_mastr-0.14.3/open_mastr/soap_api/metadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:28:13.279330 open_mastr-0.14.3/open_mastr/soap_api/metadata/archiv/
+-rw-r--r--   0 runner    (1001) docker     (127)    21554 2024-04-24 11:28:06.000000 open_mastr-0.14.3/open_mastr/soap_api/metadata/archiv/mastr_biomass_oem140.json
+-rw-r--r--   0 runner    (1001) docker     (127)    88432 2024-04-24 11:28:06.000000 open_mastr-0.14.3/open_mastr/soap_api/metadata/archiv/mastr_datapackage_oem140.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20495 2024-04-24 11:28:06.000000 open_mastr-0.14.3/open_mastr/soap_api/metadata/archiv/mastr_hydro_oem140.json
+-rw-r--r--   0 runner    (1001) docker     (127)    22621 2024-04-24 11:28:06.000000 open_mastr-0.14.3/open_mastr/soap_api/metadata/archiv/mastr_nuclear_oem140.json
+-rw-r--r--   0 runner    (1001) docker     (127)    22680 2024-04-24 11:28:06.000000 open_mastr-0.14.3/open_mastr/soap_api/metadata/archiv/mastr_solar_oem140.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18919 2024-04-24 11:28:06.000000 open_mastr-0.14.3/open_mastr/soap_api/metadata/archiv/mastr_storage_oem140.json
+-rw-r--r--   0 runner    (1001) docker     (127)    22500 2024-04-24 11:28:06.000000 open_mastr-0.14.3/open_mastr/soap_api/metadata/archiv/mastr_wind_oem140.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15770 2024-04-24 11:28:06.000000 open_mastr-0.14.3/open_mastr/soap_api/metadata/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7990 2024-04-24 11:28:06.000000 open_mastr-0.14.3/open_mastr/soap_api/metadata/description.py
+-rw-r--r--   0 runner    (1001) docker     (127)   810299 2024-04-24 11:28:06.000000 open_mastr-0.14.3/open_mastr/soap_api/metadata/mastr_datapackage.json
+-rw-r--r--   0 runner    (1001) docker     (127)    42701 2024-04-24 11:28:06.000000 open_mastr-0.14.3/open_mastr/soap_api/mirror.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-24 11:28:06.000000 open_mastr-0.14.3/open_mastr/soap_api/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-24 11:28:06.000000 open_mastr-0.14.3/open_mastr/soap_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:28:13.279330 open_mastr-0.14.3/open_mastr/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 11:28:06.000000 open_mastr-0.14.3/open_mastr/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:28:13.279330 open_mastr-0.14.3/open_mastr/utils/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-24 11:28:06.000000 open_mastr-0.14.3/open_mastr/utils/config/logging.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     9476 2024-04-24 11:28:06.000000 open_mastr-0.14.3/open_mastr/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22262 2024-04-24 11:28:06.000000 open_mastr-0.14.3/open_mastr/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6749 2024-04-24 11:28:06.000000 open_mastr-0.14.3/open_mastr/utils/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-24 11:28:06.000000 open_mastr-0.14.3/open_mastr/utils/docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27609 2024-04-24 11:28:06.000000 open_mastr-0.14.3/open_mastr/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37025 2024-04-24 11:28:06.000000 open_mastr-0.14.3/open_mastr/utils/orm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:28:13.283331 open_mastr-0.14.3/open_mastr/xml_download/
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-24 11:28:06.000000 open_mastr-0.14.3/open_mastr/xml_download/colums_to_replace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-24 11:28:06.000000 open_mastr-0.14.3/open_mastr/xml_download/utils_cleansing_bulk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-04-24 11:28:06.000000 open_mastr-0.14.3/open_mastr/xml_download/utils_download_bulk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13391 2024-04-24 11:28:06.000000 open_mastr-0.14.3/open_mastr/xml_download/utils_write_to_database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:28:13.355331 open_mastr-0.14.3/open_mastr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    49323 2024-04-24 11:28:13.000000 open_mastr-0.14.3/open_mastr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6292 2024-04-24 11:28:13.000000 open_mastr-0.14.3/open_mastr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 11:28:13.000000 open_mastr-0.14.3/open_mastr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-24 11:28:13.000000 open_mastr-0.14.3/open_mastr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-24 11:28:13.000000 open_mastr-0.14.3/open_mastr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:28:13.335331 open_mastr-0.14.3/postprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)    72938 2024-04-24 11:28:06.000000 open_mastr-0.14.3/postprocessing/BNetzA_MaStR_API.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  4242026 2024-04-24 11:28:06.000000 open_mastr-0.14.3/postprocessing/OEP-oedialect_MaStR_analyse.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  2206314 2024-04-24 11:28:06.000000 open_mastr-0.14.3/postprocessing/OEP-oedialect_MaStR_region.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   133039 2024-04-24 11:28:06.000000 open_mastr-0.14.3/postprocessing/OEP_MaStR_OPSD_Comparison.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  1554475 2024-04-24 11:28:06.000000 open_mastr-0.14.3/postprocessing/OEP_MaStR_analyze.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    16796 2024-04-24 11:28:06.000000 open_mastr-0.14.3/postprocessing/OEP_MaStR_cleaning.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127) 36893245 2024-04-24 11:28:07.000000 open_mastr-0.14.3/postprocessing/OEP_MaStR_powerunits_analyze.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    15124 2024-04-24 11:28:07.000000 open_mastr-0.14.3/postprocessing/OEP_MaStR_supplement_coords.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 11:28:07.000000 open_mastr-0.14.3/postprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:28:13.339331 open_mastr-0.14.3/postprocessing/db-cleansing/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:28:13.339331 open_mastr-0.14.3/postprocessing/db-cleansing/archiv/
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-04-24 11:28:07.000000 open_mastr-0.14.3/postprocessing/db-cleansing/archiv/open_fred-mastr-biomass-cleansing.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     5311 2024-04-24 11:28:07.000000 open_mastr-0.14.3/postprocessing/db-cleansing/archiv/open_fred-mastr-biomass-cleansing_v2.sql
+-rw-r--r--   0 runner    (1001) docker     (127)    10086 2024-04-24 11:28:07.000000 open_mastr-0.14.3/postprocessing/db-cleansing/archiv/open_fred-mastr-combustion-cleansing_v2.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-24 11:28:07.000000 open_mastr-0.14.3/postprocessing/db-cleansing/archiv/open_fred-mastr-hydro-cleansing.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-04-24 11:28:07.000000 open_mastr-0.14.3/postprocessing/db-cleansing/archiv/open_fred-mastr-hydro-cleansing_v2.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-04-24 11:28:07.000000 open_mastr-0.14.3/postprocessing/db-cleansing/archiv/open_fred-mastr-solar-cleansing.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4710 2024-04-24 11:28:07.000000 open_mastr-0.14.3/postprocessing/db-cleansing/archiv/open_fred-mastr-solar-cleansing_v2.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-04-24 11:28:07.000000 open_mastr-0.14.3/postprocessing/db-cleansing/archiv/open_fred-mastr-wind-cleansing.sql
+-rw-r--r--   0 runner    (1001) docker     (127)    11496 2024-04-24 11:28:07.000000 open_mastr-0.14.3/postprocessing/db-cleansing/archiv/open_fred-mastr-wind-cleansing_v2.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-04-24 11:28:07.000000 open_mastr-0.14.3/postprocessing/db-cleansing/rli-mastr-biomass-cleansing.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     6242 2024-04-24 11:28:07.000000 open_mastr-0.14.3/postprocessing/db-cleansing/rli-mastr-combustion-cleansing.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-24 11:28:07.000000 open_mastr-0.14.3/postprocessing/db-cleansing/rli-mastr-hydro-cleansing.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-04-24 11:28:07.000000 open_mastr-0.14.3/postprocessing/db-cleansing/rli-mastr-solar-cleansing.sql
+-rw-r--r--   0 runner    (1001) docker     (127)    19405 2024-04-24 11:28:07.000000 open_mastr-0.14.3/postprocessing/db-cleansing/rli-mastr-wind-cleansing.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-24 11:28:07.000000 open_mastr-0.14.3/postprocessing/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-24 11:28:07.000000 open_mastr-0.14.3/postprocessing/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12504 2024-04-24 11:28:07.000000 open_mastr-0.14.3/postprocessing/orm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11119 2024-04-24 11:28:07.000000 open_mastr-0.14.3/postprocessing/postprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:28:13.339331 open_mastr-0.14.3/postprocessing/remodel/
+-rw-r--r--   0 runner    (1001) docker     (127)     8107 2024-04-24 11:28:07.000000 open_mastr-0.14.3/postprocessing/remodel/rework_wind.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-24 11:28:07.000000 open_mastr-0.14.3/postprocessing/requirements_pp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-24 11:28:07.000000 open_mastr-0.14.3/postprocessing/turbine_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-04-24 11:28:07.000000 open_mastr-0.14.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:28:13.339331 open_mastr-0.14.3/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)    84559 2024-04-24 11:28:07.000000 open_mastr-0.14.3/scripts/Completeness_test.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    62479 2024-04-24 11:28:07.000000 open_mastr-0.14.3/scripts/Matching coordinates with districts.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:28:13.263330 open_mastr-0.14.3/scripts/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:28:13.343330 open_mastr-0.14.3/scripts/data/VG2500_Districts/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 11:28:07.000000 open_mastr-0.14.3/scripts/data/VG2500_Districts/VG2500_KRS.cpg
+-rw-r--r--   0 runner    (1001) docker     (127)   119202 2024-04-24 11:28:07.000000 open_mastr-0.14.3/scripts/data/VG2500_Districts/VG2500_KRS.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-24 11:28:07.000000 open_mastr-0.14.3/scripts/data/VG2500_Districts/VG2500_KRS.prj
+-rw-r--r--   0 runner    (1001) docker     (127)   993992 2024-04-24 11:28:07.000000 open_mastr-0.14.3/scripts/data/VG2500_Districts/VG2500_KRS.shp
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-24 11:28:07.000000 open_mastr-0.14.3/scripts/data/VG2500_Districts/VG2500_KRS.shx
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 11:28:07.000000 open_mastr-0.14.3/scripts/data/VG2500_Districts/aktualitaet.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   207537 2024-04-24 11:28:07.000000 open_mastr-0.14.3/scripts/data/VG2500_Districts/datenlizenz_deutschland_v2_0_eng.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-24 11:28:07.000000 open_mastr-0.14.3/scripts/data/VG2500_Districts/quellenvermerk_datenlizenz_deutschland.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:28:13.355331 open_mastr-0.14.3/scripts/data/VG5000_Municipalities/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 11:28:07.000000 open_mastr-0.14.3/scripts/data/VG5000_Municipalities/VG5000_GEM.cpg
+-rw-r--r--   0 runner    (1001) docker     (127)  3255026 2024-04-24 11:28:07.000000 open_mastr-0.14.3/scripts/data/VG5000_Municipalities/VG5000_GEM.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-24 11:28:07.000000 open_mastr-0.14.3/scripts/data/VG5000_Municipalities/VG5000_GEM.prj
+-rw-r--r--   0 runner    (1001) docker     (127)  3404636 2024-04-24 11:28:07.000000 open_mastr-0.14.3/scripts/data/VG5000_Municipalities/VG5000_GEM.shp
+-rw-r--r--   0 runner    (1001) docker     (127)    88052 2024-04-24 11:28:07.000000 open_mastr-0.14.3/scripts/data/VG5000_Municipalities/VG5000_GEM.shx
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 11:28:07.000000 open_mastr-0.14.3/scripts/data/VG5000_Municipalities/aktualitaet.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   207537 2024-04-24 11:28:07.000000 open_mastr-0.14.3/scripts/data/VG5000_Municipalities/datenlizenz_deutschland_v2_0_eng.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-24 11:28:07.000000 open_mastr-0.14.3/scripts/data/VG5000_Municipalities/quellenvermerk_datenlizenz_deutschland.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-24 11:28:07.000000 open_mastr-0.14.3/scripts/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:28:13.355331 open_mastr-0.14.3/scripts/map_checker/
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-04-24 11:28:07.000000 open_mastr-0.14.3/scripts/map_checker/DatabaseSynchronizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16018 2024-04-24 11:28:07.000000 open_mastr-0.14.3/scripts/map_checker/MapCheckerApp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6479 2024-04-24 11:28:07.000000 open_mastr-0.14.3/scripts/map_checker/MapCheckerEngine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-24 11:28:07.000000 open_mastr-0.14.3/scripts/map_checker/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-24 11:28:07.000000 open_mastr-0.14.3/scripts/map_checker/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-24 11:28:07.000000 open_mastr-0.14.3/scripts/map_checker/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-24 11:28:07.000000 open_mastr-0.14.3/scripts/mirror_mastr_csv_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-24 11:28:07.000000 open_mastr-0.14.3/scripts/mirror_mastr_dump.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-24 11:28:07.000000 open_mastr-0.14.3/scripts/mirror_mastr_processing_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-24 11:28:07.000000 open_mastr-0.14.3/scripts/mirror_mastr_update_latest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:28:13.355331 open_mastr-0.14.3/scripts/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-04-24 11:28:07.000000 open_mastr-0.14.3/scripts/utils/data_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 11:28:13.359331 open_mastr-0.14.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:28:13.355331 open_mastr-0.14.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 11:28:07.000000 open_mastr-0.14.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-24 11:28:07.000000 open_mastr-0.14.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-24 11:28:07.000000 open_mastr-0.14.3/tests/preparation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:28:13.355331 open_mastr-0.14.3/tests/soap_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     7272 2024-04-24 11:28:07.000000 open_mastr-0.14.3/tests/soap_api/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-24 11:28:07.000000 open_mastr-0.14.3/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12579 2024-04-24 11:28:07.000000 open_mastr-0.14.3/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-24 11:28:07.000000 open_mastr-0.14.3/tests/test_mastr.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-24 11:28:07.000000 open_mastr-0.14.3/tests/test_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:28:13.355331 open_mastr-0.14.3/tests/xml_download/
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-24 11:28:07.000000 open_mastr-0.14.3/tests/xml_download/test_utils_cleansing_bulk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-24 11:28:07.000000 open_mastr-0.14.3/tests/xml_download/test_utils_download_bulk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7468 2024-04-24 11:28:07.000000 open_mastr-0.14.3/tests/xml_download/test_utils_write_to_database.py
```

### Comparing `open_mastr-0.14.1/LICENSE.md` & `open_mastr-0.14.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `open_mastr-0.14.1/PKG-INFO` & `open_mastr-0.14.3/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,7 @@
-Metadata-Version: 2.1
-Name: open_mastr
-Version: 0.14.1
-Summary: A package that provides an interface for downloading and processing the data of the Marktstammdatenregister (MaStR)
-Home-page: https://github.com/OpenEnergyPlatform/open-MaStR
-Download-URL: https://github.com/OpenEnergyPlatform/open-MaStR/archive/refs/tags/v0.14.1.tar.gz
-Author: Open Energy Family
-Author-email: datenzentrum@rl-institut.de
-Maintainer: Ludwig Hülk
-Maintainer-email: datenzentrum@rl-institut.de
-Project-URL: Documentation, https://open-mastr.readthedocs.io/
-Project-URL: Changelog, https://open-mastr.readthedocs.io/en/latest/changelog.html
-Project-URL: Issue Tracker, https://github.com/OpenEnergyPlatform/open-MaStR/issues
-Project-URL: Source, https://github.com/OpenEnergyPlatform/open-MaStR
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8, <4
-Description-Content-Type: text/x-rst
-License-File: LICENSE.md
-Requires-Dist: pandas>=1.4
-Requires-Dist: numpy
-Requires-Dist: sqlalchemy
-Requires-Dist: psycopg2-binary
-Requires-Dist: zeep
-Requires-Dist: tqdm
-Requires-Dist: requests
-Requires-Dist: keyring
-Requires-Dist: tqdm
-Requires-Dist: beautifulsoup4
-Requires-Dist: pyyaml
-Requires-Dist: xmltodict
-Provides-Extra: dev
-Requires-Dist: flake8; extra == "dev"
-Requires-Dist: pylint; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: pytest-dependency; extra == "dev"
-Requires-Dist: xmltodict; extra == "dev"
-Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: bump2version; extra == "dev"
-Requires-Dist: mkdocstrings[python]; extra == "dev"
-Requires-Dist: mkdocs-material; extra == "dev"
-Requires-Dist: mkdocs-include-markdown-plugin; extra == "dev"
-Requires-Dist: mike; extra == "dev"
-
 
 .. image:: https://user-images.githubusercontent.com/14353512/199113556-4b53660f-c628-4138-8d01-3719595ecda1.png
     :align: left
     :target: https://github.com/OpenEnergyPlatform/open-MaStR
     :alt: MaStR logo
 
 ==========
@@ -155,16 +106,16 @@
 ==================
 If you want to see your project in this list, write an  
 `Issue <https://github.com/OpenEnergyPlatform/open-MaStR/issues>`_ or add
 changes in a `Pull Request <https://github.com/OpenEnergyPlatform/open-MaStR/pulls>`_.
 
 - `PV- und Windflächenrechner <https://www.agora-energiewende.de/service/pv-und-windflaechenrechner/>`_
 - `Wasserstoffatlas <https://wasserstoffatlas.de/>`_
-- `EE-Status App <https://ee-status.herokuapp.com/>`_
-
+- `EE-Status App <https://ee-status.de/>`_
+- `Digiplan Anhalt <https://digiplan.rl-institut.de/>`_
 
 
 Collaboration
 =============
 | Everyone is invited to develop this repository with good intentions.
 | Please follow the workflow described in the `CONTRIBUTING.md <https://github.com/OpenEnergyPlatform/open-MaStR/blob/production/CONTRIBUTING.md>`_.
```

### Comparing `open_mastr-0.14.1/open_mastr/mastr.py` & `open_mastr-0.14.3/open_mastr/mastr.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,30 +50,34 @@
 class Mastr:
     """
     `Mastr` is used to download the MaStR database and keep it up-to-date.
 
     A SQL database is used to mirror the MaStR database. It can be filled with
     data either from the MaStR-bulk download or from the MaStR-API.
 
+    !!! example
+
+        ```python
+        from open_mastr import Mastr
+
+        db = Mastr()
+        db.download()
+        ```
+
     Parameters
     ----------
     engine : {'sqlite', sqlalchemy.engine.Engine}, optional
         Defines the engine of the database where the MaStR is mirrored to.
         Default is 'sqlite'.
     connect_to_translated_db: boolean, optional
             Allows connection to an existing translated database. Default is 'False'.
             Only for 'sqlite'-type engines.
 
-    !!! example
-        ```python
-        from open_mastr import Mastr
 
-        db = Mastr()
-        db.download()
-        ```
+
     """
 
     def __init__(self, engine="sqlite", connect_to_translated_db=False) -> None:
 
         validate_parameter_format_for_mastr_init(engine)
 
         self.output_dir = get_output_dir()
```

### Comparing `open_mastr-0.14.1/open_mastr/soap_api/download.py` & `open_mastr-0.14.3/open_mastr/soap_api/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -410,15 +410,22 @@
 
     with open(missed_units_file, "w") as f:
         for i, error in missed_units:
             f.write(f"{i},{error}\n")
 
 
 class MaStRDownload:
-    """Use the higher level interface for bulk download
+    """
+    !!! warning
+
+        **This class is deprecated** and will not be maintained from version 0.15.0 onwards.
+        Instead use [`Mastr.download`][open_mastr.Mastr.download] with parameter
+        `method` = "bulk" to get bulk downloads of the dataset.
+
+    Use the higher level interface for bulk download
 
     `MaStRDownload` builds on top of [`MaStRAPI`][open_mastr.soap_api.download.MaStRAPI] and provides
     an interface for easier downloading.
     Use methods documented below to retrieve specific data. On the example of
     data for nuclear power plants, this looks like
 
     ```python
@@ -447,14 +454,25 @@
         parallel_processes : int or bool, optional
             Specify number of parallel unit data download, respectively
             the number of processes you want to use for downloading.
             For single-process download (avoiding the use of python
             multiprocessing package) choose False.
             Defaults to number of cores (including hyperthreading).
         """
+        log.warn(
+            """
+            The `MaStRDownload` class is deprecated and will not be maintained in the future.
+            To get a full table of the Marktstammdatenregister, use the open_mastr.Mastr.download
+            method.
+
+            If this change causes problems for you, please comment in this issue on github:
+            https://github.com/OpenEnergyPlatform/open-MaStR/issues/487
+
+            """
+        )
 
         # Number of parallel processes
         if parallel_processes == "max":
             self.parallel_processes = multiprocessing.cpu_count()
         else:
             self.parallel_processes = parallel_processes
 
@@ -758,34 +776,38 @@
 
         # In case multiple energy carriers (energietraeger) exist for one data type,
         # loop over these and join data to one list
         for et in energietraeger:
             log.info(
                 f"Get list of units with basic information for data type {data} ({et})"
             )
-            yield from basic_data_download(
-                self._mastr_api,
-                "GetListeAlleEinheiten",
-                "Einheiten",
-                chunks_start,
-                limits,
-                date_from,
-                max_retries,
-                data,
-                et=et,
-            ) if et is None else basic_data_download(
-                self._mastr_api,
-                "GetGefilterteListeStromErzeuger",
-                "Einheiten",
-                chunks_start,
-                limits,
-                date_from,
-                max_retries,
-                data,
-                et=et,
+            yield from (
+                basic_data_download(
+                    self._mastr_api,
+                    "GetListeAlleEinheiten",
+                    "Einheiten",
+                    chunks_start,
+                    limits,
+                    date_from,
+                    max_retries,
+                    data,
+                    et=et,
+                )
+                if et is None
+                else basic_data_download(
+                    self._mastr_api,
+                    "GetGefilterteListeStromErzeuger",
+                    "Einheiten",
+                    chunks_start,
+                    limits,
+                    date_from,
+                    max_retries,
+                    data,
+                    et=et,
+                )
             )
 
     def additional_data(self, data, unit_ids, data_fcn, timeout=10):
         """
         Retrieve addtional informations about units.
 
         Extended information on units is available. Depending on type, additional data from EEG
```

### Comparing `open_mastr-0.14.1/open_mastr/soap_api/metadata/LICENSE` & `open_mastr-0.14.3/open_mastr/soap_api/metadata/LICENSE`

 * *Files identical despite different names*

### Comparing `open_mastr-0.14.1/open_mastr/soap_api/metadata/create.py` & `open_mastr-0.14.3/open_mastr/soap_api/metadata/create.py`

 * *Files identical despite different names*

### Comparing `open_mastr-0.14.1/open_mastr/soap_api/metadata/description.py` & `open_mastr-0.14.3/open_mastr/soap_api/metadata/description.py`

 * *Files identical despite different names*

### Comparing `open_mastr-0.14.1/open_mastr/soap_api/mirror.py` & `open_mastr-0.14.3/open_mastr/soap_api/mirror.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,20 @@
 from open_mastr.utils.constants import ORM_MAP, UNIT_TYPE_MAP
 
 log = setup_logger()
 
 
 class MaStRMirror:
     """
+    !!! warning
+
+        **This class is deprecated** and will not be maintained from version 0.15.0 onwards.
+        Instead use [`Mastr.download`][open_mastr.Mastr.download] with parameter
+        `method` = "bulk" to mirror the MaStR dataset to a local database.
+
     Mirror the Marktstammdatenregister database and keep it up-to-date.
 
     A PostgreSQL database is used to mirror the MaStR database. It builds
     on functionality for bulk data download
     provided by [`MaStRDownload`][open_mastr.soap_api.download.MaStRDownload].
 
     A rough overview is given by the following schema on the example of wind power units.
@@ -89,14 +95,26 @@
             The database is restored from the SQL dump.
             Defaults to `None` which means nothing gets restored.
             Should be used in combination with `empty_schema=True`.
         parallel_processes: int
             Number of parallel processes used to download additional data.
             Defaults to `None`.
         """
+        log.warn(
+            """
+            The `MaStRMirror` class is deprecated and will not be maintained in the future.
+            To get a full table of the Marktstammdatenregister, use the open_mastr.Mastr.download
+            method.
+
+            If this change causes problems for you, please comment in this issue on github:
+            https://github.com/OpenEnergyPlatform/open-MaStR/issues/487
+
+            """
+        )
+
         self._engine = engine
 
         # Associate downloader
         self.mastr_dl = MaStRDownload(parallel_processes=parallel_processes)
 
         # Restore database from a dump
         if restore_dump:
@@ -975,14 +993,15 @@
         ----------
         dumpfile : str or path-like, optional
             Save path for dump including filename. When only a filename is given, the
             dump is restored from CWD.
 
 
         !!! warning
+
             If tables that are restored from the dump contain data, restore doesn't work!
 
         """
         # Interpret file name and path
         dump_file_dir, dump_file = os.path.split(dumpfile)
         cwd = os.path.abspath(os.path.dirname(dump_file_dir))
```

### Comparing `open_mastr-0.14.1/open_mastr/soap_api/parallel.py` & `open_mastr-0.14.3/open_mastr/soap_api/parallel.py`

 * *Files identical despite different names*

### Comparing `open_mastr-0.14.1/open_mastr/soap_api/utils.py` & `open_mastr-0.14.3/open_mastr/soap_api/utils.py`

 * *Files identical despite different names*

### Comparing `open_mastr-0.14.1/open_mastr/utils/config.py` & `open_mastr-0.14.3/open_mastr/utils/config.py`

 * *Files identical despite different names*

### Comparing `open_mastr-0.14.1/open_mastr/utils/constants.py` & `open_mastr-0.14.3/open_mastr/utils/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     "location",
     "market",
     "grid",
     "balancing_area",
     "permit",
     "deleted_units",
     "retrofit_units",
+    "changed_dso_assignment",
 ]
 
 # Possible values for parameter 'data' with API download method
 API_DATA = [
     "wind",
     "solar",
     "biomass",
@@ -58,14 +59,15 @@
     "grids",
     "locations_extended",
     "market_actors",
     "market_roles",
     "permit",
     "deleted_units",
     "retrofit_units",
+    "changed_dso_assignment",
 ]
 
 # Possible data types for API download
 API_DATA_TYPES = ["unit_data", "eeg_data", "kwk_data", "permit_data"]
 
 # Possible location types for API download
 API_LOCATION_TYPES = [
@@ -98,14 +100,15 @@
     "location": ["lokationen"],
     "market": ["marktakteure", "marktrollen"],
     "grid": ["netzanschlusspunkte", "netze"],
     "balancing_area": ["bilanzierungsgebiete"],
     "permit": ["einheitengenehmigung"],
     "deleted_units": ["geloeschteunddeaktivierteeinheiten"],
     "retrofit_units": ["ertuechtigungen"],
+    "changed_dso_assignment": ["einheitenaenderungnetzbetreiberzuordnungen"],
 }
 
 # Map bulk data to database table names, for csv export
 BULK_ADDITIONAL_TABLES_CSV_EXPORT_MAP = {
     "gas": [
         "gas_consumer",
         "gas_producer",
@@ -116,14 +119,15 @@
     "location": ["locations_extended"],
     "market": ["market_actors", "market_roles"],
     "grid": ["grid_connections", "grids"],
     "balancing_area": ["balancing_area"],
     "permit": ["permit"],
     "deleted_units": ["deleted_units"],
     "retrofit_units": ["retrofit_units"],
+    "changed_dso_assignment": ["changed_dso_assignment"],
 }
 
 # used to map the parameter options in open-mastr to the exact table class names in orm.py
 ORM_MAP = {
     "wind": {
         "unit_data": "WindExtended",
         "eeg_data": "WindEeg",
@@ -172,14 +176,15 @@
     "market_roles": "MarketRoles",
     "grid_connections": "GridConnections",
     "grids": "Grids",
     "balancing_area": "BalancingArea",
     "permit": "Permit",
     "deleted_units": "DeletedUnits",
     "retrofit_units": "RetrofitUnits",
+    "changed_dso_assignment": "ChangedDSOAssignment",
 }
 
 UNIT_TYPE_MAP = {
     "Windeinheit": "wind",
     "Solareinheit": "solar",
     "Biomasse": "biomass",
     "Wasser": "hydro",
@@ -306,15 +311,15 @@
     "WeicDisplayName": "weicDisplayName",
     "eegAnlagenschluessel": "eegPlantKey",
     "Nabenhoehe": "hubHeight",
     "VerhaeltnisErtragsschaetzungReferenzertrag_nv": "yieldEstimationReferenceYieldRatio_na",
     "AuflagenAbschaltungTierschutz": "requirementShutdownAnimalProtection",
     "AnlagenkennzifferAnlagenregister_nv": "plantIdentificationNumberRegister_nv",
     "BiogasDatumLeistungserhoehung": "biogasCapacityIncreaseDate",
-    "InAnspruchGenommeneAckerflaeche": "areaOfAgriculturalLandInUse",
+    "InAnspruchGenommeneLandwirtschaftlichGenutzteFlaeche": "areaOfAgriculturalLandInUse",
     "Aktenzeichen": "fileReference",
     "NetzbetreiberpruefungStatus": "gridOperatorCheckStatus",
     "AnlageBetriebsstatus": "plantOperatingStatus",
     "Gemarkung": "plot",
     "Art": "type",
     "AnschlussAnHoechstOderHochSpannung": "connectionToHighVoltageOrExtraHighVoltage",
     "MaximaleGasbezugsleistung": "maximumGasPurchaseCapacity",
@@ -507,8 +512,12 @@
     "HausnummerNichtGefunden": "houseNumberNotFound",
     "Anlagenbetreiber": "plantOperator",
     "RegistrierungsdatumMarktakteur": "marketParticipantRegistrationDate",
     "MieterstromRegistrierungsdatum": "TenantPowerRegistrationDate",
     "MastrNummer": "mastrNumber",
     "Kuestenentfernung": "distanceToCoast",
     "eegAusschreibungZuschlag": "eegAuctionBidAward",
+    "DatumUeberfuehrungInReserve": "dateTransferToReserve",
+    "ReserveartNachDemEnWG": "typeOfReserveFromEnWG",
+    "WebportalDesNetzbetreibers": "webPortalGridOperator",
+    "RegisternummerPraefix": "registerNumberPrefix",
 }
```

### Comparing `open_mastr-0.14.1/open_mastr/utils/credentials.py` & `open_mastr-0.14.3/open_mastr/utils/credentials.py`

 * *Files identical despite different names*

### Comparing `open_mastr-0.14.1/open_mastr/utils/docs.py` & `open_mastr-0.14.3/open_mastr/utils/docs.py`

 * *Files identical despite different names*

### Comparing `open_mastr-0.14.1/open_mastr/utils/helpers.py` & `open_mastr-0.14.3/open_mastr/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `open_mastr-0.14.1/open_mastr/utils/orm.py` & `open_mastr-0.14.3/open_mastr/utils/orm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from sqlalchemy.ext.declarative import declarative_base
-from sqlalchemy.schema import MetaData
+from sqlalchemy.orm import DeclarativeBase
 from sqlalchemy import (
     Column,
     Integer,
     String,
     Float,
     Sequence,
     DateTime,
     Boolean,
     func,
     Date,
     JSON,
 )
 
-meta = MetaData()
-Base = declarative_base(metadata=meta)
+
+class Base(DeclarativeBase):
+    pass
 
 
 class ParentAllTables(object):
     DatenQuelle = Column(String)
     DatumDownload = Column(Date)
 
 
@@ -130,14 +130,16 @@
     FernsteuerbarkeitNb = Column(Boolean)
     FernsteuerbarkeitDv = Column(Boolean)
     FernsteuerbarkeitDr = Column(Boolean)
     Einspeisungsart = Column(String)
     PraequalifiziertFuerRegelenergie = Column(Boolean)
     GenMastrNummer = Column(String)
     Netzbetreiberzuordnungen = Column(String)
+    ReserveartNachDemEnWG = Column(String)
+    DatumUeberfuehrungInReserve = Column(Date)
     # from bulk download
     Hausnummer_nv = Column(Boolean)
     Weic_nv = Column(Boolean)
     Kraftwerksnummer_nv = Column(Boolean)
 
 
 class WindExtended(Extended, ParentAllTables, Base):
@@ -181,15 +183,15 @@
     EinheitlicheAusrichtungUndNeigungswinkel = Column(Boolean)
     Hauptausrichtung = Column(String)
     HauptausrichtungNeigungswinkel = Column(String)
     Nebenausrichtung = Column(String)
     NebenausrichtungNeigungswinkel = Column(String)
     InAnspruchGenommeneFlaeche = Column(Float)
     ArtDerFlaeche = Column(String)
-    InAnspruchGenommeneAckerflaeche = Column(Float)
+    InAnspruchGenommeneLandwirtschaftlichGenutzteFlaeche = Column(Float)
     Nutzungsbereich = Column(String)
     Buergerenergie = Column(Boolean)
     EegMastrNummer = Column(String)
     ArtDerFlaecheIds = Column(String)
     Zaehlernummer = Column(String)
 
 
@@ -205,17 +207,14 @@
 
 class CombustionExtended(Extended, ParentAllTables, Base):
     __tablename__ = "combustion_extended"
 
     NameKraftwerk = Column(String)
     NameKraftwerksblock = Column(String)
     DatumBaubeginn = Column(Date)
-    AnzeigeEinerStilllegung = Column(Boolean)
-    ArtDerStilllegung = Column(String)
-    DatumBeginnVorlaeufigenOderEndgueltigenStilllegung = Column(Date)
     SteigerungNettonennleistungKombibetrieb = Column(Float)
     AnlageIstImKombibetrieb = Column(Boolean)
     MastrNummernKombibetrieb = Column(String)
     NetzreserveAbDatum = Column(Date)
     SicherheitsbereitschaftAbDatum = Column(Date)
     Hauptbrennstoff = Column(String)
     WeitererHauptbrennstoff = Column(String)
@@ -240,17 +239,14 @@
 
 
 class HydroExtended(Extended, ParentAllTables, Base):
     __tablename__ = "hydro_extended"
 
     NameKraftwerk = Column(String)
     ArtDerWasserkraftanlage = Column(String)
-    AnzeigeEinerStilllegung = Column(Boolean)
-    ArtDerStilllegung = Column(String)
-    DatumBeginnVorlaeufigenOderEndgueltigenStilllegung = Column(Date)
     MinderungStromerzeugung = Column(Boolean)
     BestandteilGrenzkraftwerk = Column(Boolean)
     NettonennleistungDeutschland = Column(Float)
     ArtDesZuflusses = Column(String)
     EegMastrNummer = Column(String)
 
 
@@ -270,15 +266,15 @@
     Batterietechnologie = Column(String)
     PumpbetriebLeistungsaufnahme = Column(Float)
     PumpbetriebKontinuierlichRegelbar = Column(Boolean)
     Pumpspeichertechnologie = Column(String)
     Notstromaggregat = Column(Boolean)
     BestandteilGrenzkraftwerk = Column(Boolean)
     NettonennleistungDeutschland = Column(Float)
-    ZugeordnenteWirkleistungWechselrichter = Column(Float)
+    ZugeordneteWirkleistungWechselrichter = Column(Float)
     NutzbareSpeicherkapazitaet = Column(Float)
     SpeMastrNummer = Column(String)
     EegMastrNummer = Column(String)
     EegAnlagentyp = Column(String)
     Technologie = Column(String)
     LeistungsaufnahmeBeimEinspeichern = Column(Float)
 
@@ -506,14 +502,15 @@
     SpeicherMastrNummer = Column(String)
     Gemarkung = Column(String)
     FlurFlurstuecknummern = Column(String)
     Adresszusatz = Column(String)
     DatumBeginnVoruebergehendeStilllegung = Column(Date)
     DatumDesBetreiberwechsels = Column(Date)
     DatumRegistrierungDesBetreiberwechsels = Column(Date)
+    DatumEndgueltigeStilllegung = Column(Date)
 
 
 class StorageUnits(ParentAllTables, Base):
     __tablename__ = "storage_units"
     MastrNummer = Column(String, primary_key=True)
     Registrierungsdatum = Column(Date)
     DatumLetzteAktualisierung = Column(DateTime(timezone=True))
@@ -566,14 +563,15 @@
     Erzeugungsleistung = Column(Float)
     DatumDesBetreiberwechsels = Column(Date)
     DatumRegistrierungDesBetreiberwechsels = Column(Date)
     Gemarkung = Column(String)
     FlurFlurstuecknummern = Column(String)
     GeplantesInbetriebnahmedatum = Column(Date)
     DatumBeginnVoruebergehendeStilllegung = Column(Date)
+    DatumEndgueltigeStilllegung = Column(Date)
 
 
 class GasConsumer(ParentAllTables, Base):
     __tablename__ = "gas_consumer"
 
     EinheitMastrNummer = Column(String, primary_key=True)
     DatumLetzteAktualisierung = Column(DateTime(timezone=True))
@@ -730,14 +728,16 @@
     Netz = Column(String)
     Direktvermarktungsunternehmen = Column(Boolean)
     BelieferungVonLetztverbrauchernStrom = Column(Boolean)
     BelieferungHaushaltskundenStrom = Column(Boolean)
     Stromgrosshaendler = Column(Boolean)
     MarktakteurVorname = Column(String)
     MarktakteurNachname = Column(String)
+    WebportalDesNetzbetreibers = Column(String)
+    RegisternummerPraefix = Column(String)
 
 
 class Grids(ParentAllTables, Base):
     __tablename__ = "grids"
 
     MastrNummer = Column(String, primary_key=True)
     DatumLetzteAktualisierung = Column(DateTime(timezone=True))
@@ -788,14 +788,29 @@
     Leistungserhoehung = Column(Float)
     WiederinbetriebnahmeDatum = Column(Date)
     DatumLetzteAktualisierung = Column(DateTime(timezone=True))
     Ertuechtigungsart = Column(String)
     ErtuechtigungIstZulassungspflichtig = Column(Boolean)
 
 
+class ChangedDSOAssignment(ParentAllTables, Base):
+    __tablename__ = "changed_dso_assignment"
+
+    EinheitMastrNummer = Column(String, primary_key=True)
+    LokationMastrNummer = Column(String)
+    NetzanschlusspunktMastrNummer = Column(String)
+    NetzbetreiberMastrNummerNeu = Column(String)
+    NetzbetreiberMastrNummerAlt = Column(String)
+    ArtDerAenderung = Column(String)
+    RegistrierungsdatumNetzbetreiberzuordnungsaenderung = Column(
+        DateTime(timezone=True)
+    )
+    Netzbetreiberzuordnungsaenderungsdatum = Column(DateTime(timezone=True))
+
+
 tablename_mapping = {
     "anlageneegbiomasse": {
         "__name__": BiomassEeg.__tablename__,
         "__class__": BiomassEeg,
         "replace_column_names": {
             "EegMaStRNummer": "EegMastrNummer",
             "VerknuepfteEinheitenMaStRNummern": "VerknuepfteEinheit",
@@ -919,14 +934,19 @@
         },
     },
     "bilanzierungsgebiete": {
         "__name__": BalancingArea.__tablename__,
         "__class__": BalancingArea,
         "replace_column_names": None,
     },
+    "einheitenaenderungnetzbetreiberzuordnungen": {
+        "__name__": ChangedDSOAssignment.__tablename__,
+        "__class__": ChangedDSOAssignment,
+        "replace_column_names": None,
+    },
     "einheitengaserzeuger": {
         "__name__": GasProducer.__tablename__,
         "__class__": GasProducer,
         "replace_column_names": {
             "LokationMaStRNummer": "LokationMastrNummer",
             "SpeicherMaStRNummer": "SpeicherMastrNummer",
         },
```

### Comparing `open_mastr-0.14.1/open_mastr/xml_download/colums_to_replace.py` & `open_mastr-0.14.3/open_mastr/xml_download/colums_to_replace.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,16 @@
     # anlageneegbiomasse
     # anlageneeggeosolarthermiegrubenklaerschlammdruckentspannung
     # anlageneegwasser
     # anlageneegwind
     # anlagengasspeicher
     # anlagenkwk
     # bilanzierungsgebiete
+    # einheitenaenderungnetzbetreiberzuordnungen
+    "ArtDerAenderung",
     # einheitenbiomasse
     "Hauptbrennstoff",
     "Biomasseart",
     # einheitengaserzeuger
     # einheitengasspeicher
     "Speicherart",
     # einheitengasverbraucher
```

### Comparing `open_mastr-0.14.1/open_mastr/xml_download/utils_cleansing_bulk.py` & `open_mastr-0.14.3/open_mastr/xml_download/utils_cleansing_bulk.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
                 # Handle comma seperated strings from catalog values
                 df[column_name] = (
                     df[column_name]
                     .str.split(",", expand=True)
                     .apply(lambda x: x.str.strip())
                     .replace("", None)
                     .astype("Int64")
-                    .applymap(katalogwerte.get)
+                    .map(katalogwerte.get)
                     .agg(lambda d: ",".join(i for i in d if isinstance(i, str)), axis=1)
                     .replace("", None)
                 )
             else:
                 df[column_name] = (
                     df[column_name].astype("float").astype("Int64").map(katalogwerte)
                 )
```

### Comparing `open_mastr-0.14.1/open_mastr/xml_download/utils_write_to_database.py` & `open_mastr-0.14.3/open_mastr/xml_download/utils_write_to_database.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from sqlalchemy import select
 from sqlalchemy.sql import text
 
 from open_mastr.utils.config import setup_logger
 from open_mastr.utils.helpers import data_to_include_tables
 from open_mastr.utils.orm import tablename_mapping
 from open_mastr.xml_download.utils_cleansing_bulk import cleanse_bulk_data
+from io import StringIO
 
 
 def write_mastr_xml_to_database(
     engine: sqlalchemy.engine.Engine,
     zipped_xml_file_path: str,
     data: list,
     bulk_cleansing: bool,
@@ -152,15 +153,15 @@
     xml_tablename: str,
     bulk_download_date: str,
 ) -> pd.DataFrame:
     data = f.read(file_name)
     try:
         df = pd.read_xml(data, encoding="UTF-16", compression="zip")
     except lxml.etree.XMLSyntaxError as err:
-        df = handle_xml_syntax_error(data, err)
+        df = handle_xml_syntax_error(data.decode("utf-16"), err)
 
     df = add_zero_as_first_character_for_too_short_string(df)
     df = change_column_names_to_orm_format(df, xml_tablename)
 
     # Add Column that refers to the source of the data
     df["DatenQuelle"] = "bulk"
     df["DatumDownload"] = bulk_download_date
@@ -331,50 +332,56 @@
                 con.execute(text(alter_query).execution_options(autocommit=True))
         log.info(
             "From the downloaded xml files following new attribute was "
             f"introduced: {table_name}.{column_name}"
         )
 
 
-def delete_wrong_xml_entry(err: Error, df: pd.DataFrame) -> None:
+def delete_wrong_xml_entry(err: Error, df: pd.DataFrame) -> pd.DataFrame:
     delete_entry = str(err).split("«")[0].split("»")[1]
     print(f"The entry {delete_entry} was deleted due to its false data type.")
-    df = df.replace(delete_entry, np.nan)
+    return df.replace(delete_entry, np.nan)
 
 
-def handle_xml_syntax_error(data: bytes, err: Error) -> pd.DataFrame:
+def handle_xml_syntax_error(data: str, err: Error) -> pd.DataFrame:
     """Deletes entries that cause an xml syntax error and produces DataFrame.
 
     Parameters
     -----------
-    data : bytes
-        Unzipped xml data
+    data : str
+        Decoded xml file as one string
     err : ErrorMessage
         Error message that appeared when trying to use pd.read_xml on invalid xml file.
 
     Returns
     ----------
     df : pandas.DataFrame
         DataFrame which is read from the changed xml data.
     """
-    wrong_char_position = int(str(err).split()[-4])
-    decoded_data = data.decode("utf-16")
-    loop_condition = True
-
-    shift = 0
-    while loop_condition:
-        evaluated_string = decoded_data[wrong_char_position + shift]
-        if evaluated_string == ">":
-            start_char = wrong_char_position + shift + 1
-            break
-        else:
-            shift -= 1
-    loop_condition_2 = True
-    while loop_condition_2:
-        evaluated_string = decoded_data[start_char]
-        if evaluated_string == "<":
-            break
-        else:
-            decoded_data = decoded_data[:start_char] + decoded_data[start_char + 1 :]
-    df = pd.read_xml(decoded_data)
-    print("One invalid xml expression was deleted.")
-    return df
+
+    def find_nearest_brackets(xml_string: str, position: int) -> tuple[int, int]:
+        left_bracket_position = xml_string.rfind(">", 0, position)
+        right_bracket_position = xml_string.find("<", position)
+        return left_bracket_position, right_bracket_position
+
+    data = data.splitlines()
+
+    for _ in range(100):
+        # check for maximum of 100 syntax errors, otherwise return an error
+        wrong_char_row, wrong_char_column = err.position
+        row_with_error = data[wrong_char_row - 1]
+
+        left_bracket, right_bracket = find_nearest_brackets(
+            row_with_error, wrong_char_column
+        )
+        data[wrong_char_row - 1] = (
+            row_with_error[: left_bracket + 1] + row_with_error[right_bracket:]
+        )
+        try:
+            print("One invalid xml expression was deleted.")
+            df = pd.read_xml(StringIO("\n".join(data)))
+            return df
+        except lxml.etree.XMLSyntaxError as e:
+            err = e
+            continue
+
+    raise Error("An error occured when parsing the xml file. Maybe it is corrupted?")
```

### Comparing `open_mastr-0.14.1/tests/test_helpers.py` & `open_mastr-0.14.3/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `open_mastr-0.14.1/tests/test_mastr.py` & `open_mastr-0.14.3/tests/test_mastr.py`

 * *Files identical despite different names*

