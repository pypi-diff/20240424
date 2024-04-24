# Comparing `tmp/pmss-0.0.1.tar.gz` & `tmp/pmss-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pmss-0.0.1.tar", last modified: Wed Apr 24 15:27:11 2024, max compression
+gzip compressed data, was "pmss-0.0.2.tar", last modified: Wed Apr 24 18:44:17 2024, max compression
```

## Comparing `pmss-0.0.1.tar` & `pmss-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxrwxr-x   0 pmitros   (1000) pmitros   (1000)        0 2024-04-24 15:27:11.849949 pmss-0.0.1/
--rw-r--r--   0 pmitros   (1000) pmitros   (1000)     9587 2024-04-24 15:27:11.849949 pmss-0.0.1/PKG-INFO
--rw-rw-r--   0 pmitros   (1000) pmitros   (1000)     9170 2024-04-24 15:06:49.000000 pmss-0.0.1/README.md
-drwxrwxr-x   0 pmitros   (1000) pmitros   (1000)        0 2024-04-24 15:27:11.849949 pmss-0.0.1/pmss/
--rw-rw-r--   0 pmitros   (1000) pmitros   (1000)      342 2024-04-24 15:06:49.000000 pmss-0.0.1/pmss/__init__.py
--rw-rw-r--   0 pmitros   (1000) pmitros   (1000)     2886 2024-04-24 15:06:49.000000 pmss-0.0.1/pmss/functional.py
--rw-rw-r--   0 pmitros   (1000) pmitros   (1000)     2277 2024-04-24 15:06:49.000000 pmss-0.0.1/pmss/loadfile.py
--rw-rw-r--   0 pmitros   (1000) pmitros   (1000)     3037 2024-04-24 15:09:17.000000 pmss-0.0.1/pmss/parsetab.py
--rw-rw-r--   0 pmitros   (1000) pmitros   (1000)     1922 2024-04-24 15:06:49.000000 pmss-0.0.1/pmss/pathfinder.py
--rw-rw-r--   0 pmitros   (1000) pmitros   (1000)     2191 2024-04-24 15:06:49.000000 pmss-0.0.1/pmss/pmsslex.py
--rw-rw-r--   0 pmitros   (1000) pmitros   (1000)    11950 2024-04-24 15:06:49.000000 pmss-0.0.1/pmss/pmssselectors.py
--rw-rw-r--   0 pmitros   (1000) pmitros   (1000)     9360 2024-04-24 15:06:49.000000 pmss-0.0.1/pmss/pmsstypes.py
--rw-rw-r--   0 pmitros   (1000) pmitros   (1000)     1728 2024-04-24 15:06:49.000000 pmss-0.0.1/pmss/pmssyacc.py
--rw-rw-r--   0 pmitros   (1000) pmitros   (1000)     2497 2024-04-24 15:06:49.000000 pmss-0.0.1/pmss/pretty_usage.py
--rw-rw-r--   0 pmitros   (1000) pmitros   (1000)      515 2024-04-24 15:06:49.000000 pmss-0.0.1/pmss/priority.py
--rw-rw-r--   0 pmitros   (1000) pmitros   (1000)    13696 2024-04-24 15:06:49.000000 pmss-0.0.1/pmss/rulesets.py
--rw-rw-r--   0 pmitros   (1000) pmitros   (1000)     6890 2024-04-24 15:06:49.000000 pmss-0.0.1/pmss/schema.py
--rw-rw-r--   0 pmitros   (1000) pmitros   (1000)     2054 2024-04-24 15:06:49.000000 pmss-0.0.1/pmss/settings.py
--rw-rw-r--   0 pmitros   (1000) pmitros   (1000)     1127 2024-04-24 15:06:49.000000 pmss-0.0.1/pmss/util.py
-drwxrwxr-x   0 pmitros   (1000) pmitros   (1000)        0 2024-04-24 15:27:11.849949 pmss-0.0.1/pmss.egg-info/
--rw-r--r--   0 pmitros   (1000) pmitros   (1000)     9587 2024-04-24 15:27:11.000000 pmss-0.0.1/pmss.egg-info/PKG-INFO
--rw-rw-r--   0 pmitros   (1000) pmitros   (1000)      425 2024-04-24 15:27:11.000000 pmss-0.0.1/pmss.egg-info/SOURCES.txt
--rw-rw-r--   0 pmitros   (1000) pmitros   (1000)        1 2024-04-24 15:27:11.000000 pmss-0.0.1/pmss.egg-info/dependency_links.txt
--rw-rw-r--   0 pmitros   (1000) pmitros   (1000)        4 2024-04-24 15:27:11.000000 pmss-0.0.1/pmss.egg-info/requires.txt
--rw-rw-r--   0 pmitros   (1000) pmitros   (1000)        5 2024-04-24 15:27:11.000000 pmss-0.0.1/pmss.egg-info/top_level.txt
--rw-rw-r--   0 pmitros   (1000) pmitros   (1000)      536 2024-04-24 15:10:23.000000 pmss-0.0.1/pyproject.toml
--rw-rw-r--   0 pmitros   (1000) pmitros   (1000)       38 2024-04-24 15:27:11.849949 pmss-0.0.1/setup.cfg
+drwxrwxr-x   0 brad      (1000) brad      (1000)        0 2024-04-24 18:44:17.261530 pmss-0.0.2/
+-rw-r--r--   0 brad      (1000) brad      (1000)     9587 2024-04-24 18:44:17.261530 pmss-0.0.2/PKG-INFO
+-rw-rw-r--   0 brad      (1000) brad      (1000)     9170 2024-04-24 15:59:15.000000 pmss-0.0.2/README.md
+drwxrwxr-x   0 brad      (1000) brad      (1000)        0 2024-04-24 18:44:17.261530 pmss-0.0.2/pmss/
+-rw-rw-r--   0 brad      (1000) brad      (1000)      342 2024-04-24 15:59:15.000000 pmss-0.0.2/pmss/__init__.py
+-rw-rw-r--   0 brad      (1000) brad      (1000)     2886 2024-04-24 15:59:15.000000 pmss-0.0.2/pmss/functional.py
+-rw-rw-r--   0 brad      (1000) brad      (1000)     2277 2024-04-24 15:59:15.000000 pmss-0.0.2/pmss/loadfile.py
+-rw-rw-r--   0 brad      (1000) brad      (1000)     1922 2024-04-24 15:59:15.000000 pmss-0.0.2/pmss/pathfinder.py
+-rw-rw-r--   0 brad      (1000) brad      (1000)     2191 2024-04-24 15:59:15.000000 pmss-0.0.2/pmss/pmsslex.py
+-rw-rw-r--   0 brad      (1000) brad      (1000)    11950 2024-04-24 15:59:15.000000 pmss-0.0.2/pmss/pmssselectors.py
+-rw-rw-r--   0 brad      (1000) brad      (1000)    10655 2024-04-24 15:59:15.000000 pmss-0.0.2/pmss/pmsstypes.py
+-rw-rw-r--   0 brad      (1000) brad      (1000)     1728 2024-04-24 15:59:15.000000 pmss-0.0.2/pmss/pmssyacc.py
+-rw-rw-r--   0 brad      (1000) brad      (1000)     2497 2024-04-24 15:59:15.000000 pmss-0.0.2/pmss/pretty_usage.py
+-rw-rw-r--   0 brad      (1000) brad      (1000)      515 2024-04-24 15:59:15.000000 pmss-0.0.2/pmss/priority.py
+-rw-rw-r--   0 brad      (1000) brad      (1000)    13696 2024-04-24 15:59:15.000000 pmss-0.0.2/pmss/rulesets.py
+-rw-rw-r--   0 brad      (1000) brad      (1000)     6890 2024-04-24 15:59:15.000000 pmss-0.0.2/pmss/schema.py
+-rw-rw-r--   0 brad      (1000) brad      (1000)     2054 2024-04-24 15:59:15.000000 pmss-0.0.2/pmss/settings.py
+-rw-rw-r--   0 brad      (1000) brad      (1000)     1127 2024-04-24 15:59:15.000000 pmss-0.0.2/pmss/util.py
+drwxrwxr-x   0 brad      (1000) brad      (1000)        0 2024-04-24 18:44:17.261530 pmss-0.0.2/pmss.egg-info/
+-rw-r--r--   0 brad      (1000) brad      (1000)     9587 2024-04-24 18:44:17.000000 pmss-0.0.2/pmss.egg-info/PKG-INFO
+-rw-rw-r--   0 brad      (1000) brad      (1000)      408 2024-04-24 18:44:17.000000 pmss-0.0.2/pmss.egg-info/SOURCES.txt
+-rw-rw-r--   0 brad      (1000) brad      (1000)        1 2024-04-24 18:44:17.000000 pmss-0.0.2/pmss.egg-info/dependency_links.txt
+-rw-rw-r--   0 brad      (1000) brad      (1000)        4 2024-04-24 18:44:17.000000 pmss-0.0.2/pmss.egg-info/requires.txt
+-rw-rw-r--   0 brad      (1000) brad      (1000)        5 2024-04-24 18:44:17.000000 pmss-0.0.2/pmss.egg-info/top_level.txt
+-rw-rw-r--   0 brad      (1000) brad      (1000)      536 2024-04-24 18:43:42.000000 pmss-0.0.2/pyproject.toml
+-rw-rw-r--   0 brad      (1000) brad      (1000)       38 2024-04-24 18:44:17.261530 pmss-0.0.2/setup.cfg
```

### Comparing `pmss-0.0.1/PKG-INFO` & `pmss-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmss
-Version: 0.0.1
+Version: 0.0.2
 Summary: Cascading Python settings
 Author-email: Piotr Mitros <piotr@mitros.org>
 Project-URL: Homepage, https://github.com/ETS-Nextgen/pmss
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `pmss-0.0.1/README.md` & `pmss-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pmss-0.0.1/pmss/functional.py` & `pmss-0.0.2/pmss/functional.py`

 * *Files identical despite different names*

### Comparing `pmss-0.0.1/pmss/loadfile.py` & `pmss-0.0.2/pmss/loadfile.py`

 * *Files identical despite different names*

### Comparing `pmss-0.0.1/pmss/pathfinder.py` & `pmss-0.0.2/pmss/pathfinder.py`

 * *Files identical despite different names*

### Comparing `pmss-0.0.1/pmss/pmsslex.py` & `pmss-0.0.2/pmss/pmsslex.py`

 * *Files identical despite different names*

### Comparing `pmss-0.0.1/pmss/pmssselectors.py` & `pmss-0.0.2/pmss/pmssselectors.py`

 * *Files identical despite different names*

### Comparing `pmss-0.0.1/pmss/pmsstypes.py` & `pmss-0.0.2/pmss/pmsstypes.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,21 +17,22 @@
 '''
 
 
 import configparser
 import collections
 import doctest
 import datetime
+import enum
+import functools
 import math
 import os.path
 import re
 
 _TYPES_DICT = collections.defaultdict(dict)
 
-
 class DictEnum:
     def __init__(self, d):
         self.d = d
 
     def __getattr__(self, attr):
         '''
         Just the string.
@@ -81,40 +82,72 @@
     >>> parse("/f1aa1.xza", TYPES.filename, {"exists": True})
     Traceback (most recent call last):
     ...
     ValueError: File does not exist: /f1aa1.xza (/f1aa1.xza)
     '''
     return TYPES[pmsstype]['parser'](value, **extra_args)
 
+
+class TransformType(enum.Enum):
+    Decorator = 'Decorator'
+
+
 def parser(
         type_name,
         validation_regexp=None,
         min=None,
         max=None,
         parent=None,
-        choices=None
+        choices=None,
+        transform=TransformType.Decorator
 ):
-    def inner(func):
+    '''We want to be able to call the parser as both a
+    decorator and call it without including a function.
+
+    We initially set the `type_name` parser to be an identity
+    function (or the passed in `transform` function). If this
+    function is being used as a decorator, we overwrite the
+    parser with the decorated function.
+
+    Additionally, we use a closure so we can validate (check
+    the regex, min, max, choices, etc.) the output of
+    whatever function is used for the parser.
+
+    NOTE: the `transform` parameter will do nothing (gets
+    overwritten) when this function is called as a decorator
+    '''
+    def validate_value(value_function):
         def new_func(value, **kwargs):
             if validation_regexp and isinstance(value, str):
                 if not re.match(validation_regexp, value):
                     raise ValueError(f"Value '{value}' does not match the required pattern {validation_regexp})")
             if parent:
                 value = _TYPES_DICT[parent]['parser'](value)
-            parsed = func(value, **kwargs)
+            parsed = value_function(value, **kwargs)
             if min is not None and parsed < min:
                 raise ValueError(f"Value '{value}' ('{parsed}') is less than {min}")
             if max is not None and parsed > max:
                 raise ValueError(f"Value '{value}' ('{parsed}') is more than {max}")
             if choices is not None and value not in choices:
                 raise ValueError(f"Value '{value}' ('{parsed}') is not a valid option for {type_name}. Available choices: {choices}")
             return parsed
-
-        _TYPES_DICT[type_name]['parser'] = new_func
         return new_func
+
+    def inner(func):
+        _TYPES_DICT[type_name]['parser'] = validate_value(func)
+        @functools.wraps(func)
+        def wrapper(*args, **kwargs):
+            return func(*args, **kwargs)
+        return wrapper
+
+    if transform != TransformType.Decorator:
+        transformation_func = transform if transform is not None else lambda val: val
+        if not callable(transformation_func):
+            raise TypeError('The transform paramter must be a callable function.')
+        _TYPES_DICT[type_name]['parser'] = validate_value(transformation_func)
     return inner
 
 @parser("string")
 def _convert_to_string(value):
     return str(value)
 
 @parser("boolean")
```

### Comparing `pmss-0.0.1/pmss/pmssyacc.py` & `pmss-0.0.2/pmss/pmssyacc.py`

 * *Files identical despite different names*

### Comparing `pmss-0.0.1/pmss/pretty_usage.py` & `pmss-0.0.2/pmss/pretty_usage.py`

 * *Files identical despite different names*

### Comparing `pmss-0.0.1/pmss/priority.py` & `pmss-0.0.2/pmss/priority.py`

 * *Files identical despite different names*

### Comparing `pmss-0.0.1/pmss/rulesets.py` & `pmss-0.0.2/pmss/rulesets.py`

 * *Files identical despite different names*

### Comparing `pmss-0.0.1/pmss/schema.py` & `pmss-0.0.2/pmss/schema.py`

 * *Files identical despite different names*

### Comparing `pmss-0.0.1/pmss/settings.py` & `pmss-0.0.2/pmss/settings.py`

 * *Files identical despite different names*

### Comparing `pmss-0.0.1/pmss/util.py` & `pmss-0.0.2/pmss/util.py`

 * *Files identical despite different names*

### Comparing `pmss-0.0.1/pmss.egg-info/PKG-INFO` & `pmss-0.0.2/pmss.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmss
-Version: 0.0.1
+Version: 0.0.2
 Summary: Cascading Python settings
 Author-email: Piotr Mitros <piotr@mitros.org>
 Project-URL: Homepage, https://github.com/ETS-Nextgen/pmss
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `pmss-0.0.1/pyproject.toml` & `pmss-0.0.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pmss"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Piotr Mitros", email="piotr@mitros.org" },
 ]
 description = "Cascading Python settings"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

