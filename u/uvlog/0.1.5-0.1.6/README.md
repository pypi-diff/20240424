# Comparing `tmp/uvlog-0.1.5-py3-none-any.whl.zip` & `tmp/uvlog-0.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,12 @@
-Zip file size: 15648 bytes, number of entries: 9
--rw-r--r--  2.0 unx     1119 b- defN 24-Apr-10 15:47 uvlog/__init__.py
--rw-r--r--  2.0 unx     5340 b- defN 24-Apr-10 15:47 uvlog/formatters.py
--rw-r--r--  2.0 unx     8939 b- defN 24-Apr-10 15:47 uvlog/handlers.py
--rw-r--r--  2.0 unx    20079 b- defN 24-Apr-10 15:47 uvlog/uvlog.py
--rw-r--r--  2.0 unx     1069 b- defN 24-Apr-10 15:47 uvlog-0.1.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     8020 b- defN 24-Apr-10 15:47 uvlog-0.1.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-10 15:47 uvlog-0.1.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 24-Apr-10 15:47 uvlog-0.1.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      671 b- defN 24-Apr-10 15:47 uvlog-0.1.5.dist-info/RECORD
-9 files, 45335 bytes uncompressed, 14510 bytes compressed:  68.0%
+Zip file size: 15794 bytes, number of entries: 10
+-rw-r--r--  2.0 unx     1119 b- defN 24-Apr-24 18:59 uvlog/__init__.py
+-rw-r--r--  2.0 unx     5340 b- defN 24-Apr-24 18:59 uvlog/formatters.py
+-rw-r--r--  2.0 unx     8939 b- defN 24-Apr-24 18:59 uvlog/handlers.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 18:59 uvlog/py.typed
+-rw-r--r--  2.0 unx    20079 b- defN 24-Apr-24 18:59 uvlog/uvlog.py
+-rw-r--r--  2.0 unx     1069 b- defN 24-Apr-24 19:00 uvlog-0.1.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8054 b- defN 24-Apr-24 19:00 uvlog-0.1.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-24 19:00 uvlog-0.1.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 24-Apr-24 19:00 uvlog-0.1.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      739 b- defN 24-Apr-24 19:00 uvlog-0.1.6.dist-info/RECORD
+10 files, 45437 bytes uncompressed, 14552 bytes compressed:  68.0%
```

## zipnote {}

```diff
@@ -3,26 +3,29 @@
 
 Filename: uvlog/formatters.py
 Comment: 
 
 Filename: uvlog/handlers.py
 Comment: 
 
+Filename: uvlog/py.typed
+Comment: 
+
 Filename: uvlog/uvlog.py
 Comment: 
 
-Filename: uvlog-0.1.5.dist-info/LICENSE
+Filename: uvlog-0.1.6.dist-info/LICENSE
 Comment: 
 
-Filename: uvlog-0.1.5.dist-info/METADATA
+Filename: uvlog-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: uvlog-0.1.5.dist-info/WHEEL
+Filename: uvlog-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: uvlog-0.1.5.dist-info/top_level.txt
+Filename: uvlog-0.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: uvlog-0.1.5.dist-info/RECORD
+Filename: uvlog-0.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## uvlog/__init__.py

```diff
@@ -7,15 +7,15 @@
 from uvlog.formatters import *
 from uvlog.handlers import *
 from uvlog.uvlog import *
 
 __python_version__ = "3.8"
 __author__ = "violetblackdev@gmail.com"
 __license__ = "MIT"
-__version__ = "0.1.5"
+__version__ = "0.1.6"
 
 add_formatter_type(TextFormatter)
 add_formatter_type(JSONFormatter)
 add_handler_type(StreamHandler)
 add_handler_type(QueueStreamHandler)
 
 configure(BASIC_CONFIG)
```

## Comparing `uvlog-0.1.5.dist-info/LICENSE` & `uvlog-0.1.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `uvlog-0.1.5.dist-info/METADATA` & `uvlog-0.1.6.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uvlog
-Version: 0.1.5
+Version: 0.1.6
 Summary: Pythonic logger with better performance and contextvars + JSON support out of the box
 Home-page: https://github.com/violet-black/uvlog
 Author: violetblackdev@gmail.com
 License: MIT
 Keywords: logging,logs
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -32,15 +32,16 @@
 Requires-Dist: isort ; extra == 'dev'
 Requires-Dist: black ; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: sphinx ; extra == 'docs'
 Requires-Dist: python-docs-theme ; extra == 'docs'
 Requires-Dist: m2r2 ; extra == 'docs'
 Provides-Extra: test
-Requires-Dist: pytest ==8.1.1 ; extra == 'test'
+Requires-Dist: pytest ; extra == 'test'
+Requires-Dist: coverage ; extra == 'test'
 
 [![pypi](https://img.shields.io/pypi/v/uvlog.svg)](https://pypi.python.org/pypi/uvlog/)
 [![docs](https://readthedocs.org/projects/uvlog/badge/?version=latest&style=flat)](https://uvlog.readthedocs.io)
 [![codecov](https://codecov.io/gh/violet-black/uvlog/graph/badge.svg?token=FEUUMQELFX)](https://codecov.io/gh/violet-black/uvlog)
 [![tests](https://github.com/violet-black/uvlog/actions/workflows/tests.yaml/badge.svg)](https://github.com/violet-black/uvlog/actions/workflows/tests.yaml)
 [![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

