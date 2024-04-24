# Comparing `tmp/hftbacktest-1.8.0.tar.gz` & `tmp/hftbacktest-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hftbacktest-1.8.0.tar", last modified: Fri Mar 22 14:42:35 2024, max compression
+gzip compressed data, was "hftbacktest-1.8.1.tar", last modified: Wed Apr 24 14:31:47 2024, max compression
```

## Comparing `hftbacktest-1.8.0.tar` & `hftbacktest-1.8.1.tar`

### file list

```diff
@@ -1,53 +1,44 @@
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2024-03-22 14:42:35.883895 hftbacktest-1.8.0/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1079 2023-04-27 05:42:48.000000 hftbacktest-1.8.0/LICENSE
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     9108 2024-03-22 14:42:35.883895 hftbacktest-1.8.0/PKG-INFO
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     7998 2024-03-14 11:41:33.000000 hftbacktest-1.8.0/README.rst
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2024-03-22 14:42:35.882895 hftbacktest-1.8.0/hftbacktest/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    12124 2024-03-19 13:04:24.000000 hftbacktest-1.8.0/hftbacktest/__init__.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1011 2023-04-27 05:42:48.000000 hftbacktest-1.8.0/hftbacktest/assettype.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    16000 2024-03-19 13:08:02.000000 hftbacktest-1.8.0/hftbacktest/backtest.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2024-03-22 14:42:35.882895 hftbacktest-1.8.0/hftbacktest/data/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1592 2023-04-27 05:42:48.000000 hftbacktest-1.8.0/hftbacktest/data/__init__.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2024-03-22 14:42:35.882895 hftbacktest-1.8.0/hftbacktest/data/utils/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       44 2023-04-27 05:42:48.000000 hftbacktest-1.8.0/hftbacktest/data/utils/__init__.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    12832 2024-03-22 14:39:26.000000 hftbacktest-1.8.0/hftbacktest/data/utils/binancefutures.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    10189 2024-03-22 14:34:52.000000 hftbacktest-1.8.0/hftbacktest/data/utils/binancehistmktdata.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     7967 2023-12-10 12:15:55.000000 hftbacktest-1.8.0/hftbacktest/data/utils/difforderbooksnapshot.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     2768 2024-03-22 14:39:11.000000 hftbacktest-1.8.0/hftbacktest/data/utils/snapshot.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     9425 2024-03-22 14:38:59.000000 hftbacktest-1.8.0/hftbacktest/data/utils/tardis.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    16544 2024-03-19 12:59:14.000000 hftbacktest-1.8.0/hftbacktest/data/validation.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2024-03-22 14:42:35.882895 hftbacktest-1.8.0/hftbacktest/experimental/
--rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-29 10:30:43.000000 hftbacktest-1.8.0/hftbacktest/experimental/__init__.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2024-03-22 14:42:35.883895 hftbacktest-1.8.0/hftbacktest/experimental/live/
--rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-29 10:30:43.000000 hftbacktest-1.8.0/hftbacktest/experimental/live/__init__.py
--rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)    19814 2023-11-15 14:15:34.000000 hftbacktest-1.8.0/hftbacktest/experimental/live/binancefutures.py
--rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)      422 2023-11-15 14:30:09.000000 hftbacktest-1.8.0/hftbacktest/experimental/live/custom_strategy.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     9839 2023-11-15 14:34:08.000000 hftbacktest-1.8.0/hftbacktest/experimental/live/livebroker.py
--rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)     7792 2023-04-29 10:30:43.000000 hftbacktest-1.8.0/hftbacktest/experimental/live/ordermanager.py
--rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)     3578 2023-04-29 10:30:43.000000 hftbacktest-1.8.0/hftbacktest/experimental/live/settings.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6194 2023-08-23 14:57:13.000000 hftbacktest-1.8.0/hftbacktest/marketdepth.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2024-03-22 14:42:35.883895 hftbacktest-1.8.0/hftbacktest/models/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-27 05:42:48.000000 hftbacktest-1.8.0/hftbacktest/models/__init__.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    12224 2023-12-10 12:16:05.000000 hftbacktest-1.8.0/hftbacktest/models/latencies.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     4867 2024-02-14 09:48:00.000000 hftbacktest-1.8.0/hftbacktest/models/queue.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     4856 2024-03-11 14:20:26.000000 hftbacktest-1.8.0/hftbacktest/order.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2024-03-22 14:42:35.883895 hftbacktest-1.8.0/hftbacktest/proc/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-27 05:42:48.000000 hftbacktest-1.8.0/hftbacktest/proc/__init__.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     8149 2023-12-04 12:17:36.000000 hftbacktest-1.8.0/hftbacktest/proc/local.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    19211 2023-05-18 13:30:05.000000 hftbacktest-1.8.0/hftbacktest/proc/nopartialfillexchange.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    30417 2023-12-01 13:42:13.000000 hftbacktest-1.8.0/hftbacktest/proc/partialfillexchange.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     5850 2023-12-01 13:42:13.000000 hftbacktest-1.8.0/hftbacktest/proc/proc.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     3332 2024-03-19 12:28:56.000000 hftbacktest-1.8.0/hftbacktest/reader.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    13980 2023-12-10 12:16:12.000000 hftbacktest-1.8.0/hftbacktest/stat.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     2149 2023-05-11 12:00:32.000000 hftbacktest-1.8.0/hftbacktest/state.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     7460 2023-05-26 12:41:56.000000 hftbacktest-1.8.0/hftbacktest/stats.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)      876 2023-05-11 11:04:39.000000 hftbacktest-1.8.0/hftbacktest/typing.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2024-03-22 14:42:35.882895 hftbacktest-1.8.0/hftbacktest.egg-info/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     9108 2024-03-22 14:42:35.000000 hftbacktest-1.8.0/hftbacktest.egg-info/PKG-INFO
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1330 2024-03-22 14:42:35.000000 hftbacktest-1.8.0/hftbacktest.egg-info/SOURCES.txt
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        1 2024-03-22 14:42:35.000000 hftbacktest-1.8.0/hftbacktest.egg-info/dependency_links.txt
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        1 2023-04-28 14:15:39.000000 hftbacktest-1.8.0/hftbacktest.egg-info/not-zip-safe
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       48 2024-03-22 14:42:35.000000 hftbacktest-1.8.0/hftbacktest.egg-info/requires.txt
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       12 2024-03-22 14:42:35.000000 hftbacktest-1.8.0/hftbacktest.egg-info/top_level.txt
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1249 2024-03-22 14:42:35.883895 hftbacktest-1.8.0/setup.cfg
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       61 2023-04-27 05:42:48.000000 hftbacktest-1.8.0/setup.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2024-04-24 14:31:47.996698 hftbacktest-1.8.1/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1079 2023-04-27 05:42:48.000000 hftbacktest-1.8.1/LICENSE
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     9133 2024-04-24 14:31:47.996698 hftbacktest-1.8.1/PKG-INFO
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     8022 2024-04-24 14:24:53.000000 hftbacktest-1.8.1/README.rst
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2024-04-24 14:31:47.995698 hftbacktest-1.8.1/hftbacktest/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    12124 2024-04-24 13:30:16.000000 hftbacktest-1.8.1/hftbacktest/__init__.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1011 2023-04-27 05:42:48.000000 hftbacktest-1.8.1/hftbacktest/assettype.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    16000 2024-03-19 13:08:02.000000 hftbacktest-1.8.1/hftbacktest/backtest.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2024-04-24 14:31:47.995698 hftbacktest-1.8.1/hftbacktest/data/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1592 2023-04-27 05:42:48.000000 hftbacktest-1.8.1/hftbacktest/data/__init__.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2024-04-24 14:31:47.996698 hftbacktest-1.8.1/hftbacktest/data/utils/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       44 2023-04-27 05:42:48.000000 hftbacktest-1.8.1/hftbacktest/data/utils/__init__.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    14082 2024-04-24 10:45:33.000000 hftbacktest-1.8.1/hftbacktest/data/utils/binancefutures.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    10189 2024-03-22 14:34:52.000000 hftbacktest-1.8.1/hftbacktest/data/utils/binancehistmktdata.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     7967 2023-12-10 12:15:55.000000 hftbacktest-1.8.1/hftbacktest/data/utils/difforderbooksnapshot.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     2768 2024-03-22 14:39:11.000000 hftbacktest-1.8.1/hftbacktest/data/utils/snapshot.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    10184 2024-04-24 14:11:01.000000 hftbacktest-1.8.1/hftbacktest/data/utils/tardis.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    16544 2024-04-24 14:11:20.000000 hftbacktest-1.8.1/hftbacktest/data/validation.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6194 2023-08-23 14:57:13.000000 hftbacktest-1.8.1/hftbacktest/marketdepth.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2024-04-24 14:31:47.996698 hftbacktest-1.8.1/hftbacktest/models/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-27 05:42:48.000000 hftbacktest-1.8.1/hftbacktest/models/__init__.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    12224 2023-12-10 12:16:05.000000 hftbacktest-1.8.1/hftbacktest/models/latencies.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     4867 2024-02-14 09:48:00.000000 hftbacktest-1.8.1/hftbacktest/models/queue.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     4856 2024-03-11 14:20:26.000000 hftbacktest-1.8.1/hftbacktest/order.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2024-04-24 14:31:47.996698 hftbacktest-1.8.1/hftbacktest/proc/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-27 05:42:48.000000 hftbacktest-1.8.1/hftbacktest/proc/__init__.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     8149 2023-12-04 12:17:36.000000 hftbacktest-1.8.1/hftbacktest/proc/local.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    19211 2023-05-18 13:30:05.000000 hftbacktest-1.8.1/hftbacktest/proc/nopartialfillexchange.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    30419 2024-04-14 14:19:28.000000 hftbacktest-1.8.1/hftbacktest/proc/partialfillexchange.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     5850 2023-12-01 13:42:13.000000 hftbacktest-1.8.1/hftbacktest/proc/proc.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     3332 2024-03-19 12:28:56.000000 hftbacktest-1.8.1/hftbacktest/reader.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    13980 2023-12-10 12:16:12.000000 hftbacktest-1.8.1/hftbacktest/stat.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     2149 2023-05-11 12:00:32.000000 hftbacktest-1.8.1/hftbacktest/state.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     7460 2023-05-26 12:41:56.000000 hftbacktest-1.8.1/hftbacktest/stats.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)      876 2023-05-11 11:04:39.000000 hftbacktest-1.8.1/hftbacktest/typing.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2024-04-24 14:31:47.995698 hftbacktest-1.8.1/hftbacktest.egg-info/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     9133 2024-04-24 14:31:47.000000 hftbacktest-1.8.1/hftbacktest.egg-info/PKG-INFO
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1022 2024-04-24 14:31:47.000000 hftbacktest-1.8.1/hftbacktest.egg-info/SOURCES.txt
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        1 2024-04-24 14:31:47.000000 hftbacktest-1.8.1/hftbacktest.egg-info/dependency_links.txt
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        1 2023-04-28 14:15:39.000000 hftbacktest-1.8.1/hftbacktest.egg-info/not-zip-safe
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       48 2024-04-24 14:31:47.000000 hftbacktest-1.8.1/hftbacktest.egg-info/requires.txt
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       12 2024-04-24 14:31:47.000000 hftbacktest-1.8.1/hftbacktest.egg-info/top_level.txt
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1250 2024-04-24 14:31:47.996698 hftbacktest-1.8.1/setup.cfg
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       61 2023-04-27 05:42:48.000000 hftbacktest-1.8.1/setup.py
```

### Comparing `hftbacktest-1.8.0/LICENSE` & `hftbacktest-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.0/PKG-INFO` & `hftbacktest-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hftbacktest
-Version: 1.8.0
+Version: 1.8.1
 Summary: High-frequency trading and market making backtesting tool
 Home-page: https://github.com/nkaz001/hftbacktest
 Author: nkaz001
 Author-email: nkaz001@protonmail.com
 License: MIT
 Project-URL: Docs, https://hftbacktest.readthedocs.io/en/latest/
 Project-URL: GitHub: issues, https://github.com/nkaz001/hftbacktest/issues
@@ -17,27 +17,38 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Office/Business :: Financial :: Investment
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 License-File: LICENSE
 
 ===========
 HftBacktest
 ===========
 
 |codacy| |codeql| |pypi| |downloads| |license| |docs| |github|
 
-High-Frequency Trading Backtesting Tool in Python
-=================================================
+High-Frequency Trading Backtesting Tool
+=======================================
 
-This Python framework is designed for developing high-frequency trading and market-making strategies. It focuses on accounting for both feed and order latencies, as well as the order queue position for order fill simulation. The framework aims to provide more accurate market replay-based backtesting, based on full order book and trade tick feed data.
+This framework is designed for developing high-frequency trading and market-making strategies. It focuses on accounting for both feed and order latencies, as well as the order queue position for order fill simulation. The framework aims to provide more accurate market replay-based backtesting, based on full order book and trade tick feed data.
+
+Rust implementation with experimental features
+==============================================
+
+The experimental features are currently in the early stages of development, having been completely rewritten in Rust to
+support the following features.
+
+* Backtesting of multi-asset and multi-exchange models
+* Deployment of a live trading bot using the same algo code.
+
+Please see `rust <https://github.com/nkaz001/hftbacktest/tree/master/rust>`_ directory.
 
 Key Features
 ============
 
 * Working in `Numba <https://numba.pydata.org/>`_ JIT function.
 * Complete tick-by-tick simulation with a variable time interval.
 * Full order book reconstruction based on L2 feeds(Market-By-Price).
@@ -51,15 +62,15 @@
 
 Getting started
 ===============
 
 Installation
 ------------
 
-hftbacktest supports Python 3.8+. You can install hftbacktest using ``pip``:
+hftbacktest supports Python 3.10+. You can install hftbacktest using ``pip``:
 
 .. code-block:: console
 
  pip install hftbacktest
 
 Or you can clone the latest development version from the Git repository with:
 
@@ -159,25 +170,14 @@
 * `Risk Mitigation through Price Protection in Extreme Market Conditions <https://hftbacktest.readthedocs.io/en/latest/tutorials/Risk%20Mitigation%20through%20Price%20Protection%20in%20Extreme%20Market%20Conditions.html>`_
 
 Examples
 ========
 
 You can find more examples in `examples <https://github.com/nkaz001/hftbacktest/tree/master/examples>`_ directory.
 
-Experimental features
-=====================
-
-The experimental features are currently in the early stages of development, having been completely rewritten in Rust to
-support the following features.
-
-* Backtesting of multi-asset and multi-exchange models
-* Deployment of a live trading bot using the same algo code.
-
-Please see `rust <https://github.com/nkaz001/hftbacktest/tree/master/rust>`_ directory.
-
 Contributing
 ============
 
 Thank you for considering contributing to hftbacktest! Welcome any and all help to improve the project. If you have an
 idea for an enhancement or a bug fix, please open an issue or discussion on GitHub to discuss it.
 
 The following items are examples of contributions you can make to this project:
```

### Comparing `hftbacktest-1.8.0/README.rst` & `hftbacktest-1.8.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,28 @@
 ===========
 HftBacktest
 ===========
 
 |codacy| |codeql| |pypi| |downloads| |license| |docs| |github|
 
-High-Frequency Trading Backtesting Tool in Python
-=================================================
+High-Frequency Trading Backtesting Tool
+=======================================
 
-This Python framework is designed for developing high-frequency trading and market-making strategies. It focuses on accounting for both feed and order latencies, as well as the order queue position for order fill simulation. The framework aims to provide more accurate market replay-based backtesting, based on full order book and trade tick feed data.
+This framework is designed for developing high-frequency trading and market-making strategies. It focuses on accounting for both feed and order latencies, as well as the order queue position for order fill simulation. The framework aims to provide more accurate market replay-based backtesting, based on full order book and trade tick feed data.
+
+Rust implementation with experimental features
+==============================================
+
+The experimental features are currently in the early stages of development, having been completely rewritten in Rust to
+support the following features.
+
+* Backtesting of multi-asset and multi-exchange models
+* Deployment of a live trading bot using the same algo code.
+
+Please see `rust <https://github.com/nkaz001/hftbacktest/tree/master/rust>`_ directory.
 
 Key Features
 ============
 
 * Working in `Numba <https://numba.pydata.org/>`_ JIT function.
 * Complete tick-by-tick simulation with a variable time interval.
 * Full order book reconstruction based on L2 feeds(Market-By-Price).
@@ -25,15 +36,15 @@
 
 Getting started
 ===============
 
 Installation
 ------------
 
-hftbacktest supports Python 3.8+. You can install hftbacktest using ``pip``:
+hftbacktest supports Python 3.10+. You can install hftbacktest using ``pip``:
 
 .. code-block:: console
 
  pip install hftbacktest
 
 Or you can clone the latest development version from the Git repository with:
 
@@ -133,25 +144,14 @@
 * `Risk Mitigation through Price Protection in Extreme Market Conditions <https://hftbacktest.readthedocs.io/en/latest/tutorials/Risk%20Mitigation%20through%20Price%20Protection%20in%20Extreme%20Market%20Conditions.html>`_
 
 Examples
 ========
 
 You can find more examples in `examples <https://github.com/nkaz001/hftbacktest/tree/master/examples>`_ directory.
 
-Experimental features
-=====================
-
-The experimental features are currently in the early stages of development, having been completely rewritten in Rust to
-support the following features.
-
-* Backtesting of multi-asset and multi-exchange models
-* Deployment of a live trading bot using the same algo code.
-
-Please see `rust <https://github.com/nkaz001/hftbacktest/tree/master/rust>`_ directory.
-
 Contributing
 ============
 
 Thank you for considering contributing to hftbacktest! Welcome any and all help to improve the project. If you have an
 idea for an enhancement or a bug fix, please open an issue or discussion on GitHub to discuss it.
 
 The following items are examples of contributions you can make to this project:
```

### Comparing `hftbacktest-1.8.0/hftbacktest/__init__.py` & `hftbacktest-1.8.1/hftbacktest/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
     'validate_data',
     'correct_local_timestamp',
     'correct_exch_timestamp',
     'correct_exch_timestamp_adjust',
     'correct'
 )
 
-__version__ = '1.8.0'
+__version__ = '1.8.1'
 
 
 # JIT'ed latency models
 ConstantLatency = jitclass()(ConstantLatency_)
 FeedLatency = jitclass()(FeedLatency_)
 ForwardFeedLatency = jitclass()(ForwardFeedLatency_)
 BackwardFeedLatency = jitclass()(BackwardFeedLatency_)
```

### Comparing `hftbacktest-1.8.0/hftbacktest/assettype.py` & `hftbacktest-1.8.1/hftbacktest/assettype.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.0/hftbacktest/backtest.py` & `hftbacktest-1.8.1/hftbacktest/backtest.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.0/hftbacktest/data/__init__.py` & `hftbacktest-1.8.1/hftbacktest/data/__init__.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.0/hftbacktest/data/utils/binancefutures.py` & `hftbacktest-1.8.1/hftbacktest/data/utils/binancefutures.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,27 +8,30 @@
 from .. import validate_data
 from ..validation import correct_event_order, convert_to_struct_arr
 from ... import (
     DEPTH_EVENT,
     DEPTH_CLEAR_EVENT,
     DEPTH_SNAPSHOT_EVENT,
     TRADE_EVENT,
+    COL_EVENT,
     COL_EXCH_TIMESTAMP,
     COL_LOCAL_TIMESTAMP,
     correct_local_timestamp
 )
 
 
 def convert(
         input_filename: str,
         output_filename: Optional[str] = None,
         opt: Literal['', 'm', 't', 'mt'] = '',
         base_latency: float = 0,
         compress: bool = False,
-        structured_array: bool = False
+        structured_array: bool = False,
+        timestamp_unit: Literal['us', 'ns'] = 'us',
+        combined_stream: bool = True
 ) -> NDArray:
     r"""
     Converts raw Binance Futures feed stream file into a format compatible with HftBacktest.
 
     File Format:
 
     .. code-block::
@@ -61,45 +64,63 @@
                 - best bid: ``103``
                 - best ask: ``104``
 
         base_latency: The value to be added to the feed latency.
                       See :func:`.correct_local_timestamp`.
         compress: If this is set to True, the output file will be compressed.
         structured_array: If this is set to True, the output is converted into the new format(currently only Rust impl).
+        timestamp_unit: The timestamp unit for exchange timestamp to be converted in. Binance provides timestamps in
+                        milliseconds. Both local timestamp and exchange timestamp should be in the same unit.
+        combined_stream: Raw stream type.
+                         combined stream:
+                         {"stream":"solusdt@bookTicker","data":{"e":"bookTicker","u":4456408609867,"s":"SOLUSDT","b":"142.4440","B":"50","a":"142.4450","A":"3","T":1713571200009,"E":1713571200010}}
+                         regular stream:
+                         {"e":"bookTicker","u":4456408609867,"s":"SOLUSDT","b":"142.4440","B":"50","a":"142.4450","A":"3","T":1713571200009,"E":1713571200010}
 
     Returns:
         Converted data compatible with HftBacktest.
     """
+    if timestamp_unit == 'us':
+        timestamp_slice = 16
+        timestamp_mul = 1000
+    elif timestamp_unit == 'ns':
+        timestamp_slice = 19
+        timestamp_mul = 1000000
+    else:
+        raise ValueError
     rows = []
     with gzip.open(input_filename, 'r') as f:
         while True:
             line = f.readline()
             if not line:
                 break
-            local_timestamp = int(line[:16])
-            message = json.loads(line[17:])
-            data = message.get('data')
+            local_timestamp = int(line[:timestamp_slice])
+            message = json.loads(line[timestamp_slice + 1:])
+            if combined_stream:
+                data = message.get('data')
+            else:
+                data = message
             if data is not None:
                 evt = data['e']
                 if evt == 'trade':
                     if data['X'] != 'MARKET':
                         continue
                     # event_time = data['E']
                     transaction_time = data['T']
                     price = data['p']
                     qty = data['q']
                     side = -1 if data['m'] else 1  # trade initiator's side
-                    exch_timestamp = int(transaction_time) * 1000
+                    exch_timestamp = int(transaction_time) * timestamp_mul
                     rows.append([TRADE_EVENT, exch_timestamp, local_timestamp, side, float(price), float(qty)])
                 elif evt == 'depthUpdate':
                     # event_time = data['E']
                     transaction_time = data['T']
                     bids = data['b']
                     asks = data['a']
-                    exch_timestamp = int(transaction_time) * 1000
+                    exch_timestamp = int(transaction_time) * timestamp_mul
                     rows += [[DEPTH_EVENT, exch_timestamp, local_timestamp, 1, float(bid[0]), float(bid[1])] for bid in bids]
                     rows += [[DEPTH_EVENT, exch_timestamp, local_timestamp, -1, float(ask[0]), float(ask[1])] for ask in asks]
                 elif evt == 'markPriceUpdate' and 'm' in opt:
                     # event_time = data['E']
                     transaction_time = data['T']
                     index = data['i']
                     mark_price = data['p']
@@ -111,24 +132,24 @@
                 elif evt == 'bookTicker' and 't' in opt:
                     # event_time = data['E']
                     transaction_time = data['T']
                     bid_price = data['b']
                     bid_qty = data['B']
                     ask_price = data['a']
                     ask_qty = data['A']
-                    exch_timestamp = int(transaction_time) * 1000
+                    exch_timestamp = int(transaction_time) * timestamp_mul
                     rows.append([103, exch_timestamp, local_timestamp, 1, float(bid_price), float(bid_qty)])
                     rows.append([104, exch_timestamp, local_timestamp, -1, float(ask_price), float(ask_qty)])
             else:
                 # snapshot
                 # event_time = msg['E']
                 transaction_time = message['T']
                 bids = message['bids']
                 asks = message['asks']
-                exch_timestamp = int(transaction_time) * 1000
+                exch_timestamp = int(transaction_time) * timestamp_mul
                 if len(bids) > 0:
                     bid_clear_upto = float(bids[-1][0])
                     # clears the existing market depth upto the prices in the snapshot.
                     rows.append([DEPTH_CLEAR_EVENT, exch_timestamp, local_timestamp, 1, bid_clear_upto, 0])
                     # inserts the snapshot.
                     rows += [[DEPTH_SNAPSHOT_EVENT, exch_timestamp, local_timestamp, 1, float(bid[0]), float(bid[1])]
                              for bid in bids]
@@ -147,18 +168,19 @@
 
     print('Correcting the event order')
     sorted_exch_ts = merged[np.argsort(merged[:, COL_EXCH_TIMESTAMP], kind='mergesort')]
     sorted_local_ts = merged[np.argsort(merged[:, COL_LOCAL_TIMESTAMP], kind='mergesort')]
 
     data = correct_event_order(sorted_exch_ts, sorted_local_ts, structured_array)
 
-    # Validate again.
-    num_corr = validate_data(data)
-    if num_corr < 0:
-        raise ValueError
+    if not structured_array:
+        # Validate again.
+        num_corr = validate_data(data)
+        if num_corr < 0:
+            raise ValueError
 
     if structured_array:
         data = convert_to_struct_arr(data)
 
     if output_filename is not None:
         print('Saving to %s' % output_filename)
         if compress:
```

### Comparing `hftbacktest-1.8.0/hftbacktest/data/utils/binancehistmktdata.py` & `hftbacktest-1.8.1/hftbacktest/data/utils/binancehistmktdata.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.0/hftbacktest/data/utils/difforderbooksnapshot.py` & `hftbacktest-1.8.1/hftbacktest/data/utils/difforderbooksnapshot.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.0/hftbacktest/data/utils/snapshot.py` & `hftbacktest-1.8.1/hftbacktest/data/utils/snapshot.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.0/hftbacktest/data/utils/tardis.py` & `hftbacktest-1.8.1/hftbacktest/data/utils/tardis.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,19 +21,24 @@
         input_files: List[str],
         output_filename: Optional[str] = None,
         buffer_size: int = 100_000_000,
         ss_buffer_size: int = 1_000_000,
         base_latency: float = 0,
         snapshot_mode: Literal['process', 'ignore_sod', 'ignore'] = 'process',
         compress: bool = False,
-        structured_array: bool = False
+        structured_array: bool = False,
+        timestamp_unit: Literal['us', 'ns'] = 'us'
 ) -> NDArray:
     r"""
     Converts Tardis.dev data files into a format compatible with HftBacktest.
 
+    For Tardis's Binance Futures feed data, they use the 'E' event timestamp, representing the sending time, rather
+    than the 'T' transaction time, indicating when the matching occurs. So the latency is slightly less than it actually
+    is.
+
     Args:
         input_files: Input filenames for both incremental book and trades files,
                      e.g. ['incremental_book.csv', 'trades.csv'].
         output_filename: If provided, the converted data will be saved to the specified filename in ``npz`` format.
         buffer_size: Sets a preallocated row size for the buffer.
         ss_buffer_size: Sets a preallocated row size for the snapshot.
         base_latency: The value to be added to the feed latency.
@@ -44,18 +49,25 @@
                          Since Tardis intentionally adds the SOD snapshot, not due to a message ID gap or disconnection,
                          there might not be a need to process SOD snapshot to build a complete order book.
                          Please see https://docs.tardis.dev/historical-data-details#collected-order-book-data-details
                          for more details.
                        - Otherwise, all snapshot events will be processed.
         compress: If this is set to True, the output file will be compressed.
         structured_array: If this is set to True, the output is converted into the new format(currently only Rust impl).
-
+        timestamp_unit: The timestamp unit for timestamp to be converted in. Tardis provides timestamps in microseconds.
     Returns:
         Converted data compatible with HftBacktest.
     """
+    if timestamp_unit == 'us':
+        timestamp_mul = 1
+    elif timestamp_unit == 'ns':
+        timestamp_mul = 1000
+    else:
+        raise ValueError
+
     TRADE = 0
     DEPTH = 1
 
     sets = []
     for file in input_files:
         file_type = None
         tmp = np.empty((buffer_size, 6), np.float64)
@@ -99,16 +111,16 @@
                         'amount'
                     ]:
                         file_type = DEPTH
                 elif file_type == TRADE:
                     # Insert TRADE_EVENT
                     tmp[row_num] = [
                         TRADE_EVENT,
-                        int(cols[2]),
-                        int(cols[3]),
+                        int(cols[2]) * timestamp_mul,
+                        int(cols[3]) * timestamp_mul,
                         1 if cols[5] == 'buy' else -1,
                         float(cols[6]),
                         float(cols[7])
                     ]
                     row_num += 1
                 elif file_type == DEPTH:
                     if cols[4] == 'true':
@@ -120,26 +132,26 @@
                             ss_bid = np.empty((ss_buffer_size, 6), np.float64)
                             ss_ask = np.empty((ss_buffer_size, 6), np.float64)
                             ss_bid_rn = 0
                             ss_ask_rn = 0
                         if cols[5] == 'bid':
                             ss_bid[ss_bid_rn] = [
                                 DEPTH_SNAPSHOT_EVENT,
-                                int(cols[2]),
-                                int(cols[3]),
+                                int(cols[2]) * timestamp_mul,
+                                int(cols[3]) * timestamp_mul,
                                 1,
                                 float(cols[6]),
                                 float(cols[7])
                             ]
                             ss_bid_rn += 1
                         else:
                             ss_ask[ss_ask_rn] = [
                                 DEPTH_SNAPSHOT_EVENT,
-                                int(cols[2]),
-                                int(cols[3]),
+                                int(cols[2]) * timestamp_mul,
+                                int(cols[3]) * timestamp_mul,
                                 -1,
                                 float(cols[6]),
                                 float(cols[7])
                             ]
                             ss_ask_rn += 1
                     else:
                         is_sod_snapshot = False
@@ -180,16 +192,16 @@
                                 # Add DEPTH_SNAPSHOT_EVENT for the ask snapshot
                                 tmp[row_num:row_num + len(ss_ask)] = ss_ask[:]
                                 row_num += len(ss_ask)
                             ss_ask = None
                         # Insert DEPTH_EVENT
                         tmp[row_num] = [
                             DEPTH_EVENT,
-                            int(cols[2]),
-                            int(cols[3]),
+                            int(cols[2]) * timestamp_mul,
+                            int(cols[3]) * timestamp_mul,
                             1 if cols[5] == 'bid' else -1,
                             float(cols[6]),
                             float(cols[7])
                         ]
                         row_num += 1
         sets.append(tmp[:row_num])
 
@@ -201,18 +213,19 @@
 
     print('Correcting the event order')
     sorted_exch_ts = merged[np.argsort(merged[:, COL_EXCH_TIMESTAMP], kind='mergesort')]
     sorted_local_ts = merged[np.argsort(merged[:, COL_LOCAL_TIMESTAMP], kind='mergesort')]
 
     data = correct_event_order(sorted_exch_ts, sorted_local_ts, structured_array)
 
-    # Validate again.
-    num_corr = validate_data(data)
-    if num_corr < 0:
-        raise ValueError
+    if not structured_array:
+        # Validate again.
+        num_corr = validate_data(data)
+        if num_corr < 0:
+            raise ValueError
 
     if structured_array:
         data = convert_to_struct_arr(data)
 
     if output_filename is not None:
         print('Saving to %s' % output_filename)
         if compress:
```

### Comparing `hftbacktest-1.8.0/hftbacktest/data/validation.py` & `hftbacktest-1.8.1/hftbacktest/data/validation.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.0/hftbacktest/marketdepth.py` & `hftbacktest-1.8.1/hftbacktest/marketdepth.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.0/hftbacktest/models/latencies.py` & `hftbacktest-1.8.1/hftbacktest/models/latencies.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.0/hftbacktest/models/queue.py` & `hftbacktest-1.8.1/hftbacktest/models/queue.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.0/hftbacktest/order.py` & `hftbacktest-1.8.1/hftbacktest/order.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.0/hftbacktest/proc/local.py` & `hftbacktest-1.8.1/hftbacktest/proc/local.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.0/hftbacktest/proc/nopartialfillexchange.py` & `hftbacktest-1.8.1/hftbacktest/proc/nopartialfillexchange.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.0/hftbacktest/proc/partialfillexchange.py` & `hftbacktest-1.8.1/hftbacktest/proc/partialfillexchange.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,15 +199,15 @@
                 timestamp,
                 True
             )
         elif order.price_tick == price_tick:
             # Update the order's queue position.
             self.queue_model.trade(order, qty, self)
             if self.queue_model.is_filled(order, self):
-                q_qty = np.ceil(-order.q[0] / self.depth.lot_size) * self.depth.lot_size
+                q_qty = np.floor(-order.q[0] / self.depth.lot_size) * self.depth.lot_size
                 exec_qty = min(q_qty, qty, order.leaves_qty)
                 self.__fill(
                     order,
                     exec_qty,
                     timestamp,
                     True
                 )
@@ -220,15 +220,15 @@
                 timestamp,
                 True
             )
         elif order.price_tick == price_tick:
             # Update the order's queue position.
             self.queue_model.trade(order, qty, self)
             if self.queue_model.is_filled(order, self):
-                q_qty = np.ceil(-order.q[0] / self.depth.lot_size) * self.depth.lot_size
+                q_qty = np.floor(-order.q[0] / self.depth.lot_size) * self.depth.lot_size
                 exec_qty = min(q_qty, qty, order.leaves_qty)
                 self.__fill(
                     order,
                     exec_qty,
                     timestamp,
                     True
                 )
```

### Comparing `hftbacktest-1.8.0/hftbacktest/proc/proc.py` & `hftbacktest-1.8.1/hftbacktest/proc/proc.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.0/hftbacktest/reader.py` & `hftbacktest-1.8.1/hftbacktest/reader.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.0/hftbacktest/stat.py` & `hftbacktest-1.8.1/hftbacktest/stat.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.0/hftbacktest/state.py` & `hftbacktest-1.8.1/hftbacktest/state.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.0/hftbacktest/stats.py` & `hftbacktest-1.8.1/hftbacktest/stats.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.0/hftbacktest/typing.py` & `hftbacktest-1.8.1/hftbacktest/typing.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.0/hftbacktest.egg-info/PKG-INFO` & `hftbacktest-1.8.1/hftbacktest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hftbacktest
-Version: 1.8.0
+Version: 1.8.1
 Summary: High-frequency trading and market making backtesting tool
 Home-page: https://github.com/nkaz001/hftbacktest
 Author: nkaz001
 Author-email: nkaz001@protonmail.com
 License: MIT
 Project-URL: Docs, https://hftbacktest.readthedocs.io/en/latest/
 Project-URL: GitHub: issues, https://github.com/nkaz001/hftbacktest/issues
@@ -17,27 +17,38 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Office/Business :: Financial :: Investment
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 License-File: LICENSE
 
 ===========
 HftBacktest
 ===========
 
 |codacy| |codeql| |pypi| |downloads| |license| |docs| |github|
 
-High-Frequency Trading Backtesting Tool in Python
-=================================================
+High-Frequency Trading Backtesting Tool
+=======================================
 
-This Python framework is designed for developing high-frequency trading and market-making strategies. It focuses on accounting for both feed and order latencies, as well as the order queue position for order fill simulation. The framework aims to provide more accurate market replay-based backtesting, based on full order book and trade tick feed data.
+This framework is designed for developing high-frequency trading and market-making strategies. It focuses on accounting for both feed and order latencies, as well as the order queue position for order fill simulation. The framework aims to provide more accurate market replay-based backtesting, based on full order book and trade tick feed data.
+
+Rust implementation with experimental features
+==============================================
+
+The experimental features are currently in the early stages of development, having been completely rewritten in Rust to
+support the following features.
+
+* Backtesting of multi-asset and multi-exchange models
+* Deployment of a live trading bot using the same algo code.
+
+Please see `rust <https://github.com/nkaz001/hftbacktest/tree/master/rust>`_ directory.
 
 Key Features
 ============
 
 * Working in `Numba <https://numba.pydata.org/>`_ JIT function.
 * Complete tick-by-tick simulation with a variable time interval.
 * Full order book reconstruction based on L2 feeds(Market-By-Price).
@@ -51,15 +62,15 @@
 
 Getting started
 ===============
 
 Installation
 ------------
 
-hftbacktest supports Python 3.8+. You can install hftbacktest using ``pip``:
+hftbacktest supports Python 3.10+. You can install hftbacktest using ``pip``:
 
 .. code-block:: console
 
  pip install hftbacktest
 
 Or you can clone the latest development version from the Git repository with:
 
@@ -159,25 +170,14 @@
 * `Risk Mitigation through Price Protection in Extreme Market Conditions <https://hftbacktest.readthedocs.io/en/latest/tutorials/Risk%20Mitigation%20through%20Price%20Protection%20in%20Extreme%20Market%20Conditions.html>`_
 
 Examples
 ========
 
 You can find more examples in `examples <https://github.com/nkaz001/hftbacktest/tree/master/examples>`_ directory.
 
-Experimental features
-=====================
-
-The experimental features are currently in the early stages of development, having been completely rewritten in Rust to
-support the following features.
-
-* Backtesting of multi-asset and multi-exchange models
-* Deployment of a live trading bot using the same algo code.
-
-Please see `rust <https://github.com/nkaz001/hftbacktest/tree/master/rust>`_ directory.
-
 Contributing
 ============
 
 Thank you for considering contributing to hftbacktest! Welcome any and all help to improve the project. If you have an
 idea for an enhancement or a bug fix, please open an issue or discussion on GitHub to discuss it.
 
 The following items are examples of contributions you can make to this project:
```

### Comparing `hftbacktest-1.8.0/hftbacktest.egg-info/SOURCES.txt` & `hftbacktest-1.8.1/hftbacktest.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -22,21 +22,14 @@
 hftbacktest/data/validation.py
 hftbacktest/data/utils/__init__.py
 hftbacktest/data/utils/binancefutures.py
 hftbacktest/data/utils/binancehistmktdata.py
 hftbacktest/data/utils/difforderbooksnapshot.py
 hftbacktest/data/utils/snapshot.py
 hftbacktest/data/utils/tardis.py
-hftbacktest/experimental/__init__.py
-hftbacktest/experimental/live/__init__.py
-hftbacktest/experimental/live/binancefutures.py
-hftbacktest/experimental/live/custom_strategy.py
-hftbacktest/experimental/live/livebroker.py
-hftbacktest/experimental/live/ordermanager.py
-hftbacktest/experimental/live/settings.py
 hftbacktest/models/__init__.py
 hftbacktest/models/latencies.py
 hftbacktest/models/queue.py
 hftbacktest/proc/__init__.py
 hftbacktest/proc/local.py
 hftbacktest/proc/nopartialfillexchange.py
 hftbacktest/proc/partialfillexchange.py
```

### Comparing `hftbacktest-1.8.0/setup.cfg` & `hftbacktest-1.8.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -29,21 +29,21 @@
 	
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	
 	Topic :: Office/Business :: Financial :: Investment
 
 [options]
-python_requires = >=3.8
+python_requires = >=3.10
 packages = find:
 zip_safe = False
 include_package_data = True
 install_requires = 
-	numba ~= 0.57
-	numpy < 1.25, >= 1.21
+	numba ~= 0.59
+	numpy < 1.27, >= 1.22
 	pandas
 	matplotlib
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

