# Comparing `tmp/YnExchangePY-3.2.2.tar.gz` & `tmp/YnExchangePY-3.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YnExchangePY-3.2.2.tar", last modified: Wed Apr 24 11:15:37 2024, max compression
+gzip compressed data, was "YnExchangePY-3.2.4.tar", last modified: Wed Apr 24 11:26:15 2024, max compression
```

## Comparing `YnExchangePY-3.2.2.tar` & `YnExchangePY-3.2.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 11:15:37.923386 YnExchangePY-3.2.2/
--rw-rw-rw-   0        0        0     3732 2024-04-24 11:15:37.918384 YnExchangePY-3.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     3369 2024-04-19 14:49:08.000000 YnExchangePY-3.2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 11:15:37.868411 YnExchangePY-3.2.2/YN_Exchange/
--rw-rw-rw-   0        0        0     1036 2024-04-24 11:14:19.000000 YnExchangePY-3.2.2/YN_Exchange/__init__.py
--rw-rw-rw-   0        0        0    31848 2024-04-24 11:11:46.000000 YnExchangePY-3.2.2/YN_Exchange/yn_exchange.py
-drwxrwxrwx   0        0        0        0 2024-04-24 11:15:37.914387 YnExchangePY-3.2.2/YnExchangePY.egg-info/
--rw-rw-rw-   0        0        0     3732 2024-04-24 11:15:37.000000 YnExchangePY-3.2.2/YnExchangePY.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2024-04-24 11:15:37.000000 YnExchangePY-3.2.2/YnExchangePY.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 11:15:37.000000 YnExchangePY-3.2.2/YnExchangePY.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-24 11:15:37.000000 YnExchangePY-3.2.2/YnExchangePY.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-24 11:15:37.000000 YnExchangePY-3.2.2/YnExchangePY.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 11:15:37.923386 YnExchangePY-3.2.2/setup.cfg
--rw-rw-rw-   0        0        0      674 2024-04-24 11:11:41.000000 YnExchangePY-3.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 11:26:15.221931 YnExchangePY-3.2.4/
+-rw-rw-rw-   0        0        0     3732 2024-04-24 11:26:15.206309 YnExchangePY-3.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3369 2024-04-19 14:49:08.000000 YnExchangePY-3.2.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 11:26:15.190684 YnExchangePY-3.2.4/YN_Exchange/
+-rw-rw-rw-   0        0        0    31848 2024-04-24 11:25:34.000000 YnExchangePY-3.2.4/YN_Exchange/YN_Exchange.py
+-rw-rw-rw-   0        0        0      967 2024-04-24 11:25:26.000000 YnExchangePY-3.2.4/YN_Exchange/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 11:26:15.206309 YnExchangePY-3.2.4/YnExchangePY.egg-info/
+-rw-rw-rw-   0        0        0     3732 2024-04-24 11:26:15.000000 YnExchangePY-3.2.4/YnExchangePY.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2024-04-24 11:26:15.000000 YnExchangePY-3.2.4/YnExchangePY.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 11:26:15.000000 YnExchangePY-3.2.4/YnExchangePY.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-24 11:26:15.000000 YnExchangePY-3.2.4/YnExchangePY.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-24 11:26:15.000000 YnExchangePY-3.2.4/YnExchangePY.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 11:26:15.221931 YnExchangePY-3.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      674 2024-04-24 11:25:31.000000 YnExchangePY-3.2.4/setup.py
```

### Comparing `YnExchangePY-3.2.2/PKG-INFO` & `YnExchangePY-3.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YnExchangePY
-Version: 3.2.2
+Version: 3.2.4
 Author: Yasha Najafi(YN)
 Author-email: <najafiyasha@gmail.com>
 Keywords: python,crypto,prices,crypto calculations,api,calculations
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: bs4
```

### Comparing `YnExchangePY-3.2.2/README.md` & `YnExchangePY-3.2.4/README.md`

 * *Files identical despite different names*

### Comparing `YnExchangePY-3.2.2/YN_Exchange/__init__.py` & `YnExchangePY-3.2.4/YN_Exchange/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,27 @@
-from YN_Exchange import yn_exchange
-from yn_exchange import TON_COIN_PRICE
-from yn_exchange import BTC_PRICE
-from yn_exchange import ETH_PRICE
-from yn_exchange import USDT_PRICE
-from yn_exchange import SHIB_PRICE
-from yn_exchange import BNB_PRICE
-from yn_exchange import DOGE_PRICE
-from yn_exchange import ADA_PRICE
-from yn_exchange import SOL_PRICE
-from yn_exchange import XRP_PRICE
-from yn_exchange import USDC_PRICE
-from yn_exchange import ETC_PRICE
-from yn_exchange import PEPE_PRICE
-from yn_exchange import ATM_PRICE
-from yn_exchange import BISO_PRICE
-from yn_exchange import calculator
-from yn_exchange import TRX_PRICE
-from yn_exchange import GOLD_OUNCE_PRICE
-from yn_exchange import GOLD_PRICE
-from yn_exchange import PALLADIUM_OUNCE_PRICE
-from yn_exchange import PLATINUM_OUNCE_PRICE
-from yn_exchange import SILVER_OUNCE_PRICE
-from yn_exchange import USD
-from yn_exchange import EUR
-from yn_exchange import TRY
-from yn_exchange import GBP
-from yn_exchange import AED
-import YN_Exchange.yn_exchange
+from YN_Exchange import TON_COIN_PRICE
+from YN_Exchange import BTC_PRICE
+from YN_Exchange import ETH_PRICE
+from YN_Exchange import USDT_PRICE
+from YN_Exchange import SHIB_PRICE
+from YN_Exchange import BNB_PRICE
+from YN_Exchange import DOGE_PRICE
+from YN_Exchange import ADA_PRICE
+from YN_Exchange import SOL_PRICE
+from YN_Exchange import XRP_PRICE
+from YN_Exchange import USDC_PRICE
+from YN_Exchange import ETC_PRICE
+from YN_Exchange import PEPE_PRICE
+from YN_Exchange import ATM_PRICE
+from YN_Exchange import BISO_PRICE
+from YN_Exchange import calculator
+from YN_Exchange import TRX_PRICE
+from YN_Exchange import GOLD_OUNCE_PRICE
+from YN_Exchange import GOLD_PRICE
+from YN_Exchange import PALLADIUM_OUNCE_PRICE
+from YN_Exchange import PLATINUM_OUNCE_PRICE
+from YN_Exchange import SILVER_OUNCE_PRICE
+from YN_Exchange import USD
+from YN_Exchange import EUR
+from YN_Exchange import TRY
+from YN_Exchange import GBP
+from YN_Exchange import AED
```

### Comparing `YnExchangePY-3.2.2/YN_Exchange/yn_exchange.py` & `YnExchangePY-3.2.4/YN_Exchange/YN_Exchange.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #----------------<info>-----------
 # Developed by : Yasha Najafi
 # Developer github : https://github.com/YashaNajafi
 # Developer info page : https://YashaNajafi.github.io/about_me
-# Module version : 3.2.2
+# Module version : 3.2.4
 # Module name : YN_EXCHANGE
 # Number of supported crypto : 16
 # References : https://ok-ex.io/ | https://www.tgju.org/ | https://www.xe.com/
 
 #----------------<libs>----------
 import requests
 from bs4 import BeautifulSoup
```

### Comparing `YnExchangePY-3.2.2/YnExchangePY.egg-info/PKG-INFO` & `YnExchangePY-3.2.4/YnExchangePY.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YnExchangePY
-Version: 3.2.2
+Version: 3.2.4
 Author: Yasha Najafi(YN)
 Author-email: <najafiyasha@gmail.com>
 Keywords: python,crypto,prices,crypto calculations,api,calculations
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: bs4
```

### Comparing `YnExchangePY-3.2.2/setup.py` & `YnExchangePY-3.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '3.2.2'
+VERSION = '3.2.4'
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     LONG_DESCRIPTION = "\n" + fh.read()
 
 
 # Setting up
```

