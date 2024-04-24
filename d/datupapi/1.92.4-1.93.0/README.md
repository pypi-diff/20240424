# Comparing `tmp/datupapi-1.92.4.tar.gz` & `tmp/datupapi-1.93.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datupapi-1.92.4.tar", last modified: Mon Feb 26 21:37:48 2024, max compression
+gzip compressed data, was "datupapi-1.93.0.tar", last modified: Wed Apr 24 17:15:42 2024, max compression
```

## Comparing `datupapi-1.92.4.tar` & `datupapi-1.93.0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-02-26 21:37:48.715751 datupapi-1.92.4/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1218 2024-02-26 21:37:48.715751 datupapi-1.92.4/PKG-INFO
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-02-26 21:37:48.700750 datupapi-1.92.4/datupapi/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.92.4/datupapi/__init__.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-02-26 21:37:48.701751 datupapi-1.92.4/datupapi/configure/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.92.4/datupapi/configure/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     5750 2023-06-26 23:14:24.000000 datupapi-1.92.4/datupapi/configure/config.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-02-26 21:37:48.698751 datupapi-1.92.4/datupapi/distribution/
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-02-26 21:37:48.701751 datupapi-1.92.4/datupapi/distribution/conf/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-12-14 13:56:50.000000 datupapi-1.92.4/datupapi/distribution/conf/__init__.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-02-26 21:37:48.698751 datupapi-1.92.4/datupapi/distribution/src/
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-02-26 21:37:48.702751 datupapi-1.92.4/datupapi/distribution/src/DistributionFunctions/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-12-14 13:56:50.000000 datupapi-1.92.4/datupapi/distribution/src/DistributionFunctions/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     9390 2023-12-22 18:43:58.000000 datupapi-1.92.4/datupapi/distribution/src/DistributionFunctions/functions_distribution.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-02-26 21:37:48.702751 datupapi-1.92.4/datupapi/evaluate/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.92.4/datupapi/evaluate/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7039 2023-07-06 13:37:00.000000 datupapi-1.92.4/datupapi/evaluate/errors.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-02-26 21:37:48.704751 datupapi-1.92.4/datupapi/extract/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.92.4/datupapi/extract/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    66939 2024-02-22 19:20:36.000000 datupapi-1.92.4/datupapi/extract/io.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     9338 2023-08-28 15:15:16.000000 datupapi-1.92.4/datupapi/extract/io_citrix.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-02-26 21:37:48.705751 datupapi-1.92.4/datupapi/feateng/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.92.4/datupapi/feateng/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7922 2023-06-26 23:14:24.000000 datupapi-1.92.4/datupapi/feateng/relation.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     4425 2023-06-26 23:14:24.000000 datupapi-1.92.4/datupapi/feateng/scale.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-02-26 21:37:48.705751 datupapi-1.92.4/datupapi/inventory/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.92.4/datupapi/inventory/__init__.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-02-26 21:37:48.706750 datupapi-1.92.4/datupapi/inventory/conf/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.92.4/datupapi/inventory/conf/__init__.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-02-26 21:37:48.699751 datupapi-1.92.4/datupapi/inventory/src/
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-02-26 21:37:48.706750 datupapi-1.92.4/datupapi/inventory/src/DailyUsage/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.92.4/datupapi/inventory/src/DailyUsage/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7915 2023-08-28 15:14:13.000000 datupapi-1.92.4/datupapi/inventory/src/DailyUsage/daily_usage.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-02-26 21:37:48.706750 datupapi-1.92.4/datupapi/inventory/src/Format/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.92.4/datupapi/inventory/src/Format/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     5433 2024-02-26 21:37:34.000000 datupapi-1.92.4/datupapi/inventory/src/Format/inventory_format.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-02-26 21:37:48.707751 datupapi-1.92.4/datupapi/inventory/src/InventoryFunctions/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.92.4/datupapi/inventory/src/InventoryFunctions/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    10157 2024-02-26 21:37:34.000000 datupapi-1.92.4/datupapi/inventory/src/InventoryFunctions/functions_inventory.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-02-26 21:37:48.707751 datupapi-1.92.4/datupapi/inventory/src/ProcessForecast/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.92.4/datupapi/inventory/src/ProcessForecast/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    10560 2023-08-28 15:14:13.000000 datupapi-1.92.4/datupapi/inventory/src/ProcessForecast/define_periods.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7391 2023-08-28 15:14:13.000000 datupapi-1.92.4/datupapi/inventory/src/ProcessForecast/extract_forecast.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-02-26 21:37:48.708751 datupapi-1.92.4/datupapi/inventory/src/SuggestedForecast/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.92.4/datupapi/inventory/src/SuggestedForecast/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    14066 2023-08-28 15:14:13.000000 datupapi-1.92.4/datupapi/inventory/src/SuggestedForecast/suggested_forecast.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-02-26 21:37:48.708751 datupapi-1.92.4/datupapi/inventory/src/Transformation/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.92.4/datupapi/inventory/src/Transformation/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1219 2023-08-28 15:14:13.000000 datupapi-1.92.4/datupapi/inventory/src/Transformation/inventory_transformation.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    80578 2023-06-26 23:14:24.000000 datupapi-1.92.4/datupapi/inventory/stocks.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-02-26 21:37:48.709751 datupapi-1.92.4/datupapi/predict/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.92.4/datupapi/predict/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    27677 2023-06-26 23:14:24.000000 datupapi-1.92.4/datupapi/predict/forecast.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-02-26 21:37:48.710751 datupapi-1.92.4/datupapi/prepare/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.92.4/datupapi/prepare/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1922 2023-06-26 23:14:24.000000 datupapi-1.92.4/datupapi/prepare/cleanse.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    20602 2023-10-25 22:17:02.000000 datupapi-1.92.4/datupapi/prepare/format.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     4800 2023-06-26 23:14:24.000000 datupapi-1.92.4/datupapi/prepare/format_dask.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-02-26 21:37:48.711751 datupapi-1.92.4/datupapi/training/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.92.4/datupapi/training/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    25158 2023-06-26 23:14:24.000000 datupapi-1.92.4/datupapi/training/attup.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    31654 2023-06-26 23:14:24.000000 datupapi-1.92.4/datupapi/training/deepar.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    21849 2024-02-23 15:50:42.000000 datupapi-1.92.4/datupapi/training/tft.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-02-26 21:37:48.713751 datupapi-1.92.4/datupapi/transform/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.92.4/datupapi/transform/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    18233 2023-06-26 23:14:24.000000 datupapi-1.92.4/datupapi/transform/backtesting.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    52714 2023-06-26 23:14:24.000000 datupapi-1.92.4/datupapi/transform/forecasting.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7943 2023-06-26 23:14:24.000000 datupapi-1.92.4/datupapi/transform/ranking.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-02-26 21:37:48.714751 datupapi-1.92.4/datupapi/utils/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.92.4/datupapi/utils/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     4637 2023-06-26 23:14:24.000000 datupapi-1.92.4/datupapi/utils/utils.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-02-26 21:37:48.714751 datupapi-1.92.4/datupapi.egg-info/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1218 2024-02-26 21:37:48.000000 datupapi-1.92.4/datupapi.egg-info/PKG-INFO
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1925 2024-02-26 21:37:48.000000 datupapi-1.92.4/datupapi.egg-info/SOURCES.txt
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        1 2024-02-26 21:37:48.000000 datupapi-1.92.4/datupapi.egg-info/dependency_links.txt
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)      539 2024-02-26 21:37:48.000000 datupapi-1.92.4/datupapi.egg-info/requires.txt
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        9 2024-02-26 21:37:48.000000 datupapi-1.92.4/datupapi.egg-info/top_level.txt
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)       87 2023-12-19 15:43:19.000000 datupapi-1.92.4/pyproject.toml
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)       38 2024-02-26 21:37:48.715751 datupapi-1.92.4/setup.cfg
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     2129 2024-02-26 21:37:34.000000 datupapi-1.92.4/setup.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 17:15:42.463973 datupapi-1.93.0/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1218 2024-04-24 17:15:42.462973 datupapi-1.93.0/PKG-INFO
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 17:15:42.450973 datupapi-1.93.0/datupapi/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.93.0/datupapi/__init__.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 17:15:42.451973 datupapi-1.93.0/datupapi/configure/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.93.0/datupapi/configure/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     5750 2023-06-26 23:14:24.000000 datupapi-1.93.0/datupapi/configure/config.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 17:15:42.449973 datupapi-1.93.0/datupapi/distribution/
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 17:15:42.452973 datupapi-1.93.0/datupapi/distribution/conf/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-12-14 13:56:50.000000 datupapi-1.93.0/datupapi/distribution/conf/__init__.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 17:15:42.449973 datupapi-1.93.0/datupapi/distribution/src/
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 17:15:42.452973 datupapi-1.93.0/datupapi/distribution/src/DistributionFunctions/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-12-14 13:56:50.000000 datupapi-1.93.0/datupapi/distribution/src/DistributionFunctions/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     9390 2023-12-22 18:43:58.000000 datupapi-1.93.0/datupapi/distribution/src/DistributionFunctions/functions_distribution.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 17:15:42.452973 datupapi-1.93.0/datupapi/evaluate/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.93.0/datupapi/evaluate/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7039 2023-07-06 13:37:00.000000 datupapi-1.93.0/datupapi/evaluate/errors.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 17:15:42.453973 datupapi-1.93.0/datupapi/extract/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.93.0/datupapi/extract/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    66939 2024-02-22 19:20:36.000000 datupapi-1.93.0/datupapi/extract/io.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     9338 2023-08-28 15:15:16.000000 datupapi-1.93.0/datupapi/extract/io_citrix.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 17:15:42.454973 datupapi-1.93.0/datupapi/feateng/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.93.0/datupapi/feateng/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7922 2023-06-26 23:14:24.000000 datupapi-1.93.0/datupapi/feateng/relation.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     4425 2023-06-26 23:14:24.000000 datupapi-1.93.0/datupapi/feateng/scale.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 17:15:42.455973 datupapi-1.93.0/datupapi/inventory/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.93.0/datupapi/inventory/__init__.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 17:15:42.455973 datupapi-1.93.0/datupapi/inventory/conf/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.93.0/datupapi/inventory/conf/__init__.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 17:15:42.450973 datupapi-1.93.0/datupapi/inventory/src/
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 17:15:42.455973 datupapi-1.93.0/datupapi/inventory/src/DailyUsage/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.93.0/datupapi/inventory/src/DailyUsage/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7915 2023-08-28 15:14:13.000000 datupapi-1.93.0/datupapi/inventory/src/DailyUsage/daily_usage.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 17:15:42.456973 datupapi-1.93.0/datupapi/inventory/src/Format/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.93.0/datupapi/inventory/src/Format/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     5433 2024-02-26 21:37:34.000000 datupapi-1.93.0/datupapi/inventory/src/Format/inventory_format.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 17:15:42.456973 datupapi-1.93.0/datupapi/inventory/src/InventoryFunctions/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.93.0/datupapi/inventory/src/InventoryFunctions/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    10157 2024-02-26 21:37:34.000000 datupapi-1.93.0/datupapi/inventory/src/InventoryFunctions/functions_inventory.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 17:15:42.457973 datupapi-1.93.0/datupapi/inventory/src/ProcessForecast/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.93.0/datupapi/inventory/src/ProcessForecast/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    10560 2023-08-28 15:14:13.000000 datupapi-1.93.0/datupapi/inventory/src/ProcessForecast/define_periods.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7391 2023-08-28 15:14:13.000000 datupapi-1.93.0/datupapi/inventory/src/ProcessForecast/extract_forecast.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 17:15:42.457973 datupapi-1.93.0/datupapi/inventory/src/SuggestedForecast/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.93.0/datupapi/inventory/src/SuggestedForecast/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    14066 2023-08-28 15:14:13.000000 datupapi-1.93.0/datupapi/inventory/src/SuggestedForecast/suggested_forecast.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 17:15:42.458973 datupapi-1.93.0/datupapi/inventory/src/Transformation/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.93.0/datupapi/inventory/src/Transformation/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1219 2023-08-28 15:14:13.000000 datupapi-1.93.0/datupapi/inventory/src/Transformation/inventory_transformation.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    80578 2023-06-26 23:14:24.000000 datupapi-1.93.0/datupapi/inventory/stocks.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 17:15:42.458973 datupapi-1.93.0/datupapi/predict/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.93.0/datupapi/predict/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    27677 2023-06-26 23:14:24.000000 datupapi-1.93.0/datupapi/predict/forecast.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 17:15:42.459973 datupapi-1.93.0/datupapi/prepare/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.93.0/datupapi/prepare/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1922 2023-06-26 23:14:24.000000 datupapi-1.93.0/datupapi/prepare/cleanse.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    20602 2023-10-25 22:17:02.000000 datupapi-1.93.0/datupapi/prepare/format.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     4800 2023-06-26 23:14:24.000000 datupapi-1.93.0/datupapi/prepare/format_dask.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 17:15:42.460973 datupapi-1.93.0/datupapi/training/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.93.0/datupapi/training/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    25158 2023-06-26 23:14:24.000000 datupapi-1.93.0/datupapi/training/attup.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    31654 2023-06-26 23:14:24.000000 datupapi-1.93.0/datupapi/training/deepar.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    22027 2024-04-24 17:14:57.000000 datupapi-1.93.0/datupapi/training/tft.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 17:15:42.461973 datupapi-1.93.0/datupapi/transform/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.93.0/datupapi/transform/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    18233 2023-06-26 23:14:24.000000 datupapi-1.93.0/datupapi/transform/backtesting.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    52714 2023-06-26 23:14:24.000000 datupapi-1.93.0/datupapi/transform/forecasting.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7943 2023-06-26 23:14:24.000000 datupapi-1.93.0/datupapi/transform/ranking.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 17:15:42.461973 datupapi-1.93.0/datupapi/utils/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.93.0/datupapi/utils/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     4637 2023-06-26 23:14:24.000000 datupapi-1.93.0/datupapi/utils/utils.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-24 17:15:42.462973 datupapi-1.93.0/datupapi.egg-info/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1218 2024-04-24 17:15:42.000000 datupapi-1.93.0/datupapi.egg-info/PKG-INFO
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1925 2024-04-24 17:15:42.000000 datupapi-1.93.0/datupapi.egg-info/SOURCES.txt
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        1 2024-04-24 17:15:42.000000 datupapi-1.93.0/datupapi.egg-info/dependency_links.txt
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)      539 2024-04-24 17:15:42.000000 datupapi-1.93.0/datupapi.egg-info/requires.txt
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        9 2024-04-24 17:15:42.000000 datupapi-1.93.0/datupapi.egg-info/top_level.txt
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)       87 2023-12-19 15:43:19.000000 datupapi-1.93.0/pyproject.toml
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)       38 2024-04-24 17:15:42.463973 datupapi-1.93.0/setup.cfg
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     2129 2024-04-24 17:13:57.000000 datupapi-1.93.0/setup.py
```

### Comparing `datupapi-1.92.4/PKG-INFO` & `datupapi-1.93.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datupapi
-Version: 1.92.4
+Version: 1.93.0
 Summary: Utility library to support Datup AI MLOps processes
 Author: Datup AI
 Author-email: ramiro@datup.ai
 Description-Content-Type: text/markdown
 Requires-Dist: beautifulsoup4>=4.9.3
 Requires-Dist: boto3>=1.16.54
 Requires-Dist: catboost>=1.0.4
```

### Comparing `datupapi-1.92.4/datupapi/configure/config.py` & `datupapi-1.93.0/datupapi/configure/config.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.92.4/datupapi/distribution/src/DistributionFunctions/functions_distribution.py` & `datupapi-1.93.0/datupapi/distribution/src/DistributionFunctions/functions_distribution.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.92.4/datupapi/evaluate/errors.py` & `datupapi-1.93.0/datupapi/evaluate/errors.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.92.4/datupapi/extract/io.py` & `datupapi-1.93.0/datupapi/extract/io.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.92.4/datupapi/extract/io_citrix.py` & `datupapi-1.93.0/datupapi/extract/io_citrix.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.92.4/datupapi/feateng/relation.py` & `datupapi-1.93.0/datupapi/feateng/relation.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.92.4/datupapi/feateng/scale.py` & `datupapi-1.93.0/datupapi/feateng/scale.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.92.4/datupapi/inventory/src/DailyUsage/daily_usage.py` & `datupapi-1.93.0/datupapi/inventory/src/DailyUsage/daily_usage.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.92.4/datupapi/inventory/src/Format/inventory_format.py` & `datupapi-1.93.0/datupapi/inventory/src/Format/inventory_format.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.92.4/datupapi/inventory/src/InventoryFunctions/functions_inventory.py` & `datupapi-1.93.0/datupapi/inventory/src/InventoryFunctions/functions_inventory.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.92.4/datupapi/inventory/src/ProcessForecast/define_periods.py` & `datupapi-1.93.0/datupapi/inventory/src/ProcessForecast/define_periods.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.92.4/datupapi/inventory/src/ProcessForecast/extract_forecast.py` & `datupapi-1.93.0/datupapi/inventory/src/ProcessForecast/extract_forecast.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.92.4/datupapi/inventory/src/SuggestedForecast/suggested_forecast.py` & `datupapi-1.93.0/datupapi/inventory/src/SuggestedForecast/suggested_forecast.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.92.4/datupapi/inventory/src/Transformation/inventory_transformation.py` & `datupapi-1.93.0/datupapi/inventory/src/Transformation/inventory_transformation.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.92.4/datupapi/inventory/stocks.py` & `datupapi-1.93.0/datupapi/inventory/stocks.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.92.4/datupapi/predict/forecast.py` & `datupapi-1.93.0/datupapi/predict/forecast.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.92.4/datupapi/prepare/cleanse.py` & `datupapi-1.93.0/datupapi/prepare/cleanse.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.92.4/datupapi/prepare/format.py` & `datupapi-1.93.0/datupapi/prepare/format.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.92.4/datupapi/prepare/format_dask.py` & `datupapi-1.93.0/datupapi/prepare/format_dask.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.92.4/datupapi/training/attup.py` & `datupapi-1.93.0/datupapi/training/attup.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.92.4/datupapi/training/deepar.py` & `datupapi-1.93.0/datupapi/training/deepar.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.92.4/datupapi/training/tft.py` & `datupapi-1.93.0/datupapi/training/tft.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,15 +165,17 @@
         if frequency == '2M':
             data_range = pd.date_range(start=data1.timestamp.min(), end=data1.timestamp.max(), freq=frequency)
             #data_range= data_range+pd.offsets.MonthEnd(n=data1.timestamp.max().month%2)if suffix=='' else data_range+pd.offsets.MonthBegin(n=data1.timestamp.max().month%2)
         else:
             data_range = pd.date_range(start=data1.timestamp.min(), end=data1.timestamp.max(), freq=frequency + suffix)
         data_range_df = pd.DataFrame(data_range, columns=["timestamp"]).reset_index().rename(columns={"index": "time_idx"})
         warnings.filterwarnings("ignore")  # avoid printing out absolute paths
+
         data1 = data1.sort_values(by=["timestamp", "item_id"])
+        data1["timestamp"] = pd.to_datetime(data1["timestamp"]) # ADD IVAN
         data1 = data1.merge(data_range_df, how="left", on=["timestamp"])
 
         n_features = len(data1.groupby(["item_id", "location"]).size()) if self.use_location else data1.item_id.nunique()
         max_prediction_length = self.forecast_horizon
         max_encoder_length = self.input_window
 
         #Create test_data
@@ -186,15 +188,15 @@
             item_location = data1.groupby(["item_id", "location"]).size().reset_index()
             test_data.insert(2, "item_id", np.repeat(item_location.item_id.values, max_prediction_length))
             test_data.insert(3, "location", np.repeat(item_location.location.values, max_prediction_length))
         else:
             test_data.insert(2, "item_id", np.repeat(data1.item_id.unique(), max_prediction_length))
 
         ts_column = 'timestamp'
-        test_data["timestamp"] = pd.to_datetime(test_data["timestamp"])
+        test_data["timestamp"] = pd.to_datetime(test_data["timestamp"]) # ADD IVAN
         test_data = test_data.assign(demand=0)
         data1 = pd.concat([data1, test_data], axis=0)
 
         #add holidays
         io.datalake = "unimilitar-datalake"
         holidays = io.download_object_csv(datalake_path="as-is/opendata/Holidays.csv").loc[:, :"holidays_Colombia"]
         holidays.Date = pd.to_datetime(holidays.Date)
@@ -203,15 +205,16 @@
         data1 = data1.merge(holidays, on="timestamp")
         io = IO(config_file=DOCKER_CONFIG_PATH, logfile='data_training', log_path='output/logs')
 
         #Add time related features
         timestamp = data1[["timestamp"]]
         ts_column = 'timestamp'
         data1["Mes"] = pd.to_datetime(data1[ts_column]).dt.month
-        data1["timestamp_weekofyear"] = data1[ts_column].dt.weekofyear
+        #data1["timestamp_weekofyear"] = data1[ts_column].dt.weekofyear
+        data1["timestamp_weekofyear"] = data1[ts_column].dt.isocalendar().week # ADD IVAN
         data1["timestamp_dayofyear"] = data1[ts_column].dt.dayofyear
         data1["timestamp_year"] = data1[ts_column].dt.year
         data1["timestamp_quarter"] = data1[ts_column].dt.quarter
         #data1, ts_adds_in = FW.FE_create_time_series_features(data1, ts_column, ts_adds_in=[])
         #data1=data1.drop(columns=["timestamp_month_typeofday_cross","timestamp_typeofday","timestamp_age_in_years","timestamp_month_dayofweek_cross","timestamp_is_warm","timestamp_is_cold","timestamp_is_festive","timestamp_month","timestamp_dayofweek_hour_cross","timestamp_dayofweek"])
         #data1["timestamp"]=timestamp
```

### Comparing `datupapi-1.92.4/datupapi/transform/backtesting.py` & `datupapi-1.93.0/datupapi/transform/backtesting.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.92.4/datupapi/transform/forecasting.py` & `datupapi-1.93.0/datupapi/transform/forecasting.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.92.4/datupapi/transform/ranking.py` & `datupapi-1.93.0/datupapi/transform/ranking.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.92.4/datupapi/utils/utils.py` & `datupapi-1.93.0/datupapi/utils/utils.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.92.4/datupapi.egg-info/PKG-INFO` & `datupapi-1.93.0/datupapi.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datupapi
-Version: 1.92.4
+Version: 1.93.0
 Summary: Utility library to support Datup AI MLOps processes
 Author: Datup AI
 Author-email: ramiro@datup.ai
 Description-Content-Type: text/markdown
 Requires-Dist: beautifulsoup4>=4.9.3
 Requires-Dist: boto3>=1.16.54
 Requires-Dist: catboost>=1.0.4
```

### Comparing `datupapi-1.92.4/datupapi.egg-info/SOURCES.txt` & `datupapi-1.93.0/datupapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datupapi-1.92.4/datupapi.egg-info/requires.txt` & `datupapi-1.93.0/datupapi.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `datupapi-1.92.4/setup.py` & `datupapi-1.93.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='datupapi',
-      version='1.92.4',
+      version='1.93.0',
       description='Utility library to support Datup AI MLOps processes',
       long_description_content_type="text/markdown",
       long_description="foo bar baz",
       author='Datup AI',
       author_email='ramiro@datup.ai',
       packages=[
           'datupapi',
```

