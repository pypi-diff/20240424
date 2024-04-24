# Comparing `tmp/rlp-4.0.0.tar.gz` & `tmp/rlp-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlp-4.0.0.tar", last modified: Wed Nov 29 22:25:14 2023, max compression
+gzip compressed data, was "rlp-4.0.1.tar", last modified: Wed Apr 24 16:40:41 2024, max compression
```

## Comparing `rlp-4.0.0.tar` & `rlp-4.0.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2023-11-29 22:25:14.805894 rlp-4.0.0/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1088 2023-10-06 17:26:25.000000 rlp-4.0.0/LICENSE
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      168 2023-10-10 00:59:48.000000 rlp-4.0.0/MANIFEST.in
--rw-r--r--   0 pacrob    (1000) pacrob    (1000)     4361 2023-11-29 22:25:14.805894 rlp-4.0.0/PKG-INFO
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2520 2023-10-10 00:59:48.000000 rlp-4.0.0/README.md
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3367 2023-10-12 17:23:52.000000 rlp-4.0.0/pyproject.toml
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2023-11-29 22:25:14.797894 rlp-4.0.0/rlp/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      425 2023-10-12 12:57:03.000000 rlp-4.0.0/rlp/__init__.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      159 2023-10-12 17:23:52.000000 rlp-4.0.0/rlp/atomic.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    12714 2023-10-12 15:45:18.000000 rlp-4.0.0/rlp/codec.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     6032 2023-10-12 17:23:52.000000 rlp-4.0.0/rlp/exceptions.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     6063 2023-10-10 00:59:48.000000 rlp-4.0.0/rlp/lazy.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2023-11-29 22:25:14.801894 rlp-4.0.0/rlp/sedes/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      338 2023-10-12 12:57:11.000000 rlp-4.0.0/rlp/sedes/__init__.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1639 2023-10-12 12:58:21.000000 rlp-4.0.0/rlp/sedes/big_endian_int.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2053 2023-10-11 20:29:01.000000 rlp-4.0.0/rlp/sedes/binary.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      781 2023-10-10 00:59:48.000000 rlp-4.0.0/rlp/sedes/boolean.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4986 2023-10-11 20:29:01.000000 rlp-4.0.0/rlp/sedes/lists.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      736 2023-10-10 00:59:48.000000 rlp-4.0.0/rlp/sedes/raw.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    15387 2023-10-12 17:23:52.000000 rlp-4.0.0/rlp/sedes/serializable.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2372 2023-10-11 20:29:01.000000 rlp-4.0.0/rlp/sedes/text.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       74 2023-10-10 00:59:48.000000 rlp-4.0.0/rlp/utils.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2023-11-29 22:25:14.801894 rlp-4.0.0/rlp.egg-info/
--rw-r--r--   0 pacrob    (1000) pacrob    (1000)     4361 2023-11-29 22:25:14.000000 rlp-4.0.0/rlp.egg-info/PKG-INFO
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      867 2023-11-29 22:25:14.000000 rlp-4.0.0/rlp.egg-info/SOURCES.txt
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        1 2023-11-29 22:25:14.000000 rlp-4.0.0/rlp.egg-info/dependency_links.txt
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        1 2023-11-29 22:07:14.000000 rlp-4.0.0/rlp.egg-info/not-zip-safe
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      373 2023-11-29 22:25:14.000000 rlp-4.0.0/rlp.egg-info/requires.txt
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        4 2023-11-29 22:25:14.000000 rlp-4.0.0/rlp.egg-info/top_level.txt
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       38 2023-11-29 22:25:14.805894 rlp-4.0.0/setup.cfg
--rwxrwxr-x   0 pacrob    (1000) pacrob    (1000)     1903 2023-11-29 22:21:40.000000 rlp-4.0.0/setup.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2023-11-29 22:25:14.801894 rlp-4.0.0/tests/
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2023-11-29 22:25:14.801894 rlp-4.0.0/tests/core/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       48 2023-10-10 00:59:48.000000 rlp-4.0.0/tests/core/test_import.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     7584 2023-10-10 00:59:48.000000 rlp-4.0.0/tests/rlptest.json
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4483 2023-10-10 00:59:48.000000 rlp-4.0.0/tests/speed.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2966 2023-10-10 00:59:48.000000 rlp-4.0.0/tests/test_benchmark.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3866 2023-10-11 20:29:01.000000 rlp-4.0.0/tests/test_big_endian.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3766 2023-10-12 15:52:49.000000 rlp-4.0.0/tests/test_binary_sedes.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1180 2023-10-10 00:59:48.000000 rlp-4.0.0/tests/test_boolean_serializer.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      549 2023-10-10 00:59:48.000000 rlp-4.0.0/tests/test_bytearray.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1826 2023-10-10 00:59:48.000000 rlp-4.0.0/tests/test_codec.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1708 2023-10-10 00:59:48.000000 rlp-4.0.0/tests/test_countablelist.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      471 2023-10-10 00:59:48.000000 rlp-4.0.0/tests/test_invalid.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2378 2023-10-11 20:29:01.000000 rlp-4.0.0/tests/test_json.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3132 2023-10-10 00:59:48.000000 rlp-4.0.0/tests/test_lazy.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      845 2023-10-10 00:59:48.000000 rlp-4.0.0/tests/test_raw_sedes.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2315 2023-10-10 00:59:48.000000 rlp-4.0.0/tests/test_sedes.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    18407 2023-10-11 20:29:01.000000 rlp-4.0.0/tests/test_serializable.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5049 2023-10-10 00:59:48.000000 rlp-4.0.0/tests/test_text_sedes.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-24 16:40:41.222116 rlp-4.0.1/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1088 2024-04-17 17:48:14.000000 rlp-4.0.1/LICENSE
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      196 2024-04-18 17:41:04.000000 rlp-4.0.1/MANIFEST.in
+-rw-r--r--   0 pacrob    (1000) pacrob    (1000)     4526 2024-04-24 16:40:41.222116 rlp-4.0.1/PKG-INFO
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2520 2024-04-18 17:41:04.000000 rlp-4.0.1/README.md
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3447 2024-04-18 17:41:04.000000 rlp-4.0.1/pyproject.toml
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-24 16:40:41.218116 rlp-4.0.1/rlp/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      425 2024-04-17 17:48:14.000000 rlp-4.0.1/rlp/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      159 2024-04-17 17:48:14.000000 rlp-4.0.1/rlp/atomic.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    12714 2024-04-17 17:48:14.000000 rlp-4.0.1/rlp/codec.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5824 2024-04-18 17:41:04.000000 rlp-4.0.1/rlp/exceptions.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     6063 2024-04-17 17:48:14.000000 rlp-4.0.1/rlp/lazy.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-24 16:40:41.218116 rlp-4.0.1/rlp/sedes/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      338 2024-04-17 17:48:14.000000 rlp-4.0.1/rlp/sedes/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1631 2024-04-18 17:41:04.000000 rlp-4.0.1/rlp/sedes/big_endian_int.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2045 2024-04-18 17:41:04.000000 rlp-4.0.1/rlp/sedes/binary.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      781 2024-04-17 17:48:14.000000 rlp-4.0.1/rlp/sedes/boolean.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4968 2024-04-18 17:41:04.000000 rlp-4.0.1/rlp/sedes/lists.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      736 2024-04-17 17:48:14.000000 rlp-4.0.1/rlp/sedes/raw.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    15338 2024-04-18 17:41:04.000000 rlp-4.0.1/rlp/sedes/serializable.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2372 2024-04-17 17:48:14.000000 rlp-4.0.1/rlp/sedes/text.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       74 2024-04-17 17:48:14.000000 rlp-4.0.1/rlp/utils.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-24 16:40:41.218116 rlp-4.0.1/rlp.egg-info/
+-rw-r--r--   0 pacrob    (1000) pacrob    (1000)     4526 2024-04-24 16:40:41.000000 rlp-4.0.1/rlp.egg-info/PKG-INFO
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      959 2024-04-24 16:40:41.000000 rlp-4.0.1/rlp.egg-info/SOURCES.txt
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        1 2024-04-24 16:40:41.000000 rlp-4.0.1/rlp.egg-info/dependency_links.txt
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        1 2024-04-17 17:48:14.000000 rlp-4.0.1/rlp.egg-info/not-zip-safe
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      424 2024-04-24 16:40:41.000000 rlp-4.0.1/rlp.egg-info/requires.txt
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        4 2024-04-24 16:40:41.000000 rlp-4.0.1/rlp.egg-info/top_level.txt
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       38 2024-04-24 16:40:41.222116 rlp-4.0.1/setup.cfg
+-rwxrwxr-x   0 pacrob    (1000) pacrob    (1000)     1973 2024-04-24 16:40:35.000000 rlp-4.0.1/setup.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-24 16:40:41.218116 rlp-4.0.1/tests/
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-24 16:40:41.218116 rlp-4.0.1/tests/core/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     7584 2024-04-18 17:41:04.000000 rlp-4.0.1/tests/core/rlptest.json
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4483 2024-04-18 17:41:04.000000 rlp-4.0.1/tests/core/speed.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2963 2024-04-18 17:41:04.000000 rlp-4.0.1/tests/core/test_benchmark.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3866 2024-04-18 17:41:04.000000 rlp-4.0.1/tests/core/test_big_endian.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3742 2024-04-18 17:41:04.000000 rlp-4.0.1/tests/core/test_binary_sedes.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1180 2024-04-18 17:41:04.000000 rlp-4.0.1/tests/core/test_boolean_serializer.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      526 2024-04-18 17:41:04.000000 rlp-4.0.1/tests/core/test_bytearray.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1827 2024-04-18 17:41:04.000000 rlp-4.0.1/tests/core/test_codec.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1708 2024-04-18 17:41:04.000000 rlp-4.0.1/tests/core/test_countablelist.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       91 2024-04-18 17:41:04.000000 rlp-4.0.1/tests/core/test_import_and_version.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      471 2024-04-18 17:41:04.000000 rlp-4.0.1/tests/core/test_invalid.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2383 2024-04-18 17:41:04.000000 rlp-4.0.1/tests/core/test_json.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3131 2024-04-18 17:41:04.000000 rlp-4.0.1/tests/core/test_lazy.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      845 2024-04-18 17:41:04.000000 rlp-4.0.1/tests/core/test_raw_sedes.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2265 2024-04-18 17:41:04.000000 rlp-4.0.1/tests/core/test_sedes.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    18406 2024-04-18 17:41:04.000000 rlp-4.0.1/tests/core/test_serializable.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5026 2024-04-18 17:41:04.000000 rlp-4.0.1/tests/core/test_text_sedes.py
```

### Comparing `rlp-4.0.0/LICENSE` & `rlp-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rlp-4.0.0/PKG-INFO` & `rlp-4.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlp
-Version: 4.0.0
+Version: 4.0.1
 Summary: rlp: A package for Recursive Length Prefix encoding and decoding
 Home-page: https://github.com/ethereum/pyrlp
 Author: jnnk
 Author-email: jnnknnj@gmail.com
 License: MIT
 Keywords: rlp ethereum
 Classifier: Development Status :: 3 - Alpha
@@ -12,42 +12,45 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: eth-utils>=2
 Provides-Extra: dev
 Requires-Dist: build>=0.9.0; extra == "dev"
 Requires-Dist: bumpversion>=0.5.3; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
 Requires-Dist: pre-commit>=3.4.0; extra == "dev"
 Requires-Dist: tox>=4.0.0; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 Requires-Dist: sphinx>=6.0.0; extra == "dev"
+Requires-Dist: sphinx-autobuild>=2021.3.14; extra == "dev"
 Requires-Dist: sphinx_rtd_theme>=1.0.0; extra == "dev"
 Requires-Dist: towncrier<22,>=21; extra == "dev"
 Requires-Dist: pytest>=7.0.0; extra == "dev"
 Requires-Dist: pytest-xdist>=2.4.0; extra == "dev"
 Requires-Dist: hypothesis==5.19.0; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: sphinx>=6.0.0; extra == "docs"
+Requires-Dist: sphinx-autobuild>=2021.3.14; extra == "docs"
 Requires-Dist: sphinx_rtd_theme>=1.0.0; extra == "docs"
 Requires-Dist: towncrier<22,>=21; extra == "docs"
 Provides-Extra: test
 Requires-Dist: pytest>=7.0.0; extra == "test"
 Requires-Dist: pytest-xdist>=2.4.0; extra == "test"
 Requires-Dist: hypothesis==5.19.0; extra == "test"
 Provides-Extra: rust-backend
-Requires-Dist: rusty-rlp<0.3,>=0.2.1; extra == "rust-backend"
+Requires-Dist: rusty-rlp>=0.2.1; extra == "rust-backend"
 
 # pyrlp
 
 [![Join the conversation on Discord](https://img.shields.io/discord/809793915578089484?color=blue&label=chat&logo=discord&logoColor=white)](https://discord.gg/GHryRvPB84)
 [![Build Status](https://circleci.com/gh/ethereum/pyrlp.svg?style=shield)](https://circleci.com/gh/ethereum/pyrlp)
 [![PyPI version](https://badge.fury.io/py/rlp.svg)](https://badge.fury.io/py/rlp)
 [![Python versions](https://img.shields.io/pypi/pyversions/rlp.svg)](https://pypi.python.org/pypi/rlp)
@@ -61,16 +64,16 @@
 
 ```sh
 python -m pip install rlp
 ```
 
 ## Developer Setup
 
-If you would like to hack on pyrlp, please check out the [Snake Charmers
-Tactical Manual](https://github.com/ethereum/snake-charmers-tactical-manual)
+If you would like to hack on pyrlp, please check out the
+[Snake Charmers Tactical Manual](https://github.com/ethereum/snake-charmers-tactical-manual)
 for information on how we do:
 
 - Testing
 - Pull Requests
 - Documentation
 
 We use [pre-commit](https://pre-commit.com/) to maintain consistent code style. Once
```

### Comparing `rlp-4.0.0/README.md` & `rlp-4.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 
 ```sh
 python -m pip install rlp
 ```
 
 ## Developer Setup
 
-If you would like to hack on pyrlp, please check out the [Snake Charmers
-Tactical Manual](https://github.com/ethereum/snake-charmers-tactical-manual)
+If you would like to hack on pyrlp, please check out the
+[Snake Charmers Tactical Manual](https://github.com/ethereum/snake-charmers-tactical-manual)
 for information on how we do:
 
 - Testing
 - Pull Requests
 - Documentation
 
 We use [pre-commit](https://pre-commit.com/) to maintain consistent code style. Once
```

### Comparing `rlp-4.0.0/pyproject.toml` & `rlp-4.0.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 [tool.autoflake]
-remove_all_unused_imports = "True"
 exclude = "__init__.py"
+remove_all_unused_imports = true
 
 [tool.isort]
-combine_as_imports = "True"
+combine_as_imports = true
 extra_standard_library = "pytest"
 force_grid_wrap = 1
-force_sort_within_sections = "True"
-known_third_party = "hypothesis,pytest"
+force_sort_within_sections = true
+honor_noqa = true
 known_first_party = "rlp"
+known_third_party = "hypothesis"
 multi_line_output = 3
 profile = "black"
+use_parentheses = true
 
 [tool.mypy]
-check_untyped_defs = "True"
-disallow_incomplete_defs = "True"
-disallow_untyped_defs = "True"
-disallow_any_generics = "True"
-disallow_untyped_calls = "True"
-disallow_untyped_decorators = "True"
-disallow_subclassing_any = "True"
-ignore_missing_imports = "True"
-strict_optional = "True"
-strict_equality = "True"
-warn_redundant_casts = "True"
-warn_return_any = "True"
-warn_unused_configs = "True"
-warn_unused_ignores = "True"
+check_untyped_defs = true
+disallow_any_generics = true
+disallow_incomplete_defs = true
+disallow_subclassing_any = true
+disallow_untyped_calls = true
+disallow_untyped_decorators = true
+disallow_untyped_defs = true
+ignore_missing_imports = true
+strict_equality = true
+strict_optional = true
+warn_redundant_casts = true
+warn_return_any = true
+warn_unused_configs = true
+warn_unused_ignores = true
 
 
 [tool.pydocstyle]
 # All error codes found here:
 # http://www.pydocstyle.org/en/3.0.0/error_codes.html
 #
 # Ignored:
@@ -48,37 +50,38 @@
 # D204 - 1 blank line required after class docstring
 # D205 - 1 blank line required between summary line and description
 # D212 - Multi-line docstring summary should start at the first line
 # D302 - Use u""" for Unicode docstrings
 # D400 - First line should end with a period
 # D401 - First line should be in imperative mood
 # D412 - No blank lines allowed between a section header and its content
+# D415 - First line should end with a period, question mark, or exclamation point
 add-ignore = "D200,D203,D204,D205,D212,D302,D400,D401,D412,D415"
 
 # Explanation:
 # D400 - Enabling this error code seems to make it a requirement that the first
 # sentence in a docstring is not split across two lines.  It also makes it a
 # requirement that no docstring can have a multi-sentence description without a
 # summary line.  Neither one of those requirements seem appropriate.
 
 [tool.pytest.ini_options]
 addopts = "-v --showlocals --durations 10"
-xfail_strict = "True"
-log_format = "%(levelname)8s  %(asctime)s  %(filename)20s  %(message)s"
 log_date_format = "%m-%d %H:%M:%S"
+log_format = "%(levelname)8s  %(asctime)s  %(filename)20s  %(message)s"
 markers = "benchmark"
+xfail_strict = true
 
 [tool.towncrier]
 # Read https://github.com/ethereum/pyrlp/blob/main/newsfragments/README.md for instructions
-package = "rlp"
-filename = "docs/release_notes.rst"
 directory = "newsfragments"
-underlines = ["-", "~", "^"]
-title_format = "pyrlp v{version} ({project_date})"
+filename = "docs/release_notes.rst"
 issue_format = "`#{issue} <https://github.com/ethereum/pyrlp/issues/{issue}>`__"
+package = "rlp"
+title_format = "pyrlp v{version} ({project_date})"
+underlines = ["-", "~", "^"]
 
 [[tool.towncrier.type]]
 directory = "breaking"
 name = "Breaking Changes"
 showcontent = true
 
 [[tool.towncrier.type]]
```

### Comparing `rlp-4.0.0/rlp/codec.py` & `rlp-4.0.1/rlp/codec.py`

 * *Files identical despite different names*

### Comparing `rlp-4.0.0/rlp/exceptions.py` & `rlp-4.0.1/rlp/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,39 +6,39 @@
     """
     Exception raised if encoding fails.
 
     :ivar obj: the object that could not be encoded
     """
 
     def __init__(self, message, obj):
-        super(EncodingError, self).__init__(message)
+        super().__init__(message)
         self.obj = obj
 
 
 class DecodingError(RLPException):
     """
     Exception raised if decoding fails.
 
     :ivar rlp: the RLP string that could not be decoded
     """
 
     def __init__(self, message, rlp):
-        super(DecodingError, self).__init__(message)
+        super().__init__(message)
         self.rlp = rlp
 
 
 class SerializationError(RLPException):
     """
     Exception raised if serialization fails.
 
     :ivar obj: the object that could not be serialized
     """
 
     def __init__(self, message, obj):
-        super(SerializationError, self).__init__(message)
+        super().__init__(message)
         self.obj = obj
 
 
 class ListSerializationError(SerializationError):
     """
     Exception raised if serialization by a :class:`sedes.List` fails.
 
@@ -53,15 +53,15 @@
         if message is None:
             assert index is not None
             assert element_exception is not None
             message = (
                 f"Serialization failed because of element at index {index} "
                 f'("{str(element_exception)}")'
             )
-        super(ListSerializationError, self).__init__(message, obj)
+        super().__init__(message, obj)
         self.index = index
         self.element_exception = element_exception
 
 
 class ObjectSerializationError(SerializationError):
     """
     Exception raised if serialization of a :class:`sedes.Serializable` object fails.
@@ -87,28 +87,28 @@
                 field = sedes._meta.field_names[list_exception.index]
                 message = (
                     f"Serialization failed because of field {field} "
                     f'("{str(list_exception.element_exception)}")'
                 )
         else:
             field = None
-        super(ObjectSerializationError, self).__init__(message, obj)
+        super().__init__(message, obj)
         self.field = field
         self.list_exception = list_exception
 
 
 class DeserializationError(RLPException):
     """
     Exception raised if deserialization fails.
 
     :ivar serial: the decoded RLP string that could not be deserialized
     """
 
     def __init__(self, message, serial):
-        super(DeserializationError, self).__init__(message)
+        super().__init__(message)
         self.serial = serial
 
 
 class ListDeserializationError(DeserializationError):
     """
     Exception raised if deserialization by a :class:`sedes.List` fails.
 
@@ -123,15 +123,15 @@
         if not message:
             assert index is not None
             assert element_exception is not None
             message = (
                 f"Deserialization failed because of element at index {index} "
                 f'("{str(element_exception)}")'
             )
-        super(ListDeserializationError, self).__init__(message, serial)
+        super().__init__(message, serial)
         self.index = index
         self.element_exception = element_exception
 
 
 class ObjectDeserializationError(DeserializationError):
     """
     Exception raised if deserialization by a :class:`sedes.Serializable` fails.
@@ -155,11 +155,11 @@
             else:
                 assert sedes is not None
                 field = sedes._meta.field_names[list_exception.index]
                 message = (
                     f"Deserialization failed because of field {field} "
                     f'("{str(list_exception.element_exception)}")'
                 )
-        super(ObjectDeserializationError, self).__init__(message, serial)
+        super().__init__(message, serial)
         self.sedes = sedes
         self.list_exception = list_exception
         self.field = field
```

### Comparing `rlp-4.0.0/rlp/lazy.py` & `rlp-4.0.1/rlp/lazy.py`

 * *Files identical despite different names*

### Comparing `rlp-4.0.0/rlp/sedes/big_endian_int.py` & `rlp-4.0.1/rlp/sedes/big_endian_int.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from rlp.exceptions import (
     DeserializationError,
     SerializationError,
 )
 
 
-class BigEndianInt(object):
+class BigEndianInt:
     """
     A sedes for big endian integers.
 
     :param l: the size of the serialized representation in bytes or `None` to
               use the shortest possible one
     """
```

### Comparing `rlp-4.0.0/rlp/sedes/binary.py` & `rlp-4.0.1/rlp/sedes/binary.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 )
 from rlp.exceptions import (
     DeserializationError,
     SerializationError,
 )
 
 
-class Binary(object):
+class Binary:
     """
     A sedes object for binary data of certain length.
 
     :param min_length: the minimal length in bytes or `None` for no lower limit
     :param max_length: the maximal length in bytes or `None` for no upper limit
     :param allow_empty: if true, empty strings are considered valid even if
                         a minimum length is required otherwise
```

### Comparing `rlp-4.0.0/rlp/sedes/boolean.py` & `rlp-4.0.1/rlp/sedes/boolean.py`

 * *Files identical despite different names*

### Comparing `rlp-4.0.0/rlp/sedes/lists.py` & `rlp-4.0.1/rlp/sedes/lists.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     :param strict: If true (de)serializing lists that have a length not
                    matching the sedes length will result in an error. If false
                    (de)serialization will stop as soon as either one of the
                    lists runs out of elements.
     """
 
     def __init__(self, elements=None, strict=True):
-        super(List, self).__init__()
+        super().__init__()
         self.strict = strict
 
         if elements:
             for e in elements:
                 if is_sedes(e):
                     self.append(e)
                 elif isinstance(e, Sequence):
@@ -99,15 +99,15 @@
                 yield sedes.deserialize(element)
             except DeserializationError as e:
                 raise ListDeserializationError(
                     serial=serial, element_exception=e, index=idx
                 )
 
 
-class CountableList(object):
+class CountableList:
     """
     A sedes for lists of arbitrary length.
 
     :param element_sedes: when (de-)serializing a list, this sedes will be
                           applied to all of its elements
     :param max_length: maximum number of allowed elements, or `None` for no limit
     """
```

### Comparing `rlp-4.0.0/rlp/sedes/raw.py` & `rlp-4.0.1/rlp/sedes/raw.py`

 * *Files identical despite different names*

### Comparing `rlp-4.0.0/rlp/sedes/serializable.py` & `rlp-4.0.1/rlp/sedes/serializable.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,17 +201,15 @@
 
         for value, attr in zip(field_values, self._meta.field_attrs):
             setattr(self, attr, make_immutable(value))
 
     _cached_rlp = None
 
     def as_dict(self):
-        return dict(
-            (field, value) for field, value in zip(self._meta.field_names, self)
-        )
+        return {field: value for field, value in zip(self._meta.field_names, self)}
 
     def __iter__(self):
         for attr in self._meta.field_attrs:
             yield getattr(self, attr)
 
     def __getitem__(self, idx):
         if isinstance(idx, int):
@@ -349,15 +347,15 @@
         yield from cls.__dict__.keys()
     if hasattr(cls, "__slots__"):
         yield from cls.__slots__
 
 
 class SerializableBase(abc.ABCMeta):
     def __new__(cls, name, bases, attrs):
-        super_new = super(SerializableBase, cls).__new__
+        super_new = super().__new__
 
         serializable_bases = tuple(b for b in bases if isinstance(b, SerializableBase))
         has_multiple_serializable_parents = len(serializable_bases) > 1
         is_serializable_subclass = any(serializable_bases)
         declares_fields = "fields" in attrs
 
         if not is_serializable_subclass:
```

### Comparing `rlp-4.0.0/rlp/sedes/text.py` & `rlp-4.0.1/rlp/sedes/text.py`

 * *Files identical despite different names*

### Comparing `rlp-4.0.0/rlp.egg-info/PKG-INFO` & `rlp-4.0.1/rlp.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlp
-Version: 4.0.0
+Version: 4.0.1
 Summary: rlp: A package for Recursive Length Prefix encoding and decoding
 Home-page: https://github.com/ethereum/pyrlp
 Author: jnnk
 Author-email: jnnknnj@gmail.com
 License: MIT
 Keywords: rlp ethereum
 Classifier: Development Status :: 3 - Alpha
@@ -12,42 +12,45 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: eth-utils>=2
 Provides-Extra: dev
 Requires-Dist: build>=0.9.0; extra == "dev"
 Requires-Dist: bumpversion>=0.5.3; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
 Requires-Dist: pre-commit>=3.4.0; extra == "dev"
 Requires-Dist: tox>=4.0.0; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 Requires-Dist: sphinx>=6.0.0; extra == "dev"
+Requires-Dist: sphinx-autobuild>=2021.3.14; extra == "dev"
 Requires-Dist: sphinx_rtd_theme>=1.0.0; extra == "dev"
 Requires-Dist: towncrier<22,>=21; extra == "dev"
 Requires-Dist: pytest>=7.0.0; extra == "dev"
 Requires-Dist: pytest-xdist>=2.4.0; extra == "dev"
 Requires-Dist: hypothesis==5.19.0; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: sphinx>=6.0.0; extra == "docs"
+Requires-Dist: sphinx-autobuild>=2021.3.14; extra == "docs"
 Requires-Dist: sphinx_rtd_theme>=1.0.0; extra == "docs"
 Requires-Dist: towncrier<22,>=21; extra == "docs"
 Provides-Extra: test
 Requires-Dist: pytest>=7.0.0; extra == "test"
 Requires-Dist: pytest-xdist>=2.4.0; extra == "test"
 Requires-Dist: hypothesis==5.19.0; extra == "test"
 Provides-Extra: rust-backend
-Requires-Dist: rusty-rlp<0.3,>=0.2.1; extra == "rust-backend"
+Requires-Dist: rusty-rlp>=0.2.1; extra == "rust-backend"
 
 # pyrlp
 
 [![Join the conversation on Discord](https://img.shields.io/discord/809793915578089484?color=blue&label=chat&logo=discord&logoColor=white)](https://discord.gg/GHryRvPB84)
 [![Build Status](https://circleci.com/gh/ethereum/pyrlp.svg?style=shield)](https://circleci.com/gh/ethereum/pyrlp)
 [![PyPI version](https://badge.fury.io/py/rlp.svg)](https://badge.fury.io/py/rlp)
 [![Python versions](https://img.shields.io/pypi/pyversions/rlp.svg)](https://pypi.python.org/pypi/rlp)
@@ -61,16 +64,16 @@
 
 ```sh
 python -m pip install rlp
 ```
 
 ## Developer Setup
 
-If you would like to hack on pyrlp, please check out the [Snake Charmers
-Tactical Manual](https://github.com/ethereum/snake-charmers-tactical-manual)
+If you would like to hack on pyrlp, please check out the
+[Snake Charmers Tactical Manual](https://github.com/ethereum/snake-charmers-tactical-manual)
 for information on how we do:
 
 - Testing
 - Pull Requests
 - Documentation
 
 We use [pre-commit](https://pre-commit.com/) to maintain consistent code style. Once
```

### Comparing `rlp-4.0.0/setup.py` & `rlp-4.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 from setuptools import (
     find_packages,
     setup,
 )
 
 extras_require = {
     "dev": [
@@ -13,37 +12,38 @@
         "pre-commit>=3.4.0",
         "tox>=4.0.0",
         "twine",
         "wheel",
     ],
     "docs": [
         "sphinx>=6.0.0",
+        "sphinx-autobuild>=2021.3.14",
         "sphinx_rtd_theme>=1.0.0",
         "towncrier>=21,<22",
     ],
     "test": [
         "pytest>=7.0.0",
         "pytest-xdist>=2.4.0",
         "hypothesis==5.19.0",
     ],
-    "rust-backend": ["rusty-rlp>=0.2.1, <0.3"],
+    "rust-backend": ["rusty-rlp>=0.2.1"],
 }
 
 
 extras_require["dev"] = (
     extras_require["dev"] + extras_require["docs"] + extras_require["test"]
 )
 
 with open("./README.md") as readme:
     long_description = readme.read()
 
 setup(
     name="rlp",
     # *IMPORTANT*: Don't manually change the version here. See README for more.
-    version="4.0.0",
+    version="4.0.1",
     description="""rlp: A package for Recursive Length Prefix encoding and decoding""",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="jnnk",
     author_email="jnnknnj@gmail.com",
     url="https://github.com/ethereum/pyrlp",
     include_package_data=True,
@@ -52,20 +52,21 @@
     ],
     python_requires=">=3.8, <4",
     extras_require=extras_require,
     py_modules=["rlp"],
     license="MIT",
     zip_safe=False,
     keywords="rlp ethereum",
-    packages=find_packages(exclude=["tests", "tests.*"]),
+    packages=find_packages(exclude=["scripts", "tests", "tests.*"]),
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
 )
```

### Comparing `rlp-4.0.0/tests/rlptest.json` & `rlp-4.0.1/tests/core/rlptest.json`

 * *Files identical despite different names*

### Comparing `rlp-4.0.0/tests/speed.py` & `rlp-4.0.1/tests/core/speed.py`

 * *Files identical despite different names*

### Comparing `rlp-4.0.0/tests/test_benchmark.py` & `rlp-4.0.1/tests/core/test_benchmark.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from itertools import (
     chain,
     repeat,
 )
-import sys
-
 import pytest
+import sys
 
 import rlp
 from rlp.exceptions import (
     DecodingError,
     DeserializationError,
 )
 from rlp.sedes import (
@@ -72,15 +71,15 @@
 
     return f
 
 
 def generate_test_functions():
     valid = {}
     invalid = {}
-    long_string = bytes(bytearray((i % 256 for i in range(SIZE))))
+    long_string = bytes(bytearray(i % 256 for i in range(SIZE)))
     long_list = rlp.encode([c for c in long_string])
     invalid["long_string"] = long_string
     invalid["long_list"] = long_list
 
     nested_list = rlp.encode(b"\x00")
     for _ in repeat(None, SIZE):
         nested_list += rlp.codec.length_prefix(len(nested_list), 0xC0)
```

### Comparing `rlp-4.0.0/tests/test_big_endian.py` & `rlp-4.0.1/tests/core/test_big_endian.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import binascii
+import pytest
 
 from eth_utils import (
     int_to_big_endian,
 )
-import pytest
 
 from rlp import (
     SerializationError,
 )
 from rlp.sedes import (
     BigEndianInt,
     big_endian_int,
```

### Comparing `rlp-4.0.0/tests/test_binary_sedes.py` & `rlp-4.0.1/tests/core/test_binary_sedes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: UTF-8 -*-
 import pytest
 
 from rlp import (
     SerializationError,
 )
 from rlp.sedes import (
     Binary,
```

### Comparing `rlp-4.0.0/tests/test_boolean_serializer.py` & `rlp-4.0.1/tests/core/test_boolean_serializer.py`

 * *Files identical despite different names*

### Comparing `rlp-4.0.0/tests/test_bytearray.py` & `rlp-4.0.1/tests/core/test_bytearray.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf8 -*-
 from rlp import (
     decode,
     decode_lazy,
     encode,
 )
```

### Comparing `rlp-4.0.0/tests/test_codec.py` & `rlp-4.0.1/tests/core/test_codec.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+import pytest
+
 from eth_utils import (
     decode_hex,
 )
-import pytest
 
 from rlp import (
     decode,
     encode,
 )
 from rlp.codec import (
     consume_item,
```

### Comparing `rlp-4.0.0/tests/test_countablelist.py` & `rlp-4.0.1/tests/core/test_countablelist.py`

 * *Files identical despite different names*

### Comparing `rlp-4.0.0/tests/test_json.py` & `rlp-4.0.1/tests/core/test_json.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
+import pytest
 
 from eth_utils import (
     add_0x_prefix,
     decode_hex,
     encode_hex,
 )
-import pytest
 
 import rlp
 from rlp import (
     DecodingError,
     decode,
     decode_lazy,
     encode,
@@ -45,15 +45,15 @@
     else:
         if len(list(zipped)) == len(got) == len(expected):
             return all(compare_nested(x, y) for x, y in zipped)
         else:
             return False
 
 
-with open("tests/rlptest.json") as rlptest_file:
+with open("tests/core/rlptest.json") as rlptest_file:
     test_data = json.load(rlptest_file)
     test_pieces = [
         (
             name,
             {
                 "in": normalize_input(in_out["in"]),
                 "out": add_0x_prefix(in_out["out"]),
```

### Comparing `rlp-4.0.0/tests/test_lazy.py` & `rlp-4.0.1/tests/core/test_lazy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from collections.abc import (
     Sequence,
 )
-
 import pytest
 
 import rlp
 from rlp import (
     DeserializationError,
 )
 from rlp.sedes import (
```

### Comparing `rlp-4.0.0/tests/test_raw_sedes.py` & `rlp-4.0.1/tests/core/test_raw_sedes.py`

 * *Files identical despite different names*

### Comparing `rlp-4.0.0/tests/test_sedes.py` & `rlp-4.0.1/tests/core/test_sedes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-from __future__ import (
-    unicode_literals,
-)
-
 import pytest
 
 from rlp import (
     DeserializationError,
     SerializationError,
     infer_sedes,
 )
```

### Comparing `rlp-4.0.0/tests/test_serializable.py` & `rlp-4.0.1/tests/core/test_serializable.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from multiprocessing import (
     get_context,
 )
 import pickle
-import re
-
 import pytest
+import re
 
 from rlp import (
     SerializationError,
     decode,
     encode,
     infer_sedes,
 )
```

### Comparing `rlp-4.0.0/tests/test_text_sedes.py` & `rlp-4.0.1/tests/core/test_text_sedes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# -*- coding: UTF-8 -*-
+import pytest
+
 from hypothesis import (
     given,
     strategies as st,
 )
-import pytest
 
 from rlp import (
     DeserializationError,
     SerializationError,
     decode,
     encode,
 )
```

