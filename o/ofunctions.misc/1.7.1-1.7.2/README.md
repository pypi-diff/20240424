# Comparing `tmp/ofunctions.misc-1.7.1.tar.gz` & `tmp/ofunctions.misc-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofunctions.misc-1.7.1.tar", last modified: Sun Feb 25 19:47:57 2024, max compression
+gzip compressed data, was "ofunctions.misc-1.7.2.tar", last modified: Tue Apr 23 20:42:14 2024, max compression
```

## Comparing `ofunctions.misc-1.7.1.tar` & `ofunctions.misc-1.7.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-02-25 19:47:57.641342 ofunctions.misc-1.7.1/
--rw-rw-rw-   0        0        0     1590 2023-09-30 16:02:47.000000 ofunctions.misc-1.7.1/LICENSE
--rw-rw-rw-   0        0        0    18009 2024-02-25 19:47:57.639340 ofunctions.misc-1.7.1/PKG-INFO
--rw-rw-rw-   0        0        0    16758 2024-01-09 19:54:46.000000 ofunctions.misc-1.7.1/README.md
-drwxrwxrwx   0        0        0        0 2024-02-25 19:47:57.563340 ofunctions.misc-1.7.1/ofunctions/
-drwxrwxrwx   0        0        0        0 2024-02-25 19:47:57.605374 ofunctions.misc-1.7.1/ofunctions/misc/
--rw-rw-rw-   0        0        0    16061 2024-02-25 19:47:04.000000 ofunctions.misc-1.7.1/ofunctions/misc/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-25 19:47:57.603338 ofunctions.misc-1.7.1/ofunctions.misc.egg-info/
--rw-rw-rw-   0        0        0    18009 2024-02-25 19:47:57.000000 ofunctions.misc-1.7.1/ofunctions.misc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      732 2024-02-25 19:47:57.000000 ofunctions.misc-1.7.1/ofunctions.misc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-25 19:47:57.000000 ofunctions.misc-1.7.1/ofunctions.misc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-02-25 19:47:57.000000 ofunctions.misc-1.7.1/ofunctions.misc.egg-info/namespace_packages.txt
--rw-rw-rw-   0        0        0        2 2023-10-06 16:14:59.000000 ofunctions.misc-1.7.1/ofunctions.misc.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       14 2024-02-25 19:47:57.000000 ofunctions.misc-1.7.1/ofunctions.misc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-02-25 19:47:57.000000 ofunctions.misc-1.7.1/ofunctions.misc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-25 19:47:57.642342 ofunctions.misc-1.7.1/setup.cfg
--rw-rw-rw-   0        0        0     7685 2023-09-30 20:53:03.000000 ofunctions.misc-1.7.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-25 19:47:57.637340 ofunctions.misc-1.7.1/tests/
--rw-rw-rw-   0        0        0     5866 2023-09-30 16:02:47.000000 ofunctions.misc-1.7.1/tests/test_bisection.py
--rw-rw-rw-   0        0        0     3374 2023-09-30 16:02:47.000000 ofunctions.misc-1.7.1/tests/test_checksums.py
--rw-rw-rw-   0        0        0     2037 2023-09-30 20:53:02.000000 ofunctions.misc-1.7.1/tests/test_csv.py
--rw-rw-rw-   0        0        0     1037 2023-09-30 20:53:02.000000 ofunctions.misc-1.7.1/tests/test_delayed_keyboardinterrupt.py
--rw-rw-rw-   0        0        0     8438 2023-09-30 16:02:47.000000 ofunctions.misc-1.7.1/tests/test_file_utils.py
--rw-rw-rw-   0        0        0     1023 2023-09-30 16:02:47.000000 ofunctions.misc-1.7.1/tests/test_json_sanitize.py
--rw-rw-rw-   0        0        0     3308 2023-09-30 20:53:03.000000 ofunctions.misc-1.7.1/tests/test_logger_utils.py
--rw-rw-rw-   0        0        0     1616 2023-09-30 16:02:47.000000 ofunctions.misc-1.7.1/tests/test_mailer.py
--rw-rw-rw-   0        0        0     3566 2024-01-05 13:38:01.000000 ofunctions.misc-1.7.1/tests/test_misc.py
--rw-rw-rw-   0        0        0     6659 2024-01-01 21:08:53.000000 ofunctions.misc-1.7.1/tests/test_network.py
--rw-rw-rw-   0        0        0     1188 2023-09-30 16:02:47.000000 ofunctions.misc-1.7.1/tests/test_platform.py
--rw-rw-rw-   0        0        0     4242 2023-12-30 23:40:58.000000 ofunctions.misc-1.7.1/tests/test_process.py
--rw-rw-rw-   0        0        0      940 2023-09-30 16:02:47.000000 ofunctions.misc-1.7.1/tests/test_random.py
--rw-rw-rw-   0        0        0     2426 2023-09-30 16:02:47.000000 ofunctions.misc-1.7.1/tests/test_service_control.py
--rw-rw-rw-   0        0        0     2215 2023-09-30 20:53:03.000000 ofunctions.misc-1.7.1/tests/test_string_handling.py
--rw-rw-rw-   0        0        0     8291 2024-01-09 19:54:46.000000 ofunctions.misc-1.7.1/tests/test_threading.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:42:14.885085 ofunctions.misc-1.7.2/
+-rw-rw-rw-   0        0        0     1590 2023-09-30 16:02:48.000000 ofunctions.misc-1.7.2/LICENSE
+-rw-rw-rw-   0        0        0    18009 2024-04-23 20:42:14.885085 ofunctions.misc-1.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0    16758 2024-01-09 19:54:48.000000 ofunctions.misc-1.7.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 20:42:14.806951 ofunctions.misc-1.7.2/ofunctions/
+drwxrwxrwx   0        0        0        0 2024-04-23 20:42:14.853838 ofunctions.misc-1.7.2/ofunctions/misc/
+-rw-rw-rw-   0        0        0    16373 2024-04-23 11:04:44.000000 ofunctions.misc-1.7.2/ofunctions/misc/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:42:14.885085 ofunctions.misc-1.7.2/ofunctions.misc.egg-info/
+-rw-rw-rw-   0        0        0    18009 2024-04-23 20:42:14.000000 ofunctions.misc-1.7.2/ofunctions.misc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      732 2024-04-23 20:42:14.000000 ofunctions.misc-1.7.2/ofunctions.misc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 20:42:14.000000 ofunctions.misc-1.7.2/ofunctions.misc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-23 20:42:14.000000 ofunctions.misc-1.7.2/ofunctions.misc.egg-info/namespace_packages.txt
+-rw-rw-rw-   0        0        0        2 2023-10-06 16:15:00.000000 ofunctions.misc-1.7.2/ofunctions.misc.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       14 2024-04-23 20:42:14.000000 ofunctions.misc-1.7.2/ofunctions.misc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-23 20:42:14.000000 ofunctions.misc-1.7.2/ofunctions.misc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 20:42:14.885085 ofunctions.misc-1.7.2/setup.cfg
+-rw-rw-rw-   0        0        0     7685 2023-09-30 20:53:04.000000 ofunctions.misc-1.7.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:42:14.885085 ofunctions.misc-1.7.2/tests/
+-rw-rw-rw-   0        0        0     5866 2023-09-30 16:02:48.000000 ofunctions.misc-1.7.2/tests/test_bisection.py
+-rw-rw-rw-   0        0        0     3374 2023-09-30 16:02:48.000000 ofunctions.misc-1.7.2/tests/test_checksums.py
+-rw-rw-rw-   0        0        0     2037 2023-09-30 20:53:04.000000 ofunctions.misc-1.7.2/tests/test_csv.py
+-rw-rw-rw-   0        0        0     1037 2023-09-30 20:53:04.000000 ofunctions.misc-1.7.2/tests/test_delayed_keyboardinterrupt.py
+-rw-rw-rw-   0        0        0     8438 2023-09-30 16:02:48.000000 ofunctions.misc-1.7.2/tests/test_file_utils.py
+-rw-rw-rw-   0        0        0     1023 2023-09-30 16:02:48.000000 ofunctions.misc-1.7.2/tests/test_json_sanitize.py
+-rw-rw-rw-   0        0        0     3308 2023-09-30 20:53:04.000000 ofunctions.misc-1.7.2/tests/test_logger_utils.py
+-rw-rw-rw-   0        0        0     1616 2023-09-30 16:02:48.000000 ofunctions.misc-1.7.2/tests/test_mailer.py
+-rw-rw-rw-   0        0        0     3566 2024-01-05 13:38:02.000000 ofunctions.misc-1.7.2/tests/test_misc.py
+-rw-rw-rw-   0        0        0     6659 2024-01-01 21:08:54.000000 ofunctions.misc-1.7.2/tests/test_network.py
+-rw-rw-rw-   0        0        0     1188 2023-09-30 16:02:48.000000 ofunctions.misc-1.7.2/tests/test_platform.py
+-rw-rw-rw-   0        0        0     4242 2023-12-30 23:41:00.000000 ofunctions.misc-1.7.2/tests/test_process.py
+-rw-rw-rw-   0        0        0      940 2023-09-30 16:02:48.000000 ofunctions.misc-1.7.2/tests/test_random.py
+-rw-rw-rw-   0        0        0     2426 2023-09-30 16:02:48.000000 ofunctions.misc-1.7.2/tests/test_service_control.py
+-rw-rw-rw-   0        0        0     2215 2023-09-30 20:53:04.000000 ofunctions.misc-1.7.2/tests/test_string_handling.py
+-rw-rw-rw-   0        0        0     8291 2024-01-09 19:54:48.000000 ofunctions.misc-1.7.2/tests/test_threading.py
```

### Comparing `ofunctions.misc-1.7.1/LICENSE` & `ofunctions.misc-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ofunctions.misc-1.7.1/PKG-INFO` & `ofunctions.misc-1.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofunctions.misc
-Version: 1.7.1
+Version: 1.7.2
 Summary: Collection of various functions
 Home-page: https://github.com/netinvent/ofunctions
 Author: NetInvent - Orsiris de Jong
 Author-email: contact@netinvent.fr
 Keywords: network,bisection,logging
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `ofunctions.misc-1.7.1/README.md` & `ofunctions.misc-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `ofunctions.misc-1.7.1/ofunctions/misc/__init__.py` & `ofunctions.misc-1.7.2/ofunctions/misc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 """
 
 __intname__ = "ofunctions.misc"
 __author__ = "Orsiris de Jong"
 __copyright__ = "Copyright (C) 2014-2024 Orsiris de Jong"
 __description__ = "Collection of various functions"
 __licence__ = "BSD 3 Clause"
-__version__ = "1.7.1"
-__build__ = "2024020201"
+__version__ = "1.7.2"
+__build__ = "2024042301"
 __compat__ = "python2.7+"
 
 
 import sys
 
 # python 2.7 compat fixes
 try:
@@ -39,17 +39,19 @@
 def rot13(string):
     # type: (str) -> str
     """
     Rot13 for only A-Z and a-z characters
     """
     return "".join(
         [
-            chr(ord(n) + (13 if "Z" < n < "n" or n < "N" else -13))
-            if ("a" <= n <= "z" or "A" <= n <= "Z")
-            else n
+            (
+                chr(ord(n) + (13 if "Z" < n < "n" or n < "N" else -13))
+                if ("a" <= n <= "z" or "A" <= n <= "Z")
+                else n
+            )
             for n in string
         ]
     )
 
 
 def rot47(string):
     # type: (str) -> str
@@ -384,21 +386,24 @@
                 result = value.split(unit)
                 if len(result) == 2:
                     converted_value = float(result[0]) * cls.units[unit]
                     if unit in cls.bits_units:
                         converted_value /= 8
                     break
             if not converted_value and converted_value != 0:
+                needs_raise = False
                 try:
                     converted_value = float(value)
+                # Here we intercept the original ValueError and replace it with ours
                 except ValueError:
-                    pass
-                raise ValueError(
-                    'Given string "{}" cannot be converted to bytes'.format(value)
-                )
+                    needs_raise = True
+                if needs_raise:
+                    raise ValueError(
+                        'Given string "{}" cannot be converted to bytes'.format(value)
+                    )
             value = converted_value
         if value < 0:
             raise ValueError("Negative bytes should not exist")
         return super(cls, cls).__new__(cls, value)
 
     def _from_units_to_bytes(self, string):
         # Check if we have value:
@@ -407,21 +412,23 @@
             result = string.split(unit)
             if len(result) == 2:
                 value = float(result[0]) * self.units[unit]
                 if unit in self.bits_units:
                     value /= 8
                 break
         if not value:
+            needs_raise = False
             try:
                 return float(string)
             except ValueError:
-                pass
-            raise ValueError(
-                'Given string "{}" cannot be converted to bytes'.format(string)
-            )
+                needs_raise = True
+            if needs_raise:
+                raise ValueError(
+                    'Given string "{}" cannot be converted to bytes'.format(string)
+                )
         return value
 
     def _from_bytes_to_unit(self, unit):
         result = round(self / self.units[unit], 1)
         if unit in self.bits_units:
             result *= 8
         return result
```

### Comparing `ofunctions.misc-1.7.1/ofunctions.misc.egg-info/PKG-INFO` & `ofunctions.misc-1.7.2/ofunctions.misc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofunctions.misc
-Version: 1.7.1
+Version: 1.7.2
 Summary: Collection of various functions
 Home-page: https://github.com/netinvent/ofunctions
 Author: NetInvent - Orsiris de Jong
 Author-email: contact@netinvent.fr
 Keywords: network,bisection,logging
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `ofunctions.misc-1.7.1/ofunctions.misc.egg-info/SOURCES.txt` & `ofunctions.misc-1.7.2/ofunctions.misc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ofunctions.misc-1.7.1/setup.py` & `ofunctions.misc-1.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `ofunctions.misc-1.7.1/tests/test_bisection.py` & `ofunctions.misc-1.7.2/tests/test_bisection.py`

 * *Files identical despite different names*

### Comparing `ofunctions.misc-1.7.1/tests/test_checksums.py` & `ofunctions.misc-1.7.2/tests/test_checksums.py`

 * *Files identical despite different names*

### Comparing `ofunctions.misc-1.7.1/tests/test_csv.py` & `ofunctions.misc-1.7.2/tests/test_csv.py`

 * *Files identical despite different names*

### Comparing `ofunctions.misc-1.7.1/tests/test_delayed_keyboardinterrupt.py` & `ofunctions.misc-1.7.2/tests/test_delayed_keyboardinterrupt.py`

 * *Files identical despite different names*

### Comparing `ofunctions.misc-1.7.1/tests/test_file_utils.py` & `ofunctions.misc-1.7.2/tests/test_file_utils.py`

 * *Files identical despite different names*

### Comparing `ofunctions.misc-1.7.1/tests/test_json_sanitize.py` & `ofunctions.misc-1.7.2/tests/test_json_sanitize.py`

 * *Files identical despite different names*

### Comparing `ofunctions.misc-1.7.1/tests/test_logger_utils.py` & `ofunctions.misc-1.7.2/tests/test_logger_utils.py`

 * *Files identical despite different names*

### Comparing `ofunctions.misc-1.7.1/tests/test_mailer.py` & `ofunctions.misc-1.7.2/tests/test_mailer.py`

 * *Files identical despite different names*

### Comparing `ofunctions.misc-1.7.1/tests/test_misc.py` & `ofunctions.misc-1.7.2/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `ofunctions.misc-1.7.1/tests/test_network.py` & `ofunctions.misc-1.7.2/tests/test_network.py`

 * *Files identical despite different names*

### Comparing `ofunctions.misc-1.7.1/tests/test_platform.py` & `ofunctions.misc-1.7.2/tests/test_platform.py`

 * *Files identical despite different names*

### Comparing `ofunctions.misc-1.7.1/tests/test_process.py` & `ofunctions.misc-1.7.2/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `ofunctions.misc-1.7.1/tests/test_random.py` & `ofunctions.misc-1.7.2/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `ofunctions.misc-1.7.1/tests/test_service_control.py` & `ofunctions.misc-1.7.2/tests/test_service_control.py`

 * *Files identical despite different names*

### Comparing `ofunctions.misc-1.7.1/tests/test_string_handling.py` & `ofunctions.misc-1.7.2/tests/test_string_handling.py`

 * *Files identical despite different names*

### Comparing `ofunctions.misc-1.7.1/tests/test_threading.py` & `ofunctions.misc-1.7.2/tests/test_threading.py`

 * *Files identical despite different names*

