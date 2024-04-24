# Comparing `tmp/silvio-0.2.5.tar.gz` & `tmp/silvio-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/silvio-0.2.5.tar", last modified: Fri Feb 23 11:05:54 2024, max compression
+gzip compressed data, was "dist/silvio-0.2.6.tar", last modified: Wed Apr 24 15:20:37 2024, max compression
```

## Comparing `silvio-0.2.5.tar` & `silvio-0.2.6.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxrwxr-x   0 ulf       (1000) ulf       (1000)        0 2024-02-23 11:05:54.000000 silvio-0.2.5/
--rw-rw-r--   0 ulf       (1000) ulf       (1000)      483 2021-11-05 13:03:32.000000 silvio-0.2.5/AUTHORS.rst
--rw-rw-r--   0 ulf       (1000) ulf       (1000)     3577 2021-11-05 13:03:32.000000 silvio-0.2.5/CONTRIBUTING.rst
--rw-rw-r--   0 ulf       (1000) ulf       (1000)     6751 2022-12-01 13:01:05.000000 silvio-0.2.5/DEVNOTES.rst
--rw-rw-r--   0 ulf       (1000) ulf       (1000)     1412 2024-02-22 10:24:58.000000 silvio-0.2.5/HISTORY.rst
--rw-r--r--   0 ulf       (1000) ulf       (1000)     1067 2021-09-18 10:58:15.000000 silvio-0.2.5/LICENSE
--rw-rw-r--   0 ulf       (1000) ulf       (1000)      320 2021-11-05 13:03:32.000000 silvio-0.2.5/MANIFEST.in
--rw-rw-r--   0 ulf       (1000) ulf       (1000)     7948 2024-02-23 11:05:54.000000 silvio-0.2.5/PKG-INFO
--rw-rw-r--   0 ulf       (1000) ulf       (1000)     5602 2023-09-04 15:24:00.000000 silvio-0.2.5/README.rst
-drwxrwxr-x   0 ulf       (1000) ulf       (1000)        0 2024-02-23 11:05:54.000000 silvio-0.2.5/docs/
--rw-rw-r--   0 ulf       (1000) ulf       (1000)      816 2021-11-05 13:03:32.000000 silvio-0.2.5/docs/Makefile
-drwxrwxr-x   0 ulf       (1000) ulf       (1000)        0 2024-02-23 11:05:54.000000 silvio-0.2.5/docs/_build/
-drwxrwxr-x   0 ulf       (1000) ulf       (1000)        0 2024-02-23 11:05:54.000000 silvio-0.2.5/docs/_build/html/
-drwxrwxr-x   0 ulf       (1000) ulf       (1000)        0 2024-02-23 11:05:54.000000 silvio-0.2.5/docs/_build/html/_static/
--rw-rw-r--   0 ulf       (1000) ulf       (1000)      286 2022-11-30 14:12:30.000000 silvio-0.2.5/docs/_build/html/_static/file.png
--rw-rw-r--   0 ulf       (1000) ulf       (1000)       90 2022-11-30 14:12:30.000000 silvio-0.2.5/docs/_build/html/_static/minus.png
--rw-rw-r--   0 ulf       (1000) ulf       (1000)       90 2022-11-30 14:12:30.000000 silvio-0.2.5/docs/_build/html/_static/plus.png
--rw-rw-r--   0 ulf       (1000) ulf       (1000)       28 2021-11-05 13:03:32.000000 silvio-0.2.5/docs/authors.rst
--rwxrwxr-x   0 ulf       (1000) ulf       (1000)     4769 2021-11-05 13:03:32.000000 silvio-0.2.5/docs/conf.py
--rw-rw-r--   0 ulf       (1000) ulf       (1000)       33 2021-11-05 13:03:32.000000 silvio-0.2.5/docs/contributing.rst
--rw-rw-r--   0 ulf       (1000) ulf       (1000)     9001 2021-11-05 13:03:32.000000 silvio-0.2.5/docs/design.rst
--rw-rw-r--   0 ulf       (1000) ulf       (1000)       28 2021-11-05 13:03:32.000000 silvio-0.2.5/docs/history.rst
--rw-rw-r--   0 ulf       (1000) ulf       (1000)      320 2021-11-05 13:03:32.000000 silvio-0.2.5/docs/index.rst
--rw-rw-r--   0 ulf       (1000) ulf       (1000)     1114 2021-11-05 13:03:32.000000 silvio-0.2.5/docs/installation.rst
--rw-rw-r--   0 ulf       (1000) ulf       (1000)      768 2021-11-05 13:03:32.000000 silvio-0.2.5/docs/make.bat
--rw-rw-r--   0 ulf       (1000) ulf       (1000)       27 2021-11-05 13:03:32.000000 silvio-0.2.5/docs/readme.rst
-drwxrwxr-x   0 ulf       (1000) ulf       (1000)        0 2024-02-23 11:05:54.000000 silvio-0.2.5/docs/source/
--rw-rw-r--   0 ulf       (1000) ulf       (1000)       55 2022-11-30 14:12:48.000000 silvio-0.2.5/docs/source/modules.rst
--rw-rw-r--   0 ulf       (1000) ulf       (1000)      358 2022-11-30 14:12:49.000000 silvio-0.2.5/docs/source/silvio.catalog.rst
--rw-rw-r--   0 ulf       (1000) ulf       (1000)     1607 2022-11-30 14:12:49.000000 silvio-0.2.5/docs/source/silvio.extensions.modules.rst
--rw-rw-r--   0 ulf       (1000) ulf       (1000)     1159 2022-11-30 14:12:49.000000 silvio-0.2.5/docs/source/silvio.extensions.records.gene.rst
--rw-rw-r--   0 ulf       (1000) ulf       (1000)      528 2022-11-30 14:12:49.000000 silvio-0.2.5/docs/source/silvio.extensions.records.rst
--rw-rw-r--   0 ulf       (1000) ulf       (1000)      757 2022-11-30 14:12:49.000000 silvio-0.2.5/docs/source/silvio.extensions.rst
--rw-rw-r--   0 ulf       (1000) ulf       (1000)      278 2022-11-30 14:12:49.000000 silvio-0.2.5/docs/source/silvio.extensions.sets.rst
--rw-rw-r--   0 ulf       (1000) ulf       (1000)     1855 2022-11-30 14:12:49.000000 silvio-0.2.5/docs/source/silvio.extensions.sets.shotgun_sequencing.rst
--rw-rw-r--   0 ulf       (1000) ulf       (1000)      441 2022-11-30 14:12:49.000000 silvio-0.2.5/docs/source/silvio.extensions.tools.rst
--rw-rw-r--   0 ulf       (1000) ulf       (1000)     1256 2022-11-30 14:12:49.000000 silvio-0.2.5/docs/source/silvio.extensions.utils.rst
--rw-rw-r--   0 ulf       (1000) ulf       (1000)     1892 2022-11-30 14:12:49.000000 silvio-0.2.5/docs/source/silvio.rst
--rw-rw-r--   0 ulf       (1000) ulf       (1000)       67 2021-11-05 13:03:32.000000 silvio-0.2.5/docs/usage.rst
--rw-rw-r--   0 ulf       (1000) ulf       (1000)      427 2024-02-23 11:05:54.000000 silvio-0.2.5/setup.cfg
--rw-rw-r--   0 ulf       (1000) ulf       (1000)     2151 2023-09-04 14:48:38.000000 silvio-0.2.5/setup.py
-drwxrwxr-x   0 ulf       (1000) ulf       (1000)        0 2024-02-23 11:05:54.000000 silvio-0.2.5/src/
-drwxrwxr-x   0 ulf       (1000) ulf       (1000)        0 2024-02-23 11:05:54.000000 silvio-0.2.5/src/silvio/
--rw-rw-r--   0 ulf       (1000) ulf       (1000)     1862 2024-02-22 10:23:59.000000 silvio-0.2.5/src/silvio/__init__.py
-drwxrwxr-x   0 ulf       (1000) ulf       (1000)        0 2024-02-23 11:05:54.000000 silvio-0.2.5/src/silvio/catalog/
--rw-rw-r--   0 ulf       (1000) ulf       (1000)    27146 2024-02-22 13:36:50.000000 silvio-0.2.5/src/silvio/catalog/GroExpSim.py
--rw-rw-r--   0 ulf       (1000) ulf       (1000)    15408 2023-03-29 13:23:49.000000 silvio-0.2.5/src/silvio/catalog/RecExpSim.py
--rw-rw-r--   0 ulf       (1000) ulf       (1000)        0 2022-04-07 08:32:03.000000 silvio-0.2.5/src/silvio/catalog/__init__.py
--rw-rw-r--   0 ulf       (1000) ulf       (1000)      337 2021-11-05 13:03:32.000000 silvio-0.2.5/src/silvio/config.py
-drwxrwxr-x   0 ulf       (1000) ulf       (1000)        0 2024-02-23 11:05:54.000000 silvio-0.2.5/src/silvio/data/
--rw-rw-r--   0 ulf       (1000) ulf       (1000)     1212 2021-09-18 10:48:34.000000 silvio-0.2.5/src/silvio/data/CodonTriplets.csv
-drwxrwxr-x   0 ulf       (1000) ulf       (1000)        0 2024-02-23 11:05:54.000000 silvio-0.2.5/src/silvio/data/expression_predictor/
--rw-rw-r--   0 ulf       (1000) ulf       (1000)      327 2021-09-18 10:48:34.000000 silvio-0.2.5/src/silvio/data/expression_predictor/Ecol-Promoter-AddParams.pkl
--rw-rw-r--   0 ulf       (1000) ulf       (1000)   283435 2021-09-18 10:48:34.000000 silvio-0.2.5/src/silvio/data/expression_predictor/Ecol-Promoter-predictor.pkl
--rw-rw-r--   0 ulf       (1000) ulf       (1000)      327 2021-09-18 10:48:34.000000 silvio-0.2.5/src/silvio/data/expression_predictor/Ptai-Promoter-AddParams.pkl
--rw-rw-r--   0 ulf       (1000) ulf       (1000)   401243 2021-09-18 10:48:34.000000 silvio-0.2.5/src/silvio/data/expression_predictor/Ptai-Promoter-predictor.pkl
-drwxrwxr-x   0 ulf       (1000) ulf       (1000)        0 2024-02-23 11:05:54.000000 silvio-0.2.5/src/silvio/data/metabolic_model/
--rw-rw-r--   0 ulf       (1000) ulf       (1000)   707166 2021-09-18 10:48:34.000000 silvio-0.2.5/src/silvio/data/metabolic_model/e_coli_core.xml
--rw-rw-r--   0 ulf       (1000) ulf       (1000)  5116056 2021-09-18 10:48:34.000000 silvio-0.2.5/src/silvio/data/metabolic_model/iJN746.xml
--rw-rw-r--   0 ulf       (1000) ulf       (1000)      325 2021-11-05 13:03:32.000000 silvio-0.2.5/src/silvio/events.py
--rw-rw-r--   0 ulf       (1000) ulf       (1000)     1056 2021-11-05 13:03:32.000000 silvio-0.2.5/src/silvio/experiment.py
-drwxrwxr-x   0 ulf       (1000) ulf       (1000)        0 2024-02-23 11:05:54.000000 silvio-0.2.5/src/silvio/extensions/
--rw-rw-r--   0 ulf       (1000) ulf       (1000)        0 2021-11-05 12:56:13.000000 silvio-0.2.5/src/silvio/extensions/__init__.py
--rw-rw-r--   0 ulf       (1000) ulf       (1000)      592 2022-05-03 06:53:25.000000 silvio-0.2.5/src/silvio/extensions/all_events.py
--rw-rw-r--   0 ulf       (1000) ulf       (1000)      369 2021-11-05 12:56:13.000000 silvio-0.2.5/src/silvio/extensions/common.py
-drwxrwxr-x   0 ulf       (1000) ulf       (1000)        0 2024-02-23 11:05:54.000000 silvio-0.2.5/src/silvio/extensions/modules/
--rw-rw-r--   0 ulf       (1000) ulf       (1000)        0 2021-11-05 12:56:13.000000 silvio-0.2.5/src/silvio/extensions/modules/__init__.py
--rw-rw-r--   0 ulf       (1000) ulf       (1000)     3830 2021-11-05 13:03:32.000000 silvio-0.2.5/src/silvio/extensions/modules/genome_expression.py
--rw-rw-r--   0 ulf       (1000) ulf       (1000)    10146 2021-11-05 13:03:32.000000 silvio-0.2.5/src/silvio/extensions/modules/genome_library.py
--rw-rw-r--   0 ulf       (1000) ulf       (1000)     2153 2021-11-05 13:03:32.000000 silvio-0.2.5/src/silvio/extensions/modules/genome_list.py
--rw-rw-r--   0 ulf       (1000) ulf       (1000)    12561 2023-09-01 13:31:13.000000 silvio-0.2.5/src/silvio/extensions/modules/growth_behaviour.py
--rw-rw-r--   0 ulf       (1000) ulf       (1000)     4333 2022-05-03 07:08:02.000000 silvio-0.2.5/src/silvio/extensions/modules/metabolic_flux.py
--rw-rw-r--   0 ulf       (1000) ulf       (1000)     1167 2021-11-05 13:03:32.000000 silvio-0.2.5/src/silvio/extensions/modules/phenotype_size.py
-drwxrwxr-x   0 ulf       (1000) ulf       (1000)        0 2024-02-23 11:05:54.000000 silvio-0.2.5/src/silvio/extensions/records/
--rw-rw-r--   0 ulf       (1000) ulf       (1000)        0 2021-11-05 12:56:13.000000 silvio-0.2.5/src/silvio/extensions/records/__init__.py
-drwxrwxr-x   0 ulf       (1000) ulf       (1000)        0 2024-02-23 11:05:54.000000 silvio-0.2.5/src/silvio/extensions/records/gene/
--rw-rw-r--   0 ulf       (1000) ulf       (1000)        0 2021-11-05 12:56:13.000000 silvio-0.2.5/src/silvio/extensions/records/gene/__init__.py
--rw-rw-r--   0 ulf       (1000) ulf       (1000)     1216 2021-09-18 10:07:03.000000 silvio-0.2.5/src/silvio/extensions/records/gene/crafted_gene.py
--rw-rw-r--   0 ulf       (1000) ulf       (1000)      701 2021-09-18 10:07:03.000000 silvio-0.2.5/src/silvio/extensions/records/gene/gene.py
--rw-rw-r--   0 ulf       (1000) ulf       (1000)     2131 2021-11-05 13:03:32.000000 silvio-0.2.5/src/silvio/extensions/records/gene/localized_gene.py
--rw-rw-r--   0 ulf       (1000) ulf       (1000)      544 2021-11-05 13:03:32.000000 silvio-0.2.5/src/silvio/extensions/records/gene/stub_gene.py
--rw-rw-r--   0 ulf       (1000) ulf       (1000)      598 2021-11-05 13:03:32.000000 silvio-0.2.5/src/silvio/extensions/records/growth_record.py
-drwxrwxr-x   0 ulf       (1000) ulf       (1000)        0 2024-02-23 11:05:54.000000 silvio-0.2.5/src/silvio/extensions/sets/
--rw-rw-r--   0 ulf       (1000) ulf       (1000)      537 2021-11-05 13:03:32.000000 silvio-0.2.5/src/silvio/extensions/sets/__init__.py
-drwxrwxr-x   0 ulf       (1000) ulf       (1000)        0 2024-02-23 11:05:54.000000 silvio-0.2.5/src/silvio/extensions/sets/shotgun_sequencing/
--rw-rw-r--   0 ulf       (1000) ulf       (1000)      146 2021-11-05 13:03:32.000000 silvio-0.2.5/src/silvio/extensions/sets/shotgun_sequencing/__init__.py
--rw-rw-r--   0 ulf       (1000) ulf       (1000)     8044 2021-11-05 13:03:32.000000 silvio-0.2.5/src/silvio/extensions/sets/shotgun_sequencing/assembly.py
--rw-rw-r--   0 ulf       (1000) ulf       (1000)     7636 2021-11-05 13:03:32.000000 silvio-0.2.5/src/silvio/extensions/sets/shotgun_sequencing/datatype.py
--rw-rw-r--   0 ulf       (1000) ulf       (1000)     2448 2021-11-05 13:03:32.000000 silvio-0.2.5/src/silvio/extensions/sets/shotgun_sequencing/evaluation.py
--rw-rw-r--   0 ulf       (1000) ulf       (1000)     8849 2021-11-05 13:03:32.000000 silvio-0.2.5/src/silvio/extensions/sets/shotgun_sequencing/sequencing.py
--rw-rw-r--   0 ulf       (1000) ulf       (1000)     1845 2021-11-05 13:03:32.000000 silvio-0.2.5/src/silvio/extensions/sets/shotgun_sequencing/storage.py
--rw-rw-r--   0 ulf       (1000) ulf       (1000)     5265 2021-11-05 13:03:32.000000 silvio-0.2.5/src/silvio/extensions/sets/shotgun_sequencing/visualization.py
-drwxrwxr-x   0 ulf       (1000) ulf       (1000)        0 2024-02-23 11:05:54.000000 silvio-0.2.5/src/silvio/extensions/tools/
--rw-rw-r--   0 ulf       (1000) ulf       (1000)        0 2021-11-05 13:03:32.000000 silvio-0.2.5/src/silvio/extensions/tools/__init__.py
--rw-rw-r--   0 ulf       (1000) ulf       (1000)      202 2021-11-05 13:03:32.000000 silvio-0.2.5/src/silvio/extensions/tools/shotgun_sequencing.py
-drwxrwxr-x   0 ulf       (1000) ulf       (1000)        0 2024-02-23 11:05:54.000000 silvio-0.2.5/src/silvio/extensions/utils/
--rw-rw-r--   0 ulf       (1000) ulf       (1000)        0 2021-11-05 12:56:13.000000 silvio-0.2.5/src/silvio/extensions/utils/__init__.py
--rw-rw-r--   0 ulf       (1000) ulf       (1000)      328 2021-09-18 10:07:03.000000 silvio-0.2.5/src/silvio/extensions/utils/laboratory.py
--rw-rw-r--   0 ulf       (1000) ulf       (1000)     6864 2021-09-18 10:07:03.000000 silvio-0.2.5/src/silvio/extensions/utils/misc.py
--rw-rw-r--   0 ulf       (1000) ulf       (1000)      481 2021-11-05 13:03:32.000000 silvio-0.2.5/src/silvio/extensions/utils/shotgun_sequencing.py
--rw-rw-r--   0 ulf       (1000) ulf       (1000)      777 2021-09-18 10:07:03.000000 silvio-0.2.5/src/silvio/extensions/utils/transform.py
--rw-rw-r--   0 ulf       (1000) ulf       (1000)      506 2021-09-18 10:07:03.000000 silvio-0.2.5/src/silvio/extensions/utils/visual.py
--rw-rw-r--   0 ulf       (1000) ulf       (1000)     8455 2021-11-05 13:03:32.000000 silvio-0.2.5/src/silvio/host.py
--rw-rw-r--   0 ulf       (1000) ulf       (1000)     4163 2021-11-05 13:03:32.000000 silvio-0.2.5/src/silvio/module.py
--rw-rw-r--   0 ulf       (1000) ulf       (1000)     5213 2024-02-22 15:47:08.000000 silvio-0.2.5/src/silvio/outcome.py
--rw-rw-r--   0 ulf       (1000) ulf       (1000)     3758 2021-11-05 12:56:13.000000 silvio-0.2.5/src/silvio/random.py
--rw-rw-r--   0 ulf       (1000) ulf       (1000)      253 2021-11-05 13:03:32.000000 silvio-0.2.5/src/silvio/record.py
--rw-rw-r--   0 ulf       (1000) ulf       (1000)     1036 2021-09-18 10:07:03.000000 silvio-0.2.5/src/silvio/registry.py
--rw-rw-r--   0 ulf       (1000) ulf       (1000)     1550 2021-11-05 13:03:32.000000 silvio-0.2.5/src/silvio/tool.py
--rw-rw-r--   0 ulf       (1000) ulf       (1000)      681 2021-09-18 10:07:08.000000 silvio-0.2.5/src/silvio/utils.py
-drwxrwxr-x   0 ulf       (1000) ulf       (1000)        0 2024-02-23 11:05:54.000000 silvio-0.2.5/src/silvio.egg-info/
--rw-rw-r--   0 ulf       (1000) ulf       (1000)     7948 2024-02-23 11:05:54.000000 silvio-0.2.5/src/silvio.egg-info/PKG-INFO
--rw-rw-r--   0 ulf       (1000) ulf       (1000)     3338 2024-02-23 11:05:54.000000 silvio-0.2.5/src/silvio.egg-info/SOURCES.txt
--rw-rw-r--   0 ulf       (1000) ulf       (1000)        1 2024-02-23 11:05:54.000000 silvio-0.2.5/src/silvio.egg-info/dependency_links.txt
--rw-rw-r--   0 ulf       (1000) ulf       (1000)        1 2024-02-23 11:05:54.000000 silvio-0.2.5/src/silvio.egg-info/not-zip-safe
--rw-rw-r--   0 ulf       (1000) ulf       (1000)      121 2024-02-23 11:05:54.000000 silvio-0.2.5/src/silvio.egg-info/requires.txt
--rw-rw-r--   0 ulf       (1000) ulf       (1000)        7 2024-02-23 11:05:54.000000 silvio-0.2.5/src/silvio.egg-info/top_level.txt
-drwxrwxr-x   0 ulf       (1000) ulf       (1000)        0 2024-02-23 11:05:54.000000 silvio-0.2.5/tests/
--rw-rw-r--   0 ulf       (1000) ulf       (1000)       36 2021-11-05 13:03:32.000000 silvio-0.2.5/tests/__init__.py
--rw-rw-r--   0 ulf       (1000) ulf       (1000)      477 2021-11-05 13:03:32.000000 silvio-0.2.5/tests/test_basic.py
+drwxrwxr-x   0 ulf       (1000) ulf       (1000)        0 2024-04-24 15:20:37.000000 silvio-0.2.6/
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)      483 2021-11-05 13:03:32.000000 silvio-0.2.6/AUTHORS.rst
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)     3577 2021-11-05 13:03:32.000000 silvio-0.2.6/CONTRIBUTING.rst
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)     6751 2022-12-01 13:01:05.000000 silvio-0.2.6/DEVNOTES.rst
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)     1607 2024-04-24 14:08:41.000000 silvio-0.2.6/HISTORY.rst
+-rw-r--r--   0 ulf       (1000) ulf       (1000)     1067 2021-09-18 10:58:15.000000 silvio-0.2.6/LICENSE
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)      320 2021-11-05 13:03:32.000000 silvio-0.2.6/MANIFEST.in
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)     8143 2024-04-24 15:20:37.000000 silvio-0.2.6/PKG-INFO
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)     5602 2023-09-04 15:24:00.000000 silvio-0.2.6/README.rst
+drwxrwxr-x   0 ulf       (1000) ulf       (1000)        0 2024-04-24 15:20:37.000000 silvio-0.2.6/docs/
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)      816 2021-11-05 13:03:32.000000 silvio-0.2.6/docs/Makefile
+drwxrwxr-x   0 ulf       (1000) ulf       (1000)        0 2024-04-24 15:20:37.000000 silvio-0.2.6/docs/_build/
+drwxrwxr-x   0 ulf       (1000) ulf       (1000)        0 2024-04-24 15:20:37.000000 silvio-0.2.6/docs/_build/html/
+drwxrwxr-x   0 ulf       (1000) ulf       (1000)        0 2024-04-24 15:20:37.000000 silvio-0.2.6/docs/_build/html/_static/
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)      286 2022-11-30 14:12:30.000000 silvio-0.2.6/docs/_build/html/_static/file.png
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)       90 2022-11-30 14:12:30.000000 silvio-0.2.6/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)       90 2022-11-30 14:12:30.000000 silvio-0.2.6/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)       28 2021-11-05 13:03:32.000000 silvio-0.2.6/docs/authors.rst
+-rwxrwxr-x   0 ulf       (1000) ulf       (1000)     4769 2021-11-05 13:03:32.000000 silvio-0.2.6/docs/conf.py
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)       33 2021-11-05 13:03:32.000000 silvio-0.2.6/docs/contributing.rst
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)     9001 2021-11-05 13:03:32.000000 silvio-0.2.6/docs/design.rst
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)       28 2021-11-05 13:03:32.000000 silvio-0.2.6/docs/history.rst
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)      320 2021-11-05 13:03:32.000000 silvio-0.2.6/docs/index.rst
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)     1114 2021-11-05 13:03:32.000000 silvio-0.2.6/docs/installation.rst
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)      768 2021-11-05 13:03:32.000000 silvio-0.2.6/docs/make.bat
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)       27 2021-11-05 13:03:32.000000 silvio-0.2.6/docs/readme.rst
+drwxrwxr-x   0 ulf       (1000) ulf       (1000)        0 2024-04-24 15:20:37.000000 silvio-0.2.6/docs/source/
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)       55 2022-11-30 14:12:48.000000 silvio-0.2.6/docs/source/modules.rst
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)      358 2022-11-30 14:12:49.000000 silvio-0.2.6/docs/source/silvio.catalog.rst
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)     1607 2022-11-30 14:12:49.000000 silvio-0.2.6/docs/source/silvio.extensions.modules.rst
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)     1159 2022-11-30 14:12:49.000000 silvio-0.2.6/docs/source/silvio.extensions.records.gene.rst
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)      528 2022-11-30 14:12:49.000000 silvio-0.2.6/docs/source/silvio.extensions.records.rst
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)      757 2022-11-30 14:12:49.000000 silvio-0.2.6/docs/source/silvio.extensions.rst
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)      278 2022-11-30 14:12:49.000000 silvio-0.2.6/docs/source/silvio.extensions.sets.rst
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)     1855 2022-11-30 14:12:49.000000 silvio-0.2.6/docs/source/silvio.extensions.sets.shotgun_sequencing.rst
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)      441 2022-11-30 14:12:49.000000 silvio-0.2.6/docs/source/silvio.extensions.tools.rst
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)     1256 2022-11-30 14:12:49.000000 silvio-0.2.6/docs/source/silvio.extensions.utils.rst
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)     1892 2022-11-30 14:12:49.000000 silvio-0.2.6/docs/source/silvio.rst
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)       67 2021-11-05 13:03:32.000000 silvio-0.2.6/docs/usage.rst
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)      427 2024-04-24 15:20:37.000000 silvio-0.2.6/setup.cfg
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)     2166 2024-04-24 14:09:55.000000 silvio-0.2.6/setup.py
+drwxrwxr-x   0 ulf       (1000) ulf       (1000)        0 2024-04-24 15:20:37.000000 silvio-0.2.6/src/
+drwxrwxr-x   0 ulf       (1000) ulf       (1000)        0 2024-04-24 15:20:37.000000 silvio-0.2.6/src/silvio/
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)     1862 2024-04-24 15:04:00.000000 silvio-0.2.6/src/silvio/__init__.py
+drwxrwxr-x   0 ulf       (1000) ulf       (1000)        0 2024-04-24 15:20:37.000000 silvio-0.2.6/src/silvio/catalog/
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)    27146 2024-02-22 13:36:50.000000 silvio-0.2.6/src/silvio/catalog/GroExpSim.py
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)    15583 2024-04-24 15:06:13.000000 silvio-0.2.6/src/silvio/catalog/RecExpSim.py
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)        0 2022-04-07 08:32:03.000000 silvio-0.2.6/src/silvio/catalog/__init__.py
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)      337 2021-11-05 13:03:32.000000 silvio-0.2.6/src/silvio/config.py
+drwxrwxr-x   0 ulf       (1000) ulf       (1000)        0 2024-04-24 15:20:37.000000 silvio-0.2.6/src/silvio/data/
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)     1212 2021-09-18 10:48:34.000000 silvio-0.2.6/src/silvio/data/CodonTriplets.csv
+drwxrwxr-x   0 ulf       (1000) ulf       (1000)        0 2024-04-24 15:20:37.000000 silvio-0.2.6/src/silvio/data/expression_predictor/
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)      327 2021-09-18 10:48:34.000000 silvio-0.2.6/src/silvio/data/expression_predictor/Ecol-Promoter-AddParams.pkl
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)   283435 2021-09-18 10:48:34.000000 silvio-0.2.6/src/silvio/data/expression_predictor/Ecol-Promoter-predictor.pkl
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)      327 2021-09-18 10:48:34.000000 silvio-0.2.6/src/silvio/data/expression_predictor/Ptai-Promoter-AddParams.pkl
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)   401243 2021-09-18 10:48:34.000000 silvio-0.2.6/src/silvio/data/expression_predictor/Ptai-Promoter-predictor.pkl
+drwxrwxr-x   0 ulf       (1000) ulf       (1000)        0 2024-04-24 15:20:37.000000 silvio-0.2.6/src/silvio/data/metabolic_model/
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)   707166 2021-09-18 10:48:34.000000 silvio-0.2.6/src/silvio/data/metabolic_model/e_coli_core.xml
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)  5116056 2021-09-18 10:48:34.000000 silvio-0.2.6/src/silvio/data/metabolic_model/iJN746.xml
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)      325 2021-11-05 13:03:32.000000 silvio-0.2.6/src/silvio/events.py
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)     1056 2021-11-05 13:03:32.000000 silvio-0.2.6/src/silvio/experiment.py
+drwxrwxr-x   0 ulf       (1000) ulf       (1000)        0 2024-04-24 15:20:37.000000 silvio-0.2.6/src/silvio/extensions/
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)        0 2021-11-05 12:56:13.000000 silvio-0.2.6/src/silvio/extensions/__init__.py
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)      592 2022-05-03 06:53:25.000000 silvio-0.2.6/src/silvio/extensions/all_events.py
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)      369 2021-11-05 12:56:13.000000 silvio-0.2.6/src/silvio/extensions/common.py
+drwxrwxr-x   0 ulf       (1000) ulf       (1000)        0 2024-04-24 15:20:37.000000 silvio-0.2.6/src/silvio/extensions/modules/
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)        0 2021-11-05 12:56:13.000000 silvio-0.2.6/src/silvio/extensions/modules/__init__.py
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)     3830 2021-11-05 13:03:32.000000 silvio-0.2.6/src/silvio/extensions/modules/genome_expression.py
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)    10146 2021-11-05 13:03:32.000000 silvio-0.2.6/src/silvio/extensions/modules/genome_library.py
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)     2153 2021-11-05 13:03:32.000000 silvio-0.2.6/src/silvio/extensions/modules/genome_list.py
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)    12598 2024-04-24 15:07:31.000000 silvio-0.2.6/src/silvio/extensions/modules/growth_behaviour.py
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)     4333 2022-05-03 07:08:02.000000 silvio-0.2.6/src/silvio/extensions/modules/metabolic_flux.py
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)     1167 2021-11-05 13:03:32.000000 silvio-0.2.6/src/silvio/extensions/modules/phenotype_size.py
+drwxrwxr-x   0 ulf       (1000) ulf       (1000)        0 2024-04-24 15:20:37.000000 silvio-0.2.6/src/silvio/extensions/records/
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)        0 2021-11-05 12:56:13.000000 silvio-0.2.6/src/silvio/extensions/records/__init__.py
+drwxrwxr-x   0 ulf       (1000) ulf       (1000)        0 2024-04-24 15:20:37.000000 silvio-0.2.6/src/silvio/extensions/records/gene/
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)        0 2021-11-05 12:56:13.000000 silvio-0.2.6/src/silvio/extensions/records/gene/__init__.py
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)     1216 2021-09-18 10:07:03.000000 silvio-0.2.6/src/silvio/extensions/records/gene/crafted_gene.py
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)      701 2021-09-18 10:07:03.000000 silvio-0.2.6/src/silvio/extensions/records/gene/gene.py
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)     2131 2021-11-05 13:03:32.000000 silvio-0.2.6/src/silvio/extensions/records/gene/localized_gene.py
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)      544 2021-11-05 13:03:32.000000 silvio-0.2.6/src/silvio/extensions/records/gene/stub_gene.py
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)      598 2021-11-05 13:03:32.000000 silvio-0.2.6/src/silvio/extensions/records/growth_record.py
+drwxrwxr-x   0 ulf       (1000) ulf       (1000)        0 2024-04-24 15:20:37.000000 silvio-0.2.6/src/silvio/extensions/sets/
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)      537 2021-11-05 13:03:32.000000 silvio-0.2.6/src/silvio/extensions/sets/__init__.py
+drwxrwxr-x   0 ulf       (1000) ulf       (1000)        0 2024-04-24 15:20:37.000000 silvio-0.2.6/src/silvio/extensions/sets/shotgun_sequencing/
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)      146 2021-11-05 13:03:32.000000 silvio-0.2.6/src/silvio/extensions/sets/shotgun_sequencing/__init__.py
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)     8044 2021-11-05 13:03:32.000000 silvio-0.2.6/src/silvio/extensions/sets/shotgun_sequencing/assembly.py
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)     7636 2021-11-05 13:03:32.000000 silvio-0.2.6/src/silvio/extensions/sets/shotgun_sequencing/datatype.py
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)     2448 2021-11-05 13:03:32.000000 silvio-0.2.6/src/silvio/extensions/sets/shotgun_sequencing/evaluation.py
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)     8849 2021-11-05 13:03:32.000000 silvio-0.2.6/src/silvio/extensions/sets/shotgun_sequencing/sequencing.py
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)     1845 2021-11-05 13:03:32.000000 silvio-0.2.6/src/silvio/extensions/sets/shotgun_sequencing/storage.py
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)     5265 2021-11-05 13:03:32.000000 silvio-0.2.6/src/silvio/extensions/sets/shotgun_sequencing/visualization.py
+drwxrwxr-x   0 ulf       (1000) ulf       (1000)        0 2024-04-24 15:20:37.000000 silvio-0.2.6/src/silvio/extensions/tools/
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)        0 2021-11-05 13:03:32.000000 silvio-0.2.6/src/silvio/extensions/tools/__init__.py
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)      202 2021-11-05 13:03:32.000000 silvio-0.2.6/src/silvio/extensions/tools/shotgun_sequencing.py
+drwxrwxr-x   0 ulf       (1000) ulf       (1000)        0 2024-04-24 15:20:37.000000 silvio-0.2.6/src/silvio/extensions/utils/
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)        0 2021-11-05 12:56:13.000000 silvio-0.2.6/src/silvio/extensions/utils/__init__.py
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)      328 2021-09-18 10:07:03.000000 silvio-0.2.6/src/silvio/extensions/utils/laboratory.py
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)     6864 2021-09-18 10:07:03.000000 silvio-0.2.6/src/silvio/extensions/utils/misc.py
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)      481 2021-11-05 13:03:32.000000 silvio-0.2.6/src/silvio/extensions/utils/shotgun_sequencing.py
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)      777 2021-09-18 10:07:03.000000 silvio-0.2.6/src/silvio/extensions/utils/transform.py
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)      506 2021-09-18 10:07:03.000000 silvio-0.2.6/src/silvio/extensions/utils/visual.py
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)     8455 2021-11-05 13:03:32.000000 silvio-0.2.6/src/silvio/host.py
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)     4163 2021-11-05 13:03:32.000000 silvio-0.2.6/src/silvio/module.py
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)     5213 2024-02-22 15:47:08.000000 silvio-0.2.6/src/silvio/outcome.py
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)     3758 2021-11-05 12:56:13.000000 silvio-0.2.6/src/silvio/random.py
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)      253 2021-11-05 13:03:32.000000 silvio-0.2.6/src/silvio/record.py
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)     1036 2021-09-18 10:07:03.000000 silvio-0.2.6/src/silvio/registry.py
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)     1550 2021-11-05 13:03:32.000000 silvio-0.2.6/src/silvio/tool.py
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)      681 2021-09-18 10:07:08.000000 silvio-0.2.6/src/silvio/utils.py
+drwxrwxr-x   0 ulf       (1000) ulf       (1000)        0 2024-04-24 15:20:37.000000 silvio-0.2.6/src/silvio.egg-info/
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)     8143 2024-04-24 15:20:37.000000 silvio-0.2.6/src/silvio.egg-info/PKG-INFO
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)     3338 2024-04-24 15:20:37.000000 silvio-0.2.6/src/silvio.egg-info/SOURCES.txt
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)        1 2024-04-24 15:20:37.000000 silvio-0.2.6/src/silvio.egg-info/dependency_links.txt
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)        1 2024-04-24 15:20:37.000000 silvio-0.2.6/src/silvio.egg-info/not-zip-safe
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)      130 2024-04-24 15:20:37.000000 silvio-0.2.6/src/silvio.egg-info/requires.txt
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)        7 2024-04-24 15:20:37.000000 silvio-0.2.6/src/silvio.egg-info/top_level.txt
+drwxrwxr-x   0 ulf       (1000) ulf       (1000)        0 2024-04-24 15:20:37.000000 silvio-0.2.6/tests/
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)       36 2021-11-05 13:03:32.000000 silvio-0.2.6/tests/__init__.py
+-rw-rw-r--   0 ulf       (1000) ulf       (1000)      477 2021-11-05 13:03:32.000000 silvio-0.2.6/tests/test_basic.py
```

### Comparing `silvio-0.2.5/CONTRIBUTING.rst` & `silvio-0.2.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/DEVNOTES.rst` & `silvio-0.2.6/DEVNOTES.rst`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/HISTORY.rst` & `silvio-0.2.6/HISTORY.rst`

 * *Files 26% similar despite different names*

```diff
@@ -62,8 +62,13 @@
 ------------------
 
 * GroExpSim, nightshift must be within 15h of experiment
 
 0.2.5 (2024-02-22)
 ------------------
 
-* GroExpSim, export single growth experiments to existing reference excel sheet
+* GroExpSim, export single growth experiments to existing reference excel sheet
+
+0.2.6 (2024-04-23)
+------------------
+
+* RecExpSim, add umax argument to 'make' in 'RecHost' for new argument demands of function 'Make_TempGrowthExp' in 'extesions/modules/growth_behaviour.py'
```

### Comparing `silvio-0.2.5/LICENSE` & `silvio-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/PKG-INFO` & `silvio-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silvio
-Version: 0.2.5
+Version: 0.2.6
 Summary: silvio is an environment for Simulation of Virtual Organisms. silvio contains several linked microbial models.
 Home-page: https://git.rwth-aachen.de/ulf.liebal/silvio.git
 Author: Ulf Liebal
 Author-email: ulf.liebal@rwth-aachen.de
 License: MIT license
 Keywords: biotechnology,microbiology,virtual cell,systems biology
 Platform: UNKNOWN
@@ -253,7 +253,12 @@
 * GroExpSim, nightshift must be within 15h of experiment
 
 0.2.5 (2024-02-22)
 ------------------
 
 * GroExpSim, export single growth experiments to existing reference excel sheet
 
+0.2.6 (2024-04-23)
+------------------
+
+* RecExpSim, add umax argument to 'make' in 'RecHost' for new argument demands of function 'Make_TempGrowthExp' in 'extesions/modules/growth_behaviour.py'
+
```

### Comparing `silvio-0.2.5/README.rst` & `silvio-0.2.6/README.rst`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/docs/Makefile` & `silvio-0.2.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/docs/conf.py` & `silvio-0.2.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/docs/design.rst` & `silvio-0.2.6/docs/design.rst`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/docs/installation.rst` & `silvio-0.2.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/docs/make.bat` & `silvio-0.2.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/docs/source/silvio.extensions.modules.rst` & `silvio-0.2.6/docs/source/silvio.extensions.modules.rst`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/docs/source/silvio.extensions.records.gene.rst` & `silvio-0.2.6/docs/source/silvio.extensions.records.gene.rst`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/docs/source/silvio.extensions.records.rst` & `silvio-0.2.6/docs/source/silvio.extensions.records.rst`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/docs/source/silvio.extensions.rst` & `silvio-0.2.6/docs/source/silvio.extensions.rst`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/docs/source/silvio.extensions.sets.shotgun_sequencing.rst` & `silvio-0.2.6/docs/source/silvio.extensions.sets.shotgun_sequencing.rst`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/docs/source/silvio.extensions.utils.rst` & `silvio-0.2.6/docs/source/silvio.extensions.utils.rst`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/docs/source/silvio.rst` & `silvio-0.2.6/docs/source/silvio.rst`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/setup.py` & `silvio-0.2.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,18 +12,19 @@
 
 requirements = [
     'biopython ~= 1.79',
     'cobra >= 0.22',
     'joblib >= 1.0',
     'matplotlib ~= 3.4',
     'numpy ~= 1.23',
-    'pandas ~= 1.2',
+    'pandas ~= 2.2',
     'pickleshare ~= 0.7',
     'scipy ~= 1.6',
     'jinja2<3.1.0',
+    'openpyxl'
 ]
 
 test_requirements = ['pytest>=3', ]
 
 # getting the latest version from the __init__.py file in src/silvio
 import re
 import os
```

### Comparing `silvio-0.2.5/src/silvio/__init__.py` & `silvio-0.2.6/src/silvio/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Make these deep classes and methods available on the top-level.
 # By convention, these are the public methods available for users of the library.
 
 # We use a written `__init__.py` file at the top level which makes deep references into sub-modules.
 # By doing this, all logic is inside this file and other __init__ files in the sub-folders can
 # stay empty.
 
-__version__='0.2.5'
+__version__='0.2.6'
 
 from .config import DATADIR
 from .experiment import Experiment, ExperimentException
 from .host import Host, HostException
 from .tool import Tool, ToolException
 from .outcome import SimulationException, Outcome, DataOutcome, DataWithPlotOutcome, combine_data
 from .random import Generator
```

### Comparing `silvio-0.2.5/src/silvio/catalog/GroExpSim.py` & `silvio-0.2.6/src/silvio/catalog/GroExpSim.py`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/src/silvio/catalog/RecExpSim.py` & `silvio-0.2.6/src/silvio/catalog/RecExpSim.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,15 @@
 
     def build_ecol_host ( self, name:str, seed:int ) -> RecHost :
         gen = Generator( seed )
         host = RecHost( name=name, seed=seed )
         host.make(
             opt_growth_temp= gen.pick_integer(25,40), # unit: degree celsius, source: https://application.wiley-vch.de/books/sample/3527335153_c01.pdf
             max_biomass= gen.pick_integer(30,100), # unit: in gDCW/l, source (german): https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=2&cad=rja&uact=8&ved=2ahUKEwjzt_aJ9pzpAhWGiqQKHb1jC6MQFjABegQIAhAB&url=https%3A%2F%2Fwww.repo.uni-hannover.de%2Fbitstream%2Fhandle%2F123456789%2F3512%2FDissertation.pdf%3Fsequence%3D1&usg=AOvVaw2XfGH11P9gK2F2B63mY4IM
+            umax = 1, # standard growth rate for easier result check
             infl_prom_str= gen.pick_integer(30,50), # explanation see Plot_ExpressionRate
             species_prom_str= 0.057,
             opt_primer_len= gen.pick_integer(16,28), # unit: nt, source: https://link.springer.com/article/10.1007/s10529-013-1249-8
             regressor_file= DATADIR / 'expression_predictor' / 'Ecol-Promoter-predictor.pkl',
             addparams_file= DATADIR / 'expression_predictor' / 'Ecol-Promoter-AddParams.pkl',
         )
         host.sync()
@@ -92,14 +93,15 @@
 
     def build_pput_host ( self, name:str, seed:int ) -> RecHost :
         gen = Generator( seed )
         host = RecHost( name=name, seed=seed )
         host.make(
             opt_growth_temp= gen.pick_integer(25,40), # unit: degree celsius, source: https://application.wiley-vch.de/books/sample/3527335153_c01.pdf
             max_biomass= gen.pick_integer(45,145), # unit: in gDCW/l, source 1: https://onlinelibrary.wiley.com/doi/pdf/10.1002/bit.25474, source 2: https://link.springer.com/article/10.1385/ABAB:119:1:51
+            umax = 1, # standard growth rate for easier result check
             infl_prom_str= gen.pick_integer(30,50), # explanation see Plot_ExpressionRate
             species_prom_str= 0.04,
             opt_primer_len= gen.pick_integer(16,28), # unit: nt, source: https://link.springer.com/article/10.1007/s10529-013-1249-8
             regressor_file= DATADIR / 'expression_predictor' / 'Ptai-Promoter-predictor.pkl',
             addparams_file= DATADIR / 'expression_predictor' / 'Ptai-Promoter-AddParams.pkl',
         )
         host.sync()
@@ -277,15 +279,15 @@
     genexpr: GenomeExpression
 
     ref_prom:str = 'GCCCATTGACAAGGCTCTCGCGGCCAGGTATAATTGCACG'
 
 
 
     def make ( self,
-        opt_growth_temp:int, max_biomass:int,
+        opt_growth_temp:int, max_biomass:int, umax:float,
         infl_prom_str:int, species_prom_str:int, opt_primer_len:int,
         regressor_file:Path, addparams_file:Path
     ) -> None :
 
         if not alldef( opt_growth_temp, max_biomass, infl_prom_str, species_prom_str, opt_primer_len, regressor_file, addparams_file ) :
             raise HostException("Host not initialized. Reason: incomplete arguments.")
 
@@ -305,15 +307,16 @@
         )
         self.genexpr.bind( host=self, genome=self.genome )
 
         # Setup GrowthBehaviour module
         self.growth = GrowthBehaviour()
         self.growth.make(
             opt_growth_temp=opt_growth_temp,
-            max_biomass=max_biomass
+            max_biomass=max_biomass,
+            umax = umax
         )
         self.growth.bind( host=self, genexpr=self.genexpr )
 
 
 
     def copy ( self, ref:RecHost ) -> None :
```

### Comparing `silvio-0.2.5/src/silvio/data/CodonTriplets.csv` & `silvio-0.2.6/src/silvio/data/CodonTriplets.csv`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/src/silvio/data/expression_predictor/Ecol-Promoter-predictor.pkl` & `silvio-0.2.6/src/silvio/data/expression_predictor/Ecol-Promoter-predictor.pkl`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/src/silvio/data/expression_predictor/Ptai-Promoter-predictor.pkl` & `silvio-0.2.6/src/silvio/data/expression_predictor/Ptai-Promoter-predictor.pkl`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/src/silvio/data/metabolic_model/e_coli_core.xml` & `silvio-0.2.6/src/silvio/data/metabolic_model/e_coli_core.xml`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/src/silvio/data/metabolic_model/iJN746.xml` & `silvio-0.2.6/src/silvio/data/metabolic_model/iJN746.xml`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/src/silvio/experiment.py` & `silvio-0.2.6/src/silvio/experiment.py`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/src/silvio/extensions/all_events.py` & `silvio-0.2.6/src/silvio/extensions/all_events.py`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/src/silvio/extensions/modules/genome_expression.py` & `silvio-0.2.6/src/silvio/extensions/modules/genome_expression.py`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/src/silvio/extensions/modules/genome_library.py` & `silvio-0.2.6/src/silvio/extensions/modules/genome_library.py`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/src/silvio/extensions/modules/genome_list.py` & `silvio-0.2.6/src/silvio/extensions/modules/genome_list.py`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/src/silvio/extensions/modules/growth_behaviour.py` & `silvio-0.2.6/src/silvio/extensions/modules/growth_behaviour.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,17 +34,18 @@
     # Monod Yield coefficient
     Yxs: float
     # Monod Maximum growth rate
     umax: float
 
 
 
-    def make ( self, opt_growth_temp:int, max_biomass:int ) -> None :
+    def make ( self, opt_growth_temp:int, max_biomass:int, umax:float ) -> None :
         self.opt_growth_temp = opt_growth_temp
         self.max_biomass = max_biomass
+        self.umax = umax
 
     def make2 ( self, opt_growth_temp:int, max_biomass:int , Ks:float, Yxs:float, k1:float, umax:float, OD2X ) -> None :
         self.opt_growth_temp = opt_growth_temp
         self.max_biomass = max_biomass
         self.Ks = Ks
         self.Yxs = Yxs
         self.k1 = k1
```

### Comparing `silvio-0.2.5/src/silvio/extensions/modules/metabolic_flux.py` & `silvio-0.2.6/src/silvio/extensions/modules/metabolic_flux.py`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/src/silvio/extensions/modules/phenotype_size.py` & `silvio-0.2.6/src/silvio/extensions/modules/phenotype_size.py`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/src/silvio/extensions/records/gene/crafted_gene.py` & `silvio-0.2.6/src/silvio/extensions/records/gene/crafted_gene.py`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/src/silvio/extensions/records/gene/gene.py` & `silvio-0.2.6/src/silvio/extensions/records/gene/gene.py`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/src/silvio/extensions/records/gene/localized_gene.py` & `silvio-0.2.6/src/silvio/extensions/records/gene/localized_gene.py`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/src/silvio/extensions/records/gene/stub_gene.py` & `silvio-0.2.6/src/silvio/extensions/records/gene/stub_gene.py`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/src/silvio/extensions/records/growth_record.py` & `silvio-0.2.6/src/silvio/extensions/records/growth_record.py`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/src/silvio/extensions/sets/__init__.py` & `silvio-0.2.6/src/silvio/extensions/sets/__init__.py`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/src/silvio/extensions/sets/shotgun_sequencing/assembly.py` & `silvio-0.2.6/src/silvio/extensions/sets/shotgun_sequencing/assembly.py`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/src/silvio/extensions/sets/shotgun_sequencing/datatype.py` & `silvio-0.2.6/src/silvio/extensions/sets/shotgun_sequencing/datatype.py`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/src/silvio/extensions/sets/shotgun_sequencing/evaluation.py` & `silvio-0.2.6/src/silvio/extensions/sets/shotgun_sequencing/evaluation.py`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/src/silvio/extensions/sets/shotgun_sequencing/sequencing.py` & `silvio-0.2.6/src/silvio/extensions/sets/shotgun_sequencing/sequencing.py`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/src/silvio/extensions/sets/shotgun_sequencing/storage.py` & `silvio-0.2.6/src/silvio/extensions/sets/shotgun_sequencing/storage.py`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/src/silvio/extensions/sets/shotgun_sequencing/visualization.py` & `silvio-0.2.6/src/silvio/extensions/sets/shotgun_sequencing/visualization.py`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/src/silvio/extensions/utils/misc.py` & `silvio-0.2.6/src/silvio/extensions/utils/misc.py`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/src/silvio/extensions/utils/transform.py` & `silvio-0.2.6/src/silvio/extensions/utils/transform.py`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/src/silvio/host.py` & `silvio-0.2.6/src/silvio/host.py`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/src/silvio/module.py` & `silvio-0.2.6/src/silvio/module.py`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/src/silvio/outcome.py` & `silvio-0.2.6/src/silvio/outcome.py`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/src/silvio/random.py` & `silvio-0.2.6/src/silvio/random.py`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/src/silvio/registry.py` & `silvio-0.2.6/src/silvio/registry.py`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/src/silvio/tool.py` & `silvio-0.2.6/src/silvio/tool.py`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/src/silvio/utils.py` & `silvio-0.2.6/src/silvio/utils.py`

 * *Files identical despite different names*

### Comparing `silvio-0.2.5/src/silvio.egg-info/PKG-INFO` & `silvio-0.2.6/src/silvio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silvio
-Version: 0.2.5
+Version: 0.2.6
 Summary: silvio is an environment for Simulation of Virtual Organisms. silvio contains several linked microbial models.
 Home-page: https://git.rwth-aachen.de/ulf.liebal/silvio.git
 Author: Ulf Liebal
 Author-email: ulf.liebal@rwth-aachen.de
 License: MIT license
 Keywords: biotechnology,microbiology,virtual cell,systems biology
 Platform: UNKNOWN
@@ -253,7 +253,12 @@
 * GroExpSim, nightshift must be within 15h of experiment
 
 0.2.5 (2024-02-22)
 ------------------
 
 * GroExpSim, export single growth experiments to existing reference excel sheet
 
+0.2.6 (2024-04-23)
+------------------
+
+* RecExpSim, add umax argument to 'make' in 'RecHost' for new argument demands of function 'Make_TempGrowthExp' in 'extesions/modules/growth_behaviour.py'
+
```

### Comparing `silvio-0.2.5/src/silvio.egg-info/SOURCES.txt` & `silvio-0.2.6/src/silvio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

