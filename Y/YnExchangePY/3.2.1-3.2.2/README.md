# Comparing `tmp/YnExchangePY-3.2.1.tar.gz` & `tmp/YnExchangePY-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YnExchangePY-3.2.1.tar", last modified: Wed Apr 24 10:59:47 2024, max compression
+gzip compressed data, was "YnExchangePY-3.2.2.tar", last modified: Wed Apr 24 11:15:37 2024, max compression
```

## Comparing `YnExchangePY-3.2.1.tar` & `YnExchangePY-3.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 10:59:47.447939 YnExchangePY-3.2.1/
--rw-rw-rw-   0        0        0     3732 2024-04-24 10:59:47.446940 YnExchangePY-3.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     3369 2024-04-19 14:49:08.000000 YnExchangePY-3.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 10:59:47.407961 YnExchangePY-3.2.1/YN_Exchange/
--rw-rw-rw-   0        0        0      967 2024-04-24 10:28:56.000000 YnExchangePY-3.2.1/YN_Exchange/__init__.py
--rw-rw-rw-   0        0        0    31848 2024-04-24 10:58:24.000000 YnExchangePY-3.2.1/YN_Exchange/yn_exchange.py
-drwxrwxrwx   0        0        0        0 2024-04-24 10:59:47.445940 YnExchangePY-3.2.1/YnExchangePY.egg-info/
--rw-rw-rw-   0        0        0     3732 2024-04-24 10:59:46.000000 YnExchangePY-3.2.1/YnExchangePY.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2024-04-24 10:59:46.000000 YnExchangePY-3.2.1/YnExchangePY.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 10:59:46.000000 YnExchangePY-3.2.1/YnExchangePY.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-24 10:59:46.000000 YnExchangePY-3.2.1/YnExchangePY.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-24 10:59:46.000000 YnExchangePY-3.2.1/YnExchangePY.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 10:59:47.447939 YnExchangePY-3.2.1/setup.cfg
--rw-rw-rw-   0        0        0      674 2024-04-24 10:58:33.000000 YnExchangePY-3.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 11:15:37.923386 YnExchangePY-3.2.2/
+-rw-rw-rw-   0        0        0     3732 2024-04-24 11:15:37.918384 YnExchangePY-3.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3369 2024-04-19 14:49:08.000000 YnExchangePY-3.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 11:15:37.868411 YnExchangePY-3.2.2/YN_Exchange/
+-rw-rw-rw-   0        0        0     1036 2024-04-24 11:14:19.000000 YnExchangePY-3.2.2/YN_Exchange/__init__.py
+-rw-rw-rw-   0        0        0    31848 2024-04-24 11:11:46.000000 YnExchangePY-3.2.2/YN_Exchange/yn_exchange.py
+drwxrwxrwx   0        0        0        0 2024-04-24 11:15:37.914387 YnExchangePY-3.2.2/YnExchangePY.egg-info/
+-rw-rw-rw-   0        0        0     3732 2024-04-24 11:15:37.000000 YnExchangePY-3.2.2/YnExchangePY.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2024-04-24 11:15:37.000000 YnExchangePY-3.2.2/YnExchangePY.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 11:15:37.000000 YnExchangePY-3.2.2/YnExchangePY.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-24 11:15:37.000000 YnExchangePY-3.2.2/YnExchangePY.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-24 11:15:37.000000 YnExchangePY-3.2.2/YnExchangePY.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 11:15:37.923386 YnExchangePY-3.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      674 2024-04-24 11:11:41.000000 YnExchangePY-3.2.2/setup.py
```

### Comparing `YnExchangePY-3.2.1/PKG-INFO` & `YnExchangePY-3.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YnExchangePY
-Version: 3.2.1
+Version: 3.2.2
 Author: Yasha Najafi(YN)
 Author-email: <najafiyasha@gmail.com>
 Keywords: python,crypto,prices,crypto calculations,api,calculations
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: bs4
```

### Comparing `YnExchangePY-3.2.1/README.md` & `YnExchangePY-3.2.2/README.md`

 * *Files identical despite different names*

### Comparing `YnExchangePY-3.2.1/YN_Exchange/__init__.py` & `YnExchangePY-3.2.2/YN_Exchange/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from YN_Exchange import yn_exchange
 from yn_exchange import TON_COIN_PRICE
 from yn_exchange import BTC_PRICE
 from yn_exchange import ETH_PRICE
 from yn_exchange import USDT_PRICE
 from yn_exchange import SHIB_PRICE
 from yn_exchange import BNB_PRICE
 from yn_exchange import DOGE_PRICE
@@ -21,7 +22,8 @@
 from yn_exchange import PLATINUM_OUNCE_PRICE
 from yn_exchange import SILVER_OUNCE_PRICE
 from yn_exchange import USD
 from yn_exchange import EUR
 from yn_exchange import TRY
 from yn_exchange import GBP
 from yn_exchange import AED
+import YN_Exchange.yn_exchange
```

### Comparing `YnExchangePY-3.2.1/YN_Exchange/yn_exchange.py` & `YnExchangePY-3.2.2/YN_Exchange/yn_exchange.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #----------------<info>-----------
 # Developed by : Yasha Najafi
 # Developer github : https://github.com/YashaNajafi
 # Developer info page : https://YashaNajafi.github.io/about_me
-# Module version : 3.2.1
+# Module version : 3.2.2
 # Module name : YN_EXCHANGE
 # Number of supported crypto : 16
 # References : https://ok-ex.io/ | https://www.tgju.org/ | https://www.xe.com/
 
 #----------------<libs>----------
 import requests
 from bs4 import BeautifulSoup
```

### Comparing `YnExchangePY-3.2.1/YnExchangePY.egg-info/PKG-INFO` & `YnExchangePY-3.2.2/YnExchangePY.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YnExchangePY
-Version: 3.2.1
+Version: 3.2.2
 Author: Yasha Najafi(YN)
 Author-email: <najafiyasha@gmail.com>
 Keywords: python,crypto,prices,crypto calculations,api,calculations
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: bs4
```

### Comparing `YnExchangePY-3.2.1/setup.py` & `YnExchangePY-3.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '3.2.1'
+VERSION = '3.2.2'
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     LONG_DESCRIPTION = "\n" + fh.read()
 
 
 # Setting up
```

