# Comparing `tmp/washpy-0.1.0.tar.gz` & `tmp/washpy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "washpy-0.1.0.tar", max compression
+gzip compressed data, was "washpy-0.2.0.tar", max compression
```

## Comparing `washpy-0.1.0.tar` & `washpy-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0    42028 2024-03-12 18:48:18.147180 washpy-0.1.0/LICENSE
--rw-r--r--   0        0        0     2045 2024-03-13 21:10:47.766428 washpy-0.1.0/README.md
--rw-r--r--   0        0        0      397 2024-04-09 18:58:39.436821 washpy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      315 2024-04-10 18:11:41.327256 washpy-0.1.0/washpy/__init__.py
--rw-r--r--   0        0        0     1086 2024-04-10 18:05:09.050320 washpy-0.1.0/washpy/authenticate.py
--rw-r--r--   0        0        0     7117 2024-04-17 15:28:39.170463 washpy-0.1.0/washpy/device_user.py
--rw-r--r--   0        0        0      778 2024-04-10 18:06:58.529132 washpy-0.1.0/washpy/post_new_password.py
--rw-r--r--   0        0        0     3453 2024-04-10 17:50:40.504127 washpy-0.1.0/washpy/status.py
--rw-r--r--   0        0        0     2681 1970-01-01 00:00:00.000000 washpy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    42028 2024-04-23 21:57:43.954435 washpy-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2045 2024-04-23 21:57:43.954435 washpy-0.2.0/README.md
+-rw-r--r--   0        0        0      472 2024-04-24 19:35:10.382448 washpy-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      315 2024-04-23 21:57:43.991103 washpy-0.2.0/washpy/__init__.py
+-rw-r--r--   0        0        0     1086 2024-04-23 21:57:43.987770 washpy-0.2.0/washpy/authenticate.py
+-rw-r--r--   0        0        0     3111 2024-04-24 19:26:06.083745 washpy-0.2.0/washpy/device_user.py
+-rw-r--r--   0        0        0     4549 2024-04-24 16:21:19.635915 washpy-0.2.0/washpy/pExtended.py
+-rw-r--r--   0        0        0      778 2024-04-23 21:57:43.987770 washpy-0.2.0/washpy/post_new_password.py
+-rw-r--r--   0        0        0     9487 2024-04-24 19:32:43.580101 washpy-0.2.0/washpy/state.py
+-rw-r--r--   0        0        0     3453 2024-04-23 21:57:43.987770 washpy-0.2.0/washpy/status.py
+-rw-r--r--   0        0        0     2838 1970-01-01 00:00:00.000000 washpy-0.2.0/PKG-INFO
```

### Comparing `washpy-0.1.0/LICENSE` & `washpy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `washpy-0.1.0/README.md` & `washpy-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `washpy-0.1.0/washpy/authenticate.py` & `washpy-0.2.0/washpy/authenticate.py`

 * *Files identical despite different names*

### Comparing `washpy-0.1.0/washpy/post_new_password.py` & `washpy-0.2.0/washpy/post_new_password.py`

 * *Files identical despite different names*

### Comparing `washpy-0.1.0/washpy/status.py` & `washpy-0.2.0/washpy/status.py`

 * *Files identical despite different names*

### Comparing `washpy-0.1.0/PKG-INFO` & `washpy-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: washpy
-Version: 0.1.0
+Version: 0.2.0
 Summary: A partial implementation of the Miele Professional IP Profile API
+Home-page: https://codeberg.org/johann.carl/washpy
 License: LGPL-3.0-only
 Author: Johann Carl Meyer
 Author-email: info@johannc.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: isodate (>=0.6.1,<0.7.0)
+Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: requests (==2.29.0)
+Project-URL: Repository, https://codeberg.org/johann.carl/washpy
 Description-Content-Type: text/markdown
 
 # washpy
 
 washpy offers a partial implementation of the Miele Professional IP Profile API.
 
 The project focusses on implementing the parts of the API
```

