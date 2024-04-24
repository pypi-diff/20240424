# Comparing `tmp/mo_math-7.601.24115.tar.gz` & `tmp/mo_math-7.602.24115.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mo_math-7.601.24115.tar", last modified: Wed Apr 24 08:57:51 2024, max compression
+gzip compressed data, was "mo_math-7.602.24115.tar", last modified: Wed Apr 24 10:14:56 2024, max compression
```

## Comparing `mo_math-7.601.24115.tar` & `mo_math-7.602.24115.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 08:57:51.109499 mo_math-7.601.24115/
--rw-rw-rw-   0        0        0    16725 2019-11-12 19:25:00.000000 mo_math-7.601.24115/LICENSE
--rw-rw-rw-   0        0        0     3606 2024-04-24 08:57:51.109499 mo_math-7.601.24115/PKG-INFO
--rw-rw-rw-   0        0        0     2492 2024-03-02 21:24:19.000000 mo_math-7.601.24115/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 08:57:51.086128 mo_math-7.601.24115/mo_math/
--rw-rw-rw-   0        0        0     9717 2024-04-20 01:24:30.000000 mo_math-7.601.24115/mo_math/__init__.py
--rw-rw-rw-   0        0        0     2992 2024-01-28 14:34:02.000000 mo_math-7.601.24115/mo_math/aes_crypto.py
--rw-rw-rw-   0        0        0      299 2023-05-30 00:20:59.000000 mo_math-7.601.24115/mo_math/crypto.py
--rw-rw-rw-   0        0        0      527 2023-05-30 00:20:59.000000 mo_math-7.601.24115/mo_math/hashes.py
--rw-rw-rw-   0        0        0     1535 2023-05-30 00:20:59.000000 mo_math-7.601.24115/mo_math/randoms.py
--rw-rw-rw-   0        0        0     1938 2023-05-30 00:20:59.000000 mo_math-7.601.24115/mo_math/rsa_crypto.py
--rw-rw-rw-   0        0        0    10687 2024-02-15 02:34:15.000000 mo_math-7.601.24115/mo_math/stats.py
-drwxrwxrwx   0        0        0        0 2024-04-24 08:57:51.095996 mo_math-7.601.24115/mo_math/vendor/
--rw-rw-rw-   0        0        0        0 2019-09-12 20:40:04.000000 mo_math-7.601.24115/mo_math/vendor/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 08:57:51.106532 mo_math-7.601.24115/mo_math/vendor/aespython/
--rw-rw-rw-   0        0        0        0 2019-09-12 20:40:04.000000 mo_math-7.601.24115/mo_math/vendor/aespython/__init__.py
--rw-rw-rw-   0        0        0     5568 2022-12-05 00:55:06.000000 mo_math-7.601.24115/mo_math/vendor/aespython/aes_cipher.py
--rw-rw-rw-   0        0        0    12043 2022-12-05 00:49:49.000000 mo_math-7.601.24115/mo_math/vendor/aespython/aes_tables.py
--rw-rw-rw-   0        0        0     1836 2022-12-05 00:49:49.000000 mo_math-7.601.24115/mo_math/vendor/aespython/cbc_mode.py
--rw-rw-rw-   0        0        0     1715 2022-12-05 00:49:49.000000 mo_math-7.601.24115/mo_math/vendor/aespython/cfb_mode.py
--rw-rw-rw-   0        0        0     1103 2022-12-05 00:55:06.000000 mo_math-7.601.24115/mo_math/vendor/aespython/cipher_mode.py
--rw-rw-rw-   0        0        0     5263 2022-12-05 00:49:49.000000 mo_math-7.601.24115/mo_math/vendor/aespython/key_expander.py
--rw-rw-rw-   0        0        0     1276 2022-12-05 00:49:49.000000 mo_math-7.601.24115/mo_math/vendor/aespython/mode_test.py
--rw-rw-rw-   0        0        0     1871 2022-12-05 00:49:49.000000 mo_math-7.601.24115/mo_math/vendor/aespython/ofb_mode.py
--rw-rw-rw-   0        0        0     8248 2022-12-05 00:49:49.000000 mo_math-7.601.24115/mo_math/vendor/aespython/test_keys.py
-drwxrwxrwx   0        0        0        0 2024-04-24 08:57:51.109499 mo_math-7.601.24115/mo_math/vendor/strangman/
--rw-rw-rw-   0        0        0        0 2019-09-12 20:40:06.000000 mo_math-7.601.24115/mo_math/vendor/strangman/__init__.py
--rw-rw-rw-   0        0        0     7191 2019-09-12 20:40:06.000000 mo_math-7.601.24115/mo_math/vendor/strangman/pstat.py
--rw-rw-rw-   0        0        0    55583 2022-12-04 23:23:18.000000 mo_math-7.601.24115/mo_math/vendor/strangman/stats.py
--rw-rw-rw-   0        0        0     5514 2022-12-05 00:49:49.000000 mo_math-7.601.24115/mo_math/vendor/strangman/statstest.py
-drwxrwxrwx   0        0        0        0 2024-04-24 08:57:51.109499 mo_math-7.601.24115/mo_math.egg-info/
--rw-rw-rw-   0        0        0     3606 2024-04-24 08:57:51.000000 mo_math-7.601.24115/mo_math.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      869 2024-04-24 08:57:51.000000 mo_math-7.601.24115/mo_math.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 08:57:51.000000 mo_math-7.601.24115/mo_math.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2024-04-24 08:57:51.000000 mo_math-7.601.24115/mo_math.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-24 08:57:51.000000 mo_math-7.601.24115/mo_math.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 08:57:51.109499 mo_math-7.601.24115/setup.cfg
--rw-rw-rw-   0        0        0     3700 2024-04-24 08:57:46.000000 mo_math-7.601.24115/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 10:14:56.730155 mo_math-7.602.24115/
+-rw-rw-rw-   0        0        0    16725 2019-11-12 19:25:00.000000 mo_math-7.602.24115/LICENSE
+-rw-rw-rw-   0        0        0     3606 2024-04-24 10:14:56.729022 mo_math-7.602.24115/PKG-INFO
+-rw-rw-rw-   0        0        0     2492 2024-03-02 21:24:19.000000 mo_math-7.602.24115/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 10:14:56.703606 mo_math-7.602.24115/mo_math/
+-rw-rw-rw-   0        0        0     9717 2024-04-20 01:24:30.000000 mo_math-7.602.24115/mo_math/__init__.py
+-rw-rw-rw-   0        0        0     2992 2024-01-28 14:34:02.000000 mo_math-7.602.24115/mo_math/aes_crypto.py
+-rw-rw-rw-   0        0        0      299 2023-05-30 00:20:59.000000 mo_math-7.602.24115/mo_math/crypto.py
+-rw-rw-rw-   0        0        0      527 2023-05-30 00:20:59.000000 mo_math-7.602.24115/mo_math/hashes.py
+-rw-rw-rw-   0        0        0     1535 2023-05-30 00:20:59.000000 mo_math-7.602.24115/mo_math/randoms.py
+-rw-rw-rw-   0        0        0     1938 2023-05-30 00:20:59.000000 mo_math-7.602.24115/mo_math/rsa_crypto.py
+-rw-rw-rw-   0        0        0    10687 2024-02-15 02:34:15.000000 mo_math-7.602.24115/mo_math/stats.py
+drwxrwxrwx   0        0        0        0 2024-04-24 10:14:56.712782 mo_math-7.602.24115/mo_math/vendor/
+-rw-rw-rw-   0        0        0        0 2019-09-12 20:40:04.000000 mo_math-7.602.24115/mo_math/vendor/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 10:14:56.723096 mo_math-7.602.24115/mo_math/vendor/aespython/
+-rw-rw-rw-   0        0        0        0 2019-09-12 20:40:04.000000 mo_math-7.602.24115/mo_math/vendor/aespython/__init__.py
+-rw-rw-rw-   0        0        0     5568 2022-12-05 00:55:06.000000 mo_math-7.602.24115/mo_math/vendor/aespython/aes_cipher.py
+-rw-rw-rw-   0        0        0    12043 2022-12-05 00:49:49.000000 mo_math-7.602.24115/mo_math/vendor/aespython/aes_tables.py
+-rw-rw-rw-   0        0        0     1836 2022-12-05 00:49:49.000000 mo_math-7.602.24115/mo_math/vendor/aespython/cbc_mode.py
+-rw-rw-rw-   0        0        0     1715 2022-12-05 00:49:49.000000 mo_math-7.602.24115/mo_math/vendor/aespython/cfb_mode.py
+-rw-rw-rw-   0        0        0     1103 2022-12-05 00:55:06.000000 mo_math-7.602.24115/mo_math/vendor/aespython/cipher_mode.py
+-rw-rw-rw-   0        0        0     5263 2022-12-05 00:49:49.000000 mo_math-7.602.24115/mo_math/vendor/aespython/key_expander.py
+-rw-rw-rw-   0        0        0     1276 2022-12-05 00:49:49.000000 mo_math-7.602.24115/mo_math/vendor/aespython/mode_test.py
+-rw-rw-rw-   0        0        0     1871 2022-12-05 00:49:49.000000 mo_math-7.602.24115/mo_math/vendor/aespython/ofb_mode.py
+-rw-rw-rw-   0        0        0     8248 2022-12-05 00:49:49.000000 mo_math-7.602.24115/mo_math/vendor/aespython/test_keys.py
+drwxrwxrwx   0        0        0        0 2024-04-24 10:14:56.726865 mo_math-7.602.24115/mo_math/vendor/strangman/
+-rw-rw-rw-   0        0        0        0 2019-09-12 20:40:06.000000 mo_math-7.602.24115/mo_math/vendor/strangman/__init__.py
+-rw-rw-rw-   0        0        0     7191 2019-09-12 20:40:06.000000 mo_math-7.602.24115/mo_math/vendor/strangman/pstat.py
+-rw-rw-rw-   0        0        0    55583 2022-12-04 23:23:18.000000 mo_math-7.602.24115/mo_math/vendor/strangman/stats.py
+-rw-rw-rw-   0        0        0     5514 2022-12-05 00:49:49.000000 mo_math-7.602.24115/mo_math/vendor/strangman/statstest.py
+drwxrwxrwx   0        0        0        0 2024-04-24 10:14:56.728008 mo_math-7.602.24115/mo_math.egg-info/
+-rw-rw-rw-   0        0        0     3606 2024-04-24 10:14:56.000000 mo_math-7.602.24115/mo_math.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      869 2024-04-24 10:14:56.000000 mo_math-7.602.24115/mo_math.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 10:14:56.000000 mo_math-7.602.24115/mo_math.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2024-04-24 10:14:56.000000 mo_math-7.602.24115/mo_math.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-24 10:14:56.000000 mo_math-7.602.24115/mo_math.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 10:14:56.730155 mo_math-7.602.24115/setup.cfg
+-rw-rw-rw-   0        0        0     3700 2024-04-24 10:14:52.000000 mo_math-7.602.24115/setup.py
```

### Comparing `mo_math-7.601.24115/LICENSE` & `mo_math-7.602.24115/LICENSE`

 * *Files identical despite different names*

### Comparing `mo_math-7.601.24115/PKG-INFO` & `mo_math-7.602.24115/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-math
-Version: 7.601.24115
+Version: 7.602.24115
 Summary: More Math! Many of the aggregates you are familiar with, but null-safe
 Home-page: https://github.com/klahnakoski/mo-math
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.8
@@ -13,15 +13,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-dots==9.601.24115
+Requires-Dist: mo-dots==9.602.24115
 Requires-Dist: mo-future==7.584.24095
 Provides-Extra: tests
 Requires-Dist: mo-json>=6.589.24111; extra == "tests"
 Requires-Dist: mo-testing>=8.591.24112; extra == "tests"
 
 
 # More Math!
```

### Comparing `mo_math-7.601.24115/README.md` & `mo_math-7.602.24115/README.md`

 * *Files identical despite different names*

### Comparing `mo_math-7.601.24115/mo_math/__init__.py` & `mo_math-7.602.24115/mo_math/__init__.py`

 * *Files identical despite different names*

### Comparing `mo_math-7.601.24115/mo_math/aes_crypto.py` & `mo_math-7.602.24115/mo_math/aes_crypto.py`

 * *Files identical despite different names*

### Comparing `mo_math-7.601.24115/mo_math/hashes.py` & `mo_math-7.602.24115/mo_math/hashes.py`

 * *Files identical despite different names*

### Comparing `mo_math-7.601.24115/mo_math/randoms.py` & `mo_math-7.602.24115/mo_math/randoms.py`

 * *Files identical despite different names*

### Comparing `mo_math-7.601.24115/mo_math/rsa_crypto.py` & `mo_math-7.602.24115/mo_math/rsa_crypto.py`

 * *Files identical despite different names*

### Comparing `mo_math-7.601.24115/mo_math/stats.py` & `mo_math-7.602.24115/mo_math/stats.py`

 * *Files identical despite different names*

### Comparing `mo_math-7.601.24115/mo_math/vendor/aespython/aes_cipher.py` & `mo_math-7.602.24115/mo_math/vendor/aespython/aes_cipher.py`

 * *Files identical despite different names*

### Comparing `mo_math-7.601.24115/mo_math/vendor/aespython/aes_tables.py` & `mo_math-7.602.24115/mo_math/vendor/aespython/aes_tables.py`

 * *Files identical despite different names*

### Comparing `mo_math-7.601.24115/mo_math/vendor/aespython/cbc_mode.py` & `mo_math-7.602.24115/mo_math/vendor/aespython/cbc_mode.py`

 * *Files identical despite different names*

### Comparing `mo_math-7.601.24115/mo_math/vendor/aespython/cfb_mode.py` & `mo_math-7.602.24115/mo_math/vendor/aespython/cfb_mode.py`

 * *Files identical despite different names*

### Comparing `mo_math-7.601.24115/mo_math/vendor/aespython/cipher_mode.py` & `mo_math-7.602.24115/mo_math/vendor/aespython/cipher_mode.py`

 * *Files identical despite different names*

### Comparing `mo_math-7.601.24115/mo_math/vendor/aespython/key_expander.py` & `mo_math-7.602.24115/mo_math/vendor/aespython/key_expander.py`

 * *Files identical despite different names*

### Comparing `mo_math-7.601.24115/mo_math/vendor/aespython/mode_test.py` & `mo_math-7.602.24115/mo_math/vendor/aespython/mode_test.py`

 * *Files identical despite different names*

### Comparing `mo_math-7.601.24115/mo_math/vendor/aespython/ofb_mode.py` & `mo_math-7.602.24115/mo_math/vendor/aespython/ofb_mode.py`

 * *Files identical despite different names*

### Comparing `mo_math-7.601.24115/mo_math/vendor/aespython/test_keys.py` & `mo_math-7.602.24115/mo_math/vendor/aespython/test_keys.py`

 * *Files identical despite different names*

### Comparing `mo_math-7.601.24115/mo_math/vendor/strangman/pstat.py` & `mo_math-7.602.24115/mo_math/vendor/strangman/pstat.py`

 * *Files identical despite different names*

### Comparing `mo_math-7.601.24115/mo_math/vendor/strangman/stats.py` & `mo_math-7.602.24115/mo_math/vendor/strangman/stats.py`

 * *Files identical despite different names*

### Comparing `mo_math-7.601.24115/mo_math/vendor/strangman/statstest.py` & `mo_math-7.602.24115/mo_math/vendor/strangman/statstest.py`

 * *Files identical despite different names*

### Comparing `mo_math-7.601.24115/mo_math.egg-info/PKG-INFO` & `mo_math-7.602.24115/mo_math.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-math
-Version: 7.601.24115
+Version: 7.602.24115
 Summary: More Math! Many of the aggregates you are familiar with, but null-safe
 Home-page: https://github.com/klahnakoski/mo-math
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.8
@@ -13,15 +13,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-dots==9.601.24115
+Requires-Dist: mo-dots==9.602.24115
 Requires-Dist: mo-future==7.584.24095
 Provides-Extra: tests
 Requires-Dist: mo-json>=6.589.24111; extra == "tests"
 Requires-Dist: mo-testing>=8.591.24112; extra == "tests"
 
 
 # More Math!
```

### Comparing `mo_math-7.601.24115/mo_math.egg-info/SOURCES.txt` & `mo_math-7.602.24115/mo_math.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mo_math-7.601.24115/setup.py` & `mo_math-7.602.24115/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 setup(
     author='Kyle Lahnakoski',
     author_email='kyle@lahnakoski.com',
     classifiers=["Development Status :: 4 - Beta","Programming Language :: Python :: 3.8","Programming Language :: Python :: 3.9","Topic :: Software Development :: Libraries","Topic :: Software Development :: Libraries :: Python Modules","License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)","Programming Language :: Python :: 3.10","Programming Language :: Python :: 3.11","Programming Language :: Python :: 3.12"],
     description='More Math! Many of the aggregates you are familiar with, but null-safe',
     extras_require={"tests":["mo-json>=6.589.24111","mo-testing>=8.591.24112"]},
     include_package_data=True,
-    install_requires=["mo-dots==9.601.24115","mo-future==7.584.24095"],
+    install_requires=["mo-dots==9.602.24115","mo-future==7.584.24095"],
     license='MPL 2.0',
     long_description="\n# More Math!  \n\nBasic math functions that have been stabilized to act well over `Null`/`None`/`NaN`\n\n\n|Branch      |Status   |\n|------------|---------|\n|master      |  [![Build Status](https://github.com/klahnakoski/mo-math/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/mo-math/actions/workflows/build.yml) |\n|dev         | [![Build Status](https://app.travis-ci.com/klahnakoski/mo-math.svg?branch=dev)](https://travis-ci.com/github/klahnakoski/mo-math)    |\n\n\n\n## Overview\n\nMany of the basic math functions you know and love, with the additional benefit \nthat they do not throw exceptions and do not return `NaN`. \n\nThese functions are all module methods. Be sure you call the functions \nwith `mo_math.` prefix, like \n\n    import mo_math\n\tmo_math.abs(-42)\n\nor rename the functions\n\n    from mo_math import abs as mo_abs\n    mo_abs(-42)\n\nThis prevents confusion with the `__builtin__` functions by the same name   \n\n\n## Functions\n\nFunctions are generally [conservative](https://github.com/mozilla/ActiveData/blob/dev/docs/jx_decisive_operators.md#definitions) in the face of nulls: Specifically, they return `Null` if any of their operands are not a number.\n\nMost functions need no introduction, but some are interesting:\n\n- `round(value, decimal=7, digits=None)` - Rounds to 7 decimal points, unless specified differently.  Rounding to `decimal=0` will return an `int`. The useful parameter here is `digits`, which rounds to a specified number of significant digits.\n- `floor(value, mod=1)` - The `mod`ulo parameter is used to specify the granularity of the floor function.\n- `ceiling(value, mod=1)` - Return the smallest value, that's equal or larger than `value`, with suitable granularity.\n- `mod(value, mod=1)` - Works on floats\n- `approx_str(value)` - Round values, and return `text` (`unicode` in py2, `str` in py3) \n- `sign(v)` - Missing from the Python library \n\n\nThe all-caps aggregate functions accept only one parameter; an iterable. They are [decisive](https://github.com/mozilla/ActiveData/blob/dev/docs/jx_decisive_operators.md#definitions) operators: Non-numbers are ignored, if no values are numbers then the aggregate will return `Null`.\n\n- `COUNT(values)`\n- `SUM(values)` \n- `PRODUCT(values)` \n- `MIN(values)` \n- `MAX(values)` \n\n## Crypto\n\nThe AES and RSA crypto functions provide structured input/output on top of `cryptography` library. The intent is to reveal the signed/encrypted structures so third parties can decode the data.\n",
     long_description_content_type='text/markdown',
     name='mo-math',
     packages=["mo_math.vendor.aespython","mo_math.vendor.strangman","mo_math.vendor","mo_math"],
     url='https://github.com/klahnakoski/mo-math',
-    version='7.601.24115'
+    version='7.602.24115'
 )
```

