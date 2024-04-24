# Comparing `tmp/cefi-4.6.6.tar.gz` & `tmp/cefi-4.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cefi-4.6.6.tar", max compression
+gzip compressed data, was "cefi-4.6.7.tar", max compression
```

## Comparing `cefi-4.6.6.tar` & `cefi-4.6.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1064 2024-04-20 05:06:10.580303 cefi-4.6.6/LICENSE
--rw-r--r--   0        0        0     2661 2024-04-20 05:06:10.580303 cefi-4.6.6/README.md
--rw-r--r--   0        0        0       87 2024-04-20 05:06:50.908071 cefi-4.6.6/cefi/__init__.py
--rw-r--r--   0        0        0      439 2024-04-20 05:06:10.580303 cefi-4.6.6/cefi/config.py
--rw-r--r--   0        0        0     3617 2024-04-20 05:06:10.580303 cefi-4.6.6/cefi/default_settings.toml
--rw-r--r--   0        0        0      158 2024-04-20 05:06:10.580303 cefi-4.6.6/cefi/handler/__init__.py
--rw-r--r--   0        0        0    11153 2024-04-20 05:06:10.580303 cefi-4.6.6/cefi/handler/capitalcom.py
--rw-r--r--   0        0        0     5517 2024-04-20 05:06:10.580303 cefi-4.6.6/cefi/handler/ccxt.py
--rw-r--r--   0        0        0     9015 2024-04-20 05:06:10.580303 cefi-4.6.6/cefi/handler/client.py
--rw-r--r--   0        0        0     1938 2024-04-20 05:06:10.580303 cefi-4.6.6/cefi/handler/ctrader.py
--rw-r--r--   0        0        0     7006 2024-04-20 05:06:10.580303 cefi-4.6.6/cefi/handler/ib_sync.py
--rw-r--r--   0        0        0     8160 2024-04-20 05:06:10.580303 cefi-4.6.6/cefi/main.py
--rw-r--r--   0        0        0     3772 2024-04-20 05:06:50.908071 cefi-4.6.6/pyproject.toml
--rw-r--r--   0        0        0     3657 1970-01-01 00:00:00.000000 cefi-4.6.6/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-24 04:10:13.202661 cefi-4.6.7/LICENSE
+-rw-r--r--   0        0        0     2661 2024-04-24 04:10:13.202661 cefi-4.6.7/README.md
+-rw-r--r--   0        0        0       87 2024-04-24 04:10:51.870606 cefi-4.6.7/cefi/__init__.py
+-rw-r--r--   0        0        0      439 2024-04-24 04:10:13.202661 cefi-4.6.7/cefi/config.py
+-rw-r--r--   0        0        0     3617 2024-04-24 04:10:13.202661 cefi-4.6.7/cefi/default_settings.toml
+-rw-r--r--   0        0        0      158 2024-04-24 04:10:13.202661 cefi-4.6.7/cefi/handler/__init__.py
+-rw-r--r--   0        0        0    11153 2024-04-24 04:10:13.202661 cefi-4.6.7/cefi/handler/capitalcom.py
+-rw-r--r--   0        0        0     5517 2024-04-24 04:10:13.202661 cefi-4.6.7/cefi/handler/ccxt.py
+-rw-r--r--   0        0        0     9015 2024-04-24 04:10:13.202661 cefi-4.6.7/cefi/handler/client.py
+-rw-r--r--   0        0        0     1938 2024-04-24 04:10:13.202661 cefi-4.6.7/cefi/handler/ctrader.py
+-rw-r--r--   0        0        0     7006 2024-04-24 04:10:13.202661 cefi-4.6.7/cefi/handler/ib_sync.py
+-rw-r--r--   0        0        0     8160 2024-04-24 04:10:13.202661 cefi-4.6.7/cefi/main.py
+-rw-r--r--   0        0        0     3776 2024-04-24 04:10:51.870606 cefi-4.6.7/pyproject.toml
+-rw-r--r--   0        0        0     3657 1970-01-01 00:00:00.000000 cefi-4.6.7/PKG-INFO
```

### Comparing `cefi-4.6.6/LICENSE` & `cefi-4.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cefi-4.6.6/README.md` & `cefi-4.6.7/README.md`

 * *Files identical despite different names*

### Comparing `cefi-4.6.6/cefi/default_settings.toml` & `cefi-4.6.7/cefi/default_settings.toml`

 * *Files identical despite different names*

### Comparing `cefi-4.6.6/cefi/handler/capitalcom.py` & `cefi-4.6.7/cefi/handler/capitalcom.py`

 * *Files identical despite different names*

### Comparing `cefi-4.6.6/cefi/handler/ccxt.py` & `cefi-4.6.7/cefi/handler/ccxt.py`

 * *Files identical despite different names*

### Comparing `cefi-4.6.6/cefi/handler/client.py` & `cefi-4.6.7/cefi/handler/client.py`

 * *Files identical despite different names*

### Comparing `cefi-4.6.6/cefi/handler/ctrader.py` & `cefi-4.6.7/cefi/handler/ctrader.py`

 * *Files identical despite different names*

### Comparing `cefi-4.6.6/cefi/handler/ib_sync.py` & `cefi-4.6.7/cefi/handler/ib_sync.py`

 * *Files identical despite different names*

### Comparing `cefi-4.6.6/cefi/main.py` & `cefi-4.6.7/cefi/main.py`

 * *Files identical despite different names*

### Comparing `cefi-4.6.6/pyproject.toml` & `cefi-4.6.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "cefi"
-version = "4.6.6"
+version = "4.6.7"
 description = "A python library, to interact  with Crypto Exchanges (CCXT library) and brokers (IB & Capital.com)"
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["cex, cefi, crypto, exchange, broker"]
 packages = [
     {include = "cefi"}
@@ -165,27 +165,29 @@
 
 
 
 
 
 
 
+
 [tool.poetry.group.test.dependencies]
 pytest = "^8.0.0"
-pytest-cov = "^4.1"
+pytest-cov = "^5.0.0"
 pytest-asyncio = "^0.23.0"
 pytest-mock = "^3.11.1"
 pytest-loguru = "^0.4.0"
 
 
 
 
 
 
 
+
```

### Comparing `cefi-4.6.6/PKG-INFO` & `cefi-4.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cefi
-Version: 4.6.6
+Version: 4.6.7
 Summary: A python library, to interact  with Crypto Exchanges (CCXT library) and brokers (IB & Capital.com)
 License: MIT
 Keywords: cex, cefi, crypto, exchange, broker
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cefi Version: 4.6.6 Summary: A python library, to
+Metadata-Version: 2.1 Name: cefi Version: 4.6.7 Summary: A python library, to
 interact with Crypto Exchanges (CCXT library) and brokers (IB & Capital.com)
 License: MIT Keywords: cex, cefi, crypto, exchange, broker Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com Requires-Python:
 >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: capitalcom-python
```

