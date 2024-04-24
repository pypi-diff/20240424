# Comparing `tmp/eth-bloom-3.0.0.tar.gz` & `tmp/eth_bloom-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth-bloom-3.0.0.tar", last modified: Mon Oct 30 20:00:57 2023, max compression
+gzip compressed data, was "eth_bloom-3.0.1.tar", last modified: Wed Apr 24 16:01:31 2024, max compression
```

## Comparing `eth-bloom-3.0.0.tar` & `eth_bloom-3.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2023-10-30 20:00:57.762843 eth-bloom-3.0.0/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1095 2023-10-27 21:48:59.000000 eth-bloom-3.0.0/LICENSE
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      168 2023-10-27 21:48:59.000000 eth-bloom-3.0.0/MANIFEST.in
--rw-r--r--   0 pacrob    (1000) pacrob    (1000)     8264 2023-10-30 20:00:57.758843 eth-bloom-3.0.0/PKG-INFO
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     6638 2023-10-27 21:48:59.000000 eth-bloom-3.0.0/README.md
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2023-10-30 20:00:57.758843 eth-bloom-3.0.0/eth_bloom/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      140 2023-10-27 21:48:59.000000 eth-bloom-3.0.0/eth_bloom/__init__.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2959 2023-10-27 21:48:59.000000 eth-bloom-3.0.0/eth_bloom/bloom.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2023-10-27 19:19:57.000000 eth-bloom-3.0.0/eth_bloom/py.typed
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2023-10-30 20:00:57.758843 eth-bloom-3.0.0/eth_bloom.egg-info/
--rw-r--r--   0 pacrob    (1000) pacrob    (1000)     8264 2023-10-30 20:00:57.000000 eth-bloom-3.0.0/eth_bloom.egg-info/PKG-INFO
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      362 2023-10-30 20:00:57.000000 eth-bloom-3.0.0/eth_bloom.egg-info/SOURCES.txt
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        1 2023-10-30 20:00:57.000000 eth-bloom-3.0.0/eth_bloom.egg-info/dependency_links.txt
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        1 2023-10-30 18:46:03.000000 eth-bloom-3.0.0/eth_bloom.egg-info/not-zip-safe
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      276 2023-10-30 20:00:57.000000 eth-bloom-3.0.0/eth_bloom.egg-info/requires.txt
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       10 2023-10-30 20:00:57.000000 eth-bloom-3.0.0/eth_bloom.egg-info/top_level.txt
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3448 2023-10-27 21:48:59.000000 eth-bloom-3.0.0/pyproject.toml
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       38 2023-10-30 20:00:57.762843 eth-bloom-3.0.0/setup.cfg
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1934 2023-10-30 19:57:47.000000 eth-bloom-3.0.0/setup.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2023-10-30 20:00:57.758843 eth-bloom-3.0.0/tests/
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2023-10-30 20:00:57.758843 eth-bloom-3.0.0/tests/core/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       54 2023-10-27 21:48:59.000000 eth-bloom-3.0.0/tests/core/test_import.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5955 2023-10-27 21:48:59.000000 eth-bloom-3.0.0/tests/test_bloom_filter.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-24 16:01:31.630079 eth_bloom-3.0.1/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1095 2024-04-24 15:56:43.000000 eth_bloom-3.0.1/LICENSE
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      168 2024-04-24 15:56:43.000000 eth_bloom-3.0.1/MANIFEST.in
+-rw-r--r--   0 pacrob    (1000) pacrob    (1000)     8309 2024-04-24 16:01:31.630079 eth_bloom-3.0.1/PKG-INFO
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     6632 2024-04-24 15:56:43.000000 eth_bloom-3.0.1/README.md
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-24 16:01:31.630079 eth_bloom-3.0.1/eth_bloom/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      140 2024-04-24 15:56:43.000000 eth_bloom-3.0.1/eth_bloom/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2910 2024-04-24 15:56:43.000000 eth_bloom-3.0.1/eth_bloom/bloom.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2024-04-24 15:56:43.000000 eth_bloom-3.0.1/eth_bloom/py.typed
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-24 16:01:31.630079 eth_bloom-3.0.1/eth_bloom.egg-info/
+-rw-r--r--   0 pacrob    (1000) pacrob    (1000)     8309 2024-04-24 16:01:31.000000 eth_bloom-3.0.1/eth_bloom.egg-info/PKG-INFO
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      379 2024-04-24 16:01:31.000000 eth_bloom-3.0.1/eth_bloom.egg-info/SOURCES.txt
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        1 2024-04-24 16:01:31.000000 eth_bloom-3.0.1/eth_bloom.egg-info/dependency_links.txt
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        1 2024-04-24 15:58:44.000000 eth_bloom-3.0.1/eth_bloom.egg-info/not-zip-safe
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      276 2024-04-24 16:01:31.000000 eth_bloom-3.0.1/eth_bloom.egg-info/requires.txt
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       10 2024-04-24 16:01:31.000000 eth_bloom-3.0.1/eth_bloom.egg-info/top_level.txt
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3444 2024-04-24 15:56:43.000000 eth_bloom-3.0.1/pyproject.toml
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       38 2024-04-24 16:01:31.630079 eth_bloom-3.0.1/setup.cfg
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1960 2024-04-24 16:01:25.000000 eth_bloom-3.0.1/setup.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-24 16:01:31.626079 eth_bloom-3.0.1/tests/
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-24 16:01:31.630079 eth_bloom-3.0.1/tests/core/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5905 2024-04-24 15:56:43.000000 eth_bloom-3.0.1/tests/core/test_bloom_filter.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      103 2024-04-24 15:56:43.000000 eth_bloom-3.0.1/tests/core/test_import_and_version.py
```

### Comparing `eth-bloom-3.0.0/LICENSE` & `eth_bloom-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eth-bloom-3.0.0/PKG-INFO` & `eth_bloom-3.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-bloom
-Version: 3.0.0
+Version: 3.0.1
 Summary: A python implementation of the bloom filter used by Ethereum
 Home-page: https://github.com/ethereum/eth-bloom
 Author: The Ethereum Foundation
 Author-email: snakecharmers@ethereum.org
 License: MIT
 Keywords: ethereum blockchain evm trie merkle
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -12,14 +12,15 @@
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
 Requires-Dist: eth-hash[pycryptodome]>=0.4.0
 Provides-Extra: dev
 Requires-Dist: build>=0.9.0; extra == "dev"
 Requires-Dist: bumpversion>=0.5.3; extra == "dev"
@@ -46,15 +47,15 @@
 [![PyPI version](https://badge.fury.io/py/eth-bloom.svg)](https://badge.fury.io/py/eth-bloom)
 [![Python versions](https://img.shields.io/pypi/pyversions/eth-bloom.svg)](https://pypi.python.org/pypi/eth-bloom)
 
 A python implementation of the bloom filter used by Ethereum.
 
 > This library and repository was previously located at https://github.com/pipermerriam/ethereum-bloom.  It was transferred to the Ethereum foundation github in November 2017 and renamed to `eth-bloom`.  The PyPi package was also renamed from `ethereum-bloom` to \`eth-bloom.
 
-Read more in the documentation below. [View the change log](https://github.com/ethereum/eth-bloom/blob/master/CHANGELOG.rst).
+Read more in the documentation below. [View the change log](https://github.com/ethereum/eth-bloom/blob/main/CHANGELOG.rst).
 
 For more information on what Ethereum Bloom Filters are see [here](what_is_eth-bloom.txt).
 
 ## Quickstart
 
 ```sh
 python -m pip install eth-bloom
@@ -195,14 +196,14 @@
 #### How to bumpversion
 
 The version format for this repo is `{major}.{minor}.{patch}` for stable, and
 `{major}.{minor}.{patch}-{stage}.{devnum}` for unstable (`stage` can be alpha or beta).
 
 To issue the next version in line, specify which part to bump,
 like `make release bump=minor` or `make release bump=devnum`. This is typically done from the
-master branch, except when releasing a beta (in which case the beta is released from master,
+main branch, except when releasing a beta (in which case the beta is released from main,
 and the previous stable branch is released from said branch).
 
 If you are in a beta version, `make release bump=stage` will switch to a stable.
 
 To issue an unstable version when the current version is stable, specify the
 new version explicitly, like `make release bump="--new-version 4.0.0-alpha.1 devnum"`
```

### Comparing `eth-bloom-3.0.0/README.md` & `eth_bloom-3.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [![PyPI version](https://badge.fury.io/py/eth-bloom.svg)](https://badge.fury.io/py/eth-bloom)
 [![Python versions](https://img.shields.io/pypi/pyversions/eth-bloom.svg)](https://pypi.python.org/pypi/eth-bloom)
 
 A python implementation of the bloom filter used by Ethereum.
 
 > This library and repository was previously located at https://github.com/pipermerriam/ethereum-bloom.  It was transferred to the Ethereum foundation github in November 2017 and renamed to `eth-bloom`.  The PyPi package was also renamed from `ethereum-bloom` to \`eth-bloom.
 
-Read more in the documentation below. [View the change log](https://github.com/ethereum/eth-bloom/blob/master/CHANGELOG.rst).
+Read more in the documentation below. [View the change log](https://github.com/ethereum/eth-bloom/blob/main/CHANGELOG.rst).
 
 For more information on what Ethereum Bloom Filters are see [here](what_is_eth-bloom.txt).
 
 ## Quickstart
 
 ```sh
 python -m pip install eth-bloom
@@ -154,14 +154,14 @@
 #### How to bumpversion
 
 The version format for this repo is `{major}.{minor}.{patch}` for stable, and
 `{major}.{minor}.{patch}-{stage}.{devnum}` for unstable (`stage` can be alpha or beta).
 
 To issue the next version in line, specify which part to bump,
 like `make release bump=minor` or `make release bump=devnum`. This is typically done from the
-master branch, except when releasing a beta (in which case the beta is released from master,
+main branch, except when releasing a beta (in which case the beta is released from main,
 and the previous stable branch is released from said branch).
 
 If you are in a beta version, `make release bump=stage` will switch to a stable.
 
 To issue an unstable version when the current version is stable, specify the
 new version explicitly, like `make release bump="--new-version 4.0.0-alpha.1 devnum"`
```

### Comparing `eth-bloom-3.0.0/eth_bloom/bloom.py` & `eth_bloom-3.0.1/eth_bloom/bloom.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-from __future__ import (
-    absolute_import,
-)
-
 import numbers
 import operator
 from typing import (
     TYPE_CHECKING,
     Iterable,
     Union,
 )
```

### Comparing `eth-bloom-3.0.0/eth_bloom.egg-info/PKG-INFO` & `eth_bloom-3.0.1/eth_bloom.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-bloom
-Version: 3.0.0
+Version: 3.0.1
 Summary: A python implementation of the bloom filter used by Ethereum
 Home-page: https://github.com/ethereum/eth-bloom
 Author: The Ethereum Foundation
 Author-email: snakecharmers@ethereum.org
 License: MIT
 Keywords: ethereum blockchain evm trie merkle
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -12,14 +12,15 @@
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
 Requires-Dist: eth-hash[pycryptodome]>=0.4.0
 Provides-Extra: dev
 Requires-Dist: build>=0.9.0; extra == "dev"
 Requires-Dist: bumpversion>=0.5.3; extra == "dev"
@@ -46,15 +47,15 @@
 [![PyPI version](https://badge.fury.io/py/eth-bloom.svg)](https://badge.fury.io/py/eth-bloom)
 [![Python versions](https://img.shields.io/pypi/pyversions/eth-bloom.svg)](https://pypi.python.org/pypi/eth-bloom)
 
 A python implementation of the bloom filter used by Ethereum.
 
 > This library and repository was previously located at https://github.com/pipermerriam/ethereum-bloom.  It was transferred to the Ethereum foundation github in November 2017 and renamed to `eth-bloom`.  The PyPi package was also renamed from `ethereum-bloom` to \`eth-bloom.
 
-Read more in the documentation below. [View the change log](https://github.com/ethereum/eth-bloom/blob/master/CHANGELOG.rst).
+Read more in the documentation below. [View the change log](https://github.com/ethereum/eth-bloom/blob/main/CHANGELOG.rst).
 
 For more information on what Ethereum Bloom Filters are see [here](what_is_eth-bloom.txt).
 
 ## Quickstart
 
 ```sh
 python -m pip install eth-bloom
@@ -195,14 +196,14 @@
 #### How to bumpversion
 
 The version format for this repo is `{major}.{minor}.{patch}` for stable, and
 `{major}.{minor}.{patch}-{stage}.{devnum}` for unstable (`stage` can be alpha or beta).
 
 To issue the next version in line, specify which part to bump,
 like `make release bump=minor` or `make release bump=devnum`. This is typically done from the
-master branch, except when releasing a beta (in which case the beta is released from master,
+main branch, except when releasing a beta (in which case the beta is released from main,
 and the previous stable branch is released from said branch).
 
 If you are in a beta version, `make release bump=stage` will switch to a stable.
 
 To issue an unstable version when the current version is stable, specify the
 new version explicitly, like `make release bump="--new-version 4.0.0-alpha.1 devnum"`
```

### Comparing `eth-bloom-3.0.0/pyproject.toml` & `eth_bloom-3.0.1/pyproject.toml`

 * *Files 12% similar despite different names*

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
 known_first_party = "eth_bloom"
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
@@ -59,20 +61,20 @@
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
+xfail_strict = true
 
 [tool.towncrier]
-# Read https://github.com/ethereum/eth-bloom/blob/master/newsfragments/README.md for instructions
+# Read https://github.com/ethereum/eth-bloom/blob/main/newsfragments/README.md for instructions
 package = "eth_bloom"
 filename = "CHANGELOG.rst"
 directory = "newsfragments"
 underlines = ["-", "~", "^"]
 title_format = "eth-bloom v{version} ({project_date})"
 issue_format = "`#{issue} <https://github.com/ethereum/eth-bloom/issues/{issue}>`__"
```

### Comparing `eth-bloom-3.0.0/setup.py` & `eth_bloom-3.0.1/setup.py`

 * *Files 13% similar despite different names*

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
@@ -31,15 +30,15 @@
 
 with open("./README.md") as readme:
     long_description = readme.read()
 
 setup(
     name="eth-bloom",
     # *IMPORTANT*: Don't manually change the version here. Use the 'bumpversion' utility.
-    version="3.0.0",
+    version="3.0.1",
     description="""A python implementation of the bloom filter used by Ethereum""",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="The Ethereum Foundation",
     author_email="snakecharmers@ethereum.org",
     url="https://github.com/ethereum/eth-bloom",
     include_package_data=True,
@@ -60,9 +59,10 @@
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

### Comparing `eth-bloom-3.0.0/tests/test_bloom_filter.py` & `eth_bloom-3.0.1/tests/core/test_bloom_filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-from __future__ import (
-    unicode_literals,
-)
-
 import itertools
 
 from hypothesis import (
     given,
     settings,
     strategies as st,
 )
```

