# Comparing `tmp/caosadvancedtools-0.8.0.tar.gz` & `tmp/caosadvancedtools-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caosadvancedtools-0.8.0.tar", last modified: Tue May 30 10:54:47 2023, max compression
+gzip compressed data, was "caosadvancedtools-0.9.0.tar", last modified: Mon Nov 27 11:07:54 2023, max compression
```

## Comparing `caosadvancedtools-0.8.0.tar` & `caosadvancedtools-0.9.0.tar`

### file list

```diff
@@ -1,83 +1,84 @@
-drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-05-30 10:54:47.966050 caosadvancedtools-0.8.0/
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    34283 2021-06-28 12:58:26.000000 caosadvancedtools-0.8.0/LICENSE.md
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     2419 2023-05-30 10:54:47.966050 caosadvancedtools-0.8.0/PKG-INFO
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     2102 2023-01-20 12:51:13.000000 caosadvancedtools-0.8.0/README.md
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      106 2023-05-30 10:54:47.966050 caosadvancedtools-0.8.0/setup.cfg
--rwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     6056 2023-05-30 10:53:36.000000 caosadvancedtools-0.8.0/setup.py
-drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-05-30 10:54:47.959383 caosadvancedtools-0.8.0/src/
-drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-05-30 10:54:47.962716 caosadvancedtools-0.8.0/src/caosadvancedtools/
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2021-11-02 16:30:12.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/__init__.py
-drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-05-30 10:54:47.962716 caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      159 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/__init__.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     6576 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/bloxberg.py
-drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-05-30 10:54:47.962716 caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     1287 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/__init__.py
-drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-05-30 10:54:47.962716 caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/api/
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      195 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/api/__init__.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     5531 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/api/certificate_api.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     5282 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/api/pdf_api.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    24792 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/api_client.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     8020 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/configuration.py
-drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-05-30 10:54:47.966050 caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/models/
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      864 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/models/__init__.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     7893 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/models/batch.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    12267 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/models/controller_cert_tools_generate_pdf_json_certificate.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    13035 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/models/controller_cert_tools_generate_unsigned_certificate_json_certificate.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3184 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/models/http_validation_error.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     4461 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/models/validation_error.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    13216 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/rest.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    13688 2023-05-30 10:53:36.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/cache.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    28483 2023-05-30 10:53:36.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/cfood.py
-drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-05-30 10:54:47.966050 caosadvancedtools-0.8.0/src/caosadvancedtools/cfoods/
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      873 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/cfoods/__init__.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    10328 2022-09-05 11:41:03.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/cfoods/h5.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3522 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/collect_datamodel.py
-drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-05-30 10:54:47.966050 caosadvancedtools-0.8.0/src/caosadvancedtools/converter/
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2021-06-28 12:58:26.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/converter/__init__.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     5903 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/converter/labfolder_api.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     7147 2021-06-28 12:58:26.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/converter/labfolder_export.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    31105 2023-05-30 10:53:36.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/crawler.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     1064 2021-11-02 16:30:12.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/datainconsistency.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3643 2021-11-02 16:30:12.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/datamodel_problems.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     1605 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/example_cfood.py
--rwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     4892 2023-05-30 10:53:36.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/export_related.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     2079 2021-11-02 16:30:12.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/guard.py
--rwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3629 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/import_from_xml.py
--rwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    10427 2023-03-09 08:58:02.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/loadFiles.py
-drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-05-30 10:54:47.966050 caosadvancedtools-0.8.0/src/caosadvancedtools/models/
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)       47 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/models/__init__.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     9272 2023-01-20 12:51:13.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/models/data_model.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    36974 2023-05-30 10:53:36.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/models/parser.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     7225 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/pandoc_header_tools.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3975 2021-06-28 12:58:26.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/read_md_header.py
-drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-05-30 10:54:47.966050 caosadvancedtools-0.8.0/src/caosadvancedtools/scifolder/
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      273 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/scifolder/__init__.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     5287 2021-11-02 16:30:12.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/scifolder/analysis_cfood.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3995 2022-07-15 11:33:25.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/scifolder/experiment_cfood.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     1528 2021-11-02 16:30:12.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/scifolder/generic_pattern.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     4433 2021-11-02 16:30:12.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/scifolder/publication_cfood.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3620 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/scifolder/result_table_cfood.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     4738 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/scifolder/simulation_cfood.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     4779 2021-11-02 16:30:12.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/scifolder/software_cfood.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     6965 2023-05-30 10:53:36.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/scifolder/utils.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    10013 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/scifolder/withreadme.py
-drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-05-30 10:54:47.966050 caosadvancedtools-0.8.0/src/caosadvancedtools/serverside/
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2021-11-02 16:30:12.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/serverside/__init__.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     7145 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/serverside/generic_analysis.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    13742 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/serverside/helper.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     2381 2021-11-02 16:30:12.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/serverside/logging.py
--rwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      217 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/serverside/sync.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     4916 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/structure_mapping.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3135 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/suppressKnown.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3291 2023-05-30 10:53:36.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/table_converter.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    12578 2022-06-14 14:35:20.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/table_export.py
--rwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    17103 2023-05-30 10:53:36.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/table_importer.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     7144 2023-03-09 08:58:02.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/utils.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      242 2023-05-30 10:54:47.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/version.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3400 2021-11-02 16:30:12.000000 caosadvancedtools-0.8.0/src/caosadvancedtools/webui_formatter.py
-drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-05-30 10:54:47.962716 caosadvancedtools-0.8.0/src/caosadvancedtools.egg-info/
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     2419 2023-05-30 10:54:47.000000 caosadvancedtools-0.8.0/src/caosadvancedtools.egg-info/PKG-INFO
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3186 2023-05-30 10:54:47.000000 caosadvancedtools-0.8.0/src/caosadvancedtools.egg-info/SOURCES.txt
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        1 2023-05-30 10:54:47.000000 caosadvancedtools-0.8.0/src/caosadvancedtools.egg-info/dependency_links.txt
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      165 2023-05-30 10:54:47.000000 caosadvancedtools-0.8.0/src/caosadvancedtools.egg-info/requires.txt
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)       18 2023-05-30 10:54:47.000000 caosadvancedtools-0.8.0/src/caosadvancedtools.egg-info/top_level.txt
+drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-11-27 11:07:54.532245 caosadvancedtools-0.9.0/
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    34283 2021-06-28 12:58:26.000000 caosadvancedtools-0.9.0/LICENSE.md
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     2420 2023-11-27 11:07:54.532245 caosadvancedtools-0.9.0/PKG-INFO
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     2103 2023-11-27 11:07:00.000000 caosadvancedtools-0.9.0/README.md
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      106 2023-11-27 11:07:54.532245 caosadvancedtools-0.9.0/setup.cfg
+-rwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     6067 2023-11-27 11:07:00.000000 caosadvancedtools-0.9.0/setup.py
+drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-11-27 11:07:54.518911 caosadvancedtools-0.9.0/src/
+drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-11-27 11:07:54.525578 caosadvancedtools-0.9.0/src/caosadvancedtools/
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2021-11-02 16:30:12.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/__init__.py
+drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-11-27 11:07:54.525578 caosadvancedtools-0.9.0/src/caosadvancedtools/bloxberg/
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      159 2022-06-14 14:35:20.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/bloxberg/__init__.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     6576 2022-06-14 14:35:20.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/bloxberg/bloxberg.py
+drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-11-27 11:07:54.525578 caosadvancedtools-0.9.0/src/caosadvancedtools/bloxberg/swagger_client/
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     1293 2023-11-27 11:07:00.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/bloxberg/swagger_client/__init__.py
+drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-11-27 11:07:54.525578 caosadvancedtools-0.9.0/src/caosadvancedtools/bloxberg/swagger_client/api/
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      195 2022-06-14 14:35:20.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/bloxberg/swagger_client/api/__init__.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     5531 2022-06-14 14:35:20.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/bloxberg/swagger_client/api/certificate_api.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     5282 2022-06-14 14:35:20.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/bloxberg/swagger_client/api/pdf_api.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    24788 2023-11-27 11:07:00.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/bloxberg/swagger_client/api_client.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     8020 2022-06-14 14:35:20.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/bloxberg/swagger_client/configuration.py
+drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-11-27 11:07:54.528911 caosadvancedtools-0.9.0/src/caosadvancedtools/bloxberg/swagger_client/models/
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      864 2022-06-14 14:35:20.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/bloxberg/swagger_client/models/__init__.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     7894 2023-11-27 11:07:00.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/bloxberg/swagger_client/models/batch.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    12268 2023-11-27 11:07:00.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/bloxberg/swagger_client/models/controller_cert_tools_generate_pdf_json_certificate.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    13036 2023-11-27 11:07:00.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/bloxberg/swagger_client/models/controller_cert_tools_generate_unsigned_certificate_json_certificate.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3185 2023-11-27 11:07:00.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/bloxberg/swagger_client/models/http_validation_error.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     4462 2023-11-27 11:07:00.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/bloxberg/swagger_client/models/validation_error.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    13216 2022-06-14 14:35:20.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/bloxberg/swagger_client/rest.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    13695 2023-11-27 11:07:00.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/cache.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    28483 2023-05-30 10:53:36.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/cfood.py
+drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-11-27 11:07:54.528911 caosadvancedtools-0.9.0/src/caosadvancedtools/cfoods/
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      873 2022-06-14 14:35:20.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/cfoods/__init__.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    10328 2022-09-05 11:41:03.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/cfoods/h5.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3522 2022-06-14 14:35:20.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/collect_datamodel.py
+drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-11-27 11:07:54.528911 caosadvancedtools-0.9.0/src/caosadvancedtools/converter/
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2021-06-28 12:58:26.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/converter/__init__.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     5903 2022-06-14 14:35:20.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/converter/labfolder_api.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     7147 2021-06-28 12:58:26.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/converter/labfolder_export.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    31105 2023-05-30 10:53:36.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/crawler.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     1064 2021-11-02 16:30:12.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/datainconsistency.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3643 2021-11-02 16:30:12.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/datamodel_problems.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     1605 2022-06-14 14:35:20.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/example_cfood.py
+-rwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     4892 2023-05-30 10:53:36.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/export_related.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     2079 2021-11-02 16:30:12.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/guard.py
+-rwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3629 2022-06-14 14:35:20.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/import_from_xml.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    29798 2023-11-27 11:07:00.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/json_schema_exporter.py
+-rwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    10391 2023-11-27 11:07:00.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/loadFiles.py
+drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-11-27 11:07:54.528911 caosadvancedtools-0.9.0/src/caosadvancedtools/models/
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)       47 2022-06-14 14:35:20.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/models/__init__.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    12570 2023-11-27 11:07:00.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/models/data_model.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    39403 2023-11-27 11:07:00.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/models/parser.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     7225 2022-06-14 14:35:20.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/pandoc_header_tools.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3975 2021-06-28 12:58:26.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/read_md_header.py
+drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-11-27 11:07:54.532245 caosadvancedtools-0.9.0/src/caosadvancedtools/scifolder/
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      273 2022-06-14 14:35:20.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/scifolder/__init__.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     5287 2021-11-02 16:30:12.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/scifolder/analysis_cfood.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3995 2022-07-15 11:33:25.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/scifolder/experiment_cfood.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     1528 2021-11-02 16:30:12.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/scifolder/generic_pattern.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     4433 2021-11-02 16:30:12.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/scifolder/publication_cfood.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3620 2022-06-14 14:35:20.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/scifolder/result_table_cfood.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     4738 2022-06-14 14:35:20.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/scifolder/simulation_cfood.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     4779 2021-11-02 16:30:12.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/scifolder/software_cfood.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     6965 2023-05-30 10:53:36.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/scifolder/utils.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    10013 2022-06-14 14:35:20.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/scifolder/withreadme.py
+drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-11-27 11:07:54.532245 caosadvancedtools-0.9.0/src/caosadvancedtools/serverside/
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2021-11-02 16:30:12.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/serverside/__init__.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     7145 2022-06-14 14:35:20.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/serverside/generic_analysis.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    13742 2022-06-14 14:35:20.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/serverside/helper.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     2381 2021-11-02 16:30:12.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/serverside/logging.py
+-rwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      217 2022-06-14 14:35:20.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/serverside/sync.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     4916 2022-06-14 14:35:20.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/structure_mapping.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3135 2022-06-14 14:35:20.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/suppressKnown.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3291 2023-05-30 10:53:36.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/table_converter.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    13371 2023-11-27 11:07:00.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/table_export.py
+-rwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    17408 2023-11-27 11:07:00.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/table_importer.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     7144 2023-03-09 08:58:02.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/utils.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      242 2023-11-27 11:07:53.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/version.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3400 2021-11-02 16:30:12.000000 caosadvancedtools-0.9.0/src/caosadvancedtools/webui_formatter.py
+drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-11-27 11:07:54.525578 caosadvancedtools-0.9.0/src/caosadvancedtools.egg-info/
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     2420 2023-11-27 11:07:54.000000 caosadvancedtools-0.9.0/src/caosadvancedtools.egg-info/PKG-INFO
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3232 2023-11-27 11:07:54.000000 caosadvancedtools-0.9.0/src/caosadvancedtools.egg-info/SOURCES.txt
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        1 2023-11-27 11:07:54.000000 caosadvancedtools-0.9.0/src/caosadvancedtools.egg-info/dependency_links.txt
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      176 2023-11-27 11:07:54.000000 caosadvancedtools-0.9.0/src/caosadvancedtools.egg-info/requires.txt
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)       18 2023-11-27 11:07:54.000000 caosadvancedtools-0.9.0/src/caosadvancedtools.egg-info/top_level.txt
```

### Comparing `caosadvancedtools-0.8.0/LICENSE.md` & `caosadvancedtools-0.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.8.0/PKG-INFO` & `caosadvancedtools-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caosadvancedtools
-Version: 0.8.0
+Version: 0.9.0
 Summary: advanced utilities for caosdb
 Author: Henrik tom Wörden
 Author-email: h.tomwoerden@indiscale.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: h5-crawler
 Provides-Extra: gitignore-parser
@@ -12,14 +12,15 @@
 
 # README
 
 ## Welcome
 
 This is the **CaosDB Advanced User Tools** repository and a part of the
 CaosDB project.
+
 This project contains tools that are beyond the typical use of
 the CaosDB python client. Especially, this includes the crawler which will
 typically be used by a data curator.
 
 ## Setup
 
 Please read the [README_SETUP.md](README_SETUP.md) for instructions on how to
```

### Comparing `caosadvancedtools-0.8.0/README.md` & `caosadvancedtools-0.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # README
 
 ## Welcome
 
 This is the **CaosDB Advanced User Tools** repository and a part of the
 CaosDB project.
+
 This project contains tools that are beyond the typical use of
 the CaosDB python client. Especially, this includes the crawler which will
 typically be used by a data curator.
 
 ## Setup
 
 Please read the [README_SETUP.md](README_SETUP.md) for instructions on how to
```

### Comparing `caosadvancedtools-0.8.0/setup.py` & `caosadvancedtools-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 # DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
 # THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 ########################################################################
 
 MAJOR = 0
-MINOR = 8
+MINOR = 9
 MICRO = 0
 PRE = ""  # e.g. rc0, alpha.1, 0.beta-23
 ISRELEASED = True
 
 if PRE:
     VERSION = "{}.{}.{}-{}".format(MAJOR, MINOR, MICRO, PRE)
 else:
@@ -151,17 +151,17 @@
         version=get_version_info()[0],
         description='advanced utilities for caosdb',
         long_description=long_description,
         long_description_content_type="text/markdown",
         author='Henrik tom Wörden',
         author_email='h.tomwoerden@indiscale.com',
         python_requires='>=3.7',
-        install_requires=["caosdb>=0.11.0",
+        install_requires=["linkahead>=0.13.1",
                           "jsonref",
-                          "jsonschema>=4.4.0",
+                          "jsonschema[format]>=4.4.0",
                           "numpy>=1.17.3",
                           "openpyxl>=3.0.7",
                           "pandas>=1.2.0",
                           "xlrd>=2.0",
                           ],
         extras_require={"h5-crawler": ["h5py>=3.3.0", ],
                         "gitignore-parser": ["gitignore-parser >=0.1.0", ],
```

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/bloxberg.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/bloxberg/bloxberg.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/__init__.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/bloxberg/swagger_client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,26 +9,27 @@
 
     OpenAPI spec version: 0.2.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
+from swagger_client.models.validation_error import ValidationError
+from swagger_client.models.http_validation_error import HTTPValidationError
+from swagger_client.models.controller_cert_tools_generate_unsigned_certificate_json_certificate import ControllerCertToolsGenerateUnsignedCertificateJsonCertificate
+from swagger_client.models.controller_cert_tools_generate_pdf_json_certificate import ControllerCertToolsGeneratePdfJsonCertificate
+from swagger_client.models.batch import Batch
+from swagger_client.configuration import Configuration
+from swagger_client.api_client import ApiClient
+from swagger_client.api.pdf_api import PdfApi
+from swagger_client.api.certificate_api import CertificateApi
 
 # Fake the installation
-import sys, pathlib
+import sys
+import pathlib
 __this_dir = str(pathlib.Path(__file__).parent.parent)
 if __this_dir not in sys.path:
     sys.path.append(__this_dir)
 
 # import apis into sdk package
-from swagger_client.api.certificate_api import CertificateApi
-from swagger_client.api.pdf_api import PdfApi
 # import ApiClient
-from swagger_client.api_client import ApiClient
-from swagger_client.configuration import Configuration
 # import models into sdk package
-from swagger_client.models.batch import Batch
-from swagger_client.models.controller_cert_tools_generate_pdf_json_certificate import ControllerCertToolsGeneratePdfJsonCertificate
-from swagger_client.models.controller_cert_tools_generate_unsigned_certificate_json_certificate import ControllerCertToolsGenerateUnsignedCertificateJsonCertificate
-from swagger_client.models.http_validation_error import HTTPValidationError
-from swagger_client.models.validation_error import ValidationError
```

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/api/certificate_api.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/bloxberg/swagger_client/api/certificate_api.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/api/pdf_api.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/bloxberg/swagger_client/api/pdf_api.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/api_client.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/bloxberg/swagger_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -587,15 +587,15 @@
                 reason=(
                     "Failed to parse `{0}` as datetime object"
                     .format(string)
                 )
             )
 
     def __hasattr(self, object, name):
-            return name in object.__class__.__dict__
+        return name in object.__class__.__dict__
 
     def __deserialize_model(self, data, klass):
         """Deserializes list or dict to model.
 
         :param data: dict, list.
         :param klass: class literal.
         :return: model object.
```

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/configuration.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/bloxberg/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/models/__init__.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/bloxberg/swagger_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/models/batch.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/bloxberg/swagger_client/models/batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
+
 class Batch(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/models/controller_cert_tools_generate_pdf_json_certificate.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/bloxberg/swagger_client/models/controller_cert_tools_generate_pdf_json_certificate.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
+
 class ControllerCertToolsGeneratePdfJsonCertificate(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/models/controller_cert_tools_generate_unsigned_certificate_json_certificate.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/bloxberg/swagger_client/models/controller_cert_tools_generate_unsigned_certificate_json_certificate.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
+
 class ControllerCertToolsGenerateUnsignedCertificateJsonCertificate(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/models/http_validation_error.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/bloxberg/swagger_client/models/http_validation_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
+
 class HTTPValidationError(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/models/validation_error.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/bloxberg/swagger_client/models/validation_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
+
 class ValidationError(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/bloxberg/swagger_client/rest.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/bloxberg/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/cache.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,24 +23,23 @@
 #
 # ** end header
 
 # Note: This is implementing a cache on client side. It would be great if the server would provide
 # something to replace this.
 import os
 import sqlite3
-from copy import deepcopy
+import tempfile
+import warnings
 from abc import ABC, abstractmethod
+from copy import deepcopy
 from hashlib import sha256
-import warnings
 
 import caosdb as db
 from lxml import etree
 
-import tempfile
-
 
 def put_in_container(stuff):
     if isinstance(stuff, list):
         stuff = db.Container().extend(stuff)
 
     if not isinstance(stuff, db.Container):
         stuff = db.Container().append(stuff)
@@ -340,15 +339,15 @@
     def get_previous_version(cont):
         """ Retrieve the current, unchanged version of the entities that shall
         be updated, i.e. the version before the update """
 
         old_ones = db.Container()
 
         for ent in cont:
-            old_ones.append(db.execute_query("FIND ENTITY {}".format(ent.id),
+            old_ones.append(db.execute_query("FIND ENTITY WITH ID={}".format(ent.id),
                                              unique=True))
 
         return old_ones
 
     def insert(self, cont, run_id, insert=False):
         """Insert a pending, unauthorized insert or update
```

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/cfood.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/cfood.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/cfoods/__init__.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/cfoods/__init__.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/cfoods/h5.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/cfoods/h5.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/collect_datamodel.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/collect_datamodel.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/converter/labfolder_api.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/converter/labfolder_api.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/converter/labfolder_export.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/converter/labfolder_export.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/crawler.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/crawler.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/datainconsistency.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/datainconsistency.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/datamodel_problems.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/datamodel_problems.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/example_cfood.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/example_cfood.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/export_related.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/export_related.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/guard.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/guard.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/import_from_xml.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/import_from_xml.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/loadFiles.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/loadFiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,16 +171,16 @@
                        + path})
 
         totalsize = 0  # collecting total size of all new files
 
         for f in files:
             totalsize += f.size
 
-        logger.info("Made in total {} new files with a combined size of {} "
-                    "accessible.".format(len(files), convert_size(totalsize)))
+        logger.info(
+            f"Made new files accessible: {len(files)}, combined size: {convert_size(totalsize)} ")
 
     return
 
 
 def main(argv=None):
     '''Command line options.'''
```

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/models/data_model.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/models/data_model.py`

 * *Files 22% similar despite different names*

```diff
@@ -25,16 +25,17 @@
 from copy import deepcopy
 # TODO(fspreck) for backwards compatibility with Python < 3.9 but this is
 # actually
 # [deprecated](https://docs.python.org/3/library/typing.html#typing.List), so
 # remove this, when we drop support for old Python versions.
 from typing import List
 
-import caosdb as db
-from caosdb.apiutils import compare_entities, describe_diff
+import linkahead as db
+import linkahead.common.models as models
+from linkahead.apiutils import compare_entities, describe_diff, merge_entities
 
 
 CAOSDB_INTERNAL_PROPERTIES = [
     "description",
     "name",
     "unit",
 ]
@@ -56,15 +57,16 @@
     This is possible because entities, defined in this model, are identified
     with entities in CaosDB using names. I.e. a RecordType "Experiment" in this
     model will update an existing RecordType with name "Experiment" in CaosDB.
     Thus, be carefull not to change existing Entities that were created for a
     different purpose (e.g. someone else's experiment).
 
     DataModel inherits from dict. The keys are always the names of the
-    entities. Thus you cannot have unnamed entities in your model.
+    entities. Thus you cannot have unnamed or ambiguously named entities in your
+    model.
 
     Example:
 
     # Create a DataModel with a RecordType and a Property, not assuming any
     # relation between the two.
     dm = DataModel([db.RecordType(name="myRecordType"),
                     db.Property(name="myProperty")])
@@ -257,7 +259,77 @@
         for ent in self.values():
             all_ents[ent.name] = ent
 
             for prop in ent.get_properties():
                 all_ents[prop.name] = prop
 
         return list(all_ents.values())
+
+    def get_deep(self, name: str, visited_props: dict = None, visited_parents: set = None):
+        """Attempt to resolve references for the given ``name``.
+
+        The returned entity has all the properties it inherits from its ancestry and all properties
+        have the correct descriptions and datatypes.  This methods only uses data which is available
+        in this DataModel, which acts kind of like a cache pool.
+
+        Note that this may change this data model (subsequent "get" like calls may also return
+        deeper content.)
+
+        """
+        entity = self.get(name)
+        if not entity:
+            return entity
+        if not visited_props:
+            visited_props = {}
+        if not visited_parents:
+            visited_parents = set()
+
+        importances = {
+            models.OBLIGATORY: 0,
+            models.RECOMMENDED: 1,
+            models.SUGGESTED: 2,
+        }
+
+        for parent in list(entity.get_parents()):  # Make a change-resistant list copy.
+            if parent.name in visited_parents:
+                continue
+            visited_parents.add(parent.name)
+            parent_importance = importances.get(parent._flags.get("inheritance"), 999)
+            if parent.name in self:
+                deep_parent = self.get_deep(parent.name,  # visited_props=visited_props,
+                                            visited_parents=visited_parents
+                                            )
+
+                for prop in deep_parent.properties:
+                    importance = importances[deep_parent.get_importance(prop.name)]
+                    if (importance <= parent_importance
+                            and prop.name not in [prop.name for prop in entity.properties]):
+                        entity.add_property(prop)
+            else:
+                print(f"Referenced parent \"{parent.name}\" not found in data model.")
+
+        for prop in list(entity.get_properties()):  # Make a change-resistant list copy.
+            if prop.name in visited_props:
+                if visited_props[prop.name]:
+                    deep_prop = visited_props[prop.name]
+                    merge_entities(prop, deep_prop)
+                    prop.datatype = deep_prop.datatype
+                    prop.value = deep_prop.value
+                    prop.unit = deep_prop.unit
+                continue
+            visited_props[prop.name] = None
+            if prop.name in self:
+                deep_prop = self.get_deep(prop.name, visited_props=visited_props,
+                                          visited_parents=visited_parents)
+                linked_prop = entity.get_property(prop)
+                if not linked_prop.datatype:
+                    if deep_prop.role == "Property":
+                        linked_prop.datatype = deep_prop.datatype
+                    elif deep_prop.role == "RecordType":
+                        linked_prop.datatype = deep_prop
+                if deep_prop.description:
+                    linked_prop.description = deep_prop.description
+                visited_props[prop.name] = deep_prop
+            else:
+                print(f"Referenced property \"{prop.name}\" not found in data model.")
+
+        return entity
```

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/models/parser.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/models/parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This file is a part of the CaosDB Project.
 #
-# Copyright (C) 2022 IndiScale GmbH <info@indiscale.com>
+# Copyright (C) 2023 IndiScale GmbH <info@indiscale.com>
 # Copyright (C) 2022 Florian Spreckelsen <f.spreckelsen@indiscale.com>
-# Copyright (C) 2022 Daniel Hornung <d.hornung@indiscale.com>
+# Copyright (C) 2023 Daniel Hornung <d.hornung@indiscale.com>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -38,20 +38,21 @@
 import argparse
 import json
 import jsonref
 import re
 import sys
 import yaml
 
-from typing import List
+from typing import List, Optional
 from warnings import warn
 
 import jsonschema
-import caosdb as db
+import linkahead as db
 
+from linkahead.common.datatype import get_list_datatype
 from .data_model import CAOSDB_INTERNAL_PROPERTIES, DataModel
 
 # Keywords which are allowed in data model descriptions.
 KEYWORDS = ["parent",  # deprecated, use inherit_from_* instead:
                        # https://gitlab.com/caosdb/caosdb-advanced-user-tools/-/issues/36
             "importance",
             "datatype",  # for example TEXT, INTEGER or REFERENCE
@@ -78,31 +79,14 @@
     "boolean",
     "integer",
     "number",
     "null"
 ]
 
 
-def _get_listdatatype(dtype):
-    """matches a string to check whether the type definition is a list
-
-    returns the type within the list or None, if it cannot be matched with a
-    list definition
-    """
-    # TODO: string representation should be the same as used by the server:
-    # e.g. LIST<TEXT>
-    # this should be changed in the module and the old behavour should be
-    # marked as depricated
-    match = re.match(r"^LIST[(<](?P<dt>.*)[)>]$", dtype)
-
-    if match is None:
-        return None
-    else:
-        return match.group("dt")
-
 # Taken from https://stackoverflow.com/a/53647080, CC-BY-SA, 2018 by
 # https://stackoverflow.com/users/2572431/augurar
 
 
 class SafeLineLoader(yaml.SafeLoader):
     """Load a line and keep meta-information.
 
@@ -136,133 +120,191 @@
     # @author Florian Spreckelsen
     # @date 2022-02-17
     # @review Daniel Hornung 2022-02-18
     def __init__(self, msg):
         super().__init__(msg)
 
 
-def parse_model_from_yaml(filename):
-    """Shortcut if the Parser object is not needed."""
-    parser = Parser()
+def parse_model_from_yaml(filename, existing_model: Optional[dict] = None, debug: bool = False):
+    """Parse a data model from a YAML file.
+
+This is a convenience function if the Parser object is not needed, it calls
+``Parser.parse_model_from_yaml(...)`` internally.
+
+
+Parameters
+----------
+
+existing_model : dict, optional
+  An existing model to which the created model shall be added.
+
+debug : bool, optional
+  If True, turn on miscellaneous debugging.  Default is False.
+    """
+    parser = Parser(debug=debug)
 
-    return parser.parse_model_from_yaml(filename)
+    return parser.parse_model_from_yaml(filename, existing_model=existing_model)
 
 
-def parse_model_from_string(string):
-    """Shortcut if the Parser object is not needed."""
-    parser = Parser()
+def parse_model_from_string(string, existing_model: Optional[dict] = None, debug: bool = False):
+    """Parse a data model from a YAML string
 
-    return parser.parse_model_from_string(string)
+This is a convenience function if the Parser object is not needed, it calls
+``Parser.parse_model_from_string(...)`` internally.
+
+Parameters
+----------
+
+existing_model : dict, optional
+  An existing model to which the created model shall be added.
+
+debug : bool, optional
+  If True, turn on miscellaneous debugging.  Default is False.
+    """
+    parser = Parser(debug=debug)
+
+    return parser.parse_model_from_string(string, existing_model=existing_model)
 
 
 def parse_model_from_json_schema(
         filename: str,
         top_level_recordtype: bool = True,
         types_for_missing_array_items: dict = {},
-        ignore_unspecified_array_items: bool = False
+        ignore_unspecified_array_items: bool = False,
+        existing_model: Optional[dict] = None
 ):
     """Return a datamodel parsed from a json schema definition.
 
     Parameters
     ----------
+
     filename : str
         The path of the json schema file that is to be parsed
+
     top_level_recordtype : bool, optional
         Whether there is a record type defined at the top level of the
         schema. Default is true.
+
     types_for_missing_array_items : dict, optional
         dictionary containing fall-back types for json entries with `type:
         array` but without `items` specification. Default is an empty dict.
+
     ignore_unspecified_array_items : bool, optional
         Whether to ignore `type: array` entries the type of which is not
         specified by their `items` property or given in
         `types_for_missing_array_items`. An error is raised if they are not
         ignored. Default is False.
 
+    existing_model : dict, optional
+        An existing model to which the created model shall be added.  Not implemented yet.
+
     Returns
     -------
+
     out : Datamodel
         The datamodel generated from the input schema which then can be used for
         synchronizing with CaosDB.
 
     Note
     ----
     This is an experimental feature, see ``JsonSchemaParser`` for information
     about the limitations of the current implementation.
 
     """
+    if existing_model is not None:
+        raise NotImplementedError("Adding to an existing model is not implemented yet.")
+
     # @author Florian Spreckelsen
     # @date 2022-02-17
     # @review Timm Fitschen 2023-05-25
     parser = JsonSchemaParser(types_for_missing_array_items, ignore_unspecified_array_items)
 
     return parser.parse_model_from_json_schema(filename, top_level_recordtype)
 
 
 class Parser(object):
-    def __init__(self):
+    def __init__(self, debug: bool = False):
         """Initialize an empty parser object and initialize the dictionary of entities and the list of
         treated elements.
 
+Parameters
+----------
+
+debug : bool, optional
+  If True, turn on miscellaneous debugging.  Default is False.
+
         """
         self.model = {}
         self.treated = []
+        self.debug = debug
 
-    def parse_model_from_yaml(self, filename):
+    def parse_model_from_yaml(self, filename, existing_model: Optional[dict] = None):
         """Create and return a data model from the given file.
 
         Parameters
         ----------
         filename : str
           The path to the YAML file.
 
+        existing_model : dict, optional
+          An existing model to which the created model shall be added.
+
         Returns
         -------
         out : DataModel
           The created DataModel
         """
         with open(filename, 'r') as outfile:
             ymlmodel = yaml.load(outfile, Loader=SafeLineLoader)
 
-        return self._create_model_from_dict(ymlmodel)
+        return self._create_model_from_dict(ymlmodel, existing_model=existing_model)
 
-    def parse_model_from_string(self, string):
+    def parse_model_from_string(self, string, existing_model: Optional[dict] = None):
         """Create and return a data model from the given YAML string.
 
         Parameters
         ----------
         string : str
           The YAML string.
 
+        existing_model : dict, optional
+          An existing model to which the created model shall be added.
+
         Returns
         -------
         out : DataModel
           The created DataModel
         """
         ymlmodel = yaml.load(string, Loader=SafeLineLoader)
 
-        return self._create_model_from_dict(ymlmodel)
+        return self._create_model_from_dict(ymlmodel, existing_model=existing_model)
 
-    def _create_model_from_dict(self, ymlmodel):
+    def _create_model_from_dict(self, ymlmodel, existing_model: Optional[dict] = None):
         """Create and return a data model out of the YAML dict `ymlmodel`.
 
         Parameters
         ----------
         ymlmodel : dict
           The dictionary parsed from a YAML file.
 
+        existing_model : dict, optional
+          An existing model to which the created model shall be added.
+
         Returns
         -------
         out : DataModel
           The created DataModel
         """
 
         if not isinstance(ymlmodel, dict):
             raise ValueError("Yaml file should only contain one dictionary!")
 
+        if existing_model is not None:
+            self.model.update(existing_model)
+
         # Extern keyword:
         # The extern keyword can be used to include Properties and RecordTypes
         # from existing CaosDB datamodels into the current model.
         # Any name included in the list specified by the extern keyword
         # will be used in queries to retrieve a property or (if no property exists)
         # a record type with the name of the element.
         # The retrieved entity will be added to the model.
@@ -290,15 +332,20 @@
         for name, entity in ymlmodel.items():
             self._add_entity_to_model(name, entity)
         # initialize recordtypes
         self._set_recordtypes()
         self._check_and_convert_datatypes()
 
         for name, entity in ymlmodel.items():
-            self._treat_entity(name, entity, line=ymlmodel["__line__"])
+            try:
+                self._treat_entity(name, entity, line=ymlmodel["__line__"])
+            except ValueError as err:
+                err_str = err.args[0].replace("invalid keyword:",
+                                              f"invalid keyword in line {entity['__line__']}:", 1)
+                raise ValueError(err_str, *err.args[1:]) from err
 
         return DataModel(self.model.values())
 
     @staticmethod
     def _stringify(name, context=None):
         """Make a string out of `name`.
 
@@ -341,21 +388,20 @@
 
         if name not in self.model:
             self.model[name] = None
 
         if definition is None:
             return
 
-        if (self.model[name] is None
-                and isinstance(definition, dict)
+        if (self.model[name] is None and isinstance(definition, dict)
                 # is it a property
                 and "datatype" in definition
                 # but not simply an RT of the model
-                and not (_get_listdatatype(definition["datatype"]) == name and
-                         _get_listdatatype(definition["datatype"]) in self.model)):
+                and not (get_list_datatype(definition["datatype"]) == name and
+                         get_list_datatype(definition["datatype"]) in self.model)):
 
             # and create the new property
             self.model[name] = db.Property(name=name,
                                            datatype=definition["datatype"])
         elif (self.model[name] is None and isinstance(definition, dict)
               and "role" in definition):
             if definition["role"] == "RecordType":
@@ -397,14 +443,17 @@
                         line = definition["__line__"]
 
                         if isinstance(definition[prop_type], list):
                             line = definition[prop_type][0]["__line__"]
                         raise YamlDefinitionError(line) from None
                     raise
 
+        if self.debug and self.model[name] is not None:
+            self.model[name].__line__ = definition["__line__"]
+
     def _add_to_recordtype(self, ent_name, props, importance):
         """Add properties to a RecordType.
 
         Parameters
         ----------
         ent_name : str
           The name of the entity to which the properties shall be added.
@@ -430,17 +479,17 @@
                     props["__line__"], n))
 
             if n == "__line__":
                 continue
             n = self._stringify(n)
 
             if isinstance(e, dict):
-                if "datatype" in e and _get_listdatatype(e["datatype"]) is not None:
+                if "datatype" in e and get_list_datatype(e["datatype"]) is not None:
                     # Reuse the existing datatype for lists.
-                    datatype = db.LIST(_get_listdatatype(e["datatype"]))
+                    datatype = db.LIST(get_list_datatype(e["datatype"]))
                 else:
                     # Ignore a possible e["datatype"] here if it's not a list
                     # since it has been treated in the definition of the
                     # property (entity) already
                     datatype = None
                 if "value" in e:
                     value = e["value"]
@@ -454,14 +503,17 @@
             self.model[ent_name].add_property(name=n,
                                               value=value,
                                               importance=importance,
                                               datatype=datatype)
 
     def _inherit(self, name, prop, inheritance):
         if not isinstance(prop, list):
+            if isinstance(prop, str):
+                raise YamlDefinitionError(
+                    f"Parents must be a list but is given as string: {name} > {prop}")
             raise YamlDefinitionError("Parents must be a list, error in line {}".format(
                 prop["__line__"]))
 
         for pname in prop:
             if not isinstance(pname, str):
                 raise ValueError("Only provide the names of parents.")
             self.model[name].add_parent(name=pname, inheritance=inheritance)
@@ -477,17 +529,21 @@
             if definition is None:
                 return
 
             # for setting values of properties directly:
             if not isinstance(definition, dict):
                 return
 
-            if ("datatype" in definition
-                    and definition["datatype"].startswith("LIST")):
+            # These definition items must be handled even for list props.
+            for prop_name, prop in definition.items():
+                if prop_name == "description":
+                    self.model[name].description = prop
 
+            # For lists, everything else is not needed at this level.
+            if ("datatype" in definition and definition["datatype"].startswith("LIST")):
                 return
 
             if name in self.treated:
                 raise TwiceDefinedException(name)
 
             for prop_name, prop in definition.items():
                 if prop_name == "__line__":
@@ -497,15 +553,16 @@
                 if prop_name == "unit":
                     self.model[name].unit = prop
 
                 elif prop_name == "value":
                     self.model[name].value = prop
 
                 elif prop_name == "description":
-                    self.model[name].description = prop
+                    # Handled above
+                    continue
 
                 elif prop_name == "recommended_properties":
                     self._add_to_recordtype(
                         name, prop, importance=db.RECOMMENDED)
 
                     for n, e in prop.items():
                         self._treat_entity(n, e)
@@ -571,23 +628,27 @@
 
         for key, value in self.model.items():
 
             if isinstance(value, db.Property):
                 dtype = value.datatype
                 is_list = False
 
-                if _get_listdatatype(value.datatype) is not None:
-                    dtype = _get_listdatatype(value.datatype)
+                if get_list_datatype(dtype) is not None:
+                    dtype = get_list_datatype(dtype)
                     is_list = True
 
-                if dtype in self.model:
+                dtype_name = dtype
+                if not isinstance(dtype_name, str):
+                    dtype_name = dtype.name
+
+                if dtype_name in self.model:
                     if is_list:
-                        value.datatype = db.LIST(self.model[dtype])
+                        value.datatype = db.LIST(self.model[dtype_name])
                     else:
-                        value.datatype = self.model[dtype]
+                        value.datatype = self.model[dtype_name]
 
                     continue
 
                 if dtype in [db.DOUBLE,
                              db.REFERENCE,
                              db.TEXT,
                              db.DATETIME,
@@ -601,15 +662,15 @@
                     else:
                         value.datatype = db.__getattribute__(  # pylint: disable=no-member
                             dtype)
 
                     continue
 
                 raise ValueError("Property {} has an unknown datatype: {}".format(
-                    value.name, value.datatype))
+                    value.name, dtype_name))
 
     def _set_recordtypes(self):
         """ properties are defined in first iteration; set remaining as RTs """
 
         for key, value in self.model.items():
             if value is None:
                 self.model[key] = db.RecordType(name=key)
```

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/pandoc_header_tools.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/pandoc_header_tools.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/read_md_header.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/read_md_header.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/scifolder/analysis_cfood.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/scifolder/analysis_cfood.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/scifolder/experiment_cfood.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/scifolder/experiment_cfood.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/scifolder/generic_pattern.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/scifolder/generic_pattern.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/scifolder/publication_cfood.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/scifolder/publication_cfood.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/scifolder/result_table_cfood.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/scifolder/result_table_cfood.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/scifolder/simulation_cfood.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/scifolder/simulation_cfood.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/scifolder/software_cfood.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/scifolder/software_cfood.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/scifolder/utils.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/scifolder/utils.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/scifolder/withreadme.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/scifolder/withreadme.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/serverside/generic_analysis.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/serverside/generic_analysis.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/serverside/helper.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/serverside/helper.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/serverside/logging.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/serverside/logging.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/structure_mapping.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/structure_mapping.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/suppressKnown.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/suppressKnown.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/table_converter.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/table_converter.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/table_export.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/table_export.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 # ** end header
 #
 """Collect optional and mandatory data from CaosDB records and prepare
 them for an export as a table, e.g., for the export to metadata
 repositories.
 
 """
+from inspect import signature
 import json
 import logging
 
 import caosdb as db
 
 FIND_FUNCTION = "find_func"
 QUERY = "query"
@@ -79,30 +80,30 @@
         Notes
         -----
             The entries of the export_dict are themselves dictionaries
             of the form
             ```
             {"entry_to_be_exported: {
                 "optional": True/False
-                "find_func": name of member function
+                "find_func": callable or name of member function
                 "query": query string
                 "selector": selector for the query
                 "error": error explanation
                 }
             }
             ```
             All entries are optional; `query` and `find_func` are
             mutually exclusive and an error will be raised if both are
             provided. The indivdual entries mean:
 
             - optional: True or False, if not present, the entry is
               assumed to be mandatory.
             - find_func: name of the member function that returns the
-              value for this entry. Must not exist together with
-              `query`
+              value for this entry or callable object. Must not exist
+              together with `query`
             - query: Query string for finding the value for this
               entry. If this is given, a record must be given to the
               constructor of this class. The query is then executed as
               `db.execute_query(query.format(record.id). unique=True)`
               so it must return a unique result from which the value
               can be extracted via
               `query_result.get_property_values(selector)`.
@@ -128,22 +129,24 @@
                 raise ValueError(
                     "export_dict must be either a dictionary"
                     " or the path to a json file.")
         self.record = record
         self._check_sanity_of_export_dict()
         self.raise_error_if_missing = raise_error_if_missing
         self.info = {}
+        self.all_keys = [key for key in self.export_dict]
 
     def collect_information(self):
         """Use the items of `export_dict` to collect the information for the
         export.
 
         """
 
-        for e, d in self.export_dict.items():
+        for e in self.all_keys:
+            d = self.export_dict[e]
             if QUERY in d:
                 # TODO: How do we make this more general? There might
                 # be queries that don't need the record or work with
                 # the name instead of the id.
                 q = d[QUERY].format(self.record.id)
                 try:
                     val = db.execute_query(
@@ -159,20 +162,23 @@
                     raise TableExportError(errmssg)
 
                 if val is not None:
                     self.info[e] = val
                 else:
                     self._append_missing(e, d)
             elif FIND_FUNCTION in d:
-                find_fun = getattr(self, d[FIND_FUNCTION])
                 try:
-                    self.info[e] = find_fun()
+                    val = self._call_find_function(d[FIND_FUNCTION], e)
+                    if val is not None:
+                        self.info[e] = val
+                    else:
+                        self._append_missing(e, d)
                 except Exception as exc:
                     self._append_missing(e, d)
-                    logger.debug(exc)
+                    logger.error(exc)
             # last resort: check if record has e as property:
             else:
                 try:
                     self.info[e] = self.record.get_property(e).value
                 except AttributeError as exc:
                     # either record is None, or get_property(e) returns None
                     logger.debug(exc)
@@ -196,14 +202,28 @@
                     errmssg += e + '\n'
 
             if self.raise_error_if_missing:
                 raise TableExportError(errmssg)
             else:
                 logger.error(errmssg)
 
+    def _call_find_function(self, find_function, e):
+        if callable(find_function):
+            find_fun = find_function
+        else:
+            find_fun = getattr(self, find_function)
+
+        sig = signature(find_fun)
+        params = sig.parameters
+        if len(params) > 1:
+            return find_fun(self.record, e)
+        elif len(params) > 0:
+            return find_fun(self.record)
+        return find_fun()
+
     def prepare_csv_export(self, delimiter=',', print_header=False,
                            skip_empty_optionals=False):
         """Return the values in self.info as a single-line string, separated
         by the delimiter. If header is true, a header line with the
         names of the entries, separated by the same delimiter is
         added. Header and body are separated by a newline character.
 
@@ -234,15 +254,16 @@
 
         """
         body = ""
 
         if print_header:
             header = ""
 
-        for e, d in self.export_dict.items():
+        for e in self.all_keys:
+            d = self.export_dict[e]
             if e in self.info:
                 body += str(self.info[e]) + delimiter
 
                 if print_header:
                     header += str(e) + delimiter
             else:
                 if not ("optional" in d and d["optional"]):
@@ -283,15 +304,17 @@
                     ", both a query and a function are given for finding "
                     "the value to be exported. Please spcify either a"
                     " function or a query, not both."
                 )
             # check find function if present
 
             if FIND_FUNCTION in d:
-                if not hasattr(self, d[FIND_FUNCTION]):
+                if callable(d[FIND_FUNCTION]):
+                    pass
+                elif not hasattr(self, d[FIND_FUNCTION]):
                     raise TableExportError(
                         "Find function " + d[FIND_FUNCTION] +
                         " was specified for entry " + e +
                         " but no such function could be found."
                     )
                 elif not callable(getattr(self, d[FIND_FUNCTION])):
                     raise TableExportError(
```

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/table_importer.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/table_importer.py`

 * *Files 4% similar despite different names*

```diff
@@ -318,15 +318,15 @@
 
     def check_datatype(self, df, filename=None, strict=False):
         """Check for each column whether non-null fields have the correct datatype.
 
         .. note::
 
           If columns are integer, but should be float, this method converts the respective columns
-          in place.
+          in place. The same for columns that should have string value but have numeric value.
 
         Parameters
         ----------
 
         strict: boolean, optional
           If False (the default), try to convert columns, otherwise raise an error.
 
@@ -334,17 +334,19 @@
         for key, datatype in self.datatypes.items():
             if key not in df.columns:
                 continue
             # Check for castable numeric types first: We unconditionally cast int to the default
             # float, because CaosDB does not have different sizes anyway.
             col_dtype = df.dtypes[key]
             if not strict and not np.issubdtype(col_dtype, datatype):
-                issub = np.issubdtype
                 #  These special cases should be fine.
-                if issub(col_dtype, np.integer) and issub(datatype, np.floating):
+                if ((datatype == str)
+                        or (np.issubdtype(col_dtype, np.integer)
+                            and np.issubdtype(datatype, np.floating))
+                    ):  # NOQA
                     df[key] = df[key].astype(datatype)
 
             # Now check each element
             for idx, val in df.loc[pd.notnull(df.loc[:, key]), key].items():
 
                 if not isinstance(val, datatype):
                     msg = (
@@ -384,15 +386,16 @@
 
             while okay and i < len(self.obligatory_columns):
                 key = self.obligatory_columns[i]
                 i += 1
                 if key not in df.columns:
                     continue
 
-                if pd.isnull(row.loc[key]):
+                null_check = pd.isnull(row.loc[key])
+                if (isinstance(null_check, np.ndarray) and null_check.any()) or (not isinstance(null_check, np.ndarray) and null_check):
                     errmsg = (
                         "Required information is missing ({}) in {}. row"
                         " (without header) of "
                         "file:\n{}".format(key, index+1, filename))
 
                     logger.warning(errmsg, extra={'identifier': filename,
                                                   'category': "inconsistency"})
```

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/utils.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/utils.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools/webui_formatter.py` & `caosadvancedtools-0.9.0/src/caosadvancedtools/webui_formatter.py`

 * *Files identical despite different names*

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools.egg-info/PKG-INFO` & `caosadvancedtools-0.9.0/src/caosadvancedtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caosadvancedtools
-Version: 0.8.0
+Version: 0.9.0
 Summary: advanced utilities for caosdb
 Author: Henrik tom Wörden
 Author-email: h.tomwoerden@indiscale.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: h5-crawler
 Provides-Extra: gitignore-parser
@@ -12,14 +12,15 @@
 
 # README
 
 ## Welcome
 
 This is the **CaosDB Advanced User Tools** repository and a part of the
 CaosDB project.
+
 This project contains tools that are beyond the typical use of
 the CaosDB python client. Especially, this includes the crawler which will
 typically be used by a data curator.
 
 ## Setup
 
 Please read the [README_SETUP.md](README_SETUP.md) for instructions on how to
```

### Comparing `caosadvancedtools-0.8.0/src/caosadvancedtools.egg-info/SOURCES.txt` & `caosadvancedtools-0.9.0/src/caosadvancedtools.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 src/caosadvancedtools/crawler.py
 src/caosadvancedtools/datainconsistency.py
 src/caosadvancedtools/datamodel_problems.py
 src/caosadvancedtools/example_cfood.py
 src/caosadvancedtools/export_related.py
 src/caosadvancedtools/guard.py
 src/caosadvancedtools/import_from_xml.py
+src/caosadvancedtools/json_schema_exporter.py
 src/caosadvancedtools/loadFiles.py
 src/caosadvancedtools/pandoc_header_tools.py
 src/caosadvancedtools/read_md_header.py
 src/caosadvancedtools/structure_mapping.py
 src/caosadvancedtools/suppressKnown.py
 src/caosadvancedtools/table_converter.py
 src/caosadvancedtools/table_export.py
```

