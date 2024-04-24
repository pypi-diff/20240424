# Comparing `tmp/antelope_core-0.3.0.tar.gz` & `tmp/antelope_core-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antelope_core-0.3.0.tar", last modified: Thu Mar 21 22:37:35 2024, max compression
+gzip compressed data, was "antelope_core-0.3.1.tar", last modified: Thu Apr 18 21:39:25 2024, max compression
```

## Comparing `antelope_core-0.3.0.tar` & `antelope_core-0.3.1.tar`

### file list

```diff
@@ -1,192 +1,192 @@
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.467665 antelope_core-0.3.0/
--rw-r--r--   0 b          (500) b          (506)     1520 2020-09-25 22:29:55.000000 antelope_core-0.3.0/LICENSE
--rw-r--r--   0 b          (500) b          (506)      335 2023-07-21 21:37:06.000000 antelope_core-0.3.0/MANIFEST.in
--rw-r--r--   0 b          (500) b          (506)    14232 2024-03-21 22:37:35.467665 antelope_core-0.3.0/PKG-INFO
--rw-r--r--   0 b          (500) b          (506)    13586 2023-07-21 21:50:10.000000 antelope_core-0.3.0/README.md
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.450998 antelope_core-0.3.0/antelope_core/
--rw-r--r--   0 b          (500) b          (506)     3264 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/__init__.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.450998 antelope_core-0.3.0/antelope_core/archives/
--rw-r--r--   0 b          (500) b          (506)     4638 2024-03-20 22:20:51.000000 antelope_core-0.3.0/antelope_core/archives/__init__.py
--rw-r--r--   0 b          (500) b          (506)     2364 2023-07-21 21:37:06.000000 antelope_core-0.3.0/antelope_core/archives/archive_index.py
--rw-r--r--   0 b          (500) b          (506)    19543 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/archives/basic_archive.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.450998 antelope_core-0.3.0/antelope_core/archives/data/
--rw-r--r--   0 b          (500) b          (506)    27954 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/archives/data/elcd_reference_quantities.json
--rw-r--r--   0 b          (500) b          (506)    28771 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/archives/entity_store.py
--rw-r--r--   0 b          (500) b          (506)     6288 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/archives/lc_archive.py
--rw-r--r--   0 b          (500) b          (506)     6744 2024-03-21 02:23:41.000000 antelope_core-0.3.0/antelope_core/archives/quantity_manager.py
--rw-r--r--   0 b          (500) b          (506)    43106 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/archives/term_manager.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.454331 antelope_core-0.3.0/antelope_core/archives/tests/
--rw-r--r--   0 b          (500) b          (506)       54 2019-02-15 00:01:58.000000 antelope_core-0.3.0/antelope_core/archives/tests/__init__.py
--rw-r--r--   0 b          (500) b          (506)     8577 2020-03-30 08:22:53.000000 antelope_core-0.3.0/antelope_core/archives/tests/test_base.py
--rw-r--r--   0 b          (500) b          (506)     3557 2023-07-21 21:37:06.000000 antelope_core-0.3.0/antelope_core/archives/tests/test_basic_archive.py
--rw-r--r--   0 b          (500) b          (506)     1802 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/archives/tests/test_entity_store.py
--rw-r--r--   0 b          (500) b          (506)     4143 2019-04-05 22:10:51.000000 antelope_core-0.3.0/antelope_core/archives/tests/test_json.json
--rw-r--r--   0 b          (500) b          (506)     2442 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/archives/tests/test_qdb.py
--rw-r--r--   0 b          (500) b          (506)     3044 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/archives/tests/test_quantity_manager.py
--rw-r--r--   0 b          (500) b          (506)     2286 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/archives/tests/test_quantity_relation.py
--rw-r--r--   0 b          (500) b          (506)     3013 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/archives/tests/test_term_manager.py
--rw-r--r--   0 b          (500) b          (506)     4101 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/autorange.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.454331 antelope_core-0.3.0/antelope_core/catalog/
--rw-r--r--   0 b          (500) b          (506)       70 2023-07-21 21:37:06.000000 antelope_core-0.3.0/antelope_core/catalog/__init__.py
--rw-r--r--   0 b          (500) b          (506)    18519 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/catalog/catalog.py
--rw-r--r--   0 b          (500) b          (506)      628 2020-11-05 08:47:12.000000 antelope_core-0.3.0/antelope_core/catalog/catalog_root.py
--rw-r--r--   0 b          (500) b          (506)     6104 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/catalog/configurator.py
--rw-r--r--   0 b          (500) b          (506)    22430 2024-03-21 19:57:40.000000 antelope_core-0.3.0/antelope_core/catalog/lc_catalog.py
--rw-r--r--   0 b          (500) b          (506)     8782 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/catalog/lc_resolver.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.454331 antelope_core-0.3.0/antelope_core/catalog/tests/
--rw-r--r--   0 b          (500) b          (506)        0 2018-07-26 08:24:01.000000 antelope_core-0.3.0/antelope_core/catalog/tests/__init__.py
--rw-r--r--   0 b          (500) b          (506)     5139 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/catalog/tests/test_catalogs.py
--rw-r--r--   0 b          (500) b          (506)     2316 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/catalog/tests/test_process_ref.py
--rw-r--r--   0 b          (500) b          (506)     1624 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/catalog/tests/test_quantity_refs.py
--rw-r--r--   0 b          (500) b          (506)    18075 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/catalog_query.py
--rw-r--r--   0 b          (500) b          (506)    10746 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/characterizations.py
--rw-r--r--   0 b          (500) b          (506)    17778 2024-03-20 22:20:51.000000 antelope_core-0.3.0/antelope_core/contexts.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.454331 antelope_core-0.3.0/antelope_core/data_sources/
--rw-r--r--   0 b          (500) b          (506)        0 2018-10-26 21:44:35.000000 antelope_core-0.3.0/antelope_core/data_sources/__init__.py
--rw-r--r--   0 b          (500) b          (506)     3851 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/data_sources/data_source.py
--rw-r--r--   0 b          (500) b          (506)     7497 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/data_sources/ecoinvent.py
--rw-r--r--   0 b          (500) b          (506)     1741 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/data_sources/ecoinvent_lcia.py
--rw-r--r--   0 b          (500) b          (506)     1303 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/data_sources/gwp_ipcc_2007.py
--rw-r--r--   0 b          (500) b          (506)     4614 2020-11-05 09:30:15.000000 antelope_core-0.3.0/antelope_core/data_sources/local.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.454331 antelope_core-0.3.0/antelope_core/data_sources/tests/
--rw-r--r--   0 b          (500) b          (506)        0 2018-10-26 21:44:35.000000 antelope_core-0.3.0/antelope_core/data_sources/tests/__init__.py
--rw-r--r--   0 b          (500) b          (506)     4159 2024-03-20 22:20:51.000000 antelope_core-0.3.0/antelope_core/data_sources/tests/test_aa_local.py
--rw-r--r--   0 b          (500) b          (506)     1541 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/data_sources/tests/test_ecoinvent.py
--rw-r--r--   0 b          (500) b          (506)     7319 2021-07-08 16:41:41.000000 antelope_core-0.3.0/antelope_core/data_sources/tests/test_ecoinvent_lci.py
--rw-r--r--   0 b          (500) b          (506)      815 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/data_sources/tests/test_ipcc2007.py
--rw-r--r--   0 b          (500) b          (506)     1999 2024-03-20 22:20:51.000000 antelope_core-0.3.0/antelope_core/data_sources/tests/test_traci.py
--rw-r--r--   0 b          (500) b          (506)     7401 2024-03-20 22:20:51.000000 antelope_core-0.3.0/antelope_core/data_sources/tests/test_uslci.py
--rw-r--r--   0 b          (500) b          (506)     2438 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/data_sources/traci.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.457665 antelope_core-0.3.0/antelope_core/data_sources/uslci/
--rw-r--r--   0 b          (500) b          (506)       31 2020-12-29 09:58:58.000000 antelope_core-0.3.0/antelope_core/data_sources/uslci/__init__.py
--rw-r--r--   0 b          (500) b          (506)     6853 2024-03-21 02:23:41.000000 antelope_core-0.3.0/antelope_core/data_sources/uslci/uslci.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.457665 antelope_core-0.3.0/antelope_core/entities/
--rw-r--r--   0 b          (500) b          (506)      181 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/entities/__init__.py
--rw-r--r--   0 b          (500) b          (506)    11763 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/entities/entities.py
--rw-r--r--   0 b          (500) b          (506)     4408 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/entities/flows.py
--rw-r--r--   0 b          (500) b          (506)    25036 2024-03-20 22:20:51.000000 antelope_core-0.3.0/antelope_core/entities/processes.py
--rw-r--r--   0 b          (500) b          (506)     7969 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/entities/quantities.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.457665 antelope_core-0.3.0/antelope_core/entities/tests/
--rw-r--r--   0 b          (500) b          (506)       62 2019-02-15 00:01:58.000000 antelope_core-0.3.0/antelope_core/entities/tests/__init__.py
--rw-r--r--   0 b          (500) b          (506)     1065 2021-01-07 23:11:04.000000 antelope_core-0.3.0/antelope_core/entities/tests/base_testclass.py
--rw-r--r--   0 b          (500) b          (506)    99145 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/entities/tests/test_archive.json
--rw-r--r--   0 b          (500) b          (506)     1019 2020-03-30 08:22:53.000000 antelope_core-0.3.0/antelope_core/entities/tests/test_entities.py
--rw-r--r--   0 b          (500) b          (506)      850 2020-12-29 09:58:58.000000 antelope_core-0.3.0/antelope_core/entities/tests/test_entity_refs.py
--rw-r--r--   0 b          (500) b          (506)      291 2020-03-30 08:22:53.000000 antelope_core-0.3.0/antelope_core/entities/tests/test_flows.py
--rw-r--r--   0 b          (500) b          (506)     1538 2020-03-30 08:22:53.000000 antelope_core-0.3.0/antelope_core/entities/tests/test_processes.py
--rw-r--r--   0 b          (500) b          (506)     1565 2020-09-29 22:38:38.000000 antelope_core-0.3.0/antelope_core/entities/tests/test_quantities.py
--rw-r--r--   0 b          (500) b          (506)    18234 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/entities/xlsx_editor.py
--rw-r--r--   0 b          (500) b          (506)    22640 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/exchanges.py
--rw-r--r--   0 b          (500) b          (506)     6756 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/file_accessor.py
--rw-r--r--   0 b          (500) b          (506)     1137 2023-07-21 21:37:06.000000 antelope_core-0.3.0/antelope_core/from_json.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.457665 antelope_core-0.3.0/antelope_core/implementations/
--rw-r--r--   0 b          (500) b          (506)      333 2023-07-21 21:37:06.000000 antelope_core-0.3.0/antelope_core/implementations/__init__.py
--rw-r--r--   0 b          (500) b          (506)     8735 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/implementations/background.py
--rw-r--r--   0 b          (500) b          (506)     6114 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/implementations/basic.py
--rw-r--r--   0 b          (500) b          (506)    10035 2024-03-20 22:20:51.000000 antelope_core-0.3.0/antelope_core/implementations/configure.py
--rw-r--r--   0 b          (500) b          (506)     2812 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/implementations/exchange.py
--rw-r--r--   0 b          (500) b          (506)     6800 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/implementations/index.py
--rw-r--r--   0 b          (500) b          (506)    32892 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/implementations/quantity.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.457665 antelope_core-0.3.0/antelope_core/implementations/tests/
--rw-r--r--   0 b          (500) b          (506)        0 2018-09-13 20:45:30.000000 antelope_core-0.3.0/antelope_core/implementations/tests/__init__.py
--rw-r--r--   0 b          (500) b          (506)     2056 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/implementations/tests/test_quantity.py
--rw-r--r--   0 b          (500) b          (506)    16915 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/lc_resource.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.460998 antelope_core-0.3.0/antelope_core/lcia_engine/
--rw-r--r--   0 b          (500) b          (506)     5682 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/lcia_engine/__init__.py
--rw-r--r--   0 b          (500) b          (506)     8163 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/lcia_engine/clookup.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.460998 antelope_core-0.3.0/antelope_core/lcia_engine/data/
--rw-r--r--   0 b          (500) b          (506)     8401 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/lcia_engine/data/contexts.json
--rw-r--r--   0 b          (500) b          (506)   383481 2020-03-30 08:22:53.000000 antelope_core-0.3.0/antelope_core/lcia_engine/data/flowables.json
--rw-r--r--   0 b          (500) b          (506)    30980 2021-01-07 00:24:41.000000 antelope_core-0.3.0/antelope_core/lcia_engine/data/ipcc_2007_gwp.json
--rw-r--r--   0 b          (500) b          (506)    18280 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/lcia_engine/lcia_engine.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.460998 antelope_core-0.3.0/antelope_core/lcia_engine/tests/
--rw-r--r--   0 b          (500) b          (506)        0 2020-03-30 08:22:53.000000 antelope_core-0.3.0/antelope_core/lcia_engine/tests/__init__.py
--rw-r--r--   0 b          (500) b          (506)     1645 2024-03-20 22:20:51.000000 antelope_core-0.3.0/antelope_core/lcia_engine/tests/test_biogenic_co2.py
--rw-r--r--   0 b          (500) b          (506)     2559 2020-03-30 08:22:53.000000 antelope_core-0.3.0/antelope_core/lcia_engine/tests/test_clookup.py
--rw-r--r--   0 b          (500) b          (506)      924 2020-09-29 22:38:38.000000 antelope_core-0.3.0/antelope_core/lcia_engine/tests/test_ipcc.py
--rw-r--r--   0 b          (500) b          (506)     2981 2023-07-21 21:37:06.000000 antelope_core-0.3.0/antelope_core/lcia_engine/tests/test_lcia_engine.py
--rw-r--r--   0 b          (500) b          (506)    45982 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/lcia_results.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.460998 antelope_core-0.3.0/antelope_core/providers/
--rw-r--r--   0 b          (500) b          (506)     4643 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/providers/__init__.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.460998 antelope_core-0.3.0/antelope_core/providers/data/
--rw-r--r--   0 b          (500) b          (506)       57 2019-02-15 00:01:58.000000 antelope_core-0.3.0/antelope_core/providers/data/__init__.py
--rw-r--r--   0 b          (500) b          (506)    39336 2018-07-26 08:24:01.000000 antelope_core-0.3.0/antelope_core/providers/data/list_of_methods_and_indicators_ecoinvent_v3.2.xlsx
--rw-r--r--   0 b          (500) b          (506)    95429 2019-02-15 00:01:58.000000 antelope_core-0.3.0/antelope_core/providers/data/traci_2_1_2014_dec_10_0_test.xlsx
--rw-r--r--   0 b          (500) b          (506)     9551 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/providers/ecoinvent_lcia.py
--rw-r--r--   0 b          (500) b          (506)    11083 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/providers/ecospold.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.464331 antelope_core-0.3.0/antelope_core/providers/ecospold2/
--rw-r--r--   0 b          (500) b          (506)       41 2018-07-26 08:24:01.000000 antelope_core-0.3.0/antelope_core/providers/ecospold2/__init__.py
--rw-r--r--   0 b          (500) b          (506)    24560 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/providers/ecospold2/ecospold2.py
--rw-r--r--   0 b          (500) b          (506)      564 2020-10-18 05:43:46.000000 antelope_core-0.3.0/antelope_core/providers/ecospold2/ecospold2_index.py
--rw-r--r--   0 b          (500) b          (506)     2134 2020-03-30 08:22:53.000000 antelope_core-0.3.0/antelope_core/providers/ecospold2/master_data.py
--rw-r--r--   0 b          (500) b          (506)    10917 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/providers/file_store.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.464331 antelope_core-0.3.0/antelope_core/providers/ilcd/
--rw-r--r--   0 b          (500) b          (506)       78 2018-07-26 08:24:01.000000 antelope_core-0.3.0/antelope_core/providers/ilcd/__init__.py
--rw-r--r--   0 b          (500) b          (506)    17683 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/providers/ilcd/ilcd.py
--rw-r--r--   0 b          (500) b          (506)     2314 2018-07-26 08:24:01.000000 antelope_core-0.3.0/antelope_core/providers/ilcd/ilcd_flowables.py
--rw-r--r--   0 b          (500) b          (506)     5806 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/providers/ilcd/ilcd_lcia.py
--rw-r--r--   0 b          (500) b          (506)      314 2020-09-29 23:36:41.000000 antelope_core-0.3.0/antelope_core/providers/ilcd/index.py
--rw-r--r--   0 b          (500) b          (506)     3177 2023-07-21 21:37:06.000000 antelope_core-0.3.0/antelope_core/providers/ilcd/quantity.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.464331 antelope_core-0.3.0/antelope_core/providers/ilcd/tests/
--rw-r--r--   0 b          (500) b          (506)        0 2021-01-07 00:24:41.000000 antelope_core-0.3.0/antelope_core/providers/ilcd/tests/__init__.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.450998 antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.450998 antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.450998 antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.464331 antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/
--rw-r--r--   0 b          (500) b          (506)     2712 2019-02-15 00:01:58.000000 antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-11da-a746-0800200b9a66.xml
--rw-r--r--   0 b          (500) b          (506)     2738 2019-02-15 00:01:58.000000 antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-11da-a746-0800200c9a66.xml
--rw-r--r--   0 b          (500) b          (506)     2734 2019-02-15 00:01:58.000000 antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-13da-a746-0800200c9a66.xml
--rw-r--r--   0 b          (500) b          (506)     2716 2019-02-15 00:01:58.000000 antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-22da-a746-0800200c9a66.xml
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.464331 antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flows/
--rw-r--r--   0 b          (500) b          (506)     5078 2019-02-15 00:01:58.000000 antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flows/f579de8c-8897-4bdb-9a0a-b36f8b13282e.xml
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.464331 antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/
--rw-r--r--   0 b          (500) b          (506)     2503 2019-02-15 00:01:58.000000 antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/1ff9a08c-6fc1-4509-8bcd-a5404c598755.xml
--rw-r--r--   0 b          (500) b          (506)     3551 2019-02-15 00:01:58.000000 antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/ad38d542-3fe9-439d-9b95-2f5f7752acaf.xml
--rw-r--r--   0 b          (500) b          (506)     3344 2019-02-15 00:01:58.000000 antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/cd950537-0a98-4044-9ba7-9f9a68d0a504.xml
--rw-r--r--   0 b          (500) b          (506)     4443 2019-02-15 00:01:58.000000 antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/de5104d8-3de0-4218-a29d-b7123ce9ca3c.xml
--rw-r--r--   0 b          (500) b          (506)      932 2021-01-07 00:24:41.000000 antelope_core-0.3.0/antelope_core/providers/ilcd/tests/test_ilcd.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.464331 antelope_core-0.3.0/antelope_core/providers/openlca/
--rw-r--r--   0 b          (500) b          (506)       91 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/providers/openlca/__init__.py
--rw-r--r--   0 b          (500) b          (506)     4887 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/providers/openlca/olca_accessor.py
--rw-r--r--   0 b          (500) b          (506)    12011 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/providers/openlca/olca_ref_data.py
--rw-r--r--   0 b          (500) b          (506)    24980 2024-03-20 22:20:51.000000 antelope_core-0.3.0/antelope_core/providers/openlca/openlca_jsonld.py
--rw-r--r--   0 b          (500) b          (506)      775 2024-03-20 22:20:51.000000 antelope_core-0.3.0/antelope_core/providers/openlca/schema_mapping.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.464331 antelope_core-0.3.0/antelope_core/providers/openlca/tests/
--rw-r--r--   0 b          (500) b          (506)        0 2024-01-05 07:24:59.000000 antelope_core-0.3.0/antelope_core/providers/openlca/tests/__init__.py
--rw-r--r--   0 b          (500) b          (506)       83 2024-01-05 07:57:07.000000 antelope_core-0.3.0/antelope_core/providers/openlca/tests/test_olca_ref.py
--rw-r--r--   0 b          (500) b          (506)      729 2023-07-21 21:37:06.000000 antelope_core-0.3.0/antelope_core/providers/parse_math.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.467665 antelope_core-0.3.0/antelope_core/providers/tests/
--rw-r--r--   0 b          (500) b          (506)        0 2018-07-26 08:24:01.000000 antelope_core-0.3.0/antelope_core/providers/tests/__init__.py
--rw-r--r--   0 b          (500) b          (506)      569 2020-09-29 23:35:54.000000 antelope_core-0.3.0/antelope_core/providers/tests/test_ecospold.py
--rw-r--r--   0 b          (500) b          (506)     4110 2018-07-26 08:24:01.000000 antelope_core-0.3.0/antelope_core/providers/tests/test_xml_widgets.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.467665 antelope_core-0.3.0/antelope_core/providers/traci/
--rw-r--r--   0 b          (500) b          (506)       50 2018-07-26 08:24:01.000000 antelope_core-0.3.0/antelope_core/providers/traci/__init__.py
--rw-r--r--   0 b          (500) b          (506)      653 2020-09-29 23:35:54.000000 antelope_core-0.3.0/antelope_core/providers/traci/index.py
--rw-r--r--   0 b          (500) b          (506)     3441 2019-01-17 18:55:10.000000 antelope_core-0.3.0/antelope_core/providers/traci/q_info.py
--rw-r--r--   0 b          (500) b          (506)     2076 2020-09-29 23:35:54.000000 antelope_core-0.3.0/antelope_core/providers/traci/quantity.py
--rw-r--r--   0 b          (500) b          (506)     1648 2020-03-30 08:22:53.000000 antelope_core-0.3.0/antelope_core/providers/traci/test_traci.py
--rw-r--r--   0 b          (500) b          (506)     6687 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/providers/traci/traci_2_1_spreadsheet.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.467665 antelope_core-0.3.0/antelope_core/providers/xdb_client/
--rw-r--r--   0 b          (500) b          (506)       67 2023-08-19 07:49:00.000000 antelope_core-0.3.0/antelope_core/providers/xdb_client/__init__.py
--rw-r--r--   0 b          (500) b          (506)    16888 2024-03-21 05:35:17.000000 antelope_core-0.3.0/antelope_core/providers/xdb_client/implementation.py
--rw-r--r--   0 b          (500) b          (506)     4447 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/providers/xdb_client/requester.py
--rw-r--r--   0 b          (500) b          (506)     7202 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/providers/xdb_client/rest_client.py
--rw-r--r--   0 b          (500) b          (506)     7616 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/providers/xdb_client/xdb_client.py
--rw-r--r--   0 b          (500) b          (506)     3971 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/providers/xdb_client/xdb_entities.py
--rw-r--r--   0 b          (500) b          (506)     2316 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/providers/xl_dict.py
--rw-r--r--   0 b          (500) b          (506)     1676 2020-03-30 08:22:53.000000 antelope_core-0.3.0/antelope_core/providers/xml_widgets.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.467665 antelope_core-0.3.0/antelope_core/tests/
--rw-r--r--   0 b          (500) b          (506)        0 2018-07-26 08:24:01.000000 antelope_core-0.3.0/antelope_core/tests/__init__.py
--rw-r--r--   0 b          (500) b          (506)     1007 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/tests/test_autorange.py
--rw-r--r--   0 b          (500) b          (506)    13194 2024-03-20 22:20:51.000000 antelope_core-0.3.0/antelope_core/tests/test_contexts.py
--rw-r--r--   0 b          (500) b          (506)     5637 2020-12-29 09:58:58.000000 antelope_core-0.3.0/antelope_core/tests/test_exchanges.py
--rw-r--r--   0 b          (500) b          (506)      500 2020-12-29 09:58:58.000000 antelope_core-0.3.0/antelope_core/tests/test_lcia_results.py
--rw-r--r--   0 b          (500) b          (506)     1162 2020-09-30 00:02:12.000000 antelope_core-0.3.0/antelope_core/tests/test_resources.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.450998 antelope_core-0.3.0/antelope_core.egg-info/
--rw-r--r--   0 b          (500) b          (506)    14232 2024-03-21 22:37:35.000000 antelope_core-0.3.0/antelope_core.egg-info/PKG-INFO
--rw-r--r--   0 b          (500) b          (506)     7084 2024-03-21 22:37:35.000000 antelope_core-0.3.0/antelope_core.egg-info/SOURCES.txt
--rw-r--r--   0 b          (500) b          (506)        1 2024-03-21 22:37:35.000000 antelope_core-0.3.0/antelope_core.egg-info/dependency_links.txt
--rw-r--r--   0 b          (500) b          (506)      169 2024-03-21 22:37:35.000000 antelope_core-0.3.0/antelope_core.egg-info/requires.txt
--rw-r--r--   0 b          (500) b          (506)       14 2024-03-21 22:37:35.000000 antelope_core-0.3.0/antelope_core.egg-info/top_level.txt
--rw-r--r--   0 b          (500) b          (506)       38 2024-03-21 22:37:35.467665 antelope_core-0.3.0/setup.cfg
--rw-r--r--   0 b          (500) b          (506)     3723 2024-03-21 02:23:39.000000 antelope_core-0.3.0/setup.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:39:25.389961 antelope_core-0.3.1/
+-rw-r--r--   0 b          (500) b          (506)     1520 2020-09-25 22:29:55.000000 antelope_core-0.3.1/LICENSE
+-rw-r--r--   0 b          (500) b          (506)      335 2023-07-21 21:37:06.000000 antelope_core-0.3.1/MANIFEST.in
+-rw-r--r--   0 b          (500) b          (506)    14539 2024-04-18 21:39:25.389961 antelope_core-0.3.1/PKG-INFO
+-rw-r--r--   0 b          (500) b          (506)    13586 2023-07-21 21:50:10.000000 antelope_core-0.3.1/README.md
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:39:25.379961 antelope_core-0.3.1/antelope_core/
+-rw-r--r--   0 b          (500) b          (506)     3264 2024-04-18 21:33:40.000000 antelope_core-0.3.1/antelope_core/__init__.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:39:25.379961 antelope_core-0.3.1/antelope_core/archives/
+-rw-r--r--   0 b          (500) b          (506)     4638 2024-03-20 22:20:51.000000 antelope_core-0.3.1/antelope_core/archives/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     2526 2024-04-18 21:33:40.000000 antelope_core-0.3.1/antelope_core/archives/archive_index.py
+-rw-r--r--   0 b          (500) b          (506)    19740 2024-04-18 21:33:40.000000 antelope_core-0.3.1/antelope_core/archives/basic_archive.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:39:25.379961 antelope_core-0.3.1/antelope_core/archives/data/
+-rw-r--r--   0 b          (500) b          (506)    27954 2024-04-18 21:33:40.000000 antelope_core-0.3.1/antelope_core/archives/data/elcd_reference_quantities.json
+-rw-r--r--   0 b          (500) b          (506)    28771 2023-07-21 21:50:10.000000 antelope_core-0.3.1/antelope_core/archives/entity_store.py
+-rw-r--r--   0 b          (500) b          (506)     6288 2023-07-21 21:50:10.000000 antelope_core-0.3.1/antelope_core/archives/lc_archive.py
+-rw-r--r--   0 b          (500) b          (506)     6744 2024-04-18 21:33:40.000000 antelope_core-0.3.1/antelope_core/archives/quantity_manager.py
+-rw-r--r--   0 b          (500) b          (506)    43313 2024-04-18 21:33:40.000000 antelope_core-0.3.1/antelope_core/archives/term_manager.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:39:25.379961 antelope_core-0.3.1/antelope_core/archives/tests/
+-rw-r--r--   0 b          (500) b          (506)       54 2019-02-15 00:01:58.000000 antelope_core-0.3.1/antelope_core/archives/tests/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     8577 2020-03-30 08:22:53.000000 antelope_core-0.3.1/antelope_core/archives/tests/test_base.py
+-rw-r--r--   0 b          (500) b          (506)     3557 2023-07-21 21:37:06.000000 antelope_core-0.3.1/antelope_core/archives/tests/test_basic_archive.py
+-rw-r--r--   0 b          (500) b          (506)     1802 2023-07-21 21:50:10.000000 antelope_core-0.3.1/antelope_core/archives/tests/test_entity_store.py
+-rw-r--r--   0 b          (500) b          (506)     4143 2019-04-05 22:10:51.000000 antelope_core-0.3.1/antelope_core/archives/tests/test_json.json
+-rw-r--r--   0 b          (500) b          (506)     2442 2024-04-18 21:33:40.000000 antelope_core-0.3.1/antelope_core/archives/tests/test_qdb.py
+-rw-r--r--   0 b          (500) b          (506)     3044 2023-07-21 21:50:10.000000 antelope_core-0.3.1/antelope_core/archives/tests/test_quantity_manager.py
+-rw-r--r--   0 b          (500) b          (506)     2286 2023-07-21 21:50:10.000000 antelope_core-0.3.1/antelope_core/archives/tests/test_quantity_relation.py
+-rw-r--r--   0 b          (500) b          (506)     3013 2023-07-21 21:50:10.000000 antelope_core-0.3.1/antelope_core/archives/tests/test_term_manager.py
+-rw-r--r--   0 b          (500) b          (506)     4101 2023-07-21 21:50:10.000000 antelope_core-0.3.1/antelope_core/autorange.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:39:25.379961 antelope_core-0.3.1/antelope_core/catalog/
+-rw-r--r--   0 b          (500) b          (506)       70 2023-07-21 21:37:06.000000 antelope_core-0.3.1/antelope_core/catalog/__init__.py
+-rw-r--r--   0 b          (500) b          (506)    19147 2024-04-18 21:33:40.000000 antelope_core-0.3.1/antelope_core/catalog/catalog.py
+-rw-r--r--   0 b          (500) b          (506)      628 2020-11-05 08:47:12.000000 antelope_core-0.3.1/antelope_core/catalog/catalog_root.py
+-rw-r--r--   0 b          (500) b          (506)     6104 2023-07-21 21:50:10.000000 antelope_core-0.3.1/antelope_core/catalog/configurator.py
+-rw-r--r--   0 b          (500) b          (506)    23881 2024-04-18 21:33:40.000000 antelope_core-0.3.1/antelope_core/catalog/lc_catalog.py
+-rw-r--r--   0 b          (500) b          (506)     8998 2024-04-18 21:33:40.000000 antelope_core-0.3.1/antelope_core/catalog/lc_resolver.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:39:25.379961 antelope_core-0.3.1/antelope_core/catalog/tests/
+-rw-r--r--   0 b          (500) b          (506)        0 2018-07-26 08:24:01.000000 antelope_core-0.3.1/antelope_core/catalog/tests/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     5440 2024-04-18 21:33:40.000000 antelope_core-0.3.1/antelope_core/catalog/tests/test_catalogs.py
+-rw-r--r--   0 b          (500) b          (506)     2316 2023-07-21 21:50:10.000000 antelope_core-0.3.1/antelope_core/catalog/tests/test_process_ref.py
+-rw-r--r--   0 b          (500) b          (506)     1609 2024-04-18 21:33:40.000000 antelope_core-0.3.1/antelope_core/catalog/tests/test_quantity_refs.py
+-rw-r--r--   0 b          (500) b          (506)    18611 2024-04-18 21:37:01.000000 antelope_core-0.3.1/antelope_core/catalog_query.py
+-rw-r--r--   0 b          (500) b          (506)    10746 2024-04-18 21:33:40.000000 antelope_core-0.3.1/antelope_core/characterizations.py
+-rw-r--r--   0 b          (500) b          (506)    18315 2024-04-18 21:33:40.000000 antelope_core-0.3.1/antelope_core/contexts.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:39:25.383295 antelope_core-0.3.1/antelope_core/data_sources/
+-rw-r--r--   0 b          (500) b          (506)        0 2018-10-26 21:44:35.000000 antelope_core-0.3.1/antelope_core/data_sources/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     3851 2023-07-21 21:50:10.000000 antelope_core-0.3.1/antelope_core/data_sources/data_source.py
+-rw-r--r--   0 b          (500) b          (506)     7497 2023-07-21 21:50:10.000000 antelope_core-0.3.1/antelope_core/data_sources/ecoinvent.py
+-rw-r--r--   0 b          (500) b          (506)     1741 2023-07-21 21:50:10.000000 antelope_core-0.3.1/antelope_core/data_sources/ecoinvent_lcia.py
+-rw-r--r--   0 b          (500) b          (506)     1303 2023-07-21 21:50:10.000000 antelope_core-0.3.1/antelope_core/data_sources/gwp_ipcc_2007.py
+-rw-r--r--   0 b          (500) b          (506)     4614 2020-11-05 09:30:15.000000 antelope_core-0.3.1/antelope_core/data_sources/local.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:39:25.383295 antelope_core-0.3.1/antelope_core/data_sources/tests/
+-rw-r--r--   0 b          (500) b          (506)        0 2018-10-26 21:44:35.000000 antelope_core-0.3.1/antelope_core/data_sources/tests/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     4159 2024-03-20 22:20:51.000000 antelope_core-0.3.1/antelope_core/data_sources/tests/test_aa_local.py
+-rw-r--r--   0 b          (500) b          (506)     1541 2023-07-21 21:50:10.000000 antelope_core-0.3.1/antelope_core/data_sources/tests/test_ecoinvent.py
+-rw-r--r--   0 b          (500) b          (506)     7319 2021-07-08 16:41:41.000000 antelope_core-0.3.1/antelope_core/data_sources/tests/test_ecoinvent_lci.py
+-rw-r--r--   0 b          (500) b          (506)      820 2024-04-18 21:33:40.000000 antelope_core-0.3.1/antelope_core/data_sources/tests/test_ipcc2007.py
+-rw-r--r--   0 b          (500) b          (506)     1999 2024-03-20 22:20:51.000000 antelope_core-0.3.1/antelope_core/data_sources/tests/test_traci.py
+-rw-r--r--   0 b          (500) b          (506)     7401 2024-03-20 22:20:51.000000 antelope_core-0.3.1/antelope_core/data_sources/tests/test_uslci.py
+-rw-r--r--   0 b          (500) b          (506)     2438 2023-07-21 21:50:10.000000 antelope_core-0.3.1/antelope_core/data_sources/traci.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:39:25.383295 antelope_core-0.3.1/antelope_core/data_sources/uslci/
+-rw-r--r--   0 b          (500) b          (506)       31 2020-12-29 09:58:58.000000 antelope_core-0.3.1/antelope_core/data_sources/uslci/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     6853 2024-03-21 02:23:41.000000 antelope_core-0.3.1/antelope_core/data_sources/uslci/uslci.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:39:25.383295 antelope_core-0.3.1/antelope_core/entities/
+-rw-r--r--   0 b          (500) b          (506)      181 2023-07-21 21:50:10.000000 antelope_core-0.3.1/antelope_core/entities/__init__.py
+-rw-r--r--   0 b          (500) b          (506)    11984 2024-04-18 21:33:40.000000 antelope_core-0.3.1/antelope_core/entities/entities.py
+-rw-r--r--   0 b          (500) b          (506)     4021 2024-04-18 21:33:40.000000 antelope_core-0.3.1/antelope_core/entities/flows.py
+-rw-r--r--   0 b          (500) b          (506)    25036 2024-03-20 22:20:51.000000 antelope_core-0.3.1/antelope_core/entities/processes.py
+-rw-r--r--   0 b          (500) b          (506)     7969 2024-04-18 21:33:40.000000 antelope_core-0.3.1/antelope_core/entities/quantities.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:39:25.383295 antelope_core-0.3.1/antelope_core/entities/tests/
+-rw-r--r--   0 b          (500) b          (506)       62 2019-02-15 00:01:58.000000 antelope_core-0.3.1/antelope_core/entities/tests/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     1065 2021-01-07 23:11:04.000000 antelope_core-0.3.1/antelope_core/entities/tests/base_testclass.py
+-rw-r--r--   0 b          (500) b          (506)    99145 2024-04-18 21:33:40.000000 antelope_core-0.3.1/antelope_core/entities/tests/test_archive.json
+-rw-r--r--   0 b          (500) b          (506)     1019 2020-03-30 08:22:53.000000 antelope_core-0.3.1/antelope_core/entities/tests/test_entities.py
+-rw-r--r--   0 b          (500) b          (506)      850 2020-12-29 09:58:58.000000 antelope_core-0.3.1/antelope_core/entities/tests/test_entity_refs.py
+-rw-r--r--   0 b          (500) b          (506)      291 2020-03-30 08:22:53.000000 antelope_core-0.3.1/antelope_core/entities/tests/test_flows.py
+-rw-r--r--   0 b          (500) b          (506)     1538 2020-03-30 08:22:53.000000 antelope_core-0.3.1/antelope_core/entities/tests/test_processes.py
+-rw-r--r--   0 b          (500) b          (506)     1565 2020-09-29 22:38:38.000000 antelope_core-0.3.1/antelope_core/entities/tests/test_quantities.py
+-rw-r--r--   0 b          (500) b          (506)    18234 2023-07-21 21:50:10.000000 antelope_core-0.3.1/antelope_core/entities/xlsx_editor.py
+-rw-r--r--   0 b          (500) b          (506)    22640 2023-07-21 21:50:10.000000 antelope_core-0.3.1/antelope_core/exchanges.py
+-rw-r--r--   0 b          (500) b          (506)     6896 2024-04-18 21:33:40.000000 antelope_core-0.3.1/antelope_core/file_accessor.py
+-rw-r--r--   0 b          (500) b          (506)     1137 2023-07-21 21:37:06.000000 antelope_core-0.3.1/antelope_core/from_json.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:39:25.383295 antelope_core-0.3.1/antelope_core/implementations/
+-rw-r--r--   0 b          (500) b          (506)      333 2023-07-21 21:37:06.000000 antelope_core-0.3.1/antelope_core/implementations/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     8759 2024-04-18 21:33:44.000000 antelope_core-0.3.1/antelope_core/implementations/background.py
+-rw-r--r--   0 b          (500) b          (506)     6114 2024-04-18 21:33:40.000000 antelope_core-0.3.1/antelope_core/implementations/basic.py
+-rw-r--r--   0 b          (500) b          (506)    10083 2024-04-18 21:33:40.000000 antelope_core-0.3.1/antelope_core/implementations/configure.py
+-rw-r--r--   0 b          (500) b          (506)     2812 2023-07-21 21:50:10.000000 antelope_core-0.3.1/antelope_core/implementations/exchange.py
+-rw-r--r--   0 b          (500) b          (506)     6800 2024-04-18 21:33:40.000000 antelope_core-0.3.1/antelope_core/implementations/index.py
+-rw-r--r--   0 b          (500) b          (506)    33026 2024-04-18 21:33:40.000000 antelope_core-0.3.1/antelope_core/implementations/quantity.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:39:25.383295 antelope_core-0.3.1/antelope_core/implementations/tests/
+-rw-r--r--   0 b          (500) b          (506)        0 2018-09-13 20:45:30.000000 antelope_core-0.3.1/antelope_core/implementations/tests/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     2056 2023-07-21 21:50:10.000000 antelope_core-0.3.1/antelope_core/implementations/tests/test_quantity.py
+-rw-r--r--   0 b          (500) b          (506)    17430 2024-04-18 21:33:40.000000 antelope_core-0.3.1/antelope_core/lc_resource.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:39:25.383295 antelope_core-0.3.1/antelope_core/lcia_engine/
+-rw-r--r--   0 b          (500) b          (506)     5682 2024-04-18 21:33:40.000000 antelope_core-0.3.1/antelope_core/lcia_engine/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     8163 2023-07-21 21:50:10.000000 antelope_core-0.3.1/antelope_core/lcia_engine/clookup.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:39:25.383295 antelope_core-0.3.1/antelope_core/lcia_engine/data/
+-rw-r--r--   0 b          (500) b          (506)     8401 2024-04-18 21:33:40.000000 antelope_core-0.3.1/antelope_core/lcia_engine/data/contexts.json
+-rw-r--r--   0 b          (500) b          (506)   383481 2020-03-30 08:22:53.000000 antelope_core-0.3.1/antelope_core/lcia_engine/data/flowables.json
+-rw-r--r--   0 b          (500) b          (506)    30980 2021-01-07 00:24:41.000000 antelope_core-0.3.1/antelope_core/lcia_engine/data/ipcc_2007_gwp.json
+-rw-r--r--   0 b          (500) b          (506)    19228 2024-04-18 21:33:40.000000 antelope_core-0.3.1/antelope_core/lcia_engine/lcia_engine.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:39:25.383295 antelope_core-0.3.1/antelope_core/lcia_engine/tests/
+-rw-r--r--   0 b          (500) b          (506)        0 2020-03-30 08:22:53.000000 antelope_core-0.3.1/antelope_core/lcia_engine/tests/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     1645 2024-03-20 22:20:51.000000 antelope_core-0.3.1/antelope_core/lcia_engine/tests/test_biogenic_co2.py
+-rw-r--r--   0 b          (500) b          (506)     2559 2020-03-30 08:22:53.000000 antelope_core-0.3.1/antelope_core/lcia_engine/tests/test_clookup.py
+-rw-r--r--   0 b          (500) b          (506)      924 2020-09-29 22:38:38.000000 antelope_core-0.3.1/antelope_core/lcia_engine/tests/test_ipcc.py
+-rw-r--r--   0 b          (500) b          (506)     2981 2023-07-21 21:37:06.000000 antelope_core-0.3.1/antelope_core/lcia_engine/tests/test_lcia_engine.py
+-rw-r--r--   0 b          (500) b          (506)    45982 2024-04-18 21:33:40.000000 antelope_core-0.3.1/antelope_core/lcia_results.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:39:25.386628 antelope_core-0.3.1/antelope_core/providers/
+-rw-r--r--   0 b          (500) b          (506)     4643 2024-04-18 21:33:40.000000 antelope_core-0.3.1/antelope_core/providers/__init__.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:39:25.386628 antelope_core-0.3.1/antelope_core/providers/data/
+-rw-r--r--   0 b          (500) b          (506)       57 2019-02-15 00:01:58.000000 antelope_core-0.3.1/antelope_core/providers/data/__init__.py
+-rw-r--r--   0 b          (500) b          (506)    39336 2018-07-26 08:24:01.000000 antelope_core-0.3.1/antelope_core/providers/data/list_of_methods_and_indicators_ecoinvent_v3.2.xlsx
+-rw-r--r--   0 b          (500) b          (506)    95429 2019-02-15 00:01:58.000000 antelope_core-0.3.1/antelope_core/providers/data/traci_2_1_2014_dec_10_0_test.xlsx
+-rw-r--r--   0 b          (500) b          (506)     9551 2023-07-21 21:50:10.000000 antelope_core-0.3.1/antelope_core/providers/ecoinvent_lcia.py
+-rw-r--r--   0 b          (500) b          (506)    11083 2023-07-21 21:50:10.000000 antelope_core-0.3.1/antelope_core/providers/ecospold.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:39:25.386628 antelope_core-0.3.1/antelope_core/providers/ecospold2/
+-rw-r--r--   0 b          (500) b          (506)       41 2018-07-26 08:24:01.000000 antelope_core-0.3.1/antelope_core/providers/ecospold2/__init__.py
+-rw-r--r--   0 b          (500) b          (506)    24560 2023-07-21 21:50:10.000000 antelope_core-0.3.1/antelope_core/providers/ecospold2/ecospold2.py
+-rw-r--r--   0 b          (500) b          (506)      564 2020-10-18 05:43:46.000000 antelope_core-0.3.1/antelope_core/providers/ecospold2/ecospold2_index.py
+-rw-r--r--   0 b          (500) b          (506)     2134 2020-03-30 08:22:53.000000 antelope_core-0.3.1/antelope_core/providers/ecospold2/master_data.py
+-rw-r--r--   0 b          (500) b          (506)    10917 2023-07-21 21:50:10.000000 antelope_core-0.3.1/antelope_core/providers/file_store.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:39:25.386628 antelope_core-0.3.1/antelope_core/providers/ilcd/
+-rw-r--r--   0 b          (500) b          (506)       78 2018-07-26 08:24:01.000000 antelope_core-0.3.1/antelope_core/providers/ilcd/__init__.py
+-rw-r--r--   0 b          (500) b          (506)    17683 2023-07-21 21:50:10.000000 antelope_core-0.3.1/antelope_core/providers/ilcd/ilcd.py
+-rw-r--r--   0 b          (500) b          (506)     2314 2018-07-26 08:24:01.000000 antelope_core-0.3.1/antelope_core/providers/ilcd/ilcd_flowables.py
+-rw-r--r--   0 b          (500) b          (506)     5806 2023-07-21 21:50:10.000000 antelope_core-0.3.1/antelope_core/providers/ilcd/ilcd_lcia.py
+-rw-r--r--   0 b          (500) b          (506)      314 2020-09-29 23:36:41.000000 antelope_core-0.3.1/antelope_core/providers/ilcd/index.py
+-rw-r--r--   0 b          (500) b          (506)     3177 2023-07-21 21:37:06.000000 antelope_core-0.3.1/antelope_core/providers/ilcd/quantity.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:39:25.386628 antelope_core-0.3.1/antelope_core/providers/ilcd/tests/
+-rw-r--r--   0 b          (500) b          (506)        0 2021-01-07 00:24:41.000000 antelope_core-0.3.1/antelope_core/providers/ilcd/tests/__init__.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:39:25.376628 antelope_core-0.3.1/antelope_core/providers/ilcd/tests/data/
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:39:25.376628 antelope_core-0.3.1/antelope_core/providers/ilcd/tests/data/ilcd_test/
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:39:25.376628 antelope_core-0.3.1/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:39:25.386628 antelope_core-0.3.1/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/
+-rw-r--r--   0 b          (500) b          (506)     2712 2019-02-15 00:01:58.000000 antelope_core-0.3.1/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-11da-a746-0800200b9a66.xml
+-rw-r--r--   0 b          (500) b          (506)     2738 2019-02-15 00:01:58.000000 antelope_core-0.3.1/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-11da-a746-0800200c9a66.xml
+-rw-r--r--   0 b          (500) b          (506)     2734 2019-02-15 00:01:58.000000 antelope_core-0.3.1/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-13da-a746-0800200c9a66.xml
+-rw-r--r--   0 b          (500) b          (506)     2716 2019-02-15 00:01:58.000000 antelope_core-0.3.1/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-22da-a746-0800200c9a66.xml
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:39:25.386628 antelope_core-0.3.1/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flows/
+-rw-r--r--   0 b          (500) b          (506)     5078 2019-02-15 00:01:58.000000 antelope_core-0.3.1/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flows/f579de8c-8897-4bdb-9a0a-b36f8b13282e.xml
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:39:25.386628 antelope_core-0.3.1/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/
+-rw-r--r--   0 b          (500) b          (506)     2503 2019-02-15 00:01:58.000000 antelope_core-0.3.1/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/1ff9a08c-6fc1-4509-8bcd-a5404c598755.xml
+-rw-r--r--   0 b          (500) b          (506)     3551 2019-02-15 00:01:58.000000 antelope_core-0.3.1/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/ad38d542-3fe9-439d-9b95-2f5f7752acaf.xml
+-rw-r--r--   0 b          (500) b          (506)     3344 2019-02-15 00:01:58.000000 antelope_core-0.3.1/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/cd950537-0a98-4044-9ba7-9f9a68d0a504.xml
+-rw-r--r--   0 b          (500) b          (506)     4443 2019-02-15 00:01:58.000000 antelope_core-0.3.1/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/de5104d8-3de0-4218-a29d-b7123ce9ca3c.xml
+-rw-r--r--   0 b          (500) b          (506)      932 2021-01-07 00:24:41.000000 antelope_core-0.3.1/antelope_core/providers/ilcd/tests/test_ilcd.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:39:25.386628 antelope_core-0.3.1/antelope_core/providers/openlca/
+-rw-r--r--   0 b          (500) b          (506)       91 2024-04-18 21:33:40.000000 antelope_core-0.3.1/antelope_core/providers/openlca/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     4887 2024-04-18 21:33:40.000000 antelope_core-0.3.1/antelope_core/providers/openlca/olca_accessor.py
+-rw-r--r--   0 b          (500) b          (506)    12011 2024-04-18 21:33:40.000000 antelope_core-0.3.1/antelope_core/providers/openlca/olca_ref_data.py
+-rw-r--r--   0 b          (500) b          (506)    24980 2024-03-20 22:20:51.000000 antelope_core-0.3.1/antelope_core/providers/openlca/openlca_jsonld.py
+-rw-r--r--   0 b          (500) b          (506)      775 2024-03-20 22:20:51.000000 antelope_core-0.3.1/antelope_core/providers/openlca/schema_mapping.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:39:25.386628 antelope_core-0.3.1/antelope_core/providers/openlca/tests/
+-rw-r--r--   0 b          (500) b          (506)        0 2024-01-05 07:24:59.000000 antelope_core-0.3.1/antelope_core/providers/openlca/tests/__init__.py
+-rw-r--r--   0 b          (500) b          (506)       83 2024-01-05 07:57:07.000000 antelope_core-0.3.1/antelope_core/providers/openlca/tests/test_olca_ref.py
+-rw-r--r--   0 b          (500) b          (506)      729 2023-07-21 21:37:06.000000 antelope_core-0.3.1/antelope_core/providers/parse_math.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:39:25.386628 antelope_core-0.3.1/antelope_core/providers/tests/
+-rw-r--r--   0 b          (500) b          (506)        0 2018-07-26 08:24:01.000000 antelope_core-0.3.1/antelope_core/providers/tests/__init__.py
+-rw-r--r--   0 b          (500) b          (506)      569 2020-09-29 23:35:54.000000 antelope_core-0.3.1/antelope_core/providers/tests/test_ecospold.py
+-rw-r--r--   0 b          (500) b          (506)     4110 2018-07-26 08:24:01.000000 antelope_core-0.3.1/antelope_core/providers/tests/test_xml_widgets.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:39:25.386628 antelope_core-0.3.1/antelope_core/providers/traci/
+-rw-r--r--   0 b          (500) b          (506)       50 2018-07-26 08:24:01.000000 antelope_core-0.3.1/antelope_core/providers/traci/__init__.py
+-rw-r--r--   0 b          (500) b          (506)      653 2020-09-29 23:35:54.000000 antelope_core-0.3.1/antelope_core/providers/traci/index.py
+-rw-r--r--   0 b          (500) b          (506)     3441 2019-01-17 18:55:10.000000 antelope_core-0.3.1/antelope_core/providers/traci/q_info.py
+-rw-r--r--   0 b          (500) b          (506)     2076 2020-09-29 23:35:54.000000 antelope_core-0.3.1/antelope_core/providers/traci/quantity.py
+-rw-r--r--   0 b          (500) b          (506)     1648 2020-03-30 08:22:53.000000 antelope_core-0.3.1/antelope_core/providers/traci/test_traci.py
+-rw-r--r--   0 b          (500) b          (506)     6687 2023-07-21 21:50:10.000000 antelope_core-0.3.1/antelope_core/providers/traci/traci_2_1_spreadsheet.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:39:25.389961 antelope_core-0.3.1/antelope_core/providers/xdb_client/
+-rw-r--r--   0 b          (500) b          (506)       67 2023-08-19 07:49:00.000000 antelope_core-0.3.1/antelope_core/providers/xdb_client/__init__.py
+-rw-r--r--   0 b          (500) b          (506)    16890 2024-04-18 21:33:40.000000 antelope_core-0.3.1/antelope_core/providers/xdb_client/implementation.py
+-rw-r--r--   0 b          (500) b          (506)     4447 2024-04-18 21:33:40.000000 antelope_core-0.3.1/antelope_core/providers/xdb_client/requester.py
+-rw-r--r--   0 b          (500) b          (506)     7202 2024-04-18 21:33:40.000000 antelope_core-0.3.1/antelope_core/providers/xdb_client/rest_client.py
+-rw-r--r--   0 b          (500) b          (506)     7616 2024-04-18 21:33:40.000000 antelope_core-0.3.1/antelope_core/providers/xdb_client/xdb_client.py
+-rw-r--r--   0 b          (500) b          (506)     3971 2024-04-18 21:33:40.000000 antelope_core-0.3.1/antelope_core/providers/xdb_client/xdb_entities.py
+-rw-r--r--   0 b          (500) b          (506)     2316 2023-07-21 21:50:10.000000 antelope_core-0.3.1/antelope_core/providers/xl_dict.py
+-rw-r--r--   0 b          (500) b          (506)     1676 2020-03-30 08:22:53.000000 antelope_core-0.3.1/antelope_core/providers/xml_widgets.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:39:25.389961 antelope_core-0.3.1/antelope_core/tests/
+-rw-r--r--   0 b          (500) b          (506)        0 2018-07-26 08:24:01.000000 antelope_core-0.3.1/antelope_core/tests/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     1007 2023-07-21 21:50:10.000000 antelope_core-0.3.1/antelope_core/tests/test_autorange.py
+-rw-r--r--   0 b          (500) b          (506)    13733 2024-04-18 21:33:40.000000 antelope_core-0.3.1/antelope_core/tests/test_contexts.py
+-rw-r--r--   0 b          (500) b          (506)     5637 2020-12-29 09:58:58.000000 antelope_core-0.3.1/antelope_core/tests/test_exchanges.py
+-rw-r--r--   0 b          (500) b          (506)      500 2020-12-29 09:58:58.000000 antelope_core-0.3.1/antelope_core/tests/test_lcia_results.py
+-rw-r--r--   0 b          (500) b          (506)     1162 2020-09-30 00:02:12.000000 antelope_core-0.3.1/antelope_core/tests/test_resources.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:39:25.389961 antelope_core-0.3.1/antelope_core.egg-info/
+-rw-r--r--   0 b          (500) b          (506)    14539 2024-04-18 21:39:25.000000 antelope_core-0.3.1/antelope_core.egg-info/PKG-INFO
+-rw-r--r--   0 b          (500) b          (506)     7084 2024-04-18 21:39:25.000000 antelope_core-0.3.1/antelope_core.egg-info/SOURCES.txt
+-rw-r--r--   0 b          (500) b          (506)        1 2024-04-18 21:39:25.000000 antelope_core-0.3.1/antelope_core.egg-info/dependency_links.txt
+-rw-r--r--   0 b          (500) b          (506)      169 2024-04-18 21:39:25.000000 antelope_core-0.3.1/antelope_core.egg-info/requires.txt
+-rw-r--r--   0 b          (500) b          (506)       14 2024-04-18 21:39:25.000000 antelope_core-0.3.1/antelope_core.egg-info/top_level.txt
+-rw-r--r--   0 b          (500) b          (506)       38 2024-04-18 21:39:25.389961 antelope_core-0.3.1/setup.cfg
+-rw-r--r--   0 b          (500) b          (506)     4059 2024-04-18 21:38:08.000000 antelope_core-0.3.1/setup.py
```

### Comparing `antelope_core-0.3.0/LICENSE` & `antelope_core-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/PKG-INFO` & `antelope_core-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: antelope_core
-Version: 0.3.0
-Home-page: https://github.com/AntelopeLCA/core
-Author: Brandon Kuczenski
-Author-email: bkuczenski@ucsb.edu
-License: BSD 3-Clause
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: XML
-Provides-Extra: write_to_excel
-License-File: LICENSE
-
 ![](https://travis-ci.com/AntelopeLCA/core.svg?branch=master&status=passed) ![](https://coveralls.io/repos/github/AntelopeLCA/core/badge.svg?branch=master)
 
 # core
 Antelope Catalog - reference implementation.
 
 This repository provides code that enables access to different forms of life cycle 
 inventory and impact assessment data, ideally from both local and remote sources.  It
```

### Comparing `antelope_core-0.3.0/README.md` & `antelope_core-0.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,35 @@
+Metadata-Version: 2.1
+Name: antelope_core
+Version: 0.3.1
+Home-page: https://github.com/AntelopeLCA/core
+Author: Brandon Kuczenski
+Author-email: bkuczenski@ucsb.edu
+License: BSD 3-Clause
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: synonym_dict>=0.2.4
+Requires-Dist: antelope_interface>=0.2.4
+Requires-Dist: xlstools>=0.1.3
+Requires-Dist: python-magic>=0.4.18
+Requires-Dist: requests>=2.25
+Requires-Dist: pydantic>=2.5.0
+Provides-Extra: xml
+Requires-Dist: lxml>=1.2.0; extra == "xml"
+Provides-Extra: write-to-excel
+Requires-Dist: xlsxwriter>=1.3.7; extra == "write-to-excel"
+
 ![](https://travis-ci.com/AntelopeLCA/core.svg?branch=master&status=passed) ![](https://coveralls.io/repos/github/AntelopeLCA/core/badge.svg?branch=master)
 
 # core
 Antelope Catalog - reference implementation.
 
 This repository provides code that enables access to different forms of life cycle 
 inventory and impact assessment data, ideally from both local and remote sources.  It
```

### Comparing `antelope_core-0.3.0/antelope_core/__init__.py` & `antelope_core-0.3.1/antelope_core/__init__.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/archives/__init__.py` & `antelope_core-0.3.1/antelope_core/archives/__init__.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/archives/archive_index.py` & `antelope_core-0.3.1/antelope_core/archives/archive_index.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,26 +25,28 @@
 
 class LcIndex(AbstractIndex, LcArchive):
     _ns_uuid_required = None
     def serialize(self, exchanges=False, characterizations=False, values=False, domesticate=False):
         return super(LcIndex, self).serialize(exchanges=False, characterizations=False, values=False, domesticate=False)
 
 
-def index_archive(archive, source, ref=None, signifier='index', force=False):
+def index_archive(archive, source, ref=None, signifier='index', force=False, save=True):
     if source is None:
-        raise AssertionError('Source is required')
-    if not bool(re.search('\.gz$', source)):
-        source += '.gz'
-    if source == archive.source:
-        raise ArchiveError('Index must have a different source from original archive')
-    if os.path.exists(source):
-        if force:
-            print('File exists: %s. Overwriting..' % source)
-        else:
-            raise FileExistsError(source)
+        if save is True:
+            raise AssertionError('Source is required')
+    else:
+        if not bool(re.search('\.gz$', source)):
+            source += '.gz'
+        if source == archive.source:
+            raise ArchiveError('Index must have a different source from original archive')
+        if save and os.path.exists(source):
+            if force:
+                print('File exists: %s. Overwriting..' % source)
+            else:
+                raise FileExistsError(source)
 
     if ref is None or ref == archive.ref:
         ref = archive.construct_new_ref(signifier=signifier)
 
     if isinstance(archive, LcArchive):
         index = LcIndex(source, ref=ref, static=True, **archive.init_args)
         types = LC_ENTITY_TYPES
@@ -58,9 +60,11 @@
     # import original archives list of names
     names = defaultdict(list)
     for s, r in archive.names.items():
         names[r].append(s)
 
     index.load_from_dict({'catalogNames': names})
 
-    index.write_to_file(source, gzip=True)
+    if save:
+        print('Saving index to file %s' % source)
+        index.write_to_file(source, gzip=True)
     return index
```

### Comparing `antelope_core-0.3.0/antelope_core/archives/basic_archive.py` & `antelope_core-0.3.1/antelope_core/archives/basic_archive.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,27 +101,30 @@
         """
         init_args = j.pop('initArgs', {})
         ns_uuid = j.pop('nsUuid', j.pop('ns_uuid', None))  # this is for opening legacy files
         if ns_uuid is None:
             ns_uuid = init_args.pop('ns_uuid', None)
         kwargs.update(init_args)
 
-        old_ref = j.pop('dataReference', ref)
-        existing_ref = kwargs.pop('dataReference', old_ref)  # this will be the latest of init[dataRef], [dataRef], ref
+        old_ref = j.pop('dataReference', ref)  # make sure we do not pass a dataReference to the mechanism
+        # existing_ref = kwargs.pop('dataReference', old_ref)  # picks the crustiest of (init[dataRef], [dataRef], ref)
+        if ref is None:  # this picks the FIRST PRESENT of ref, [dataRef], init[dataRef]
+            ref = kwargs.pop('dataReference', old_ref)
 
         if filename is None:
             source = j.pop('dataSource')
         else:
             source = filename
-        ar = cls(source, ref=existing_ref, ns_uuid=ns_uuid, static=True, **kwargs)
-        if ref != ar.ref:
-            ar.set_origin(ref)
+        ar = cls(source, ref=ref, ns_uuid=ns_uuid, static=True, **kwargs)
 
         ar.load_from_dict(j, jsonfile=filename)
 
+        if ref != ar.ref:
+            ar.set_origin(ref)
+
         return ar
 
     def __init__(self, *args, contexts=None, flowables=None, term_manager=None, **kwargs):
         super(BasicArchive, self).__init__(*args, **kwargs)
         self._tm = term_manager or TermManager(contexts=contexts, flowables=flowables)
         self._set_query()
```

### Comparing `antelope_core-0.3.0/antelope_core/archives/data/elcd_reference_quantities.json` & `antelope_core-0.3.1/antelope_core/archives/data/elcd_reference_quantities.json`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/archives/entity_store.py` & `antelope_core-0.3.1/antelope_core/archives/entity_store.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/archives/lc_archive.py` & `antelope_core-0.3.1/antelope_core/archives/lc_archive.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/archives/quantity_manager.py` & `antelope_core-0.3.1/antelope_core/archives/quantity_manager.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/archives/term_manager.py` & `antelope_core-0.3.1/antelope_core/archives/term_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,19 +55,21 @@
 
 from antelope import EntityNotFound
 from ..contexts import ContextManager, NullContext
 from .quantity_manager import QuantityManager
 
 from ..characterizations import Characterization, DuplicateCharacterizationError
 
+import logging
+
 
 DuplicateCharacterization = namedtuple('DuplicateCharacterization', ('qq_link', 'fb', 'cx_list', 'origin', 'flowable', 'location'))
 
 
-class FactorCollision(Exception):
+class FactorConflict(Exception):
     pass
 
 
 ''' # cannot figure out what this is supposed to guard against
 class QuantityConflict(Exception):
     pass
 '''
@@ -370,15 +372,15 @@
                         cand = (combo[k], cl[k])
                         if cand[0].value == cand[1].value:
                             continue
                         fq_conflicts.append(cand)  # but it's really only a conflict if the cf values differ
 
         if len(fq_conflicts) > 0:
             print('%d Merge conflicts encountered' % len(fq_conflicts))
-            raise FactorCollision(fq_conflicts)
+            raise FactorConflict(fq_conflicts)
 
         for qq, f_dict in self._q_dict.items():
             # once we are sure there are no conflicts, we perform the actual merge
             for syn in syns:
                 if syn not in f_dict:
                     continue
                 cl = f_dict[syn]
@@ -565,15 +567,15 @@
             rq = self.add_quantity(ref_quantity)
 
         try:
             qq = self._canonical_q(query_quantity)
         except KeyError:
             qq = self.add_quantity(query_quantity)
 
-        cf = self._find_exact_cf(qq, fb, cx, origin, flowable)
+        cf = self._find_exact_cf(qq, fb, cx, origin)
 
         if location is None:
             location = 'GLO'
 
         if cf is None:
             # create our new Characterization with the provided flowable, not the detected flowable
             new_cf = Characterization(flowable, rq, qq, context=cx, origin=origin)
@@ -586,61 +588,67 @@
 
             # add our new CF to the lookup tree
             self._qassign(qq, fb, new_cf, context=cx)
 
             return new_cf
         else:
             if cf.ref_quantity != rq:
-                # create a conversion-factor instead:
-                if value == 0:
-                    # we cannot interpret a 0 as a cf- so we ditch
-                    return cf
-
-                try:
-                    factor = value / cf[location]
-                except ZeroDivisionError:
-                    try:
-                        factor = value / cf.value
-                    except TypeError:  # dict = fail
-                        factor = value
-
-                # this recurses to add a cf between our flow's ref quantity and the ref quantity of the already-seen cf
                 try:
-                    self.add_characterization(fb, rq, cf.ref_quantity, factor, context=cx, origin=origin,
-                                              location=location, overwrite=overwrite)
+                    return self._create_conversion_cf(cf)
                 except DuplicateCharacterizationError as e:
                     print((qq.link, fb, cx.as_list(), origin, flowable, location))
                     print('recursing to %s %s' % (cf.ref_quantity.name, cf.ref_quantity.uuid))
                     print('ignoring duplicate characterization %s' % e)
-                return cf
+                    return cf
             # update entry in the lookup tree
             elif isinstance(value, dict):
                 cf.update_values(**value)
             else:
                 try:
                     cf.add_value(value, location=location, overwrite=overwrite)
                 except DuplicateCharacterizationError as e:
                     self._dupes.append(DuplicateCharacterization(qq.link, fb, cx.as_list(), origin, flowable, location))
                     print('ignoring duplicate characterization %s' % e)
             return cf
 
+    def _create_conversion_cf(self, ex_cf, rq, cx, origin, location, value, overwrite=False):
+        # create a conversion-factor instead:
+        if value == 0:
+            # we cannot interpret a 0 as a cf- so we ditch
+            return ex_cf
+
+        try:
+            factor = value / ex_cf[location]
+        except ZeroDivisionError:
+            logging.error('Zero-division on conversion CF %s\n%s' % (value, ex_cf))
+            try:
+                factor = value / ex_cf.value
+            except TypeError:  # dict = fail
+                factor = value
+
+        if factor < 0:
+            logging.warning('Negative conversion CF %s\n%s' % (factor, ex_cf))
+
+        # this recurses to add a cf between our flow's ref quantity and the ref quantity of the already-seen cf
+        return self.add_characterization(ex_cf.flowable, rq, ex_cf.ref_quantity, factor, context=cx, origin=origin,
+                                         location=location, overwrite=overwrite)
+
     '''
     Info Retrieval
     '''
-    def _find_exact_cf(self, qq, fb, cx, origin, flowable):
+    def _find_exact_cf(self, qq, fb, cx, origin):
         """
         The purpose of this function is to retrieve an exact CF if one exists.
         WHY does this not take rq into account??
 
         origin used in subclasses
         :param qq:
         :param fb:
         :param cx:
         :param origin:
-        :param flowable: using this in subclass
         :return:
         """
         try:
             clookup = self._qlookup(qq, fb)
         except NoFQEntry:
             return None
         if cx in clookup:
@@ -713,15 +721,15 @@
         """
         Assigns the cf to the mapping; does subclass-specific collision checking
         :param cl:
         :param new_cf:
         :return:
         """
         if context in cl:
-            raise FactorCollision
+            raise FactorConflict
         cl[context] = new_cf
 
     def _qassign(self, qq, fb, new_cf, context=None):
         """
         Assigns the new_cf to the canonical quantity and flowable, taking context and origin from new_cf
         :param qq: a canonical quantity
         :param fb: a canonical flowable
```

### Comparing `antelope_core-0.3.0/antelope_core/archives/tests/test_base.py` & `antelope_core-0.3.1/antelope_core/archives/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/archives/tests/test_basic_archive.py` & `antelope_core-0.3.1/antelope_core/archives/tests/test_basic_archive.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/archives/tests/test_entity_store.py` & `antelope_core-0.3.1/antelope_core/archives/tests/test_entity_store.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/archives/tests/test_json.json` & `antelope_core-0.3.1/antelope_core/archives/tests/test_json.json`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/archives/tests/test_qdb.py` & `antelope_core-0.3.1/antelope_core/archives/tests/test_qdb.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/archives/tests/test_quantity_manager.py` & `antelope_core-0.3.1/antelope_core/archives/tests/test_quantity_manager.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/archives/tests/test_quantity_relation.py` & `antelope_core-0.3.1/antelope_core/archives/tests/test_quantity_relation.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/archives/tests/test_term_manager.py` & `antelope_core-0.3.1/antelope_core/archives/tests/test_term_manager.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/autorange.py` & `antelope_core-0.3.1/antelope_core/autorange.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/catalog/catalog.py` & `antelope_core-0.3.1/antelope_core/catalog/catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,18 +25,20 @@
 import hashlib
 from collections import defaultdict
 
 from ..archives import InterfaceError, EntityExists
 from ..lcia_engine import LciaDb
 
 
-from antelope import CatalogRef, UnknownOrigin, InvalidQuery  # , EntityNotFound
+from antelope import UnknownOrigin, InvalidQuery  # , EntityNotFound
 from ..catalog_query import CatalogQuery, INTERFACE_TYPES, zap_inventory
 from .lc_resolver import LcCatalogResolver
 from ..lc_resource import LcResource
+from ..archives import REF_QTYS
+from ..lcia_engine import DEFAULT_CONTEXTS, DEFAULT_FLOWABLES
 # from lcatools.flowdb.compartments import REFERENCE_INT  # reference intermediate flows
 
 
 class DuplicateEntries(Exception):
     pass
 
 
@@ -70,14 +72,16 @@
      LcCatalog._reference_qtys: reference quantities file in root
      LcCatalog._compartments: local compartments file (outmoded in Context Refactor)
 
 
     """
     @property
     def resource_dir(self):
+        if self._rootdir is None:
+            return None
         return os.path.join(self._rootdir, 'resources')
 
     @property
     def _download_dir(self):
         return os.path.join(self._rootdir, 'downloads')
 
     @staticmethod
@@ -102,57 +106,66 @@
     @property
     def _cache_dir(self):
         return os.path.join(self._rootdir, 'cache')
 
     def cache_file(self, source):
         return os.path.join(self._cache_dir, self._source_hash_file(source) + '.json.gz')
 
+    def check_cache(self, source):
+        return os.path.exists(self.cache_file(source))
+
     @property
     def archive_dir(self):
         return os.path.join(self._rootdir, 'archives')
 
     '''
     @property
     def _entity_cache(self):
         return os.path.join(self._rootdir, 'entity_cache.json')
     '''
 
     @property
     def _reference_qtys(self):
+        if self._rootdir is None:
+            return REF_QTYS
         return os.path.join(self._rootdir, 'reference-quantities.json')
 
     '''
     @property
     def _compartments(self):
         """
         Deprecated
         :return:
         """
         return os.path.join(self._rootdir, 'local-compartments.json')
     '''
 
     @property
     def _contexts(self):
+        if self._rootdir is None:
+            return DEFAULT_CONTEXTS
         return os.path.join(self._rootdir, 'local-contexts.json')
 
     @property
     def _flowables(self):
+        if self._rootdir is None:
+            return DEFAULT_FLOWABLES
         return os.path.join(self._rootdir, 'local-flowables.json')
 
     def _localize_source(self, source):
-        if source is None:
+        if source is None or self._rootdir is None:
             return None
         if source.startswith(self._rootdir):
             # return re.sub('^%s' % self._rootdir, '$CAT_ROOT', source)
             # Should work on both mac and windows
             return os.path.join('$CAT_ROOT', os.path.relpath(source, self._rootdir))
         return source
 
     def abs_path(self, rel_path):
-        if os.path.isabs(rel_path):
+        if os.path.isabs(rel_path) or self._rootdir is None:
             return rel_path
         elif rel_path.startswith('$CAT_ROOT'):
             # return re.sub('^\$CAT_ROOT', self.root, rel_path)
             # Should work on both mac and windows
             return os.path.abspath(os.path.join(self.root, os.path.relpath(rel_path, '$CAT_ROOT')))
         return os.path.abspath(os.path.join(self.root, rel_path))
 
@@ -165,18 +178,22 @@
         Instantiates a catalog based on the resources provided in resource_dir
         :param rootdir: directory storing LcResource files.
         :param strict_clookup: [True] whether to enforce uniqueness on characterization factors (raise an error when a
          non-matching duplicate characterization is encountered). If False, selection among conflicting factors is
          not well defined and may be done interactively or unpredictably
         :param kwargs: passed to Qdb
         """
-        self._rootdir = os.path.abspath(rootdir)
-        if not os.path.exists(self._rootdir):
-            raise FileNotFoundError(self._rootdir)
-        self._resolver = LcCatalogResolver(self.resource_dir)
+        if rootdir is None:
+            self._rootdir = None
+            self._resolver = LcCatalogResolver(None)
+        else:
+            self._rootdir = os.path.abspath(rootdir)
+            if not os.path.exists(self._rootdir):
+                raise FileNotFoundError(self._rootdir)
+            self._resolver = LcCatalogResolver(self.resource_dir)
 
         """
         _archives := source -> archive
         _names :=  ref:interface -> source
         _nicknames := nickname -> source
         """
         self._nicknames = dict()  # keep a collection of shorthands for origins
```

### Comparing `antelope_core-0.3.0/antelope_core/catalog/catalog_root.py` & `antelope_core-0.3.1/antelope_core/catalog/catalog_root.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/catalog/configurator.py` & `antelope_core-0.3.1/antelope_core/catalog/configurator.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/catalog/lc_catalog.py` & `antelope_core-0.3.1/antelope_core/catalog/lc_catalog.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-import tempfile
-
 from antelope.xdb_tokens import ResourceSpec
 
-from .catalog import StaticCatalog
+from .catalog import StaticCatalog, CatalogError
 from ..archives import REF_QTYS, archive_from_json
 from ..lc_resource import LcResource
 from ..lcia_engine import DEFAULT_CONTEXTS, DEFAULT_FLOWABLES
 from ..providers.xdb_client.rest_client import RestClient
 
 import requests
 from requests.exceptions import HTTPError
 
 from shutil import copy2, rmtree
 import os
 import glob
-import json
+import logging
 import hashlib
 import getpass
 
 # TEST_ROOT = os.path.join(os.path.dirname(__file__), 'cat-test')  # volatile, inspectable
 
 
 def download_file(url, local_file, md5sum=None):
@@ -44,14 +42,17 @@
         download with an MD5 digest.
         :param url:
         :param md5sum:
         :param force:
         :param localize: whether to return the filename relative to the catalog root
         :return: the full path to the downloaded file 
         """
+        if self._test:
+            logging.error('Cannot save files locally during tester operation')
+            raise CatalogError
         local_file = os.path.join(self._download_dir, self._source_hash_file(url))
         if os.path.exists(local_file):
             if force:
                 print('File exists.. re-downloading.')
             else:
                 print('File already downloaded.  Force=True to re-download.')
                 if localize:
@@ -73,69 +74,87 @@
     @classmethod
     def make_tester(cls, **kwargs):
         """
         Sets a flag that tells the rootdir to be deleted when the catalog is garbage collected
         :param kwargs:
         :return:
         """
-        tmp = tempfile.mkdtemp()
-        return cls(tmp, _test=True, **kwargs)
+        # tmp = tempfile.mkdtemp()
+        return cls(None, _test=True, **kwargs)
 
     """
     @classmethod
     def load_tester(cls):
         return cls(TEST_ROOT)
     """
 
     @property
     def _dirs(self):
         for x in (self._cache_dir, self._index_dir, self.resource_dir, self.archive_dir, self._download_dir):
             yield x
 
+    def check_cache(self, source):
+        if self._test:
+            return False
+        return super(LcCatalog, self).check_cache(source)
+
     def _make_rootdir(self):
         for x in self._dirs:
             os.makedirs(x, exist_ok=True)
         if not os.path.exists(self._contexts):
             copy2(DEFAULT_CONTEXTS, self._contexts)
         if not os.path.exists(self._flowables):
             copy2(DEFAULT_FLOWABLES, self._flowables)
         if not os.path.exists(self._reference_qtys):
             copy2(REF_QTYS, self._reference_qtys)
 
     def __init__(self, rootdir, _test=False, **kwargs):
-        self._rootdir = os.path.abspath(rootdir)
-        self._make_rootdir()  # this will be a git clone / fork;; clones reference quantities
         self._test = _test
+        if self._test:
+            self._rootdir = None
+        else:
+            self._rootdir = os.path.abspath(rootdir)
+            self._make_rootdir()  # this will be a git clone / fork;; clones reference quantities
         self._blackbook_client = None
         super(LcCatalog, self).__init__(self._rootdir, **kwargs)
 
     def __del__(self):
         """
         This is unreliable- temp directories tend to accumulate
         :return:
         """
         if self._blackbook_client:
             self._blackbook_client.close()
-        if self._test:
-            # print('tryna delete %s' % self.root)
-            rmtree(self.root, ignore_errors=True)
+        # if self._test:  # no longer need to do this
+        #     # print('tryna delete %s' % self.root)
+        #     rmtree(self.root, ignore_errors=True)
 
     def save_local_changes(self):
+        if self._test:
+            logging.warning('Cannot save changes during tester operation')
+            return
         self._qdb.write_to_file(self._reference_qtys, characterizations=True, values=True)
         self.lcia_engine.save_flowables(self._flowables)
         self.lcia_engine.save_contexts(self._contexts)
 
     def restore_contexts(self, really=False):
+        if self._test:
+            logging.warning('Cannot save changes during tester operation')
+            return
         if really:
             print('Overwriting local contexts')
             copy2(DEFAULT_CONTEXTS, self._contexts)
         else:
             print('pass really=True if you really want to overwrite local contexts')
 
     def restore_qdb(self, really=False):
+        # this is all deprecated-- need to rework how qdb is initialized and re-initialized
+        if self._test:
+            logging.info('Cannot save changes during tester operation')
+            return
         if really:
             copy2(REF_QTYS, self._reference_qtys)
             print('Reference quantities restored. Please re-initialize the catalog.')
 
     '''
     Create + Add data resources
     '''
@@ -146,25 +165,35 @@
         :param reference:
         :param source:
         :param ds_type:
         :param store: [True] permanently store this resource
         :param kwargs: interfaces=None, priority=0, static=False; **kwargs passed to archive constructor
         :return:
         """
-        source = self._localize_source(source)
-        return self._resolver.new_resource(reference, source, ds_type, store=store, **kwargs)  # explicit store= for doc purposes
+        if self._test:
+            store = False
+        else:
+            source = self._localize_source(source)
+        res = self._resolver.new_resource(reference, source, ds_type, store=store, **kwargs)  # explicit store= for doc purposes
+        if res.origin in self._nicknames:
+            self._nicknames.pop(res.origin)
+        return res
 
     def add_resource(self, resource, store=True):
         """
         Add an existing LcResource to the catalog.
         :param resource:
         :param store: [True] permanently store this resource
         :return:
         """
+        if self._test:
+            store = False
         self._resolver.add_resource(resource, store=store)
+        if resource.origin in self._nicknames:
+            self._nicknames.pop(resource.origin)
 
     def purge_resource_archive(self, resource: LcResource):
         """
         - find all cached queries that could return the resource
         - check their cached ifaces to see if they use our archive
         - delete those entries from the cache
         :param resource:
@@ -279,16 +308,16 @@
         :param kwargs: init args to add to returned resources, such as 'verify' certificate paths
         :return:
         """
         res = list(self.resources(origin))
         if len(res) > 0:
             return self.refresh_xdb_tokens(origin)
         else:
-            resource_dict = self._blackbook_client.get_one(dict, 'origins', origin, 'resource')
-            return self._configure_blackbook_resources(resource_dict, store=store, **kwargs)
+            resource_list = self._blackbook_client.get_many(ResourceSpec, 'origins', origin, 'resource')
+            return self._configure_blackbook_resources(resource_list, store=store, **kwargs)
 
     '''
     def get_blackbook_resources_by_client(self, bb_client, username, origin, store=False):
         """
         this uses the local maintenance client rather than the REST client
         :param bb_client:
         :param username:
@@ -296,64 +325,62 @@
         :param store:
         :return:
         """
         resource_dict = bb_client.retrieve_resource(username, origin)
         return self._finish_get_blackbook_resources(resource_dict, store=store)
     '''
 
-    def _configure_blackbook_resources(self, resource_dict, store=False, **kwargs):
+    def _configure_blackbook_resources(self, resource_list, store=False, **kwargs):
         """
         Emerging issue here in the xdb/oryx context-- we need to be able to replace resources even if they are
         serialized and already initialized.
 
         response: this is easy- the XdbClient provider (and subclasses) has refresh_token and refresh_auth methods
         already.
 
         What this function does: for each entry in resource dict:
          - find the first resource that matches origin + ds_type
          - if one exists, update it:
            = if source matches, update token
            = else, update source and token
          - else: create it
 
-        :param resource_dict: a dict of origin: [resource specs]
+        :param resource_dict: a list of [resource specs]
         :return:
         """
 
         rtn = []
 
-        for recv_origin, res_list in resource_dict.items():
-            # self._resolver.delete_origin(recv_origin)
-            for res in res_list:
-                if not isinstance(res, ResourceSpec):
-                    res = ResourceSpec(**res)
-                try:
-                    exis = next(x for x in self.resources(recv_origin) if x.ds_type == res.ds_type)
-                    exis.init_args.update(kwargs)
-                    exis.check(self)
-                    # one exists-- update it
-                    exis.init_args.update(res.options)
-                    if exis.source == res.source:
-                        exis.archive.refresh_token(res.options['token'])
-                    else:
-                        exis.source = res.source
-                        exis.archive.refresh_auth(res.source, res.options['token'])
-                    for i in res.interfaces:
-                        if i not in exis.interfaces:
-                            exis.add_interface(i)
-                    for i in exis.interfaces:
-                        if i not in res.interfaces:
-                            exis.remove_interface(i)
-                    if store:
-                        exis.write_to_file(self.resource_dir)
-                    rtn.append(exis)
-                except StopIteration:
-                    r = LcResource(**res.model_dump(), **kwargs)
-                    self.add_resource(r, store=store)
-                    rtn.append(r)
+        for res in resource_list:
+            if not isinstance(res, ResourceSpec):
+                res = ResourceSpec(**res)
+            try:
+                exis = next(x for x in self.resources(res.origin) if x.ds_type == res.ds_type)
+                exis.init_args.update(kwargs)
+                exis.check(self)
+                # one exists-- update it
+                exis.init_args.update(res.options)
+                if exis.source == res.source:
+                    exis.archive.refresh_token(res.options['token'])
+                else:
+                    exis.source = res.source
+                    exis.archive.refresh_auth(res.source, res.options['token'])
+                for i in res.interfaces:
+                    if i not in exis.interfaces:
+                        exis.add_interface(i)
+                for i in exis.interfaces:
+                    if i not in res.interfaces:
+                        exis.remove_interface(i)
+                if store:
+                    exis.write_to_file(self.resource_dir)
+                rtn.append(exis)
+            except StopIteration:
+                r = LcResource(**res.model_dump(), **kwargs)
+                self.add_resource(r, store=store)
+                rtn.append(r)
         return rtn
 
     def refresh_xdb_tokens(self, origin):
         """
         requires an active blackbook client (try blackbook_authenticate() if it has expired)
         :param origin:
         :return:
@@ -373,98 +400,103 @@
     '''
     Manage resources locally
      - index
      - cache
      - static archive (performs load_all())
     '''
 
-    def _index_source(self, source, priority, force=False):
+    def _index_source(self, source, priority, force=False, save=True):
         """
         Instructs the resource to create an index of itself in the specified file; creates a new resource for the
         index
         :param source:
         :param priority:
         :param force:
         :return:
         """
         res = next(r for r in self._resolver.resources_with_source(source))
         res.check(self)
         priority = min([priority, res.priority])  # why are we doing this?? we want index to have higher priority i.e. get loaded second
-        stored = self._resolver.is_permanent(res)
+        store = (self._resolver.is_permanent(res) or save) and not self._test
 
         # save configuration hints in derived index
         cfg = None
-        if stored:
-            if len(res.config['hints']) > 0:
-                cfg = {'hints': res.config['hints']}
-
-        inx_file = self._index_file(source)
-        inx_local = self._localize_source(inx_file)
-
-        if os.path.exists(inx_file):
-            if not force:
-                print('Not overwriting existing index. force=True to override.')
-                try:
-                    ex_res = next(r for r in self._resolver.resources_with_source(inx_local))
-                    return ex_res.origin
-                except StopIteration:
-                    # index file exists, but no matching resource
-                    inx = archive_from_json(inx_file)
-                    self.new_resource(inx.ref, inx_local, 'json', priority=priority, store=stored,
-                                      interfaces='index', _internal=True, static=True, preload_archive=inx,
-                                      config=cfg)
-
-                    return inx.ref
-
-            print('Re-indexing %s' % source)
-            # TODO: need to delete the old index resource!!
-            stale_res = list(self._resolver.resources_with_source(inx_local))
-            stale_refs = list(set(res.origin for res in stale_res))
-            for stale in stale_res:
-                # this should be postponed to after creation of new, but that fails in case of naming collision (bc YYYYMMDD)
-                # so golly gee we just delete-first.
-                print('deleting %s' % stale.origin)
-                self.delete_resource(stale)
-            # we also need to delete derived internal resources
-            for stale_ref in stale_refs:
-                for stale in list(self.resources(stale_ref)):
-                    if stale.internal:
-                        self.delete_resource(stale)
+        if len(res.config['hints']) > 0:
+            cfg = {'hints': res.config['hints']}
 
-        the_index = res.make_index(inx_file, force=force)
-        self.new_resource(the_index.ref, inx_local, 'json', priority=priority, store=stored, interfaces='index',
+        if store:
+            inx_file = self._index_file(source)
+            inx_local = self._localize_source(inx_file)
+
+            if os.path.exists(inx_file):
+                if not force:
+                    print('Not overwriting existing index. force=True to override.')
+                    try:
+                        ex_res = next(r for r in self._resolver.resources_with_source(inx_local))
+                        return ex_res.origin
+                    except StopIteration:
+                        # index file exists, but no matching resource
+                        inx = archive_from_json(inx_file)
+                        self.new_resource(inx.ref, inx_local, 'json', priority=priority, store=store,
+                                          interfaces='index', _internal=True, static=True, preload_archive=inx,
+                                          config=cfg)
+
+                        return inx.ref
+
+                print('Re-indexing %s' % source)
+                # TODO: need to delete the old index resource!!
+                stale_res = list(self._resolver.resources_with_source(inx_local))
+                stale_refs = list(set(res.origin for res in stale_res))
+                for stale in stale_res:
+                    # this should be postponed to after creation of new, but that fails in case of naming collision (bc YYYYMMDD)
+                    # so golly gee we just delete-first.
+                    print('deleting %s' % stale.origin)
+                    self.delete_resource(stale)
+                # we also need to delete derived internal resources
+                for stale_ref in stale_refs:
+                    for stale in list(self.resources(stale_ref)):
+                        if stale.internal:
+                            self.delete_resource(stale)
+        else:
+            inx_file = inx_local = None
+
+        the_index = res.make_index(inx_file, force=force, save=store)
+        if inx_local is None:
+            inx_local = the_index.ref
+        self.new_resource(the_index.ref, inx_local, 'json', priority=priority, store=store, interfaces='index',
                           _internal=True, static=True, preload_archive=the_index, config=cfg)
 
         return the_index.ref
 
-    def index_ref(self, origin, interface=None, source=None, priority=60, force=False, strict=True):
+    def index_ref(self, origin, interface=None, source=None, priority=60, save=True, force=False, strict=True):
         """
         Creates an index for the specified resource.  'origin' and 'interface' must resolve to one or more LcResources
         that all have the same source specification.  That source archive gets indexed, and index resources are created
         for all the LcResources that were returned.
 
         Performs load_all() on the source archive, writes the archive to a compressed json file in the local index
         directory, and creates a new LcResource pointing to the JSON file.   Aborts if the index file already exists
         (override with force=True).
         :param origin:
         :param interface: [None]
         :param source: find_single_source input
         :param priority: [60] priority setting for the new index
+        :param save: [True] whether to save the index
         :param force: [False] if True, overwrite existing index
         :param strict: [True] whether to be strict
         :return:
         """
         if not force:
             try:
                 ix = next(self.gen_interfaces(origin, itype='index', strict=False))
                 return ix.origin
             except StopIteration:
                 pass
         source = self._find_single_source(origin, interface, source=source, strict=strict)
-        return self._index_source(source, priority, force=force)
+        return self._index_source(source, priority, force=force, save=save)
 
     def cache_ref(self, origin, interface=None, source=None, static=False):
         source = self._find_single_source(origin, interface, source=source)
         self.create_source_cache(source, static=static)
 
     def create_source_cache(self, source, static=False):
         """
@@ -481,18 +513,22 @@
                 return
             print('Archiving static resource %s' % res)
         res.check(self)
         res.make_cache(self.cache_file(self._localize_source(source)))
 
     def _background_for_origin(self, ref, strict=False):
         res = self.get_resource(ref, iface='exchange')
-        inx_ref = self.index_ref(ref, interface='exchange', strict=strict)
-        bk_file = self._localize_source(os.path.join(self.archive_dir, '%s_background.mat' % inx_ref))
+        store = self._resolver.is_permanent(res) and not self._test
+        inx_ref = self.index_ref(ref, interface='exchange', strict=strict, save=store)
+        if store:
+            bk_file = self._localize_source(os.path.join(self.archive_dir, '%s_background.mat' % inx_ref))
+        else:
+            bk_file = '%s_background.mat' % inx_ref
         bk = LcResource(inx_ref, bk_file, 'Background', interfaces='background', priority=99,
-                        save_after=True, _internal=True)
+                        save_after=store, _internal=True)
         bk.config = res.config
         bk.check(self)  # ImportError if antelope_background pkg not found;; also applies configs
         self.add_resource(bk)
         return bk.make_interface('background')  # when the interface is returned, it will trigger setup_bm
 
     def gen_interfaces(self, origin, itype=None, strict=False, ):
         """
```

### Comparing `antelope_core-0.3.0/antelope_core/catalog/lc_resolver.py` & `antelope_core-0.3.1/antelope_core/catalog/lc_resolver.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,19 +21,23 @@
      archives by turning the fragments into processes.
 
     This file could probably be re-thought, especially in the era of resources delivered via web.  For now, we will
      monkeypatch.
     """
     def __init__(self, resource_dir):
         self._resource_dir = resource_dir
-        if not os.path.exists(resource_dir):
+        if not self.test and not os.path.exists(resource_dir):
             os.makedirs(resource_dir)
         self._resources = defaultdict(list)
         self.index_resources()
 
+    @property
+    def test(self):
+        return self._resource_dir is None
+
     def delete_origin(self, origin):
         """
         remove all resources for a given origin.
 
         :param origin:
         :return:
         """
@@ -75,29 +79,31 @@
         except json.JSONDecodeError:
             print('Skipping Invalid resource file %s' % path)
             # os.remove(path)
             return
         self._resources[org] = resources
 
     def index_resources(self):
+        if self.test:
+            return
         for org in os.listdir(self._resource_dir):
             self._update_semantic_ref(org)
 
     def add_resource(self, resource, store=True):
         """
         Add a resource to the resolver's list.  By default, save the resource permanently as a file in resources dir.
         :param resource:
         :param store: [True] if False, add the resource to memory only
         :return:
         """
         if resource.exists(self._resource_dir) or self.has_resource(resource):
             # do nothing
             print('Resource already exists')
             return
-        if store and os.path.exists(self._resource_dir):
+        if (not self.test) and store and os.path.exists(self._resource_dir):
             resource.write_to_file(self._resource_dir)
         self._resources[resource.origin].append(resource)
 
     def has_resource(self, resource):
         s = resource.serialize()
         return any(k.matches(s) for k in self._resources[resource.origin])
 
@@ -132,14 +138,16 @@
     def resources_with_source(self, source):
         for ref, ress in self._resources.items():
             for r in ress:
                 if r.source == source:
                     yield r
 
     def is_permanent(self, resource):
+        if self.test:
+            return False
         return resource.exists(self._resource_dir)
 
     def resolve(self, req, interfaces=None, strict=False):
         """
         Fuzzy resolver returns all resources that match the request and have equal or greater specificity.
         'uslci.clean' will match queries for 'uslci' but not for 'uslci.original' or 'uslci.clean.allocated'.
         However, 'uslci.clean.allocated' will match a query for 'uslci.clean'
@@ -207,15 +215,15 @@
         Writes the resource file into the resource_dir containing only the resources that are both
         (1) provided to the method and (2) already present in the resource_dir.  The purpose of this is to allow
         deletion of single resources for a particular origin.
         :param ref:
         :param resources:
         :return:
         """
-        if not os.path.exists(self._resource_dir):
+        if self.test or not os.path.exists(self._resource_dir):
             return
         j = [k.serialize() for k in resources if k.exists(self._resource_dir)]
         if len(j) == 0:
             os.remove(os.path.join(self._resource_dir, ref))
             return
         with open(os.path.join(self._resource_dir, ref), 'w') as fp:
             json.dump({ref: j}, fp)
```

### Comparing `antelope_core-0.3.0/antelope_core/catalog/tests/test_catalogs.py` & `antelope_core-0.3.1/antelope_core/catalog/tests/test_catalogs.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 from .. import LcCatalog
 from ...lc_resource import LcResource
 from ...catalog_query import CatalogQuery, READONLY_INTERFACE_TYPES
 from ...archives.tests import basic_archive_src
 
 
 import os
+import tempfile
 import unittest
+from shutil import rmtree
 
 
 uslci_fg = LcResource('test.uslci', '/data/LCI/USLCI/USLCI_Processes_ecospold1.zip', 'EcospoldV1Archive',
                       interfaces='inventory',
                       priority=40,
                       static=False,
                       prefix='USLCI_Processes_ecospold1/USLCI_Processes_ecospold1')
@@ -40,19 +42,28 @@
 test_resource = LcResource('test.basic', basic_archive_src, 'json',
                            interfaces=('basic', 'exchange'))
 
 
 class LcCatalogFixture(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
-        cls._cat = LcCatalog.make_tester()
+        """
+        Purpose of this class is to test behavior of persistent catalogs, so we should not use make_tester()
+        :return:
+        """
+        cls.tmp = tempfile.mkdtemp()
+        cls._cat = LcCatalog(cls.tmp)
         cls._cat.add_resource(uslci_fg)
         cls._cat.add_resource(uslci_bg)
         cls._cat.add_resource(test_resource)
 
+    @classmethod
+    def tearDownClass(cls) -> None:
+        rmtree(cls.tmp)
+
     def test_resolver_index(self):
         self.assertSetEqual({r for r in self._cat.origins}, {'local.qdb', 'test.uslci', 'test.uslci.allocated',
                                                                 'test.basic'})
     @unittest.skip  # this doesn't work at all-- priority (and resolver generally) still need to be tested
     def test_priority(self):
         # TODO!
         q = CatalogQuery('test.uslci', catalog=self._cat)
@@ -119,10 +130,9 @@
         self.assertTrue(os.path.exists(abs_path))  # abs_path exists
         self._cat.delete_resource(res, delete_source=True)
         self.assertFalse(os.path.exists(abs_path))  # abs_path removed
 
     # def test_lcia_db(self):
 
 
-
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `antelope_core-0.3.0/antelope_core/catalog/tests/test_process_ref.py` & `antelope_core-0.3.1/antelope_core/catalog/tests/test_process_ref.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/catalog/tests/test_quantity_refs.py` & `antelope_core-0.3.1/antelope_core/catalog/tests/test_quantity_refs.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 
 class QuantityRefTest(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         cls.gwp = next(cat.query(org).lcia_methods(Name='Global Warming'))  # canonical
         cls.gwp_ref = cat._qdb[cls.gwp.external_ref]  # original ref (locally stored)
-        cls.gwp_true = cat.get_archive(cls.gwp_ref.origin).get(cls.gwp_ref.external_ref)  # authentic entity
+        cls.gwp_true = cat.get_archive(org).get(cls.gwp_ref.external_ref)  # authentic entity
 
     def test_origins(self):
         self.assertEqual(self.gwp.origin, org)
         self.assertEqual(self.gwp_ref.origin, org)
         self.assertEqual(self.gwp._query.origin, 'local.qdb')
         res = cat.get_resource(org)
         self.assertEqual(self.gwp_true.origin, res.archive.names[res.source])
```

### Comparing `antelope_core-0.3.0/antelope_core/catalog_query.py` & `antelope_core-0.3.1/antelope_core/catalog_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 """
 Query Interface -- used to operate catalog refs
 """
 
-from antelope import (IndexInterface, BackgroundInterface, ExchangeInterface, QuantityInterface, EntityNotFound,
-                      UnknownOrigin,
-                      ExchangeRef, comp_dir, BaseEntity)
-#                      ForegroundInterface,
-#                      IndexRequired, PropertyExists,
-#                      )
-from antelope.refs.exchange_ref import RxRef
+from antelope import (BasicInterface, IndexInterface, BackgroundInterface, ExchangeInterface, QuantityInterface,
+                      EntityNotFound, UnknownOrigin,
+                      ExchangeRef, comp_dir, CatalogRef)
 
-from antelope.models import LciaResult as LciaResultModel, Characterization as CharacterizationModel
+from antelope.refs import FlowRef, RxRef
+
+from antelope.models import Entity, LciaResult as LciaResultModel, Characterization as CharacterizationModel
 
 from .lcia_results import LciaResult
 from .characterizations import QRResult, Characterization
 from .contexts import NullContext
 
 from synonym_dict import InconsistentLineage
 
@@ -39,15 +37,15 @@
     pass
 
 
 class BadInterfaceSpec(Exception):
     pass
 
 
-class CatalogQuery(IndexInterface, BackgroundInterface, ExchangeInterface, QuantityInterface):
+class CatalogQuery(BasicInterface, IndexInterface, BackgroundInterface, ExchangeInterface, QuantityInterface):
     """
     A CatalogQuery is a class that performs any supported query against a supplied catalog.
     Supported queries are defined in the lcatools.interfaces, which are all abstract.
     Implementations also subclass the abstract classes.
 
     This reduces code duplication (all the catalog needs to do is provide interfaces) and ensures consistent signatures.
 
@@ -231,15 +229,15 @@
     '''
     '''
     def get_context(self, term, **kwargs):
         cx = super(CatalogQuery, self).get_context(term, **kwargs)
         return self._tm[cx]
     '''
 
-    def get_canonical(self, quantity: str | BaseEntity, **kwargs):
+    def get_canonical(self, quantity, **kwargs):
         try:
             # print('Gone canonical')
             q_can = self._tm.get_canonical(quantity)
         except EntityNotFound:
             if hasattr(quantity, 'entity_type') and quantity.entity_type == 'quantity':
                 print('Missing canonical quantity-- adding to LciaDb')
                 self._catalog.register_entity_ref(quantity)
@@ -343,24 +341,21 @@
             
             True, the data won't match the source.  but we will still RECOGNIZE the source because we will register the 
             quantity terms with the term manager.  Which we WEREN"T doing before.
             
             A corollary of this is that CatalogQuery.get() should get_canonical FIRST
             '''
             try:
-                return self._tm.get_canonical(entity.link)
+                _ = self._tm.get_canonical(entity)
             except EntityNotFound:
-                try:
-                    _ = self._tm.get_canonical(entity)
-                except EntityNotFound:
-                    self._catalog.register_entity_ref(e_ref)
-                    return self._tm.get_canonical(entity)
-                # print('@@@ Canonical quantity missing link-- adding direct to qm')  # I predict this never occurs
-                # in fact, it occurred several times immediately
-                return self._tm.add_quantity(entity)  # this will be identical to _ unless there is a unit conflict
+                self._catalog.register_entity_ref(e_ref)
+                return self._tm.get_canonical(entity)
+            # print('@@@ Canonical quantity missing link-- adding direct to qm')  # I predict this never occurs
+            # in fact, it occurred several times immediately
+            return self._tm.add_quantity(entity)  # this will be identical to _ unless there is a unit conflict
         else:
             return e_ref
 
     '''
     de-reference Characterization factor models
     '''
 
@@ -396,33 +391,47 @@
         """
         Constructs a Detailed LCIA result from a background LCIA query, when we don't have a list of exchanges
         :param process_ref:
         :param quantity:
         :param res_m:
         :return:
         """
+        if isinstance(quantity, str):
+            try:
+                quantity = self._tm.get_canonical(quantity)
+            except EntityNotFound:
+                quantity = CatalogRef.from_json(res_m.quantity.serialize())  # dumbest thing ever
+
         res = LciaResult(quantity, scenario=res_m.scenario, scale=res_m.scale)
         process = self.get(process_ref)
         for c in res_m.components:
             for d in c.details:
                 value = d.result / d.factor.value
                 cx = self._tm[tuple(d.factor.context)]
+                rq = self.get_canonical(d.exchange.quantity_ref)
                 try:
-                    flow_ref = self.cascade(d.exchange.origin).get(d.exchange.external_ref)
+                    # OK - here we are making redundant orphan FlowRefs, one per detail, to avoid excess API calls.
+                    flow_ref = FlowRef(d.exchange.external_ref, self.cascade(d.exchange.origin),
+                                       name=d.exchange.name, reference_entity=rq, context=cx)
                 except UnknownOrigin:
-                    flow_ref = self.get(d.exchange.external_ref, origin=d.exchange.origin)
-                ex_dir = comp_dir(cx.sense)
+                    flow_ref = FlowRef(d.exchange.external_ref, self, masquerade=d.exchange.origin,
+                                       name=d.exchange.name, reference_entity=rq, context=cx)
+                ex_dir = d.exchange.direction
+                '''
                 if ex_dir is None:
                     print('Bad context: %s' % list(cx))
                     print('using "Output" direction')
                     ex_dir = 'Output'
+                '''
+                if cx.sense:
+                    if ex_dir != comp_dir(cx.sense):
+                        value *= -1  # DetailedLciaResult will negate the result internally
                 ex = ExchangeRef(process, flow_ref,
                                  ex_dir,
                                  termination=cx, value=value)
-                rq = self.get_canonical(d.exchange.quantity_ref)
                 cf = QRResult(d.factor.flowable, rq, quantity, cx,
                               d.factor.locale, d.factor.origin, d.factor.value)
                 res.add_score(c.component, ex, cf)
         for s in res_m.summaries:
             res.add_summary(s.component, s.component, s.node_weight, s.unit_score)
         return res
```

### Comparing `antelope_core-0.3.0/antelope_core/characterizations.py` & `antelope_core-0.3.1/antelope_core/characterizations.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/contexts.py` & `antelope_core-0.3.1/antelope_core/contexts.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
    all contexts, as long as a more applicable characterization is not found.
  - on the query side, NullContext indicates that a context was specified but no match was found.  Queries with
    NullContext should not match any existing characterizations (except NullContext itself).
 
 The NullContext should be returned by the context manager
 """
 
-from synonym_dict import Compartment, CompartmentManager, NonSpecificCompartment, TermExists
+from synonym_dict import Compartment, CompartmentManager, NonSpecificCompartment, TermExists, MergeError
 from synonym_dict.compartments.compartment import InvalidSubCompartment
 from antelope import valid_sense
 
 SINKS = {'emission', 'emissions'}
 SOURCES = {'resource', 'resources'}
 
 ELEMENTARY = {'elementary flows'} | SINKS | SOURCES
@@ -361,15 +361,18 @@
             parent = new
         return new
     '''
 
     def _add_but_not_protected(self, entry, context):
         self.add_synonym(entry, context.fullname)
         if context.name.lower() not in PROTECTED:
-            self.add_synonym(entry, context.name)
+            try:
+                self.add_synonym(entry, context.name)
+            except TermExists:
+                pass
 
     def find_matching_context(self, context):
         """
         A complicated function to both (1) retrieve the best / most-specific "canonical" context for a given "foreign"
         (i.e. incoming) context and also (2) add the full semantic content of the foreign context to the canonical
         context manager.
 
@@ -429,15 +432,21 @@
                     else:  # new
                         """
                         DWR! Changing core behavior! We have an existing match but our foreign context is more specific
                         so-- add a new canonical context
                         
                         (old behavior was to smush all foreign subcontexts together into the canonical context)
                         """
-                        nxt = self.new_entry(this.name, parent=current, sense=this.sense)
+                        try:
+                            nxt = self.new_entry(this.name, parent=current, sense=this.sense)
+                        except MergeError:
+                            # for some reason USLCI FY21 has a "from ground, subterranean" category??
+                            merge_name = ', '.join([current.name, this.name])
+                            nxt = self.new_entry(merge_name, parent=current, sense=this.sense)
+                            # this fix is awfully special-purpose but hey- things are mostly working
                         nxt.add_origin(this.origin)
                         self._add_but_not_protected(nxt, this)
                         current = nxt
         if current is not NullContext:
             self._add_but_not_protected(current, context)
         return current
```

### Comparing `antelope_core-0.3.0/antelope_core/data_sources/data_source.py` & `antelope_core-0.3.1/antelope_core/data_sources/data_source.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/data_sources/ecoinvent.py` & `antelope_core-0.3.1/antelope_core/data_sources/ecoinvent.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/data_sources/ecoinvent_lcia.py` & `antelope_core-0.3.1/antelope_core/data_sources/ecoinvent_lcia.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/data_sources/gwp_ipcc_2007.py` & `antelope_core-0.3.1/antelope_core/data_sources/gwp_ipcc_2007.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/data_sources/local.py` & `antelope_core-0.3.1/antelope_core/data_sources/local.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/data_sources/tests/test_aa_local.py` & `antelope_core-0.3.1/antelope_core/data_sources/tests/test_aa_local.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/data_sources/tests/test_ecoinvent.py` & `antelope_core-0.3.1/antelope_core/data_sources/tests/test_ecoinvent.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/data_sources/tests/test_ecoinvent_lci.py` & `antelope_core-0.3.1/antelope_core/data_sources/tests/test_ecoinvent_lci.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/data_sources/tests/test_ipcc2007.py` & `antelope_core-0.3.1/antelope_core/data_sources/tests/test_ipcc2007.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,13 +22,13 @@
 
     def test_num_entities(self):
         self.assertEqual(self.query.count('quantity'), 2)
         self.assertEqual(self.query.count('flow'), 0)
 
     def test_gwp(self):
         gwp = next(self.query.lcia_methods())
-        self.assertEqual(gwp.name, 'Global Warming Air [kg CO2 eq] [LCIA]')
+        self.assertEqual(gwp.name, 'Global Warming Air [kg CO2 eq] [TRACI 2.1]')
         self.assertEqual(len([k for k in gwp.factors()]), 91)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `antelope_core-0.3.0/antelope_core/data_sources/tests/test_traci.py` & `antelope_core-0.3.1/antelope_core/data_sources/tests/test_traci.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/data_sources/tests/test_uslci.py` & `antelope_core-0.3.1/antelope_core/data_sources/tests/test_uslci.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/data_sources/traci.py` & `antelope_core-0.3.1/antelope_core/data_sources/traci.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/data_sources/uslci/uslci.py` & `antelope_core-0.3.1/antelope_core/data_sources/uslci/uslci.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/entities/entities.py` & `antelope_core-0.3.1/antelope_core/entities/entities.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,29 +72,46 @@
                 continue
             self[k] = v
 
     @property
     def reference_entity(self):
         return self._reference_entity
 
+    def _make_ref(self, query):
+        """
+        Type-Specific Ref maker.
+        :param query:
+        :return: a CatalogRef
+        """
+        d = dict()
+        for k in self.properties():
+            v = self._d[k]
+            if hasattr(v, 'make_ref'):
+                v = v.make_ref(query)
+            d[k] = v
+        '''
+        for k in self.signature_fields():
+            if k == self._ref_field:
+                continue
+            if k in self._d:
+                d[k] = self._d[k]
+        '''
+        # this is a potential DWR--
+        # if the query does not match the entity, we want the ref to have the authentic origin
+        # we're expecting this to only occur from within CatalogQuery._grounded_query() -> UnknownOrigin
+        if 'uuid' not in d:
+            if self.uuid is not None:
+                d['uuid'] = self.uuid
+        if query.origin != self.origin:
+            d['masquerade'] = self.origin
+        return CatalogRef.from_query(self.external_ref, query, self.entity_type, **d)
+
     def make_ref(self, query):
         if self._query_ref is None:
-            d = dict()
-            for k in self.signature_fields():
-                if k == self._ref_field:
-                    continue
-                if k in self._d:
-                    d[k] = self._d[k]
-            # this is a potential DWR--
-            # if the query does not match the entity, we want the ref to have the authentic origin
-            # we're expecting this to only occur from within CatalogQuery._grounded_query() -> UnknownOrigin
-            if query.origin != self.origin:
-                d['masquerade'] = self.origin
-            self._query_ref = CatalogRef.from_query(self.external_ref, query, self.entity_type,
-                                                    uuid=self.uuid, **d)
+            self._query_ref = self._make_ref(query)
         return self._query_ref
 
     @property
     def entity_type(self):
         return self._entity_type
 
     @property
@@ -137,20 +154,14 @@
     def reference_field(self):
         return self._ref_field
 
     @property
     def external_ref(self):
         return self._external_ref
 
-    def get_signature(self):
-        k = dict()
-        for i in self.signature_fields():
-            k[i] = self[i]
-        return k
-
     @property
     def uuid(self):
         return self._uuid
 
     @uuid.setter
     def uuid(self, key):
         if self._uuid is not None:
```

### Comparing `antelope_core-0.3.0/antelope_core/entities/flows.py` & `antelope_core-0.3.1/antelope_core/entities/flows.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,29 +58,21 @@
         for k in self._new_fields:
             if k not in self._d:
                 self._d[k] = ''
 
         if self.reference_entity is None:
             print('Warning: no reference quantity for flow %s' % external_ref)
 
-    def make_ref(self, query):
-        if self._query_ref is None:
-            d = dict()
-            for k in self.signature_fields():
-                if k == self._ref_field:
-                    continue
-                if k in self._d:
-                    d[k] = self._d[k]
-            self._query_ref = CatalogRef.from_query(self.external_ref, query, self.entity_type,
-                                                    uuid=self.uuid, **d)
-            self._query_ref.context = self.context
-            for k, v in self._chars_seen.items():
-                self._query_ref._chars_seen[k] = v  # this is hacky obv
+    def _make_ref(self, query):
+        query_ref = super(LcFlow, self)._make_ref(query)
+        query_ref.context = self.context
+        for k, v in self._chars_seen.items():
+            query_ref._chars_seen[k] = v  # this is hacky obv
 
-        return self._query_ref
+        return query_ref
 
     def __str__(self):
         cas = self.get('CasNumber')
         if cas is None:
             cas = ''
         if len(cas) > 0:
             cas = ' (CAS ' + cas + ')'
```

### Comparing `antelope_core-0.3.0/antelope_core/entities/processes.py` & `antelope_core-0.3.1/antelope_core/entities/processes.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/entities/quantities.py` & `antelope_core-0.3.1/antelope_core/entities/quantities.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/entities/tests/base_testclass.py` & `antelope_core-0.3.1/antelope_core/entities/tests/base_testclass.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/entities/tests/test_archive.json` & `antelope_core-0.3.1/antelope_core/entities/tests/test_archive.json`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/entities/tests/test_entities.py` & `antelope_core-0.3.1/antelope_core/entities/tests/test_entities.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/entities/tests/test_entity_refs.py` & `antelope_core-0.3.1/antelope_core/entities/tests/test_entity_refs.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/entities/tests/test_processes.py` & `antelope_core-0.3.1/antelope_core/entities/tests/test_processes.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/entities/tests/test_quantities.py` & `antelope_core-0.3.1/antelope_core/entities/tests/test_quantities.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/entities/xlsx_editor.py` & `antelope_core-0.3.1/antelope_core/entities/xlsx_editor.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/exchanges.py` & `antelope_core-0.3.1/antelope_core/exchanges.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/file_accessor.py` & `antelope_core-0.3.1/antelope_core/file_accessor.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,17 +27,18 @@
     'index': 50,
     'background': 80
 }
 
 
 class FileAccessor(object):
 
-    def __init__(self, load_path):
+    def __init__(self, load_path, prefix=None):
         self._path = os.path.abspath(load_path)  # this has the benefits of collapsing '..' and trimming trailing '/'
         self._origins = os.listdir(self._path)
+        self._prefix = prefix
 
     @property
     def path(self):
         return self._path
 
     @property
     def origins(self):
@@ -106,29 +107,32 @@
 
     def create_resource(self, source, basic=False, **kwargs):
         if not source.startswith(self._path):
             raise ValueError('Path not contained within our filespace')
         rel_source = source[len(self._path)+1:]
         org, iface, ds_type, fn = rel_source.split(os.path.sep)  # note os.pathsep is totally different
 
+        if self._prefix is not None:
+            org = '.'.join([str(self._prefix), org])
+
         cfg = self.read_config(source)
         cfg.update(kwargs)
         priority = cfg.pop('priority', DEFAULT_PRIORITIES[iface])
 
         # do this last
         ifaces = set()
         ifaces.add(iface)
         for ad in cfg.pop('add_interfaces', ()):
             if ad in INTERFACE_TYPES:
                 ifaces.add(ad)
         if basic:
             ifaces.add('basic')
-        if iface == 'index':
-            # TODO: WORKAROUND: automatically add 'basic' to index interfaces until we have it sorted out
-            ifaces.add('basic')
+        # if iface == 'index':
+        #     # TODO: WORKAROUND: automatically add 'basic' to index interfaces until we have it sorted out
+        #     ifaces.add('basic')
 
         return LcResource(org, source, ds_type, interfaces=tuple(ifaces), priority=priority, **cfg)
 
 
 class ResourceLoader(FileAccessor):
     """
     This class crawls a directory structure and adds all the specified resources to the catalog provided as
```

### Comparing `antelope_core-0.3.0/antelope_core/from_json.py` & `antelope_core-0.3.1/antelope_core/from_json.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/implementations/background.py` & `antelope_core-0.3.1/antelope_core/implementations/background.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import re
 from itertools import chain
 
 from .basic import BasicImplementation
-from antelope import BackgroundInterface, ExteriorFlow, EntityNotFound, comp_dir  # , ProductFlow
+from antelope import BackgroundInterface, EntityNotFound, comp_dir  # , ProductFlow
+from antelope.models import ExteriorFlow
 from antelope_core.contexts import Context
 
 
 class NonStaticBackground(Exception):
     pass
 
 
@@ -100,15 +101,15 @@
                 dirn = comp_dir(cx.sense)  # this is already w.r.t. interior
                 '''
                 if self.is_elementary(f):
                     yield ExteriorFlow(self._archive.ref, f, 'Output', f['Compartment'])
                 else:
                     yield ExteriorFlow(self._archive.ref, f, 'Output', None)
                 '''
-                yield ExteriorFlow(self._archive.ref, f, dirn, cx)
+                yield ExteriorFlow.from_background(f, dirn, cx)
 
     def consumers(self, process, ref_flow=None, **kwargs):
         """
         Not supported for trivial backgrounds
         :param process:
         :param ref_flow:
         :param kwargs:
```

### Comparing `antelope_core-0.3.0/antelope_core/implementations/basic.py` & `antelope_core-0.3.1/antelope_core/implementations/basic.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/implementations/configure.py` & `antelope_core-0.3.1/antelope_core/implementations/configure.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,16 @@
         All options should be supplied as a dict of iterables, where the keys are the configuration methods and
         the entries in each iterable are tuples corresponding to the configuration parameters, properly ordered.
 
         Configuration options should be idempotent; applying them several times should have the same effect as
         applying them once.
         :return:
         """
+        if len(config) == 0:
+            return
         print('Applying configuration to %s' % self._archive)
         # re_index = False
         '''
         # self._apply_config(config, 'add_terms')
         for k in _config['add_terms']:
             print('adding %s synonyms (%s|%d)' % (k[0], k[1], len(k) - 1))
             self.add_terms(*k)
```

### Comparing `antelope_core-0.3.0/antelope_core/implementations/exchange.py` & `antelope_core-0.3.1/antelope_core/implementations/exchange.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/implementations/index.py` & `antelope_core-0.3.1/antelope_core/implementations/index.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/implementations/quantity.py` & `antelope_core-0.3.1/antelope_core/implementations/quantity.py`

 * *Files 0% similar despite different names*

```diff
@@ -498,14 +498,17 @@
                         res = QuantityConversion(query=qq, context=cx)
                         qr_geog.append(self._ref_qty_conversion(rq, fb, cx, res, loc))
 
                 return qr_results, qr_geog, qr_mismatch
 
         for cf in self._archive.tm.factors_for_flowable(fb, quantity=qq, context=cx, **kwargs):
             res = QuantityConversion(cf.query(locale), query=qq, context=cx)
+            if res.value == 0:  # no unit conversion will change this
+                qr_results.append(res)
+                continue
             try:
                 qr_results.append(self._ref_qty_conversion(rq, fb, cx, res, locale))
             except ConversionReferenceMismatch:
                 qr_mismatch.append(QuantityConversionError(res, rq))
             except LocaleMismatch as e:
                 locales = e.args[0]
                 for loc in locales:
```

### Comparing `antelope_core-0.3.0/antelope_core/implementations/tests/test_quantity.py` & `antelope_core-0.3.1/antelope_core/implementations/tests/test_quantity.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/lc_resource.py` & `antelope_core-0.3.1/antelope_core/lc_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
 
         try:
             self._archive = create_archive(src, self.ds_type, factory=herd_factory,
                                            ref=self.origin, **kwargs)
         except FileNotFoundError as e:
             raise ResourceInvalid('%s: %s' % (self.origin, e.filename))
 
-        if catalog is not None and os.path.exists(catalog.cache_file(self.source)):
+        if catalog is not None and catalog.check_cache(self.source):
             update_archive(self._archive, catalog.cache_file(self.source))
         self._static |= self._archive.static
         if self.static and self.ds_type.lower() != 'json':
             self._archive.load_all()  # static json archives are loaded on open- load_all() would be redundant
 
     @property
     def is_loaded(self):
@@ -154,24 +154,31 @@
 
     def check(self, catalog):
         if self._archive is None:
             # TODO: try/catch exceptions or return false
             print('QQQQQQQQQQQQQQQQQQ %s QQQQQQQQQQQQQQQQQQ' % self.origin)
             self._instantiate(catalog)
             self.apply_config(catalog)  # can't remember why I set this to happen recurrently- but it's no good
+            ''' # on second thought, I dont think we want to do this-- catalog_names is a mapping of ref to source
+            if catalog:
+                for name in self.archive.catalog_names:
+                    if name not in catalog.origins:
+                        catalog.add_nickname(name, self.origin)
+            '''
+
         return True
 
     def save(self, catalog):
         self.write_to_file(catalog.resource_dir)
 
-    def make_index(self, index_file, force=True):
+    def make_index(self, index_file, force=True, save=True):
         self.check(None)
         self._archive.load_all()
 
-        the_index = index_archive(self._archive, index_file, force=force)
+        the_index = index_archive(self._archive, index_file, force=force, save=save)
 
         return the_index
 
     def make_cache(self, cache_file):
         # note: do not make descendant
         self._archive.write_to_file(cache_file, complete=True, gzip=True)
         print('Created archive of %s containing:' % self._archive)
@@ -179,15 +186,15 @@
 
     def make_interface(self, iface):
         return self._archive.make_interface(iface)
 
     def apply_config(self, catalog=None):
         # if len(self._config) == 0:  # NOW we don't even need to alter blackbook!!!
         #    return
-        print('Applying stored configuration')
+        # print('Applying stored configuration')
         try:
             self._archive.make_interface('configure').apply_config(self._config)
         except InterfaceError:
             pass
         # we are moving this below apply_config to allow the archive to add/edit hints, which it can do because
         # it receives the authentic config dict as an argument
         if catalog is not None:
@@ -289,14 +296,16 @@
             flags.append('%d cfg' % len(self._config))
         fgs = ' '.join(flags)
 
         return 'LcResource(%s, dataSource=%s:%s, %s [%d]%s)' % (self.origin, self.source, self.ds_type,
                                                                 [k for k in self.interfaces], self.priority, fgs)
 
     def exists(self, path):
+        if path is None:
+            return False
         filename = os.path.join(path, self.origin)
         if os.path.exists(filename):
             try:
                 with open(filename, 'r') as fp:
                     j = json.load(fp)
             except json.JSONDecodeError:
                 return False
@@ -356,15 +365,18 @@
             try:
                 cf = self.archive.make_interface('configure')
                 for cfg, cfgs in config_dict.items():
                     for args in cfgs:
                         cf.check_config(cfg, args)
             except InterfaceError:
                 pass
-        self._config = config_dict
+        # apply config without replacing it blindly
+        for k, v in config_dict.items():
+            for t in v:
+                self._config[k].add(tuple(t))
 
     def satisfies(self, ifaces):
         if ifaces is None:
             return True
         if isinstance(ifaces, str):
             ifaces = [ifaces]
         for i in ifaces:
```

### Comparing `antelope_core-0.3.0/antelope_core/lcia_engine/__init__.py` & `antelope_core-0.3.1/antelope_core/lcia_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/lcia_engine/clookup.py` & `antelope_core-0.3.1/antelope_core/lcia_engine/clookup.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/lcia_engine/data/contexts.json` & `antelope_core-0.3.1/antelope_core/lcia_engine/data/contexts.json`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/lcia_engine/data/flowables.json` & `antelope_core-0.3.1/antelope_core/lcia_engine/data/flowables.json`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/lcia_engine/data/ipcc_2007_gwp.json` & `antelope_core-0.3.1/antelope_core/lcia_engine/data/ipcc_2007_gwp.json`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/lcia_engine/lcia_engine.py` & `antelope_core-0.3.1/antelope_core/lcia_engine/lcia_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+import logging
 from collections import defaultdict
 import os
 
-from ..archives.term_manager import TermManager, NoFQEntry
+from ..archives.term_manager import TermManager, NoFQEntry, DuplicateCharacterization
 from ..contexts import Context, NullContext
-from .clookup import CLookup, SCLookup
+from .clookup import CLookup, SCLookup, FactorCollision
 
 from antelope.flows.flow import flowname_is_biogenic
 
 from synonym_dict import TermExists, FlowablesDict
 # from synonym_dict.example_compartments.compartment_manager import InconsistentLineage  # this is not needed
 
 
@@ -341,29 +342,44 @@
         count = 0
         for cf in quantity.factors():
             count += 1
             # print(cf)
             try:
                 fb = self._fm[cf.flowable]
             except KeyError:
-                fb = self._create_flowable(*quantity.query_synonyms(cf.flowable))
+                if quantity.has_lcia_engine():  # this is the native quantity, remember
+                    fb = self._create_flowable(*quantity.query_synonyms(cf.flowable))
+                else:
+                    fb = self._create_flowable(cf.flowable)
 
             self.add_quantity(cf.ref_quantity)  # this may lead to the creation of non-converting quantities if units mismatch
 
             cx = self[cf.context]
 
-            self._qassign(qq, fb, cf, context=cx)
+            try:
+                self._qassign(qq, fb, cf, context=cx)
+            except FactorCollision:
+                rq = self._canonical_q(cf.ref_quantity)
+                ex_cf = self._find_exact_cf(qq, fb, cx, quantity.origin)
+                if rq != ex_cf.ref_quantity:
+                    for loc in cf.locations:
+                        cf = self._create_conversion_cf(ex_cf, rq, cx, qq.origin, loc, cf[loc], overwrite=False)
+                        logging.info('Created unit-conversion CF\n%s' % cf)
+                else:
+                    logging.warning('FactorCollision for %s into %s: %g != %g' % (fb, cx, cf.value, ex_cf.value))
+                    self._dupes.append(DuplicateCharacterization(qq.link, fb, cx.as_list(), qq.origin, cf.flowable, None))
+
         self._factors_for_later[quantity] = True
         print('Imported %d factors for %s' % (count, quantity))
 
     def _check_factors(self, qq):
         if hasattr(self._factors_for_later[qq], 'factors'):
             self.import_cfs(self._factors_for_later.pop(qq))
 
-    def _find_exact_cf(self, qq, fb, cx, origin, flowable):
+    def _find_exact_cf(self, qq, fb, cx, origin):
         try:
             ql = self._qlookup(qq, fb)
         except NoFQEntry:
             return None
         # cfs = ql._context_origin(cx, origin=origin)
         # if fb is self._fm['water']:  # this is not how to handle this
         #     cx = self.add_subcontext(cx, 'flow', flowable)
```

### Comparing `antelope_core-0.3.0/antelope_core/lcia_engine/tests/test_biogenic_co2.py` & `antelope_core-0.3.1/antelope_core/lcia_engine/tests/test_biogenic_co2.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/lcia_engine/tests/test_clookup.py` & `antelope_core-0.3.1/antelope_core/lcia_engine/tests/test_clookup.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/lcia_engine/tests/test_ipcc.py` & `antelope_core-0.3.1/antelope_core/lcia_engine/tests/test_ipcc.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/lcia_engine/tests/test_lcia_engine.py` & `antelope_core-0.3.1/antelope_core/lcia_engine/tests/test_lcia_engine.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/lcia_results.py` & `antelope_core-0.3.1/antelope_core/lcia_results.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/providers/__init__.py` & `antelope_core-0.3.1/antelope_core/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/providers/data/list_of_methods_and_indicators_ecoinvent_v3.2.xlsx` & `antelope_core-0.3.1/antelope_core/providers/data/list_of_methods_and_indicators_ecoinvent_v3.2.xlsx`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/providers/data/traci_2_1_2014_dec_10_0_test.xlsx` & `antelope_core-0.3.1/antelope_core/providers/data/traci_2_1_2014_dec_10_0_test.xlsx`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/providers/ecoinvent_lcia.py` & `antelope_core-0.3.1/antelope_core/providers/ecoinvent_lcia.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/providers/ecospold.py` & `antelope_core-0.3.1/antelope_core/providers/ecospold.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/providers/ecospold2/ecospold2.py` & `antelope_core-0.3.1/antelope_core/providers/ecospold2/ecospold2.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/providers/ecospold2/ecospold2_index.py` & `antelope_core-0.3.1/antelope_core/providers/ecospold2/ecospold2_index.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/providers/ecospold2/master_data.py` & `antelope_core-0.3.1/antelope_core/providers/ecospold2/master_data.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/providers/file_store.py` & `antelope_core-0.3.1/antelope_core/providers/file_store.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/providers/ilcd/ilcd.py` & `antelope_core-0.3.1/antelope_core/providers/ilcd/ilcd.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/providers/ilcd/ilcd_flowables.py` & `antelope_core-0.3.1/antelope_core/providers/ilcd/ilcd_flowables.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/providers/ilcd/ilcd_lcia.py` & `antelope_core-0.3.1/antelope_core/providers/ilcd/ilcd_lcia.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/providers/ilcd/quantity.py` & `antelope_core-0.3.1/antelope_core/providers/ilcd/quantity.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-11da-a746-0800200b9a66.xml` & `antelope_core-0.3.1/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-11da-a746-0800200b9a66.xml`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-11da-a746-0800200c9a66.xml` & `antelope_core-0.3.1/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-11da-a746-0800200c9a66.xml`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-13da-a746-0800200c9a66.xml` & `antelope_core-0.3.1/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-13da-a746-0800200c9a66.xml`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-22da-a746-0800200c9a66.xml` & `antelope_core-0.3.1/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-22da-a746-0800200c9a66.xml`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flows/f579de8c-8897-4bdb-9a0a-b36f8b13282e.xml` & `antelope_core-0.3.1/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flows/f579de8c-8897-4bdb-9a0a-b36f8b13282e.xml`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/1ff9a08c-6fc1-4509-8bcd-a5404c598755.xml` & `antelope_core-0.3.1/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/1ff9a08c-6fc1-4509-8bcd-a5404c598755.xml`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/ad38d542-3fe9-439d-9b95-2f5f7752acaf.xml` & `antelope_core-0.3.1/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/ad38d542-3fe9-439d-9b95-2f5f7752acaf.xml`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/cd950537-0a98-4044-9ba7-9f9a68d0a504.xml` & `antelope_core-0.3.1/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/cd950537-0a98-4044-9ba7-9f9a68d0a504.xml`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/de5104d8-3de0-4218-a29d-b7123ce9ca3c.xml` & `antelope_core-0.3.1/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/de5104d8-3de0-4218-a29d-b7123ce9ca3c.xml`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/providers/ilcd/tests/test_ilcd.py` & `antelope_core-0.3.1/antelope_core/providers/ilcd/tests/test_ilcd.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/providers/openlca/olca_accessor.py` & `antelope_core-0.3.1/antelope_core/providers/openlca/olca_accessor.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/providers/openlca/olca_ref_data.py` & `antelope_core-0.3.1/antelope_core/providers/openlca/olca_ref_data.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/providers/openlca/openlca_jsonld.py` & `antelope_core-0.3.1/antelope_core/providers/openlca/openlca_jsonld.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/providers/openlca/schema_mapping.py` & `antelope_core-0.3.1/antelope_core/providers/openlca/schema_mapping.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/providers/parse_math.py` & `antelope_core-0.3.1/antelope_core/providers/parse_math.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/providers/tests/test_ecospold.py` & `antelope_core-0.3.1/antelope_core/providers/tests/test_ecospold.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/providers/tests/test_xml_widgets.py` & `antelope_core-0.3.1/antelope_core/providers/tests/test_xml_widgets.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/providers/traci/index.py` & `antelope_core-0.3.1/antelope_core/providers/traci/index.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/providers/traci/q_info.py` & `antelope_core-0.3.1/antelope_core/providers/traci/q_info.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/providers/traci/quantity.py` & `antelope_core-0.3.1/antelope_core/providers/traci/quantity.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/providers/traci/test_traci.py` & `antelope_core-0.3.1/antelope_core/providers/traci/test_traci.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/providers/traci/traci_2_1_spreadsheet.py` & `antelope_core-0.3.1/antelope_core/providers/traci/traci_2_1_spreadsheet.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/providers/xdb_client/implementation.py` & `antelope_core-0.3.1/antelope_core/providers/xdb_client/implementation.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,15 +208,15 @@
             return list(self._resolve_ex(ex)
                         for ex in self._archive.r.get_many(AllocatedExchange, _ref(node), _ref(ref_flow), 'inventory'))
         elif scenario:
             return list(self._resolve_ex(ex)
                         for ex in self._archive.r.get_many(AllocatedExchange, _ref(node), 'inventory',
                                                            scenario=scenario))
         else:
-            return list(self._resolve_ex(ex) for ex in self._archive.r.get_many(AllocatedExchange, _ref(node),
+            return list(self._resolve_ex(ex) for ex in self._archive.r.get_many(UnallocatedExchange, _ref(node),
                                                                                 'inventory'))
 
     def dependencies(self, process, ref_flow=None, **kwargs):
         if ref_flow:
             # process inventory
             return list(self._resolve_ex(ex) for ex in self._archive.r.get_many(AllocatedExchange, _ref(process),
                                                                                 _ref(ref_flow), 'dependencies'))
```

### Comparing `antelope_core-0.3.0/antelope_core/providers/xdb_client/requester.py` & `antelope_core-0.3.1/antelope_core/providers/xdb_client/requester.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/providers/xdb_client/rest_client.py` & `antelope_core-0.3.1/antelope_core/providers/xdb_client/rest_client.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/providers/xdb_client/xdb_client.py` & `antelope_core-0.3.1/antelope_core/providers/xdb_client/xdb_client.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/providers/xdb_client/xdb_entities.py` & `antelope_core-0.3.1/antelope_core/providers/xdb_client/xdb_entities.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/providers/xl_dict.py` & `antelope_core-0.3.1/antelope_core/providers/xl_dict.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/providers/xml_widgets.py` & `antelope_core-0.3.1/antelope_core/providers/xml_widgets.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/tests/test_autorange.py` & `antelope_core-0.3.1/antelope_core/tests/test_autorange.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/tests/test_contexts.py` & `antelope_core-0.3.1/antelope_core/tests/test_contexts.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,14 +203,26 @@
         r = self.cm.add_compartments(r_l)
         e = self.cm.add_compartments(e_l)
         self.assertEqual(r.name, 'subterranean')
         self.assertEqual(e.name, 'to water, subterranean')
         self.assertListEqual(r.as_list(), ['elementary flows', 'Resources', 'from water', 'subterranean'])
         self.assertListEqual(e.as_list(), ['elementary flows', 'Emissions', 'to water', 'subterranean'])
 
+    def test_remote_merge_error(self):
+        sub_g = ['resources', 'ground', 'subterranean']
+        sub_w = ['resources', 'water', 'subterranean']
+        gs = self.cm.add_compartments(sub_g)
+        ws = self.cm.add_compartments(sub_w)
+        self.assertEqual(gs.name, 'subterranean')
+        self.assertEqual(ws.name, 'from water, subterranean')
+        cxx = Context('from water')
+        cxxx = Context('subterranean', parent=cxx)
+        cxxx.add_origin('far.away')
+        self.assertIs(self.cm.find_matching_context(cxxx), ws)
+
 
 class DefaultContextsTest(unittest.TestCase):
     def setUp(self):
         self.cm = ContextManager(source_file=DEFAULT_CONTEXTS)
 
     def test_load(self):
         self.assertEqual(len(self.cm), NUM_DEFAULT_CONTEXTS)
```

### Comparing `antelope_core-0.3.0/antelope_core/tests/test_exchanges.py` & `antelope_core-0.3.1/antelope_core/tests/test_exchanges.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core/tests/test_resources.py` & `antelope_core-0.3.1/antelope_core/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/antelope_core.egg-info/PKG-INFO` & `antelope_core-0.3.1/antelope_core.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 Metadata-Version: 2.1
-Name: antelope-core
-Version: 0.3.0
+Name: antelope_core
+Version: 0.3.1
 Home-page: https://github.com/AntelopeLCA/core
 Author: Brandon Kuczenski
 Author-email: bkuczenski@ucsb.edu
 License: BSD 3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: XML
-Provides-Extra: write_to_excel
 License-File: LICENSE
+Requires-Dist: synonym_dict>=0.2.4
+Requires-Dist: antelope_interface>=0.2.4
+Requires-Dist: xlstools>=0.1.3
+Requires-Dist: python-magic>=0.4.18
+Requires-Dist: requests>=2.25
+Requires-Dist: pydantic>=2.5.0
+Provides-Extra: xml
+Requires-Dist: lxml>=1.2.0; extra == "xml"
+Provides-Extra: write-to-excel
+Requires-Dist: xlsxwriter>=1.3.7; extra == "write-to-excel"
 
 ![](https://travis-ci.com/AntelopeLCA/core.svg?branch=master&status=passed) ![](https://coveralls.io/repos/github/AntelopeLCA/core/badge.svg?branch=master)
 
 # core
 Antelope Catalog - reference implementation.
 
 This repository provides code that enables access to different forms of life cycle
```

### Comparing `antelope_core-0.3.0/antelope_core.egg-info/SOURCES.txt` & `antelope_core-0.3.1/antelope_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `antelope_core-0.3.0/setup.py` & `antelope_core-0.3.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.3.0'
+VERSION = '0.3.1'
 
 requires = [
     "synonym_dict>=0.2.4",
-    "antelope_interface>=0.2.3",
+    "antelope_interface>=0.2.4",
     "xlstools>=0.1.3",
     "python-magic>=0.4.18",
     "requests>=2.25",
     "pydantic>=2.5.0"
 ]
 
 # optional: pylzma
 """
 Version History
 
+0.3.1   2024-04-18 - upate antelope-interface to 0.2.4
+
 0.3.0   2024-01-05 - 0.3-branch development version, supporting end-user access to vault.lc resources 
 
 # ^ 0.3.* 0.3-branch fork   
 # v 0.2.* main / master for legacy projects
 
+0.2.4   2024-04-17 - Remove antelope.ExteriorFlow in favor of antelope.models.ExteriorFlow
+
+0.2.3   2024-03-21 - compatibility release for antelope_interface upgrades and terminology changes
+                     OpenLCA v2 schema handled
+                     lots of cloud work 
+
 0.2.1   2023-04-10 - xdb passes benchmarks
                      pydantic models moved into interface
                      sys_lci and bg_lcia operational, both locally and remotely
 
 0.2.0   2023-04-07 - "release" virtualize branch. 
                    - Add pydantic models for everything
                    - add an XDB client implementation for remote operation
```

