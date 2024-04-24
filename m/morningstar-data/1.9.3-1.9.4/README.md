# Comparing `tmp/morningstar_data-1.9.3.tar.gz` & `tmp/morningstar_data-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morningstar_data-1.9.3.tar", max compression
+gzip compressed data, was "morningstar_data-1.9.4.tar", max compression
```

## Comparing `morningstar_data-1.9.3.tar` & `morningstar_data-1.9.4.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0      558 2024-04-15 19:48:03.045795 morningstar_data-1.9.3/LICENSE
--rw-r--r--   0        0        0    11417 2024-04-15 19:48:03.045795 morningstar_data-1.9.3/README.md
--rw-r--r--   0        0        0      168 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/__init__.py
--rw-r--r--   0        0        0      598 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/_base.py
--rw-r--r--   0        0        0     4233 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/_utils.py
--rw-r--r--   0        0        0       82 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/_version.py
--rw-r--r--   0        0        0       61 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/datalake/__init__.py
--rw-r--r--   0        0        0       62 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/datalake/_data_objects/__init__.py
--rw-r--r--   0        0        0      557 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/datalake/_data_objects/_file.py
--rw-r--r--   0        0        0      763 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/datalake/_data_objects/_table.py
--rw-r--r--   0        0        0      996 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/datalake/_data_objects/csvfile.py
--rw-r--r--   0        0        0     2202 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/datalake/_data_objects/temptable.py
--rw-r--r--   0        0        0      544 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/datalake/_error_messages.py
--rw-r--r--   0        0        0      937 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/datalake/_exceptions.py
--rw-r--r--   0        0        0     5604 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/datalake/base.py
--rw-r--r--   0        0        0     1171 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/__init__.py
--rw-r--r--   0        0        0     2432 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_api.py
--rw-r--r--   0        0        0      179 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_backend_apis/__init__.py
--rw-r--r--   0        0        0     2075 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_backend_apis/_delivery_backend.py
--rw-r--r--   0        0        0     4790 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_backend_apis/_holdings_backend.py
--rw-r--r--   0        0        0     3372 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_backend_apis/_signed_url_backend.py
--rw-r--r--   0        0        0     3795 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_base_api.py
--rw-r--r--   0        0        0     5076 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_config.py
--rw-r--r--   0        0        0     1999 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_config_key.py
--rw-r--r--   0        0        0     7854 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_core_api.py
--rw-r--r--   0        0        0      197 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_data_objects/__init__.py
--rw-r--r--   0        0        0     2296 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_data_objects/_custom_data_points_types.py
--rw-r--r--   0        0        0    26798 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_data_objects/_data_points_object.py
--rw-r--r--   0        0        0     7574 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_data_objects/_investments_object.py
--rw-r--r--   0        0        0     2887 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_data_point.py
--rw-r--r--   0        0        0     1453 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_data_type.py
--rw-r--r--   0        0        0     1614 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_decorator.py
--rw-r--r--   0        0        0    14042 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_error_messages.py
--rw-r--r--   0        0        0     3711 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_exceptions.py
--rw-r--r--   0        0        0        0 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_investment/__init__.py
--rw-r--r--   0        0        0     4620 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_investment/_asset_flow_data.py
--rw-r--r--   0        0        0     1560 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_investment/_common.py
--rw-r--r--   0        0        0     9136 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_investment/_data.py
--rw-r--r--   0        0        0     8526 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_investment/_normal_data.py
--rw-r--r--   0        0        0     5127 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_investment/_peer_group_data.py
--rw-r--r--   0        0        0      162 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_portfolio/__init__.py
--rw-r--r--   0        0        0     1273 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_portfolio/_common.py
--rw-r--r--   0        0        0     8263 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_portfolio/_portfolio_holdings_entity.py
--rw-r--r--   0        0        0     8023 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_portfolio/_portfolio_settings.py
--rw-r--r--   0        0        0      719 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_portfolio/_portfolio_type.py
--rw-r--r--   0        0        0    11071 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_portfolio_data_set.py
--rw-r--r--   0        0        0     3356 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_utils.py
--rw-r--r--   0        0        0    13081 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/asset_flow.py
--rw-r--r--   0        0        0    16435 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/custom_database.py
--rw-r--r--   0        0        0     1513 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/data_type.py
--rw-r--r--   0        0        0    45132 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/holdings.py
--rw-r--r--   0        0        0    18226 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/investment.py
--rw-r--r--   0        0        0    32429 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/lookup.py
--rw-r--r--   0        0        0     6154 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/peer_group.py
--rw-r--r--   0        0        0    19460 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/performance_report.py
--rw-r--r--   0        0        0    37410 2024-04-15 19:48:03.061795 morningstar_data-1.9.3/morningstar_data/direct/portfolio.py
--rw-r--r--   0        0        0    11511 2024-04-15 19:48:03.061795 morningstar_data-1.9.3/morningstar_data/direct/returns.py
--rw-r--r--   0        0        0      455 2024-04-15 19:48:03.061795 morningstar_data-1.9.3/morningstar_data/direct/user_items/__init__.py
--rw-r--r--   0        0        0      582 2024-04-15 19:48:03.061795 morningstar_data-1.9.3/morningstar_data/direct/user_items/_utils.py
--rw-r--r--   0        0        0     7910 2024-04-15 19:48:03.061795 morningstar_data-1.9.3/morningstar_data/direct/user_items/data_set.py
--rw-r--r--   0        0        0    13091 2024-04-15 19:48:03.061795 morningstar_data-1.9.3/morningstar_data/direct/user_items/investment_lists.py
--rw-r--r--   0        0        0    11276 2024-04-15 19:48:03.061795 morningstar_data-1.9.3/morningstar_data/direct/user_items/portfolio.py
--rw-r--r--   0        0        0    10433 2024-04-15 19:48:03.061795 morningstar_data-1.9.3/morningstar_data/direct/user_items/search_criteria.py
--rw-r--r--   0        0        0     4768 2024-04-15 19:48:03.061795 morningstar_data-1.9.3/morningstar_data/lookup.py
--rw-r--r--   0        0        0       90 2024-04-15 19:48:03.061795 morningstar_data-1.9.3/morningstar_data/mdapi/__init__.py
--rw-r--r--   0        0        0     2359 2024-04-15 19:48:03.061795 morningstar_data-1.9.3/morningstar_data/mdapi/_exceptions.py
--rw-r--r--   0        0        0     6116 2024-04-15 19:48:03.061795 morningstar_data-1.9.3/morningstar_data/mdapi/_mdapi.py
--rw-r--r--   0        0        0     1303 2024-04-15 19:48:03.061795 morningstar_data-1.9.3/morningstar_data/mdapi/_types.py
--rw-r--r--   0        0        0      128 2024-04-15 19:48:03.061795 morningstar_data-1.9.3/morningstar_data/utils/__init__.py
--rw-r--r--   0        0        0    10975 2024-04-15 19:48:03.061795 morningstar_data-1.9.3/morningstar_data/utils/_delivery_config.py
--rw-r--r--   0        0        0     5814 2024-04-15 19:48:03.061795 morningstar_data-1.9.3/morningstar_data/utils/_helpers.py
--rw-r--r--   0        0        0    18353 2024-04-15 19:48:03.061795 morningstar_data-1.9.3/morningstar_data/utils/delivery.py
--rw-r--r--   0        0        0     2316 2024-04-15 19:50:17.752446 morningstar_data-1.9.3/pyproject.toml
--rw-r--r--   0        0        0    12424 1970-01-01 00:00:00.000000 morningstar_data-1.9.3/PKG-INFO
+-rw-r--r--   0        0        0      558 2024-04-24 18:18:23.695464 morningstar_data-1.9.4/LICENSE
+-rw-r--r--   0        0        0    11417 2024-04-24 18:18:23.695464 morningstar_data-1.9.4/README.md
+-rw-r--r--   0        0        0      168 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/__init__.py
+-rw-r--r--   0        0        0      598 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/_base.py
+-rw-r--r--   0        0        0     4233 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/_utils.py
+-rw-r--r--   0        0        0       82 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/_version.py
+-rw-r--r--   0        0        0       61 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/datalake/__init__.py
+-rw-r--r--   0        0        0       62 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/datalake/_data_objects/__init__.py
+-rw-r--r--   0        0        0      557 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/datalake/_data_objects/_file.py
+-rw-r--r--   0        0        0      763 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/datalake/_data_objects/_table.py
+-rw-r--r--   0        0        0      996 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/datalake/_data_objects/csvfile.py
+-rw-r--r--   0        0        0     2202 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/datalake/_data_objects/temptable.py
+-rw-r--r--   0        0        0      544 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/datalake/_error_messages.py
+-rw-r--r--   0        0        0      937 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/datalake/_exceptions.py
+-rw-r--r--   0        0        0     5604 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/datalake/base.py
+-rw-r--r--   0        0        0     1171 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/direct/__init__.py
+-rw-r--r--   0        0        0     2432 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/direct/_api.py
+-rw-r--r--   0        0        0      179 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/direct/_backend_apis/__init__.py
+-rw-r--r--   0        0        0     2075 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/direct/_backend_apis/_delivery_backend.py
+-rw-r--r--   0        0        0     4790 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/direct/_backend_apis/_holdings_backend.py
+-rw-r--r--   0        0        0     3372 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/direct/_backend_apis/_signed_url_backend.py
+-rw-r--r--   0        0        0     3795 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/direct/_base_api.py
+-rw-r--r--   0        0        0     5076 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/direct/_config.py
+-rw-r--r--   0        0        0     1999 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/direct/_config_key.py
+-rw-r--r--   0        0        0     7854 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/direct/_core_api.py
+-rw-r--r--   0        0        0      197 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/direct/_data_objects/__init__.py
+-rw-r--r--   0        0        0     2296 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/direct/_data_objects/_custom_data_points_types.py
+-rw-r--r--   0        0        0    26798 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/direct/_data_objects/_data_points_object.py
+-rw-r--r--   0        0        0     7574 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/direct/_data_objects/_investments_object.py
+-rw-r--r--   0        0        0     2887 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/direct/_data_point.py
+-rw-r--r--   0        0        0     1453 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/direct/_data_type.py
+-rw-r--r--   0        0        0     1614 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/direct/_decorator.py
+-rw-r--r--   0        0        0    14042 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/direct/_error_messages.py
+-rw-r--r--   0        0        0     3711 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/direct/_exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/direct/_investment/__init__.py
+-rw-r--r--   0        0        0     4620 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/direct/_investment/_asset_flow_data.py
+-rw-r--r--   0        0        0     1560 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/direct/_investment/_common.py
+-rw-r--r--   0        0        0     9136 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/direct/_investment/_data.py
+-rw-r--r--   0        0        0     8526 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/direct/_investment/_normal_data.py
+-rw-r--r--   0        0        0     5127 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/direct/_investment/_peer_group_data.py
+-rw-r--r--   0        0        0      162 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/direct/_portfolio/__init__.py
+-rw-r--r--   0        0        0     1273 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/direct/_portfolio/_common.py
+-rw-r--r--   0        0        0     8263 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/direct/_portfolio/_portfolio_holdings_entity.py
+-rw-r--r--   0        0        0     8023 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/direct/_portfolio/_portfolio_settings.py
+-rw-r--r--   0        0        0      719 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/direct/_portfolio/_portfolio_type.py
+-rw-r--r--   0        0        0    11071 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/direct/_portfolio_data_set.py
+-rw-r--r--   0        0        0     3356 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/direct/_utils.py
+-rw-r--r--   0        0        0    13081 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/direct/asset_flow.py
+-rw-r--r--   0        0        0    16435 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/direct/custom_database.py
+-rw-r--r--   0        0        0     1513 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/direct/data_type.py
+-rw-r--r--   0        0        0    45132 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/direct/holdings.py
+-rw-r--r--   0        0        0    18226 2024-04-24 18:18:23.703464 morningstar_data-1.9.4/morningstar_data/direct/investment.py
+-rw-r--r--   0        0        0    32429 2024-04-24 18:18:23.707464 morningstar_data-1.9.4/morningstar_data/direct/lookup.py
+-rw-r--r--   0        0        0     6154 2024-04-24 18:18:23.707464 morningstar_data-1.9.4/morningstar_data/direct/peer_group.py
+-rw-r--r--   0        0        0    19460 2024-04-24 18:18:23.707464 morningstar_data-1.9.4/morningstar_data/direct/performance_report.py
+-rw-r--r--   0        0        0    37410 2024-04-24 18:18:23.707464 morningstar_data-1.9.4/morningstar_data/direct/portfolio.py
+-rw-r--r--   0        0        0    11511 2024-04-24 18:18:23.707464 morningstar_data-1.9.4/morningstar_data/direct/returns.py
+-rw-r--r--   0        0        0      455 2024-04-24 18:18:23.707464 morningstar_data-1.9.4/morningstar_data/direct/user_items/__init__.py
+-rw-r--r--   0        0        0      582 2024-04-24 18:18:23.707464 morningstar_data-1.9.4/morningstar_data/direct/user_items/_utils.py
+-rw-r--r--   0        0        0     7910 2024-04-24 18:18:23.707464 morningstar_data-1.9.4/morningstar_data/direct/user_items/data_set.py
+-rw-r--r--   0        0        0    13091 2024-04-24 18:18:23.707464 morningstar_data-1.9.4/morningstar_data/direct/user_items/investment_lists.py
+-rw-r--r--   0        0        0    11276 2024-04-24 18:18:23.707464 morningstar_data-1.9.4/morningstar_data/direct/user_items/portfolio.py
+-rw-r--r--   0        0        0    10433 2024-04-24 18:18:23.707464 morningstar_data-1.9.4/morningstar_data/direct/user_items/search_criteria.py
+-rw-r--r--   0        0        0     4768 2024-04-24 18:18:23.707464 morningstar_data-1.9.4/morningstar_data/lookup.py
+-rw-r--r--   0        0        0       90 2024-04-24 18:18:23.707464 morningstar_data-1.9.4/morningstar_data/mdapi/__init__.py
+-rw-r--r--   0        0        0     2359 2024-04-24 18:18:23.707464 morningstar_data-1.9.4/morningstar_data/mdapi/_exceptions.py
+-rw-r--r--   0        0        0     6170 2024-04-24 18:18:23.707464 morningstar_data-1.9.4/morningstar_data/mdapi/_mdapi.py
+-rw-r--r--   0        0        0     1496 2024-04-24 18:18:23.707464 morningstar_data-1.9.4/morningstar_data/mdapi/_types.py
+-rw-r--r--   0        0        0      128 2024-04-24 18:18:23.707464 morningstar_data-1.9.4/morningstar_data/utils/__init__.py
+-rw-r--r--   0        0        0    10975 2024-04-24 18:18:23.707464 morningstar_data-1.9.4/morningstar_data/utils/_delivery_config.py
+-rw-r--r--   0        0        0     5814 2024-04-24 18:18:23.707464 morningstar_data-1.9.4/morningstar_data/utils/_helpers.py
+-rw-r--r--   0        0        0    18353 2024-04-24 18:18:23.707464 morningstar_data-1.9.4/morningstar_data/utils/delivery.py
+-rw-r--r--   0        0        0     2316 2024-04-24 18:20:33.891639 morningstar_data-1.9.4/pyproject.toml
+-rw-r--r--   0        0        0    12424 1970-01-01 00:00:00.000000 morningstar_data-1.9.4/PKG-INFO
```

### Comparing `morningstar_data-1.9.3/LICENSE` & `morningstar_data-1.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/README.md` & `morningstar_data-1.9.4/README.md`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/_base.py` & `morningstar_data-1.9.4/morningstar_data/_base.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/_utils.py` & `morningstar_data-1.9.4/morningstar_data/_utils.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/datalake/_data_objects/_file.py` & `morningstar_data-1.9.4/morningstar_data/datalake/_data_objects/_file.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/datalake/_data_objects/_table.py` & `morningstar_data-1.9.4/morningstar_data/datalake/_data_objects/_table.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/datalake/_data_objects/csvfile.py` & `morningstar_data-1.9.4/morningstar_data/datalake/_data_objects/csvfile.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/datalake/_data_objects/temptable.py` & `morningstar_data-1.9.4/morningstar_data/datalake/_data_objects/temptable.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/datalake/_error_messages.py` & `morningstar_data-1.9.4/morningstar_data/datalake/_error_messages.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/datalake/_exceptions.py` & `morningstar_data-1.9.4/morningstar_data/datalake/_exceptions.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/datalake/base.py` & `morningstar_data-1.9.4/morningstar_data/datalake/base.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/direct/__init__.py` & `morningstar_data-1.9.4/morningstar_data/direct/__init__.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/direct/_api.py` & `morningstar_data-1.9.4/morningstar_data/direct/_api.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/direct/_backend_apis/_delivery_backend.py` & `morningstar_data-1.9.4/morningstar_data/direct/_backend_apis/_delivery_backend.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/direct/_backend_apis/_holdings_backend.py` & `morningstar_data-1.9.4/morningstar_data/direct/_backend_apis/_holdings_backend.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/direct/_backend_apis/_signed_url_backend.py` & `morningstar_data-1.9.4/morningstar_data/direct/_backend_apis/_signed_url_backend.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/direct/_base_api.py` & `morningstar_data-1.9.4/morningstar_data/direct/_base_api.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/direct/_config.py` & `morningstar_data-1.9.4/morningstar_data/direct/_config.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/direct/_config_key.py` & `morningstar_data-1.9.4/morningstar_data/direct/_config_key.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/direct/_core_api.py` & `morningstar_data-1.9.4/morningstar_data/direct/_core_api.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/direct/_data_objects/_custom_data_points_types.py` & `morningstar_data-1.9.4/morningstar_data/direct/_data_objects/_custom_data_points_types.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/direct/_data_objects/_data_points_object.py` & `morningstar_data-1.9.4/morningstar_data/direct/_data_objects/_data_points_object.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/direct/_data_objects/_investments_object.py` & `morningstar_data-1.9.4/morningstar_data/direct/_data_objects/_investments_object.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/direct/_data_point.py` & `morningstar_data-1.9.4/morningstar_data/direct/_data_point.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/direct/_data_type.py` & `morningstar_data-1.9.4/morningstar_data/direct/_data_type.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/direct/_decorator.py` & `morningstar_data-1.9.4/morningstar_data/direct/_decorator.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/direct/_error_messages.py` & `morningstar_data-1.9.4/morningstar_data/direct/_error_messages.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/direct/_exceptions.py` & `morningstar_data-1.9.4/morningstar_data/direct/_exceptions.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/direct/_investment/_asset_flow_data.py` & `morningstar_data-1.9.4/morningstar_data/direct/_investment/_asset_flow_data.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/direct/_investment/_common.py` & `morningstar_data-1.9.4/morningstar_data/direct/_investment/_common.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/direct/_investment/_data.py` & `morningstar_data-1.9.4/morningstar_data/direct/_investment/_data.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/direct/_investment/_normal_data.py` & `morningstar_data-1.9.4/morningstar_data/direct/_investment/_normal_data.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/direct/_investment/_peer_group_data.py` & `morningstar_data-1.9.4/morningstar_data/direct/_investment/_peer_group_data.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/direct/_portfolio/_common.py` & `morningstar_data-1.9.4/morningstar_data/direct/_portfolio/_common.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/direct/_portfolio/_portfolio_holdings_entity.py` & `morningstar_data-1.9.4/morningstar_data/direct/_portfolio/_portfolio_holdings_entity.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/direct/_portfolio/_portfolio_settings.py` & `morningstar_data-1.9.4/morningstar_data/direct/_portfolio/_portfolio_settings.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/direct/_portfolio/_portfolio_type.py` & `morningstar_data-1.9.4/morningstar_data/direct/_portfolio/_portfolio_type.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/direct/_portfolio_data_set.py` & `morningstar_data-1.9.4/morningstar_data/direct/_portfolio_data_set.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/direct/_utils.py` & `morningstar_data-1.9.4/morningstar_data/direct/_utils.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/direct/asset_flow.py` & `morningstar_data-1.9.4/morningstar_data/direct/asset_flow.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/direct/custom_database.py` & `morningstar_data-1.9.4/morningstar_data/direct/custom_database.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/direct/data_type.py` & `morningstar_data-1.9.4/morningstar_data/direct/data_type.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/direct/holdings.py` & `morningstar_data-1.9.4/morningstar_data/direct/holdings.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/direct/investment.py` & `morningstar_data-1.9.4/morningstar_data/direct/investment.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/direct/lookup.py` & `morningstar_data-1.9.4/morningstar_data/direct/lookup.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/direct/peer_group.py` & `morningstar_data-1.9.4/morningstar_data/direct/peer_group.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/direct/performance_report.py` & `morningstar_data-1.9.4/morningstar_data/direct/performance_report.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/direct/portfolio.py` & `morningstar_data-1.9.4/morningstar_data/direct/portfolio.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/direct/returns.py` & `morningstar_data-1.9.4/morningstar_data/direct/returns.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/direct/user_items/_utils.py` & `morningstar_data-1.9.4/morningstar_data/direct/user_items/_utils.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/direct/user_items/data_set.py` & `morningstar_data-1.9.4/morningstar_data/direct/user_items/data_set.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/direct/user_items/investment_lists.py` & `morningstar_data-1.9.4/morningstar_data/direct/user_items/investment_lists.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/direct/user_items/portfolio.py` & `morningstar_data-1.9.4/morningstar_data/direct/user_items/portfolio.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/direct/user_items/search_criteria.py` & `morningstar_data-1.9.4/morningstar_data/direct/user_items/search_criteria.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/lookup.py` & `morningstar_data-1.9.4/morningstar_data/lookup.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/mdapi/_exceptions.py` & `morningstar_data-1.9.4/morningstar_data/mdapi/_exceptions.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/mdapi/_mdapi.py` & `morningstar_data-1.9.4/morningstar_data/mdapi/_mdapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,17 +75,18 @@
         "https://",
         requests.adapters.HTTPAdapter(
             max_retries=urllib3.util.Retry(total=3, backoff_factor=0.1, status_forcelist=[500, 502, 503, 504])
         ),
     )
 
     task_start_time = int(time.time())
+    task_time_limit = task.task_timeout_seconds
     while not task.is_complete():
-        if time.time() - task_start_time > POLL_TIMEOUT:
-            raise MdApiTaskTimeoutException(task_id=task.id, timeout_time=POLL_TIMEOUT)
+        if time.time() - task_start_time > task_time_limit:
+            raise MdApiTaskTimeoutException(task_id=task.id, timeout_time=task_time_limit)
         time.sleep(task.next_poll_delay_milliseconds / 1000.0)
         task = _check_task_status(task.poll_url, task_start_time, task_status_request_session)
     return task
 
 
 def _check_task_status(polling_url: str, task_start_time: float, task_status_request_session: requests.Session) -> MdapiTask:
     request_headers = _get_headers()
```

### Comparing `morningstar_data-1.9.3/morningstar_data/mdapi/_types.py` & `morningstar_data-1.9.4/morningstar_data/mdapi/_types.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from dataclasses import dataclass, field
 from enum import Enum
 from typing import List, Optional
 
+DEFAULT_POLL_INTERVAL_MILLISECONDS = 1000
+DEFAULT_POLL_TIMEOUT_SECONDS = 900  # seconds (15 minutes)
+
 
 class TaskStatus(str, Enum):
     SUCCESS = "success"
     PENDING = "pending"
     FAILURE = "failure"
 
 
@@ -20,15 +23,16 @@
     id: str
     # TODO: Add request_id
     poll_url: str
     status: TaskStatus = TaskStatus.PENDING
     result: Optional[TaskResult] = None
     error_class: Optional[str] = None
     error_message: Optional[str] = None
-    next_poll_delay_milliseconds: int = 1000
+    next_poll_delay_milliseconds: int = DEFAULT_POLL_INTERVAL_MILLISECONDS
+    task_timeout_seconds: int = DEFAULT_POLL_TIMEOUT_SECONDS
 
     def is_complete(self) -> bool:
         return self.status != TaskStatus.PENDING
 
     def is_successful(self) -> bool:
         return self.status == TaskStatus.SUCCESS
```

### Comparing `morningstar_data-1.9.3/morningstar_data/utils/_delivery_config.py` & `morningstar_data-1.9.4/morningstar_data/utils/_delivery_config.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/utils/_helpers.py` & `morningstar_data-1.9.4/morningstar_data/utils/_helpers.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/morningstar_data/utils/delivery.py` & `morningstar_data-1.9.4/morningstar_data/utils/delivery.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.3/pyproject.toml` & `morningstar_data-1.9.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "morningstar_data"
-version = "1.9.3"
+version = "1.9.4"
 description = "Morningstar Data"
 authors = ["Morningstar, Inc."]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://www.morningstar.com/products/md-python-package"
 documentation = "https://docs-analyticslab.morningstar.com/latest/index.html"
```

### Comparing `morningstar_data-1.9.3/PKG-INFO` & `morningstar_data-1.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morningstar-data
-Version: 1.9.3
+Version: 1.9.4
 Summary: Morningstar Data
 Home-page: https://www.morningstar.com/products/md-python-package
 License: Apache-2.0
 Author: Morningstar, Inc.
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

