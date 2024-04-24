# Comparing `tmp/setech-1.2.1.tar.gz` & `tmp/setech-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setech-1.2.1.tar", last modified: Tue Apr 16 11:12:15 2024, max compression
+gzip compressed data, was "setech-1.3.0.tar", last modified: Wed Apr 24 12:15:38 2024, max compression
```

## Comparing `setech-1.2.1.tar` & `setech-1.3.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-16 11:12:15.919209 setech-1.2.1/
--rw-r--r--   0 eriks     (1000) eriks     (1000)     1059 2024-04-03 10:57:10.000000 setech-1.2.1/LICENCE
--rw-r--r--   0 eriks     (1000) eriks     (1000)     5345 2024-04-16 11:12:15.919209 setech-1.2.1/PKG-INFO
--rw-r--r--   0 eriks     (1000) eriks     (1000)     4473 2024-04-03 21:15:13.000000 setech-1.2.1/README.md
--rw-r--r--   0 eriks     (1000) eriks     (1000)     1912 2024-04-16 11:12:09.000000 setech-1.2.1/pyproject.toml
--rw-r--r--   0 eriks     (1000) eriks     (1000)       38 2024-04-16 11:12:15.919209 setech-1.2.1/setup.cfg
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-16 11:12:15.915876 setech-1.2.1/src/
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-16 11:12:15.915876 setech-1.2.1/src/setech/
--rw-r--r--   0 eriks     (1000) eriks     (1000)      117 2024-04-16 11:12:09.000000 setech-1.2.1/src/setech/__init__.py
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-16 11:12:15.915876 setech-1.2.1/src/setech/api_client/
--rw-r--r--   0 eriks     (1000) eriks     (1000)      115 2024-04-03 13:03:49.000000 setech-1.2.1/src/setech/api_client/__init__.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     6368 2024-04-16 11:12:02.000000 setech-1.2.1/src/setech/api_client/_base.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     2332 2024-04-16 11:12:02.000000 setech-1.2.1/src/setech/api_client/async_client.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     2237 2024-04-16 11:12:02.000000 setech-1.2.1/src/setech/api_client/sync_client.py
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-16 11:12:15.919209 setech-1.2.1/src/setech/constants/
--rw-r--r--   0 eriks     (1000) eriks     (1000)      125 2024-04-03 14:55:19.000000 setech-1.2.1/src/setech/constants/__init__.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)      519 2024-04-03 14:22:18.000000 setech-1.2.1/src/setech/constants/date.py
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-16 11:12:15.919209 setech-1.2.1/src/setech/logging/
--rw-r--r--   0 eriks     (1000) eriks     (1000)      138 2024-04-10 13:57:32.000000 setech-1.2.1/src/setech/logging/__init__.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     1394 2024-04-03 20:53:03.000000 setech-1.2.1/src/setech/logging/formatters.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     1718 2024-04-04 13:24:48.000000 setech-1.2.1/src/setech/logging/handlers.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)        0 2024-03-19 14:21:21.000000 setech-1.2.1/src/setech/py.typed
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-16 11:12:15.919209 setech-1.2.1/src/setech/utils/
--rw-r--r--   0 eriks     (1000) eriks     (1000)     1058 2024-04-16 11:12:02.000000 setech-1.2.1/src/setech/utils/__init__.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)      878 2024-04-16 11:12:02.000000 setech-1.2.1/src/setech/utils/numeric.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     3954 2024-04-16 11:12:02.000000 setech-1.2.1/src/setech/utils/parse.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     5598 2024-04-10 13:57:32.000000 setech-1.2.1/src/setech/utils/ssn.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     1097 2024-04-03 14:55:19.000000 setech-1.2.1/src/setech/utils/text.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     1034 2024-04-12 10:20:23.000000 setech-1.2.1/src/setech/utils/validators.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)      324 2024-04-16 11:12:02.000000 setech-1.2.1/src/setech/utils/various.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     1204 2024-04-16 11:12:02.000000 setech-1.2.1/src/setech/utils/warnings.py
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-16 11:12:15.919209 setech-1.2.1/src/setech.egg-info/
--rw-r--r--   0 eriks     (1000) eriks     (1000)     5345 2024-04-16 11:12:15.000000 setech-1.2.1/src/setech.egg-info/PKG-INFO
--rw-r--r--   0 eriks     (1000) eriks     (1000)      761 2024-04-16 11:12:15.000000 setech-1.2.1/src/setech.egg-info/SOURCES.txt
--rw-r--r--   0 eriks     (1000) eriks     (1000)        1 2024-04-16 11:12:15.000000 setech-1.2.1/src/setech.egg-info/dependency_links.txt
--rw-r--r--   0 eriks     (1000) eriks     (1000)       50 2024-04-16 11:12:15.000000 setech-1.2.1/src/setech.egg-info/requires.txt
--rw-r--r--   0 eriks     (1000) eriks     (1000)        7 2024-04-16 11:12:15.000000 setech-1.2.1/src/setech.egg-info/top_level.txt
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-24 12:15:38.740177 setech-1.3.0/
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     1059 2024-04-03 10:57:10.000000 setech-1.3.0/LICENCE
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     5375 2024-04-24 12:15:38.740177 setech-1.3.0/PKG-INFO
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     4473 2024-04-03 21:15:13.000000 setech-1.3.0/README.md
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     1932 2024-04-24 12:15:32.000000 setech-1.3.0/pyproject.toml
+-rw-r--r--   0 eriks     (1000) eriks     (1000)       38 2024-04-24 12:15:38.740177 setech-1.3.0/setup.cfg
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-24 12:15:38.736844 setech-1.3.0/src/
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-24 12:15:38.740177 setech-1.3.0/src/setech/
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      117 2024-04-24 12:15:32.000000 setech-1.3.0/src/setech/__init__.py
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-24 12:15:38.740177 setech-1.3.0/src/setech/api_client/
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      115 2024-04-03 13:03:49.000000 setech-1.3.0/src/setech/api_client/__init__.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     6368 2024-04-16 11:12:02.000000 setech-1.3.0/src/setech/api_client/_base.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     2332 2024-04-16 11:12:02.000000 setech-1.3.0/src/setech/api_client/async_client.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     2237 2024-04-16 11:12:02.000000 setech-1.3.0/src/setech/api_client/sync_client.py
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-24 12:15:38.740177 setech-1.3.0/src/setech/constants/
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      125 2024-04-24 12:12:00.000000 setech-1.3.0/src/setech/constants/__init__.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      519 2024-04-24 12:12:00.000000 setech-1.3.0/src/setech/constants/date.py
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-24 12:15:38.740177 setech-1.3.0/src/setech/logging/
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      138 2024-04-10 13:57:32.000000 setech-1.3.0/src/setech/logging/__init__.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     1394 2024-04-03 20:53:03.000000 setech-1.3.0/src/setech/logging/formatters.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     1718 2024-04-04 13:24:48.000000 setech-1.3.0/src/setech/logging/handlers.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)        0 2024-03-19 14:21:21.000000 setech-1.3.0/src/setech/py.typed
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-24 12:15:38.740177 setech-1.3.0/src/setech/utils/
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     1276 2024-04-24 12:12:00.000000 setech-1.3.0/src/setech/utils/__init__.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      878 2024-04-16 11:12:02.000000 setech-1.3.0/src/setech/utils/numeric.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     4031 2024-04-24 12:12:00.000000 setech-1.3.0/src/setech/utils/parse.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     5634 2024-04-24 12:12:00.000000 setech-1.3.0/src/setech/utils/ssn.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     2140 2024-04-24 12:12:00.000000 setech-1.3.0/src/setech/utils/text.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      264 2024-04-24 12:12:00.000000 setech-1.3.0/src/setech/utils/time.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     1082 2024-04-24 12:12:00.000000 setech-1.3.0/src/setech/utils/validators.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      318 2024-04-24 12:12:00.000000 setech-1.3.0/src/setech/utils/various.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     1336 2024-04-24 12:12:00.000000 setech-1.3.0/src/setech/utils/warnings.py
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-24 12:15:38.740177 setech-1.3.0/src/setech.egg-info/
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     5375 2024-04-24 12:15:38.000000 setech-1.3.0/src/setech.egg-info/PKG-INFO
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      786 2024-04-24 12:15:38.000000 setech-1.3.0/src/setech.egg-info/SOURCES.txt
+-rw-r--r--   0 eriks     (1000) eriks     (1000)        1 2024-04-24 12:15:38.000000 setech-1.3.0/src/setech.egg-info/dependency_links.txt
+-rw-r--r--   0 eriks     (1000) eriks     (1000)       65 2024-04-24 12:15:38.000000 setech-1.3.0/src/setech.egg-info/requires.txt
+-rw-r--r--   0 eriks     (1000) eriks     (1000)        7 2024-04-24 12:15:38.000000 setech-1.3.0/src/setech.egg-info/top_level.txt
```

### Comparing `setech-1.2.1/LICENCE` & `setech-1.3.0/LICENCE`

 * *Files identical despite different names*

### Comparing `setech-1.2.1/PKG-INFO` & `setech-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setech
-Version: 1.2.1
+Version: 1.3.0
 Summary: Setech utilities
 Author-email: Eriks Karls <eriks.karls@sefinance.lv>
 Project-URL: Homepage, https://pypi.org/project/setech/
 Keywords: setech,logging,api-client,utility,utils
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -16,14 +16,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 License-File: LICENCE
 Requires-Dist: httpx[http2]~=0.27.0
 Requires-Dist: pydantic~=2.6
 Requires-Dist: num2words~=0.5
+Requires-Dist: unidecode~=1.3
 
 # Example code
 ```python
 # client.py
 from setech import SyncClient
```

### Comparing `setech-1.2.1/README.md` & `setech-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `setech-1.2.1/pyproject.toml` & `setech-1.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -23,28 +23,29 @@
   "Programming Language :: Python :: 3 :: Only",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 dependencies = [
   "httpx[http2]~=0.27.0",
   "pydantic~=2.6",
-  "num2words~=0.5"
+  "num2words~=0.5",
+  "unidecode~=1.3"
 ]
 
 
 [project.urls]
 "Homepage" = "https://pypi.org/project/setech/"
 
 
 [tool.setuptools.dynamic]
 version = { attr = "setech.__version__" }
 
 
 [tool.bumpversion]
-current_version = "1.2.1"
+current_version = "1.3.0"
 commit = true
 tag = true
 tag_name = "v{new_version}"
 tag_message = "Bump version: {current_version} → {new_version}"
 allow_dirty = false
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
 serialize = ["{major}.{minor}.{patch}"]
```

### Comparing `setech-1.2.1/src/setech/api_client/_base.py` & `setech-1.3.0/src/setech/api_client/_base.py`

 * *Files identical despite different names*

### Comparing `setech-1.2.1/src/setech/api_client/async_client.py` & `setech-1.3.0/src/setech/api_client/async_client.py`

 * *Files identical despite different names*

### Comparing `setech-1.2.1/src/setech/api_client/sync_client.py` & `setech-1.3.0/src/setech/api_client/sync_client.py`

 * *Files identical despite different names*

### Comparing `setech-1.2.1/src/setech/constants/date.py` & `setech-1.3.0/src/setech/constants/date.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     7: "jūlijs",
     8: "augusts",
     9: "septembris",
     10: "oktobris",
     11: "novembris",
     12: "decembris",
 }
-LATVIAN_MONTH_MAP_GEN = {
+LATVIAN_MONTH_MAP_ACU = {
     1: "janvārī",
     2: "februārī",
     3: "martā",
     4: "aprīlī",
     5: "maijā",
     6: "jūnijā",
     7: "jūlijā",
```

### Comparing `setech-1.2.1/src/setech/logging/formatters.py` & `setech-1.3.0/src/setech/logging/formatters.py`

 * *Files identical despite different names*

### Comparing `setech-1.2.1/src/setech/logging/handlers.py` & `setech-1.3.0/src/setech/logging/handlers.py`

 * *Files identical despite different names*

### Comparing `setech-1.2.1/src/setech/utils/__init__.py` & `setech-1.3.0/src/setech/utils/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,45 @@
 from .numeric import round_decimal
 from .parse import (
     SetechJSONEncoder,
     as_decimal,
     as_decimal_or_none,
     jsonify_value,
     shorten_value,
+    shortify_log_dict,
     shortify_log_extra_data,
     str_as_date,
     str_as_date_or_none,
 )
-from .ssn import generate_aged_latvian_personal_code, generate_random_latvian_personal_code
-from .text import convert_datetime_to_latvian_words, convert_number_to_latvian_words
+from .ssn import PersonalCode, generate_aged_latvian_personal_code, generate_random_latvian_personal_code
+from .text import convert_datetime_to_latvian_words, convert_number_to_latvian_words, slugify, transliterate
+from .time import time_now, time_utc_now
 from .validators import validate_iban, validate_latvian_personal_code
 from .various import get_logger, get_nonce
+from .warnings import deprecated
 
 __all__ = [
     "round_decimal",
     "SetechJSONEncoder",
     "as_decimal",
     "as_decimal_or_none",
     "jsonify_value",
     "shorten_value",
+    "shortify_log_dict",
     "shortify_log_extra_data",
     "str_as_date",
     "str_as_date_or_none",
-    "convert_datetime_to_latvian_words",
-    "convert_number_to_latvian_words",
+    "PersonalCode",
     "generate_aged_latvian_personal_code",
     "generate_random_latvian_personal_code",
+    "convert_datetime_to_latvian_words",
+    "convert_number_to_latvian_words",
+    "slugify",
+    "transliterate",
+    "time_now",
+    "time_utc_now",
     "validate_iban",
     "validate_latvian_personal_code",
     "get_logger",
     "get_nonce",
-    "shorten_value",
-    "shortify_log_extra_data",
+    "deprecated",
 ]
```

### Comparing `setech-1.2.1/src/setech/utils/numeric.py` & `setech-1.3.0/src/setech/utils/numeric.py`

 * *Files identical despite different names*

### Comparing `setech-1.2.1/src/setech/utils/parse.py` & `setech-1.3.0/src/setech/utils/parse.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,74 +1,61 @@
 import dataclasses
 import datetime
 import decimal
 import json
+import typing
 import warnings
-from typing import Any
 
-from pydantic import BaseModel
+import pydantic
 
-from setech.utils.warnings import deprecated
+from .warnings import deprecated as _deprecate
 
 __all__ = [
     "SetechJSONEncoder",
     "as_decimal",
     "as_decimal_or_none",
     "jsonify_value",
     "shorten_value",
+    "shortify_log_dict",
     "shortify_log_extra_data",
     "str_as_date",
     "str_as_date_or_none",
 ]
 
 
-def str_as_date(date_str: str, date_format: str = "%Y-%m-%d") -> datetime.date:
-    datetime_object = datetime.datetime.strptime(date_str, date_format)
-    return datetime_object.date()
-
-
-def str_as_date_or_none(date_str: str | None, date_format: str = "%Y-%m-%d") -> datetime.date | None:
-    if not isinstance(date_str, str):
-        return None
-    try:
-        return str_as_date(date_str, date_format)
-    except (ValueError, TypeError):
-        return None
-
-
 def as_decimal(decimal_str: str | int | float) -> decimal.Decimal:
     return decimal.Decimal(str(decimal_str))
 
 
 def as_decimal_or_none(decimal_str: str | int | float | None) -> decimal.Decimal | None:
     if not isinstance(decimal_str, (str | int | float)):
         return None
     try:
         return as_decimal(decimal_str)
     except (decimal.DecimalException, TypeError):
         return None
 
 
-def jsonify_value(value: Any) -> Any:
+def jsonify_value(value: typing.Any) -> typing.Any:
     """Return JSON'ified version of the object type-casted using SetechJSONEncoder
 
     :param value: any object
     :return: json compatible object
     """
     return json.loads(json.dumps(value, cls=SetechJSONEncoder))
 
 
 class SetechJSONEncoder(json.JSONEncoder):
-    def default(self, obj: Any) -> Any:
+    def default(self, obj: typing.Any) -> typing.Any:
         try:
             if isinstance(obj, decimal.Decimal):
                 return str(obj)
             if isinstance(obj, (datetime.datetime, datetime.date)):
                 return obj.isoformat()
-            if isinstance(obj, BaseModel):
+            if isinstance(obj, pydantic.BaseModel):
                 return obj.model_dump()
             if isinstance(obj, datetime.timedelta):
                 return dict(__type__="timedelta", total_seconds=obj.total_seconds())
             if isinstance(obj, set):
                 return sorted(obj, key=str)
             if hasattr(obj, "as_dict"):
                 return obj.as_dict
@@ -79,15 +66,15 @@
             return super().default(obj)
         except TypeError as exc:
             if "not JSON serializable" in str(exc):
                 return str(obj)
             raise exc  # pragma: no cover
 
 
-def shorten_value(value: Any) -> Any:
+def shorten_value(value: typing.Any) -> typing.Any:
     """Recursively shorten long string values and return a shortened version copy object.
 
     :param value: Object in which to recursively search for strings to shorten
     :return: Shortened version of the value
     """
     if isinstance(value, str):
         return f"{value[:30]}...{value[-30:]}" if isinstance(value, str) and len(value) > 64 else value
@@ -96,23 +83,37 @@
     if isinstance(value, tuple):
         return tuple(shorten_value(v) for v in value)
     if isinstance(value, dict):
         return {k: shorten_value(v) for k, v in value.items()}
     return value
 
 
-def shortify_log_extra_data(log_value: Any) -> dict[str, Any]:
+def shortify_log_extra_data(log_value: typing.Any) -> dict[str, typing.Any]:
     """Shorten long values and normalize (to json compatible format) dictionary values
 
     :param log_value: Object to convert into json log favourable format
     :return: shortened and normalized object
     """
     shortened_log_value = shorten_value(jsonify_value(log_value))
     if not isinstance(shortened_log_value, dict):
         shortened_log_value = {"extra_data": shortened_log_value}
     return shortened_log_value
 
 
-@deprecated(new_method=shortify_log_extra_data)
-def shortify_log_dict(dct: Any) -> dict[str, Any]:
-    warnings.warn("Deprecated method name! Use `shortify_log_extra_data` instead", DeprecationWarning, 2)
+def str_as_date(date_str: str, date_format: str = "%Y-%m-%d") -> datetime.date:
+    datetime_object = datetime.datetime.strptime(date_str, date_format)
+    return datetime_object.date()
+
+
+def str_as_date_or_none(date_str: str | None, date_format: str = "%Y-%m-%d") -> datetime.date | None:
+    if not isinstance(date_str, str):
+        return None
+    try:
+        return str_as_date(date_str, date_format)
+    except (ValueError, TypeError):
+        return None
+
+
+@_deprecate(new_method=shortify_log_extra_data)
+def shortify_log_dict(dct: typing.Any) -> dict[str, typing.Any]:
+    warnings.warn("Deprecated method! Use `shortify_log_extra_data` instead", DeprecationWarning, 2)
     return shortify_log_extra_data(dct)
```

### Comparing `setech-1.2.1/src/setech/utils/ssn.py` & `setech-1.3.0/src/setech/utils/ssn.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import datetime
-from random import randint
-from typing import NamedTuple
+import random
+import typing
 
 __all__ = [
     "generate_random_latvian_personal_code",
     "generate_aged_latvian_personal_code",
     "PersonalCode",
 ]
 
@@ -18,22 +18,22 @@
     return PersonalCode.generate_legacy_with_check_digit().dashed
 
 
 def generate_aged_latvian_personal_code(years: int) -> str:
     return PersonalCode.generate_legacy_with_check_digit(years).dashed
 
 
-class PersonalCode(NamedTuple):
+class PersonalCode(typing.NamedTuple):
     first_part: str
     second_part: str
     has_check_digit: bool = False
 
     @classmethod
     def generate_anonymous_personal_code(cls) -> "PersonalCode":
-        pc = f"3{randint(2 * 10 ** 9, 10 * 10 ** 9 - 1)}"
+        pc = f"3{random.randint(2 * 10 ** 9, 10 * 10 ** 9 - 1)}"
         first_part = pc[:6]
         second_part = pc[6:]
         instance = cls(first_part, second_part)
         return instance
 
     @classmethod
     def generate_anonymous_with_check_digit(cls) -> "PersonalCode":
@@ -52,20 +52,22 @@
                 raise ValueError(
                     "Too young for legacy Personal Code! years < "
                     f"{(datetime.date.today() - FINAL_LEGACY_DATE).days // 365}"
                 )
             min_age_in_days = abs(years) * 365
             max_age_in_days = abs(years + 1) * 365
             birthdate = datetime.date.today() - datetime.timedelta(
-                days=randint(min_age_in_days + 1, max_age_in_days - 1)
+                days=random.randint(min_age_in_days + 1, max_age_in_days - 1)
             )
         else:
             max_age_in_days = (FINAL_LEGACY_DATE - START_LEGACY_DATE).days
             min_age_in_days = 1
-            birthdate = FINAL_LEGACY_DATE - datetime.timedelta(days=randint(min_age_in_days + 1, max_age_in_days - 1))
+            birthdate = FINAL_LEGACY_DATE - datetime.timedelta(
+                days=random.randint(min_age_in_days + 1, max_age_in_days - 1)
+            )
         return cls._create_from_birthday(birthdate)
 
     @classmethod
     def generate_legacy_for_birthday(cls, *args: datetime.date | int) -> "PersonalCode":
         if len(args) == 1:
             if not isinstance(args[0], datetime.date):
                 raise ValueError(
@@ -94,15 +96,15 @@
             )
         return cls._create_from_birthday(birthday)
 
     @classmethod
     def _create_from_birthday(cls, birthday: datetime.date) -> "PersonalCode":
         first_part = f"{birthday.day:02d}{birthday.month:02d}{str(birthday.year)[2:]}"
         century_digit = 2 if birthday.year // 2000 else 1 if birthday.year // 1900 else 0
-        second_part = f"{century_digit}{randint(0, 999):03}"
+        second_part = f"{century_digit}{random.randint(0, 999):03}"
         tmp = cls(first_part, second_part)
         check_digit = tmp._get_checksum_digit()
         if check_digit == 10:
             return cls._create_from_birthday(birthday)
         second_part = f"{second_part}{check_digit}"
         return cls(first_part, second_part, True)
```

### Comparing `setech-1.2.1/src/setech/utils/validators.py` & `setech-1.3.0/src/setech/utils/validators.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import re
-from string import ascii_uppercase
+import string
 
-from setech.utils.ssn import PersonalCode
+import setech.utils.ssn
+
+__all__ = ["validate_iban", "validate_latvian_personal_code"]
 
 
 def validate_iban(iban: str) -> bool:
     # Sanitization and sanity check
     _iban = iban.upper().replace(" ", "")
     if not re.search(r"^[A-Z0-9]{10,32}$", _iban):
         return False
     char_map = {str(i): i for i in range(10)}
-    char_map.update({l: i for i, l in enumerate(ascii_uppercase, start=10)})
+    char_map.update({l: i for i, l in enumerate(string.ascii_uppercase, start=10)})
 
     letters = {ord(k): str(v) for k, v in char_map.items()}
 
     zeros_iban = _iban[:2] + "00" + _iban[4:]
     iban_inverted = zeros_iban[4:] + zeros_iban[:4]
     iban_numbered = iban_inverted.translate(letters)
 
@@ -24,8 +26,8 @@
         iban_inverted = _iban[4:] + _iban[:4]
         iban_numbered = iban_inverted.translate(letters)
         return int(iban_numbered) % 97 == 1
     return False
 
 
 def validate_latvian_personal_code(personal_code: str) -> bool:
-    return PersonalCode(personal_code[:6], personal_code[-5:], True).is_valid
+    return setech.utils.ssn.PersonalCode(personal_code[:6], personal_code[-5:], True).is_valid
```

### Comparing `setech-1.2.1/src/setech.egg-info/PKG-INFO` & `setech-1.3.0/src/setech.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setech
-Version: 1.2.1
+Version: 1.3.0
 Summary: Setech utilities
 Author-email: Eriks Karls <eriks.karls@sefinance.lv>
 Project-URL: Homepage, https://pypi.org/project/setech/
 Keywords: setech,logging,api-client,utility,utils
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -16,14 +16,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 License-File: LICENCE
 Requires-Dist: httpx[http2]~=0.27.0
 Requires-Dist: pydantic~=2.6
 Requires-Dist: num2words~=0.5
+Requires-Dist: unidecode~=1.3
 
 # Example code
 ```python
 # client.py
 from setech import SyncClient
```

### Comparing `setech-1.2.1/src/setech.egg-info/SOURCES.txt` & `setech-1.3.0/src/setech.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -18,10 +18,11 @@
 src/setech/logging/formatters.py
 src/setech/logging/handlers.py
 src/setech/utils/__init__.py
 src/setech/utils/numeric.py
 src/setech/utils/parse.py
 src/setech/utils/ssn.py
 src/setech/utils/text.py
+src/setech/utils/time.py
 src/setech/utils/validators.py
 src/setech/utils/various.py
 src/setech/utils/warnings.py
```

