# Comparing `tmp/pkscreener-0.44.20240422.286.tar.gz` & `tmp/pkscreener-0.44.20240423.287.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240422.286.tar", last modified: Mon Apr 22 22:15:58 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240423.287.tar", last modified: Tue Apr 23 19:19:18 2024, max compression
```

## Comparing `pkscreener-0.44.20240422.286.tar` & `pkscreener-0.44.20240423.287.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 22:15:58.374098 pkscreener-0.44.20240422.286/
--rw-rw-rw-   0        0        0     1086 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-04-22 22:15:58.374098 pkscreener-0.44.20240422.286/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/README.md
-drwxrwxrwx   0        0        0        0 2024-04-22 22:15:58.359072 pkscreener-0.44.20240422.286/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 22:15:58.374098 pkscreener-0.44.20240422.286/pkscreener/classes/
--rw-rw-rw-   0        0        0    10156 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    26011 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0     9925 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0     7038 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3237 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    29415 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    10999 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    20931 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    18737 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8120 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    17306 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   112580 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    49099 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    79894 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-04-22 22:15:51.000000 pkscreener-0.44.20240422.286/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     4935 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   122052 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/globals.py
--rw-rw-rw-   0        0        0      595 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    48027 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    23583 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-04-22 22:15:58.359072 pkscreener-0.44.20240422.286/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-04-22 22:15:58.000000 pkscreener-0.44.20240422.286/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1318 2024-04-22 22:15:58.000000 pkscreener-0.44.20240422.286/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 22:15:58.000000 pkscreener-0.44.20240422.286/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-04-22 22:15:58.000000 pkscreener-0.44.20240422.286/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-22 22:15:58.000000 pkscreener-0.44.20240422.286/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-04-22 22:15:58.000000 pkscreener-0.44.20240422.286/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-22 22:15:58.374098 pkscreener-0.44.20240422.286/setup.cfg
--rw-rw-rw-   0        0        0     4727 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 19:19:18.571424 pkscreener-0.44.20240423.287/
+-rw-rw-rw-   0        0        0     1086 2024-04-23 19:16:10.000000 pkscreener-0.44.20240423.287/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-04-23 19:16:10.000000 pkscreener-0.44.20240423.287/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-04-23 19:19:18.571424 pkscreener-0.44.20240423.287/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-04-23 19:16:10.000000 pkscreener-0.44.20240423.287/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 19:19:18.555166 pkscreener-0.44.20240423.287/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-04-23 19:16:10.000000 pkscreener-0.44.20240423.287/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 19:19:18.571424 pkscreener-0.44.20240423.287/pkscreener/classes/
+-rw-rw-rw-   0        0        0    10156 2024-04-23 19:16:10.000000 pkscreener-0.44.20240423.287/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-04-23 19:16:10.000000 pkscreener-0.44.20240423.287/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-04-23 19:16:10.000000 pkscreener-0.44.20240423.287/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-04-23 19:16:10.000000 pkscreener-0.44.20240423.287/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    26011 2024-04-23 19:16:10.000000 pkscreener-0.44.20240423.287/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0     9896 2024-04-23 19:16:10.000000 pkscreener-0.44.20240423.287/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     7038 2024-04-23 19:16:10.000000 pkscreener-0.44.20240423.287/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3237 2024-04-23 19:16:10.000000 pkscreener-0.44.20240423.287/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    29415 2024-04-23 19:16:10.000000 pkscreener-0.44.20240423.287/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    10999 2024-04-23 19:16:10.000000 pkscreener-0.44.20240423.287/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    20931 2024-04-23 19:16:10.000000 pkscreener-0.44.20240423.287/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    19689 2024-04-23 19:16:10.000000 pkscreener-0.44.20240423.287/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-04-23 19:16:10.000000 pkscreener-0.44.20240423.287/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8120 2024-04-23 19:16:10.000000 pkscreener-0.44.20240423.287/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-04-23 19:16:10.000000 pkscreener-0.44.20240423.287/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-04-23 19:16:10.000000 pkscreener-0.44.20240423.287/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    17306 2024-04-23 19:16:10.000000 pkscreener-0.44.20240423.287/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-04-23 19:16:10.000000 pkscreener-0.44.20240423.287/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-04-23 19:16:10.000000 pkscreener-0.44.20240423.287/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   113351 2024-04-23 19:16:10.000000 pkscreener-0.44.20240423.287/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    51318 2024-04-23 19:16:10.000000 pkscreener-0.44.20240423.287/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-04-23 19:16:10.000000 pkscreener-0.44.20240423.287/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    79894 2024-04-23 19:16:10.000000 pkscreener-0.44.20240423.287/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-04-23 19:16:10.000000 pkscreener-0.44.20240423.287/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-04-23 19:19:09.000000 pkscreener-0.44.20240423.287/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     4935 2024-04-23 19:16:10.000000 pkscreener-0.44.20240423.287/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-04-23 19:16:10.000000 pkscreener-0.44.20240423.287/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   122559 2024-04-23 19:16:10.000000 pkscreener-0.44.20240423.287/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      595 2024-04-23 19:16:10.000000 pkscreener-0.44.20240423.287/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    48027 2024-04-23 19:16:10.000000 pkscreener-0.44.20240423.287/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    23583 2024-04-23 19:16:10.000000 pkscreener-0.44.20240423.287/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-04-23 19:19:18.555166 pkscreener-0.44.20240423.287/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-04-23 19:19:18.000000 pkscreener-0.44.20240423.287/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1318 2024-04-23 19:19:18.000000 pkscreener-0.44.20240423.287/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 19:19:18.000000 pkscreener-0.44.20240423.287/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-04-23 19:19:18.000000 pkscreener-0.44.20240423.287/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-23 19:19:18.000000 pkscreener-0.44.20240423.287/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-04-23 19:19:18.000000 pkscreener-0.44.20240423.287/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-23 19:19:18.571424 pkscreener-0.44.20240423.287/setup.cfg
+-rw-rw-rw-   0        0        0     4727 2024-04-23 19:16:10.000000 pkscreener-0.44.20240423.287/setup.py
```

### Comparing `pkscreener-0.44.20240422.286/LICENSE` & `pkscreener-0.44.20240423.287/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.286/LICENSE-Others` & `pkscreener-0.44.20240423.287/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.286/PKG-INFO` & `pkscreener-0.44.20240423.287/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240422.286
+Version: 0.44.20240423.287
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240422.286.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240423.287.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240422.285/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240422.286/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240422.285/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240422.286/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240422.285/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240422.286/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240422.286/README.md` & `pkscreener-0.44.20240423.287/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240422.285/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240422.286/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240422.285/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240422.286/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240422.285/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240422.286/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240422.286/pkscreener/__init__.py` & `pkscreener-0.44.20240423.287/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.286/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240423.287/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.286/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240423.287/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.286/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240423.287/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.286/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240423.287/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.286/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240423.287/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.286/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240423.287/pkscreener/classes/Fetcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,14 @@
                     + colorText.FAIL
                     + "=> Failed to fetch!"
                     + colorText.END,
                     end="\r",
                     flush=True,
                 )
                 raise StockDataEmptyException
-                return None
             OutputControls().printOutput(
                 colorText.BOLD + colorText.GREEN + "=> Done!" + colorText.END,
                 end="\r",
                 flush=True,
             )
         return data
```

### Comparing `pkscreener-0.44.20240422.286/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240423.287/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.286/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240423.287/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.286/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240423.287/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.286/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240423.287/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.286/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240423.287/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.286/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240423.287/pkscreener/classes/PKScanRunner.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 from PKDevTools.classes import Archiver
 from PKDevTools.classes.ColorText import colorText
 from PKDevTools.classes.PKDateUtilities import PKDateUtilities
 from PKDevTools.classes.log import default_logger
 from PKDevTools.classes.PKGitFolderDownloader import downloadFolder
 from PKDevTools.classes.PKMultiProcessorClient import PKMultiProcessorClient
+from PKDevTools.classes.multiprocessing_logging import LogQueueReader
 
 from pkscreener.classes.StockScreener import StockScreener
 from pkscreener.classes.CandlePatterns import CandlePatterns
 from pkscreener.classes.ConfigManager import parser, tools
 from PKDevTools.classes.OutputControls import OutputControls
 # from PKDevTools.classes.PKJoinableQueue import PKJoinableQueue
 
@@ -94,21 +95,22 @@
             ]
         )
         return screenResults, saveResults
 
     def initQueues(minimumCount=0):
         tasks_queue = multiprocessing.JoinableQueue()
         results_queue = multiprocessing.Queue()
+        logging_queue = multiprocessing.Queue()
 
         totalConsumers = min(minimumCount, multiprocessing.cpu_count())
         if totalConsumers == 1:
             totalConsumers = 2  # This is required for single core machine
         if PKScanRunner.configManager.cacheEnabled is True and multiprocessing.cpu_count() > 2:
             totalConsumers -= 1
-        return tasks_queue, results_queue, totalConsumers
+        return tasks_queue, results_queue, totalConsumers, logging_queue
 
     def populateQueues(items, tasks_queue, exit=False):
         # default_logger().debug(f"Unfinished items in task_queue: {tasks_queue.qsize()}")
         for item in items:
             tasks_queue.put(item)
         if exit:
             # Append exit signal for each process indicated by None
@@ -236,21 +238,29 @@
                     choices = f"{choices}_"
                 choices = f"{choices}{selectedChoice[choice]}"
         if choices.endswith("_"):
             choices = choices[:-1]
         choices = f"{choices}{'_i' if isIntraday else ''}"
         return choices
 
-    def refreshDatabase():
-        for worker in PKScanRunner.consumers:
+    def refreshDatabase(consumers,stockDictPrimary,stockDictSecondary):
+        for worker in consumers:
+            worker.objectDictionaryPrimary = stockDictPrimary
+            worker.objectDictionarySecondary = stockDictSecondary
             worker.refreshDatabase = True
             
-    def runScanWithParams(userPassedArgs,keyboardInterruptEvent,screenCounter,screenResultsCounter,stockDict,testing, backtestPeriod, menuOption, samplingDuration, items,screenResults, saveResults, backtest_df,scanningCb,tasks_queue, results_queue, consumers):
+    def runScanWithParams(userPassedArgs,keyboardInterruptEvent,screenCounter,screenResultsCounter,stockDictPrimary,stockDictSecondary,testing, backtestPeriod, menuOption, samplingDuration, items,screenResults, saveResults, backtest_df,scanningCb,tasks_queue, results_queue, consumers,logging_queue):
         if tasks_queue is None or results_queue is None or consumers is None:
-            tasks_queue, results_queue, consumers = PKScanRunner.prepareToRunScan(keyboardInterruptEvent,screenCounter, screenResultsCounter, stockDict, items)
+            tasks_queue, results_queue, consumers,logging_queue = PKScanRunner.prepareToRunScan(keyboardInterruptEvent,screenCounter, screenResultsCounter, stockDictPrimary,stockDictSecondary, items)
+            try:
+                if logging_queue is not None:
+                    log_queue_reader = LogQueueReader(logging_queue)
+                    log_queue_reader.start()
+            except:
+                pass
         PKScanRunner.tasks_queue = tasks_queue
         PKScanRunner.results_queue = results_queue
         PKScanRunner.consumers = consumers
         screenResults, saveResults, backtest_df = scanningCb(
                     menuOption,
                     items,
                     PKScanRunner.tasks_queue,
@@ -264,42 +274,48 @@
                     backtest_df,
                     testing=testing,
                 )
 
         OutputControls().printOutput(colorText.END)
         if userPassedArgs is not None and userPassedArgs.monitor is None:
             PKScanRunner.terminateAllWorkers(consumers, tasks_queue, testing)
-        return screenResults, saveResults,backtest_df,tasks_queue, results_queue, consumers
+        return screenResults, saveResults,backtest_df,tasks_queue, results_queue, consumers, logging_queue
 
-    def prepareToRunScan(keyboardInterruptEvent, screenCounter, screenResultsCounter, stockDict, items):
-        tasks_queue, results_queue, totalConsumers = PKScanRunner.initQueues(len(items))
+    def prepareToRunScan(keyboardInterruptEvent, screenCounter, screenResultsCounter, stockDictPrimary,stockDictSecondary, items):
+        tasks_queue, results_queue, totalConsumers, logging_queue = PKScanRunner.initQueues(len(items))
         scr = ScreeningStatistics.ScreeningStatistics(PKScanRunner.configManager, default_logger())
         exists, cache_file = Utility.tools.afterMarketStockDataExists(intraday=PKScanRunner.configManager.isIntradayConfig())
+        sec_cache_file = cache_file if "intraday_" in cache_file else f"intraday_{cache_file}"
         consumers = [
                     PKMultiProcessorClient(
                         StockScreener().screenStocks,
                         tasks_queue,
                         results_queue,
+                        logging_queue,
                         screenCounter,
                         screenResultsCounter,
-                        # stockDict,
-                        cache_file if exists else stockDict,
+                        stockDictPrimary,
+                        stockDictSecondary,
                         PKScanRunner.fetcher.proxyServer,
                         keyboardInterruptEvent,
                         default_logger(),
                         PKScanRunner.fetcher,
                         PKScanRunner.configManager,
                         PKScanRunner.candlePatterns,
                         scr,
+                        None,
+                        None
+                        #cache_file if exists else None,
+                        #sec_cache_file,
                     )
                     for _ in range(totalConsumers)
                 ]
         PKScanRunner.startWorkers(consumers)
-        return tasks_queue,results_queue,consumers
-    
+        return tasks_queue,results_queue,consumers,logging_queue
+
     def startWorkers(consumers):
         try:
             from pytest_cov.embed import cleanup_on_signal, cleanup_on_sigterm
         except ImportError:
             pass
         else:
             if sys.platform.startswith("win"):
```

### Comparing `pkscreener-0.44.20240422.286/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240423.287/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.286/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240423.287/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.286/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240423.287/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.286/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240423.287/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.286/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240423.287/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.286/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240423.287/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.286/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240423.287/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.286/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240423.287/pkscreener/classes/ScreeningStatistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,16 @@
 from PKDevTools.classes.SuppressOutput import SuppressOutput
 # from PKDevTools.classes.log import measure_time
 
 # Exception for only downloading stock data and not screening
 class DownloadDataOnly(Exception):
     pass
 
+class EligibilityConditionNotMet(Exception):
+    pass
 
 # Exception for stocks which are not newly listed when screening only for Newly Listed
 class NotNewlyListed(Exception):
     pass
 
 
 # Exception for stocks which are not stage two
@@ -726,14 +728,16 @@
         if df is None or len(df) == 0:
             return False
         if rsiKey not in df.columns:
             return False
         data = df.copy()
         data = data[::-1]
         data = data.tail(3)
+        if len(data) < 3:
+            return False
         dayMinus2RSI = data["RSI"].iloc[0]
         dayMinus1RSI = data["RSI"].iloc[1]
         dayRSI = data["RSI"].iloc[2]
         returnValue = (dayMinus2RSI <= 35 and dayMinus1RSI > dayMinus2RSI and dayRSI > dayMinus1RSI) or \
                 (dayMinus1RSI <= 35 and dayRSI > dayMinus1RSI)
         if rsiKey == "RSI":
             returnValue = self.findRisingRSI(df, rsiKey="RSIi") or returnValue
@@ -1342,46 +1346,51 @@
             result_df.sort_values(by="Time", inplace=True)
         return result_df[::-1]
 
     # Preprocess the acquired data
     def preprocessData(self, df, daysToLookback=None):
         assert isinstance(df, pd.DataFrame)
         data = df.copy()
-        data = data.replace(np.inf, np.nan).replace(-np.inf, np.nan).dropna(how="all")
-        # self.default_logger.info(f"Preprocessing data:\n{data.head(1)}\n")
-        if daysToLookback is None:
-            daysToLookback = self.configManager.daysToLookback
-        if self.configManager.useEMA:
-            sma = pktalib.EMA(data["Close"], timeperiod=50)
-            lma = pktalib.EMA(data["Close"], timeperiod=200)
-            ssma = pktalib.EMA(data["Close"], timeperiod=9)
-            data.insert(len(data.columns), "SMA", sma)
-            data.insert(len(data.columns), "LMA", lma)
-            data.insert(len(data.columns), "SSMA", ssma)
-        else:
-            sma = pktalib.SMA(data["Close"], timeperiod=50)
-            lma = pktalib.SMA(data["Close"], timeperiod=200)
-            ssma = pktalib.SMA(data["Close"], timeperiod=9)
-            data.insert(len(data.columns), "SMA", sma)
-            data.insert(len(data.columns), "LMA", lma)
-            data.insert(len(data.columns), "SSMA", ssma)
-        vol = pktalib.SMA(data["Volume"], timeperiod=20)
-        rsi = pktalib.RSI(data["Close"], timeperiod=14)
-        data.insert(len(data.columns), "VolMA", vol)
-        data.insert(len(data.columns), "RSI", rsi)
-        cci = pktalib.CCI(data["High"], data["Low"], data["Close"], timeperiod=14)
-        data.insert(len(data.columns), "CCI", cci)
         try:
-            fastk, fastd = pktalib.STOCHRSI(
-                data["Close"], timeperiod=14, fastk_period=5, fastd_period=3, fastd_matype=0
-            )
-            data.insert(len(data.columns), "FASTK", fastk)
-            data.insert(len(data.columns), "FASTD", fastd)
-        except:
-            pass
+            data = data.replace(np.inf, np.nan).replace(-np.inf, np.nan).dropna(how="all")
+            # self.default_logger.info(f"Preprocessing data:\n{data.head(1)}\n")
+            if daysToLookback is None:
+                daysToLookback = self.configManager.daysToLookback
+            if self.configManager.useEMA:
+                sma = pktalib.EMA(data["Close"], timeperiod=50)
+                lma = pktalib.EMA(data["Close"], timeperiod=200)
+                ssma = pktalib.EMA(data["Close"], timeperiod=9)
+                data.insert(len(data.columns), "SMA", sma)
+                data.insert(len(data.columns), "LMA", lma)
+                data.insert(len(data.columns), "SSMA", ssma)
+            else:
+                sma = pktalib.SMA(data["Close"], timeperiod=50)
+                lma = pktalib.SMA(data["Close"], timeperiod=200)
+                ssma = pktalib.SMA(data["Close"], timeperiod=9)
+                data.insert(len(data.columns), "SMA", sma)
+                data.insert(len(data.columns), "LMA", lma)
+                data.insert(len(data.columns), "SSMA", ssma)
+            vol = pktalib.SMA(data["Volume"], timeperiod=20)
+            rsi = pktalib.RSI(data["Close"], timeperiod=14)
+            data.insert(len(data.columns), "VolMA", vol)
+            data.insert(len(data.columns), "RSI", rsi)
+            cci = pktalib.CCI(data["High"], data["Low"], data["Close"], timeperiod=14)
+            data.insert(len(data.columns), "CCI", cci)
+            try:
+                fastk, fastd = pktalib.STOCHRSI(
+                    data["Close"], timeperiod=14, fastk_period=5, fastd_period=3, fastd_matype=0
+                )
+                data.insert(len(data.columns), "FASTK", fastk)
+                data.insert(len(data.columns), "FASTD", fastd)
+            except Exception as e:
+                self.default_logger.debug(e, exc_info=True)
+                pass
+        except Exception as e:
+                self.default_logger.debug(e, exc_info=True)
+                pass
         data = data[::-1]  # Reverse the dataframe
         # data = data.fillna(0)
         # data = data.replace([np.inf, -np.inf], 0)
         fullData = data
         trimmedData = data.head(daysToLookback)
         return (fullData, trimmedData)
 
@@ -1396,14 +1405,16 @@
         data = data[::-1]  # Reverse the dataframe so that its the oldest date first
         data["SMA20"] = pktalib.SMA(data["Close"], 20)
         data["SMA20V"] = pktalib.SMA(data["Volume"], 20)
         data = data[
             ::-1
         ]  # Reverse the dataframe so that it's the most recent date first
         recent = data.head(3)
+        if len(recent) < 3:
+            return False
         cond1 = recent["Close"].iloc[0] > recent["Close"].iloc[1]
         cond2 = cond1 and (recent["Close"].iloc[0] > recent["SMA20"].iloc[0])
         cond3 = cond2 and (recent["Close"].iloc[1] > recent["High"].iloc[2])
         cond4 = cond3 and (recent["Volume"].iloc[0] > recent["SMA20V"].iloc[0])
         cond5 = cond4 and (recent["Volume"].iloc[1] > recent["SMA20V"].iloc[0])
         return cond5
 
@@ -1465,14 +1476,16 @@
 
     # Find Conflucence
     def validateConfluence(self, stock, df, screenDict, saveDict, percentage=0.1,confFilter=3):
         if df is None or len(df) == 0:
             return False
         data = df.copy()
         recent = data.head(2)
+        if len(recent) < 2:
+            return False
         is50DMAUpTrend = (recent["SMA"].iloc[0] > recent["SMA"].iloc[1])
         is50DMADownTrend = (recent["SMA"].iloc[0] < recent["SMA"].iloc[1])
         isGoldenCrossOver = (recent["SMA"].iloc[0] >= recent["LMA"].iloc[0]) and \
                             (recent["SMA"].iloc[1] <= recent["LMA"].iloc[1])
         isDeadCrossOver = (recent["SMA"].iloc[0] <= recent["LMA"].iloc[0]) and \
                             (recent["SMA"].iloc[1] >= recent["LMA"].iloc[1])
         is50DMA = (recent["SMA"].iloc[0] <= recent["Close"].iloc[0])
@@ -1564,14 +1577,16 @@
         if df is None or len(df) == 0:
             return False
         data = df.copy()
         day0 = data
         day1 = data[1:]
         day2 = data[2:]
         day3 = data[3:]
+        if len(day1) < 1 or len(day2) < 1 or len(day3) < 1:
+            return False
         higherHighs = (
             (day0["High"].iloc[0] > day1["High"].iloc[0])
             and (day1["High"].iloc[0] > day2["High"].iloc[0])
             and (day2["High"].iloc[0] > day3["High"].iloc[0])
         )
         higherLows = (
             (day0["Low"].iloc[0] > day1["Low"].iloc[0])
@@ -1782,14 +1797,16 @@
         data = data.replace([np.inf, -np.inf], 0)
         if daysForLowestVolume is None:
             daysForLowestVolume = 30
         if len(data) < daysForLowestVolume:
             return False
         data = data.head(daysForLowestVolume)
         recent = data.head(1)
+        if len(recent) < 1:
+            return False
         if (recent["Volume"].iloc[0] <= data.describe()["Volume"]["min"]) and recent[
             "Volume"
         ][0] != np.nan:
             return True
         return False
 
     # Validate LTP within limits
@@ -1894,54 +1911,54 @@
             if len(data) < 3:
                 return False
             for row in data.iterrows():
                 # All 3 candles should be Green and NOT Circuits
                 yc = row[1]["Close"]
                 yo = row[1]["Open"]
                 if yc <= yo:
-                    self.default_logger.info(
-                        f'Stock:{saveDict["Stock"]}, is not a momentum-gainer because yesterday-close ({yc}) <= yesterday-open ({yo})'
-                    )
+                    # self.default_logger.info(
+                    #     f'Stock:{saveDict["Stock"]}, is not a momentum-gainer because yesterday-close ({yc}) <= yesterday-open ({yo})'
+                    # )
                     return False
             openDesc = data.sort_values(by=["Open"], ascending=False)
             closeDesc = data.sort_values(by=["Close"], ascending=False)
             volDesc = data.sort_values(by=["Volume"], ascending=False)
             try:
                 if (
                     data.equals(openDesc)
                     and data.equals(closeDesc)
                     and data.equals(volDesc)
                 ):
-                    self.default_logger.info(
-                        f'Stock:{saveDict["Stock"]}, open,close and volume equal from day before yesterday. A potential momentum-gainer!'
-                    )
+                    # self.default_logger.info(
+                    #     f'Stock:{saveDict["Stock"]}, open,close and volume equal from day before yesterday. A potential momentum-gainer!'
+                    # )
                     to = data["Open"].iloc[0]
                     yc = data["Close"].iloc[1]
                     yo = data["Open"].iloc[1]
                     dyc = data["Close"].iloc[2]
                     if (to >= yc) and (yo >= dyc):
-                        self.default_logger.info(
-                            f'Stock:{saveDict["Stock"]}, is a momentum-gainer because today-open ({to}) >= yesterday-close ({yc}) and yesterday-open({yo}) >= day-before-close({dyc})'
-                        )
+                        # self.default_logger.info(
+                        #     f'Stock:{saveDict["Stock"]}, is a momentum-gainer because today-open ({to}) >= yesterday-close ({yc}) and yesterday-open({yo}) >= day-before-close({dyc})'
+                        # )
                         saved = self.findCurrentSavedValue(screenDict, saveDict, "Pattern")
                         screenDict["Pattern"] = (
                             saved[0]
                             + colorText.BOLD
                             + colorText.GREEN
                             + "Momentum Gainer"
                             + colorText.END
                         )
                         saveDict["Pattern"] = saved[1] + "Momentum Gainer"
                         return True
-                    self.default_logger.info(
-                        f'Stock:{saveDict["Stock"]}, is not a momentum-gainer because either today-open ({to}) < yesterday-close ({yc}) or yesterday-open({yo}) < day-before-close({dyc})'
-                    )
+                    # self.default_logger.info(
+                    #     f'Stock:{saveDict["Stock"]}, is not a momentum-gainer because either today-open ({to}) < yesterday-close ({yc}) or yesterday-open({yo}) < day-before-close({dyc})'
+                    # )
             except IndexError as e: # pragma: no cover
                 self.default_logger.debug(e, exc_info=True)
-                # self.default_logger.debug(data)
+                self.default_logger.debug(data)
                 pass
             return False
         except Exception as e:  # pragma: no cover
             self.default_logger.debug(e, exc_info=True)
             return False
 
     #@measure_time
@@ -2098,14 +2115,16 @@
     # Find if stock is newly listed
     def validateNewlyListed(self, df, daysToLookback):
         if df is None or len(df) == 0:
             return False
         data = df.copy()
         daysToLookback = int(daysToLookback[:-1])
         recent = data.head(1)
+        if len(recent) < 1:
+            return False
         if len(data) < daysToLookback and (
             recent["Close"].iloc[0] != np.nan and recent["Close"].iloc[0] > 0
         ):
             return True
         return False
 
     # Validate if the stock prices are at least rising by 2% for the last 3 sessions
```

### Comparing `pkscreener-0.44.20240422.286/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240423.287/pkscreener/classes/StockScreener.py`

 * *Files 7% similar despite different names*

```diff
@@ -95,33 +95,33 @@
         start_time = time.time()
         try:
             with hostRef.processingCounter.get_lock():
                 hostRef.processingCounter.value += 1
 
             volumeRatio, period = self.determineBasicConfigs(stock, newlyListedOnly, volumeRatio, logLevel, hostRef, configManager, screener, userArgsLog)
             # hostRef.default_logger.info(
-            #     f"For stock:{stock}, stock exists in objectDictionary:{hostRef.objectDictionary.get(stock)}, cacheEnabled:{configManager.cacheEnabled}, isTradingTime:{self.isTradingTime}, downloadOnly:{downloadOnly}"
+            #     f"For stock:{stock}, stock exists in objectDictionary:{hostRef.objectDictionaryPrimary.get(stock)}, cacheEnabled:{configManager.cacheEnabled}, isTradingTime:{self.isTradingTime}, downloadOnly:{downloadOnly}"
             # )
-            data = self.getRelevantDataForStock(totalSymbols, shouldCache, stock, downloadOnly, printCounter, backtestDuration, hostRef,hostRef.objectDictionary, configManager, fetcher, period, testData,exchangeName)
+            data = self.getRelevantDataForStock(totalSymbols, shouldCache, stock, downloadOnly, printCounter, backtestDuration, hostRef,hostRef.objectDictionaryPrimary, configManager, fetcher, period, testData,exchangeName)
             if not configManager.isIntradayConfig() and configManager.calculatersiintraday:
                 # Daily data is already available in "data" above.
                 # We need the intraday data for 1-d RSI values when config is not for intraday
-                intraday_data = self.getRelevantDataForStock(totalSymbols, shouldCache, stock, downloadOnly, printCounter, backtestDuration, hostRef, hostRef.secondaryObjectDictionary, configManager, fetcher, period, testData,exchangeName)
+                intraday_data = self.getRelevantDataForStock(totalSymbols, shouldCache, stock, downloadOnly, printCounter, backtestDuration, hostRef, hostRef.objectDictionarySecondary, configManager, fetcher, period, testData,exchangeName)
                 # if intraday_data is not None:
                 #     if len(intraday_data) == 0:
                 #         return None
                 # else:
                 #     return None
             else:
                 intraday_data = data
             if data is not None:
                 if len(data) == 0 or len(data) < backtestDuration:
-                    return None
+                    raise StockDataEmptyException(f"Data length:{len(data)}")
             else:
-                return None
+                raise StockDataEmptyException(f"Data is None: {data}")
             # hostRef.default_logger.info(f"Will pre-process data:\n{data.tail(10)}")
             fullData, processedData, data = self.getCleanedDataForDuration(backtestDuration, portfolio, screeningDictionary, saveDictionary, configManager, screener, data)
             if backtestDuration == 0 and configManager.calculatersiintraday:
                 if (intraday_data is not None and not intraday_data.empty):
                     intraday_fullData, intraday_processedData = screener.preprocessData(
                         intraday_data, daysToLookback=configManager.effectiveDaysToLookback
                     )
@@ -132,17 +132,17 @@
                     intraday_processedData = intraday_processedData.head(len(processedData))
                     data = data.tail(len(intraday_data))
                     intraday_data = intraday_data.tail(len(data))
                     # Indexes won't match. Hence, we'd need to fallback on tolist
                     processedData.loc[:,"RSIi"] = intraday_processedData["RSI"].tolist()
                     fullData.loc[:,"RSIi"] = intraday_fullData["RSI"].tolist()
 
-            def returnLegibleData():
+            def returnLegibleData(exceptionMessage=None):
                 if backtestDuration == 0 or menuOption not in ["B"]:
-                    return None
+                    raise ScreeningStatistics.EligibilityConditionNotMet(exceptionMessage)
                 elif (backtestDuration > 0 and backtestDuration <= configManager.maxBacktestWindow):
                     screener.validateMovingAverages(
                         processedData, screeningDictionary, saveDictionary, maRange=1.25
                     )
                     screener.findTrend(
                         processedData,
                         screeningDictionary,
@@ -161,15 +161,15 @@
                             backtestDuration,
                         )
             if newlyListedOnly:
                 if not screener.validateNewlyListed(fullData, period):
                     raise ScreeningStatistics.NotNewlyListed
 
             if processedData.empty:
-                return returnLegibleData()
+                raise StockDataEmptyException("Empty processedData")
             
             with SuppressOutput(suppress_stderr=(logLevel==logging.NOTSET), suppress_stdout=(not (printCounter or testbuild))):
                 self.updateStock(stock, screeningDictionary, saveDictionary, executeOption, exchangeName)
                 
                 self.performBasicLTPChecks(executeOption, screeningDictionary, saveDictionary, fullData, configManager, screener, exchangeName)
                 hasMinVolumeRatio = self.performBasicVolumeChecks(executeOption, volumeRatio, screeningDictionary, saveDictionary, processedData, configManager, screener)
                 
@@ -196,15 +196,15 @@
                 isVSA = False
                 isCandlePattern = False
                 isLowestVolume = False
                 hasBbandsSqz = False
 
                 isValidityCheckMet = self.performValidityCheckForExecuteOptions(executeOption,screener,fullData,screeningDictionary,saveDictionary,processedData)
                 if not isValidityCheckMet:
-                    return returnLegibleData()
+                    return returnLegibleData("Validity Check not met!")
                 isShortTermBullish = (executeOption == 11 and isValidityCheckMet)
                 if newlyListedOnly:
                     isIpoBase = screener.validateIpoBase(
                         stock, fullData, screeningDictionary, saveDictionary
                     )
                 if executeOption in [1,2]:
                     isBreaking = screener.findBreakoutValue(
@@ -218,134 +218,134 @@
                         isPotentialBreaking = screener.findPotentialBreakout(
                             fullData,
                             screeningDictionary,
                             saveDictionary,
                             daysToLookback=configManager.daysToLookback,
                         )
                         if not (isBreaking or isPotentialBreaking) or not hasMinVolumeRatio:
-                            return returnLegibleData()
+                            return returnLegibleData(f"isBreaking:{isBreaking},isPotentialBreaking:{isPotentialBreaking},hasMinVolumeRatio:{hasMinVolumeRatio}")
                     elif executeOption == 2:
                         if not (isBreaking) or not hasMinVolumeRatio:
-                            return returnLegibleData()
+                            return returnLegibleData(f"isBreaking:{isBreaking},hasMinVolumeRatio:{hasMinVolumeRatio}")
                 elif executeOption == 3:
                     consolidationValue = screener.validateConsolidation(
                         processedData,
                         screeningDictionary,
                         saveDictionary,
                         percentage=configManager.consolidationPercentage,
                     )
                     if ((consolidationValue == 0 or consolidationValue > configManager.consolidationPercentage)):
-                        return returnLegibleData()
+                        return returnLegibleData(f"consolidationValue:{consolidationValue}")
                 elif executeOption == 4:
                     isLowestVolume = screener.validateLowestVolume(
                         processedData, daysForLowestVolume
                     )
                     if not isLowestVolume:
-                        return returnLegibleData()
+                        return returnLegibleData(f"isLowestVolume:{isLowestVolume}")
                 elif executeOption == 5:
                     isValidRsi = screener.validateRSI(
                         processedData, screeningDictionary, saveDictionary, minRSI, maxRSI
                     )
                     if not isValidRsi:
-                        return returnLegibleData()
+                        return returnLegibleData(f"isValidRsi:{isValidRsi}")
                 elif executeOption == 6:
                     if reversalOption == 10:
                         hasRSIMAReversal = screener.findRSICrossingMA(processedData,
                                                                       screeningDictionary,
                                                                       saveDictionary,
                                                                       lookFor=maLength) # 1 =Buy, 2 =Sell, 3 = Any
                         if not hasRSIMAReversal:
-                            return returnLegibleData()
+                            return returnLegibleData(f"hasRSIMAReversal:{hasRSIMAReversal}")
                     elif reversalOption == 9:
                         hasRisingRSIReversal = screener.findRisingRSI(processedData)
                         if not hasRisingRSIReversal:
-                            return returnLegibleData()
+                            return returnLegibleData(f"hasRisingRSIReversal:{hasRisingRSIReversal}")
                     elif reversalOption == 8:
                         hasPsarRSIReversal = screener.findPSARReversalWithRSI(
                             processedData,
                             screeningDictionary,
                             saveDictionary
                             # minRSI=maLength if maLength is not None else 40,
                         )
                         if not hasPsarRSIReversal:
-                            return returnLegibleData()
+                            return returnLegibleData(f"hasPsarRSIReversal:{hasPsarRSIReversal}")
                     elif reversalOption == 6:
                         isNR = screener.validateNarrowRange(
                             processedData,
                             screeningDictionary,
                             saveDictionary,
                             nr=maLength if maLength is not None else 4,
                         )
                         if not isNR:
-                            return returnLegibleData()
+                            return returnLegibleData(f"isNR:{isNR}")
                     elif reversalOption == 5:
                         isVSA = screener.validateVolumeSpreadAnalysis(
                             processedData, screeningDictionary, saveDictionary
                         )
                         if not isVSA:
-                            return returnLegibleData()
+                            return returnLegibleData(f"isVSA:{isVSA}")
                     elif reversalOption == 4 and maLength is not None:
                         isMaSupport = screener.findReversalMA(
                             fullData, screeningDictionary, saveDictionary, maLength
                         )
                         if not isMaSupport:
-                            return returnLegibleData()
+                            return returnLegibleData(f"isMaSupport:{isMaSupport}")
                     elif reversalOption == 7:
                         if sys.version_info >= (3, 11):
                             isLorentzian = screener.validateLorentzian(
                                 fullData,
                                 screeningDictionary,
                                 saveDictionary,
                                 lookFor=maLength, # 1 =Buy, 2 =Sell, 3 = Any
                             )
                             if not isLorentzian:
-                                return returnLegibleData()
+                                return returnLegibleData(f"isLorentzian:{isLorentzian}")
                 elif executeOption == 7:
                     if respChartPattern == 3:
                         isConfluence = screener.validateConfluence(
                             stock,
                             processedData,
                             screeningDictionary,
                             saveDictionary,
                             percentage=insideBarToLookback,
                             confFilter=(maLength if maLength > 0 else 3) # 1 = Conf up, 2 = Conf Down, 3 = all
                         )
                         if not isConfluence:
-                            return returnLegibleData()
+                            return returnLegibleData(f"isConfluence:{isConfluence}")
                     elif respChartPattern == 4:
                         isVCP = screener.validateVCP(
                             fullData, screeningDictionary, saveDictionary
                         )
                         if not isVCP:
-                            return returnLegibleData()
+                            return returnLegibleData(f"isVCP:{isVCP}")
                     elif respChartPattern == 5:
                         if Imports["scipy"]:
                             isBuyingTrendline = screener.findTrendlines(
                                 fullData, screeningDictionary, saveDictionary
                             )
                             if not isBuyingTrendline:
-                                return returnLegibleData()
+                                return returnLegibleData(f"isBuyingTrendline:{isBuyingTrendline}")
                     elif respChartPattern == 6:
                         hasBbandsSqz = screener.findBbandsSqueeze(fullData, screeningDictionary, saveDictionary, filter=(maLength if maLength > 0 else 4))
                         if not hasBbandsSqz:
-                            return returnLegibleData()
+                            return returnLegibleData(f"hasBbandsSqz:{hasBbandsSqz}")
                     elif respChartPattern == 7:
                         isCandlePattern = candlePatterns.findPattern(
                         processedData, screeningDictionary, saveDictionary)
                         if not isCandlePattern:
-                            return returnLegibleData()
+                            return returnLegibleData(f"isCandlePattern:{isCandlePattern}")
                         
                 elif executeOption == 10:
                     isPriceRisingByAtLeast2Percent = (
                         screener.validatePriceRisingByAtLeast2Percent(
                             processedData, screeningDictionary, saveDictionary
                         )
                     )
                     if not isPriceRisingByAtLeast2Percent:
-                        return returnLegibleData()
+                        return returnLegibleData(f"isPriceRisingByAtLeast2Percent:{isPriceRisingByAtLeast2Percent}")
                 # Must-run, but only at the end
                 try:
                     if executeOption != 7 or (executeOption == 7 and respChartPattern != 7):
                     # Only 'doji' and 'inside' is internally implemented by pandas_ta.
                     # Otherwise, for the rest of the candle patterns, they also need
                     # TA-Lib. So if TA-Lib is not available, it will throw exception
                     # We can live with no-patterns if user has not installed ta-lib
@@ -375,63 +375,63 @@
                                 saveDictionary,
                                 testbuild,
                                 stock,
                                 onlyMF=(executeOption == 21 and reversalOption in [5,6]),
                                 hostData=data,
                                 exchangeName=exchangeName
                             )
-                            hostRef.objectDictionary[stock] = data.to_dict("split")
+                            hostRef.objectDictionaryPrimary[stock] = data.to_dict("split")
                 except np.RankWarning as e: # pragma: no cover 
                     hostRef.default_logger.debug(e, exc_info=True)
                     screeningDictionary["Trend"] = "Unknown"
                     saveDictionary["Trend"] = "Unknown"
                 # CCI also uses "Trend" value from findTrend above.
                 # So it must only be called after findTrend
                 if executeOption == 8:
                     isValidCci = screener.validateCCI(
                         processedData, screeningDictionary, saveDictionary, minRSI, maxRSI
                     )
                     if not isValidCci:
-                        return returnLegibleData()
+                        return returnLegibleData(f"isValidCci:{isValidCci}")
 
                 if not (isConfluence or isShortTermBullish or isMaSupport):
                     isMaReversal = screener.validateMovingAverages(
                         processedData, screeningDictionary, saveDictionary, maRange=1.25
                     )
                 if executeOption == 6:
                     if reversalOption == 1 and not (str(saveDictionary["Pattern"]).split(",")[0]
                                                                     in CandlePatterns.reversalPatternsBullish
                                                                     or isMaReversal > 0):
-                        return returnLegibleData()
+                        return returnLegibleData(f"reversalOption:{reversalOption},isMaReversal:{isMaReversal},{CandlePatterns.reversalPatternsBullish}")
                     elif reversalOption == 2 and not (str(saveDictionary["Pattern"]).split(",")[0]
                                                                     in CandlePatterns.reversalPatternsBearish
                                                                     or isMaReversal < 0):
-                        return returnLegibleData()
+                        return returnLegibleData(f"reversalOption:{reversalOption},isMaReversal:{isMaReversal},{CandlePatterns.reversalPatternsBearish}")
                 # validateInsideBar needs "Trend" to be already defined
                 # ValidateInsideBar also needs "MA-Signal" to be setup
                 if executeOption == 7 and respChartPattern < 3:
                     isInsideBar = screener.validateInsideBar(
                                 processedData,
                                 screeningDictionary,
                                 saveDictionary,
                                 chartPattern=respChartPattern,
                                 daysToLookback=insideBarToLookback,
                             )
                     if isInsideBar ==0:
-                        return returnLegibleData()
+                        return returnLegibleData(f"isInsideBar:{isInsideBar}")
 
                 if not (isLorentzian or (isInsideBar !=0) or isBuyingTrendline or isIpoBase or isNR or isVCP or isVSA):
                     isMomentum = screener.validateMomentum(
                         processedData, screeningDictionary, saveDictionary
                     )
                     if executeOption == 6 and reversalOption ==3 and not isMomentum:
-                        return returnLegibleData()
+                        return returnLegibleData(f"executeOption:{executeOption},reversalOption:{reversalOption},isMomentum:{isMomentum}")
 
                 with hostRef.processingResultsCounter.get_lock():
-                    hostRef.default_logger.debug(f"ExecuteOption:{executeOption}:{reversalOption}:{respChartPattern}:{maLength}. Elapsed: {time.time() - start_time}")
+                    # hostRef.default_logger.debug(f"ExecuteOption:{executeOption}:{reversalOption}:{respChartPattern}:{maLength}. Elapsed: {time.time() - start_time}")
                     if (
                         (executeOption == 0)
                         or ((
                             (
                                 (executeOption == 1 and (isBreaking or isPotentialBreaking))
                                 or (executeOption == 2 and isBreaking)
                             )
@@ -536,71 +536,76 @@
                                 saveDictionary,
                                 testbuild,
                                 stock,
                                 onlyMF=(executeOption == 21 and reversalOption in [5,6]),
                                 hostData=data,
                                 exchangeName=exchangeName
                             )
-                            hostRef.objectDictionary[stock] = data.to_dict("split")
+                            hostRef.objectDictionaryPrimary[stock] = data.to_dict("split")
 
                         hostRef.processingResultsCounter.value += 1
                         return (
                             screeningDictionary,
                             saveDictionary,
                             data,
                             stock,
                             backtestDuration,
                         )
 
         except KeyboardInterrupt: # pragma: no cover
             # Capturing Ctr+C Here isn't a great idea
             pass
         except StockDataEmptyException as e: # pragma: no cover
-            hostRef.default_logger.debug(e, exc_info=True)
+            if not data.isnull().values.all(axis=0)[0]:
+                hostRef.default_logger.debug(f"StockDataEmptyException:{stock}: {e}", exc_info=True)
+            pass
+        except ScreeningStatistics.EligibilityConditionNotMet as e:
+            # hostRef.default_logger.debug(f"EligibilityConditionNotMet:{stock}: {e}", exc_info=True)
             pass
         except ScreeningStatistics.NotNewlyListed as e: # pragma: no cover
-            hostRef.default_logger.debug(e, exc_info=True)
+            # hostRef.default_logger.debug(f"NotNewlyListed:{stock}: {e}", exc_info=True)
             pass
         except ScreeningStatistics.NotAStageTwoStock as e: # pragma: no cover
-            # hostRef.default_logger.debug(e, exc_info=True)
+            # hostRef.default_logger.debug(f"NotAStageTwoStock:{stock}: {e}", exc_info=True)
             pass
         except ScreeningStatistics.NotEnoughVolumeAsPerConfig as e: # pragma: no cover 
+            # hostRef.default_logger.debug(f"NotEnoughVolumeAsPerConfig:{stock}: {e}", exc_info=True)
             pass
         except ScreeningStatistics.DownloadDataOnly as e: # pragma: no cover
-            # hostRef.default_logger.debug(e, exc_info=True)
+            # hostRef.default_logger.debug(f"DownloadDataOnly:{stock}: {e}", exc_info=True)
             try:
-                data = hostRef.objectDictionary.get(stock)
+                data = hostRef.objectDictionaryPrimary.get(stock)
                 if data is not None:
                     data = pd.DataFrame(data["data"], columns=data["columns"], index=data["index"])
                     screener.getMutualFundStatus(stock, hostData=data, force=True, exchangeName=exchangeName)
-                    hostRef.objectDictionary[stock] = data.to_dict("split")
+                    hostRef.objectDictionaryPrimary[stock] = data.to_dict("split")
             except Exception as ex:
                 hostRef.default_logger.debug(f"MFIStatus: {stock}:\n{ex}", exc_info=True)
                 pass
             try:
                 screener.getFairValue(stock,hostData=data, force=True,exchangeName=exchangeName)
-                hostRef.objectDictionary[stock] = data.to_dict("split")
+                hostRef.objectDictionaryPrimary[stock] = data.to_dict("split")
             except Exception as ex:
                 hostRef.default_logger.debug(f"FairValue: {stock}:\n{ex}", exc_info=True)
                 pass
             pass
         except ScreeningStatistics.LTPNotInConfiguredRange as e: # pragma: no cover
-            # hostRef.default_logger.debug(e, exc_info=True)
+            # hostRef.default_logger.debug(f"LTPNotInConfiguredRange:{stock}: {e}", exc_info=True)
             pass
         except KeyError as e: # pragma: no cover
-            print(e)
-            hostRef.default_logger.debug(e, exc_info=True)
+            hostRef.default_logger.debug(f"KeyError:{stock}: {e}", exc_info=True)
             pass
         except OSError as e: # pragma: no cover
+            hostRef.default_logger.debug(f"OSError:{stock}: {e}", exc_info=True)
             pass
         except Exception as e:  # pragma: no cover
-            hostRef.default_logger.debug(e, exc_info=True)
+            hostRef.default_logger.debug(f"Exception:{stock}: {e}", exc_info=True)
             if testbuild or printCounter:
-                import traceback
-                traceback.print_exc()
+                # import traceback
+                # traceback.print_exc()
                 OutputControls().printOutput(e)
                 OutputControls().printOutput(
                     colorText.FAIL
                     + (
                         "\n[+] Exception Occured while Screening %s! Skipping this stock.."
                         % stock
                     )
@@ -656,15 +661,15 @@
                     processedData,
                     screeningDictionary,
                     saveDictionary,
                     volumeRatio=volumeRatio,
                     minVolume=minVolume,
                 )
         if (not hasMinVolQty and executeOption > 0) or (executeOption == 9 and not hasMinVolumeRatio):
-            raise ScreeningStatistics.NotEnoughVolumeAsPerConfig
+            raise ScreeningStatistics.NotEnoughVolumeAsPerConfig(f"hasMinVolQty:{hasMinVolQty},executeOption:{executeOption},hasMinVolumeRatio:{hasMinVolumeRatio}")
         return hasMinVolumeRatio
 
     def performBasicLTPChecks(self, executeOption, screeningDictionary, saveDictionary, fullData, configManager, screener,exchangeName):
         isLtpValid, verifyStageTwo = screener.validateLTP(
                     fullData,
                     screeningDictionary,
                     saveDictionary,
@@ -689,14 +694,16 @@
     def getCleanedDataForDuration(self, backtestDuration, portfolio, screeningDictionary, saveDictionary, configManager, screener, data):
         fullData = None
         processedData = None
         if backtestDuration == 0:
             fullData, processedData = screener.preprocessData(
                     data, daysToLookback=configManager.effectiveDaysToLookback
                 )
+            if processedData.empty:
+                raise StockDataEmptyException(f"Empty processedData with data length ({len(data)})")
             if portfolio:
                 data = data[::-1]
                 screener.validateLTPForPortfolioCalc(
                         data, screeningDictionary, saveDictionary,requestedPeriod=backtestDuration
                     )
                 data = data[::-1]
         else:
@@ -855,24 +862,24 @@
     
     def setupLoggers(self, hostRef, screener, logLevel, stock):
         # Set the loglevels for both the caller and screener
         # Also add handlers that are specific to this sub-process which
         # will continue with the screening. Each sub-process would have
         # its own logger but going into the same file/console > to that
         # of the parent logger.
-        if hostRef.default_logger.level > 0:
-            return
-        else:
-            hostRef.default_logger.info(f"Beginning the stock screening for stock:{stock}")
-        hostRef.default_logger.level = logLevel
-        screener.default_logger.level = logLevel
-        log_file_path = os.path.join(Archiver.get_user_outputs_dir(), "pkscreener-logs.txt")
-        hostRef.default_logger.addHandlers(log_file_path=log_file_path, levelname=logLevel)
-        screener.default_logger.addHandlers(log_file_path=log_file_path, levelname=logLevel)
-        hostRef.default_logger.info(f"Beginning the stock screening for stock:{stock}")
+        # if hostRef.default_logger.level > 0:
+        #     return
+        # else:
+        # hostRef.default_logger.info(f"Beginning the stock screening for stock:{stock}")
+        # hostRef.default_logger.level = logLevel
+        screener.default_logger = hostRef.default_logger
+        # log_file_path = os.path.join(Archiver.get_user_outputs_dir(), "pkscreener-logs.txt")
+        # hostRef.default_logger.addHandlers(log_file_path=log_file_path, levelname=logLevel)
+        # screener.default_logger.addHandlers(log_file_path=log_file_path, levelname=logLevel)
+        # hostRef.default_logger.info(f"Beginning the stock screening for stock:{stock}")
 
     def initResultDictionaries(self):
         periods = self.configManager.periodsRange
         columns = [
             "Stock",
             "LTP",
             "%Chng",
```

### Comparing `pkscreener-0.44.20240422.286/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240423.287/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.286/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240423.287/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.286/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240423.287/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.286/pkscreener/classes/keys.py` & `pkscreener-0.44.20240423.287/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.286/pkscreener/courbd.ttf` & `pkscreener-0.44.20240423.287/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.286/pkscreener/globals.py` & `pkscreener-0.44.20240423.287/pkscreener/globals.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,42 +116,44 @@
 newlyListedOnly = False
 screenCounter = None
 screener = ScreeningStatistics.ScreeningStatistics(configManager, default_logger())
 screenResults = None
 backtest_df = None
 screenResultsCounter = None
 selectedChoice = {"0": "", "1": "", "2": "", "3": "", "4": ""}
-stockDict = None
+stockDictPrimary = None
+stockDictSecondary = None
 userPassedArgs = None
 elapsed_time = 0
 start_time = 0
 test_messages_queue = []
 strategyFilter=[]
 listStockCodes = None
 tasks_queue = None
 results_queue = None
 consumers = None
+logging_queue = None
 
 def finishScreening(
     downloadOnly,
     testing,
-    stockDict,
+    stockDictPrimary,
     configManager,
     loadCount,
     testBuild,
     screenResults,
     saveResults,
     user=None,
 ):
     if "RUNNER" in os.environ.keys():
         # There's no need to prompt the user to save xls report or to save data locally.
         # This scan must have been triggered by github workflow by a user or scheduled job
         return
     global defaultAnswer, menuChoiceHierarchy, userPassedArgs, selectedChoice
-    saveDownloadedData(downloadOnly, testing, stockDict, configManager, loadCount)
+    saveDownloadedData(downloadOnly, testing, stockDictPrimary, configManager, loadCount)
     if not testBuild and not downloadOnly and not testing:
         saveNotifyResultsFile(
             screenResults, saveResults, defaultAnswer, menuChoiceHierarchy, user=user
         )
 
 
 def getDownloadChoices(defaultAnswer=None):
@@ -621,27 +623,27 @@
     return screenResults, saveResults
 
 def isInterrupted():
     global keyboardInterruptEventFired
     return keyboardInterruptEventFired
 
 def refreshStockData(startupoptions=None):
-    global stockDict, loadedStockData, listStockCodes
+    global consumers,stockDictPrimary, loadedStockData, listStockCodes, stockDictSecondary
     options = startupoptions.replace("|","").split(" ")[0].replace(":i","")
     loadedStockData = False
     options, menuOption, indexOption, executeOption = getTopLevelMenuChoices(
         options, False, False, defaultAnswer='Y'
     )
     listStockCodes = prepareStocksForScreening(testing=False, downloadOnly=False, listStockCodes=None,indexOption=indexOption)
     loadDatabaseOrFetch(downloadOnly=False, listStockCodes=listStockCodes, menuOption=menuOption,indexOption=indexOption)
-    PKScanRunner.refreshDatabase()
+    PKScanRunner.refreshDatabase(consumers,stockDictPrimary,stockDictSecondary)
 
 # @tracelog
 def main(userArgs=None,optionalFinalOutcome_df=None):
-    global listStockCodes, screenResults, selectedChoice, defaultAnswer, menuChoiceHierarchy, screenCounter, screenResultsCounter, stockDict, userPassedArgs, loadedStockData, keyboardInterruptEvent, loadCount, maLength, newlyListedOnly, keyboardInterruptEventFired,strategyFilter, elapsed_time, start_time
+    global listStockCodes, screenResults, selectedChoice, defaultAnswer, menuChoiceHierarchy, screenCounter, screenResultsCounter, stockDictPrimary, stockDictSecondary, userPassedArgs, loadedStockData, keyboardInterruptEvent, loadCount, maLength, newlyListedOnly, keyboardInterruptEventFired,strategyFilter, elapsed_time, start_time
     selectedChoice = {"0": "", "1": "", "2": "", "3": "", "4": ""}
     elapsed_time = 0
     start_time = 0
     testing = False if userArgs is None else (userArgs.testbuild and userArgs.prodbuild)
     testBuild = False if userArgs is None else (userArgs.testbuild and not testing)
     downloadOnly = False if userArgs is None else userArgs.download
     startupoptions = None if userArgs is None else userArgs.options
@@ -653,16 +655,17 @@
     if keyboardInterruptEventFired:
         return None, None
     screenCounter = multiprocessing.Value("i", 1)
     screenResultsCounter = multiprocessing.Value("i", 0)
     if keyboardInterruptEvent is None and not keyboardInterruptEventFired:
         keyboardInterruptEvent = multiprocessing.Manager().Event()
     keyboardInterruptEventFired = False
-    if stockDict is None:
-        stockDict = multiprocessing.Manager().dict()
+    if stockDictPrimary is None:
+        stockDictPrimary = multiprocessing.Manager().dict()
+        stockDictSecondary = multiprocessing.Manager().dict()
         loadCount = 0
     endOfdayCandles = None
     minRSI = 0
     maxRSI = 100
     insideBarToLookback = 7
     respChartPattern = None
     daysForLowestVolume = 30
@@ -1098,19 +1101,19 @@
                     + colorText.END
                 )
                 sys.exit(0)
             elif indexOption == "E":
                 return handleMonitorFiveEMA()
             else:
                 if str(menuOption).upper() == "C":
-                    stockDict,endOfdayCandles = PKMarketOpenCloseAnalyser.getStockDataForSimulation()
-                    if stockDict is None or endOfdayCandles is None:
+                    stockDictPrimary,endOfdayCandles = PKMarketOpenCloseAnalyser.getStockDataForSimulation()
+                    if stockDictPrimary is None or endOfdayCandles is None:
                         OutputControls().printOutput(f"Cannot proceed! Stock data is unavailable. Please check the error logs/messages !")
                         return None, None
-                    listStockCodes = sorted(list(filter(None,list(set(stockDict.keys())))))
+                    listStockCodes = sorted(list(filter(None,list(set(stockDictPrimary.keys())))))
                 listStockCodes = prepareStocksForScreening(testing, downloadOnly, listStockCodes, indexOption)
         except urllib.error.URLError as e:
             default_logger().debug(e, exc_info=True)
             OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.FAIL
                 + "\n\n[+] Oops! It looks like you don't have an Internet connectivity at the moment!"
@@ -1129,15 +1132,15 @@
             # and 
             configManager.cacheEnabled
             and not loadedStockData
             and not testing
         ):
             loadDatabaseOrFetch(downloadOnly, listStockCodes, menuOption, indexOption)
             
-        loadCount = len(stockDict) if stockDict is not None else 0
+        loadCount = len(stockDictPrimary) if stockDictPrimary is not None else 0
 
         if downloadOnly:
             OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.WARN
                 + "[+] Starting download.. Press Ctrl+C to stop!"
             )
@@ -1189,19 +1192,19 @@
                     )
                 fillerPlaceHolder = fillerPlaceHolder + 1
                 actualHistoricalDuration = samplingDuration - fillerPlaceHolder
                 if actualHistoricalDuration >= 0:
                     progressbar()
         sys.stdout.write(f"\x1b[1A") # Replace the download progress bar and start writing on the same line
         if not keyboardInterruptEventFired:
-            global tasks_queue, results_queue, consumers
-            screenResults, saveResults, backtest_df, tasks_queue, results_queue, consumers = PKScanRunner.runScanWithParams(userPassedArgs,keyboardInterruptEvent,screenCounter,screenResultsCounter,stockDict,testing, backtestPeriod, menuOption, samplingDuration, items,screenResults, saveResults, backtest_df,scanningCb=runScanners,tasks_queue=tasks_queue, results_queue=results_queue, consumers=consumers)
+            global tasks_queue, results_queue, consumers, logging_queue
+            screenResults, saveResults, backtest_df, tasks_queue, results_queue, consumers,logging_queue = PKScanRunner.runScanWithParams(userPassedArgs,keyboardInterruptEvent,screenCounter,screenResultsCounter,stockDictPrimary,stockDictSecondary,testing, backtestPeriod, menuOption, samplingDuration, items,screenResults, saveResults, backtest_df,scanningCb=runScanners,tasks_queue=tasks_queue, results_queue=results_queue, consumers=consumers,logging_queue=logging_queue)
             if menuOption in ["C"]:
                 runOptionName = PKScanRunner.getFormattedChoices(userPassedArgs,selectedChoice)
-                PKMarketOpenCloseAnalyser.runOpenCloseAnalysis(stockDict,endOfdayCandles,screenResults, saveResults,runOptionName=runOptionName)
+                PKMarketOpenCloseAnalyser.runOpenCloseAnalysis(stockDictPrimary,endOfdayCandles,screenResults, saveResults,runOptionName=runOptionName)
             if downloadOnly and menuOption in ["X"]:
                 screener.getFreshMFIStatus(stock="LatestCheckedOnDate")
                 screener.getFairValue(stock="LatestCheckedOnDate", force=True)
             if not downloadOnly and menuOption in ["X", "G", "C"]:
                 if menuOption == "G":
                     userPassedArgs.backtestdaysago = backtestPeriod
                 if screenResults is not None and len(screenResults) > 0:
@@ -1298,15 +1301,15 @@
                         testing,
                         user=user,
                     )
         if menuOption in ["X","C"] and userPassedArgs.monitor is None:
             finishScreening(
                 downloadOnly,
                 testing,
-                stockDict,
+                stockDictPrimary,
                 configManager,
                 loadCount,
                 testBuild,
                 screenResults,
                 saveResults,
                 user,
             )
@@ -1335,15 +1338,15 @@
             if "GSHEET_SERVICE_ACCOUNT_DEV" in os.environ.keys() and (userPassedArgs.backtestdaysago is None):# or userPassedArgs.log:
                 begin = time.time()
                 creds = os.environ.get("GSHEET_SERVICE_ACCOUNT_DEV")
                 OutputControls().printOutput(f"{colorText.GREEN}[+] Saving data to Google Spreadsheets now...{colorText.END}")
                 gClient = PKSpreadsheets(credentialDictStr=creds)
                 runOption = PKScanRunner.getFormattedChoices(userPassedArgs,selectedChoice)
                 df = saveResults.copy()
-                df["LastTradeDate"], df["LastTradeTime"] = getLatestTradeDateTime(stockDict)
+                df["LastTradeDate"], df["LastTradeTime"] = getLatestTradeDateTime(stockDictPrimary)
                 gClient.df_to_sheet(df=df,sheetName=runOption)
                 OutputControls().printOutput(f"{colorText.GREEN} => Done in {round(time.time()-begin,2)}s{colorText.END}")
     except:
         pass
     if userPassedArgs.runintradayanalysis:
         analysis_df = screenResults.copy()
         analysis_df.reset_index(inplace=True)
@@ -1354,51 +1357,51 @@
         else:
             optionalFinalOutcome_df = pd.concat([optionalFinalOutcome_df, analysis_df], axis=0)
         return optionalFinalOutcome_df, saveResults
     elif userPassedArgs.monitor is not None:
         return screenResults, saveResults
 
 def loadDatabaseOrFetch(downloadOnly, listStockCodes, menuOption, indexOption):
-    global stockDict, configManager, defaultAnswer, userPassedArgs, loadedStockData
+    global stockDictPrimary,stockDictSecondary, configManager, defaultAnswer, userPassedArgs, loadedStockData
     if menuOption not in ["C"]:
-        stockDict = Utility.tools.loadStockData(
-                    stockDict,
+        stockDictPrimary = Utility.tools.loadStockData(
+                    stockDictPrimary,
                     configManager,
                     downloadOnly=downloadOnly,
                     defaultAnswer=defaultAnswer,
                     forceLoad=(menuOption in ["X", "B", "G", "S"]),
                     stockCodes = listStockCodes,
                     exchangeSuffix = "" if (indexOption == 15 or (configManager.defaultIndex == 15 and indexOption == 0)) else ".NS"
             )
     if not configManager.isIntradayConfig() and configManager.calculatersiintraday:
         candleDuration = (userPassedArgs.intraday if (userPassedArgs is not None and userPassedArgs.intraday is not None) else "1m")
         configManager.toggleConfig(candleDuration=candleDuration,clearCache=False)
         # We also need to load the intraday data to be able to calculate intraday RSI
         Utility.tools.loadStockData(
-                        {},
+                        stockDictSecondary,
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
 
-def getLatestTradeDateTime(stockDict):
-    stocks = list(stockDict.keys())
+def getLatestTradeDateTime(stockDictPrimary):
+    stocks = list(stockDictPrimary.keys())
     stock = stocks[0]
     try:
         lastTradeDate = PKDateUtilities.currentDateTime().strftime("%Y-%m-%d")
         lastTradeTime_ist = PKDateUtilities.currentDateTime().strftime("%H:%M:%S")
-        df = pd.DataFrame(data=stockDict[stock]["data"],
-                        columns=stockDict[stock]["columns"],
-                        index=stockDict[stock]["index"])
+        df = pd.DataFrame(data=stockDictPrimary[stock]["data"],
+                        columns=stockDictPrimary[stock]["columns"],
+                        index=stockDictPrimary[stock]["index"])
         ts = df.index[-1]
         lastTraded = pd.to_datetime(ts, unit='s', utc=True) #.tz_convert("Asia/Kolkata")
         lastTradeDate = lastTraded.strftime("%Y-%m-%d")
         lastTradeTime = lastTraded.strftime("%H:%M:%S")
         if lastTradeTime == "00:00:00":
             lastTradeTime = lastTradeTime_ist
     except:
@@ -2272,32 +2275,32 @@
         backtest_df,
         sellSignal,
     )
     elapsed_time = time.time() - start_time
     return backtest_df
 
 
-def saveDownloadedData(downloadOnly, testing, stockDict, configManager, loadCount):
+def saveDownloadedData(downloadOnly, testing, stockDictPrimary, configManager, loadCount):
     global userPassedArgs, keyboardInterruptEventFired
     argsIntraday = userPassedArgs is not None and userPassedArgs.intraday is not None
     intradayConfig = configManager.isIntradayConfig()
     intraday = intradayConfig or argsIntraday
     if not keyboardInterruptEventFired and (downloadOnly or (
         configManager.cacheEnabled and not PKDateUtilities.isTradingTime() and not testing
     )):
         OutputControls().printOutput(
             colorText.BOLD
             + colorText.GREEN
             + "[+] Caching Stock Data for future use, Please Wait... "
             + colorText.END,
             end="",
         )
-        Utility.tools.saveStockData(stockDict, configManager, loadCount, intraday)
+        Utility.tools.saveStockData(stockDictPrimary, configManager, loadCount, intraday)
         if downloadOnly:
-            Utility.tools.saveStockData(stockDict, configManager, loadCount, intraday, downloadOnly=downloadOnly)
+            Utility.tools.saveStockData(stockDictPrimary, configManager, loadCount, intraday, downloadOnly=downloadOnly)
     else:
         OutputControls().printOutput(colorText.BOLD + colorText.GREEN + "[+] Skipped Saving!" + colorText.END)
 
 
 def saveNotifyResultsFile(
     screenResults, saveResults, defaultAnswer, menuChoiceHierarchy, user=None
 ):
```

### Comparing `pkscreener-0.44.20240422.286/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240423.287/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.286/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240423.287/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.286/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240423.287/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.286/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240423.287/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240422.286
+Version: 0.44.20240423.287
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240422.286.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240423.287.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240422.285/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240422.286/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240422.285/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240422.286/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240422.285/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240422.286/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240422.286/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240423.287/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.286/setup.py` & `pkscreener-0.44.20240423.287/setup.py`

 * *Files identical despite different names*

