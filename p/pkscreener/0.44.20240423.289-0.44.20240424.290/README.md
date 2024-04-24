# Comparing `tmp/pkscreener-0.44.20240423.289.tar.gz` & `tmp/pkscreener-0.44.20240424.290.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240423.289.tar", last modified: Tue Apr 23 23:41:57 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240424.290.tar", last modified: Wed Apr 24 10:49:30 2024, max compression
```

## Comparing `pkscreener-0.44.20240423.289.tar` & `pkscreener-0.44.20240424.290.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 23:41:57.121715 pkscreener-0.44.20240423.289/
--rw-rw-rw-   0        0        0     1086 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-04-23 23:41:57.121715 pkscreener-0.44.20240423.289/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 23:41:57.105994 pkscreener-0.44.20240423.289/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 23:41:57.121715 pkscreener-0.44.20240423.289/pkscreener/classes/
--rw-rw-rw-   0        0        0    10156 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    25815 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0     9868 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0     7038 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3237 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    29415 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    10999 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    20931 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    19689 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8120 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    17306 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   113351 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    51052 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    81010 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-04-23 23:41:46.000000 pkscreener-0.44.20240423.289/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     4935 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   122733 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/globals.py
--rw-rw-rw-   0        0        0      595 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    48027 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    23654 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-04-23 23:41:57.105994 pkscreener-0.44.20240423.289/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-04-23 23:41:57.000000 pkscreener-0.44.20240423.289/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1318 2024-04-23 23:41:57.000000 pkscreener-0.44.20240423.289/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 23:41:57.000000 pkscreener-0.44.20240423.289/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-04-23 23:41:57.000000 pkscreener-0.44.20240423.289/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-23 23:41:57.000000 pkscreener-0.44.20240423.289/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-04-23 23:41:57.000000 pkscreener-0.44.20240423.289/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-23 23:41:57.121715 pkscreener-0.44.20240423.289/setup.cfg
--rw-rw-rw-   0        0        0     4727 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 10:49:30.436711 pkscreener-0.44.20240424.290/
+-rw-rw-rw-   0        0        0     1086 2024-04-24 10:42:24.000000 pkscreener-0.44.20240424.290/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-04-24 10:42:24.000000 pkscreener-0.44.20240424.290/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-04-24 10:49:30.436711 pkscreener-0.44.20240424.290/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-04-24 10:42:24.000000 pkscreener-0.44.20240424.290/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 10:49:30.420402 pkscreener-0.44.20240424.290/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-04-24 10:42:24.000000 pkscreener-0.44.20240424.290/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 10:49:30.436711 pkscreener-0.44.20240424.290/pkscreener/classes/
+-rw-rw-rw-   0        0        0    10156 2024-04-24 10:42:24.000000 pkscreener-0.44.20240424.290/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-04-24 10:42:24.000000 pkscreener-0.44.20240424.290/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-04-24 10:42:24.000000 pkscreener-0.44.20240424.290/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-04-24 10:42:24.000000 pkscreener-0.44.20240424.290/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    25815 2024-04-24 10:42:24.000000 pkscreener-0.44.20240424.290/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0     9868 2024-04-24 10:42:24.000000 pkscreener-0.44.20240424.290/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     7038 2024-04-24 10:42:24.000000 pkscreener-0.44.20240424.290/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-04-24 10:42:24.000000 pkscreener-0.44.20240424.290/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    29415 2024-04-24 10:42:24.000000 pkscreener-0.44.20240424.290/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    10999 2024-04-24 10:42:24.000000 pkscreener-0.44.20240424.290/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    20931 2024-04-24 10:42:24.000000 pkscreener-0.44.20240424.290/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    19689 2024-04-24 10:42:24.000000 pkscreener-0.44.20240424.290/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-04-24 10:42:24.000000 pkscreener-0.44.20240424.290/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8120 2024-04-24 10:42:24.000000 pkscreener-0.44.20240424.290/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-04-24 10:42:24.000000 pkscreener-0.44.20240424.290/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-04-24 10:42:24.000000 pkscreener-0.44.20240424.290/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    17306 2024-04-24 10:42:24.000000 pkscreener-0.44.20240424.290/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-04-24 10:42:24.000000 pkscreener-0.44.20240424.290/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-04-24 10:42:24.000000 pkscreener-0.44.20240424.290/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   113351 2024-04-24 10:42:24.000000 pkscreener-0.44.20240424.290/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    51052 2024-04-24 10:42:24.000000 pkscreener-0.44.20240424.290/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-04-24 10:42:24.000000 pkscreener-0.44.20240424.290/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    81600 2024-04-24 10:42:24.000000 pkscreener-0.44.20240424.290/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-04-24 10:42:24.000000 pkscreener-0.44.20240424.290/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-04-24 10:49:16.000000 pkscreener-0.44.20240424.290/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     4935 2024-04-24 10:42:24.000000 pkscreener-0.44.20240424.290/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-04-24 10:42:24.000000 pkscreener-0.44.20240424.290/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   122769 2024-04-24 10:42:24.000000 pkscreener-0.44.20240424.290/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      595 2024-04-24 10:42:25.000000 pkscreener-0.44.20240424.290/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    48027 2024-04-24 10:42:25.000000 pkscreener-0.44.20240424.290/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    25380 2024-04-24 10:42:25.000000 pkscreener-0.44.20240424.290/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-04-24 10:49:30.436711 pkscreener-0.44.20240424.290/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-04-24 10:49:30.000000 pkscreener-0.44.20240424.290/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1318 2024-04-24 10:49:30.000000 pkscreener-0.44.20240424.290/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 10:49:30.000000 pkscreener-0.44.20240424.290/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-04-24 10:49:30.000000 pkscreener-0.44.20240424.290/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-24 10:49:30.000000 pkscreener-0.44.20240424.290/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-04-24 10:49:30.000000 pkscreener-0.44.20240424.290/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-24 10:49:30.436711 pkscreener-0.44.20240424.290/setup.cfg
+-rw-rw-rw-   0        0        0     4727 2024-04-24 10:42:25.000000 pkscreener-0.44.20240424.290/setup.py
```

### Comparing `pkscreener-0.44.20240423.289/LICENSE` & `pkscreener-0.44.20240424.290/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.289/LICENSE-Others` & `pkscreener-0.44.20240424.290/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.289/PKG-INFO` & `pkscreener-0.44.20240424.290/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240423.289
+Version: 0.44.20240424.290
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240423.289.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240424.290.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240423.288/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240423.289/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240423.288/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240423.289/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240423.288/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240423.289/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240423.289/README.md` & `pkscreener-0.44.20240424.290/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240423.288/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240423.289/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240423.288/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240423.289/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240423.288/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240423.289/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240423.289/pkscreener/__init__.py` & `pkscreener-0.44.20240424.290/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.289/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240424.290/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.289/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240424.290/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.289/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240424.290/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.289/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240424.290/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.289/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240424.290/pkscreener/classes/ConfigManager.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         self.showPastStrategyData = False
         # This determines how many days apart the backtest calculations are run.
         # For example, for weekly backtest calculations, set this to 5 (5 days = 1 week)
         # For fortnightly, set this to 10 and so on (10 trading sessions = 2 weeks)
         self.backtestPeriodFactor = 1
         self.maxDashboardWidgetsPerRow = 6
         self.calculatersiintraday = False
-        self.defaultMonitorOptions = "X:12:9:2.5,|X:0:5:0:50:i 1m,X:12:2,X:12:5:0:30,X:12:6:3,X:12:6:7:1,X:12:6:8,X:12:6:9,X:12:6:10:1,X:12:7:3:.02:1,X:12:7:6:1,X:12:17,X:12:23,X:12:24,X:12:10,X:12:12:i 1m,X:12:12:i 5m,X:12:13:i 1m"
+        self.defaultMonitorOptions = "X:12:9:2.5,|X:0:5:0:40:i 1m,X:12:2,X:12:5:0:30,X:12:6:3,X:12:6:7:1,X:12:6:8,X:12:6:9,X:12:6:10:1,X:12:7:3:.02:1,X:12:7:6:1,X:12:17,X:12:23,X:12:24,X:12:10,X:12:12:i 1m,X:12:12:i 5m,X:12:13:i 1m"
 
         self.daysToLookback = 22 * self.backtestPeriodFactor  # 1 month
         self.periods = [1,2,3,4,5,10,15,22,30]
         if self.maxBacktestWindow > self.periods[-1]:
             self.periods.extend(self.maxBacktestWindow)
 
     @property
```

### Comparing `pkscreener-0.44.20240423.289/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240424.290/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.289/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240424.290/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.289/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240424.290/pkscreener/classes/MarketStatus.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,18 +18,20 @@
     FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
     AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
     LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
     OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
     SOFTWARE.
 
 """
-
+import os
 from PKNSETools.PKNSEStockDataFetcher import nseStockDataFetcher
 from PKDevTools.classes.Singleton import SingletonType, SingletonMixin
 from PKDevTools.classes.log import default_logger
+from PKDevTools.classes.SuppressOutput import SuppressOutput
+from PKDevTools.classes import log as log
 
 class MarketStatus(SingletonMixin, metaclass=SingletonType):
     nseFetcher = nseStockDataFetcher()
     def __init__(self):
         super(MarketStatus, self).__init__()
 
     @property
@@ -57,20 +59,24 @@
     @marketStatus.setter
     def marketStatus(self, status):
         self.attributes["marketStatus"] = status
 
     def getMarketStatus(self, progress=None, task_id=0, exchangeSymbol="^NSEI",namedOnly=False):
         lngStatus = ""
         try:
-            if progress:
-                progress[task_id] = {"progress": 0, "total": 1}
-            _,lngStatus,_ = MarketStatus.nseFetcher.capitalMarketStatus(exchange=exchangeSymbol)
-            if exchangeSymbol in ["^NSEI","^BSESN"] and not namedOnly:
-                _,bseStatus,_ = MarketStatus.nseFetcher.capitalMarketStatus(exchange="^BSESN")
-                lngStatus = f"{lngStatus} | {bseStatus}"
+            suppressLogs = True
+            if "PKDevTools_Default_Log_Level" in os.environ.keys():
+                suppressLogs = os.environ["PKDevTools_Default_Log_Level"] == str(log.logging.NOTSET)
+            with SuppressOutput(suppress_stdout=suppressLogs, suppress_stderr=suppressLogs):
+                if progress:
+                    progress[task_id] = {"progress": 0, "total": 1}
+                _,lngStatus,_ = MarketStatus.nseFetcher.capitalMarketStatus(exchange=exchangeSymbol)
+                if exchangeSymbol in ["^NSEI","^BSESN"] and not namedOnly:
+                    _,bseStatus,_ = MarketStatus.nseFetcher.capitalMarketStatus(exchange="^BSESN")
+                    lngStatus = f"{lngStatus} | {bseStatus}"
             if progress:
                 progress[task_id] = {"progress": 1, "total": 1}
         except Exception as e:# pragma: no cover
             default_logger().debug(e, exc_info=True)
             pass
         self.marketStatus = lngStatus
         return lngStatus
```

### Comparing `pkscreener-0.44.20240423.289/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240424.290/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.289/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240424.290/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.289/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240424.290/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.289/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240424.290/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.289/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240424.290/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.289/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240424.290/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.289/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240424.290/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.289/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240424.290/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.289/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240424.290/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.289/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240424.290/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.289/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240424.290/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.289/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240424.290/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.289/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240424.290/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.289/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240424.290/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.289/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240424.290/pkscreener/classes/Utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -791,15 +791,15 @@
                 default_logger().debug(e, exc_info=True)
         else:
             OutputControls().printOutput(
                 colorText.BOLD + colorText.GREEN + "=> Already Cached." + colorText.END
             )
 
     def downloadLatestData(stockDict,configManager,stockCodes=[],exchangeSuffix=".NS",downloadOnly=False):
-        numStocksPerIteration = int(len(stockCodes)/5) + 1
+        numStocksPerIteration = int(len(stockCodes)/int(len(stockCodes)/10)) + 1
         queueCounter = 0
         iterations = int(len(stockCodes)/numStocksPerIteration) + 1
         tasksList = []
         while queueCounter < iterations:
             stocks = []
             if queueCounter < iterations:
                 stocks = stockCodes[numStocksPerIteration* queueCounter : numStocksPerIteration* (queueCounter + 1)]
@@ -810,15 +810,18 @@
             task.userData = stocks
             if len(stocks) > 0:
                 tasksList.append(task)
             queueCounter += 1
         
         processedStocks = []
         if len(tasksList) > 0:
-            PKScheduler.scheduleTasks(tasksList=tasksList, label=f"Downloading latest data [{configManager.period},{configManager.duration}] (Total={len(stockCodes)} records in {len(tasksList)} batches){'Be Patient!' if len(stockCodes)> 2000 else ''}",timeout=3*configManager.longTimeout*(4 if downloadOnly else 1),minAcceptableCompletionPercentage=(100 if downloadOnly else 80))
+            PKScheduler.scheduleTasks(tasksList=tasksList, 
+                                      label=f"Downloading latest data [{configManager.period},{configManager.duration}] (Total={len(stockCodes)} records in {len(tasksList)} batches){'Be Patient!' if len(stockCodes)> 2000 else ''}",
+                                      timeout=(5+2.5*configManager.longTimeout*(4 if downloadOnly else 1)), # 5 sec additional time for multiprocessing setup
+                                      minAcceptableCompletionPercentage=(100 if downloadOnly else 100))
             for task in tasksList:
                 if task.result is not None:
                     for stock in task.userData:
                         taskResult = task.result.get(f"{stock}{exchangeSuffix}")
                         if taskResult is not None:
                             stockDict[stock] = taskResult.to_dict("split")
                             processedStocks.append(stock)
@@ -839,17 +842,19 @@
     ):
         isIntraday = isIntraday or configManager.isIntradayConfig()
         exists, cache_file = tools.afterMarketStockDataExists(
             isIntraday, forceLoad=forceLoad
         )
         initialLoadCount = len(stockDict)
         leftOutStocks = None
+        recentDownloadFromOriginAttempted = False
         isTrading = PKDateUtilities.isTradingTime() and not PKDateUtilities.isTodayHoliday()[0]
         # stockCodes is not None mandates that we start our work based on the downloaded data from yesterday
         if (stockCodes is not None and len(stockCodes) > 0) and (isTrading or downloadOnly):
+            recentDownloadFromOriginAttempted = True
             stockDict, leftOutStocks = tools.downloadLatestData(stockDict,configManager,stockCodes,exchangeSuffix=exchangeSuffix,downloadOnly=downloadOnly)
             if len(leftOutStocks) > int(len(stockCodes)*0.05):
                 # More than 5 % of stocks are still remaining
                 stockDict, _ = tools.downloadLatestData(stockDict,configManager,leftOutStocks,exchangeSuffix=exchangeSuffix,downloadOnly=downloadOnly)
             # return stockDict
         if downloadOnly or isTrading:
             # We don't want to download from local stale pkl file or stale file at server
@@ -872,21 +877,24 @@
         if not stockDataLoaded:
             OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.FAIL
                 + "[+] Cache unavailable on pkscreener server, Continuing.."
                 + colorText.END
             )
+        if not stockDataLoaded and not recentDownloadFromOriginAttempted:
+            stockDict, _ = tools.downloadLatestData(stockDict,configManager,stockCodes,exchangeSuffix=exchangeSuffix,downloadOnly=downloadOnly)
         # See if we need to save stock data
         stockDataLoaded = stockDataLoaded or (len(stockDict) > 0 and (len(stockDict) != initialLoadCount))
         if stockDataLoaded:
             tools.saveStockData(stockDict,configManager,initialLoadCount,isIntraday,downloadOnly, forceSave=stockDataLoaded)
         return stockDict
 
     def loadDataFromLocalPickle(stockDict, configManager, downloadOnly, defaultAnswer, exchangeSuffix, cache_file, isTrading):
+        stockDataLoaded = False
         with open(
                 os.path.join(Archiver.get_user_outputs_dir(), cache_file), "rb"
             ) as f:
             try:
                 stockData = pickle.load(f)
                 if not downloadOnly:
                     OutputControls().printOutput(
@@ -958,14 +966,15 @@
                         + colorText.END
                     )
                 if tools.promptFileExists(defaultAnswer=defaultAnswer) == "Y":
                     configManager.deleteFileWithPattern()
         return stockDict, stockDataLoaded
 
     def downloadSavedDataFromServer(stockDict, configManager, downloadOnly, defaultAnswer, retrial, forceLoad, stockCodes, exchangeSuffix, isIntraday, forceRedownload, cache_file, isTrading):
+        stockDataLoaded = False
         OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.FAIL
                     + "[+] Market Stock Data is not cached, or forced to redownload .."
                     + colorText.END
                 )
         OutputControls().printOutput(
```

### Comparing `pkscreener-0.44.20240423.289/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240424.290/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.289/pkscreener/classes/keys.py` & `pkscreener-0.44.20240424.290/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.289/pkscreener/courbd.ttf` & `pkscreener-0.44.20240424.290/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.289/pkscreener/globals.py` & `pkscreener-0.44.20240424.290/pkscreener/globals.py`

 * *Files 0% similar despite different names*

```diff
@@ -1523,14 +1523,15 @@
     isIntraday = userPassedArgs.intraday is not None
     if configManager.isIntradayConfig() or isIntraday:
         configManager.toggleConfig(candleDuration="1d", clearCache=False)
 
 def prepareStocksForScreening(testing, downloadOnly, listStockCodes, indexOption):
     if not downloadOnly:
         updateMenuChoiceHierarchy()
+    indexOption = int(indexOption)
     if listStockCodes is None or len(listStockCodes) == 0:
         if indexOption >= 0 and indexOption <= 14:
             shouldSuppress = not OutputControls().enableMultipleLineOutput
             with SuppressOutput(suppress_stderr=shouldSuppress, suppress_stdout=shouldSuppress):
                 listStockCodes = fetcher.fetchStockCodes(
                                 indexOption, stockCode=None
                             )
```

### Comparing `pkscreener-0.44.20240423.289/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240424.290/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.289/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240424.290/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.289/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240424.290/pkscreener/pkscreenercli.py`

 * *Files 4% similar despite different names*

```diff
@@ -364,55 +364,86 @@
                     dbTimestamp = PKDateUtilities.currentDateTime().strftime("%H:%M:%S")
                     elapsed_time = 0
                     if start_time is None:
                         start_time = time.time()
                     else:
                         elapsed_time = round(time.time() - start_time,2)
                         start_time = time.time()
-                if MarketMonitor().monitorIndex == 0 and args.options is not None:
-                    # Load the stock data afresh for each cycle
-                    refreshStockData(args.options)
                 monitorOption_org = MarketMonitor().currentMonitorOption()
                 monitorOption = monitorOption_org
                 lastComponent = monitorOption.split(":")[-1]
                 if "i" in lastComponent:
                     # We need to switch to intraday scan
                     monitorOption = monitorOption.replace(lastComponent,"")
                     args.intraday = lastComponent.replace("i","").strip()
+                    configManager.toggleConfig(candleDuration=args.intraday, clearCache=False)
                 else:
                     # We need to switch to daily scan
                     args.intraday = None
                     configManager.toggleConfig(candleDuration='1d', clearCache=False)
                 if monitorOption.startswith("|"):
                     monitorOption = monitorOption.replace("|","")
                     # We need to pipe the output from previous run into the next one
                     if resultStocks is not None:
                         resultStocks = ",".join(resultStocks)
                         monitorOption = f"{monitorOption}:{resultStocks}"
-                args.options = monitorOption
+                args.options = monitorOption.replace("::",":")
+                if MarketMonitor().monitorIndex == 1 and args.options is not None and plainResults is not None:
+                    # Load the stock data afresh for each cycle
+                    refreshStockData(args.options)
             try: 
                 results = None
                 plainResults = None
                 resultStocks = None
                 results, plainResults = main(userArgs=args)
                 if isInterrupted():
                     sys.exit(0)
+                # while pipeResults(plainResults,args):
+                #     results, plainResults = main(userArgs=args)
             except SystemExit:
                 sys.exit(0)
-            except Exception:
-                # traceback.print_exc()
+            except Exception as e:
+                default_logger().debug(e, exc_info=True)
                 # Probably user cancelled an operation by choosing a cancel sub-menu somewhere
                 pass
             if plainResults is not None and not plainResults.empty:
                 plainResults = plainResults[~plainResults.index.duplicated(keep='first')]
                 results = results[~results.index.duplicated(keep='first')]
                 resultStocks = plainResults.index
             if results is not None and args.monitor and len(monitorOption_org) > 0:
                 MarketMonitor().refresh(screen_df=results,screenOptions=monitorOption_org, chosenMenu=updateMenuChoiceHierarchy(),dbTimestamp=f"{dbTimestamp} | CycleTime:{elapsed_time}s")
 
+def pipeResults(prevOutput,args):
+    nextOnes = args.options.split(";")
+    if len(nextOnes) > 1:
+        monitorOption = nextOnes[1]
+        if len(monitorOption) == 0:
+            return False
+        lastComponent = monitorOption.split(":")[-1]
+        if "i" in lastComponent:
+            # We need to switch to intraday scan
+            monitorOption = monitorOption.replace(lastComponent,"")
+            args.intraday = lastComponent.replace("i","").strip()
+            configManager.toggleConfig(candleDuration=args.intraday, clearCache=False)
+        else:
+            # We need to switch to daily scan
+            args.intraday = None
+            configManager.toggleConfig(candleDuration='1d', clearCache=False)
+        if monitorOption.startswith("|"):
+            monitorOption = monitorOption.replace("|","")
+            # We need to pipe the output from previous run into the next one
+            if prevOutput is not None and not prevOutput.empty:
+                prevOutput_results = prevOutput[~prevOutput.index.duplicated(keep='first')]
+                prevOutput_results = prevOutput_results.index
+                prevOutput_results = ",".join(prevOutput_results)
+                monitorOption = f"{monitorOption}:{prevOutput_results}"
+        args.options = monitorOption.replace("::",":")
+        args.options = args.options + ";".join(nextOnes[2:])
+        return True
+    return False
 
 def pkscreenercli():
     global originalStdOut
     if sys.platform.startswith("darwin"):
         try:
             multiprocessing.set_start_method("fork")
         except RuntimeError as e:# pragma: no cover
```

### Comparing `pkscreener-0.44.20240423.289/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240424.290/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240423.289
+Version: 0.44.20240424.290
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240423.289.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240424.290.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240423.288/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240423.289/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240423.288/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240423.289/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240423.288/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240423.289/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240423.289/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240424.290/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.289/setup.py` & `pkscreener-0.44.20240424.290/setup.py`

 * *Files identical despite different names*

