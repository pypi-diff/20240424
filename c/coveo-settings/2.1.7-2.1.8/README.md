# Comparing `tmp/coveo_settings-2.1.7.tar.gz` & `tmp/coveo_settings-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coveo_settings-2.1.7.tar", max compression
+gzip compressed data, was "coveo_settings-2.1.8.tar", max compression
```

## Comparing `coveo_settings-2.1.7.tar` & `coveo_settings-2.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     6639 2024-03-24 12:46:07.131114 coveo_settings-2.1.7/README.md
--rw-r--r--   0        0        0      472 2024-03-24 12:46:07.131114 coveo_settings-2.1.7/coveo_settings/__init__.py
--rw-r--r--   0        0        0      333 2024-03-24 12:46:07.131114 coveo_settings-2.1.7/coveo_settings/annotations.py
--rw-r--r--   0        0        0      411 2024-03-24 12:46:07.131114 coveo_settings-2.1.7/coveo_settings/any_setting.py
--rw-r--r--   0        0        0      844 2024-03-24 12:46:07.131114 coveo_settings-2.1.7/coveo_settings/bool_setting.py
--rw-r--r--   0        0        0      862 2024-03-24 12:46:07.131114 coveo_settings-2.1.7/coveo_settings/dict_setting.py
--rw-r--r--   0        0        0      904 2024-03-24 12:46:07.131114 coveo_settings-2.1.7/coveo_settings/exceptions.py
--rw-r--r--   0        0        0      441 2024-03-24 12:46:07.131114 coveo_settings-2.1.7/coveo_settings/float_setting.py
--rw-r--r--   0        0        0      537 2024-03-24 12:46:07.131114 coveo_settings-2.1.7/coveo_settings/int_setting.py
--rw-r--r--   0        0        0      554 2024-03-24 12:46:07.131114 coveo_settings-2.1.7/coveo_settings/mock.py
--rw-r--r--   0        0        0     1459 2024-03-24 12:46:07.131114 coveo_settings-2.1.7/coveo_settings/path_setting.py
--rw-r--r--   0        0        0        0 2024-03-24 12:46:07.131114 coveo_settings-2.1.7/coveo_settings/py.typed
--rw-r--r--   0        0        0    14447 2024-03-24 12:46:07.131114 coveo_settings-2.1.7/coveo_settings/setting_abc.py
--rw-r--r--   0        0        0      155 2024-03-24 12:46:07.131114 coveo_settings-2.1.7/coveo_settings/settings.py
--rw-r--r--   0        0        0     1112 2024-03-24 12:46:07.131114 coveo_settings-2.1.7/coveo_settings/string_setting.py
--rw-r--r--   0        0        0      414 2024-03-24 12:46:07.131114 coveo_settings-2.1.7/coveo_settings/validation.py
--rw-r--r--   0        0        0      675 2024-03-24 12:46:27.507057 coveo_settings-2.1.7/pyproject.toml
--rw-r--r--   0        0        0     7175 1970-01-01 00:00:00.000000 coveo_settings-2.1.7/PKG-INFO
+-rw-r--r--   0        0        0     6639 2024-04-24 12:47:02.303192 coveo_settings-2.1.8/README.md
+-rw-r--r--   0        0        0      472 2024-04-24 12:47:02.303192 coveo_settings-2.1.8/coveo_settings/__init__.py
+-rw-r--r--   0        0        0      333 2024-04-24 12:47:02.303192 coveo_settings-2.1.8/coveo_settings/annotations.py
+-rw-r--r--   0        0        0      411 2024-04-24 12:47:02.303192 coveo_settings-2.1.8/coveo_settings/any_setting.py
+-rw-r--r--   0        0        0      860 2024-04-24 12:47:02.303192 coveo_settings-2.1.8/coveo_settings/bool_setting.py
+-rw-r--r--   0        0        0      862 2024-04-24 12:47:02.303192 coveo_settings-2.1.8/coveo_settings/dict_setting.py
+-rw-r--r--   0        0        0      904 2024-04-24 12:47:02.303192 coveo_settings-2.1.8/coveo_settings/exceptions.py
+-rw-r--r--   0        0        0      441 2024-04-24 12:47:02.303192 coveo_settings-2.1.8/coveo_settings/float_setting.py
+-rw-r--r--   0        0        0      537 2024-04-24 12:47:02.303192 coveo_settings-2.1.8/coveo_settings/int_setting.py
+-rw-r--r--   0        0        0      554 2024-04-24 12:47:02.303192 coveo_settings-2.1.8/coveo_settings/mock.py
+-rw-r--r--   0        0        0     1459 2024-04-24 12:47:02.303192 coveo_settings-2.1.8/coveo_settings/path_setting.py
+-rw-r--r--   0        0        0        0 2024-04-24 12:47:02.303192 coveo_settings-2.1.8/coveo_settings/py.typed
+-rw-r--r--   0        0        0    14447 2024-04-24 12:47:02.303192 coveo_settings-2.1.8/coveo_settings/setting_abc.py
+-rw-r--r--   0        0        0      155 2024-04-24 12:47:02.303192 coveo_settings-2.1.8/coveo_settings/settings.py
+-rw-r--r--   0        0        0     1112 2024-04-24 12:47:02.303192 coveo_settings-2.1.8/coveo_settings/string_setting.py
+-rw-r--r--   0        0        0      414 2024-04-24 12:47:02.303192 coveo_settings-2.1.8/coveo_settings/validation.py
+-rw-r--r--   0        0        0      675 2024-04-24 12:47:23.703219 coveo_settings-2.1.8/pyproject.toml
+-rw-r--r--   0        0        0     7175 1970-01-01 00:00:00.000000 coveo_settings-2.1.8/PKG-INFO
```

### Comparing `coveo_settings-2.1.7/README.md` & `coveo_settings-2.1.8/README.md`

 * *Files identical despite different names*

### Comparing `coveo_settings-2.1.7/coveo_settings/bool_setting.py` & `coveo_settings-2.1.8/coveo_settings/bool_setting.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,18 +6,18 @@
     """
     Setting that handles bool values.
 
     Unlike Python, the bool conversion only allows for a few specific keywords to guard against mistakes.
     For instance, empty objects (strings, lists, dicts) or None will raise an exception.
     """
 
-    TRUE_VALUES = ("true", "yes", "1", "y")
-    FALSE_VALUES = ("false", "no", "0", "n")
+    TRUE_VALUES = ("true", "yes", "1", "y", "on")
+    FALSE_VALUES = ("false", "no", "0", "n", "off")
 
     @staticmethod
     def _cast(value: ConfigValue) -> bool:
         """Converts any supported value to a bool."""
-        value = str(value).lower()
+        value = str(value).casefold()
         if value not in BoolSetting.TRUE_VALUES + BoolSetting.FALSE_VALUES:
             raise ValueError(f"Cannot determine boolean from {value}")
 
         return value in BoolSetting.TRUE_VALUES
```

### Comparing `coveo_settings-2.1.7/coveo_settings/dict_setting.py` & `coveo_settings-2.1.8/coveo_settings/dict_setting.py`

 * *Files identical despite different names*

### Comparing `coveo_settings-2.1.7/coveo_settings/exceptions.py` & `coveo_settings-2.1.8/coveo_settings/exceptions.py`

 * *Files identical despite different names*

### Comparing `coveo_settings-2.1.7/coveo_settings/int_setting.py` & `coveo_settings-2.1.8/coveo_settings/int_setting.py`

 * *Files identical despite different names*

### Comparing `coveo_settings-2.1.7/coveo_settings/mock.py` & `coveo_settings-2.1.8/coveo_settings/mock.py`

 * *Files identical despite different names*

### Comparing `coveo_settings-2.1.7/coveo_settings/path_setting.py` & `coveo_settings-2.1.8/coveo_settings/path_setting.py`

 * *Files identical despite different names*

### Comparing `coveo_settings-2.1.7/coveo_settings/setting_abc.py` & `coveo_settings-2.1.8/coveo_settings/setting_abc.py`

 * *Files identical despite different names*

### Comparing `coveo_settings-2.1.7/coveo_settings/string_setting.py` & `coveo_settings-2.1.8/coveo_settings/string_setting.py`

 * *Files identical despite different names*

### Comparing `coveo_settings-2.1.7/pyproject.toml` & `coveo_settings-2.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "coveo-settings"
-version = "2.1.7"
+version = "2.1.8"
 description = "Settings driven by environment variables."
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/coveooss/coveo-python-oss/tree/main/coveo-settings"
 authors = ["Jonathan Piché <tools@coveo.com>"]
```

### Comparing `coveo_settings-2.1.7/PKG-INFO` & `coveo_settings-2.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coveo-settings
-Version: 2.1.7
+Version: 2.1.8
 Summary: Settings driven by environment variables.
 Home-page: https://github.com/coveooss/coveo-python-oss/tree/main/coveo-settings
 License: Apache-2.0
 Author: Jonathan Piché
 Author-email: tools@coveo.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: Apache Software License
```

