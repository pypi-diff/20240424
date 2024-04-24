# Comparing `tmp/logutil-0.1.7.tar.gz` & `tmp/logutil-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logutil-0.1.7.tar", last modified: Tue Apr  9 14:00:50 2024, max compression
+gzip compressed data, was "logutil-0.1.8.tar", max compression
```

## Comparing `logutil-0.1.7.tar` & `logutil-0.1.8.tar`

### file list

```diff
@@ -1,23 +1,8 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:00:50.969852 logutil-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-09 14:00:40.000000 logutil-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-09 14:00:50.969852 logutil-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-09 14:00:40.000000 logutil-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:00:50.965852 logutil-0.1.7/logutil/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-09 14:00:40.000000 logutil-0.1.7/logutil/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:00:50.969852 logutil-0.1.7/logutil/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:00:40.000000 logutil-0.1.7/logutil/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-09 14:00:40.000000 logutil-0.1.7/logutil/src/init_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-09 14:00:40.000000 logutil-0.1.7/logutil/src/init_loguru.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:00:50.965852 logutil-0.1.7/logutil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-09 14:00:50.000000 logutil-0.1.7/logutil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-09 14:00:50.000000 logutil-0.1.7/logutil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:00:50.000000 logutil-0.1.7/logutil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-09 14:00:50.000000 logutil-0.1.7/logutil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-09 14:00:50.000000 logutil-0.1.7/logutil.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-09 14:00:40.000000 logutil-0.1.7/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1197 2024-04-09 14:00:50.969852 logutil-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-09 14:00:40.000000 logutil-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:00:50.969852 logutil-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:00:40.000000 logutil-0.1.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:00:40.000000 logutil-0.1.7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-09 14:00:40.000000 logutil-0.1.7/tests/test_core.py
+-rw-r--r--   0        0        0    11357 2024-04-24 09:24:00.675216 logutil-0.1.8/LICENSE
+-rw-r--r--   0        0        0     1552 2024-04-24 09:24:00.675216 logutil-0.1.8/README.md
+-rw-r--r--   0        0        0      165 2024-04-24 09:24:00.675216 logutil-0.1.8/logutil/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 09:24:00.675216 logutil-0.1.8/logutil/src/__init__.py
+-rw-r--r--   0        0        0     4542 2024-04-24 09:24:00.675216 logutil-0.1.8/logutil/src/init_logging.py
+-rw-r--r--   0        0        0     4764 2024-04-24 09:24:00.675216 logutil-0.1.8/logutil/src/init_loguru.py
+-rw-r--r--   0        0        0     1327 2024-04-24 09:24:26.135186 logutil-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2184 1970-01-01 00:00:00.000000 logutil-0.1.8/PKG-INFO
```

### Comparing `logutil-0.1.7/LICENSE` & `logutil-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `logutil-0.1.7/PKG-INFO` & `logutil-0.1.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,87 +1,81 @@
 Metadata-Version: 2.1
 Name: logutil
-Version: 0.1.7
+Version: 0.1.8
 Summary: Easy initialization of standard python logging and loguru
-Home-page: UNKNOWN
-Author: Yaroslav Kopotilov
-Author-email: datascience@tuta.io
 License: Apache License, Version 2.0
-Description: # Logutil
-        
-        (Extremely) easy initialization for `logging` and `loguru`
-        
-        ## Why
-        
-        This packages makes it (extremely) easy to send `logging` and `loguru` logs to 
-        - streams
-        - files
-        - sentry
-        - pushover
-        - slack
-        
-        ## Installation
-        
-        - Logging only: `pip install logutil`
-        - ... + loguru: `pip install logutil[loguru]`
-        - ... + pushover/sentry/slack: `pip install logutil[notifiers]`
-        - ... + loguru + pushover/sentry/slack: `pip install logutil[all]`
-        
-        ## Examples
-        
-        ### Standard python logging
-        
-        ```python
-        from logutil import init_logging, get_logging_logger
-        init_logging(
-            name='data_feeds',
-            sentry_on=True,
-            sentry_dsn='<your sentry dsn string>',
-            sentry_breadcramp_level='INFO',
-            sentry_event_level='WARNING',
-        )
-        logger = get_logging_logger('data_feeds')
-        logger.info('Test INFO message (logging)')
-        logger.warning('Test WARNING message (logging)')
-        ```
-        ```
-        2020-07-19T12:59:18.740Z data_feeds INFO: Test INFO message (logging)
-        2020-07-19T12:59:18.740Z data_feeds WARNING: Test WARNING message (logging)
-        ```
-        
-        ### Loguru
-        
-        ```python
-        from logutil import init_loguru, get_loguru_logger
-        init_loguru()
-        logger = get_loguru_logger(
-            slack_on=True,
-            slack_level='WARNING',
-            slack_webhook_url='<your slack app webhook url string>',
-        )
-        logger.info('Test INFO message (loguru)')
-        logger.warning('Test WARNING message (loguru)')
-        ```
-        ```
-        2020-07-19T12:56:20.771Z __main__ INFO: Test INFO message (loguru)
-        2020-07-19T12:56:20.771Z __main__ WARNING: Test WARNING message (loguru)
-        ```
-        
-        ## Notes
-        
-        - Formatting is ignored for `sentry` notifications with `logging`
-        
-Keywords: logging loguru
-Platform: UNKNOWN
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
+Author: Mysterious Ben
+Author-email: datascience@tuta.io
+Requires-Python: >=3.8,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
-Provides-Extra: loguru
-Provides-Extra: notifiers
-Provides-Extra: all
+
+# Logutil
+
+(Extremely) easy initialization for `logging` and `loguru`
+
+## Why
+
+This packages makes it (extremely) easy to send `logging` and `loguru` logs to 
+- streams
+- files
+- sentry
+- pushover
+- slack
+
+## Installation
+
+- Logging only: `pip install logutil`
+- ... + loguru: `pip install logutil[loguru]`
+- ... + pushover/sentry/slack: `pip install logutil[notifiers]`
+- ... + loguru + pushover/sentry/slack: `pip install logutil[all]`
+
+## Examples
+
+### Standard python logging
+
+```python
+from logutil import init_logging, get_logging_logger
+init_logging(
+    name='data_feeds',
+    sentry_on=True,
+    sentry_dsn='<your sentry dsn string>',
+    sentry_breadcramp_level='INFO',
+    sentry_event_level='WARNING',
+)
+logger = get_logging_logger('data_feeds')
+logger.info('Test INFO message (logging)')
+logger.warning('Test WARNING message (logging)')
+```
+```
+2020-07-19T12:59:18.740Z data_feeds INFO: Test INFO message (logging)
+2020-07-19T12:59:18.740Z data_feeds WARNING: Test WARNING message (logging)
+```
+
+### Loguru
+
+```python
+from logutil import init_loguru, get_loguru_logger
+init_loguru()
+logger = get_loguru_logger(
+    slack_on=True,
+    slack_level='WARNING',
+    slack_webhook_url='<your slack app webhook url string>',
+)
+logger.info('Test INFO message (loguru)')
+logger.warning('Test WARNING message (loguru)')
+```
+```
+2020-07-19T12:56:20.771Z __main__ INFO: Test INFO message (loguru)
+2020-07-19T12:56:20.771Z __main__ WARNING: Test WARNING message (loguru)
+```
+
+## Notes
+
+- Formatting is ignored for `sentry` notifications with `logging`
+
```

### Comparing `logutil-0.1.7/README.md` & `logutil-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `logutil-0.1.7/logutil/src/init_logging.py` & `logutil-0.1.8/logutil/src/init_logging.py`

 * *Files identical despite different names*

### Comparing `logutil-0.1.7/logutil/src/init_loguru.py` & `logutil-0.1.8/logutil/src/init_loguru.py`

 * *Files identical despite different names*

### Comparing `logutil-0.1.7/pyproject.toml` & `logutil-0.1.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 [tool.poetry]
 name = "logutil"
-version = "0.1.7"
+version = "0.1.8"
 description = "Easy initialization of standard python logging and loguru"
 authors = ["Mysterious Ben <datascience@tuta.io>"]
 license = "Apache License, Version 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 [tool.poetry.group.loguru.dependencies]
-loguru = "^0.5.3"
+loguru = "^0.5"
 
 [tool.poetry.group.notifiers.dependencies]
-notifiers = "^1.2.1"
-sentry-sdk = "^1.3.1"
+notifiers = "^1.2"
+sentry-sdk = "^1.3"
 
 [tool.poetry.group.all.dependencies]
-loguru = "^0.5.3"
-notifiers = "^1.2.1"
-sentry-sdk = "^1.3.1"
+loguru = "^0.5"
+notifiers = "^1.2"
+sentry-sdk = "^1.3"
 
 [tool.poetry.group.dev.dependencies]
-ruff = "^0.3.5"
-mypy = "^1.9.0"
-pylint = "^3.1.0"
-black = "^24.3.0"
-pytest = "^8.1.1"
-pre-commit = "^3.5.0"
-isort = "^5.13.2"
+ruff = "^0.3"
+mypy = ">=0.910"
+pylint = "^3.1"
+black = "^24.3"
+pytest = "^8"
+pre-commit = "^3.5"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.black]
```

