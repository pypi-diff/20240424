# Comparing `tmp/febraban_code-0.1.0.tar.gz` & `tmp/febraban_code-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "febraban_code-0.1.0.tar", max compression
+gzip compressed data, was "febraban_code-0.1.1.tar", max compression
```

## Comparing `febraban_code-0.1.0.tar` & `febraban_code-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1071 2024-02-29 19:21:58.510804 febraban_code-0.1.0/LICENSE
--rw-r--r--   0        0        0     3419 2024-03-02 21:56:27.911173 febraban_code-0.1.0/README.md
--rw-r--r--   0        0        0       81 2024-02-29 19:31:35.354820 febraban_code-0.1.0/febraban_code/__init__.py
--rw-r--r--   0        0        0     8649 2024-03-02 21:47:23.651157 febraban_code-0.1.0/febraban_code/febraban_code.py
--rw-r--r--   0        0        0      373 2024-03-04 14:53:15.715920 febraban_code-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4372 1970-01-01 00:00:00.000000 febraban_code-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-02-29 19:21:58.510804 febraban_code-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3419 2024-03-02 21:56:27.911173 febraban_code-0.1.1/README.md
+-rw-r--r--   0        0        0       81 2024-02-29 19:31:35.354820 febraban_code-0.1.1/febraban_code/__init__.py
+-rw-r--r--   0        0        0     8539 2024-04-24 18:24:32.524940 febraban_code-0.1.1/febraban_code/febraban_code.py
+-rw-r--r--   0        0        0      373 2024-04-24 18:24:58.672941 febraban_code-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4372 1970-01-01 00:00:00.000000 febraban_code-0.1.1/PKG-INFO
```

### Comparing `febraban_code-0.1.0/LICENSE` & `febraban_code-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `febraban_code-0.1.0/README.md` & `febraban_code-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `febraban_code-0.1.0/febraban_code/febraban_code.py` & `febraban_code-0.1.1/febraban_code/febraban_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,29 +51,28 @@
     def __get_dv_module_11(self, number: str) -> int:
         """
         - number : str
             The number for which to calculate the module 11 check digit.
 
         Returns the calculated check digit.
         """
-        multiplier = 2
+        multiplier = 4
         total = 0
 
-        for element in number[::-1]:
-            result = int(element) * multiplier
-            multiplier = (2 if multiplier == 9 else multiplier + 1)
-            total += result
-
-        remainder = total % 11
-        exceptions = {0: 0, 1: 0, 10: 1}
-        if remainder in exceptions:
-            return exceptions[remainder]
+        for digit in range(0, len(number)):
+            total += int(number[digit]) * multiplier
+            multiplier = 10 if multiplier == 2 else multiplier
+            multiplier -= 1
 
-        dv_calculated = 11 - remainder
-        return dv_calculated
+        dv = 11 - total % 11
+
+        if dv in {0, 10, 11}:
+            return 1
+
+        return dv
 
     def __get_expiry(self, expiry_factor: str) -> date:
         """
         - expiry_factor : str
             The factor used to calculate the expiry date.
 
         Returns the calculated expiry date.
```

### Comparing `febraban_code-0.1.0/PKG-INFO` & `febraban_code-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: febraban-code
-Version: 0.1.0
+Version: 0.1.1
 Summary: FebrabanCode Class for parsing and validating Febraban codes used in Brazil.
 License: MIT
 Keywords: digitable line,brazil,bar code,febraban
 Author: Ricardo Castro
 Author-email: srrenks@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
```

