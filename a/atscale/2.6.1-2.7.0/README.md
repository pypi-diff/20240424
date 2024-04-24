# Comparing `tmp/atscale-2.6.1.tar.gz` & `tmp/atscale-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atscale-2.6.1.tar", last modified: Fri Feb 23 19:23:21 2024, max compression
+gzip compressed data, was "atscale-2.7.0.tar", last modified: Mon Apr 22 20:38:40 2024, max compression
```

## Comparing `atscale-2.6.1.tar` & `atscale-2.7.0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxrwx   0        0        0        0 2024-02-23 19:23:21.225015 atscale-2.6.1/
--rw-rw-rw-   0        0        0      700 2022-07-06 15:15:12.000000 atscale-2.6.1/LICENSE.md
--rw-rw-rw-   0        0        0     1455 2024-02-23 19:23:21.225015 atscale-2.6.1/PKG-INFO
--rw-rw-rw-   0        0        0      482 2023-09-18 18:36:55.000000 atscale-2.6.1/README.md
-drwxrwxrwx   0        0        0        0 2024-02-23 19:23:21.176929 atscale-2.6.1/atscale/
--rw-rw-rw-   0        0        0      395 2024-02-23 17:44:22.000000 atscale-2.6.1/atscale/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-23 19:23:21.193362 atscale-2.6.1/atscale/base/
--rw-rw-rw-   0        0        0       21 2023-07-07 20:29:28.000000 atscale-2.6.1/atscale/base/__init__.py
--rw-rw-rw-   0        0        0     6906 2023-09-07 14:56:27.000000 atscale-2.6.1/atscale/base/config.py
--rw-rw-rw-   0        0        0     8120 2024-02-09 15:04:46.000000 atscale-2.6.1/atscale/base/endpoints.py
--rw-rw-rw-   0        0        0    20388 2024-02-09 15:04:46.000000 atscale-2.6.1/atscale/base/enums.py
--rw-rw-rw-   0        0        0     2531 2024-02-09 15:04:46.000000 atscale-2.6.1/atscale/base/secrets_manager.py
--rw-rw-rw-   0        0        0    12335 2024-02-09 15:04:46.000000 atscale-2.6.1/atscale/base/templates.py
-drwxrwxrwx   0        0        0        0 2024-02-23 19:23:21.193362 atscale-2.6.1/atscale/client/
--rw-rw-rw-   0        0        0       66 2023-07-07 20:29:28.000000 atscale-2.6.1/atscale/client/__init__.py
--rw-rw-rw-   0        0        0    25512 2024-02-09 15:04:46.000000 atscale-2.6.1/atscale/client/client.py
-drwxrwxrwx   0        0        0        0 2024-02-23 19:23:21.193362 atscale-2.6.1/atscale/connection/
--rw-rw-rw-   0        0        0        0 2023-09-07 14:56:27.000000 atscale-2.6.1/atscale/connection/__init__.py
--rw-rw-rw-   0        0        0    38672 2024-02-23 17:44:22.000000 atscale-2.6.1/atscale/connection/connection.py
-drwxrwxrwx   0        0        0        0 2024-02-23 19:23:21.193362 atscale-2.6.1/atscale/data_model/
--rw-rw-rw-   0        0        0       81 2023-07-07 20:29:28.000000 atscale-2.6.1/atscale/data_model/__init__.py
--rw-rw-rw-   0        0        0   205132 2024-02-23 17:44:22.000000 atscale-2.6.1/atscale/data_model/data_model.py
--rw-rw-rw-   0        0        0    75168 2024-02-23 17:44:22.000000 atscale-2.6.1/atscale/data_model/data_model_helpers.py
-drwxrwxrwx   0        0        0        0 2024-02-23 19:23:21.193362 atscale-2.6.1/atscale/db/
--rw-rw-rw-   0        0        0       70 2023-07-07 20:29:28.000000 atscale-2.6.1/atscale/db/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-23 19:23:21.207181 atscale-2.6.1/atscale/db/connections/
--rw-rw-rw-   0        0        0      571 2023-07-07 20:29:28.000000 atscale-2.6.1/atscale/db/connections/__init__.py
--rw-rw-rw-   0        0        0     9644 2024-02-09 15:04:46.000000 atscale-2.6.1/atscale/db/connections/bigquery.py
--rw-rw-rw-   0        0        0    16607 2024-02-11 22:17:47.000000 atscale-2.6.1/atscale/db/connections/databricks.py
--rw-rw-rw-   0        0        0    10720 2024-02-09 15:04:46.000000 atscale-2.6.1/atscale/db/connections/iris.py
--rw-rw-rw-   0        0        0     9818 2024-02-09 15:04:46.000000 atscale-2.6.1/atscale/db/connections/mssql.py
--rw-rw-rw-   0        0        0     6373 2024-02-23 16:17:51.000000 atscale-2.6.1/atscale/db/connections/postgres.py
--rw-rw-rw-   0        0        0     6756 2024-02-09 15:04:46.000000 atscale-2.6.1/atscale/db/connections/redshift.py
--rw-rw-rw-   0        0        0    20790 2024-02-11 22:17:47.000000 atscale-2.6.1/atscale/db/connections/snowflake.py
--rw-rw-rw-   0        0        0    10946 2024-02-09 15:04:46.000000 atscale-2.6.1/atscale/db/connections/synapse.py
--rw-rw-rw-   0        0        0    12976 2024-02-11 22:17:47.000000 atscale-2.6.1/atscale/db/sql_connection.py
--rw-rw-rw-   0        0        0     7486 2024-02-09 15:04:46.000000 atscale-2.6.1/atscale/db/sqlalchemy_connection.py
-drwxrwxrwx   0        0        0        0 2024-02-23 19:23:21.208373 atscale-2.6.1/atscale/eda/
--rw-rw-rw-   0        0        0       72 2023-09-18 18:36:55.000000 atscale-2.6.1/atscale/eda/__init__.py
--rw-rw-rw-   0        0        0    77355 2024-02-09 21:45:12.000000 atscale-2.6.1/atscale/eda/feature_engineering.py
--rw-rw-rw-   0        0        0    21347 2024-02-09 15:04:46.000000 atscale-2.6.1/atscale/eda/linear_regression.py
--rw-rw-rw-   0        0        0    19471 2024-02-09 15:04:46.000000 atscale-2.6.1/atscale/eda/pca.py
--rw-rw-rw-   0        0        0    10825 2024-02-09 15:04:46.000000 atscale-2.6.1/atscale/eda/stats.py
-drwxrwxrwx   0        0        0        0 2024-02-23 19:23:21.208373 atscale-2.6.1/atscale/errors/
--rw-rw-rw-   0        0        0        0 2023-02-24 14:58:41.000000 atscale-2.6.1/atscale/errors/__init__.py
--rw-rw-rw-   0        0        0     4202 2024-02-09 15:04:46.000000 atscale-2.6.1/atscale/errors/atscale_errors.py
-drwxrwxrwx   0        0        0        0 2024-02-23 19:23:21.208373 atscale-2.6.1/atscale/parsers/
--rw-rw-rw-   0        0        0        0 2023-02-24 14:58:45.000000 atscale-2.6.1/atscale/parsers/__init__.py
--rw-rw-rw-   0        0        0     2116 2024-02-09 15:04:46.000000 atscale-2.6.1/atscale/parsers/data_model_parser.py
--rw-rw-rw-   0        0        0     2986 2024-02-09 15:04:46.000000 atscale-2.6.1/atscale/parsers/dataset_parser.py
--rw-rw-rw-   0        0        0     2469 2024-02-09 15:04:46.000000 atscale-2.6.1/atscale/parsers/dictionary_parser.py
--rw-rw-rw-   0        0        0    18649 2024-02-09 15:04:46.000000 atscale-2.6.1/atscale/parsers/project_parser.py
-drwxrwxrwx   0        0        0        0 2024-02-23 19:23:21.208373 atscale-2.6.1/atscale/project/
--rw-rw-rw-   0        0        0       70 2023-07-07 20:29:28.000000 atscale-2.6.1/atscale/project/__init__.py
--rw-rw-rw-   0        0        0    34132 2024-02-09 15:04:46.000000 atscale-2.6.1/atscale/project/project.py
--rw-rw-rw-   0        0        0     1003 2024-02-09 15:04:46.000000 atscale-2.6.1/atscale/project/project_helpers.py
-drwxrwxrwx   0        0        0        0 2024-02-23 19:23:21.225015 atscale-2.6.1/atscale/utils/
--rw-rw-rw-   0        0        0        0 2024-02-09 15:04:46.000000 atscale-2.6.1/atscale/utils/__init__.py
--rw-rw-rw-   0        0        0    17899 2024-02-09 15:04:46.000000 atscale-2.6.1/atscale/utils/bulk_operator_utils.py
--rw-rw-rw-   0        0        0    11619 2024-02-09 15:04:46.000000 atscale-2.6.1/atscale/utils/db_utils.py
--rw-rw-rw-   0        0        0    30934 2024-02-09 15:04:46.000000 atscale-2.6.1/atscale/utils/dimension_utils.py
--rw-rw-rw-   0        0        0    12124 2024-02-09 15:04:46.000000 atscale-2.6.1/atscale/utils/dmv_utils.py
--rw-rw-rw-   0        0        0    15723 2024-02-09 15:04:46.000000 atscale-2.6.1/atscale/utils/eda_utils.py
--rw-rw-rw-   0        0        0    53315 2024-02-11 22:17:47.000000 atscale-2.6.1/atscale/utils/feature_utils.py
--rw-rw-rw-   0        0        0     2932 2024-02-09 15:04:46.000000 atscale-2.6.1/atscale/utils/input_utils.py
--rw-rw-rw-   0        0        0     8341 2024-02-09 15:04:46.000000 atscale-2.6.1/atscale/utils/metadata_utils.py
--rw-rw-rw-   0        0        0    38955 2024-02-09 15:04:46.000000 atscale-2.6.1/atscale/utils/model_utils.py
--rw-rw-rw-   0        0        0     8996 2024-02-09 15:04:46.000000 atscale-2.6.1/atscale/utils/prediction_utils.py
--rw-rw-rw-   0        0        0    14813 2024-02-09 15:04:46.000000 atscale-2.6.1/atscale/utils/project_utils.py
--rw-rw-rw-   0        0        0    19007 2024-02-23 17:44:22.000000 atscale-2.6.1/atscale/utils/query_utils.py
--rw-rw-rw-   0        0        0    11094 2024-02-09 15:04:46.000000 atscale-2.6.1/atscale/utils/request_utils.py
--rw-rw-rw-   0        0        0     3637 2024-02-09 15:04:46.000000 atscale-2.6.1/atscale/utils/time_utils.py
--rw-rw-rw-   0        0        0    11817 2024-02-09 15:04:46.000000 atscale-2.6.1/atscale/utils/validation_utils.py
-drwxrwxrwx   0        0        0        0 2024-02-23 19:23:21.176929 atscale-2.6.1/atscale.egg-info/
--rw-rw-rw-   0        0        0     1455 2024-02-23 19:23:20.000000 atscale-2.6.1/atscale.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1912 2024-02-23 19:23:20.000000 atscale-2.6.1/atscale.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-23 19:23:20.000000 atscale-2.6.1/atscale.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1111 2024-02-23 19:23:20.000000 atscale-2.6.1/atscale.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-02-23 19:23:20.000000 atscale-2.6.1/atscale.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-23 19:23:21.225015 atscale-2.6.1/setup.cfg
--rw-rw-rw-   0        0        0     2971 2024-02-23 17:44:22.000000 atscale-2.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 20:38:40.567929 atscale-2.7.0/
+-rw-rw-rw-   0        0        0      700 2022-07-06 15:15:12.000000 atscale-2.7.0/LICENSE.md
+-rw-rw-rw-   0        0        0     1455 2024-04-22 20:38:40.567929 atscale-2.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0      482 2023-09-18 18:36:55.000000 atscale-2.7.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-22 20:38:40.503610 atscale-2.7.0/atscale/
+-rw-rw-rw-   0        0        0      395 2024-04-22 19:08:26.000000 atscale-2.7.0/atscale/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-22 20:38:40.531201 atscale-2.7.0/atscale/base/
+-rw-rw-rw-   0        0        0       21 2023-07-07 20:29:28.000000 atscale-2.7.0/atscale/base/__init__.py
+-rw-rw-rw-   0        0        0     6906 2023-09-07 14:56:27.000000 atscale-2.7.0/atscale/base/config.py
+-rw-rw-rw-   0        0        0     7965 2024-04-22 18:55:35.000000 atscale-2.7.0/atscale/base/endpoints.py
+-rw-rw-rw-   0        0        0    20388 2024-04-10 19:55:47.000000 atscale-2.7.0/atscale/base/enums.py
+-rw-rw-rw-   0        0        0     2531 2024-04-10 19:55:47.000000 atscale-2.7.0/atscale/base/secrets_manager.py
+-rw-rw-rw-   0        0        0    12335 2024-04-10 19:55:47.000000 atscale-2.7.0/atscale/base/templates.py
+drwxrwxrwx   0        0        0        0 2024-04-22 20:38:40.531878 atscale-2.7.0/atscale/client/
+-rw-rw-rw-   0        0        0       66 2023-07-07 20:29:28.000000 atscale-2.7.0/atscale/client/__init__.py
+-rw-rw-rw-   0        0        0    26960 2024-04-22 18:55:35.000000 atscale-2.7.0/atscale/client/client.py
+drwxrwxrwx   0        0        0        0 2024-04-22 20:38:40.534171 atscale-2.7.0/atscale/connection/
+-rw-rw-rw-   0        0        0        0 2023-09-07 14:56:27.000000 atscale-2.7.0/atscale/connection/__init__.py
+-rw-rw-rw-   0        0        0    38808 2024-04-22 18:55:35.000000 atscale-2.7.0/atscale/connection/connection.py
+drwxrwxrwx   0        0        0        0 2024-04-22 20:38:40.537172 atscale-2.7.0/atscale/data_model/
+-rw-rw-rw-   0        0        0       81 2023-07-07 20:29:28.000000 atscale-2.7.0/atscale/data_model/__init__.py
+-rw-rw-rw-   0        0        0   210011 2024-04-22 18:55:35.000000 atscale-2.7.0/atscale/data_model/data_model.py
+-rw-rw-rw-   0        0        0    75155 2024-04-22 18:55:35.000000 atscale-2.7.0/atscale/data_model/data_model_helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-22 20:38:40.538879 atscale-2.7.0/atscale/db/
+-rw-rw-rw-   0        0        0       70 2023-07-07 20:29:28.000000 atscale-2.7.0/atscale/db/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-22 20:38:40.545870 atscale-2.7.0/atscale/db/connections/
+-rw-rw-rw-   0        0        0      571 2023-07-07 20:29:28.000000 atscale-2.7.0/atscale/db/connections/__init__.py
+-rw-rw-rw-   0        0        0     9644 2024-04-10 19:55:47.000000 atscale-2.7.0/atscale/db/connections/bigquery.py
+-rw-rw-rw-   0        0        0    16593 2024-04-22 18:55:35.000000 atscale-2.7.0/atscale/db/connections/databricks.py
+-rw-rw-rw-   0        0        0    10732 2024-04-22 18:55:35.000000 atscale-2.7.0/atscale/db/connections/iris.py
+-rw-rw-rw-   0        0        0     9831 2024-04-22 18:55:35.000000 atscale-2.7.0/atscale/db/connections/mssql.py
+-rw-rw-rw-   0        0        0     6385 2024-04-22 18:55:35.000000 atscale-2.7.0/atscale/db/connections/postgres.py
+-rw-rw-rw-   0        0        0     6768 2024-04-22 18:55:35.000000 atscale-2.7.0/atscale/db/connections/redshift.py
+-rw-rw-rw-   0        0        0    20662 2024-04-22 18:55:35.000000 atscale-2.7.0/atscale/db/connections/snowflake.py
+-rw-rw-rw-   0        0        0    10958 2024-04-22 18:55:35.000000 atscale-2.7.0/atscale/db/connections/synapse.py
+-rw-rw-rw-   0        0        0    12976 2024-04-10 19:55:47.000000 atscale-2.7.0/atscale/db/sql_connection.py
+-rw-rw-rw-   0        0        0     7486 2024-04-10 19:55:47.000000 atscale-2.7.0/atscale/db/sqlalchemy_connection.py
+drwxrwxrwx   0        0        0        0 2024-04-22 20:38:40.548380 atscale-2.7.0/atscale/eda/
+-rw-rw-rw-   0        0        0       72 2023-09-18 18:36:55.000000 atscale-2.7.0/atscale/eda/__init__.py
+-rw-rw-rw-   0        0        0    77355 2024-04-10 19:55:47.000000 atscale-2.7.0/atscale/eda/feature_engineering.py
+-rw-rw-rw-   0        0        0    21347 2024-04-10 19:55:47.000000 atscale-2.7.0/atscale/eda/linear_regression.py
+-rw-rw-rw-   0        0        0    19471 2024-04-10 19:55:47.000000 atscale-2.7.0/atscale/eda/pca.py
+-rw-rw-rw-   0        0        0    10825 2024-04-10 19:55:47.000000 atscale-2.7.0/atscale/eda/stats.py
+drwxrwxrwx   0        0        0        0 2024-04-22 20:38:40.548380 atscale-2.7.0/atscale/errors/
+-rw-rw-rw-   0        0        0        0 2023-02-24 14:58:41.000000 atscale-2.7.0/atscale/errors/__init__.py
+-rw-rw-rw-   0        0        0     4202 2024-04-10 19:55:47.000000 atscale-2.7.0/atscale/errors/atscale_errors.py
+drwxrwxrwx   0        0        0        0 2024-04-22 20:38:40.554171 atscale-2.7.0/atscale/parsers/
+-rw-rw-rw-   0        0        0        0 2023-02-24 14:58:45.000000 atscale-2.7.0/atscale/parsers/__init__.py
+-rw-rw-rw-   0        0        0     2116 2024-04-10 19:55:47.000000 atscale-2.7.0/atscale/parsers/data_model_parser.py
+-rw-rw-rw-   0        0        0     2986 2024-04-10 19:55:47.000000 atscale-2.7.0/atscale/parsers/dataset_parser.py
+-rw-rw-rw-   0        0        0     2469 2024-04-10 19:55:47.000000 atscale-2.7.0/atscale/parsers/dictionary_parser.py
+-rw-rw-rw-   0        0        0    18649 2024-04-10 19:55:47.000000 atscale-2.7.0/atscale/parsers/project_parser.py
+drwxrwxrwx   0        0        0        0 2024-04-22 20:38:40.556304 atscale-2.7.0/atscale/project/
+-rw-rw-rw-   0        0        0       70 2023-07-07 20:29:28.000000 atscale-2.7.0/atscale/project/__init__.py
+-rw-rw-rw-   0        0        0    33818 2024-04-22 18:55:35.000000 atscale-2.7.0/atscale/project/project.py
+-rw-rw-rw-   0        0        0     1003 2024-04-10 19:55:47.000000 atscale-2.7.0/atscale/project/project_helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-22 20:38:40.566929 atscale-2.7.0/atscale/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-10 19:55:47.000000 atscale-2.7.0/atscale/utils/__init__.py
+-rw-rw-rw-   0        0        0    17899 2024-04-10 19:55:47.000000 atscale-2.7.0/atscale/utils/bulk_operator_utils.py
+-rw-rw-rw-   0        0        0    11619 2024-04-10 19:55:47.000000 atscale-2.7.0/atscale/utils/db_utils.py
+-rw-rw-rw-   0        0        0    30934 2024-04-10 19:55:47.000000 atscale-2.7.0/atscale/utils/dimension_utils.py
+-rw-rw-rw-   0        0        0    12124 2024-04-10 19:55:47.000000 atscale-2.7.0/atscale/utils/dmv_utils.py
+-rw-rw-rw-   0        0        0    15723 2024-04-10 19:55:47.000000 atscale-2.7.0/atscale/utils/eda_utils.py
+-rw-rw-rw-   0        0        0    53315 2024-04-10 19:55:47.000000 atscale-2.7.0/atscale/utils/feature_utils.py
+-rw-rw-rw-   0        0        0     2932 2024-04-10 19:55:47.000000 atscale-2.7.0/atscale/utils/input_utils.py
+-rw-rw-rw-   0        0        0     8341 2024-04-10 19:55:47.000000 atscale-2.7.0/atscale/utils/metadata_utils.py
+-rw-rw-rw-   0        0        0    38955 2024-04-10 19:55:47.000000 atscale-2.7.0/atscale/utils/model_utils.py
+-rw-rw-rw-   0        0        0     8996 2024-04-10 19:55:47.000000 atscale-2.7.0/atscale/utils/prediction_utils.py
+-rw-rw-rw-   0        0        0    14813 2024-04-10 19:55:47.000000 atscale-2.7.0/atscale/utils/project_utils.py
+-rw-rw-rw-   0        0        0    36388 2024-04-22 18:55:35.000000 atscale-2.7.0/atscale/utils/query_utils.py
+-rw-rw-rw-   0        0        0    10754 2024-04-22 18:55:35.000000 atscale-2.7.0/atscale/utils/request_utils.py
+-rw-rw-rw-   0        0        0     3637 2024-04-10 19:55:47.000000 atscale-2.7.0/atscale/utils/time_utils.py
+-rw-rw-rw-   0        0        0    11817 2024-04-10 19:55:47.000000 atscale-2.7.0/atscale/utils/validation_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-22 20:38:40.525228 atscale-2.7.0/atscale.egg-info/
+-rw-rw-rw-   0        0        0     1455 2024-04-22 20:38:40.000000 atscale-2.7.0/atscale.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1912 2024-04-22 20:38:40.000000 atscale-2.7.0/atscale.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 20:38:40.000000 atscale-2.7.0/atscale.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1124 2024-04-22 20:38:40.000000 atscale-2.7.0/atscale.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-22 20:38:40.000000 atscale-2.7.0/atscale.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-22 20:38:40.568929 atscale-2.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     2987 2024-04-22 18:55:35.000000 atscale-2.7.0/setup.py
```

### Comparing `atscale-2.6.1/LICENSE.md` & `atscale-2.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `atscale-2.6.1/PKG-INFO` & `atscale-2.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atscale
-Version: 2.6.1
+Version: 2.7.0
 Summary: The AI-Link package created by AtScale
 Home-page: https://www.atscale.com/
 Author: The AI-Link Development Team at AtScale
 Author-email: ailink@atscale.com
 License: UNKNOWN
 Project-URL: HomePage, https://www.atscale.com/
 Project-URL: Documentation, https://documentation.ai-link.atscale.com/user-guide/
```

### Comparing `atscale-2.6.1/atscale/base/config.py` & `atscale-2.7.0/atscale/base/config.py`

 * *Files identical despite different names*

### Comparing `atscale-2.6.1/atscale/base/endpoints.py` & `atscale-2.7.0/atscale/base/endpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,23 +20,18 @@
     published_project_id: str,
 ):
     return f"{atconn.engine_url}/projects/orgId/{atconn.organization}/schema/{published_project_id}"
 
 
 def _endpoint_query_view_recent_queries(
     atconn,
-    date_time: str,
-    limit: int = 21,
+    query_id: str,
 ):
-    """Returns the queries from the previous 5 minutes"""
-    return (
-        f"{atconn.engine_url}/queries/orgId/{atconn.organization}"
-        f"?limit={limit}&userId={atconn.username}&querySource=user"
-        f"&queryStarted=5m&queryDateTimeStart={date_time}"
-    )
+    """Returns the query log for the given id"""
+    return f"{atconn.engine_url}/queries/orgId/{atconn.organization}?queryId={query_id}"
 
 
 def _endpoint_warehouse_databases(
     atconn,
     warehouse_id: str,
 ):
     """<engine_url>/data-sources/ordId/<organization>"""
@@ -147,15 +142,15 @@
     return f"{atconn.engine_url}/license/capabilities"
 
 
 def _endpoint_atscale_query_submit(
     atconn,
 ):
     """Sends an AtScale query"""
-    return f"{atconn.engine_url}/query/orgId/{atconn.organization}/submit"
+    return f"{atconn.engine_url}/query/orgId/{atconn.organization}/submit/json"
 
 
 def _endpoint_design_draft_project(
     atconn,
     draft_project_id: str,
 ):
     return (
```

### Comparing `atscale-2.6.1/atscale/base/enums.py` & `atscale-2.7.0/atscale/base/enums.py`

 * *Files identical despite different names*

### Comparing `atscale-2.6.1/atscale/base/secrets_manager.py` & `atscale-2.7.0/atscale/base/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `atscale-2.6.1/atscale/base/templates.py` & `atscale-2.7.0/atscale/base/templates.py`

 * *Files identical despite different names*

### Comparing `atscale-2.6.1/atscale/client/client.py` & `atscale-2.7.0/atscale/client/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import logging
 from typing import List, Dict, Tuple, Union
+import requests
 from requests import Session
 from pandas import DataFrame
 from inspect import getfullargspec
 
 from atscale.base import config
 from atscale.connection.connection import _Connection
 from atscale.base import endpoints
@@ -94,14 +95,18 @@
             d = design_center_server_port
         elif d is None:  # if the value wasn't found in the Config file, let's use the default
             d = config.DEFAULT_DESIGN_CENTER_PORT
 
         # if we didn't find these values in the Config work above and they weren't passed in, then we didn't get enough info
         if s is None:
             raise ValueError(f"Value for server cannot be null.")
+
+        # check that we are connecting to the installer version
+        self._version_check(s)
+
         # otherwise we'll go ahead and make the connection object
         self._atconn = _Connection(s, u, p, o, d, dc, dp, v)
 
     @property
     def session(self) -> Session:
         return self._atconn.session
 
@@ -139,14 +144,41 @@
             organization,
             design_center_server_port,
             jdbc_driver_class,
             jdbc_driver_path,
             verify,
         )
 
+    def _version_check(self, server: str):
+        if server[-1] == "/":
+            server = server[:-1]
+        # try to hit the installer engine version endpoint
+        try:
+            resp = requests.get(
+                f"{server}:10502/version",
+                timeout=5,
+            )
+        except:
+            # if it didn't work then we can't reach the server for some reason
+            logger.warn("Unable to verify AtScale server version.")
+            return False
+        else:
+            if resp.ok and resp.text.startswith("202"):
+                # if that worked and the version starts with 202 then they have the installer AtScale
+                return True
+            elif resp.ok and not resp.text.startswith("202"):
+                # if that worked but the version starts with 202 then they have the container AtScale but this version of AI-Link only supports the installer version
+                logger.error(
+                    "AtScale server is runnning container version which requires upgrading to AI-Link versions 3.0.0 or greater"
+                )
+                return False
+        # if we didn't error or get a usable version then we can't reach the server for some reason
+        logger.warn("Unable to verify AtScale server version.")
+        return False
+
     def create_empty_project(
         self,
         project_name: str,
     ) -> Project:
         """Creates an empty project in the associated org
 
         Args:
```

### Comparing `atscale-2.6.1/atscale/connection/connection.py` & `atscale-2.7.0/atscale/connection/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import getpass
 import json
 import logging
 import time
 from typing import Dict, List, Tuple, Union
-import cryptocode
+from cryptography.fernet import Fernet
 import requests
 from html import unescape
 import re
 from inspect import getfullargspec
 
 from atscale.errors import atscale_errors
 from atscale.utils import request_utils, input_utils, validation_utils
 from atscale.base import endpoints, templates, enums
 
+import psycopg2
+
 logger = logging.getLogger(__name__)
 
 
 class _Connection:
     """An object responsible for the fundamental level of connection and communication to AtScale in the explicit
     realm of a user and an organization."""
 
@@ -52,16 +54,17 @@
         if len(server) > 0 and server[-1] == "/":
             server = server[:-1]
         self.session = requests.Session()
         self.session.verify = verify
         self._design_center_url = f"{server}:{design_center_server_port}"
         # use the setter so it can throw exception if username is None
         self._username: str = username
+        self.__fernet = Fernet(Fernet.generate_key())
         if password:
-            self._password = cryptocode.encrypt(password, self.username)
+            self._password = self.__fernet.encrypt(password.encode())
         else:
             self._password = None
         self.jdbc_string = None
         self.jdbc_driver_path = jdbc_driver_path
         self.jdbc_driver_class = jdbc_driver_class
         self._organization = organization
         # token as private var; see: https://docs.python.org/3/tutorial/classes.html#private-variables
@@ -194,15 +197,15 @@
         inspection = getfullargspec(self.password)
         validation_utils.validate_by_type_hints(inspection=inspection, func_params=locals())
 
         if value is None:
             raise ValueError("Password cannot be null.")
         # set token to none to require (re)connect
         self.__set_token(None)
-        self._password = cryptocode.encrypt(value, self.username)
+        self._password = self.__fernet.encrypt(value.encode())
 
     def __set_token(
         self,
         value,
     ):
         """Private method as a convenience for maintaining headers when the token is changed.
         See https://docs.python.org/3/tutorial/classes.html#private-variables
@@ -248,14 +251,24 @@
                 "Unable to determine engine url. Your token may be expired or authentication was incorrect. Please verify information and reconnect."
             )
         else:
             raise atscale_errors.AtScaleServerError(
                 "Unable to determine engine url. Please verify connection information and reconnect."
             )
 
+    def _get_postgres_conn(self, data_model):
+        conn = psycopg2.connect(
+            host=self.design_center_url.split("//")[1].split(":")[0],
+            database=data_model.project.project_name,
+            user=self._username,
+            password=self.__fernet.decrypt(self._password).decode(),
+            port=15432,
+        )
+        return conn
+
     def _submit_request(
         self,
         request_type: enums.RequestType,
         url: str,
         content_type: str = "json",
         data: str = "",
         raises: bool = False,
@@ -357,15 +370,15 @@
             url = endpoints._endpoint_auth_bearer(self)
             if not self.username:
                 username = input_utils.get_string_input(msg=f"Please enter your AtScale username: ")
             else:
                 username = self._username
 
             if self._password:
-                password = cryptocode.decrypt(self._password, self.username)
+                password = self.__fernet.decrypt(self._password).decode()
             else:
                 password = getpass.getpass(
                     prompt=f"Please enter your AtScale password for user '{username}': "
                 )
 
             response = self.session.get(
                 url,
@@ -381,17 +394,17 @@
             else:
                 self._password = None
                 resp = json.loads(response.text)
                 # this makes sense as we don't know what kind of error it is
                 raise Exception(resp["response"]["error"])
         # if we get here it worked so persist the fields we want to keep
         self._user_id = self._get_user_id_from_session()
-        # we want to pull the username from the server because auth is case insensitive which can cause problemns later
-        self._username = self._get_username()
-        self._password = cryptocode.encrypt(password, self._username)
+        # we might want to pull the username from the server because auth is case insensitive which can cause problemns later
+        # self._username = self._get_username()
+        self._password = self.__fernet.encrypt(password.encode())
 
     def _validate_license(
         self,
         specific_feature_flag=None,
     ) -> bool:
         """Validates that the AtScale server has the necessary flags in its license.
 
@@ -597,36 +610,30 @@
                 gen_aggs=gen_aggs,
                 fake_results=fake_results,
                 use_local_cache=use_local_cache,
                 use_aggregate_cache=use_aggregate_cache,
                 timeout=timeout,
             )
         )
-        attempts = 5
+        attempts = 10
         done = False
         while attempts > 0 and done == False:
             response = self._submit_request(
                 request_type=enums.RequestType.POST,
                 url=endpoints._endpoint_atscale_query_submit(self),
                 data=json_data,
             )
-            content = str(
-                response.text
-            )  # using text instead of content so we can process special characters
-            if re.search("<succeeded>(.*?)</succeeded>", content).group(1) == "false" and (
+            data = json.loads(response.text)
+            if data["metadata"]["succeeded"] == False and (
                 "Error during query planning: no such vertex in graph"
-                in re.search(
-                    "<error-message>(.*?)</error-message>", " ".join(content.split("\n"))
-                ).group(1)
+                in data["metadata"]["error-message"]
                 or "Error during query planning: key not found: AnonymousKey("
-                in re.search(
-                    "<error-message>(.*?)</error-message>", " ".join(content.split("\n"))
-                ).group(1)
+                in data["metadata"]["error-message"]
             ):
-                time.sleep(3)
+                time.sleep(1)
                 attempts = attempts - 1
             else:
                 done = True
         return response
 
     def _get_jdbc_connection(self):
         """Returns a jaydebeapi connection to the data model
@@ -642,15 +649,15 @@
         if self.jdbc_driver_path == "":
             raise atscale_errors.WorkFlowError(
                 "Cannot create jdbc connection because jdbc_driver_path is not set on the Client"
             )
         return jaydebeapi.connect(
             self.jdbc_driver_class,
             self.jdbc_string,
-            [self.username, cryptocode.decrypt(self._password, self.username)],
+            [self.username, self.__fernet.decrypt(self._password).decode()],
             self.jdbc_driver_path,
         )
 
     def _get_connected_warehouses(self) -> List[Dict]:
         """Returns metadata on all warehouses visible to the connection
 
         Returns:
```

### Comparing `atscale-2.6.1/atscale/data_model/data_model.py` & `atscale-2.7.0/atscale/data_model/data_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import logging
 from inspect import getfullargspec
 import json
+import warnings
 import pandas as pd
+from pandas import read_sql_query
+
 from typing import Callable, List, Dict, Union, Any, Tuple
 
 from atscale.errors import atscale_errors
 from atscale.db.sql_connection import SQLConnection
 from atscale.parsers import (
     data_model_parser,
     project_parser,
@@ -1083,43 +1086,48 @@
         filter_equals: Dict[str, str] = None,
         filter_greater: Dict[str, str] = None,
         filter_less: Dict[str, str] = None,
         filter_greater_or_equal: Dict[str, str] = None,
         filter_less_or_equal: Dict[str, str] = None,
         filter_not_equal: Dict[str, str] = None,
         filter_in: Dict[str, list] = None,
+        filter_not_in: Dict[str, list] = None,
         filter_between: Dict[str, tuple] = None,
         filter_like: Dict[str, str] = None,
+        filter_not_like: Dict[str, str] = None,
         filter_rlike: Dict[str, str] = None,
         filter_null: List[str] = None,
         filter_not_null: List[str] = None,
         order_by: List[Tuple[str, str]] = None,
         limit: int = None,
         comment: str = None,
         use_aggs: bool = True,
         gen_aggs: bool = True,
         fake_results: bool = False,
         use_local_cache: bool = True,
         use_aggregate_cache: bool = True,
         timeout: int = 10,
         raise_multikey_warning: bool = True,
+        use_postgres: bool = False,
     ) -> pd.DataFrame:
         """Submits a query against the published project using the supplied information and returns the results in a pandas DataFrame.
 
         Args:
             feature_list (List[str]): The list of feature query names to query.
             filter_equals (Dict[str, str], optional): Filters results based on the feature equaling the value. Defaults to None.
             filter_greater (Dict[str, str], optional): Filters results based on the feature being greater than the value. Defaults to None.
             filter_less (Dict[str, str], optional): Filters results based on the feature being less than the value. Defaults to None.
             filter_greater_or_equal (Dict[str, str], optional): Filters results based on the feature being greater or equaling the value. Defaults to None.
             filter_less_or_equal (Dict[str, str], optional): Filters results based on the feature being less or equaling the value. Defaults to None.
             filter_not_equal (Dict[str, str], optional): Filters results based on the feature not equaling the value. Defaults to None.
             filter_in (Dict[str, list], optional): Filters results based on the feature being contained in the values. Defaults to None.
+            filter_not_in (Dict[str, list], optional): Filters results based on the feature not being contained in the values. Defaults to None.
             filter_between (Dict[str, tuple], optional): Filters results based on the feature being between the values. Defaults to None.
             filter_like (Dict[str, str], optional): Filters results based on the feature being like the clause. Defaults to None.
+            filter_not_like (Dict[str, str], optional): Filters results based on the feature not being like the clause. Defaults to None.
             filter_rlike (Dict[str, str], optional): Filters results based on the feature being matched by the regular expression. Defaults to None.
             filter_null (List[str], optional): Filters results to show null values of the specified features. Defaults to None.
             filter_not_null (List[str], optional): Filters results to exclude null values of the specified features. Defaults to None.
             order_by (List[Tuple[str, str]]): The sort order for the returned dataframe. Accepts a list of tuples of the
                 feature query name and ordering respectively: [('feature_name_1', 'DESC'), ('feature_2', 'ASC') ...].
                 Defaults to None for AtScale Engine default sorting.
             limit (int, optional): Limit the number of results. Defaults to None for no limit.
@@ -1127,81 +1135,118 @@
             use_aggs (bool, optional): Whether to allow the query to use aggs. Defaults to True.
             gen_aggs (bool, optional): Whether to allow the query to generate aggs. Defaults to True.
             fake_results (bool, optional): Whether to use fake results, often used to train aggregates with queries
                 that will frequently be used. Defaults to False.
             use_local_cache (bool, optional): Whether to allow the query to use the local cache. Defaults to True.
             use_aggregate_cache (bool, optional): Whether to allow the query to use the aggregate cache. Defaults to True.
             timeout (int, optional): The number of minutes to wait for a response before timing out. Defaults to 10.
-            raise_multikey_warning (str, optional): Whether to warn if a query contains attributes that have multiple key columns. Defaults to True.
+            raise_multikey_warning (bool, optional): Whether to warn if a query contains attributes that have multiple key columns. Defaults to True.
+            use_postgres (bool, optional): Whether to use Postgres dialect for inbound query. Will only work if the current organization is configured to use Postgres inbound queries. Defaults to False.
 
         Returns:
             DataFrame: A pandas DataFrame containing the query results.
         """
         inspection = getfullargspec(self.get_data)
         validation_utils.validate_by_type_hints(inspection=inspection, func_params=locals())
 
         # check that we are using a published project
         project_helpers._check_published(self.project)
 
         # set use_aggs and gen_aggs to True because we set them in the json when using the api
         # and this stops the flags being commented into the query
-        query = query_utils._generate_atscale_query(
-            data_model=self,
-            feature_list=feature_list,
-            filter_equals=filter_equals,
-            filter_greater=filter_greater,
-            filter_less=filter_less,
-            filter_greater_or_equal=filter_greater_or_equal,
-            filter_less_or_equal=filter_less_or_equal,
-            filter_not_equal=filter_not_equal,
-            filter_in=filter_in,
-            filter_between=filter_between,
-            filter_like=filter_like,
-            filter_rlike=filter_rlike,
-            filter_null=filter_null,
-            filter_not_null=filter_not_null,
-            order_by=order_by,
-            limit=limit,
-            comment=comment,
-            raise_multikey_warning=raise_multikey_warning,
-        )
+        if not use_postgres:
+            query = query_utils._generate_atscale_query(
+                data_model=self,
+                feature_list=feature_list,
+                filter_equals=filter_equals,
+                filter_greater=filter_greater,
+                filter_less=filter_less,
+                filter_greater_or_equal=filter_greater_or_equal,
+                filter_less_or_equal=filter_less_or_equal,
+                filter_not_equal=filter_not_equal,
+                filter_in=filter_in,
+                filter_not_in=filter_not_in,
+                filter_between=filter_between,
+                filter_like=filter_like,
+                filter_not_like=filter_not_like,
+                filter_rlike=filter_rlike,
+                filter_null=filter_null,
+                filter_not_null=filter_not_null,
+                order_by=order_by,
+                limit=limit,
+                comment=comment,
+                raise_multikey_warning=raise_multikey_warning,
+            )
+            queryResponse = self.project._atconn._post_atscale_query(
+                query,
+                self.project.project_name,
+                use_aggs=use_aggs,
+                gen_aggs=gen_aggs,
+                fake_results=fake_results,
+                use_local_cache=use_local_cache,
+                use_aggregate_cache=use_aggregate_cache,
+                timeout=timeout,
+            )
 
-        queryResponse = self.project._atconn._post_atscale_query(
-            query,
-            self.project.project_name,
-            use_aggs=use_aggs,
-            gen_aggs=gen_aggs,
-            fake_results=fake_results,
-            use_local_cache=use_local_cache,
-            use_aggregate_cache=use_aggregate_cache,
-            timeout=timeout,
-        )
+            df: pd.DataFrame = request_utils.parse_rest_query_response(queryResponse)
+        else:
+            query = query_utils._generate_atscale_query_postgres(
+                data_model=self,
+                feature_list=feature_list,
+                filter_equals=filter_equals,
+                filter_greater=filter_greater,
+                filter_less=filter_less,
+                filter_greater_or_equal=filter_greater_or_equal,
+                filter_less_or_equal=filter_less_or_equal,
+                filter_not_equal=filter_not_equal,
+                filter_in=filter_in,
+                filter_not_in=filter_not_in,
+                filter_between=filter_between,
+                filter_like=filter_like,
+                filter_not_like=filter_not_like,
+                filter_rlike=filter_rlike,
+                filter_null=filter_null,
+                filter_not_null=filter_not_null,
+                order_by=order_by,
+                limit=limit,
+                comment=comment,
+                raise_multikey_warning=raise_multikey_warning,
+            )
 
-        df: pd.DataFrame = request_utils.parse_rest_query_response(queryResponse)
+            with warnings.catch_warnings():
+                warnings.filterwarnings(
+                    "ignore",
+                    message=".*pandas only supports SQLAlchemy connectable",
+                )
+                conn = self.project._atconn._get_postgres_conn(self)
+                df = read_sql_query(query, conn)
+                conn.close()
 
         model_utils._check_duplicate_features_get_data(feature_list)
 
         return df
 
     def get_data_direct(
         self,
         dbconn: SQLConnection,
         feature_list: List[str],
-        filter_equals=None,
-        filter_greater=None,
-        filter_less=None,
-        filter_greater_or_equal=None,
-        filter_less_or_equal=None,
-        filter_not_equal=None,
-        filter_in=None,
-        filter_between=None,
-        filter_like=None,
-        filter_rlike=None,
-        filter_null=None,
-        filter_not_null=None,
+        filter_equals: Dict[str, str] = None,
+        filter_greater: Dict[str, str] = None,
+        filter_less: Dict[str, str] = None,
+        filter_greater_or_equal: Dict[str, str] = None,
+        filter_less_or_equal: Dict[str, str] = None,
+        filter_not_equal: Dict[str, str] = None,
+        filter_in: Dict[str, list] = None,
+        filter_not_in: Dict[str, list] = None,
+        filter_between: Dict[str, tuple] = None,
+        filter_like: Dict[str, str] = None,
+        filter_not_like: Dict[str, str] = None,
+        filter_rlike: Dict[str, str] = None,
+        filter_null: Dict[str, str] = None,
+        filter_not_null: Dict[str, str] = None,
         order_by: List[Tuple[str, str]] = None,
         limit=None,
         comment=None,
         use_aggs=True,
         gen_aggs=True,
         raise_multikey_warning=True,
     ) -> pd.DataFrame:
@@ -1214,16 +1259,18 @@
             filter_equals (Dict[str, str], optional): A dictionary of features to filter for equality to the value. Defaults to None.
             filter_greater (Dict[str, str], optional): A dictionary of features to filter greater than the value. Defaults to None.
             filter_less (Dict[str, str], optional): A dictionary of features to filter less than the value. Defaults to None.
             filter_greater_or_equal (Dict[str, str], optional): A dictionary of features to filter greater than or equal to the value. Defaults to None.
             filter_less_or_equal (Dict[str, str], optional): A dictionary of features to filter less than or equal to the value. Defaults to None.
             filter_not_equal (Dict[str, str], optional): A dictionary of features to filter not equal to the value. Defaults to None.
             filter_in (Dict[str, list], optional): A dictionary of features to filter in a list. Defaults to None.
+            filter_not_in (Dict[str, list], optional): Filters results based on the feature not being contained in the values. Defaults to None.
             filter_between (Dict[str, tuple], optional): A dictionary of features to filter between the tuple values. Defaults to None.
             filter_like (Dict[str, str], optional): A dictionary of features to filter like the value. Defaults to None.
+            filter_not_like (Dict[str, str], optional): Filters results based on the feature not being like the clause. Defaults to None.
             filter_rlike (Dict[str, str], optional): A dictionary of features to filter rlike the value. Defaults to None.
             filter_null (List[str], optional): A list of features to filter for null. Defaults to None.
             filter_not_null (List[str], optional): A list of features to filter for not null. Defaults to None.
             order_by (List[Tuple[str, str]]): The sort order for the returned dataframe. Accepts a list of tuples of the
                 feature query name and ordering respectively: [('feature_name_1', 'DESC'), ('feature_2', 'ASC') ...].
                 Defaults to None for AtScale Engine default sorting.
             limit (int, optional): A limit to put on the query. Defaults to None.
@@ -1250,16 +1297,18 @@
                     filter_equals=filter_equals,
                     filter_greater=filter_greater,
                     filter_less=filter_less,
                     filter_greater_or_equal=filter_greater_or_equal,
                     filter_less_or_equal=filter_less_or_equal,
                     filter_not_equal=filter_not_equal,
                     filter_in=filter_in,
+                    filter_not_in=filter_not_in,
                     filter_between=filter_between,
                     filter_like=filter_like,
+                    filter_not_like=filter_not_like,
                     filter_rlike=filter_rlike,
                     filter_null=filter_null,
                     filter_not_null=filter_not_null,
                     order_by=order_by,
                     limit=limit,
                     comment=comment,
                     raise_multikey_warning=raise_multikey_warning,
@@ -1279,16 +1328,18 @@
         filter_equals: Dict[str, str] = None,
         filter_greater: Dict[str, str] = None,
         filter_less: Dict[str, str] = None,
         filter_greater_or_equal: Dict[str, str] = None,
         filter_less_or_equal: Dict[str, str] = None,
         filter_not_equal: Dict[str, str] = None,
         filter_in: Dict[str, list] = None,
+        filter_not_in: Dict[str, list] = None,
         filter_between: Dict[str, tuple] = None,
         filter_like: Dict[str, str] = None,
+        filter_not_like: Dict[str, str] = None,
         filter_rlike: Dict[str, str] = None,
         filter_null: List[str] = None,
         filter_not_null: List[str] = None,
         order_by: List[Tuple[str, str]] = None,
         limit: int = None,
         comment: str = None,
         use_aggs=True,
@@ -1302,16 +1353,18 @@
             filter_equals (Dict[str, str], optional): Filters results based on the feature equaling the value. Defaults to None.
             filter_greater (Dict[str, str], optional): Filters results based on the feature being greater than the value. Defaults to None.
             filter_less (Dict[str, str], optional): Filters results based on the feature being less than the value. Defaults to None.
             filter_greater_or_equal (Dict[str, str], optional): Filters results based on the feature being greater or equaling the value. Defaults to None.
             filter_less_or_equal (Dict[str, str], optional): Filters results based on the feature being less or equaling the value. Defaults to None.
             filter_not_equal (Dict[str, str], optional): Filters results based on the feature not equaling the value. Defaults to None.
             filter_in (Dict[str, list], optional): Filters results based on the feature being contained in the values. Defaults to None.
+            filter_not_in (Dict[str, list], optional): Filters results based on the feature not being contained in the values. Defaults to None.
             filter_between (Dict[str, tuple], optional): Filters results based on the feature being between the values. Defaults to None.
             filter_like (Dict[str, str], optional): Filters results based on the feature being like the clause. Defaults to None.
+            filter_not_like (Dict[str, str], optional): Filters results based on the feature not being like the clause. Defaults to None.
             filter_rlike (Dict[str, str], optional): Filters results based on the feature being matched by the regular expression. Defaults to None.
             filter_null (List[str], optional): Filters results to show null values of the specified features. Defaults to None.
             filter_not_null (List[str], optional): Filters results to exclude null values of the specified features. Defaults to None.
             order_by (List[Tuple[str, str]]): The sort order for the returned dataframe. Accepts a list of tuples of the
                 feature query name and ordering respectively: [('feature_name_1', 'DESC'), ('feature_2', 'ASC') ...].
                 Defaults to None for AtScale Engine default sorting.
             limit (int, optional): Limit the number of results. Defaults to None for no limit.
@@ -1335,16 +1388,18 @@
             filter_equals=filter_equals,
             filter_greater=filter_greater,
             filter_less=filter_less,
             filter_greater_or_equal=filter_greater_or_equal,
             filter_less_or_equal=filter_less_or_equal,
             filter_not_equal=filter_not_equal,
             filter_in=filter_in,
+            filter_not_in=filter_not_in,
             filter_between=filter_between,
             filter_like=filter_like,
+            filter_not_like=filter_not_like,
             filter_rlike=filter_rlike,
             filter_null=filter_null,
             filter_not_null=filter_not_null,
             order_by=order_by,
             limit=limit,
             comment=comment,
             use_aggs=use_aggs,
@@ -1385,16 +1440,18 @@
         filter_equals: Dict[str, str] = None,
         filter_greater: Dict[str, str] = None,
         filter_less: Dict[str, str] = None,
         filter_greater_or_equal: Dict[str, str] = None,
         filter_less_or_equal: Dict[str, str] = None,
         filter_not_equal: Dict[str, str] = None,
         filter_in: Dict[str, list] = None,
+        filter_not_in: Dict[str, list] = None,
         filter_between: Dict[str, tuple] = None,
         filter_like: Dict[str, str] = None,
+        filter_not_like: Dict[str, str] = None,
         filter_rlike: Dict[str, str] = None,
         filter_null: List[str] = None,
         filter_not_null: List[str] = None,
         order_by: List[Tuple[str, str]] = None,
         limit: int = None,
         comment: str = None,
         use_aggs=True,
@@ -1412,16 +1469,18 @@
             filter_equals (Dict[str, str], optional): Filters results based on the feature equaling the value. Defaults to None.
             filter_greater (Dict[str, str], optional): Filters results based on the feature being greater than the value. Defaults to None.
             filter_less (Dict[str, str], optional): Filters results based on the feature being less than the value. Defaults to None.
             filter_greater_or_equal (Dict[str, str], optional): Filters results based on the feature being greater or equaling the value. Defaults to None.
             filter_less_or_equal (Dict[str, str], optional): Filters results based on the feature being less or equaling the value. Defaults to None.
             filter_not_equal (Dict[str, str], optional): Filters results based on the feature not equaling the value. Defaults to None.
             filter_in (Dict[str, list], optional): Filters results based on the feature being contained in the values. Defaults to None.
+            filter_not_in (Dict[str, list], optional): Filters results based on the feature not being contained in the values. Defaults to None.
             filter_between (Dict[str, tuple], optional): Filters results based on the feature being between the values. Defaults to None.
             filter_like (Dict[str, str], optional): Filters results based on the feature being like the clause. Defaults to None.
+            filter_not_like (Dict[str, str], optional): Filters results based on the feature not being like the clause. Defaults to None.
             filter_rlike (Dict[str, str], optional): Filters results based on the feature being matched by the regular expression. Defaults to None.
             filter_null (List[str], optional): Filters results to show null values of the specified features. Defaults to None.
             filter_not_null (List[str], optional): Filters results to exclude null values of the specified features. Defaults to None.
             order_by (List[Tuple[str, str]]): The sort order for the returned dataframe. Accepts a list of tuples of the
                 feature query name and ordering respectively: [('feature_name_1', 'DESC'), ('feature_2', 'ASC') ...].
                 Defaults to None for AtScale Engine default sorting.
             limit (int, optional): Limit the number of results. Defaults to None for no limit.
@@ -1452,16 +1511,18 @@
                 filter_equals=filter_equals,
                 filter_greater=filter_greater,
                 filter_less=filter_less,
                 filter_greater_or_equal=filter_greater_or_equal,
                 filter_less_or_equal=filter_less_or_equal,
                 filter_not_equal=filter_not_equal,
                 filter_in=filter_in,
+                filter_not_in=filter_not_in,
                 filter_between=filter_between,
                 filter_like=filter_like,
+                filter_not_like=filter_not_like,
                 filter_rlike=filter_rlike,
                 filter_null=filter_null,
                 filter_not_null=filter_not_null,
                 order_by=order_by,
                 limit=limit,
                 comment=comment,
                 raise_multikey_warning=raise_multikey_warning,
@@ -1495,16 +1556,18 @@
         filter_equals: Dict[str, str] = None,
         filter_greater: Dict[str, str] = None,
         filter_less: Dict[str, str] = None,
         filter_greater_or_equal: Dict[str, str] = None,
         filter_less_or_equal: Dict[str, str] = None,
         filter_not_equal: Dict[str, str] = None,
         filter_in: Dict[str, list] = None,
+        filter_not_in: Dict[str, list] = None,
         filter_between: Dict[str, tuple] = None,
         filter_like: Dict[str, str] = None,
+        filter_not_like: Dict[str, str] = None,
         filter_rlike: Dict[str, str] = None,
         filter_null: List[str] = None,
         filter_not_null: List[str] = None,
         order_by: List[Tuple[str, str]] = None,
         limit: int = None,
         comment: str = None,
         use_aggs=True,
@@ -1520,16 +1583,18 @@
             filter_equals (Dict[str, str], optional): Filters results based on the feature equaling the value. Defaults to None.
             filter_greater (Dict[str, str], optional): Filters results based on the feature being greater than the value. Defaults to None.
             filter_less (Dict[str, str], optional): Filters results based on the feature being less than the value. Defaults to None.
             filter_greater_or_equal (Dict[str, str], optional): Filters results based on the feature being greater or equaling the value. Defaults to None.
             filter_less_or_equal (Dict[str, str], optional): Filters results based on the feature being less or equaling the value. Defaults to None.
             filter_not_equal (Dict[str, str], optional): Filters results based on the feature not equaling the value. Defaults to None.
             filter_in (Dict[str, list], optional): Filters results based on the feature being contained in the values. Defaults to None.
+            filter_not_in (Dict[str, list], optional): Filters results based on the feature not being contained in the values. Defaults to None.
             filter_between (Dict[str, tuple], optional): Filters results based on the feature being between the values. Defaults to None.
             filter_like (Dict[str, str], optional): Filters results based on the feature being like the clause. Defaults to None.
+            filter_not_like (Dict[str, str], optional): Filters results based on the feature not being like the clause. Defaults to None.
             filter_rlike (Dict[str, str], optional): Filters results based on the feature being matched by the regular expression. Defaults to None.
             filter_null (List[str], optional): Filters results to show null values of the specified features. Defaults to None.
             filter_not_null (List[str], optional): Filters results to exclude null values of the specified features. Defaults to None.
             order_by (List[Tuple[str, str]]): The sort order for the returned dataframe. Accepts a list of tuples of the
                 feature query name and ordering respectively: [('feature_name_1', 'DESC'), ('feature_2', 'ASC') ...].
                 Defaults to None for AtScale Engine default sorting.
             limit (int, optional): Limit the number of results. Defaults to None for no limit.
@@ -1560,16 +1625,18 @@
                 filter_equals=filter_equals,
                 filter_greater=filter_greater,
                 filter_less=filter_less,
                 filter_greater_or_equal=filter_greater_or_equal,
                 filter_less_or_equal=filter_less_or_equal,
                 filter_not_equal=filter_not_equal,
                 filter_in=filter_in,
+                filter_not_in=filter_not_in,
                 filter_between=filter_between,
                 filter_like=filter_like,
+                filter_not_like=filter_not_like,
                 filter_rlike=filter_rlike,
                 filter_null=filter_null,
                 filter_not_null=filter_not_null,
                 order_by=order_by,
                 limit=limit,
                 comment=comment,
                 raise_multikey_warning=raise_multikey_warning,
@@ -1590,24 +1657,26 @@
         model_utils._check_duplicate_features_get_data(feature_list)
 
         return df
 
     def get_database_query(
         self,
         feature_list: List[str],
-        filter_equals: Dict[str, Any] = None,
-        filter_greater: Dict[str, Any] = None,
-        filter_less: Dict[str, Any] = None,
-        filter_greater_or_equal: Dict[str, Any] = None,
-        filter_less_or_equal: Dict[str, Any] = None,
-        filter_not_equal: Dict[str, Any] = None,
-        filter_in: Dict[str, List[Any]] = None,
+        filter_equals: Dict[str, str] = None,
+        filter_greater: Dict[str, str] = None,
+        filter_less: Dict[str, str] = None,
+        filter_greater_or_equal: Dict[str, str] = None,
+        filter_less_or_equal: Dict[str, str] = None,
+        filter_not_equal: Dict[str, str] = None,
+        filter_in: Dict[str, list] = None,
+        filter_not_in: Dict[str, list] = None,
         filter_between: Dict[str, tuple] = None,
-        filter_like: Dict[str, Any] = None,
-        filter_rlike: Dict[str, Any] = None,
+        filter_like: Dict[str, str] = None,
+        filter_not_like: Dict[str, str] = None,
+        filter_rlike: Dict[str, str] = None,
         filter_null: List[str] = None,
         filter_not_null: List[str] = None,
         order_by: List[Tuple[str, str]] = None,
         limit: int = None,
         comment: str = None,
         use_aggs: bool = True,
         gen_aggs: bool = True,
@@ -1620,16 +1689,18 @@
             filter_equals (Dict[str, str], optional): A dictionary of features to filter for equality to the value. Defaults to None.
             filter_greater (Dict[str, str], optional): A dictionary of features to filter greater than the value. Defaults to None.
             filter_less (Dict[str, str], optional): A dictionary of features to filter less than the value. Defaults to None.
             filter_greater_or_equal (Dict[str, str], optional): A dictionary of features to filter greater than or equal to the value. Defaults to None.
             filter_less_or_equal (Dict[str, str], optional): A dictionary of features to filter less than or equal to the value. Defaults to None.
             filter_not_equal (Dict[str, str], optional): A dictionary of features to filter not equal to the value. Defaults to None.
             filter_in (Dict[str, list], optional): A dictionary of features to filter in a list. Defaults to None.
+            filter_not_in (Dict[str, list], optional): A dictionary of features to filter not in a list. Defaults to None.
             filter_between (Dict[str, tuple], optional): A dictionary of features to filter between the tuple values. Defaults to None.
             filter_like (Dict[str, str], optional): A dictionary of features to filter like the value. Defaults to None.
+            filter_not_like (Dict[str, str], optional): A dictionary of features to filter not like the value. Defaults to None.
             filter_rlike (Dict[str, str], optional): A dictionary of features to filter rlike the value. Defaults to None.
             filter_null (List[str], optional): A list of features to filter for null. Defaults to None.
             filter_not_null (List[str], optional): A list of features to filter for not null. Defaults to None.
             order_by (List[Tuple[str, str]]): The sort order for the returned query. Accepts a list of tuples of the
                 feature query name and ordering respectively: [('feature_name_1', 'DESC'), ('feature_2', 'ASC') ...].
                 Defaults to None for AtScale Engine default sorting.
             limit (int, optional): A limit to put on the query. Defaults to None.
@@ -1655,16 +1726,18 @@
                 filter_equals=filter_equals,
                 filter_greater=filter_greater,
                 filter_less=filter_less,
                 filter_greater_or_equal=filter_greater_or_equal,
                 filter_less_or_equal=filter_less_or_equal,
                 filter_not_equal=filter_not_equal,
                 filter_in=filter_in,
+                filter_not_in=filter_not_in,
                 filter_between=filter_between,
                 filter_like=filter_like,
+                filter_not_like=filter_not_like,
                 filter_rlike=filter_rlike,
                 filter_null=filter_null,
                 filter_not_null=filter_not_null,
                 order_by=order_by,
                 limit=limit,
                 comment=comment,
                 raise_multikey_warning=raise_multikey_warning,
```

### Comparing `atscale-2.6.1/atscale/data_model/data_model_helpers.py` & `atscale-2.7.0/atscale/data_model/data_model_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -775,15 +775,15 @@
     """
     return_dict = {}
 
     cube = [x for x in project_dict["cubes"]["cube"] if x["name"] == data_model_name][0]
     if "attributes" not in cube or "attribute" not in cube["attributes"]:
         return {}  # Meaning no features have been added yet
 
-    feature_info = [y for y in [x for x in cube["attributes"]["attribute"]]]
+    feature_info = [x for x in cube["attributes"]["attribute"]]
 
     for i in feature_info:
         return_dict[i["name"]] = {}
 
     for i in feature_info:
         return_dict[i["name"]]["caption"] = i.get("properties", {}).get("caption", "")
         return_dict[i["name"]]["atscale_type"] = _get_agg_type(i)
```

### Comparing `atscale-2.6.1/atscale/db/connections/__init__.py` & `atscale-2.7.0/atscale/db/connections/__init__.py`

 * *Files identical despite different names*

### Comparing `atscale-2.6.1/atscale/db/connections/bigquery.py` & `atscale-2.7.0/atscale/db/connections/bigquery.py`

 * *Files identical despite different names*

### Comparing `atscale-2.6.1/atscale/db/connections/databricks.py` & `atscale-2.7.0/atscale/db/connections/databricks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pandas import DataFrame
-import cryptocode
+from cryptography.fernet import Fernet
 import getpass
 from typing import Dict, List
 import logging
 import numpy as np
 from inspect import getfullargspec
 
 from atscale.errors import atscale_errors
@@ -63,17 +63,18 @@
         except ImportError as e:
             raise atscale_errors.AtScaleExtrasDependencyImportError("databricks", str(e))
 
         super().__init__(warehouse_id)
 
         inspection = getfullargspec(self.__init__)
         validation_utils.validate_by_type_hints(inspection=inspection, func_params=locals())
+        self.__fernet = Fernet(Fernet.generate_key())
 
         if token:
-            self._token = cryptocode.encrypt(token, self.platform_type_str)
+            self._token = self.__fernet.encrypt(token.encode())
         else:
             self._token = None
         self._host = host
         self._catalog = catalog
         self._schema = schema
         self._http_path = http_path
         self._port = port
@@ -93,15 +94,15 @@
     def token(
         self,
         value,
     ):
         # validate the non-null inputs
         if value is None:
             raise ValueError(f"The following required parameters are None: value")
-        self._token = cryptocode.encrypt(value, self.platform_type_str)
+        self._token = self.__fernet.encrypt(value.encode())
         self.dispose_engine()
 
     @property
     def host(self) -> str:
         return self._host
 
     @host.setter
@@ -184,19 +185,18 @@
         self._token = None
         self.dispose_engine()
 
     def _get_connection_url(self):
         from sqlalchemy.engine import URL
 
         if not self._token:
-            self._token = cryptocode.encrypt(
-                getpass.getpass(prompt="Please enter your Databricks token: "),
-                self.platform_type_str,
+            self._token = self.__fernet.encrypt(
+                getpass.getpass(prompt="Please enter your Databricks token: ").encode()
             )
-        token = cryptocode.decrypt(self._token, self.platform_type_str)
+        token = self.__fernet.decrypt(self._token).decode()
         connection_url = URL.create(
             "databricks+connector",
             username="token",
             password=token,
             host=self._host,
             port=self._port,
             database=self._catalog,
@@ -232,15 +232,15 @@
         validation_utils.validate_by_type_hints(inspection=inspection, func_params=locals())
 
         from databricks import sql
 
         connection = sql.connect(
             server_hostname=self._host,
             http_path=self._http_path,
-            access_token=cryptocode.decrypt(self._token, self.platform_type_str),
+            access_token=self.__fernet.decrypt(self._token).decode(),
         )
         cursor = connection.cursor()
 
         results = []
         for query in query_list:
             cursor.execute(query)
             result = cursor.fetchall_arrow()
@@ -282,15 +282,15 @@
             )
 
         from databricks import sql
 
         connection = sql.connect(
             server_hostname=self._host,
             http_path=self._http_path,
-            access_token=cryptocode.decrypt(self._token, self.platform_type_str),
+            access_token=self.__fernet.decrypt(self._token).decode(),
         )
         cursor = connection.cursor()
 
         tables = cursor.tables(
             table_name=table_name, schema_name=self.schema, catalog_name=self.catalog
         ).fetchall()
         cursor.execute(f"USE CATALOG {self.catalog}")
```

### Comparing `atscale-2.6.1/atscale/db/connections/iris.py` & `atscale-2.7.0/atscale/db/connections/iris.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import getpass
 from typing import Dict
-import cryptocode
+from cryptography.fernet import Fernet
 import logging
 from pandas import DataFrame, read_sql_query
 from inspect import getfullargspec
 
 from atscale.utils import validation_utils
 from atscale.errors import atscale_errors
 from atscale.db.sql_connection import SQLConnection
@@ -69,16 +69,18 @@
 
         self.username = username
         self.host = host
         self.namespace = namespace
         self.driver = driver
         self.schema = schema
         self.port = port
+        self.__fernet = Fernet(Fernet.generate_key())
+
         if password:
-            self._password = cryptocode.encrypt(password, self.platform_type_str)
+            self._password = self.__fernet.encrypt(password.encode())
         else:
             self._password = None
 
         try:
             validation_connection = pyodbc.connect(self._get_connection_url(), autommit=True)
             validation_connection.close()
         except:
@@ -93,15 +95,15 @@
     def password(
         self,
         value,
     ):
         # validate the non-null inputs
         if value is None:
             raise ValueError(f"The following required parameters are None: value")
-        self._password = cryptocode.encrypt(value, self.platform_type_str)
+        self._password = self.__fernet.encrypt(value.encode())
 
     @property
     def _database(self):
         return self.namespace
 
     @property
     def _schema(self):
@@ -109,19 +111,18 @@
 
     def clear_auth(self):
         """Clears any authentication information, like password or token from the connection."""
         self._password = None
 
     def _get_connection_url(self):
         if not self._password:
-            self._password = cryptocode.encrypt(
-                getpass.getpass(prompt="Please enter your IRIS password: "),
-                self.platform_type_str,
+            self._password = self.__fernet.encrypt(
+                getpass.getpass(prompt="Please enter your IRIS password: ").encode()
             )
-        password = cryptocode.decrypt(self._password, self.platform_type_str)
+        password = self.__fernet.decrypt(self._password).decode()
         connection_url = f"DRIVER={self.driver};SERVER={self.host};PORT={self.port};DATABASE={self.namespace};UID={self.username};PWD={password}"
         return connection_url
 
     @staticmethod
     def _format_types(
         dataframe: DataFrame,
     ) -> Dict:
```

### Comparing `atscale-2.6.1/atscale/db/connections/mssql.py` & `atscale-2.7.0/atscale/db/connections/mssql.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import getpass
-import cryptocode
+from cryptography.fernet import Fernet
 import logging
 from inspect import getfullargspec
 
 from atscale.errors import atscale_errors
 from atscale.utils import validation_utils
 from atscale.db.sqlalchemy_connection import SQLAlchemyConnection
 
@@ -72,16 +72,18 @@
 
         self._username = username
         self._host = host
         self._database = database
         self._driver = driver
         self._schema = schema
         self._port = port
+        self.__fernet = Fernet(Fernet.generate_key())
+
         if password:
-            self._password = cryptocode.encrypt(password, self.platform_type_str)
+            self._password = self.__fernet.encrypt(password.encode())
         else:
             self._password = None
 
         try:
             validation_connection = self.engine.connect()
             validation_connection.close()
             self.dispose_engine()
@@ -187,15 +189,15 @@
     def password(
         self,
         value,
     ):
         # validate the non-null inputs
         if value is None:
             raise ValueError(f"The following required parameters are None: value")
-        self._password = cryptocode.encrypt(value, self.platform_type_str)
+        self._password = self.__fernet.encrypt(value.encode())
         self.dispose_engine()
 
     @property
     def engine(self):
         from sqlalchemy import create_engine
 
         if self._engine is not None:
@@ -213,19 +215,18 @@
         self._password = None
         self.dispose_engine()
 
     def _get_connection_url(self):
         from sqlalchemy.engine import URL
 
         if not self._password:
-            self._password = cryptocode.encrypt(
-                getpass.getpass(prompt="Please enter your Synapse password: "),
-                self.platform_type_str,
+            self._password = self.__fernet.encrypt(
+                getpass.getpass(prompt="Please enter your Synapse password: ").encode(),
             )
-        password = cryptocode.decrypt(self._password, self.platform_type_str)
+        password = self.__fernet.decrypt(self._password).decode()
 
         # Below is an example of passing through the exact string to pyodbc. I'm using the sqlalchemy URL to pass in autocommit becuase of an azure issue.
         # There may be another way to do that with the pass through approach but not sure, as that has to be set not just on connectino but driver I think,
         # according to docs.
         # connection_string = f'DRIVER={{{self.driver}}};SERVER={self.host};PORT={self.port};DATABASE={self.database};UID={self.username};PWD={password}'
         # connection_url = URL.create("mssql+pyodbc", query={"odbc_connect": connection_string})
```

### Comparing `atscale-2.6.1/atscale/db/connections/postgres.py` & `atscale-2.7.0/atscale/db/connections/postgres.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import getpass
-import cryptocode
+from cryptography.fernet import Fernet
 from inspect import getfullargspec
 import logging
 
 from atscale.errors import atscale_errors
 from atscale.db.sqlalchemy_connection import SQLAlchemyConnection
 from atscale.utils import validation_utils
 
@@ -52,16 +52,18 @@
         validation_utils.validate_by_type_hints(inspection=inspection, func_params=locals())
 
         self._username = username
         self._host = host
         self._database = database
         self._schema = schema
         self._port = port
+        self.__fernet = Fernet(Fernet.generate_key())
+
         if password:
-            self._password = cryptocode.encrypt(password, self.platform_type_str)
+            self._password = self.__fernet.encrypt(password.encode())
         else:
             self._password = None
 
         try:
             validation_connection = self.engine.connect()
             validation_connection.close()
             self.dispose_engine()
@@ -152,15 +154,15 @@
     def password(
         self,
         value,
     ):
         # validate the non-null inputs
         if value is None:
             raise ValueError(f"The following required parameters are None: value")
-        self._password = cryptocode.encrypt(value, self.platform_type_str)
+        self._password = self.__fernet.encrypt(value.encode())
         self.dispose_engine()
 
     def clear_auth(self):
         """Clears any authentication information, like password or token from the connection."""
         self._password = None
         self.dispose_engine()
 
@@ -168,19 +170,18 @@
     def _column_quote():
         return '"'
 
     def _get_connection_url(self):
         from sqlalchemy.engine import URL
 
         if not self._password:
-            self._password = cryptocode.encrypt(
-                getpass.getpass(prompt="Please enter your password for Postgres: "),
-                self.platform_type_str,
+            self._password = self.__fernet.encrypt(
+                getpass.getpass(prompt="Please enter your password for Postgres: ").encode()
             )
-        password = cryptocode.decrypt(self._password, self.platform_type_str)
+        password = self.__fernet.decrypt(self._password).decode()
         connection_url = URL.create(
             "postgresql",
             username=self._username,
             password=password,
             host=self._host,
             port=self._port,
             database=self._database,
```

### Comparing `atscale-2.6.1/atscale/db/connections/redshift.py` & `atscale-2.7.0/atscale/db/connections/redshift.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import getpass
-import cryptocode
+from cryptography.fernet import Fernet
 from inspect import getfullargspec
 import logging
 
 from atscale.errors import atscale_errors
 from atscale.db.sqlalchemy_connection import SQLAlchemyConnection
 from atscale.utils import validation_utils
 
@@ -52,16 +52,18 @@
         validation_utils.validate_by_type_hints(inspection=inspection, func_params=locals())
 
         self._username = username
         self._host = host
         self._database = database
         self._schema = schema
         self._port = port
+        self.__fernet = Fernet(Fernet.generate_key())
+
         if password:
-            self._password = cryptocode.encrypt(password, self.platform_type_str)
+            self._password = self.__fernet.encrypt(password.encode())
         else:
             self._password = None
 
         try:
             validation_connection = self.engine.connect()
             validation_connection.close()
             self.dispose_engine()
@@ -152,15 +154,15 @@
     def password(
         self,
         value,
     ):
         # validate the non-null inputs
         if value is None:
             raise ValueError(f"The following required parameters are None: value")
-        self._password = cryptocode.encrypt(value, self.platform_type_str)
+        self._password = self.__fernet.encrypt(value.encode())
         self.dispose_engine()
 
     @property
     def engine(self):
         if self._engine is not None:
             return self._engine
 
@@ -175,19 +177,18 @@
         self._password = None
         self.dispose_engine()
 
     def _get_connection_url(self):
         from sqlalchemy.engine import URL
 
         if not self._password:
-            self._password = cryptocode.encrypt(
-                getpass.getpass(prompt="Please enter your password for Redshift: "),
-                self.platform_type_str,
+            self._password = self.__fernet.encrypt(
+                getpass.getpass(prompt="Please enter your password for Redshift: ").encode()
             )
-        password = cryptocode.decrypt(self._password, self.platform_type_str)
+        password = self.__fernet.decrypt(self._password).decode()
         connection_url = URL.create(
             "redshift+redshift_connector",
             username=self._username,
             password=password,
             host=self._host,
             port=self._port,
             database=self._database,
```

### Comparing `atscale-2.6.1/atscale/db/connections/snowflake.py` & `atscale-2.7.0/atscale/db/connections/snowflake.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import getpass
-import cryptocode
+from cryptography.fernet import Fernet
 import logging
 import ssl
 from typing import Dict, List
 import pandas as pd
 from inspect import getfullargspec
 
 from atscale.errors import atscale_errors
@@ -67,35 +67,36 @@
         validation_utils.validate_by_type_hints(inspection=inspection, func_params=locals())
 
         self._username = username
         self._account = account
         self._warehouse = warehouse
         self._database = database
         self._schema = schema
+        self.__fernet = Fernet(Fernet.generate_key())
 
         auth_methods = []
         if token:
-            self._token = cryptocode.encrypt(token, self.platform_type_str)
+            self._token = self.__fernet.encrypt(token.encode())
             auth_methods.append("token")
         else:
             self._token = None
         if private_key:
             try:
-                self._private_key = cryptocode.encrypt(
-                    ssl.DER_cert_to_PEM_cert(private_key), self.platform_type_str
+                self._private_key = self.__fernet.encrypt(
+                    ssl.DER_cert_to_PEM_cert(private_key).encode()
                 )
             except:
                 raise ValueError(
                     "Error parsing private key, make sure it is a valid DER encoded byte string"
                 )
             auth_methods.append("private_key")
         else:
             self._private_key = None
         if password:
-            self._password = cryptocode.encrypt(password, self.platform_type_str)
+            self._password = self.__fernet.encrypt(password.encode())
             auth_methods.append("password")
         else:
             self._password = None
         if len(auth_methods) > 1:
             logger.warning(
                 f"Multiple auth methods passed: {auth_methods} this may result in unintended authorization behavior."
             )
@@ -193,15 +194,15 @@
     def password(
         self,
         value,
     ):
         # validate the non-null inputs
         if value is None:
             raise ValueError(f"The following required parameters are None: value")
-        self._password = cryptocode.encrypt(value, self.platform_type_str)
+        self._password = self.__fernet.encrypt(value.encode())
         self.dispose_engine()
 
     @property
     def private_key(self) -> str:
         raise atscale_errors.UnsupportedOperationException("Private Key cannot be retrieved.")
 
     @private_key.setter
@@ -209,17 +210,15 @@
         self,
         value,
     ):
         # validate the non-null inputs
         if value is None:
             raise ValueError(f"The following required parameters are None: value")
         try:
-            self._private_key = cryptocode.encrypt(
-                ssl.DER_cert_to_PEM_cert(value), self.platform_type_str
-            )
+            self._private_key = self.__fernet.encrypt(ssl.DER_cert_to_PEM_cert(value).encode())
         except:
             raise ValueError(
                 "Error parsing private key, make sure it is a valid DER encoded byte string"
             )
         self.dispose_engine()
 
     @property
@@ -230,15 +229,15 @@
     def token(
         self,
         value,
     ):
         # validate the non-null inputs
         if value is None:
             raise ValueError(f"The following required parameters are None: value")
-        self._token = cryptocode.encrypt(value, self.platform_type_str)
+        self._token = self.__fernet.encrypt(value.encode())
         self.dispose_engine()
 
     @property
     def role(self) -> str:
         return self._role
 
     @role.setter
@@ -281,25 +280,23 @@
     def _lin_reg_str():
         return "::FLOAT AS vals UNION ALL "
 
     def _get_connection_url(self):
         from sqlalchemy.engine import URL
 
         if self._authenticator == "oauth" and not self._token:
-            self._token = cryptocode.encrypt(
-                getpass.getpass(prompt="Please enter your oauth token for Snowflake: "),
-                self.platform_type_str,
+            self._token = self.__fernet.encrypt(
+                getpass.getpass(prompt="Please enter your oauth token for Snowflake: ").encode()
             )
         if not self._private_key and not self._token:
             if not self._password:
-                self._password = cryptocode.encrypt(
-                    getpass.getpass(prompt="Please enter your password for Snowflake: "),
-                    self.platform_type_str,
+                self._password = self.__fernet.encrypt(
+                    getpass.getpass(prompt="Please enter your password for Snowflake: ").encode()
                 )
-            password = cryptocode.decrypt(self._password, self.platform_type_str)
+            password = self.__fernet.decrypt(self._password).decode()
             connection_url = URL.create(
                 "snowflake",
                 username=self._username,
                 password=password,
                 host=self._account,
                 database=self._database + "/" + self._schema,
             )
@@ -313,18 +310,18 @@
         return connection_url
 
     def _get_connection_parameters(self):
         parameters = {"warehouse": self._warehouse, "authenticator": self._authenticator}
         if self._role:
             parameters["role"] = self._role
         if self._token:
-            parameters["token"] = cryptocode.decrypt(self._token, self.platform_type_str)
+            parameters["token"] = self.__fernet.decrypt(self._token).decode()
         if self._private_key:
             parameters["private_key"] = ssl.PEM_cert_to_DER_cert(
-                cryptocode.decrypt(self._private_key, self.platform_type_str)
+                self.__fernet.decrypt(self._private_key).decode()
             )
         return parameters
 
     def _fix_table_name(
         self,
         table_name: str,
     ):
```

### Comparing `atscale-2.6.1/atscale/db/connections/synapse.py` & `atscale-2.7.0/atscale/db/connections/synapse.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import getpass
 from typing import Dict
-import cryptocode
+from cryptography.fernet import Fernet
 import logging
 from pandas import DataFrame, read_sql_query
 from inspect import getfullargspec
 
 from atscale.utils import validation_utils
 from atscale.errors import atscale_errors
 from atscale.db.sql_connection import SQLConnection
@@ -69,16 +69,18 @@
 
         self.username = username
         self.host = host
         self.database = database
         self.driver = driver
         self.schema = schema
         self.port = port
+        self.__fernet = Fernet(Fernet.generate_key())
+
         if password:
-            self._password = cryptocode.encrypt(password, self.platform_type_str)
+            self._password = self.__fernet.encrypt(password.encode())
         else:
             self._password = None
 
         try:
             validation_connection = po.connect(self._get_connection_url(), autommit=True)
             validation_connection.close()
         except:
@@ -93,15 +95,15 @@
     def password(
         self,
         value,
     ):
         # validate the non-null inputs
         if value is None:
             raise ValueError(f"The following required parameters are None: value")
-        self._password = cryptocode.encrypt(value, self.platform_type_str)
+        self._password = self.__fernet.encrypt(value.encode())
 
     @property
     def _database(self) -> str:
         return self.database
 
     @property
     def _schema(self) -> str:
@@ -109,19 +111,18 @@
 
     def clear_auth(self):
         """Clears any authentication information, like password or token from the connection."""
         self._password = None
 
     def _get_connection_url(self):
         if not self._password:
-            self._password = cryptocode.encrypt(
-                getpass.getpass(prompt="Please enter your Synapse password: "),
-                self.platform_type_str,
+            self._password = self.__fernet.encrypt(
+                getpass.getpass(prompt="Please enter your Synapse password: ").encode()
             )
-        password = cryptocode.decrypt(self._password, self.platform_type_str)
+        password = self.__fernet.decrypt(self._password).decode()
         connection_url = f"DRIVER={self.driver};SERVER={self.host};PORT={self.port};DATABASE={self.database};UID={self.username};PWD={password}"
         return connection_url
 
     @staticmethod
     def _format_types(
         dataframe: DataFrame,
     ) -> Dict:
```

### Comparing `atscale-2.6.1/atscale/db/sql_connection.py` & `atscale-2.7.0/atscale/db/sql_connection.py`

 * *Files identical despite different names*

### Comparing `atscale-2.6.1/atscale/db/sqlalchemy_connection.py` & `atscale-2.7.0/atscale/db/sqlalchemy_connection.py`

 * *Files identical despite different names*

### Comparing `atscale-2.6.1/atscale/eda/feature_engineering.py` & `atscale-2.7.0/atscale/eda/feature_engineering.py`

 * *Files identical despite different names*

### Comparing `atscale-2.6.1/atscale/eda/linear_regression.py` & `atscale-2.7.0/atscale/eda/linear_regression.py`

 * *Files identical despite different names*

### Comparing `atscale-2.6.1/atscale/eda/pca.py` & `atscale-2.7.0/atscale/eda/pca.py`

 * *Files identical despite different names*

### Comparing `atscale-2.6.1/atscale/eda/stats.py` & `atscale-2.7.0/atscale/eda/stats.py`

 * *Files identical despite different names*

### Comparing `atscale-2.6.1/atscale/errors/atscale_errors.py` & `atscale-2.7.0/atscale/errors/atscale_errors.py`

 * *Files identical despite different names*

### Comparing `atscale-2.6.1/atscale/parsers/data_model_parser.py` & `atscale-2.7.0/atscale/parsers/data_model_parser.py`

 * *Files identical despite different names*

### Comparing `atscale-2.6.1/atscale/parsers/dataset_parser.py` & `atscale-2.7.0/atscale/parsers/dataset_parser.py`

 * *Files identical despite different names*

### Comparing `atscale-2.6.1/atscale/parsers/dictionary_parser.py` & `atscale-2.7.0/atscale/parsers/dictionary_parser.py`

 * *Files identical despite different names*

### Comparing `atscale-2.6.1/atscale/parsers/project_parser.py` & `atscale-2.7.0/atscale/parsers/project_parser.py`

 * *Files identical despite different names*

### Comparing `atscale-2.6.1/atscale/project/project.py` & `atscale-2.7.0/atscale/project/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -716,28 +716,23 @@
                 else:
                     raise atscale_errors.DependentMeasureException(
                         f"The following measures were protected, so the deletion was aborted: {features_to_delete}"
                     )
         self._update_project(project_dict=temp_json, publish=publish)
 
     def get_data_models(self) -> List[Dict[str, str]]:
-        """Prints all Data Models that are visible for the associated Project. Returns a list of dicts
-            for each of the listed Projects. List index should match printed index.
+        """Returns a list of dicts for each of the data models in the project.
 
         Returns:
             List[Dict[str,str]]: List of 'id':'name' pairs of available Data Models.
         """
 
         data_model_dict_list = project_parser.get_data_models(self._get_dict())
         data_model_dict_list = sorted(data_model_dict_list, key=lambda d: d["name"].upper())
 
-        print("Note: Data Model ID is expected in Data Model constructor.")
-        for i, dct in enumerate(data_model_dict_list):
-            print(f"Index:{i} ID: {dct['id']}: Name: {dct['name']}")
-
         return data_model_dict_list
 
     def get_connected_warehouse(self) -> str:
         """Returns the warehouse id utilized in this project
 
         Returns:
             str: the warehouse id
```

### Comparing `atscale-2.6.1/atscale/project/project_helpers.py` & `atscale-2.7.0/atscale/project/project_helpers.py`

 * *Files identical despite different names*

### Comparing `atscale-2.6.1/atscale/utils/bulk_operator_utils.py` & `atscale-2.7.0/atscale/utils/bulk_operator_utils.py`

 * *Files identical despite different names*

### Comparing `atscale-2.6.1/atscale/utils/db_utils.py` & `atscale-2.7.0/atscale/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `atscale-2.6.1/atscale/utils/dimension_utils.py` & `atscale-2.7.0/atscale/utils/dimension_utils.py`

 * *Files identical despite different names*

### Comparing `atscale-2.6.1/atscale/utils/dmv_utils.py` & `atscale-2.7.0/atscale/utils/dmv_utils.py`

 * *Files identical despite different names*

### Comparing `atscale-2.6.1/atscale/utils/eda_utils.py` & `atscale-2.7.0/atscale/utils/eda_utils.py`

 * *Files identical despite different names*

### Comparing `atscale-2.6.1/atscale/utils/feature_utils.py` & `atscale-2.7.0/atscale/utils/feature_utils.py`

 * *Files identical despite different names*

### Comparing `atscale-2.6.1/atscale/utils/input_utils.py` & `atscale-2.7.0/atscale/utils/input_utils.py`

 * *Files identical despite different names*

### Comparing `atscale-2.6.1/atscale/utils/metadata_utils.py` & `atscale-2.7.0/atscale/utils/metadata_utils.py`

 * *Files identical despite different names*

### Comparing `atscale-2.6.1/atscale/utils/model_utils.py` & `atscale-2.7.0/atscale/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `atscale-2.6.1/atscale/utils/prediction_utils.py` & `atscale-2.7.0/atscale/utils/prediction_utils.py`

 * *Files identical despite different names*

### Comparing `atscale-2.6.1/atscale/utils/project_utils.py` & `atscale-2.7.0/atscale/utils/project_utils.py`

 * *Files identical despite different names*

### Comparing `atscale-2.6.1/atscale/utils/request_utils.py` & `atscale-2.7.0/atscale/utils/request_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -240,34 +240,24 @@
 
     Args:
        response (requests.Response): The response used to formulate the dataframe that the function returns.
 
     Returns:
         pandas.DataFrame: the parsed query response
     """
-    content = str(
-        response.text
-    )  # using text instead of content so we can process special characters
-    if re.search("<succeeded>(.*?)</succeeded>", content).group(1) == "false":
-        raise atscale_errors.AtScaleServerError(
-            re.search("<error-message>(.*?)</error-message>", " ".join(content.split("\n"))).group(
-                1
-            )
-        )
-    column_names = re.findall("<name>(.*?)</name>", content)
-    row_text = re.findall("<row>(.*?)</row>", content)
-    rows = []
-    for row in row_text:
-        row = row.replace('<column null="true"/>', "<column></column>")
-        cells = re.findall("<column>(.*?)</column>", row)
-        rows.append(cells)
-    df = pd.DataFrame(data=rows, columns=column_names)
+    data = json.loads(response.text)
+    if data["metadata"]["succeeded"] == False:
+        raise atscale_errors.AtScaleServerError(data["metadata"]["error-message"])
+    column_types = {}
+    for column in data["metadata"]["columns"]:
+        column_types[column["name"]] = column["type"]
+    df = pd.DataFrame(columns=[x["name"] for x in data["metadata"]["columns"]], data=data["data"])
     for column in df.columns:
         df[column] = pd.to_numeric(df[column].values, errors="ignore")
-        if not pd.api.types.is_numeric_dtype(df[column]):
+        if "date" in column_types[column].lower() or "time" in column_types[column].lower():
             try:
                 first_value_index = df[column].first_valid_index()
                 # leave as nan if all null
                 if first_value_index is not None:
                     # If date parse fails, just pass and leave the column as is
                     # infer_datetime_format is needed prior to Pandas 2.0.0 we can remove this if that becomes our required version
                     if int(pd.__version__.split(".")[0]) == 1:
```

### Comparing `atscale-2.6.1/atscale/utils/time_utils.py` & `atscale-2.7.0/atscale/utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `atscale-2.6.1/atscale/utils/validation_utils.py` & `atscale-2.7.0/atscale/utils/validation_utils.py`

 * *Files identical despite different names*

### Comparing `atscale-2.6.1/atscale.egg-info/PKG-INFO` & `atscale-2.7.0/atscale.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atscale
-Version: 2.6.1
+Version: 2.7.0
 Summary: The AI-Link package created by AtScale
 Home-page: https://www.atscale.com/
 Author: The AI-Link Development Team at AtScale
 Author-email: ailink@atscale.com
 License: UNKNOWN
 Project-URL: HomePage, https://www.atscale.com/
 Project-URL: Documentation, https://documentation.ai-link.atscale.com/user-guide/
```

### Comparing `atscale-2.6.1/atscale.egg-info/SOURCES.txt` & `atscale-2.7.0/atscale.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atscale-2.6.1/atscale.egg-info/requires.txt` & `atscale-2.7.0/atscale.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 pandas
 requests>=2.0.0
 aenum
-cryptocode>=0.1
+cryptography
+psycopg2-binary
 
 [databricks]
 databricks-sql-connector
 sqlalchemy-databricks>=0.1.0
 
 [dev]
 pandas-gbq!=0.17.6
```

### Comparing `atscale-2.6.1/setup.py` & `atscale-2.7.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 # read the contents of your README file
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 NAME = "atscale"
-VERSION = "2.6.1"
+VERSION = "2.7.0"
 DESCRIPTION = "The AI-Link package created by AtScale"
 URL = "https://www.atscale.com/"
 AUTHOR = "The AI-Link Development Team at AtScale"
 AUTHOR_EMAIL = "ailink@atscale.com"
 REQUIRES_PYTHON = ">=3.8.0"
-REQUIRED = ["pandas", "requests>=2.0.0", "aenum", "cryptocode>=0.1"]
+REQUIRED = ["pandas", "requests>=2.0.0", "aenum", "cryptography", "psycopg2-binary"]
 
 SPARK_REQUIRED = ["pyspark>=3.4.0"]
 JDBC_REQUIRED = ["jaydebeapi>=1.2.3"]
 
 SQLALCHEMY_REQUIRED = ["sqlalchemy>=1.4.29,<2.0"]
 PYODBC_REQUIRED = ["pyodbc>=4.0.27"]
```

