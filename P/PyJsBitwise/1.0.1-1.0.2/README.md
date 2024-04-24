# Comparing `tmp/PyJsBitwise-1.0.1.tar.gz` & `tmp/pyjsbitwise-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyJsBitwise-1.0.1.tar", last modified: Mon Apr  1 12:04:25 2024, max compression
+gzip compressed data, was "pyjsbitwise-1.0.2.tar", last modified: Wed Apr 24 05:21:34 2024, max compression
```

## Comparing `PyJsBitwise-1.0.1.tar` & `pyjsbitwise-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:04:25.065053 PyJsBitwise-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-01 12:04:16.000000 PyJsBitwise-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-01 12:04:25.065053 PyJsBitwise-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-01 12:04:16.000000 PyJsBitwise-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 12:04:25.065053 PyJsBitwise-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-01 12:04:16.000000 PyJsBitwise-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:04:25.061053 PyJsBitwise-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:04:25.065053 PyJsBitwise-1.0.1/src/PyJsBitwise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-01 12:04:25.000000 PyJsBitwise-1.0.1/src/PyJsBitwise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-01 12:04:25.000000 PyJsBitwise-1.0.1/src/PyJsBitwise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 12:04:25.000000 PyJsBitwise-1.0.1/src/PyJsBitwise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-01 12:04:25.000000 PyJsBitwise-1.0.1/src/PyJsBitwise.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:04:25.065053 PyJsBitwise-1.0.1/src/pyjsbitwise/
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-04-01 12:04:16.000000 PyJsBitwise-1.0.1/src/pyjsbitwise/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 05:21:34.632336 pyjsbitwise-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-24 05:21:28.000000 pyjsbitwise-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-24 05:21:34.632336 pyjsbitwise-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-24 05:21:28.000000 pyjsbitwise-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 05:21:34.632336 pyjsbitwise-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-24 05:21:28.000000 pyjsbitwise-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 05:21:34.632336 pyjsbitwise-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 05:21:34.632336 pyjsbitwise-1.0.2/src/PyJsBitwise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-24 05:21:34.000000 pyjsbitwise-1.0.2/src/PyJsBitwise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-24 05:21:34.000000 pyjsbitwise-1.0.2/src/PyJsBitwise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 05:21:34.000000 pyjsbitwise-1.0.2/src/PyJsBitwise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 05:21:34.000000 pyjsbitwise-1.0.2/src/PyJsBitwise.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 05:21:34.632336 pyjsbitwise-1.0.2/src/pyjsbitwise/
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-24 05:21:28.000000 pyjsbitwise-1.0.2/src/pyjsbitwise/__init__.py
```

### Comparing `PyJsBitwise-1.0.1/LICENSE` & `pyjsbitwise-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyJsBitwise-1.0.1/PKG-INFO` & `pyjsbitwise-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyJsBitwise
-Version: 1.0.1
+Version: 1.0.2
 Summary: JavaScript-flavored bitwise operations.
 Home-page: https://github.com/Pairman/PyJsBitwise
 Author: Pairman
 Author-email: pairmanxlr@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/Pairman/PyJsBitwise
 Project-URL: Changelog, https://github.com/Pairman/PyJsBitwise/blob/main/CHANGELOG.md
@@ -37,9 +37,9 @@
 bwxor(2**31, 2**31-1) # -1
 ```
 
 Shift left, right and unsigned right like JavaScript's <<, >>, >>>:
 ```python
 lshift(1, 32) # 1
 rshift(-2, -31) # -1
-urshift(-1,0) # 4294967295
+urshift(-1, 0) # 4294967295
 ```
```

### Comparing `PyJsBitwise-1.0.1/README.md` & `pyjsbitwise-1.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -21,9 +21,9 @@
 bwxor(2**31, 2**31-1) # -1
 ```
 
 Shift left, right and unsigned right like JavaScript's <<, >>, >>>:
 ```python
 lshift(1, 32) # 1
 rshift(-2, -31) # -1
-urshift(-1,0) # 4294967295
+urshift(-1, 0) # 4294967295
 ```
```

### Comparing `PyJsBitwise-1.0.1/setup.py` & `pyjsbitwise-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
 	long_description = f.read()
 
 setup(
 	name = "PyJsBitwise",
-	version = "1.0.1",
+	version = "1.0.2",
 	author = "Pairman",
 	author_email = "pairmanxlr@gmail.com",
 	description = "JavaScript-flavored bitwise operations.",
 	long_description = long_description,
 	long_description_content_type = "text/markdown",
 	license = "GNU General Public License v3 (GPLv3)",
 	keywords = ["javascript", "js", "bitwise", "shift"],
```

### Comparing `PyJsBitwise-1.0.1/src/PyJsBitwise.egg-info/PKG-INFO` & `pyjsbitwise-1.0.2/src/PyJsBitwise.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyJsBitwise
-Version: 1.0.1
+Version: 1.0.2
 Summary: JavaScript-flavored bitwise operations.
 Home-page: https://github.com/Pairman/PyJsBitwise
 Author: Pairman
 Author-email: pairmanxlr@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/Pairman/PyJsBitwise
 Project-URL: Changelog, https://github.com/Pairman/PyJsBitwise/blob/main/CHANGELOG.md
@@ -37,9 +37,9 @@
 bwxor(2**31, 2**31-1) # -1
 ```
 
 Shift left, right and unsigned right like JavaScript's <<, >>, >>>:
 ```python
 lshift(1, 32) # 1
 rshift(-2, -31) # -1
-urshift(-1,0) # 4294967295
+urshift(-1, 0) # 4294967295
 ```
```

### Comparing `PyJsBitwise-1.0.1/src/pyjsbitwise/__init__.py` & `pyjsbitwise-1.0.2/src/pyjsbitwise/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-from functools import reduce
-from math import isnan
+from functools import reduce as _reduce
+from math import isnan as _isnan
 
 def i32cast(n):
 	"""Overlow behavior of signed 32-bit integer.
  	:param n: Number to be owerflowed. Int or float.
   	:return: The overflowed result. Int.
  	"""
-	return 0 if n == None or isnan(n) else (int(n) + 0x80000000) % 0x100000000 - 0x80000000
+	return 0 if n == None or _isnan(n) else (int(n) + 0x80000000) % 0x100000000 - 0x80000000
 
 def lshift(n, i):
 	"""JavaScript-flavored bitwise shift left (<<).
  	:param n: Number to be owerflowed. Int or float.
  	:param i: Number of bits to shift by. Int.
   	:return: The shift result. Int.
  	"""
-	if n == None or isnan(n):
+	if n == None or _isnan(n):
 		return 0
 	n = int(n) & 0xFFFFFFFF
-	i = int(i) & 0x1F
+	i = 0 if i == None or _isnan(n) else int(i) & 0x1F
 	return i32cast(n << i if i >= 0 else n >> -i)
 
 def rshift(n, i):
 	"""JavaScript-flavored shift right (>>).
  	:param n: Number to be owerflowed. Int or float.
  	:param i: Number of bits to shift by. Int.
   	:return: The shift result. Int.
  	"""
-	if n == None or isnan(n):
+	if n == None or _isnan(n):
 		return 0
 	n = (int(n) & 0xFFFFFFFF) if type(n) is float else i32cast(n)
-	i = int(i) & 0x1F
+	i = 0 if i == None or _isnan(n) else int(i) & 0x1F
 	return i32cast(n >> i if i >= 0 else n << -i)
 
 def urshift(n, i):
 	"""JavaScript-flavored unsigned shift right (>>>).
  	:param n: Number to be owerflowed. Int or float.
  	:param i: Number of bits to shift by. Int.
   	:return: The shift result. Int.
  	"""
-	if n == None or isnan(n):
+	if n == None or _isnan(n):
 		return 0
 	n = int(n) & 0xFFFFFFFF
-	i = int(i) & 0x1F
+	i = 0 if i == None or _isnan(n) else int(i) & 0x1F
 	return (n >> i if i >= 0 else -n << -i) & 0xffffffff
 
 def bwnot(n):
 	"""JavaScript-flavored bitwise not (~).
  	:param m: Number. Int or float.
   	:return: The bitwise-not result. Int.
  	"""
 	return ~i32cast(n)
 
 def bwand(*args):
 	"""JavaScript-flavored bitwise and (&).
  	:param *args: Numbers. Int or float.
   	:return: The bitwise-and result. Int.
  	"""
-	return reduce(lambda m, n: i32cast(m) & i32cast(n), args)
+	return _reduce(lambda m, n: i32cast(m) & i32cast(n), args)
 
 def bwor(*args):
 	"""JavaScript-flavored bitwise or (|).
  	:param *args: Numbers. Int or float.
   	:return: The bitwise-or result. Int.
  	"""
-	return reduce(lambda m, n: i32cast(m) | i32cast(n), args)
+	return _reduce(lambda m, n: i32cast(m) | i32cast(n), args)
 
 def bwxor(*args):
 	"""JavaScript-flavored bitwise xor (^).
  	:param *args: Numbers. Int or float.
   	:return: The bitwise-xor result. Int.
  	"""
-	return reduce(lambda m, n: i32cast(m) ^ i32cast(n), args)
+	return _reduce(lambda m, n: i32cast(m) ^ i32cast(n), args)
```

