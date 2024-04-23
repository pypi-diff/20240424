# Comparing `tmp/pkscreener-0.44.20240423.288.tar.gz` & `tmp/pkscreener-0.44.20240423.289.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240423.288.tar", last modified: Tue Apr 23 22:31:19 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240423.289.tar", last modified: Tue Apr 23 23:41:57 2024, max compression
```

## Comparing `pkscreener-0.44.20240423.288.tar` & `pkscreener-0.44.20240423.289.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 22:31:19.331580 pkscreener-0.44.20240423.288/
--rw-rw-rw-   0        0        0     1086 2024-04-23 22:26:48.000000 pkscreener-0.44.20240423.288/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-04-23 22:26:48.000000 pkscreener-0.44.20240423.288/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-04-23 22:31:19.331580 pkscreener-0.44.20240423.288/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-04-23 22:26:48.000000 pkscreener-0.44.20240423.288/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 22:31:19.315962 pkscreener-0.44.20240423.288/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-04-23 22:26:48.000000 pkscreener-0.44.20240423.288/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 22:31:19.331580 pkscreener-0.44.20240423.288/pkscreener/classes/
--rw-rw-rw-   0        0        0    10156 2024-04-23 22:26:48.000000 pkscreener-0.44.20240423.288/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-04-23 22:26:48.000000 pkscreener-0.44.20240423.288/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-04-23 22:26:48.000000 pkscreener-0.44.20240423.288/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-04-23 22:26:48.000000 pkscreener-0.44.20240423.288/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    25815 2024-04-23 22:26:48.000000 pkscreener-0.44.20240423.288/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0     9868 2024-04-23 22:26:48.000000 pkscreener-0.44.20240423.288/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0     7038 2024-04-23 22:26:48.000000 pkscreener-0.44.20240423.288/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3237 2024-04-23 22:26:48.000000 pkscreener-0.44.20240423.288/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    29415 2024-04-23 22:26:48.000000 pkscreener-0.44.20240423.288/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    10999 2024-04-23 22:26:48.000000 pkscreener-0.44.20240423.288/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    20931 2024-04-23 22:26:48.000000 pkscreener-0.44.20240423.288/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    19689 2024-04-23 22:26:48.000000 pkscreener-0.44.20240423.288/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-04-23 22:26:48.000000 pkscreener-0.44.20240423.288/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8120 2024-04-23 22:26:48.000000 pkscreener-0.44.20240423.288/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-04-23 22:26:48.000000 pkscreener-0.44.20240423.288/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-04-23 22:26:48.000000 pkscreener-0.44.20240423.288/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    17306 2024-04-23 22:26:48.000000 pkscreener-0.44.20240423.288/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-04-23 22:26:48.000000 pkscreener-0.44.20240423.288/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-04-23 22:26:48.000000 pkscreener-0.44.20240423.288/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   113351 2024-04-23 22:26:48.000000 pkscreener-0.44.20240423.288/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    51052 2024-04-23 22:26:48.000000 pkscreener-0.44.20240423.288/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-04-23 22:26:48.000000 pkscreener-0.44.20240423.288/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    80501 2024-04-23 22:26:48.000000 pkscreener-0.44.20240423.288/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-04-23 22:26:48.000000 pkscreener-0.44.20240423.288/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-04-23 22:31:12.000000 pkscreener-0.44.20240423.288/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     4935 2024-04-23 22:26:48.000000 pkscreener-0.44.20240423.288/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-04-23 22:26:48.000000 pkscreener-0.44.20240423.288/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   122559 2024-04-23 22:26:48.000000 pkscreener-0.44.20240423.288/pkscreener/globals.py
--rw-rw-rw-   0        0        0      595 2024-04-23 22:26:48.000000 pkscreener-0.44.20240423.288/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    48027 2024-04-23 22:26:48.000000 pkscreener-0.44.20240423.288/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    23654 2024-04-23 22:26:48.000000 pkscreener-0.44.20240423.288/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-04-23 22:31:19.315962 pkscreener-0.44.20240423.288/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-04-23 22:31:19.000000 pkscreener-0.44.20240423.288/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1318 2024-04-23 22:31:19.000000 pkscreener-0.44.20240423.288/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 22:31:19.000000 pkscreener-0.44.20240423.288/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-04-23 22:31:19.000000 pkscreener-0.44.20240423.288/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-23 22:31:19.000000 pkscreener-0.44.20240423.288/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-04-23 22:31:19.000000 pkscreener-0.44.20240423.288/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-23 22:31:19.331580 pkscreener-0.44.20240423.288/setup.cfg
--rw-rw-rw-   0        0        0     4727 2024-04-23 22:26:48.000000 pkscreener-0.44.20240423.288/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 23:41:57.121715 pkscreener-0.44.20240423.289/
+-rw-rw-rw-   0        0        0     1086 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-04-23 23:41:57.121715 pkscreener-0.44.20240423.289/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 23:41:57.105994 pkscreener-0.44.20240423.289/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 23:41:57.121715 pkscreener-0.44.20240423.289/pkscreener/classes/
+-rw-rw-rw-   0        0        0    10156 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    25815 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0     9868 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     7038 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3237 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    29415 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    10999 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    20931 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    19689 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8120 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    17306 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   113351 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    51052 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    81010 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-04-23 23:41:46.000000 pkscreener-0.44.20240423.289/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     4935 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   122733 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      595 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    48027 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    23654 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-04-23 23:41:57.105994 pkscreener-0.44.20240423.289/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-04-23 23:41:57.000000 pkscreener-0.44.20240423.289/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1318 2024-04-23 23:41:57.000000 pkscreener-0.44.20240423.289/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 23:41:57.000000 pkscreener-0.44.20240423.289/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-04-23 23:41:57.000000 pkscreener-0.44.20240423.289/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-23 23:41:57.000000 pkscreener-0.44.20240423.289/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-04-23 23:41:57.000000 pkscreener-0.44.20240423.289/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-23 23:41:57.121715 pkscreener-0.44.20240423.289/setup.cfg
+-rw-rw-rw-   0        0        0     4727 2024-04-23 23:36:19.000000 pkscreener-0.44.20240423.289/setup.py
```

### Comparing `pkscreener-0.44.20240423.288/LICENSE` & `pkscreener-0.44.20240423.289/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.288/LICENSE-Others` & `pkscreener-0.44.20240423.289/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.288/PKG-INFO` & `pkscreener-0.44.20240423.289/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240423.288
+Version: 0.44.20240423.289
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240423.288.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240423.289.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240423.287/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240423.288/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240423.287/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240423.288/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240423.287/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240423.288/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240423.288/README.md` & `pkscreener-0.44.20240423.289/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240423.287/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240423.288/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240423.287/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240423.288/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240423.287/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240423.288/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240423.288/pkscreener/__init__.py` & `pkscreener-0.44.20240423.289/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.288/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240423.289/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.288/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240423.289/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.288/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240423.289/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.288/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240423.289/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.288/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240423.289/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.288/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240423.289/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.288/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240423.289/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.288/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240423.289/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.288/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240423.289/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.288/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240423.289/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.288/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240423.289/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.288/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240423.289/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.288/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240423.289/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.288/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240423.289/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.288/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240423.289/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.288/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240423.289/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.288/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240423.289/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.288/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240423.289/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.288/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240423.289/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.288/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240423.289/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.288/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240423.289/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.288/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240423.289/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.288/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240423.289/pkscreener/classes/Utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -808,23 +808,26 @@
             fn_args = (stocks, configManager.period, configManager.duration,exchangeSuffix)
             task = PKTask(f"DataDownload-{queueCounter}",long_running_fn=fetcher.fetchStockDataWithArgs,long_running_fn_args=fn_args)
             task.userData = stocks
             if len(stocks) > 0:
                 tasksList.append(task)
             queueCounter += 1
         
+        processedStocks = []
         if len(tasksList) > 0:
             PKScheduler.scheduleTasks(tasksList=tasksList, label=f"Downloading latest data [{configManager.period},{configManager.duration}] (Total={len(stockCodes)} records in {len(tasksList)} batches){'Be Patient!' if len(stockCodes)> 2000 else ''}",timeout=3*configManager.longTimeout*(4 if downloadOnly else 1),minAcceptableCompletionPercentage=(100 if downloadOnly else 80))
             for task in tasksList:
                 if task.result is not None:
                     for stock in task.userData:
                         taskResult = task.result.get(f"{stock}{exchangeSuffix}")
                         if taskResult is not None:
                             stockDict[stock] = taskResult.to_dict("split")
-        return stockDict
+                            processedStocks.append(stock)
+        leftOutStocks = list(set(stockCodes)-set(processedStocks))
+        return stockDict, leftOutStocks
 
     def loadStockData(
         stockDict,
         configManager,
         downloadOnly=False,
         defaultAnswer=None,
         retrial=False,
@@ -835,20 +838,24 @@
         forceRedownload=False
     ):
         isIntraday = isIntraday or configManager.isIntradayConfig()
         exists, cache_file = tools.afterMarketStockDataExists(
             isIntraday, forceLoad=forceLoad
         )
         initialLoadCount = len(stockDict)
+        leftOutStocks = None
         isTrading = PKDateUtilities.isTradingTime() and not PKDateUtilities.isTodayHoliday()[0]
         # stockCodes is not None mandates that we start our work based on the downloaded data from yesterday
         if (stockCodes is not None and len(stockCodes) > 0) and (isTrading or downloadOnly):
-            stockDict = tools.downloadLatestData(stockDict,configManager,stockCodes,exchangeSuffix=exchangeSuffix,downloadOnly=downloadOnly)
+            stockDict, leftOutStocks = tools.downloadLatestData(stockDict,configManager,stockCodes,exchangeSuffix=exchangeSuffix,downloadOnly=downloadOnly)
+            if len(leftOutStocks) > int(len(stockCodes)*0.05):
+                # More than 5 % of stocks are still remaining
+                stockDict, _ = tools.downloadLatestData(stockDict,configManager,leftOutStocks,exchangeSuffix=exchangeSuffix,downloadOnly=downloadOnly)
             # return stockDict
-        if downloadOnly:
+        if downloadOnly or isTrading:
             # We don't want to download from local stale pkl file or stale file at server
             return stockDict
         
         default_logger().info(
             f"Stock data cache file:{cache_file} exists ->{str(exists)}"
         )
         stockDataLoaded = False
```

### Comparing `pkscreener-0.44.20240423.288/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240423.289/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.288/pkscreener/classes/keys.py` & `pkscreener-0.44.20240423.289/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.288/pkscreener/courbd.ttf` & `pkscreener-0.44.20240423.289/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.288/pkscreener/globals.py` & `pkscreener-0.44.20240423.289/pkscreener/globals.py`

 * *Files 0% similar despite different names*

```diff
@@ -630,15 +630,15 @@
     global consumers,stockDictPrimary, loadedStockData, listStockCodes, stockDictSecondary
     options = startupoptions.replace("|","").split(" ")[0].replace(":i","")
     loadedStockData = False
     options, menuOption, indexOption, executeOption = getTopLevelMenuChoices(
         options, False, False, defaultAnswer='Y'
     )
     listStockCodes = prepareStocksForScreening(testing=False, downloadOnly=False, listStockCodes=None,indexOption=indexOption)
-    loadDatabaseOrFetch(downloadOnly=False, listStockCodes=listStockCodes, menuOption=menuOption,indexOption=indexOption)
+    stockDictPrimary,stockDictSecondary = loadDatabaseOrFetch(downloadOnly=False, listStockCodes=listStockCodes, menuOption=menuOption,indexOption=indexOption)
     PKScanRunner.refreshDatabase(consumers,stockDictPrimary,stockDictSecondary)
 
 # @tracelog
 def main(userArgs=None,optionalFinalOutcome_df=None):
     global listStockCodes, screenResults, selectedChoice, defaultAnswer, menuChoiceHierarchy, screenCounter, screenResultsCounter, stockDictPrimary, stockDictSecondary, userPassedArgs, loadedStockData, keyboardInterruptEvent, loadCount, maLength, newlyListedOnly, keyboardInterruptEventFired,strategyFilter, elapsed_time, start_time
     selectedChoice = {"0": "", "1": "", "2": "", "3": "", "4": ""}
     elapsed_time = 0
@@ -1130,15 +1130,15 @@
             # not downloadOnly
             # and not PKDateUtilities.isTradingTime()
             # and 
             configManager.cacheEnabled
             and not loadedStockData
             and not testing
         ):
-            loadDatabaseOrFetch(downloadOnly, listStockCodes, menuOption, indexOption)
+            stockDictPrimary,stockDictSecondary = loadDatabaseOrFetch(downloadOnly, listStockCodes, menuOption, indexOption)
             
         loadCount = len(stockDictPrimary) if stockDictPrimary is not None else 0
 
         if downloadOnly:
             OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.WARN
@@ -1368,30 +1368,31 @@
                     configManager,
                     downloadOnly=downloadOnly,
                     defaultAnswer=defaultAnswer,
                     forceLoad=(menuOption in ["X", "B", "G", "S"]),
                     stockCodes = listStockCodes,
                     exchangeSuffix = "" if (indexOption == 15 or (configManager.defaultIndex == 15 and indexOption == 0)) else ".NS"
             )
-    if not configManager.isIntradayConfig() and configManager.calculatersiintraday:
+    if menuOption not in ["C"] and not configManager.isIntradayConfig() and configManager.calculatersiintraday:
         candleDuration = (userPassedArgs.intraday if (userPassedArgs is not None and userPassedArgs.intraday is not None) else "1m")
         configManager.toggleConfig(candleDuration=candleDuration,clearCache=False)
         # We also need to load the intraday data to be able to calculate intraday RSI
-        Utility.tools.loadStockData(
+        stockDictSecondary = Utility.tools.loadStockData(
                         stockDictSecondary,
                         configManager,
                         downloadOnly=downloadOnly,
                         defaultAnswer=defaultAnswer,
                         forceLoad=(menuOption in ["X", "B", "G", "S"]),
                         stockCodes = listStockCodes,
                         isIntraday=True,
                         exchangeSuffix = "" if (indexOption == 15 or (configManager.defaultIndex == 15 and indexOption == 0)) else ".NS"
                 )
         resetConfigToDefault()
     loadedStockData = True
+    return stockDictPrimary, stockDictSecondary
 
 def getLatestTradeDateTime(stockDictPrimary):
     stocks = list(stockDictPrimary.keys())
     stock = stocks[0]
     try:
         lastTradeDate = PKDateUtilities.currentDateTime().strftime("%Y-%m-%d")
         lastTradeTime_ist = PKDateUtilities.currentDateTime().strftime("%H:%M:%S")
```

### Comparing `pkscreener-0.44.20240423.288/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240423.289/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.288/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240423.289/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.288/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240423.289/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.288/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240423.289/pkscreener.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240423.288
+Version: 0.44.20240423.289
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240423.288.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240423.289.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240423.287/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240423.288/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240423.287/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240423.288/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240423.287/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240423.288/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240423.288/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240423.289/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240423.288/setup.py` & `pkscreener-0.44.20240423.289/setup.py`

 * *Files identical despite different names*

