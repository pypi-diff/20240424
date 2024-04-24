# Comparing `tmp/pybankid-1.0.1.tar.gz` & `tmp/pybankid-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybankid-1.0.1.tar", last modified: Fri Apr 12 21:51:33 2024, max compression
+gzip compressed data, was "pybankid-1.1.0.tar", last modified: Wed Apr 24 20:34:12 2024, max compression
```

## Comparing `pybankid-1.0.1.tar` & `pybankid-1.1.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:51:33.917935 pybankid-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-12 21:51:29.000000 pybankid-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-12 21:51:29.000000 pybankid-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8038 2024-04-12 21:51:33.917935 pybankid-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-04-12 21:51:29.000000 pybankid-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:51:33.909934 pybankid-1.0.1/bankid/
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-12 21:51:29.000000 pybankid-1.0.1/bankid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-12 21:51:29.000000 pybankid-1.0.1/bankid/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14872 2024-04-12 21:51:29.000000 pybankid-1.0.1/bankid/asyncclient.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-12 21:51:29.000000 pybankid-1.0.1/bankid/baseclient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:51:33.909934 pybankid-1.0.1/bankid/certs/
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-04-12 21:51:29.000000 pybankid-1.0.1/bankid/certs/FPTestcert4_20220818.p12
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-12 21:51:29.000000 pybankid-1.0.1/bankid/certs/FPTestcert4_20220818_cert.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-12 21:51:29.000000 pybankid-1.0.1/bankid/certs/FPTestcert4_20220818_key.pem
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-04-12 21:51:29.000000 pybankid-1.0.1/bankid/certs/FPTestcert4_20230629.p12
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-12 21:51:29.000000 pybankid-1.0.1/bankid/certs/FPTestcert4_20230629_cert.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-12 21:51:29.000000 pybankid-1.0.1/bankid/certs/FPTestcert4_20230629_key.pem
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-12 21:51:29.000000 pybankid-1.0.1/bankid/certs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-12 21:51:29.000000 pybankid-1.0.1/bankid/certs/appapi.bankid.com.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-12 21:51:29.000000 pybankid-1.0.1/bankid/certs/appapi.test.bankid.com.pem
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-12 21:51:29.000000 pybankid-1.0.1/bankid/certs/appapi2.bankid.com.pem
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-12 21:51:29.000000 pybankid-1.0.1/bankid/certs/appapi2.test.bankid.com.pem
--rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-04-12 21:51:29.000000 pybankid-1.0.1/bankid/certutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-12 21:51:29.000000 pybankid-1.0.1/bankid/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:51:33.913935 pybankid-1.0.1/bankid/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 21:51:29.000000 pybankid-1.0.1/bankid/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-12 21:51:29.000000 pybankid-1.0.1/bankid/experimental/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9708 2024-04-12 21:51:29.000000 pybankid-1.0.1/bankid/experimental/verify.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-12 21:51:29.000000 pybankid-1.0.1/bankid/qr.py
--rw-r--r--   0 runner    (1001) docker     (127)    14794 2024-04-12 21:51:29.000000 pybankid-1.0.1/bankid/syncclient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:51:33.905934 pybankid-1.0.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:51:33.913935 pybankid-1.0.1/examples/qrdemo/
--rw-r--r--   0 runner    (1001) docker     (127)    11296 2024-04-12 21:51:29.000000 pybankid-1.0.1/examples/qrdemo/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-12 21:51:29.000000 pybankid-1.0.1/examples/qrdemo/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:51:33.913935 pybankid-1.0.1/examples/qrdemo/qrdemo/
--rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-04-12 21:51:29.000000 pybankid-1.0.1/examples/qrdemo/qrdemo/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:51:33.913935 pybankid-1.0.1/examples/qrdemo/qrdemo/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-12 21:51:29.000000 pybankid-1.0.1/examples/qrdemo/qrdemo/templates/auth_complete.html
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-12 21:51:29.000000 pybankid-1.0.1/examples/qrdemo/qrdemo/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-04-12 21:51:29.000000 pybankid-1.0.1/examples/qrdemo/qrdemo/templates/qr.html
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-12 21:51:29.000000 pybankid-1.0.1/examples/qrdemo/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:51:33.913935 pybankid-1.0.1/pybankid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8038 2024-04-12 21:51:33.000000 pybankid-1.0.1/pybankid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-12 21:51:33.000000 pybankid-1.0.1/pybankid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 21:51:33.000000 pybankid-1.0.1/pybankid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-12 21:51:33.000000 pybankid-1.0.1/pybankid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 21:51:33.000000 pybankid-1.0.1/pybankid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-12 21:51:29.000000 pybankid-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-12 21:51:33.917935 pybankid-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-12 21:51:29.000000 pybankid-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:51:33.913935 pybankid-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 21:51:29.000000 pybankid-1.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-12 21:51:29.000000 pybankid-1.0.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-04-12 21:51:29.000000 pybankid-1.0.1/tests/test_asyncclient.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-12 21:51:29.000000 pybankid-1.0.1/tests/test_certutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-12 21:51:29.000000 pybankid-1.0.1/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-04-12 21:51:29.000000 pybankid-1.0.1/tests/test_syncclient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:34:12.146315 pybankid-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-24 20:34:08.000000 pybankid-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-24 20:34:08.000000 pybankid-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8265 2024-04-24 20:34:12.146315 pybankid-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7306 2024-04-24 20:34:08.000000 pybankid-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:34:12.138315 pybankid-1.1.0/bankid/
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-24 20:34:08.000000 pybankid-1.1.0/bankid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-24 20:34:08.000000 pybankid-1.1.0/bankid/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15147 2024-04-24 20:34:08.000000 pybankid-1.1.0/bankid/asyncclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-04-24 20:34:08.000000 pybankid-1.1.0/bankid/baseclient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:34:12.142315 pybankid-1.1.0/bankid/certs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-04-24 20:34:08.000000 pybankid-1.1.0/bankid/certs/FPTestcert4_20220818.p12
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-24 20:34:08.000000 pybankid-1.1.0/bankid/certs/FPTestcert4_20220818_cert.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-24 20:34:08.000000 pybankid-1.1.0/bankid/certs/FPTestcert4_20220818_key.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-04-24 20:34:08.000000 pybankid-1.1.0/bankid/certs/FPTestcert4_20230629.p12
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-24 20:34:08.000000 pybankid-1.1.0/bankid/certs/FPTestcert4_20230629_cert.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-24 20:34:08.000000 pybankid-1.1.0/bankid/certs/FPTestcert4_20230629_key.pem
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-24 20:34:08.000000 pybankid-1.1.0/bankid/certs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-24 20:34:08.000000 pybankid-1.1.0/bankid/certs/appapi.bankid.com.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-24 20:34:08.000000 pybankid-1.1.0/bankid/certs/appapi.test.bankid.com.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-24 20:34:08.000000 pybankid-1.1.0/bankid/certs/appapi2.bankid.com.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-24 20:34:08.000000 pybankid-1.1.0/bankid/certs/appapi2.test.bankid.com.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-04-24 20:34:08.000000 pybankid-1.1.0/bankid/certutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-04-24 20:34:08.000000 pybankid-1.1.0/bankid/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:34:12.142315 pybankid-1.1.0/bankid/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:34:08.000000 pybankid-1.1.0/bankid/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-24 20:34:08.000000 pybankid-1.1.0/bankid/experimental/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9708 2024-04-24 20:34:08.000000 pybankid-1.1.0/bankid/experimental/verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-24 20:34:08.000000 pybankid-1.1.0/bankid/qr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15055 2024-04-24 20:34:08.000000 pybankid-1.1.0/bankid/syncclient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:34:12.138315 pybankid-1.1.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:34:12.142315 pybankid-1.1.0/examples/qrdemo/
+-rw-r--r--   0 runner    (1001) docker     (127)    11296 2024-04-24 20:34:08.000000 pybankid-1.1.0/examples/qrdemo/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-24 20:34:08.000000 pybankid-1.1.0/examples/qrdemo/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:34:12.142315 pybankid-1.1.0/examples/qrdemo/qrdemo/
+-rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-04-24 20:34:08.000000 pybankid-1.1.0/examples/qrdemo/qrdemo/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:34:12.142315 pybankid-1.1.0/examples/qrdemo/qrdemo/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-24 20:34:08.000000 pybankid-1.1.0/examples/qrdemo/qrdemo/templates/auth_complete.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-24 20:34:08.000000 pybankid-1.1.0/examples/qrdemo/qrdemo/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-04-24 20:34:08.000000 pybankid-1.1.0/examples/qrdemo/qrdemo/templates/qr.html
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-24 20:34:08.000000 pybankid-1.1.0/examples/qrdemo/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:34:12.146315 pybankid-1.1.0/pybankid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8265 2024-04-24 20:34:12.000000 pybankid-1.1.0/pybankid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-24 20:34:12.000000 pybankid-1.1.0/pybankid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 20:34:12.000000 pybankid-1.1.0/pybankid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-24 20:34:12.000000 pybankid-1.1.0/pybankid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 20:34:12.000000 pybankid-1.1.0/pybankid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 20:34:08.000000 pybankid-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-24 20:34:12.146315 pybankid-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-24 20:34:08.000000 pybankid-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:34:12.146315 pybankid-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:34:08.000000 pybankid-1.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-24 20:34:08.000000 pybankid-1.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5784 2024-04-24 20:34:08.000000 pybankid-1.1.0/tests/test_asyncclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-24 20:34:08.000000 pybankid-1.1.0/tests/test_certutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-24 20:34:08.000000 pybankid-1.1.0/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-04-24 20:34:08.000000 pybankid-1.1.0/tests/test_syncclient.py
```

### Comparing `pybankid-1.0.1/LICENSE` & `pybankid-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.1/PKG-INFO` & `pybankid-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybankid
-Version: 1.0.1
+Version: 1.1.0
 Summary: BankID Relying Party client for Python
 Home-page: https://github.com/hbldh/pybankid
 Author: Henrik Blidh
 Author-email: henrik.blidh@nedomkull.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -15,28 +15,26 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx
-Requires-Dist: importlib-resources>=5.12.0
 Provides-Extra: signature-verification
 Requires-Dist: pyOpenSSL; extra == "signature-verification"
-Requires-Dist: pytz; extra == "signature-verification"
 Requires-Dist: asn1crypto; extra == "signature-verification"
+Requires-Dist: pytz; extra == "signature-verification"
 
 
 # PyBankID
 
 ![Build and Test](https://github.com/hbldh/pybankid/workflows/Build%20and%20Test/badge.svg)
 ![Documentation Status](https://readthedocs.org/projects/pybankid/badge/?version=latest)
-![PyPI Version](http://img.shields.io/pypi/v/pybankid.svg)
-![PyPI License](http://img.shields.io/pypi/l/pybankid.svg)
-![Coverage](https://coveralls.io/repos/github/hbldh/pybankid/badge.svg?branch=master)
+![PyPI Version](https://img.shields.io/pypi/v/pybankid)
+![PyPI License](https://img.shields.io/pypi/l/pybankid)
 
 PyBankID is a client for providing BankID services as a Relying Party, i.e., providing authentication and signing functionality to end users. This package provides a simplifying interface for initiating authentication and signing orders and then collecting the results from the BankID servers.
 
 The only supported BankID API version supported by PyBankID from version 1.0.0 is v6.0, which means that the Secure Start solution is the only supported way of providing BankID services. PyBankID versions prior to 1.0.0 will not work after 1st of May 2024.
 
 If you intend to use PyBankID in your project, you are advised to read the [BankID Integration Guide](https://www.bankid.com/en/utvecklare/guider/teknisk-integrationsguide) before doing anything else. There, one can find information about how the BankID methods are defined and how to use them.
 
@@ -46,29 +44,29 @@
 
 ```bash
 pip install pybankid
 ```
 
 ## Usage
 
-PyBankID provides both a synchronous and an asynchronous client for communication with BankID services. The example below will use the asynchronous client, but the synchronous client is used in the same way by merely omitting the `await` keyword.
+PyBankID provides both a synchronous and an asynchronous client for communication with BankID services. The example below will use the synchronous client, but the asynchronous client is used in an identical fashion, only using the `await` keyword before each function call.
 
 ### Synchronous client
 
 ```python
 from bankid import BankIDClient
 client = BankIDClient(certificates=(
-    'path/to/certificate.pem', 
-    'path/to/key.pem', 
+    'path/to/certificate.pem',
+    'path/to/key.pem',
 ))
 ```
 
 Connection to the production server is the default in the client. If a test server is desired, send in the `test_server=True` keyword in the init of the client.
 
-When using the JSON client, authentication and signing calls require the end user's IP address to be included in all calls. An authentication order is initiated as such:
+All authentication and signing calls require the end user's IP address to be included. An authentication order is initiated as such:
 
 ```python
 client.authenticate(end_user_ip='194.168.2.25')
 {
     'orderRef': 'ee3421ea-2096-4000-8130-82648efe0927',
     'autoStartToken': 'e8df5c3c-c67b-4a01-bfe5-fefeab760beb',
     'qrStartToken': '01f94e28-857f-4d8a-bf8e-6c5a24466658',
@@ -103,15 +101,15 @@
     'orderRef': 'ee3421ea-2096-4000-8130-82648efe0927',
     'autoStartToken': 'e8df5c3c-c67b-4a01-bfe5-fefeab760beb',
     'qrStartToken': '01f94e28-857f-4d8a-bf8e-6c5a24466658',
     'qrStartSecret': 'b4214886-3b5b-46ab-bc08-6862fddc0e06'
 }
 ```
 
-If someone else than the one you specified tries to authenticate or sign, the BankID app will state that the request is not intended for the user.
+If someone other than the one you specified tries to authenticate or sign, the BankID app will state that the request is not intended for the user.
 
 The status of an order can then be studied by polling with the `collect` method using the received `orderRef`:
 
 ```python
 client.collect(order_ref="a9b791c3-459f-492b-bf61-23027876140b")
 {
     'hintCode': 'outstandingTransaction',
@@ -150,43 +148,47 @@
         }
     },
     'orderRef': 'a9b791c3-459f-492b-bf61-23027876140b',
     'status': 'complete'
 }
 ```
 
+Please note that the `collect` method should be used sparingly: in the [BankID Integration Guide](https://www.bankid.com/en/utvecklare/guider/teknisk-integrationsguide) it is specified that _"collect should be called every two seconds and must not be called more frequent than once per second"_.
 
-Please note that the `collect` method should be used sparingly: in the [BankID Integration Guide](https://www.bankid.com/en/utvecklare/guider/teknisk-integrationsguide) it is specified that *"collect should be called every two seconds and must not be called more frequent than once per second"*.
+PyBankID also implements the `phone/auth` and `phone/sign` methods, for performing authentication and signing with
+users that are contacted through phone. For documentation on this, see [PyBankID's Read the Docs page](https://pybankid.readthedocs.io/en/latest/).
 
 ### Asynchronous client
 
-The asynchronous client is used in the same way as the synchronous client, but the methods are blocking.
+The asynchronous client is used in the same way as the synchronous client, with the difference that all request are performed asynchronously.
 
 The synchronous guide above can be used as a reference for the asynchronous client as well, by simply adding the `await` keyword:
 
 ```python
-from bankid import BankIDClientAsync
-client = BankIDClientAsync(certificates=(
-    'path/to/certificate.pem', 
-    'path/to/key.pem', 
+from bankid import BankIDAsyncClient
+client = BankIDAsyncClient(certificates=(
+    'path/to/certificate.pem',
+    'path/to/key.pem',
 ))
 
 await client.authenticate(end_user_ip='194.168.2.25')
 {
     'orderRef': 'ee3421ea-2096-4000-8130-82648efe0927',
     'autoStartToken': 'e8df5c3c-c67b-4a01-bfe5-fefeab760beb',
     'qrStartToken': '01f94e28-857f-4d8a-bf8e-6c5a24466658',
     'qrStartSecret': 'b4214886-3b5b-46ab-bc08-6862fddc0e06'
 }
 ```
 
-
 ## PyBankID and QR codes
 
-PyBankID can generate QR codes for you, and there is an example application in the [examples folder of the repo](https://github.com/hbldh/pybankid/tree/master/examples) where a Flask application called `qrdemo` shows one way to do authentication with animated QR codes.
+PyBankID can generate QR codes for you, and there is an example application in the [examples folder of the repo](https://github.com/hbldh/pybankid/tree/master/examples), where a Flask application called `qrdemo` shows one way to do authentication with animated QR codes.
+
+The QR code content generation is done with the `generate_qr_code_content` method on the BankID Client instances, or directly
+through the identically named method in `bankid.qr` module.
 
 ## Certificates
 
 ### Production certificates
 
 If you want to use BankID in a production environment, then you will have to purchase this service from one of the [selling banks](https://www.bankid.com/foretag/anslut-foeretag). They will then provide you with a certificate that can be used to authenticate your company/application with the BankID servers.
 
@@ -203,15 +205,7 @@
 cert_and_key = bankid.create_bankid_test_server_cert_and_key(
     dir_to_save_cert_and_key_in)
 print(cert_and_key)
 ['/home/hbldh/certificate.pem', '/home/hbldh/key.pem']
 client = bankid.BankIDClient(
     certificates=cert_and_key, test_server=True)
 ```
-
-## Testing
-
-The PyBankID solution can be tested with [pytest](https://pytest.org/):
-
-```bash
-pytest tests/
-```
```

### Comparing `pybankid-1.0.1/README.md` & `pybankid-1.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # PyBankID
 
 ![Build and Test](https://github.com/hbldh/pybankid/workflows/Build%20and%20Test/badge.svg)
 ![Documentation Status](https://readthedocs.org/projects/pybankid/badge/?version=latest)
-![PyPI Version](http://img.shields.io/pypi/v/pybankid.svg)
-![PyPI License](http://img.shields.io/pypi/l/pybankid.svg)
-![Coverage](https://coveralls.io/repos/github/hbldh/pybankid/badge.svg?branch=master)
+![PyPI Version](https://img.shields.io/pypi/v/pybankid)
+![PyPI License](https://img.shields.io/pypi/l/pybankid)
 
 PyBankID is a client for providing BankID services as a Relying Party, i.e., providing authentication and signing functionality to end users. This package provides a simplifying interface for initiating authentication and signing orders and then collecting the results from the BankID servers.
 
 The only supported BankID API version supported by PyBankID from version 1.0.0 is v6.0, which means that the Secure Start solution is the only supported way of providing BankID services. PyBankID versions prior to 1.0.0 will not work after 1st of May 2024.
 
 If you intend to use PyBankID in your project, you are advised to read the [BankID Integration Guide](https://www.bankid.com/en/utvecklare/guider/teknisk-integrationsguide) before doing anything else. There, one can find information about how the BankID methods are defined and how to use them.
 
@@ -18,29 +17,29 @@
 
 ```bash
 pip install pybankid
 ```
 
 ## Usage
 
-PyBankID provides both a synchronous and an asynchronous client for communication with BankID services. The example below will use the asynchronous client, but the synchronous client is used in the same way by merely omitting the `await` keyword.
+PyBankID provides both a synchronous and an asynchronous client for communication with BankID services. The example below will use the synchronous client, but the asynchronous client is used in an identical fashion, only using the `await` keyword before each function call.
 
 ### Synchronous client
 
 ```python
 from bankid import BankIDClient
 client = BankIDClient(certificates=(
-    'path/to/certificate.pem', 
-    'path/to/key.pem', 
+    'path/to/certificate.pem',
+    'path/to/key.pem',
 ))
 ```
 
 Connection to the production server is the default in the client. If a test server is desired, send in the `test_server=True` keyword in the init of the client.
 
-When using the JSON client, authentication and signing calls require the end user's IP address to be included in all calls. An authentication order is initiated as such:
+All authentication and signing calls require the end user's IP address to be included. An authentication order is initiated as such:
 
 ```python
 client.authenticate(end_user_ip='194.168.2.25')
 {
     'orderRef': 'ee3421ea-2096-4000-8130-82648efe0927',
     'autoStartToken': 'e8df5c3c-c67b-4a01-bfe5-fefeab760beb',
     'qrStartToken': '01f94e28-857f-4d8a-bf8e-6c5a24466658',
@@ -75,15 +74,15 @@
     'orderRef': 'ee3421ea-2096-4000-8130-82648efe0927',
     'autoStartToken': 'e8df5c3c-c67b-4a01-bfe5-fefeab760beb',
     'qrStartToken': '01f94e28-857f-4d8a-bf8e-6c5a24466658',
     'qrStartSecret': 'b4214886-3b5b-46ab-bc08-6862fddc0e06'
 }
 ```
 
-If someone else than the one you specified tries to authenticate or sign, the BankID app will state that the request is not intended for the user.
+If someone other than the one you specified tries to authenticate or sign, the BankID app will state that the request is not intended for the user.
 
 The status of an order can then be studied by polling with the `collect` method using the received `orderRef`:
 
 ```python
 client.collect(order_ref="a9b791c3-459f-492b-bf61-23027876140b")
 {
     'hintCode': 'outstandingTransaction',
@@ -122,43 +121,47 @@
         }
     },
     'orderRef': 'a9b791c3-459f-492b-bf61-23027876140b',
     'status': 'complete'
 }
 ```
 
+Please note that the `collect` method should be used sparingly: in the [BankID Integration Guide](https://www.bankid.com/en/utvecklare/guider/teknisk-integrationsguide) it is specified that _"collect should be called every two seconds and must not be called more frequent than once per second"_.
 
-Please note that the `collect` method should be used sparingly: in the [BankID Integration Guide](https://www.bankid.com/en/utvecklare/guider/teknisk-integrationsguide) it is specified that *"collect should be called every two seconds and must not be called more frequent than once per second"*.
+PyBankID also implements the `phone/auth` and `phone/sign` methods, for performing authentication and signing with
+users that are contacted through phone. For documentation on this, see [PyBankID's Read the Docs page](https://pybankid.readthedocs.io/en/latest/).
 
 ### Asynchronous client
 
-The asynchronous client is used in the same way as the synchronous client, but the methods are blocking.
+The asynchronous client is used in the same way as the synchronous client, with the difference that all request are performed asynchronously.
 
 The synchronous guide above can be used as a reference for the asynchronous client as well, by simply adding the `await` keyword:
 
 ```python
-from bankid import BankIDClientAsync
-client = BankIDClientAsync(certificates=(
-    'path/to/certificate.pem', 
-    'path/to/key.pem', 
+from bankid import BankIDAsyncClient
+client = BankIDAsyncClient(certificates=(
+    'path/to/certificate.pem',
+    'path/to/key.pem',
 ))
 
 await client.authenticate(end_user_ip='194.168.2.25')
 {
     'orderRef': 'ee3421ea-2096-4000-8130-82648efe0927',
     'autoStartToken': 'e8df5c3c-c67b-4a01-bfe5-fefeab760beb',
     'qrStartToken': '01f94e28-857f-4d8a-bf8e-6c5a24466658',
     'qrStartSecret': 'b4214886-3b5b-46ab-bc08-6862fddc0e06'
 }
 ```
 
-
 ## PyBankID and QR codes
 
-PyBankID can generate QR codes for you, and there is an example application in the [examples folder of the repo](https://github.com/hbldh/pybankid/tree/master/examples) where a Flask application called `qrdemo` shows one way to do authentication with animated QR codes.
+PyBankID can generate QR codes for you, and there is an example application in the [examples folder of the repo](https://github.com/hbldh/pybankid/tree/master/examples), where a Flask application called `qrdemo` shows one way to do authentication with animated QR codes.
+
+The QR code content generation is done with the `generate_qr_code_content` method on the BankID Client instances, or directly
+through the identically named method in `bankid.qr` module.
 
 ## Certificates
 
 ### Production certificates
 
 If you want to use BankID in a production environment, then you will have to purchase this service from one of the [selling banks](https://www.bankid.com/foretag/anslut-foeretag). They will then provide you with a certificate that can be used to authenticate your company/application with the BankID servers.
 
@@ -175,15 +178,7 @@
 cert_and_key = bankid.create_bankid_test_server_cert_and_key(
     dir_to_save_cert_and_key_in)
 print(cert_and_key)
 ['/home/hbldh/certificate.pem', '/home/hbldh/key.pem']
 client = bankid.BankIDClient(
     certificates=cert_and_key, test_server=True)
 ```
-
-## Testing
-
-The PyBankID solution can be tested with [pytest](https://pytest.org/):
-
-```bash
-pytest tests/
-```
```

### Comparing `pybankid-1.0.1/bankid/__init__.py` & `pybankid-1.1.0/bankid/__init__.py`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.1/bankid/asyncclient.py` & `pybankid-1.1.0/bankid/syncclient.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,41 @@
-from typing import Optional, Tuple, Dict, Any
+from typing import Any, Dict, Tuple, Union
 
 import httpx
 
 from bankid.baseclient import BankIDClientBaseclass
 from bankid.exceptions import get_json_error_class
 
 
-class BankIDAsyncClient(BankIDClientBaseclass):
-    """The asynchronous client to use for communicating with BankID servers via the v6 API.
+class BankIDClient(BankIDClientBaseclass[httpx.Client]):
+    """The synchronous client to use for communicating with BankID servers via the v6 API.
 
     :param certificates: Tuple of string paths to the certificate to use and
         the key to sign with.
     :type certificates: tuple
     :param test_server: Use the test server for authenticating and signing.
     :type test_server: bool
     :param request_timeout: Timeout for BankID requests.
     :type request_timeout: int
 
     """
 
-    def __init__(self, certificates: Tuple[str, str], test_server: bool = False, request_timeout: Optional[int] = None):
+    def __init__(self, certificates: Tuple[str, str], test_server: bool = False, request_timeout: int = 5):
         super().__init__(certificates, test_server, request_timeout)
 
-        kwargs = {
-            "cert": self.certs,
-            "headers": {"Content-Type": "application/json"},
-            "verify": self.verify_cert,
-        }
-        if request_timeout:
-            kwargs["timeout"] = request_timeout
-        self.client = httpx.AsyncClient(**kwargs)
+        headers= {"Content-Type": "application/json"}
+        self.client = httpx.Client(cert=self.certs, headers=headers, verify=str(self.verify_cert), timeout=request_timeout)
 
-    async def authenticate(
+    def authenticate(
         self,
         end_user_ip: str,
-        requirement: Dict[str, Any] = None,
-        user_visible_data: str = None,
-        user_non_visible_data: str = None,
-        user_visible_data_format: str = None,
+        requirement: Union[Dict[str, Any], None] = None,
+        user_visible_data: Union[str, None] = None,
+        user_non_visible_data: Union[str, None] = None,
+        user_visible_data_format: Union[str, None] = None,
     ) -> Dict[str, str]:
         """Request an authentication order. The :py:meth:`collect` method
         is used to query the status of the order.
 
         Example data returned:
 
         .. code-block:: json
@@ -78,29 +72,29 @@
             end_user_ip,
             requirement=requirement,
             user_visible_data=user_visible_data,
             user_non_visible_data=user_non_visible_data,
             user_visible_data_format=user_visible_data_format,
         )
 
-        response = await self.client.post(self._auth_endpoint, json=data)
+        response = self.client.post(self._auth_endpoint, json=data)
 
         if response.status_code == 200:
-            return response.json()
+            return response.json()  # type: ignore[no-any-return]
         else:
             raise get_json_error_class(response)
 
-    async def phone_authenticate(
+    def phone_authenticate(
         self,
         personal_number: str,
         call_initiator: str,
-        requirement: Dict[str, Any] = None,
-        user_visible_data: str = None,
-        user_non_visible_data: str = None,
-        user_visible_data_format: str = None,
+        requirement: Union[Dict[str, Any], None] = None,
+        user_visible_data: Union[str, None] = None,
+        user_non_visible_data: Union[str, None] = None,
+        user_visible_data_format: Union[str, None] = None,
     ) -> Dict[str, str]:
         """Initiates an authentication order when the user is talking
         to the RP over the phone. The :py:meth:`collect` method
         is used to query the status of the order.
 
         Example data returned:
 
@@ -143,28 +137,28 @@
             user_visible_data=user_visible_data,
             user_non_visible_data=user_non_visible_data,
             user_visible_data_format=user_visible_data_format,
         )
         data["personalNumber"] = personal_number
         data["callInitiator"] = call_initiator
 
-        response = await self.client.post(self._phone_auth_endpoint, json=data)
+        response = self.client.post(self._phone_auth_endpoint, json=data)
 
         if response.status_code == 200:
-            return response.json()
+            return response.json()  # type: ignore[no-any-return]
         else:
             raise get_json_error_class(response)
 
-    async def sign(
+    def sign(
         self,
-        end_user_ip,
+        end_user_ip: str,
         user_visible_data: str,
-        requirement: Dict[str, Any] = None,
-        user_non_visible_data: str = None,
-        user_visible_data_format: str = None,
+        requirement: Union[Dict[str, Any], None] = None,
+        user_non_visible_data: Union[str, None] = None,
+        user_visible_data_format: Union[str, None] = None,
     ) -> Dict[str, str]:
         """Request a signing order. The :py:meth:`collect` method
         is used to query the status of the order.
 
         Example data returned:
 
         .. code-block:: json
@@ -198,33 +192,32 @@
         data = self._create_payload(
             end_user_ip,
             requirement=requirement,
             user_visible_data=user_visible_data,
             user_non_visible_data=user_non_visible_data,
             user_visible_data_format=user_visible_data_format,
         )
-
-        response = await self.client.post(self._sign_endpoint, json=data)
+        response = self.client.post(self._sign_endpoint, json=data)
 
         if response.status_code == 200:
-            return response.json()
+            return response.json()  # type: ignore[no-any-return]
         else:
             raise get_json_error_class(response)
 
-    async def phone_sign(
+    def phone_sign(
         self,
         personal_number: str,
         call_initiator: str,
         user_visible_data: str,
-        requirement: Dict[str, Any] = None,
-        user_non_visible_data: str = None,
-        user_visible_data_format: str = None,
+        requirement: Union[Dict[str, Any], None] = None,
+        user_non_visible_data: Union[str, None] = None,
+        user_visible_data_format: Union[str, None] = None,
     ) -> Dict[str, str]:
         """Initiates an authentication order when the user is talking to
-        the RP over the phone. The :py:meth:`collect` method
+        the RP over the phone.  The :py:meth:`collect` method
         is used to query the status of the order.
 
         Example data returned:
 
         .. code-block:: json
 
             {
@@ -262,22 +255,22 @@
             user_visible_data=user_visible_data,
             user_non_visible_data=user_non_visible_data,
             user_visible_data_format=user_visible_data_format,
         )
         data["personalNumber"] = personal_number
         data["callInitiator"] = call_initiator
 
-        response = await self.client.post(self._phone_sign_endpoint, json=data)
+        response = self.client.post(self._phone_sign_endpoint, json=data)
 
         if response.status_code == 200:
-            return response.json()
+            return response.json()  # type: ignore[no-any-return]
         else:
             raise get_json_error_class(response)
 
-    async def collect(self, order_ref: str) -> dict:
+    def collect(self, order_ref: str) -> dict:
         """Collects the result of a sign or auth order using the
         ``orderRef`` as reference.
 
         RP should keep on calling collect every two seconds if status is pending.
         RP must abort if status indicates failed. The user identity is returned
         when complete.
 
@@ -334,34 +327,34 @@
         :type order_ref: str
         :return: The CollectResponse parsed to a dictionary.
         :rtype: dict
         :raises BankIDError: raises a subclass of this error
                              when error has been returned from server.
 
         """
-        response = await self.client.post(self._collect_endpoint, json={"orderRef": order_ref})
+        response = self.client.post(self._collect_endpoint, json={"orderRef": order_ref})
 
         if response.status_code == 200:
-            return response.json()
+            return response.json()  # type: ignore[no-any-return]
         else:
             raise get_json_error_class(response)
 
-    async def cancel(self, order_ref: str) -> bool:
+    def cancel(self, order_ref: str) -> bool:
         """Cancels an ongoing sign or auth order.
 
         This is typically used if the user cancels the order
         in your service or app.
 
         :param order_ref: The UUID string specifying which order to cancel.
         :type order_ref: str
         :return: Boolean regarding success of cancellation.
         :rtype: bool
         :raises BankIDError: raises a subclass of this error
                              when error has been returned from server.
 
         """
-        response = await self.client.post(self._cancel_endpoint, json={"orderRef": order_ref})
+        response = self.client.post(self._cancel_endpoint, json={"orderRef": order_ref})
 
         if response.status_code == 200:
-            return response.json() == {}
+            return response.json() == {}  # type: ignore[no-any-return]
         else:
             raise get_json_error_class(response)
```

### Comparing `pybankid-1.0.1/bankid/baseclient.py` & `pybankid-1.1.0/bankid/baseclient.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 import base64
 from datetime import datetime
-from typing import Tuple, Optional, Dict, Any
+from typing import Tuple, Dict, Any, Union, TypeVar, Generic
 from urllib.parse import urljoin
 
 from bankid.qr import generate_qr_code_content
 from bankid.certutils import resolve_cert_path
 
+import httpx
 
-class BankIDClientBaseclass:
+TClient = TypeVar("TClient", httpx.AsyncClient, httpx.Client)
+
+
+class BankIDClientBaseclass(Generic[TClient]):
     """Baseclass for BankID clients.
 
     Both the synchronous and asynchronous clients inherit from this base class and has the methods implemented here.
     """
 
+    client: TClient
+
     def __init__(
         self,
         certificates: Tuple[str, str],
         test_server: bool = False,
-        request_timeout: Optional[int] = None,
+        request_timeout: int = 5,
     ):
         self.certs = certificates
-        self._request_timeout = request_timeout
 
         if test_server:
             self.api_url = "https://appapi2.test.bankid.com/rp/v6.0/"
             self.verify_cert = resolve_cert_path("appapi2.test.bankid.com.pem")
         else:
             self.api_url = "https://appapi2.bankid.com/rp/v6.0/"
             self.verify_cert = resolve_cert_path("appapi2.bankid.com.pem")
@@ -32,36 +37,31 @@
         self._auth_endpoint = urljoin(self.api_url, "auth")
         self._phone_auth_endpoint = urljoin(self.api_url, "phone/auth")
         self._sign_endpoint = urljoin(self.api_url, "sign")
         self._phone_sign_endpoint = urljoin(self.api_url, "phone/sign")
         self._collect_endpoint = urljoin(self.api_url, "collect")
         self._cancel_endpoint = urljoin(self.api_url, "cancel")
 
-        self.client = None
-
     @staticmethod
-    def generate_qr_code_content(qr_start_token: str, start_t: [float, datetime], qr_start_secret: str) -> str:
+    def generate_qr_code_content(qr_start_token: str, start_t: Union[float, datetime], qr_start_secret: str) -> str:
         return generate_qr_code_content(qr_start_token, start_t, qr_start_secret)
 
     @staticmethod
-    def _encode_user_data(user_data):
-        if isinstance(user_data, str):
-            return base64.b64encode(user_data.encode("utf-8")).decode("ascii")
-        else:
-            return base64.b64encode(user_data).decode("ascii")
+    def _encode_user_data(user_data: str) -> str:
+        return base64.b64encode(user_data.encode("utf-8")).decode("ascii")
 
     def _create_payload(
         self,
-        end_user_ip: str = None,
-        requirement: Dict[str, Any] = None,
-        user_visible_data: str = None,
-        user_non_visible_data: str = None,
-        user_visible_data_format: str = None,
-    ):
-        data = {}
+        end_user_ip: Union[str, None] = None,
+        requirement: Union[Dict[str, Any], None] = None,
+        user_visible_data: Union[str, None] = None,
+        user_non_visible_data: Union[str, None] = None,
+        user_visible_data_format: Union[str, None] = None,
+    ) -> Dict[str, str]:
+        data: Dict[str, Any] = {}
         if end_user_ip:
             data["endUserIp"] = end_user_ip
         if requirement and isinstance(requirement, dict):
             data["requirement"] = requirement
         if user_visible_data:
             data["userVisibleData"] = self._encode_user_data(user_visible_data)
         if user_non_visible_data:
```

### Comparing `pybankid-1.0.1/bankid/certs/FPTestcert4_20220818.p12` & `pybankid-1.1.0/bankid/certs/FPTestcert4_20220818.p12`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.1/bankid/certs/FPTestcert4_20220818_cert.pem` & `pybankid-1.1.0/bankid/certs/FPTestcert4_20220818_cert.pem`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.1/bankid/certs/FPTestcert4_20220818_key.pem` & `pybankid-1.1.0/bankid/certs/FPTestcert4_20220818_key.pem`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.1/bankid/certs/FPTestcert4_20230629.p12` & `pybankid-1.1.0/bankid/certs/FPTestcert4_20230629.p12`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.1/bankid/certs/FPTestcert4_20230629_cert.pem` & `pybankid-1.1.0/bankid/certs/FPTestcert4_20230629_cert.pem`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.1/bankid/certs/FPTestcert4_20230629_key.pem` & `pybankid-1.1.0/bankid/certs/FPTestcert4_20230629_key.pem`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.1/bankid/certs/appapi.bankid.com.pem` & `pybankid-1.1.0/bankid/certs/appapi.bankid.com.pem`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.1/bankid/certs/appapi.test.bankid.com.pem` & `pybankid-1.1.0/bankid/certs/appapi.test.bankid.com.pem`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.1/bankid/certs/appapi2.bankid.com.pem` & `pybankid-1.1.0/bankid/certs/appapi2.bankid.com.pem`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.1/bankid/certs/appapi2.test.bankid.com.pem` & `pybankid-1.1.0/bankid/certs/appapi2.test.bankid.com.pem`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.1/bankid/certutils.py` & `pybankid-1.1.0/bankid/certutils.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,57 +3,58 @@
 :mod:`bankid.certutils` -- Certificate Utilities
 ================================================
 .. moduleauthor:: hbldh <henrik.blidh@nedomkull.com>
 """
 
 import os
 import subprocess
-from typing import Tuple
+from typing import Tuple, Union
 
-import importlib_resources
+import pathlib
+import importlib.resources
 
 from bankid.certs import get_test_cert_p12
 from bankid.exceptions import BankIDError
 
 _TEST_CERT_PASSWORD = "qwerty123"
 
 
-def resolve_cert_path(file: str) -> str:
-    ref = importlib_resources.files("bankid.certs") / file
-    with importlib_resources.as_file(ref) as path:
-        return str(path)
+def resolve_cert_path(file: str) -> pathlib.Path:
+    path = importlib.resources.files("bankid.certs").joinpath(file)
+    assert isinstance(path, pathlib.Path)
+    return path
 
 
-def create_bankid_test_server_cert_and_key(destination_path: str) -> Tuple[str]:
+def create_bankid_test_server_cert_and_key(destination_path: str = ".") -> Tuple[str, str]:
     """Split the bundled test certificate into certificate and key parts and save them
     as separate files, stored in PEM format.
 
     If the environment variable TEST_CERT_FILE is set, use this file
     instead of fetching the P12 certificate.
 
-    :param destination_path: The directory to save certificate and key files to.
+    :param destination_path: The directory to save certificate and key files to. Default is the current directory.
     :type destination_path: str
     :returns: The path tuple ``(cert_path, key_path)``.
     :rtype: tuple
 
     """
-    if os.getenv("TEST_CERT_FILE"):
+    if test_cert_file := os.getenv("TEST_CERT_FILE"):
         certificate, key = split_certificate(
-            os.getenv("TEST_CERT_FILE"), destination_path, password=_TEST_CERT_PASSWORD
+            test_cert_file, destination_path, password=_TEST_CERT_PASSWORD
         )
 
     else:
         # Fetch testP12 certificate path
         certificate, key = split_certificate(str(get_test_cert_p12()), destination_path, password=_TEST_CERT_PASSWORD)
 
     # Return path tuples.
     return certificate, key
 
 
-def split_certificate(certificate_path, destination_folder, password=None):
+def split_certificate(certificate_path: str, destination_folder: str, password: Union[str, None] = None) -> Tuple[str, str]:
     """Splits a PKCS12 certificate into Base64-encoded DER certificate and key.
 
     This method splits a potentially password-protected
     `PKCS12 <https://en.wikipedia.org/wiki/PKCS_12>`_ certificate
     (format ``.p12`` or ``.pfx``) into one certificate and one key part, both in
     `pem <https://en.wikipedia.org/wiki/X.509#Certificate_filename_extensions>`_
     format.
@@ -61,27 +62,27 @@
     :returns: Tuple of certificate and key string data.
     :rtype: tuple
 
     """
     try:
         # Attempt Linux and Darwin call first.
         p = subprocess.Popen(["openssl", "version"], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-        sout, serr = p.communicate()
+        sout, _ = p.communicate()
         openssl_executable_version = sout.decode().lower()
         if not (openssl_executable_version.startswith("openssl") or openssl_executable_version.startswith("libressl")):
             raise BankIDError("OpenSSL executable could not be found. " "Splitting cannot be performed.")
         openssl_executable = "openssl"
     except Exception:
         # Attempt to call on standard Git for Windows path.
         p = subprocess.Popen(
             ["C:\\Program Files\\Git\\mingw64\\bin\\openssl.exe", "version"],
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
         )
-        sout, serr = p.communicate()
+        sout, _ = p.communicate()
         if not sout.decode().lower().startswith("openssl"):
             raise BankIDError("OpenSSL executable could not be found. " "Splitting cannot be performed.")
         openssl_executable = "C:\\Program Files\\Git\\mingw64\\bin\\openssl.exe"
 
     if not os.path.exists(os.path.abspath(os.path.expanduser(destination_folder))):
         os.makedirs(os.path.abspath(os.path.expanduser(destination_folder)))
 
@@ -126,15 +127,15 @@
     if p.returncode:
         raise BankIDError("Error converting certificate: {0}".format(err.decode("utf-8")))
 
     # Return path tuples.
     return out_cert_path, out_key_path
 
 
-def main(verbose=True):
+def main(verbose: bool = True) -> Tuple[str, str]:
     paths = create_bankid_test_server_cert_and_key(os.path.expanduser("~"))
     if verbose:
         print("Saved certificate as {0}".format(paths[0]))
         print("Saved key as {0}".format(paths[1]))
     return paths
```

### Comparing `pybankid-1.0.1/bankid/exceptions.py` & `pybankid-1.1.0/bankid/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-# -*- coding: utf-8 -*-
+from __future__ import annotations
+import httpx
+from typing import Any, Dict, Union
 
 
-def get_json_error_class(response):
+def get_json_error_class(response: httpx.Response) -> BankIDError:
     data = response.json()
     error_class = _JSON_ERROR_CODE_TO_CLASS.get(data.get("errorCode"), BankIDError)
     return error_class("{0}: {1}".format(data.get("errorCode"), data.get("details")), raw_data=data)
 
 
 class BankIDError(Exception):
     """Parent exception class for all PyBankID errors."""
 
-    def __init__(self, *args, **kwargs):
-        super(BankIDError, self).__init__(*args)
-        self.rfa = None
-        self.json = kwargs.get("raw_data", {})
+    def __init__(self, *args: Any, raw_data: Union[Dict[str, Any], None] = None, **kwargs: Any) -> None:
+        super(BankIDError, self).__init__(*args, **kwargs)
+        self.rfa: Union[int, None] = None
+        self.json = raw_data or {}
 
 
 class BankIDWarning(Warning):
     """Warning class for PyBankID."""
 
     pass
 
@@ -31,15 +33,15 @@
 
     **Action by RP:** RP must not try the same request again.
     This is an internal error within RP's system and must not be '
     communicated to the user as a BankID error.
 
     """
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
 
 
 class AlreadyInProgressError(BankIDError):
     """Failure to create new order due to one already in progress.
 
     **Code:** ``alreadyInProgress``
@@ -49,15 +51,15 @@
 
     **Action by RP:** RP must inform the user that a login or signing
     operation is already initiated for this user.
     Message RFA4 should be used.
 
     """
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
         self.rfa = 4
 
 
 class InternalError(BankIDError):
     """Remote server error.
 
@@ -67,15 +69,15 @@
 
     **Action by RP:** RP must not automatically try again. RP must
     inform the user that a technical error has
     occurred. Message RFA5 should be used.
 
     """
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
         self.rfa = 5
 
 
 class MaintenanceError(BankIDError):
     """The service is temporarily out of service.
 
@@ -83,15 +85,15 @@
 
     **Action by RP:** RP may try again without informing the user.
     If this error is returned repeatedly, RP must inform the user.
     Message RFA5.
 
     """
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
         self.rfa = 5
 
 
 class UnauthorizedError(BankIDError):
     """RP does not have access to the service.
 
@@ -99,50 +101,50 @@
 
     **Action by RP:** RP must not try the same request again.
     This is an internal error within RP's system and must not be '
     communicated to the user as a BankID error.
 
     """
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
 
 
 class NotFoundError(BankIDError):
     """An erroneous URL path was used.
 
     **Code:** ``notFound``
 
     **Action by RP:** RP must not try the same request again.
     This is an internal error within RP's system and must not be '
     communicated to the user as a BankID error.
 
     """
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
 
 
 class RequestTimeoutError(BankIDError):
     """It took too long time to transmit the request.
 
     **Code:** ``requestTimeout``
 
     **Action by RP:** RP must not automatically try again.
     This error may occur if the processing at RP or the communication is too
     slow. RP must inform the user. Message RFA5
 
     """
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
         self.rfa = 5
 
 
-_JSON_ERROR_CODE_TO_CLASS = {
+_JSON_ERROR_CODE_TO_CLASS: Dict[str, type[BankIDError]] = {
     "invalidParameters": InvalidParametersError,
     "alreadyInProgress": AlreadyInProgressError,
     "unauthorized": UnauthorizedError,
     "notFound": NotFoundError,
     # 'methodNotAllowed': ,  # This will not be handled here...
     "requestTimeout": RequestTimeoutError,
     # 'unsupportedMediaType': ,  # This will not be handled here...
```

### Comparing `pybankid-1.0.1/bankid/experimental/helper.py` & `pybankid-1.1.0/bankid/experimental/helper.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,18 +22,14 @@
 
 class BankIdSignatureContainer:
     def __init__(self, signature):
         self.root = ET.fromstring(signature.decode)
         self.raw = signature
 
     @property
-    def signature_value(self):
-        return B64Value(self.root[1].text).decode
-
-    @property
     def signed_data_digest(self):
         return self.root[0][2][2]
 
     @property
     def key_data_digest(self):
         return self.root[0][3][2]
```

### Comparing `pybankid-1.0.1/bankid/experimental/verify.py` & `pybankid-1.1.0/bankid/experimental/verify.py`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.1/bankid/qr.py` & `pybankid-1.1.0/bankid/qr.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+from typing import Union
+
 import hashlib
 import hmac
 import time
 from datetime import datetime
 from math import floor
 
 
-def generate_qr_code_content(qr_start_token: str, start_t: [float, datetime], qr_start_secret: str) -> str:
+def generate_qr_code_content(qr_start_token: str, start_t: Union[float, datetime], qr_start_secret: str) -> str:
     """Given QR start token, time.time() or UTC datetime when initiated authentication call was made and the
     QR start secret, calculate the current QR code content to display.
     """
     if isinstance(start_t, datetime):
         start_t = start_t.timestamp()
     elapsed_seconds_since_call = int(floor(time.time() - start_t))
     qr_auth_code = hmac.new(
```

### Comparing `pybankid-1.0.1/bankid/syncclient.py` & `pybankid-1.1.0/bankid/asyncclient.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,41 @@
-from typing import Optional, Tuple, Dict, Any
+from typing import Any, Dict, Tuple, Union
 
 import httpx
 
 from bankid.baseclient import BankIDClientBaseclass
 from bankid.exceptions import get_json_error_class
 
 
-class BankIDClient(BankIDClientBaseclass):
-    """The synchronous client to use for communicating with BankID servers via the v6 API.
+class BankIDAsyncClient(BankIDClientBaseclass[httpx.AsyncClient]):
+    """The asynchronous client to use for communicating with BankID servers via the v6 API.
 
     :param certificates: Tuple of string paths to the certificate to use and
         the key to sign with.
     :type certificates: tuple
     :param test_server: Use the test server for authenticating and signing.
     :type test_server: bool
     :param request_timeout: Timeout for BankID requests.
     :type request_timeout: int
 
     """
 
-    def __init__(self, certificates: Tuple[str, str], test_server: bool = False, request_timeout: Optional[int] = None):
+    def __init__(self, certificates: Tuple[str, str], test_server: bool = False, request_timeout: int = 5):
         super().__init__(certificates, test_server, request_timeout)
 
-        kwargs = {
-            "cert": self.certs,
-            "headers": {"Content-Type": "application/json"},
-            "verify": self.verify_cert,
-        }
-        if request_timeout:
-            kwargs["timeout"] = request_timeout
-        self.client = httpx.Client(**kwargs)
+        headers = {"Content-Type": "application/json"}
+        self.client = httpx.AsyncClient(cert=self.certs, headers=headers, verify=str(self.verify_cert), timeout=request_timeout)
 
-    def authenticate(
+    async def authenticate(
         self,
         end_user_ip: str,
-        requirement: Dict[str, Any] = None,
-        user_visible_data: str = None,
-        user_non_visible_data: str = None,
-        user_visible_data_format: str = None,
+        requirement: Union[Dict[str, Any], None] = None,
+        user_visible_data: Union[str, None]  = None,
+        user_non_visible_data: Union[str, None]  = None,
+        user_visible_data_format: Union[str, None]  = None,
     ) -> Dict[str, str]:
         """Request an authentication order. The :py:meth:`collect` method
         is used to query the status of the order.
 
         Example data returned:
 
         .. code-block:: json
@@ -78,29 +72,29 @@
             end_user_ip,
             requirement=requirement,
             user_visible_data=user_visible_data,
             user_non_visible_data=user_non_visible_data,
             user_visible_data_format=user_visible_data_format,
         )
 
-        response = self.client.post(self._auth_endpoint, json=data)
+        response = await self.client.post(self._auth_endpoint, json=data)
 
         if response.status_code == 200:
-            return response.json()
+            return response.json()  # type: ignore[no-any-return]
         else:
             raise get_json_error_class(response)
 
-    def phone_authenticate(
+    async def phone_authenticate(
         self,
         personal_number: str,
         call_initiator: str,
-        requirement: Dict[str, Any] = None,
-        user_visible_data: str = None,
-        user_non_visible_data: str = None,
-        user_visible_data_format: str = None,
+        requirement: Union[Dict[str, Any], None] = None,
+        user_visible_data: Union[str, None] = None,
+        user_non_visible_data: Union[str, None] = None,
+        user_visible_data_format: Union[str, None] = None,
     ) -> Dict[str, str]:
         """Initiates an authentication order when the user is talking
         to the RP over the phone. The :py:meth:`collect` method
         is used to query the status of the order.
 
         Example data returned:
 
@@ -143,28 +137,28 @@
             user_visible_data=user_visible_data,
             user_non_visible_data=user_non_visible_data,
             user_visible_data_format=user_visible_data_format,
         )
         data["personalNumber"] = personal_number
         data["callInitiator"] = call_initiator
 
-        response = self.client.post(self._phone_auth_endpoint, json=data)
+        response = await self.client.post(self._phone_auth_endpoint, json=data)
 
         if response.status_code == 200:
-            return response.json()
+            return response.json()  # type: ignore[no-any-return]
         else:
             raise get_json_error_class(response)
 
-    def sign(
+    async def sign(
         self,
         end_user_ip: str,
         user_visible_data: str,
-        requirement: Dict[str, Any] = None,
-        user_non_visible_data: str = None,
-        user_visible_data_format: str = None,
+        requirement: Union[Dict[str, Any], None] = None,
+        user_non_visible_data: Union[str, None] = None,
+        user_visible_data_format: Union[str, None] = None,
     ) -> Dict[str, str]:
         """Request a signing order. The :py:meth:`collect` method
         is used to query the status of the order.
 
         Example data returned:
 
         .. code-block:: json
@@ -198,32 +192,33 @@
         data = self._create_payload(
             end_user_ip,
             requirement=requirement,
             user_visible_data=user_visible_data,
             user_non_visible_data=user_non_visible_data,
             user_visible_data_format=user_visible_data_format,
         )
-        response = self.client.post(self._sign_endpoint, json=data)
+
+        response = await self.client.post(self._sign_endpoint, json=data)
 
         if response.status_code == 200:
-            return response.json()
+            return response.json()  # type: ignore[no-any-return]
         else:
             raise get_json_error_class(response)
 
-    def phone_sign(
+    async def phone_sign(
         self,
         personal_number: str,
         call_initiator: str,
         user_visible_data: str,
-        requirement: Dict[str, Any] = None,
-        user_non_visible_data: str = None,
-        user_visible_data_format: str = None,
+        requirement: Union[Dict[str, Any], None] = None,
+        user_non_visible_data: Union[str, None] = None,
+        user_visible_data_format: Union[str, None] = None,
     ) -> Dict[str, str]:
         """Initiates an authentication order when the user is talking to
-        the RP over the phone.  The :py:meth:`collect` method
+        the RP over the phone. The :py:meth:`collect` method
         is used to query the status of the order.
 
         Example data returned:
 
         .. code-block:: json
 
             {
@@ -261,22 +256,22 @@
             user_visible_data=user_visible_data,
             user_non_visible_data=user_non_visible_data,
             user_visible_data_format=user_visible_data_format,
         )
         data["personalNumber"] = personal_number
         data["callInitiator"] = call_initiator
 
-        response = self.client.post(self._phone_sign_endpoint, json=data)
+        response = await self.client.post(self._phone_sign_endpoint, json=data)
 
         if response.status_code == 200:
-            return response.json()
+            return response.json()  # type: ignore[no-any-return]
         else:
             raise get_json_error_class(response)
 
-    def collect(self, order_ref: str) -> dict:
+    async def collect(self, order_ref: str) -> dict:
         """Collects the result of a sign or auth order using the
         ``orderRef`` as reference.
 
         RP should keep on calling collect every two seconds if status is pending.
         RP must abort if status indicates failed. The user identity is returned
         when complete.
 
@@ -333,34 +328,34 @@
         :type order_ref: str
         :return: The CollectResponse parsed to a dictionary.
         :rtype: dict
         :raises BankIDError: raises a subclass of this error
                              when error has been returned from server.
 
         """
-        response = self.client.post(self._collect_endpoint, json={"orderRef": order_ref})
+        response = await self.client.post(self._collect_endpoint, json={"orderRef": order_ref})
 
         if response.status_code == 200:
-            return response.json()
+            return response.json()  # type: ignore[no-any-return]
         else:
             raise get_json_error_class(response)
 
-    def cancel(self, order_ref: str) -> bool:
+    async def cancel(self, order_ref: str) -> bool:
         """Cancels an ongoing sign or auth order.
 
         This is typically used if the user cancels the order
         in your service or app.
 
         :param order_ref: The UUID string specifying which order to cancel.
         :type order_ref: str
         :return: Boolean regarding success of cancellation.
         :rtype: bool
         :raises BankIDError: raises a subclass of this error
                              when error has been returned from server.
 
         """
-        response = self.client.post(self._cancel_endpoint, json={"orderRef": order_ref})
+        response = await self.client.post(self._cancel_endpoint, json={"orderRef": order_ref})
 
         if response.status_code == 200:
-            return response.json() == {}
+            return response.json() == {}  # type: ignore[no-any-return]
         else:
             raise get_json_error_class(response)
```

### Comparing `pybankid-1.0.1/examples/qrdemo/.gitignore` & `pybankid-1.1.0/examples/qrdemo/.gitignore`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.1/examples/qrdemo/README.md` & `pybankid-1.1.0/examples/qrdemo/README.md`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.1/examples/qrdemo/qrdemo/app.py` & `pybankid-1.1.0/examples/qrdemo/qrdemo/app.py`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.1/examples/qrdemo/qrdemo/templates/auth_complete.html` & `pybankid-1.1.0/examples/qrdemo/qrdemo/templates/auth_complete.html`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.1/examples/qrdemo/qrdemo/templates/index.html` & `pybankid-1.1.0/examples/qrdemo/qrdemo/templates/index.html`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.1/examples/qrdemo/qrdemo/templates/qr.html` & `pybankid-1.1.0/examples/qrdemo/qrdemo/templates/qr.html`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.1/pybankid.egg-info/PKG-INFO` & `pybankid-1.1.0/pybankid.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybankid
-Version: 1.0.1
+Version: 1.1.0
 Summary: BankID Relying Party client for Python
 Home-page: https://github.com/hbldh/pybankid
 Author: Henrik Blidh
 Author-email: henrik.blidh@nedomkull.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -15,28 +15,26 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx
-Requires-Dist: importlib-resources>=5.12.0
 Provides-Extra: signature-verification
 Requires-Dist: pyOpenSSL; extra == "signature-verification"
-Requires-Dist: pytz; extra == "signature-verification"
 Requires-Dist: asn1crypto; extra == "signature-verification"
+Requires-Dist: pytz; extra == "signature-verification"
 
 
 # PyBankID
 
 ![Build and Test](https://github.com/hbldh/pybankid/workflows/Build%20and%20Test/badge.svg)
 ![Documentation Status](https://readthedocs.org/projects/pybankid/badge/?version=latest)
-![PyPI Version](http://img.shields.io/pypi/v/pybankid.svg)
-![PyPI License](http://img.shields.io/pypi/l/pybankid.svg)
-![Coverage](https://coveralls.io/repos/github/hbldh/pybankid/badge.svg?branch=master)
+![PyPI Version](https://img.shields.io/pypi/v/pybankid)
+![PyPI License](https://img.shields.io/pypi/l/pybankid)
 
 PyBankID is a client for providing BankID services as a Relying Party, i.e., providing authentication and signing functionality to end users. This package provides a simplifying interface for initiating authentication and signing orders and then collecting the results from the BankID servers.
 
 The only supported BankID API version supported by PyBankID from version 1.0.0 is v6.0, which means that the Secure Start solution is the only supported way of providing BankID services. PyBankID versions prior to 1.0.0 will not work after 1st of May 2024.
 
 If you intend to use PyBankID in your project, you are advised to read the [BankID Integration Guide](https://www.bankid.com/en/utvecklare/guider/teknisk-integrationsguide) before doing anything else. There, one can find information about how the BankID methods are defined and how to use them.
 
@@ -46,29 +44,29 @@
 
 ```bash
 pip install pybankid
 ```
 
 ## Usage
 
-PyBankID provides both a synchronous and an asynchronous client for communication with BankID services. The example below will use the asynchronous client, but the synchronous client is used in the same way by merely omitting the `await` keyword.
+PyBankID provides both a synchronous and an asynchronous client for communication with BankID services. The example below will use the synchronous client, but the asynchronous client is used in an identical fashion, only using the `await` keyword before each function call.
 
 ### Synchronous client
 
 ```python
 from bankid import BankIDClient
 client = BankIDClient(certificates=(
-    'path/to/certificate.pem', 
-    'path/to/key.pem', 
+    'path/to/certificate.pem',
+    'path/to/key.pem',
 ))
 ```
 
 Connection to the production server is the default in the client. If a test server is desired, send in the `test_server=True` keyword in the init of the client.
 
-When using the JSON client, authentication and signing calls require the end user's IP address to be included in all calls. An authentication order is initiated as such:
+All authentication and signing calls require the end user's IP address to be included. An authentication order is initiated as such:
 
 ```python
 client.authenticate(end_user_ip='194.168.2.25')
 {
     'orderRef': 'ee3421ea-2096-4000-8130-82648efe0927',
     'autoStartToken': 'e8df5c3c-c67b-4a01-bfe5-fefeab760beb',
     'qrStartToken': '01f94e28-857f-4d8a-bf8e-6c5a24466658',
@@ -103,15 +101,15 @@
     'orderRef': 'ee3421ea-2096-4000-8130-82648efe0927',
     'autoStartToken': 'e8df5c3c-c67b-4a01-bfe5-fefeab760beb',
     'qrStartToken': '01f94e28-857f-4d8a-bf8e-6c5a24466658',
     'qrStartSecret': 'b4214886-3b5b-46ab-bc08-6862fddc0e06'
 }
 ```
 
-If someone else than the one you specified tries to authenticate or sign, the BankID app will state that the request is not intended for the user.
+If someone other than the one you specified tries to authenticate or sign, the BankID app will state that the request is not intended for the user.
 
 The status of an order can then be studied by polling with the `collect` method using the received `orderRef`:
 
 ```python
 client.collect(order_ref="a9b791c3-459f-492b-bf61-23027876140b")
 {
     'hintCode': 'outstandingTransaction',
@@ -150,43 +148,47 @@
         }
     },
     'orderRef': 'a9b791c3-459f-492b-bf61-23027876140b',
     'status': 'complete'
 }
 ```
 
+Please note that the `collect` method should be used sparingly: in the [BankID Integration Guide](https://www.bankid.com/en/utvecklare/guider/teknisk-integrationsguide) it is specified that _"collect should be called every two seconds and must not be called more frequent than once per second"_.
 
-Please note that the `collect` method should be used sparingly: in the [BankID Integration Guide](https://www.bankid.com/en/utvecklare/guider/teknisk-integrationsguide) it is specified that *"collect should be called every two seconds and must not be called more frequent than once per second"*.
+PyBankID also implements the `phone/auth` and `phone/sign` methods, for performing authentication and signing with
+users that are contacted through phone. For documentation on this, see [PyBankID's Read the Docs page](https://pybankid.readthedocs.io/en/latest/).
 
 ### Asynchronous client
 
-The asynchronous client is used in the same way as the synchronous client, but the methods are blocking.
+The asynchronous client is used in the same way as the synchronous client, with the difference that all request are performed asynchronously.
 
 The synchronous guide above can be used as a reference for the asynchronous client as well, by simply adding the `await` keyword:
 
 ```python
-from bankid import BankIDClientAsync
-client = BankIDClientAsync(certificates=(
-    'path/to/certificate.pem', 
-    'path/to/key.pem', 
+from bankid import BankIDAsyncClient
+client = BankIDAsyncClient(certificates=(
+    'path/to/certificate.pem',
+    'path/to/key.pem',
 ))
 
 await client.authenticate(end_user_ip='194.168.2.25')
 {
     'orderRef': 'ee3421ea-2096-4000-8130-82648efe0927',
     'autoStartToken': 'e8df5c3c-c67b-4a01-bfe5-fefeab760beb',
     'qrStartToken': '01f94e28-857f-4d8a-bf8e-6c5a24466658',
     'qrStartSecret': 'b4214886-3b5b-46ab-bc08-6862fddc0e06'
 }
 ```
 
-
 ## PyBankID and QR codes
 
-PyBankID can generate QR codes for you, and there is an example application in the [examples folder of the repo](https://github.com/hbldh/pybankid/tree/master/examples) where a Flask application called `qrdemo` shows one way to do authentication with animated QR codes.
+PyBankID can generate QR codes for you, and there is an example application in the [examples folder of the repo](https://github.com/hbldh/pybankid/tree/master/examples), where a Flask application called `qrdemo` shows one way to do authentication with animated QR codes.
+
+The QR code content generation is done with the `generate_qr_code_content` method on the BankID Client instances, or directly
+through the identically named method in `bankid.qr` module.
 
 ## Certificates
 
 ### Production certificates
 
 If you want to use BankID in a production environment, then you will have to purchase this service from one of the [selling banks](https://www.bankid.com/foretag/anslut-foeretag). They will then provide you with a certificate that can be used to authenticate your company/application with the BankID servers.
 
@@ -203,15 +205,7 @@
 cert_and_key = bankid.create_bankid_test_server_cert_and_key(
     dir_to_save_cert_and_key_in)
 print(cert_and_key)
 ['/home/hbldh/certificate.pem', '/home/hbldh/key.pem']
 client = bankid.BankIDClient(
     certificates=cert_and_key, test_server=True)
 ```
-
-## Testing
-
-The PyBankID solution can be tested with [pytest](https://pytest.org/):
-
-```bash
-pytest tests/
-```
```

### Comparing `pybankid-1.0.1/pybankid.egg-info/SOURCES.txt` & `pybankid-1.1.0/pybankid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.1/setup.py` & `pybankid-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.1/tests/conftest.py` & `pybankid-1.1.0/tests/conftest.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,60 +1,48 @@
 import random
-from typing import Awaitable
 
-import httpx
 import pytest
-import pytest_asyncio
+from typing import List, Tuple
 
 from bankid.certs import get_test_cert_and_key
 
 
-@pytest.fixture()
+@pytest.fixture(scope="session")
 def ip_address() -> str:
-    with httpx.Client() as client:
-        response = client.get("https://httpbin.org/ip")
-        return response.json()["origin"].split(",")[0]
-
-
-@pytest_asyncio.fixture()
-async def ip_address_async() -> str:
-    async with httpx.AsyncClient() as client:
-        response = await client.get("https://httpbin.org/ip")
-        return response.json()["origin"].split(",")[0]
+    return "127.0.0.1"
 
 
 @pytest.fixture()
-def cert_and_key():
+def cert_and_key() -> Tuple[str, str]:
     cert, key = get_test_cert_and_key()
     return str(cert), str(key)
 
 
 @pytest.fixture()
-def random_personal_number():
+def random_personal_number() -> str:
     """Simple random Swedish personal number generator."""
 
-    def _luhn_digit(id_):
+    def _luhn_digit(id_: str) -> int:
         """Calculate Luhn control digit for personal number.
 
         Code adapted from `Faker
         <https://github.com/joke2k/faker/blob/master/faker/providers/ssn
         /sv_SE/__init__.py>`_.
 
         :param id_: The partial number to calculate checksum of.
         :type id_: str
         :return: Integer digit in [0, 9].
         :rtype: int
 
         """
 
-        def digits_of(n):
+        def digits_of(n: int) -> List[int]:
             return [int(i) for i in str(n)]
 
-        id_ = int(id_) * 10
-        digits = digits_of(id_)
+        digits = digits_of(int(id_) * 10)
         checksum = sum(digits[-1::-2])
         for k in digits[-2::-2]:
             checksum += sum(digits_of(k * 2))
         checksum %= 10
 
         return checksum if checksum == 0 else 10 - checksum
```

### Comparing `pybankid-1.0.1/tests/test_asyncclient.py` & `pybankid-1.1.0/tests/test_asyncclient.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,127 +11,129 @@
 Created on 2023-12-15
 
 """
 
 import uuid
 
 import pytest
+from typing import Tuple
 
 from bankid import BankIDAsyncClient, exceptions
 
 
 @pytest.mark.asyncio
-async def test_authentication_and_collect(cert_and_key, ip_address_async):
+async def test_authentication_and_collect(cert_and_key: Tuple[str, str], ip_address: str) -> None:
     """Authenticate call and then collect with the returned orderRef UUID."""
     c = BankIDAsyncClient(certificates=cert_and_key, test_server=True)
-    assert "appapi2.test.bankid.com.pem" in c.verify_cert
-    out = await c.authenticate(ip_address_async)
+    assert "appapi2.test.bankid.com.pem" in str(c.verify_cert)
+    out = await c.authenticate(ip_address)
+
     assert isinstance(out, dict)
     # UUID.__init__ performs the UUID compliance assertion.
-    uuid.UUID(out.get("orderRef"), version=4)
-    collect_status = await c.collect(out.get("orderRef"))
+    order_ref = uuid.UUID(out["orderRef"], version=4)
+    collect_status = await c.collect(str(order_ref))
     assert collect_status.get("status") == "pending"
     assert collect_status.get("hintCode") in ("outstandingTransaction", "noClient")
 
 
 @pytest.mark.asyncio
-async def test_sign_and_collect(cert_and_key, ip_address_async):
+async def test_sign_and_collect(cert_and_key: Tuple[str, str], ip_address: str) -> None:
     """Sign call and then collect with the returned orderRef UUID."""
 
     c = BankIDAsyncClient(certificates=cert_and_key, test_server=True)
     out = await c.sign(
-        ip_address_async,
+        ip_address,
         user_visible_data="The data to be signed",
         user_non_visible_data="Non visible data",
     )
     assert isinstance(out, dict)
     # UUID.__init__ performs the UUID compliance assertion.
-    uuid.UUID(out.get("orderRef"), version=4)
-    collect_status = await c.collect(out.get("orderRef"))
+    order_ref = uuid.UUID(out["orderRef"], version=4)
+    collect_status = await c.collect(str(order_ref))
     assert collect_status.get("status") == "pending"
     assert collect_status.get("hintCode") in ("outstandingTransaction", "noClient")
 
 
 @pytest.mark.asyncio
-async def test_phone_sign_and_collect(cert_and_key, random_personal_number):
+async def test_phone_sign_and_collect(cert_and_key: Tuple[str, str], random_personal_number: str) -> None:
     """Phone sign call and then collect with the returned orderRef UUID."""
 
     c = BankIDAsyncClient(certificates=cert_and_key, test_server=True)
     out = await c.phone_sign(random_personal_number, "RP", user_visible_data="The data to be signed")
     assert isinstance(out, dict)
     # UUID.__init__ performs the UUID compliance assertion.
-    order_ref = uuid.UUID(out.get("orderRef"), version=4)
-    collect_status = await c.collect(out.get("orderRef"))
+    order_ref = uuid.UUID(out["orderRef"], version=4)
+    collect_status = await c.collect(str(order_ref))
     assert collect_status.get("status") == "pending"
     assert collect_status.get("hintCode") in ("outstandingTransaction", "noClient")
 
 
 @pytest.mark.asyncio
-async def test_invalid_orderref_raises_error(cert_and_key):
+async def test_invalid_orderref_raises_error(cert_and_key: Tuple[str, str]) -> None:
     c = BankIDAsyncClient(certificates=cert_and_key, test_server=True)
     with pytest.raises(exceptions.InvalidParametersError):
         await c.collect("invalid-uuid")
 
 
 @pytest.mark.asyncio
-async def test_already_in_progress_raises_error(cert_and_key, ip_address_async, random_personal_number):
+async def test_already_in_progress_raises_error(cert_and_key: Tuple[str, str], ip_address: str, random_personal_number: str) -> None:
     c = BankIDAsyncClient(certificates=cert_and_key, test_server=True)
-    await c.authenticate(ip_address_async, requirement={"personalNumber": random_personal_number})
+    await c.authenticate(ip_address, requirement={"personalNumber": random_personal_number})
     with pytest.raises(exceptions.AlreadyInProgressError):
-        await c.authenticate(ip_address_async, requirement={"personalNumber": random_personal_number})
+        await c.authenticate(ip_address, requirement={"personalNumber": random_personal_number})
 
 
 @pytest.mark.asyncio
-async def test_already_in_progress_raises_error_2(cert_and_key, ip_address_async, random_personal_number):
+async def test_already_in_progress_raises_error_2(cert_and_key: Tuple[str, str], ip_address: str, random_personal_number: str) -> None:
     c = BankIDAsyncClient(certificates=cert_and_key, test_server=True)
     await c.sign(
-        ip_address_async,
+        ip_address,
         requirement={"personalNumber": random_personal_number},
         user_visible_data="Text to sign",
     )
     with pytest.raises(exceptions.AlreadyInProgressError):
         await c.sign(
-            ip_address_async, requirement={"personalNumber": random_personal_number}, user_visible_data="Text to sign"
+            ip_address, requirement={"personalNumber": random_personal_number}, user_visible_data="Text to sign"
         )
 
 
 @pytest.mark.asyncio
-async def test_authentication_and_cancel(cert_and_key, ip_address_async):
+async def test_authentication_and_cancel(cert_and_key: Tuple[str, str], ip_address: str) -> None:
     """Authenticate call and then cancel it"""
     c = BankIDAsyncClient(certificates=cert_and_key, test_server=True)
-    out = await c.authenticate(ip_address_async)
+    out = await c.authenticate(ip_address)
     assert isinstance(out, dict)
     # UUID.__init__ performs the UUID compliance assertion.
-    order_ref = uuid.UUID(out.get("orderRef"), version=4)
-    collect_status = await c.collect(out.get("orderRef"))
+    order_ref = uuid.UUID(out["orderRef"], version=4)
+    collect_status = await c.collect(str(order_ref))
     assert collect_status.get("status") == "pending"
     assert collect_status.get("hintCode") in ("outstandingTransaction", "noClient")
     success = await c.cancel(str(order_ref))
     assert success
     with pytest.raises(exceptions.InvalidParametersError):
-        collect_status = await c.collect(out.get("orderRef"))
+        collect_status = await c.collect(str(order_ref))
 
 
 @pytest.mark.asyncio
-async def test_phone_authentication_and_cancel(cert_and_key, random_personal_number):
+async def test_phone_authentication_and_cancel(cert_and_key: Tuple[str, str], random_personal_number: str) -> None:
     """Phone authenticate call and then cancel it"""
 
     c = BankIDAsyncClient(certificates=cert_and_key, test_server=True)
     out = await c.phone_authenticate(random_personal_number, "user")
     assert isinstance(out, dict)
     # UUID.__init__ performs the UUID compliance assertion.
-    order_ref = uuid.UUID(out.get("orderRef"), version=4)
-    collect_status = await c.collect(out.get("orderRef"))
+    order_ref = uuid.UUID(out["orderRef"], version=4)
+    collect_status = await c.collect(str(order_ref))
     assert collect_status.get("status") == "pending"
     assert collect_status.get("hintCode") in ("outstandingTransaction", "noClient")
     success = await c.cancel(str(order_ref))
     assert success
     with pytest.raises(exceptions.InvalidParametersError):
-        collect_status = await c.collect(out.get("orderRef"))
+        collect_status = await c.collect(str(order_ref))
 
 
 @pytest.mark.asyncio
-async def test_cancel_with_invalid_uuid(cert_and_key):
+async def test_cancel_with_invalid_uuid(cert_and_key: Tuple[str, str]) -> None:
     c = BankIDAsyncClient(certificates=cert_and_key, test_server=True)
     invalid_order_ref = uuid.uuid4()
     with pytest.raises(exceptions.InvalidParametersError):
         await c.cancel(str(invalid_order_ref))
```

### Comparing `pybankid-1.0.1/tests/test_syncclient.py` & `pybankid-1.1.0/tests/test_syncclient.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,131 +12,132 @@
 
 Created on 2024-01-18
 
 """
 import uuid
 
 import pytest
+from typing import Tuple
 
 try:
     from unittest import mock
 except:
-    import mock
+    import mock  # type: ignore[no-redef]
 
 from bankid import BankIDClient, exceptions
 
 
-def test_authentication_and_collect(cert_and_key, ip_address, random_personal_number):
+def test_authentication_and_collect(cert_and_key: Tuple[str, str], ip_address: str, random_personal_number: str) -> None:
     """Authenticate call and then collect with the returned orderRef UUID."""
 
     c = BankIDClient(certificates=cert_and_key, test_server=True)
-    assert "appapi2.test.bankid.com.pem" in c.verify_cert
-    out = c.authenticate(ip_address, random_personal_number)
+    assert "appapi2.test.bankid.com.pem" in str(c.verify_cert)
+    out = c.authenticate(ip_address, requirement={"personalNumber": random_personal_number})
     assert isinstance(out, dict)
     # UUID.__init__ performs the UUID compliance assertion.
-    order_ref = uuid.UUID(out.get("orderRef"), version=4)
-    collect_status = c.collect(out.get("orderRef"))
-    assert collect_status.get("status") == "pending"
-    assert collect_status.get("hintCode") in ("outstandingTransaction", "noClient")
+    order_ref = uuid.UUID(out["orderRef"], version=4)
+    collect_status = c.collect(str(order_ref))
+    assert collect_status["status"] == "pending"
+    assert collect_status["hintCode"] in ("outstandingTransaction", "noClient")
 
 
-def test_sign_and_collect(cert_and_key, ip_address):
+def test_sign_and_collect(cert_and_key: Tuple[str, str], ip_address: str) -> None:
     """Sign call and then collect with the returned orderRef UUID."""
 
     c = BankIDClient(certificates=cert_and_key, test_server=True)
     out = c.sign(
         ip_address,
         user_visible_data="The data to be signed",
         user_non_visible_data="Non visible data",
     )
     assert isinstance(out, dict)
     # UUID.__init__ performs the UUID compliance assertion.
-    order_ref = uuid.UUID(out.get("orderRef"), version=4)
-    collect_status = c.collect(out.get("orderRef"))
-    assert collect_status.get("status") == "pending"
-    assert collect_status.get("hintCode") in ("outstandingTransaction", "noClient")
+    order_ref = uuid.UUID(out["orderRef"], version=4)
+    collect_status = c.collect(str(order_ref))
+    assert collect_status["status"] == "pending"
+    assert collect_status["hintCode"] in ("outstandingTransaction", "noClient")
 
 
-def test_phone_sign_and_collect(cert_and_key, random_personal_number):
+def test_phone_sign_and_collect(cert_and_key: Tuple[str, str], random_personal_number: str) -> None:
     """Phone sign call and then collect with the returned orderRef UUID."""
 
     c = BankIDClient(certificates=cert_and_key, test_server=True)
     out = c.phone_sign(random_personal_number, "user", user_visible_data="The data to be signed")
     assert isinstance(out, dict)
     # UUID.__init__ performs the UUID compliance assertion.
-    order_ref = uuid.UUID(out.get("orderRef"), version=4)
-    collect_status = c.collect(out.get("orderRef"))
-    assert collect_status.get("status") == "pending"
-    assert collect_status.get("hintCode") in ("outstandingTransaction", "noClient")
+    order_ref = uuid.UUID(out["orderRef"], version=4)
+    collect_status = c.collect(str(order_ref))
+    assert collect_status["status"] == "pending"
+    assert collect_status["hintCode"] in ("outstandingTransaction", "noClient")
 
 
-def test_invalid_orderref_raises_error(cert_and_key):
+def test_invalid_orderref_raises_error(cert_and_key: Tuple[str, str]) -> None:
     c = BankIDClient(certificates=cert_and_key, test_server=True)
     with pytest.raises(exceptions.InvalidParametersError):
         collect_status = c.collect("invalid-uuid")
 
 
-def test_already_in_progress_raises_error(cert_and_key, ip_address, random_personal_number):
+def test_already_in_progress_raises_error(cert_and_key: Tuple[str, str], ip_address: str, random_personal_number: str) -> None:
     c = BankIDClient(certificates=cert_and_key, test_server=True)
     out = c.authenticate(ip_address, requirement={"personalNumber": random_personal_number})
     with pytest.raises(exceptions.AlreadyInProgressError):
         out2 = c.authenticate(ip_address, requirement={"personalNumber": random_personal_number})
 
 
-def test_already_in_progress_raises_error_2(cert_and_key, ip_address, random_personal_number):
+def test_already_in_progress_raises_error_2(cert_and_key: Tuple[str, str], ip_address: str, random_personal_number: str) -> None:
     c = BankIDClient(certificates=cert_and_key, test_server=True)
     out = c.sign(ip_address, requirement={"personalNumber": random_personal_number}, user_visible_data="Text to sign")
     with pytest.raises(exceptions.AlreadyInProgressError):
         out2 = c.sign(
             ip_address, requirement={"personalNumber": random_personal_number}, user_visible_data="Text to sign"
         )
 
 
-def test_authentication_and_cancel(cert_and_key, ip_address, random_personal_number):
+def test_authentication_and_cancel(cert_and_key: Tuple[str, str], ip_address: str, random_personal_number: str) -> None:
     """Authenticate call and then cancel it"""
 
     c = BankIDClient(certificates=cert_and_key, test_server=True)
     out = c.authenticate(ip_address, requirement={"personalNumber": random_personal_number})
     assert isinstance(out, dict)
     # UUID.__init__ performs the UUID compliance assertion.
-    order_ref = uuid.UUID(out.get("orderRef"), version=4)
-    collect_status = c.collect(out.get("orderRef"))
-    assert collect_status.get("status") == "pending"
-    assert collect_status.get("hintCode") in ("outstandingTransaction", "noClient")
+    order_ref = uuid.UUID(out["orderRef"], version=4)
+    collect_status = c.collect(str(order_ref))
+    assert collect_status["status"] == "pending"
+    assert collect_status["hintCode"] in ("outstandingTransaction", "noClient")
     success = c.cancel(str(order_ref))
     assert success
     with pytest.raises(exceptions.InvalidParametersError):
-        collect_status = c.collect(out.get("orderRef"))
+        collect_status = c.collect(str(order_ref))
 
 
-def test_phone_authentication_and_cancel(cert_and_key, random_personal_number):
+def test_phone_authentication_and_cancel(cert_and_key: Tuple[str, str], random_personal_number: str) -> None:
     """Phone authenticate call and then cancel it"""
 
     c = BankIDClient(certificates=cert_and_key, test_server=True)
     out = c.phone_authenticate(random_personal_number, "user")
     assert isinstance(out, dict)
     # UUID.__init__ performs the UUID compliance assertion.
-    order_ref = uuid.UUID(out.get("orderRef"), version=4)
-    collect_status = c.collect(out.get("orderRef"))
-    assert collect_status.get("status") == "pending"
-    assert collect_status.get("hintCode") in ("outstandingTransaction", "noClient")
+    order_ref = uuid.UUID(out["orderRef"], version=4)
+    collect_status = c.collect(str(order_ref))
+    assert collect_status["status"] == "pending"
+    assert collect_status["hintCode"] in ("outstandingTransaction", "noClient")
     success = c.cancel(str(order_ref))
     assert success
     with pytest.raises(exceptions.InvalidParametersError):
-        collect_status = c.collect(out.get("orderRef"))
+        collect_status = c.collect(str(order_ref))
 
 
-def test_cancel_with_invalid_uuid(cert_and_key):
+def test_cancel_with_invalid_uuid(cert_and_key: Tuple[str, str]) -> None:
     c = BankIDClient(certificates=cert_and_key, test_server=True)
     invalid_order_ref = uuid.uuid4()
     with pytest.raises(exceptions.InvalidParametersError):
         cancel_status = c.cancel(str(invalid_order_ref))
 
 
 @pytest.mark.parametrize(
     "test_server, endpoint",
     [(False, "appapi2.bankid.com"), (True, "appapi2.test.bankid.com")],
 )
-def test_correct_prod_server_urls(cert_and_key, test_server, endpoint):
+def test_correct_prod_server_urls(cert_and_key: Tuple[str, str], test_server: bool, endpoint: str) -> None:
     c = BankIDClient(certificates=cert_and_key, test_server=test_server)
     assert c.api_url == "https://{0}/rp/v6.0/".format(endpoint)
-    assert "{0}.pem".format(endpoint) in c.verify_cert
+    assert "{0}.pem".format(endpoint) in str(c.verify_cert)
```

