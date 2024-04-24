# Comparing `tmp/filip-0.4.0.tar.gz` & `tmp/filip-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filip-0.4.0.tar", last modified: Tue Apr  9 16:33:38 2024, max compression
+gzip compressed data, was "filip-0.4.1.tar", last modified: Wed Apr 24 12:17:26 2024, max compression
```

## Comparing `filip-0.4.0.tar` & `filip-0.4.1.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 16:33:38.094662 filip-0.4.0/
--rw-rw-rw-   0 root         (0) root         (0)     1503 2023-02-07 11:46:33.000000 filip-0.4.0/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)    15059 2024-04-09 16:33:38.094662 filip-0.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    13308 2024-04-09 16:16:47.000000 filip-0.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 16:33:38.066662 filip-0.4.0/filip/
--rw-rw-rw-   0 root         (0) root         (0)      174 2024-04-09 16:16:47.000000 filip-0.4.0/filip/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 16:33:38.070662 filip-0.4.0/filip/clients/
--rw-rw-rw-   0 root         (0) root         (0)       46 2022-05-08 11:29:06.000000 filip-0.4.0/filip/clients/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11772 2024-04-09 14:07:38.000000 filip-0.4.0/filip/clients/base_http_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 16:33:38.070662 filip-0.4.0/filip/clients/mqtt/
--rw-rw-rw-   0 root         (0) root         (0)       96 2022-05-08 11:29:06.000000 filip-0.4.0/filip/clients/mqtt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    33015 2024-04-03 12:39:18.000000 filip-0.4.0/filip/clients/mqtt/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 16:33:38.070662 filip-0.4.0/filip/clients/mqtt/encoder/
--rw-rw-rw-   0 root         (0) root         (0)       94 2022-05-08 11:29:06.000000 filip-0.4.0/filip/clients/mqtt/encoder/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3198 2022-05-08 11:29:06.000000 filip-0.4.0/filip/clients/mqtt/encoder/base_encoder.py
--rw-rw-rw-   0 root         (0) root         (0)     1258 2022-05-08 11:29:06.000000 filip-0.4.0/filip/clients/mqtt/encoder/json.py
--rw-rw-rw-   0 root         (0) root         (0)     2148 2022-05-08 11:29:06.000000 filip-0.4.0/filip/clients/mqtt/encoder/ulralight.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 16:33:38.070662 filip-0.4.0/filip/clients/ngsi_ld/
--rw-rw-rw-   0 root         (0) root         (0)       72 2022-05-08 11:29:06.000000 filip-0.4.0/filip/clients/ngsi_ld/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 16:33:38.074662 filip-0.4.0/filip/clients/ngsi_v2/
--rw-rw-rw-   0 root         (0) root         (0)      203 2022-05-08 11:29:06.000000 filip-0.4.0/filip/clients/ngsi_v2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    86424 2024-04-09 16:16:47.000000 filip-0.4.0/filip/clients/ngsi_v2/cb.py
--rw-rw-rw-   0 root         (0) root         (0)     8321 2024-01-02 12:41:27.000000 filip-0.4.0/filip/clients/ngsi_v2/client.py
--rw-rw-rw-   0 root         (0) root         (0)    27515 2024-04-09 14:07:38.000000 filip-0.4.0/filip/clients/ngsi_v2/iota.py
--rw-rw-rw-   0 root         (0) root         (0)    49805 2024-04-09 16:16:47.000000 filip-0.4.0/filip/clients/ngsi_v2/quantumleap.py
--rw-rw-rw-   0 root         (0) root         (0)     1397 2024-01-02 12:41:27.000000 filip-0.4.0/filip/config.py
--rw-rw-rw-   0 root         (0) root         (0)      239 2024-01-02 12:41:27.000000 filip-0.4.0/filip/custom_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 16:33:38.062662 filip-0.4.0/filip/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 16:33:38.074662 filip-0.4.0/filip/data/unece-units/
--rw-rw-rw-   0 root         (0) root         (0)      464 2022-05-08 11:29:06.000000 filip-0.4.0/filip/data/unece-units/levels.csv
--rw-rw-rw-   0 root         (0) root         (0)   194959 2022-05-08 11:29:06.000000 filip-0.4.0/filip/data/unece-units/units_of_measure.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 16:33:38.078662 filip-0.4.0/filip/models/
--rw-rw-rw-   0 root         (0) root         (0)       30 2024-04-09 14:07:38.000000 filip-0.4.0/filip/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4559 2024-04-09 16:16:47.000000 filip-0.4.0/filip/models/base.py
--rw-rw-rw-   0 root         (0) root         (0)      437 2022-05-08 11:29:06.000000 filip-0.4.0/filip/models/mqtt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 16:33:38.078662 filip-0.4.0/filip/models/ngsi_ld/
--rw-rw-rw-   0 root         (0) root         (0)       63 2022-05-08 11:29:06.000000 filip-0.4.0/filip/models/ngsi_ld/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 16:33:38.082662 filip-0.4.0/filip/models/ngsi_v2/
--rw-rw-rw-   0 root         (0) root         (0)       62 2024-04-09 14:07:38.000000 filip-0.4.0/filip/models/ngsi_v2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18442 2024-04-09 16:16:47.000000 filip-0.4.0/filip/models/ngsi_v2/base.py
--rw-rw-rw-   0 root         (0) root         (0)    26010 2024-04-09 16:16:47.000000 filip-0.4.0/filip/models/ngsi_v2/context.py
--rw-rw-rw-   0 root         (0) root         (0)    24046 2024-04-09 16:16:47.000000 filip-0.4.0/filip/models/ngsi_v2/iot.py
--rw-rw-rw-   0 root         (0) root         (0)     6020 2024-04-09 14:07:38.000000 filip-0.4.0/filip/models/ngsi_v2/registrations.py
--rw-rw-rw-   0 root         (0) root         (0)    14721 2024-04-09 14:07:38.000000 filip-0.4.0/filip/models/ngsi_v2/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     5541 2024-01-02 12:41:27.000000 filip-0.4.0/filip/models/ngsi_v2/timeseries.py
--rw-rw-rw-   0 root         (0) root         (0)    11295 2024-02-02 14:29:51.000000 filip-0.4.0/filip/models/ngsi_v2/units.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 16:33:38.082662 filip-0.4.0/filip/semantics/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-05-08 11:29:06.000000 filip-0.4.0/filip/semantics/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 16:33:38.086662 filip-0.4.0/filip/semantics/ontology_parser/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-05-08 11:29:06.000000 filip-0.4.0/filip/semantics/ontology_parser/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    28335 2022-05-08 11:29:06.000000 filip-0.4.0/filip/semantics/ontology_parser/post_processer.py
--rw-rw-rw-   0 root         (0) root         (0)    35716 2022-05-08 11:29:06.000000 filip-0.4.0/filip/semantics/ontology_parser/rdfparser.py
--rw-rw-rw-   0 root         (0) root         (0)     9315 2022-05-08 11:29:06.000000 filip-0.4.0/filip/semantics/ontology_parser/vocabulary_builder.py
--rw-rw-rw-   0 root         (0) root         (0)    46106 2024-01-02 12:41:27.000000 filip-0.4.0/filip/semantics/semantics_manager.py
--rw-rw-rw-   0 root         (0) root         (0)    59987 2024-02-02 14:29:51.000000 filip-0.4.0/filip/semantics/semantics_models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 16:33:38.086662 filip-0.4.0/filip/semantics/vocabulary/
--rw-rw-rw-   0 root         (0) root         (0)      561 2022-05-08 11:29:06.000000 filip-0.4.0/filip/semantics/vocabulary/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6920 2022-05-08 11:29:06.000000 filip-0.4.0/filip/semantics/vocabulary/combined_relations.py
--rw-rw-rw-   0 root         (0) root         (0)    27900 2024-01-02 12:41:27.000000 filip-0.4.0/filip/semantics/vocabulary/entities.py
--rw-rw-rw-   0 root         (0) root         (0)    20101 2024-01-02 12:41:27.000000 filip-0.4.0/filip/semantics/vocabulary/relation.py
--rw-rw-rw-   0 root         (0) root         (0)     7662 2024-01-02 12:41:27.000000 filip-0.4.0/filip/semantics/vocabulary/source.py
--rw-rw-rw-   0 root         (0) root         (0)    19010 2022-05-08 11:29:06.000000 filip-0.4.0/filip/semantics/vocabulary/vocabulary.py
--rw-rw-rw-   0 root         (0) root         (0)    33798 2022-08-18 11:43:30.000000 filip-0.4.0/filip/semantics/vocabulary_configurator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 16:33:38.090662 filip-0.4.0/filip/utils/
--rw-rw-rw-   0 root         (0) root         (0)      209 2022-05-08 11:29:06.000000 filip-0.4.0/filip/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5703 2024-04-03 16:20:56.000000 filip-0.4.0/filip/utils/cleanup.py
--rw-rw-rw-   0 root         (0) root         (0)     2364 2022-05-08 11:29:06.000000 filip-0.4.0/filip/utils/data.py
--rw-rw-rw-   0 root         (0) root         (0)      607 2022-05-08 11:29:06.000000 filip-0.4.0/filip/utils/datetime.py
--rw-rw-rw-   0 root         (0) root         (0)     4960 2023-02-07 12:15:27.000000 filip-0.4.0/filip/utils/filter.py
--rw-rw-rw-   0 root         (0) root         (0)       44 2022-05-08 11:29:06.000000 filip-0.4.0/filip/utils/geo_ql.py
--rw-rw-rw-   0 root         (0) root         (0)     1312 2022-08-18 11:14:35.000000 filip-0.4.0/filip/utils/iot.py
--rw-rw-rw-   0 root         (0) root         (0)     5049 2024-01-02 12:41:27.000000 filip-0.4.0/filip/utils/model_generation.py
--rw-rw-rw-   0 root         (0) root         (0)    12495 2023-10-30 16:39:03.000000 filip-0.4.0/filip/utils/simple_ql.py
--rw-rw-rw-   0 root         (0) root         (0)     4859 2024-01-02 12:41:27.000000 filip-0.4.0/filip/utils/validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 16:33:38.090662 filip-0.4.0/filip.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15059 2024-04-09 16:33:38.000000 filip-0.4.0/filip.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2013 2024-04-09 16:33:38.000000 filip-0.4.0/filip.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 16:33:38.000000 filip-0.4.0/filip.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      349 2024-04-09 16:33:38.000000 filip-0.4.0/filip.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-09 16:33:38.000000 filip-0.4.0/filip.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       79 2024-04-09 16:33:38.094662 filip-0.4.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2939 2024-04-09 16:16:47.000000 filip-0.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 16:33:38.090662 filip-0.4.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1575 2024-01-02 12:41:27.000000 filip-0.4.0/tests/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)     3239 2022-05-08 11:29:06.000000 filip-0.4.0/tests/test_logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:17:26.679440 filip-0.4.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1503 2023-02-07 11:46:33.000000 filip-0.4.1/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)    15098 2024-04-24 12:17:26.679440 filip-0.4.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    13308 2024-04-23 10:23:31.000000 filip-0.4.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:17:26.663441 filip-0.4.1/filip/
+-rw-rw-rw-   0 root         (0) root         (0)      174 2024-04-24 11:49:31.000000 filip-0.4.1/filip/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:17:26.667441 filip-0.4.1/filip/clients/
+-rw-rw-rw-   0 root         (0) root         (0)       46 2022-05-08 11:29:06.000000 filip-0.4.1/filip/clients/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11772 2024-04-22 15:48:00.000000 filip-0.4.1/filip/clients/base_http_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:17:26.667441 filip-0.4.1/filip/clients/mqtt/
+-rw-rw-rw-   0 root         (0) root         (0)       96 2022-05-08 11:29:06.000000 filip-0.4.1/filip/clients/mqtt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    33014 2024-04-23 10:23:31.000000 filip-0.4.1/filip/clients/mqtt/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:17:26.667441 filip-0.4.1/filip/clients/mqtt/encoder/
+-rw-rw-rw-   0 root         (0) root         (0)       94 2022-05-08 11:29:06.000000 filip-0.4.1/filip/clients/mqtt/encoder/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3198 2022-05-08 11:29:06.000000 filip-0.4.1/filip/clients/mqtt/encoder/base_encoder.py
+-rw-rw-rw-   0 root         (0) root         (0)     1258 2022-05-08 11:29:06.000000 filip-0.4.1/filip/clients/mqtt/encoder/json.py
+-rw-rw-rw-   0 root         (0) root         (0)     2148 2022-05-08 11:29:06.000000 filip-0.4.1/filip/clients/mqtt/encoder/ulralight.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:17:26.667441 filip-0.4.1/filip/clients/ngsi_ld/
+-rw-rw-rw-   0 root         (0) root         (0)       72 2022-05-08 11:29:06.000000 filip-0.4.1/filip/clients/ngsi_ld/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:17:26.667441 filip-0.4.1/filip/clients/ngsi_v2/
+-rw-rw-rw-   0 root         (0) root         (0)      203 2022-05-08 11:29:06.000000 filip-0.4.1/filip/clients/ngsi_v2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    88177 2024-04-24 06:42:35.000000 filip-0.4.1/filip/clients/ngsi_v2/cb.py
+-rw-rw-rw-   0 root         (0) root         (0)     8321 2024-01-02 12:41:27.000000 filip-0.4.1/filip/clients/ngsi_v2/client.py
+-rw-rw-rw-   0 root         (0) root         (0)    27515 2024-04-22 15:48:00.000000 filip-0.4.1/filip/clients/ngsi_v2/iota.py
+-rw-rw-rw-   0 root         (0) root         (0)    49784 2024-04-23 10:23:31.000000 filip-0.4.1/filip/clients/ngsi_v2/quantumleap.py
+-rw-rw-rw-   0 root         (0) root         (0)     1397 2024-01-02 12:41:27.000000 filip-0.4.1/filip/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      239 2024-01-02 12:41:27.000000 filip-0.4.1/filip/custom_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:17:26.659440 filip-0.4.1/filip/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:17:26.667441 filip-0.4.1/filip/data/unece-units/
+-rw-rw-rw-   0 root         (0) root         (0)      464 2022-05-08 11:29:06.000000 filip-0.4.1/filip/data/unece-units/levels.csv
+-rw-rw-rw-   0 root         (0) root         (0)   194959 2022-05-08 11:29:06.000000 filip-0.4.1/filip/data/unece-units/units_of_measure.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:17:26.667441 filip-0.4.1/filip/models/
+-rw-rw-rw-   0 root         (0) root         (0)       30 2024-04-22 15:48:00.000000 filip-0.4.1/filip/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4560 2024-04-23 10:23:31.000000 filip-0.4.1/filip/models/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      437 2022-05-08 11:29:06.000000 filip-0.4.1/filip/models/mqtt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:17:26.667441 filip-0.4.1/filip/models/ngsi_ld/
+-rw-rw-rw-   0 root         (0) root         (0)       63 2022-05-08 11:29:06.000000 filip-0.4.1/filip/models/ngsi_ld/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:17:26.671440 filip-0.4.1/filip/models/ngsi_v2/
+-rw-rw-rw-   0 root         (0) root         (0)       62 2024-04-22 15:48:00.000000 filip-0.4.1/filip/models/ngsi_v2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18442 2024-04-22 15:48:00.000000 filip-0.4.1/filip/models/ngsi_v2/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    26277 2024-04-24 06:42:35.000000 filip-0.4.1/filip/models/ngsi_v2/context.py
+-rw-rw-rw-   0 root         (0) root         (0)    24046 2024-04-24 11:49:31.000000 filip-0.4.1/filip/models/ngsi_v2/iot.py
+-rw-rw-rw-   0 root         (0) root         (0)     6020 2024-04-22 15:48:00.000000 filip-0.4.1/filip/models/ngsi_v2/registrations.py
+-rw-rw-rw-   0 root         (0) root         (0)    14721 2024-04-22 15:48:00.000000 filip-0.4.1/filip/models/ngsi_v2/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5541 2024-01-02 12:41:27.000000 filip-0.4.1/filip/models/ngsi_v2/timeseries.py
+-rw-rw-rw-   0 root         (0) root         (0)    11295 2024-02-02 14:29:51.000000 filip-0.4.1/filip/models/ngsi_v2/units.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:17:26.671440 filip-0.4.1/filip/semantics/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-05-08 11:29:06.000000 filip-0.4.1/filip/semantics/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:17:26.671440 filip-0.4.1/filip/semantics/ontology_parser/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-05-08 11:29:06.000000 filip-0.4.1/filip/semantics/ontology_parser/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    28335 2022-05-08 11:29:06.000000 filip-0.4.1/filip/semantics/ontology_parser/post_processer.py
+-rw-rw-rw-   0 root         (0) root         (0)    35716 2022-05-08 11:29:06.000000 filip-0.4.1/filip/semantics/ontology_parser/rdfparser.py
+-rw-rw-rw-   0 root         (0) root         (0)     9315 2022-05-08 11:29:06.000000 filip-0.4.1/filip/semantics/ontology_parser/vocabulary_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)    46106 2024-01-02 12:41:27.000000 filip-0.4.1/filip/semantics/semantics_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)    59987 2024-02-02 14:29:51.000000 filip-0.4.1/filip/semantics/semantics_models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:17:26.675440 filip-0.4.1/filip/semantics/vocabulary/
+-rw-rw-rw-   0 root         (0) root         (0)      561 2022-05-08 11:29:06.000000 filip-0.4.1/filip/semantics/vocabulary/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6920 2022-05-08 11:29:06.000000 filip-0.4.1/filip/semantics/vocabulary/combined_relations.py
+-rw-rw-rw-   0 root         (0) root         (0)    27900 2024-01-02 12:41:27.000000 filip-0.4.1/filip/semantics/vocabulary/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)    20101 2024-01-02 12:41:27.000000 filip-0.4.1/filip/semantics/vocabulary/relation.py
+-rw-rw-rw-   0 root         (0) root         (0)     7662 2024-01-02 12:41:27.000000 filip-0.4.1/filip/semantics/vocabulary/source.py
+-rw-rw-rw-   0 root         (0) root         (0)    19010 2022-05-08 11:29:06.000000 filip-0.4.1/filip/semantics/vocabulary/vocabulary.py
+-rw-rw-rw-   0 root         (0) root         (0)    33798 2022-08-18 11:43:30.000000 filip-0.4.1/filip/semantics/vocabulary_configurator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:17:26.675440 filip-0.4.1/filip/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      209 2022-05-08 11:29:06.000000 filip-0.4.1/filip/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8643 2024-04-23 10:23:31.000000 filip-0.4.1/filip/utils/cleanup.py
+-rw-rw-rw-   0 root         (0) root         (0)     2364 2022-05-08 11:29:06.000000 filip-0.4.1/filip/utils/data.py
+-rw-rw-rw-   0 root         (0) root         (0)      607 2022-05-08 11:29:06.000000 filip-0.4.1/filip/utils/datetime.py
+-rw-rw-rw-   0 root         (0) root         (0)     4960 2023-02-07 12:15:27.000000 filip-0.4.1/filip/utils/filter.py
+-rw-rw-rw-   0 root         (0) root         (0)       44 2022-05-08 11:29:06.000000 filip-0.4.1/filip/utils/geo_ql.py
+-rw-rw-rw-   0 root         (0) root         (0)     1312 2022-08-18 11:14:35.000000 filip-0.4.1/filip/utils/iot.py
+-rw-rw-rw-   0 root         (0) root         (0)     5049 2024-01-02 12:41:27.000000 filip-0.4.1/filip/utils/model_generation.py
+-rw-rw-rw-   0 root         (0) root         (0)    12495 2023-10-30 16:39:03.000000 filip-0.4.1/filip/utils/simple_ql.py
+-rw-rw-rw-   0 root         (0) root         (0)     4859 2024-04-24 06:42:35.000000 filip-0.4.1/filip/utils/validators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:17:26.675440 filip-0.4.1/filip.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15098 2024-04-24 12:17:26.000000 filip-0.4.1/filip.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2013 2024-04-24 12:17:26.000000 filip-0.4.1/filip.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 12:17:26.000000 filip-0.4.1/filip.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      373 2024-04-24 12:17:26.000000 filip-0.4.1/filip.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-24 12:17:26.000000 filip-0.4.1/filip.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       79 2024-04-24 12:17:26.679440 filip-0.4.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2986 2024-04-24 11:49:31.000000 filip-0.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:17:26.675440 filip-0.4.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1575 2024-01-02 12:41:27.000000 filip-0.4.1/tests/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3239 2022-05-08 11:29:06.000000 filip-0.4.1/tests/test_logging.py
```

### Comparing `filip-0.4.0/LICENSE.md` & `filip-0.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `filip-0.4.0/PKG-INFO` & `filip-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: filip
-Version: 0.4.0
+Version: 0.4.1
 Summary: [FI]WARE [Li]brary for [P]ython
 Home-page: https://github.com/RWTH-EBC/filip
-Download-URL: https://github.com/RWTH-EBC/FiLiP/archive/refs/tags/v0.4.0.tar.gz
+Download-URL: https://github.com/RWTH-EBC/FiLiP/archive/refs/tags/v0.4.1.tar.gz
 Author: RWTH Aachen University, E.ON Energy Research Center, Institute        of Energy Efficient Buildings and Indoor Climate
 Author-email: tstorek@eonerc.rwth-aachen.de
 Project-URL: Documentation, https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/FiLiP/master/docs/index.html
 Project-URL: Source, https://github.com/RWTH-EBC/filip
-Project-URL: Download, https://github.com/RWTH-EBC/FiLiP/archive/refs/tags/v0.4.0.tar.gz
+Project-URL: Download, https://github.com/RWTH-EBC/FiLiP/archive/refs/tags/v0.4.1.tar.gz
 Keywords: iot,fiware,semantic
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -28,14 +28,15 @@
 Requires-Dist: pydantic~=2.5.2
 Requires-Dist: pydantic-settings~=2.0.0
 Requires-Dist: stringcase>=1.2.0
 Requires-Dist: rdflib~=6.0.0
 Requires-Dist: regex~=2023.10.3
 Requires-Dist: requests~=2.31.0
 Requires-Dist: rapidfuzz~=3.4.0
+Requires-Dist: geojson-pydantic~=1.0.2
 Requires-Dist: wget~=3.2
 Provides-Extra: semantics
 Requires-Dist: igraph~=0.11.2; extra == "semantics"
 Requires-Dist: pandas~=1.3.5; python_version < "3.9"
 Requires-Dist: pandas~=2.1.4; python_version >= "3.9"
 
 ![E.ON EBC RWTH Aachen University](https://raw.githubusercontent.com/RWTH-EBC/FiLiP/master/docs/logos/EBC_Logo.png)
```

### Comparing `filip-0.4.0/README.md` & `filip-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `filip-0.4.0/filip/clients/base_http_client.py` & `filip-0.4.1/filip/clients/base_http_client.py`

 * *Files identical despite different names*

### Comparing `filip-0.4.0/filip/clients/mqtt/client.py` & `filip-0.4.1/filip/clients/mqtt/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 topic subscription for FIWARE's IoT communication pattern.
 """
 import itertools
 import logging
 import warnings
 from datetime import datetime
 from typing import Any, Callable, Dict, List, Tuple, Union
-
 import paho.mqtt.client as mqtt
 
 from filip.clients.mqtt.encoder import BaseEncoder, Json, Ultralight
 from filip.models.mqtt import IoTAMQTTMessageType
 from filip.models.ngsi_v2.iot import \
     Device, \
     PayloadProtocol, \
```

### Comparing `filip-0.4.0/filip/clients/mqtt/encoder/base_encoder.py` & `filip-0.4.1/filip/clients/mqtt/encoder/base_encoder.py`

 * *Files identical despite different names*

### Comparing `filip-0.4.0/filip/clients/mqtt/encoder/json.py` & `filip-0.4.1/filip/clients/mqtt/encoder/json.py`

 * *Files identical despite different names*

### Comparing `filip-0.4.0/filip/clients/mqtt/encoder/ulralight.py` & `filip-0.4.1/filip/clients/mqtt/encoder/ulralight.py`

 * *Files identical despite different names*

### Comparing `filip-0.4.0/filip/clients/ngsi_v2/cb.py` & `filip-0.4.1/filip/clients/ngsi_v2/cb.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,64 +193,82 @@
             self.logger.error(err)
             raise
 
     # CONTEXT MANAGEMENT API ENDPOINTS
     # Entity Operations
     def post_entity(
         self,
-        entity: ContextEntity,
+        entity: Union[ContextEntity, ContextEntityKeyValues],
         update: bool = False,
         patch: bool = False,
         override_attr_metadata: bool = True,
+        key_values: bool = False,
     ):
         """
         Function registers an Object with the NGSI Context Broker,
         if it already exists it can be automatically updated (overwritten)
         if the update bool is True.
         First a post request with the entity is tried, if the response code
         is 422 the entity is uncrossable, as it already exists there are two
         options, either overwrite it, if the attribute have changed
         (e.g. at least one new/new values) (update = True) or leave
         it the way it is (update=False)
         If you only want to manipulate the entities values, you need to set
         patch argument.
 
         Args:
-            entity (ContextEntity):
+            entity (ContextEntity/ContextEntityKeyValues):
                 Context Entity Object
             update (bool):
                 If the response.status_code is 422, whether the override and
                 existing entity
             patch (bool):
                 If the response.status_code is 422, whether to manipulate the
                 existing entity. Omitted if update `True`.
             override_attr_metadata:
                 Only applies for patch equal to `True`.
                 Whether to override or append the attribute's metadata.
                 `True` for overwrite or `False` for update/append
-
+            key_values(bool):
+                By default False. If set to True, "options=keyValues" will
+                be included in params of  post request. The payload uses
+                the keyValues simplified entity representation, i.e.
+                ContextEntityKeyValues.
         """
         url = urljoin(self.base_url, "v2/entities")
         headers = self.headers.copy()
+        params = {}
+        options = []
+        if key_values:
+            assert isinstance(entity, ContextEntityKeyValues)
+            options.append("keyValues")
+        else:
+            assert isinstance(entity, ContextEntity)
+        if options:
+            params.update({'options': ",".join(options)})
         try:
             res = self.post(
-                url=url, headers=headers, json=entity.model_dump(exclude_none=True)
+                url=url, headers=headers, json=entity.model_dump(exclude_none=True),
+                params=params,
             )
             if res.ok:
                 self.logger.info("Entity successfully posted!")
                 return res.headers.get("Location")
             res.raise_for_status()
         except requests.RequestException as err:
             if update and err.response.status_code == 422:
                 return self.override_entity(
-                    entity=entity)
+                    entity=entity, key_values=key_values)
             if patch and err.response.status_code == 422:
-                return self.patch_entity(
-                    entity=entity, override_attr_metadata=override_attr_metadata
-                )
+                if not key_values:
+                    return self.patch_entity(
+                        entity=entity, override_attr_metadata=override_attr_metadata
+                    )
+                else:
+                    return self.update_entity_key_values(entity=entity)
             msg = f"Could not post entity {entity.id}"
             self.log_error(err=err, msg=msg)
             raise
 
     def get_entity_list(
         self,
         *,
@@ -736,20 +754,20 @@
             else:
                 res.raise_for_status()
         except requests.RequestException as err:
             msg = f"Could not update or append attributes of entity" f" {entity.id} !"
             self.log_error(err=err, msg=msg)
             raise
 
-    def update_entity_key_value(self,
-                                entity: Union[ContextEntityKeyValues, dict],):
+    def update_entity_key_values(self,
+                                 entity: Union[ContextEntityKeyValues, dict],):
         """
         The entity are updated with a ContextEntityKeyValues object or a
         dictionary contain the simplified entity data. This corresponds to a
-        'PATcH' request.
+        'PATCH' request.
         Only existing attribute can be updated!
 
         Args:
             entity: A ContextEntityKeyValues object or a dictionary contain
             the simplified entity data
 
         """
@@ -773,19 +791,19 @@
                 res.raise_for_status()
         except requests.RequestException as err:
             msg = f"Could not update attributes of entity" \
                   f" {entity.id} !"
             self.log_error(err=err, msg=msg)
             raise
 
-    def update_entity_attributes_key_value(self,
-                                           entity_id: str,
-                                           attrs: dict,
-                                           entity_type: str = None,
-                                           ):
+    def update_entity_attributes_key_values(self,
+                                            entity_id: str,
+                                            attrs: dict,
+                                            entity_type: str = None,
+                                            ):
         """
         Update entity with attributes in keyValues form.
         This corresponds to a 'PATcH' request.
         Only existing attribute can be updated!
 
         Args:
             entity_id: Entity id to be updated
@@ -808,15 +826,15 @@
 
         entity_dict = attrs.copy()
         entity_dict.update({
             "id": entity_id,
             "type": entity_type
         })
         entity = ContextEntityKeyValues(**entity_dict)
-        self.update_entity_key_value(entity=entity)
+        self.update_entity_key_values(entity=entity)
 
     def update_existing_entity_attributes(
             self,
             entity_id: str,
             entity_type: str,
             attrs: List[Union[NamedContextAttribute,
                               Dict[str, ContextAttribute]]],
@@ -875,86 +893,103 @@
             else:
                 res.raise_for_status()
         except requests.RequestException as err:
             msg = f"Could not update attributes of entity" f" {entity.id} !"
             self.log_error(err=err, msg=msg)
             raise
 
-    def override_entity(self, entity: ContextEntity):
+    def override_entity(self,
+                        entity: Union[ContextEntity, ContextEntityKeyValues],
+                        **kwargs
+                        ):
         """
         The request payload is an object representing the attributes to
         override the existing entity.
 
         Note:
             If you want to manipulate you should rather use patch_entity.
 
         Args:
-            entity (ContextEntity):
+            entity (ContextEntity or ContextEntityKeyValues):
         Returns:
             None
         """
-        self.replace_entity_attributes(entity_id=entity.id,
-                                       entity_type=entity.type,
-                                       attrs=entity.get_properties())
+        return self.replace_entity_attributes(entity_id=entity.id,
+                                              entity_type=entity.type,
+                                              attrs=entity.get_attributes(),
+                                              **kwargs
+                                              )
 
     def replace_entity_attributes(
             self,
             entity_id: str,
             entity_type: str,
-            attrs: List[Union[NamedContextAttribute,
+            attrs: Union[List[Union[NamedContextAttribute,
                               Dict[str, ContextAttribute]]],
-            forcedUpdate: bool = False
+                         Dict],
+            forcedUpdate: bool = False,
+            key_values: bool = False,
     ):
         """
         The attributes previously existing in the entity are removed and
         replaced by the ones in the request. This corresponds to a 'PUT'
         request.
 
         Args:
             entity_id: Entity id to be updated
             entity_type: Entity type, to avoid ambiguity in case there are
                 several entities with the same entity id.
-            attrs: List of attributes to add to the entity
+            attrs: List of attributes to add to the entity or dict of
+                attributes in case of key_values=True.
             forcedUpdate: Update operation have to trigger any matching
                 subscription, no matter if there is an actual attribute
                 update or no instead of the default behavior, which is to
                 updated only if attribute is effectively updated.
+            key_values(bool):
+                By default False. If set to True, "options=keyValues" will
+                be included in params of the request. The payload uses
+                the keyValues simplified entity representation, i.e.
+                ContextEntityKeyValues.
         Returns:
             None
         """
         url = urljoin(self.base_url, f"v2/entities/{entity_id}/attrs")
         headers = self.headers.copy()
         params = {}
         options = []
         if forcedUpdate:
             options.append("forcedUpdate")
+        if key_values:
+            options.append("keyValues")
+            assert isinstance(attrs, dict)
+        else:
+            entity = ContextEntity(id=entity_id, type=entity_type)
+            entity.add_attributes(attrs)
+            attrs = entity.model_dump(
+                    exclude={"id", "type"},
+                    exclude_none=True
+                )
         if options:
             params.update({'options': ",".join(options)})
         if entity_type:
             params.update({"type": entity_type})
 
-        entity = ContextEntity(id=entity_id, type=entity_type)
-        entity.add_attributes(attrs)
-
         try:
             res = self.put(
                 url=url,
                 headers=headers,
-                json=entity.model_dump(
-                    exclude={"id", "type"},
-                    exclude_none=True
-                ),
+                json=attrs,
                 params=params,
             )
             if res.ok:
-                self.logger.info("Entity '%s' successfully " "updated!", entity.id)
+                self.logger.info("Entity '%s' successfully " "updated!", entity_id)
             else:
                 res.raise_for_status()
         except requests.RequestException as err:
-            msg = f"Could not replace attribute of entity {entity.id} !"
+            msg = f"Could not replace attribute of entity {entity_id} !"
             self.log_error(err=err, msg=msg)
             raise
 
     # Attribute operations
     def get_attribute(
         self,
         entity_id: str,
@@ -1615,15 +1650,15 @@
             msg = f"Could not delete registration {registration_id} !"
             self.log_error(err=err, msg=msg)
             raise
 
     # Batch operation API
     def update(self,
                *,
-               entities: List[ContextEntity],
+               entities: List[Union[ContextEntity, ContextEntityKeyValues]],
                action_type: Union[ActionType, str],
                update_format: str = None,
                forcedUpdate: bool = False,
                override_metadata: bool = False,
                ) -> None:
         """
         This operation allows to create, update and/or delete several entities
@@ -1672,21 +1707,21 @@
         headers.update({"Content-Type": "application/json"})
         params = {}
         options = []
         if override_metadata:
             options.append("overrideMetadata")
         if forcedUpdate:
             options.append("forcedUpdate")
-        if options:
-            params.update({'options': ",".join(options)})
         if update_format:
             assert (
                 update_format == "keyValues"
             ), "Only 'keyValues' is allowed as update format"
-            params.update({"options": "keyValues"})
+            options.append("keyValues")
+        if options:
+            params.update({'options': ",".join(options)})
         update = Update(actionType=action_type, entities=entities)
         try:
             res = self.post(
                 url=url,
                 headers=headers,
                 params=params,
                 json=update.model_dump(by_alias=True),
```

### Comparing `filip-0.4.0/filip/clients/ngsi_v2/client.py` & `filip-0.4.1/filip/clients/ngsi_v2/client.py`

 * *Files identical despite different names*

### Comparing `filip-0.4.0/filip/clients/ngsi_v2/iota.py` & `filip-0.4.1/filip/clients/ngsi_v2/iota.py`

 * *Files identical despite different names*

### Comparing `filip-0.4.0/filip/clients/ngsi_v2/quantumleap.py` & `filip-0.4.1/filip/clients/ngsi_v2/quantumleap.py`

 * *Files 3% similar despite different names*

```diff
@@ -180,56 +180,17 @@
                 history.
             throttling (int): Minimal period of time in seconds which must
                 elapse between two consecutive notifications.
             time_index_attribute (String): The name of a custom attribute to be
                 used as a
             time index.
         """
-        headers = self.headers.copy()
-        params = {}
-        url = urljoin(self.base_url, 'v2/subscribe')
-        validate_http_url(cb_url)
-        cb_url = urljoin(str(cb_url), 'v2')
-        params.update({'orionUrl': cb_url.encode('utf-8')})
-
-        validate_http_url(ql_url)
-        ql_url = urljoin(str(ql_url), 'v2')
-        params.update({'quantumleapUrl': ql_url.encode('utf-8')})
-
-        if entity_type:
-            params.update({'entityType': entity_type})
-        if entity_id:
-            params.update({'entityId': entity_id})
-        if id_pattern:
-            params.update({'idPattern': id_pattern})
-        if attributes:
-            params.update({'attributes': attributes})
-        if observed_attributes:
-            params.update({'observedAttributes': observed_attributes})
-        if notified_attributes:
-            params.update({'notifiedAttributes': notified_attributes})
-        if throttling or throttling == 0:
-            if throttling >= 0 and type(throttling) == int:
-                params.update({'throttling': throttling})
-            else:
-                raise TypeError("Throttling must be a positive integer or zero")
-        if time_index_attribute:
-            params.update({'timeIndexAttribute': time_index_attribute})
-
-        try:
-            res = self.post(url=url, headers=headers, params=params)
-            if res.ok:
-                msg = "Subscription created successfully!"
-                self.logger.info(msg)
-
-            res.raise_for_status()
-        except requests.exceptions.RequestException as err:
-            msg = "Could not create subscription."
-            self.log_error(err=err, msg=msg)
-            raise
+        raise DeprecationWarning("Subscription endpoint of Quantumleap API is "
+                                 "deprecated, use the ORION subscription endpoint "
+                                 "instead")
 
     def delete_entity(self, entity_id: str,
                       entity_type: Optional[str] = None) -> str:
         """
         Given an entity (with type and id), delete all its historical records.
 
         Args:
@@ -298,14 +259,15 @@
             raise
 
     # QUERY API ENDPOINTS
     def __query_builder(self,
                         url,
                         *,
                         entity_id: str = None,
+                        id_pattern: str = None,
                         options: str = None,
                         entity_type: str = None,
                         aggr_method: Union[str, AggrMethod] = None,
                         aggr_period: Union[str, AggrPeriod] = None,
                         from_date: str = None,
                         to_date: str = None,
                         last_n: int = None,
@@ -340,18 +302,23 @@
                 response will return the last 9 values. Make sure you don't
                 give more offset than the number of results.
             georel:
             geometry:
             coords:
             attrs:
             aggr_scope:
+            id_pattern (str): The pattern covering the entity ids for which
+                to subscribe. The pattern follow regular expressions (POSIX
+                Extendede) e.g. ".*", "Room.*". Detail information:
+                https://en.wikibooks.org/wiki/Regular_Expressions/POSIX-Extended_Regular_Expressions
 
         Returns:
             Dict
         """
+        assert (id_pattern is None or entity_id is None), "Cannot have both id and idPattern as parameter."
         params = {}
         headers = self.headers.copy()
         max_records_per_request = 10000
         # create a double ending queue
         res_q: Deque[Dict] = deque([])
 
         if options:
@@ -383,14 +350,16 @@
         if attrs:
             params.update({'attrs': attrs})
         if aggr_scope:
             aggr_scope = AggrScope(aggr_scope)
             params.update({'aggr_scope': aggr_scope.value})
         if entity_id:
             params.update({'id': entity_id})
+        if id_pattern:
+            params.update({'idPattern': id_pattern})
 
         # This loop will chop large requests into smaller junks.
         # The individual functions will then merge the final response models
         for i in count(0, max_records_per_request):
             try:
                 params['offset'] = offset + i
 
@@ -427,14 +396,15 @@
 
         self.logger.info("Successfully retrieved entity data")
         return res_q
 
     # v2/entities
     def get_entities(self, *,
                      entity_type: str = None,
+                     id_pattern: str = None,
                      from_date: str = None,
                      to_date: str = None,
                      limit: int = 10000,
                      offset: int = None
                      ) -> List[TimeSeriesHeader]:
         """
         Get list of all available entities and their context information
@@ -442,14 +412,18 @@
 
         Args:
             entity_type (str): Comma-separated list of entity types whose data
                 are to be included in the response. Use only one (no comma)
                 when required. If used to resolve ambiguity for the given
                 entityId, make sure the given entityId exists for this
                 entityType.
+            id_pattern (str): The pattern covering the entity ids for which
+                to subscribe. The pattern follow regular expressions (POSIX
+                Extendede) e.g. ".*", "Room.*". Detail information:
+                https://en.wikibooks.org/wiki/Regular_Expressions/POSIX-Extended_Regular_Expressions
             from_date (str): The starting date and time (inclusive) from which
                 the context information is queried. Must be in ISO8601 format
                 (e.g., 2018-01-05T15:44:34)
             to_date (str): The final date and time (inclusive) from which the
                 context information is queried. Must be in ISO8601 format
                 (e.g., 2018-01-05T15:44:34).
             limit (int): Maximum number of results to be retrieved.
@@ -457,19 +431,21 @@
             offset (int): Offset for the results.
 
         Returns:
             List of TimeSeriesHeader
         """
         url = urljoin(self.base_url, 'v2/entities')
         res = self.__query_builder(url=url,
+                                   id_pattern=id_pattern,
                                    entity_type=entity_type,
                                    from_date=from_date,
                                    to_date=to_date,
                                    limit=limit,
                                    offset=offset)
+        
         ta = TypeAdapter(List[TimeSeriesHeader])
         return ta.validate_python(res[0])
 
     # /entities/{entityId}
     def get_entity_by_id(self,
                          entity_id: str,
                          *,
@@ -817,14 +793,15 @@
 
     # /types/{entityType}
     def get_entity_by_type(self,
                            entity_type: str,
                            *,
                            attrs: str = None,
                            entity_id: str = None,
+                           id_pattern: str = None,
                            aggr_method: Union[str, AggrMethod] = None,
                            aggr_period: Union[str, AggrPeriod] = None,
                            from_date: str = None,
                            to_date: str = None,
                            last_n: int = None,
                            limit: int = 10000,
                            offset: int = None,
@@ -838,14 +815,15 @@
         History of N attributes of N entities of the same type.
         For example, query the average pressure, temperature and humidity of
         this month in all the weather stations.
         """
         url = urljoin(self.base_url, f'v2/types/{entity_type}')
         res_q = self.__query_builder(url=url,
                                      entity_id=entity_id,
+                                     id_pattern=id_pattern,
                                      attrs=attrs,
                                      options=options,
                                      aggr_method=aggr_method,
                                      aggr_period=aggr_period,
                                      from_date=from_date,
                                      to_date=to_date,
                                      last_n=last_n,
@@ -870,14 +848,15 @@
 
     # /types/{entityType}/value
     def get_entity_values_by_type(self,
                                   entity_type: str,
                                   *,
                                   attrs: str = None,
                                   entity_id: str = None,
+                                  id_pattern: str = None,
                                   aggr_method: Union[str, AggrMethod] = None,
                                   aggr_period: Union[str, AggrPeriod] = None,
                                   from_date: str = None,
                                   to_date: str = None,
                                   last_n: int = None,
                                   limit: int = 10000,
                                   offset: int = None,
@@ -892,14 +871,15 @@
         For example, query the average pressure, temperature and humidity (
         values only, no metadata) of this month in
         all the weather stations.
         """
         url = urljoin(self.base_url, f'v2/types/{entity_type}/value')
         res_q = self.__query_builder(url=url,
                                      entity_id=entity_id,
+                                     id_pattern=id_pattern,
                                      attrs=attrs,
                                      options=options,
                                      entity_type=entity_type,
                                      aggr_method=aggr_method,
                                      aggr_period=aggr_period,
                                      from_date=from_date,
                                      to_date=to_date,
@@ -924,14 +904,15 @@
 
     # /types/{entityType}/attrs/{attrName}
     def get_entity_attr_by_type(self,
                                 entity_type: str,
                                 attr_name: str,
                                 *,
                                 entity_id: str = None,
+                                id_pattern: str = None,
                                 aggr_method: Union[str, AggrMethod] = None,
                                 aggr_period: Union[str, AggrPeriod] = None,
                                 from_date: str = None,
                                 to_date: str = None,
                                 last_n: int = None,
                                 limit: int = 10000,
                                 offset: int = None,
@@ -980,14 +961,15 @@
         Returns:
             Response Model
         """
         url = urljoin(self.base_url, f'v2/types/{entity_type}/attrs'
                                      f'/{attr_name}')
         res_q = self.__query_builder(url=url,
                                      entity_id=entity_id,
+                                     id_pattern=id_pattern,
                                      options=options,
                                      entity_type=entity_type,
                                      aggr_method=aggr_method,
                                      aggr_period=aggr_period,
                                      from_date=from_date,
                                      to_date=to_date,
                                      last_n=last_n,
@@ -1025,14 +1007,15 @@
 
     # /types/{entityType}/attrs/{attrName}/value
     def get_entity_attr_values_by_type(self,
                                        entity_type: str,
                                        attr_name: str,
                                        *,
                                        entity_id: str = None,
+                                       id_pattern: str = None,
                                        aggr_method: Union[
                                            str, AggrMethod] = None,
                                        aggr_period: Union[
                                            str, AggrPeriod] = None,
                                        from_date: str = None,
                                        to_date: str = None,
                                        last_n: int = None,
@@ -1075,14 +1058,15 @@
         Returns:
             Response Model
         """
         url = urljoin(self.base_url, f'v2/types/{entity_type}/attrs/'
                                      f'{attr_name}/value')
         res_q = self.__query_builder(url=url,
                                      entity_id=entity_id,
+                                     id_pattern=id_pattern,
                                      options=options,
                                      entity_type=entity_type,
                                      aggr_method=aggr_method,
                                      aggr_period=aggr_period,
                                      from_date=from_date,
                                      to_date=to_date,
                                      last_n=last_n,
```

### Comparing `filip-0.4.0/filip/config.py` & `filip-0.4.1/filip/config.py`

 * *Files identical despite different names*

### Comparing `filip-0.4.0/filip/data/unece-units/units_of_measure.csv` & `filip-0.4.1/filip/data/unece-units/units_of_measure.csv`

 * *Files identical despite different names*

### Comparing `filip-0.4.0/filip/models/base.py` & `filip-0.4.1/filip/models/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         default="",
         max_length=50,
         description="Fiware service used for multi-tenancy",
         pattern=r"\w*$",
     )
     service_path: str = Field(
         alias="fiware-servicepath",
-        default="",
+        default="/",
         description="Fiware service path",
         max_length=51,
     )
     valid_service = field_validator("service")(validate_fiware_service)
     valid_service_path = field_validator("service_path")(validate_fiware_service_path)
```

### Comparing `filip-0.4.0/filip/models/ngsi_v2/base.py` & `filip-0.4.1/filip/models/ngsi_v2/base.py`

 * *Files identical despite different names*

### Comparing `filip-0.4.0/filip/models/ngsi_v2/context.py` & `filip-0.4.1/filip/models/ngsi_v2/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,24 @@
     UNIQUE = (
         "unique",
         "unique mode. This mode is just like values mode, "
         "except that values are not repeated",
     )
 
 
+class PropertyFormat(str, Enum):
+    """
+    Format to decide if properties of ContextEntity class are returned as
+    List of NamedContextAttributes or as Dict of ContextAttributes.
+    """
+
+    LIST = "list"
+    DICT = "dict"
+
+
 class ContextAttribute(BaseAttribute, BaseValueAttribute):
     """
     Model for an attribute is represented by a JSON object with the following
     syntax:
 
     The attribute value is specified by the value property, whose value may
     be any JSON datatype.
@@ -169,23 +179,23 @@
             else:
                 # if this statement is reached not proper default-value for
                 # `type` was found and pydantic will raise the correct error
                 super().__init__(id=id, **data)
         # This will result in usual behavior
         super().__init__(id=id, type=type, **data)
 
+    def get_attributes(self) -> dict:
+        """
+        Get the attribute of the entity with the given name in
+        dict format
 
-class PropertyFormat(str, Enum):
-    """
-    Format to decide if properties of ContextEntity class are returned as
-    List of NamedContextAttributes or as Dict of ContextAttributes.
-    """
-
-    LIST = "list"
-    DICT = "dict"
+        Returns:
+            dict
+        """
+        return self.model_dump(exclude={"id", "type"})
 
 
 class ContextEntity(ContextEntityKeyValues):
     """
     Context entities, or simply entities, are the center of gravity in the
     FIWARE NGSI information model. An entity represents a thing, i.e., any
     physical or logical object (e.g., a sensor, a person, a room, an issue in
@@ -669,15 +679,15 @@
     """
 
     action_type: Union[ActionType, str] = Field(
         alias="actionType",
         description="actionType, to specify the kind of update action to do: "
         "either append, appendStrict, update, delete, or replace. ",
     )
-    entities: List[ContextEntity] = Field(
+    entities: List[Union[ContextEntity, ContextEntityKeyValues]] = Field(
         description="an array of entities, each entity specified using the "
         "JSON entity representation format "
     )
 
     @field_validator("action_type")
     @classmethod
     def check_action_type(cls, action):
```

### Comparing `filip-0.4.0/filip/models/ngsi_v2/iot.py` & `filip-0.4.1/filip/models/ngsi_v2/iot.py`

 * *Files identical despite different names*

### Comparing `filip-0.4.0/filip/models/ngsi_v2/registrations.py` & `filip-0.4.1/filip/models/ngsi_v2/registrations.py`

 * *Files identical despite different names*

### Comparing `filip-0.4.0/filip/models/ngsi_v2/subscriptions.py` & `filip-0.4.1/filip/models/ngsi_v2/subscriptions.py`

 * *Files identical despite different names*

### Comparing `filip-0.4.0/filip/models/ngsi_v2/timeseries.py` & `filip-0.4.1/filip/models/ngsi_v2/timeseries.py`

 * *Files identical despite different names*

### Comparing `filip-0.4.0/filip/models/ngsi_v2/units.py` & `filip-0.4.1/filip/models/ngsi_v2/units.py`

 * *Files identical despite different names*

### Comparing `filip-0.4.0/filip/semantics/ontology_parser/post_processer.py` & `filip-0.4.1/filip/semantics/ontology_parser/post_processer.py`

 * *Files identical despite different names*

### Comparing `filip-0.4.0/filip/semantics/ontology_parser/rdfparser.py` & `filip-0.4.1/filip/semantics/ontology_parser/rdfparser.py`

 * *Files identical despite different names*

### Comparing `filip-0.4.0/filip/semantics/ontology_parser/vocabulary_builder.py` & `filip-0.4.1/filip/semantics/ontology_parser/vocabulary_builder.py`

 * *Files identical despite different names*

### Comparing `filip-0.4.0/filip/semantics/semantics_manager.py` & `filip-0.4.1/filip/semantics/semantics_manager.py`

 * *Files identical despite different names*

### Comparing `filip-0.4.0/filip/semantics/semantics_models.py` & `filip-0.4.1/filip/semantics/semantics_models.py`

 * *Files identical despite different names*

### Comparing `filip-0.4.0/filip/semantics/vocabulary/__init__.py` & `filip-0.4.1/filip/semantics/vocabulary/__init__.py`

 * *Files identical despite different names*

### Comparing `filip-0.4.0/filip/semantics/vocabulary/combined_relations.py` & `filip-0.4.1/filip/semantics/vocabulary/combined_relations.py`

 * *Files identical despite different names*

### Comparing `filip-0.4.0/filip/semantics/vocabulary/entities.py` & `filip-0.4.1/filip/semantics/vocabulary/entities.py`

 * *Files identical despite different names*

### Comparing `filip-0.4.0/filip/semantics/vocabulary/relation.py` & `filip-0.4.1/filip/semantics/vocabulary/relation.py`

 * *Files identical despite different names*

### Comparing `filip-0.4.0/filip/semantics/vocabulary/source.py` & `filip-0.4.1/filip/semantics/vocabulary/source.py`

 * *Files identical despite different names*

### Comparing `filip-0.4.0/filip/semantics/vocabulary/vocabulary.py` & `filip-0.4.1/filip/semantics/vocabulary/vocabulary.py`

 * *Files identical despite different names*

### Comparing `filip-0.4.0/filip/semantics/vocabulary_configurator.py` & `filip-0.4.1/filip/semantics/vocabulary_configurator.py`

 * *Files identical despite different names*

### Comparing `filip-0.4.0/filip/utils/data.py` & `filip-0.4.1/filip/utils/data.py`

 * *Files identical despite different names*

### Comparing `filip-0.4.0/filip/utils/datetime.py` & `filip-0.4.1/filip/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `filip-0.4.0/filip/utils/filter.py` & `filip-0.4.1/filip/utils/filter.py`

 * *Files identical despite different names*

### Comparing `filip-0.4.0/filip/utils/iot.py` & `filip-0.4.1/filip/utils/iot.py`

 * *Files identical despite different names*

### Comparing `filip-0.4.0/filip/utils/model_generation.py` & `filip-0.4.1/filip/utils/model_generation.py`

 * *Files identical despite different names*

### Comparing `filip-0.4.0/filip/utils/simple_ql.py` & `filip-0.4.1/filip/utils/simple_ql.py`

 * *Files identical despite different names*

### Comparing `filip-0.4.0/filip/utils/validators.py` & `filip-0.4.1/filip/utils/validators.py`

 * *Files identical despite different names*

### Comparing `filip-0.4.0/filip.egg-info/PKG-INFO` & `filip-0.4.1/filip.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: filip
-Version: 0.4.0
+Version: 0.4.1
 Summary: [FI]WARE [Li]brary for [P]ython
 Home-page: https://github.com/RWTH-EBC/filip
-Download-URL: https://github.com/RWTH-EBC/FiLiP/archive/refs/tags/v0.4.0.tar.gz
+Download-URL: https://github.com/RWTH-EBC/FiLiP/archive/refs/tags/v0.4.1.tar.gz
 Author: RWTH Aachen University, E.ON Energy Research Center, Institute        of Energy Efficient Buildings and Indoor Climate
 Author-email: tstorek@eonerc.rwth-aachen.de
 Project-URL: Documentation, https://ebc.pages.rwth-aachen.de/EBC_all/github_ci/FiLiP/master/docs/index.html
 Project-URL: Source, https://github.com/RWTH-EBC/filip
-Project-URL: Download, https://github.com/RWTH-EBC/FiLiP/archive/refs/tags/v0.4.0.tar.gz
+Project-URL: Download, https://github.com/RWTH-EBC/FiLiP/archive/refs/tags/v0.4.1.tar.gz
 Keywords: iot,fiware,semantic
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -28,14 +28,15 @@
 Requires-Dist: pydantic~=2.5.2
 Requires-Dist: pydantic-settings~=2.0.0
 Requires-Dist: stringcase>=1.2.0
 Requires-Dist: rdflib~=6.0.0
 Requires-Dist: regex~=2023.10.3
 Requires-Dist: requests~=2.31.0
 Requires-Dist: rapidfuzz~=3.4.0
+Requires-Dist: geojson-pydantic~=1.0.2
 Requires-Dist: wget~=3.2
 Provides-Extra: semantics
 Requires-Dist: igraph~=0.11.2; extra == "semantics"
 Requires-Dist: pandas~=1.3.5; python_version < "3.9"
 Requires-Dist: pandas~=2.1.4; python_version >= "3.9"
 
 ![E.ON EBC RWTH Aachen University](https://raw.githubusercontent.com/RWTH-EBC/FiLiP/master/docs/logos/EBC_Logo.png)
```

### Comparing `filip-0.4.0/filip.egg-info/SOURCES.txt` & `filip-0.4.1/filip.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `filip-0.4.0/setup.py` & `filip-0.4.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,19 +14,20 @@
                     'pydantic~=2.5.2',
                     'pydantic-settings~=2.0.0',
                     'stringcase>=1.2.0',
                     'rdflib~=6.0.0',
                     'regex~=2023.10.3',
                     'requests~=2.31.0',
                     'rapidfuzz~=3.4.0',
+                    'geojson-pydantic~=1.0.2',
                     'wget~=3.2']
 
 SETUP_REQUIRES = INSTALL_REQUIRES.copy()
 
-VERSION = '0.4.0'
+VERSION = '0.4.1'
 
 setuptools.setup(
     name='filip',
     version=VERSION,
     author='RWTH Aachen University, E.ON Energy Research Center, Institute\
         of Energy Efficient Buildings and Indoor Climate',
     author_email='tstorek@eonerc.rwth-aachen.de',
```

### Comparing `filip-0.4.0/tests/test_config.py` & `filip-0.4.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `filip-0.4.0/tests/test_logging.py` & `filip-0.4.1/tests/test_logging.py`

 * *Files identical despite different names*

