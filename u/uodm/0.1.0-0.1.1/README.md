# Comparing `tmp/uodm-0.1.0.tar.gz` & `tmp/uodm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uodm-0.1.0.tar", last modified: Tue Apr 23 13:46:45 2024, max compression
+gzip compressed data, was "uodm-0.1.1.tar", last modified: Wed Apr 24 15:24:16 2024, max compression
```

## Comparing `uodm-0.1.0.tar` & `uodm-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1211 2024-04-23 12:08:19.992618 uodm-0.1.0/LICENSE
--rw-r--r--   0        0        0     2456 2024-04-23 13:42:23.647218 uodm-0.1.0/README.md
--rw-r--r--   0        0        0      488 2024-04-23 13:46:45.003975 uodm-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      667 2024-04-23 12:55:06.946411 uodm-0.1.0/src/uodm/__init__.py
--rw-r--r--   0        0        0     5531 2024-04-23 13:16:16.896606 uodm-0.1.0/src/uodm/uodm.py
--rw-r--r--   0        0        0        0 2024-04-23 12:45:59.201089 uodm-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     2799 1970-01-01 00:00:00.000000 uodm-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-23 12:08:19.992618 uodm-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2451 2024-04-23 13:49:15.123787 uodm-0.1.1/README.md
+-rw-r--r--   0        0        0      488 2024-04-24 15:24:16.303126 uodm-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      667 2024-04-23 12:55:06.946411 uodm-0.1.1/src/uodm/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 15:22:51.793479 uodm-0.1.1/src/uodm/py.typed
+-rw-r--r--   0        0        0     5531 2024-04-23 13:16:16.896606 uodm-0.1.1/src/uodm/uodm.py
+-rw-r--r--   0        0        0        0 2024-04-23 12:45:59.201089 uodm-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     2794 1970-01-01 00:00:00.000000 uodm-0.1.1/PKG-INFO
```

### Comparing `uodm-0.1.0/LICENSE` & `uodm-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `uodm-0.1.0/README.md` & `uodm-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 ```
 
 ## Installation
 
 Grab the latest release with a simple pip command:
 
 ``` bash
-pip install git+https://github.com/yourgithub/uodm.git#egg=uodm
+pip install git+https://github.com/bobuk/uodm.git#egg=uodm
 ```
 
 or just `pip install uodm` if you're ok to use the latest release.
 Don't forget to wear your seatbelt, this thing is fast! 🚗💨
 
 
 ## Contributing
```

### Comparing `uodm-0.1.0/src/uodm/__init__.py` & `uodm-0.1.1/src/uodm/__init__.py`

 * *Files identical despite different names*

### Comparing `uodm-0.1.0/src/uodm/uodm.py` & `uodm-0.1.1/src/uodm/uodm.py`

 * *Files identical despite different names*

### Comparing `uodm-0.1.0/PKG-INFO` & `uodm-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uodm
-Version: 0.1.0
+Version: 0.1.1
 Summary: ultraminimalistic Python library for simple object-document mappint for asyncronous mongodb
 Author-Email: Grigory Bakunov <bobuk@rubedo.cloud>
 License: Unlicense
 Requires-Python: >=3.12
 Requires-Dist: pydantic>=2.7.0
 Requires-Dist: motor>=3.4.0
 Description-Content-Type: text/markdown
@@ -60,15 +60,15 @@
 ```
 
 ## Installation
 
 Grab the latest release with a simple pip command:
 
 ``` bash
-pip install git+https://github.com/yourgithub/uodm.git#egg=uodm
+pip install git+https://github.com/bobuk/uodm.git#egg=uodm
 ```
 
 or just `pip install uodm` if you're ok to use the latest release.
 Don't forget to wear your seatbelt, this thing is fast! 🚗💨
 
 
 ## Contributing
```

