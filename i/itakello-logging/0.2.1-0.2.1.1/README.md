# Comparing `tmp/itakello_logging-0.2.1.tar.gz` & `tmp/itakello_logging-0.2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itakello_logging-0.2.1.tar", last modified: Sat Apr 20 13:01:53 2024, max compression
+gzip compressed data, was "itakello_logging-0.2.1.1.tar", last modified: Wed Apr 24 09:12:33 2024, max compression
```

## Comparing `itakello_logging-0.2.1.tar` & `itakello_logging-0.2.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:01:53.152658 itakello_logging-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-20 13:01:39.000000 itakello_logging-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-20 13:01:53.152658 itakello_logging-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-20 13:01:39.000000 itakello_logging-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 13:01:53.152658 itakello_logging-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-20 13:01:39.000000 itakello_logging-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:01:53.148658 itakello_logging-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:01:53.148658 itakello_logging-0.2.1/src/itakello_logging/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-20 13:01:39.000000 itakello_logging-0.2.1/src/itakello_logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-04-20 13:01:39.000000 itakello_logging-0.2.1/src/itakello_logging/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:01:53.148658 itakello_logging-0.2.1/src/itakello_logging/filters/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-20 13:01:39.000000 itakello_logging-0.2.1/src/itakello_logging/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-20 13:01:39.000000 itakello_logging-0.2.1/src/itakello_logging/filters/custom_exclude.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-20 13:01:39.000000 itakello_logging-0.2.1/src/itakello_logging/filters/ignore_root.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:01:53.148658 itakello_logging-0.2.1/src/itakello_logging/formatters/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 13:01:39.000000 itakello_logging-0.2.1/src/itakello_logging/formatters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-20 13:01:39.000000 itakello_logging-0.2.1/src/itakello_logging/formatters/console.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:01:53.148658 itakello_logging-0.2.1/src/itakello_logging/loggers/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-20 13:01:39.000000 itakello_logging-0.2.1/src/itakello_logging/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-20 13:01:39.000000 itakello_logging-0.2.1/src/itakello_logging/loggers/custom_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:01:53.148658 itakello_logging-0.2.1/src/itakello_logging/test_logs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 13:01:39.000000 itakello_logging-0.2.1/src/itakello_logging/test_logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-20 13:01:39.000000 itakello_logging-0.2.1/src/itakello_logging/test_logs/test_logs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:01:53.152658 itakello_logging-0.2.1/src/itakello_logging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-20 13:01:53.000000 itakello_logging-0.2.1/src/itakello_logging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-20 13:01:53.000000 itakello_logging-0.2.1/src/itakello_logging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 13:01:53.000000 itakello_logging-0.2.1/src/itakello_logging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-20 13:01:53.000000 itakello_logging-0.2.1/src/itakello_logging.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:12:33.976057 itakello_logging-0.2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-24 09:12:23.000000 itakello_logging-0.2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-24 09:12:33.976057 itakello_logging-0.2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-24 09:12:23.000000 itakello_logging-0.2.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 09:12:33.976057 itakello_logging-0.2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-24 09:12:23.000000 itakello_logging-0.2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:12:33.972057 itakello_logging-0.2.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:12:33.972057 itakello_logging-0.2.1.1/src/itakello_logging/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-24 09:12:23.000000 itakello_logging-0.2.1.1/src/itakello_logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-04-24 09:12:23.000000 itakello_logging-0.2.1.1/src/itakello_logging/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:12:33.972057 itakello_logging-0.2.1.1/src/itakello_logging/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-24 09:12:23.000000 itakello_logging-0.2.1.1/src/itakello_logging/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-24 09:12:23.000000 itakello_logging-0.2.1.1/src/itakello_logging/filters/custom_exclude.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-24 09:12:23.000000 itakello_logging-0.2.1.1/src/itakello_logging/filters/ignore_root.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:12:33.972057 itakello_logging-0.2.1.1/src/itakello_logging/formatters/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 09:12:23.000000 itakello_logging-0.2.1.1/src/itakello_logging/formatters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-24 09:12:23.000000 itakello_logging-0.2.1.1/src/itakello_logging/formatters/console.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:12:33.976057 itakello_logging-0.2.1.1/src/itakello_logging/loggers/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-24 09:12:23.000000 itakello_logging-0.2.1.1/src/itakello_logging/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-24 09:12:23.000000 itakello_logging-0.2.1.1/src/itakello_logging/loggers/custom_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:12:33.976057 itakello_logging-0.2.1.1/src/itakello_logging/test_logs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:12:23.000000 itakello_logging-0.2.1.1/src/itakello_logging/test_logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-24 09:12:23.000000 itakello_logging-0.2.1.1/src/itakello_logging/test_logs/test_logs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:12:33.976057 itakello_logging-0.2.1.1/src/itakello_logging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-24 09:12:33.000000 itakello_logging-0.2.1.1/src/itakello_logging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-24 09:12:33.000000 itakello_logging-0.2.1.1/src/itakello_logging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 09:12:33.000000 itakello_logging-0.2.1.1/src/itakello_logging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-24 09:12:33.000000 itakello_logging-0.2.1.1/src/itakello_logging.egg-info/top_level.txt
```

### Comparing `itakello_logging-0.2.1/LICENSE` & `itakello_logging-0.2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `itakello_logging-0.2.1/PKG-INFO` & `itakello_logging-0.2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itakello_logging
-Version: 0.2.1
+Version: 0.2.1.1
 Summary: A custom logging library by Itakello
 Home-page: https://github.com/Itakello/itakello_logging
 Author: Itakello
 Author-email: maxste000@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `itakello_logging-0.2.1/README.md` & `itakello_logging-0.2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `itakello_logging-0.2.1/setup.py` & `itakello_logging-0.2.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="itakello_logging",
-    version="0.2.1",
+    version="0.2.1.1",
     author="Itakello",
     author_email="maxste000@gmail.com",
     description="A custom logging library by Itakello",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Itakello/itakello_logging",
     package_dir={"": "src"},
```

### Comparing `itakello_logging-0.2.1/src/itakello_logging/core.py` & `itakello_logging-0.2.1.1/src/itakello_logging/core.py`

 * *Files identical despite different names*

### Comparing `itakello_logging-0.2.1/src/itakello_logging/formatters/console.py` & `itakello_logging-0.2.1.1/src/itakello_logging/formatters/console.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
     CONFIRMATION_LEVEL = 25
     INSTRUCTION_LEVEL = 24
 
     color_codes = {
         logging.DEBUG: "\033[94m",  # Blue
         CONFIRMATION_LEVEL: "\033[92m",  # Green
-        INSTRUCTION_LEVEL: "\033[33m",  # Orange
+        INSTRUCTION_LEVEL: "\033[36m",  # Orange
         logging.WARNING: "\033[93m",  # Yellow
         logging.ERROR: "\033[91m",  # Red
         logging.CRITICAL: "\033[95m",  # Magenta
     }
 
     def format(self, record):
         level_color = self.color_codes.get(
```

### Comparing `itakello_logging-0.2.1/src/itakello_logging/loggers/custom_logger.py` & `itakello_logging-0.2.1.1/src/itakello_logging/loggers/custom_logger.py`

 * *Files identical despite different names*

### Comparing `itakello_logging-0.2.1/src/itakello_logging.egg-info/PKG-INFO` & `itakello_logging-0.2.1.1/src/itakello_logging.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itakello_logging
-Version: 0.2.1
+Version: 0.2.1.1
 Summary: A custom logging library by Itakello
 Home-page: https://github.com/Itakello/itakello_logging
 Author: Itakello
 Author-email: maxste000@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `itakello_logging-0.2.1/src/itakello_logging.egg-info/SOURCES.txt` & `itakello_logging-0.2.1.1/src/itakello_logging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

