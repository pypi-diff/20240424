# Comparing `tmp/dxsp-9.0.6.tar.gz` & `tmp/dxsp-9.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-9.0.6.tar", max compression
+gzip compressed data, was "dxsp-9.0.7.tar", max compression
```

## Comparing `dxsp-9.0.6.tar` & `dxsp-9.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1064 2024-03-30 11:12:17.745669 dxsp-9.0.6/LICENSE
--rw-r--r--   0        0        0     2487 2024-03-30 11:12:17.745669 dxsp-9.0.6/README.md
--rw-r--r--   0        0        0       83 2024-03-30 11:14:02.749996 dxsp-9.0.6/dxsp/__init__.py
--rw-r--r--   0        0        0      439 2024-03-30 11:12:17.745669 dxsp-9.0.6/dxsp/config.py
--rw-r--r--   0        0        0     5845 2024-03-30 11:12:17.745669 dxsp-9.0.6/dxsp/default_settings.toml
--rw-r--r--   0        0        0      204 2024-03-30 11:12:17.745669 dxsp-9.0.6/dxsp/handler/__init__.py
--rw-r--r--   0        0        0    11124 2024-03-30 11:12:17.745669 dxsp-9.0.6/dxsp/handler/client.py
--rw-r--r--   0        0        0     4224 2024-03-30 11:12:17.745669 dxsp-9.0.6/dxsp/handler/kwenta.py
--rw-r--r--   0        0        0     3965 2024-03-30 11:12:17.745669 dxsp-9.0.6/dxsp/handler/oneinch.py
--rw-r--r--   0        0        0     4572 2024-03-30 11:12:17.745669 dxsp-9.0.6/dxsp/handler/uniswap.py
--rw-r--r--   0        0        0     3382 2024-03-30 11:12:17.745669 dxsp-9.0.6/dxsp/handler/zerox.py
--rw-r--r--   0        0        0     9007 2024-03-30 11:12:17.745669 dxsp-9.0.6/dxsp/main.py
--rw-r--r--   0        0        0      158 2024-03-30 11:12:17.745669 dxsp-9.0.6/dxsp/utils/__init__.py
--rw-r--r--   0        0        0     5856 2024-03-30 11:12:17.745669 dxsp-9.0.6/dxsp/utils/account_utils.py
--rw-r--r--   0        0        0    15840 2024-03-30 11:12:17.745669 dxsp-9.0.6/dxsp/utils/contract_utils.py
--rw-r--r--   0        0        0     1349 2024-03-30 11:12:17.745669 dxsp-9.0.6/dxsp/utils/utils.py
--rw-r--r--   0        0        0     3604 2024-03-30 11:14:02.749996 dxsp-9.0.6/pyproject.toml
--rw-r--r--   0        0        0     3499 1970-01-01 00:00:00.000000 dxsp-9.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-06 07:43:36.149440 dxsp-9.0.7/LICENSE
+-rw-r--r--   0        0        0     2487 2024-04-06 07:43:36.149440 dxsp-9.0.7/README.md
+-rw-r--r--   0        0        0       83 2024-04-06 07:45:21.253326 dxsp-9.0.7/dxsp/__init__.py
+-rw-r--r--   0        0        0      439 2024-04-06 07:43:36.149440 dxsp-9.0.7/dxsp/config.py
+-rw-r--r--   0        0        0     5845 2024-04-06 07:43:36.149440 dxsp-9.0.7/dxsp/default_settings.toml
+-rw-r--r--   0        0        0      204 2024-04-06 07:43:36.149440 dxsp-9.0.7/dxsp/handler/__init__.py
+-rw-r--r--   0        0        0    11124 2024-04-06 07:43:36.149440 dxsp-9.0.7/dxsp/handler/client.py
+-rw-r--r--   0        0        0     4224 2024-04-06 07:43:36.149440 dxsp-9.0.7/dxsp/handler/kwenta.py
+-rw-r--r--   0        0        0     3965 2024-04-06 07:43:36.149440 dxsp-9.0.7/dxsp/handler/oneinch.py
+-rw-r--r--   0        0        0     4572 2024-04-06 07:43:36.149440 dxsp-9.0.7/dxsp/handler/uniswap.py
+-rw-r--r--   0        0        0     3382 2024-04-06 07:43:36.149440 dxsp-9.0.7/dxsp/handler/zerox.py
+-rw-r--r--   0        0        0     9007 2024-04-06 07:43:36.149440 dxsp-9.0.7/dxsp/main.py
+-rw-r--r--   0        0        0      158 2024-04-06 07:43:36.149440 dxsp-9.0.7/dxsp/utils/__init__.py
+-rw-r--r--   0        0        0     5856 2024-04-06 07:43:36.149440 dxsp-9.0.7/dxsp/utils/account_utils.py
+-rw-r--r--   0        0        0    15840 2024-04-06 07:43:36.149440 dxsp-9.0.7/dxsp/utils/contract_utils.py
+-rw-r--r--   0        0        0     1349 2024-04-06 07:43:36.149440 dxsp-9.0.7/dxsp/utils/utils.py
+-rw-r--r--   0        0        0     3606 2024-04-06 07:45:21.253326 dxsp-9.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3499 1970-01-01 00:00:00.000000 dxsp-9.0.7/PKG-INFO
```

### Comparing `dxsp-9.0.6/LICENSE` & `dxsp-9.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-9.0.6/README.md` & `dxsp-9.0.7/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-9.0.6/dxsp/default_settings.toml` & `dxsp-9.0.7/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-9.0.6/dxsp/handler/client.py` & `dxsp-9.0.7/dxsp/handler/client.py`

 * *Files identical despite different names*

### Comparing `dxsp-9.0.6/dxsp/handler/kwenta.py` & `dxsp-9.0.7/dxsp/handler/kwenta.py`

 * *Files identical despite different names*

### Comparing `dxsp-9.0.6/dxsp/handler/oneinch.py` & `dxsp-9.0.7/dxsp/handler/oneinch.py`

 * *Files identical despite different names*

### Comparing `dxsp-9.0.6/dxsp/handler/uniswap.py` & `dxsp-9.0.7/dxsp/handler/uniswap.py`

 * *Files identical despite different names*

### Comparing `dxsp-9.0.6/dxsp/handler/zerox.py` & `dxsp-9.0.7/dxsp/handler/zerox.py`

 * *Files identical despite different names*

### Comparing `dxsp-9.0.6/dxsp/main.py` & `dxsp-9.0.7/dxsp/main.py`

 * *Files identical despite different names*

### Comparing `dxsp-9.0.6/dxsp/utils/account_utils.py` & `dxsp-9.0.7/dxsp/utils/account_utils.py`

 * *Files identical despite different names*

### Comparing `dxsp-9.0.6/dxsp/utils/contract_utils.py` & `dxsp-9.0.7/dxsp/utils/contract_utils.py`

 * *Files identical despite different names*

### Comparing `dxsp-9.0.6/dxsp/utils/utils.py` & `dxsp-9.0.7/dxsp/utils/utils.py`

 * *Files identical despite different names*

### Comparing `dxsp-9.0.6/pyproject.toml` & `dxsp-9.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "dxsp"
-version = "9.0.6"
+version = "9.0.7"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [
     {include = "dxsp"}
 ]
@@ -25,15 +25,15 @@
 dynaconf = ">=3.2.0"
 loguru = ">=0.6.0"
 pycoingecko = "3.1.0"
 requests = "^2.31.0"
 web3 = "6.16.0"
 uniswap-python = "0.7.1"
 kwenta = "1.2.0"
-eth-ape = "0.7.13"
+eth-ape = "0.7.14"
 #eth-tester = "0.9.1b2"
 # brownie_safe = {version="0.8.5", python = ">=3.11,<3.12"}
 # eth-brownie = "1.20.1"
 #web3client = "1.3.7"
 
 
 [tool.poetry.group.dev.dependencies]
@@ -87,14 +87,15 @@
 
 
 
 
 
 
 
+
 [tool.poetry.group.test.dependencies]
 pytest = "^7.0"
 pytest-cov = "^4.1"
 pytest-asyncio = "^0.23.0"
 pytest-mock = "^3.11.1"
 pytest-loguru = "^0.4.0"
 eth_tester = "^0.9.0b2"
@@ -126,14 +127,15 @@
 
 
 
 
 
 
 
+
```

### Comparing `dxsp-9.0.6/PKG-INFO` & `dxsp-9.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 9.0.6
+Version: 9.0.7
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: dynaconf (>=3.2.0)
-Requires-Dist: eth-ape (==0.7.13)
+Requires-Dist: eth-ape (==0.7.14)
 Requires-Dist: kwenta (==1.2.0)
 Requires-Dist: loguru (>=0.6.0)
 Requires-Dist: pycoingecko (==3.1.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: uniswap-python (==0.7.1)
 Requires-Dist: web3 (==6.16.0)
 Project-URL: Changelog, https://github.com/mraniki/dxsp/blob/dev/CHANGELOG.rst
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: dxsp Version: 9.0.6 Summary: DXSP (DeX SwaP), A
+Metadata-Version: 2.1 Name: dxsp Version: 9.0.7 Summary: DXSP (DeX SwaP), A
 defi swap helper package. Swap made easy. License: MIT Author: mraniki Author-
 email: 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Dist: dynaconf (>=3.2.0) Requires-Dist:
-eth-ape (==0.7.13) Requires-Dist: kwenta (==1.2.0) Requires-Dist: loguru
+eth-ape (==0.7.14) Requires-Dist: kwenta (==1.2.0) Requires-Dist: loguru
 (>=0.6.0) Requires-Dist: pycoingecko (==3.1.0) Requires-Dist: requests
 (>=2.31.0,<3.0.0) Requires-Dist: uniswap-python (==0.7.1) Requires-Dist: web3
 (==6.16.0) Project-URL: Changelog, https://github.com/mraniki/dxsp/blob/dev/
 CHANGELOG.rst Project-URL: Issues, https://github.com/mraniki/dxsp/issues
 Project-URL: Support, https://github.com/mraniki/dxsp/discussions Description-
 Content-Type: text/markdown
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_W_i_k_i_-_%_2_3_0_0_0_0_0_0_._s_v_g_?_s_t_y_l_e_=_f_o_r_-
```

