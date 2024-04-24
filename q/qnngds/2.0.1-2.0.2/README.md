# Comparing `tmp/qnngds-2.0.1.tar.gz` & `tmp/qnngds-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qnngds-2.0.1.tar", last modified: Mon Apr 22 18:39:31 2024, max compression
+gzip compressed data, was "qnngds-2.0.2.tar", last modified: Tue Apr 23 13:35:13 2024, max compression
```

## Comparing `qnngds-2.0.1.tar` & `qnngds-2.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1081 2024-04-22 18:39:28.953620 qnngds-2.0.1/LICENSE.txt
--rw-r--r--   0        0        0     1129 2024-04-22 18:39:28.953620 qnngds-2.0.1/README.md
--rw-r--r--   0        0        0     1161 2024-04-22 18:39:31.949625 qnngds-2.0.1/pyproject.toml
--rw-r--r--   0        0        0      508 2024-04-22 18:39:28.969620 qnngds-2.0.1/src/qnngds/__init__.py
--rw-r--r--   0        0        0      291 2024-04-22 18:39:28.969620 qnngds-2.0.1/src/qnngds/_default_param.py
--rw-r--r--   0        0        0    22568 2024-04-22 18:39:28.969620 qnngds-2.0.1/src/qnngds/cells.py
--rw-r--r--   0        0        0    10495 2024-04-22 18:39:28.969620 qnngds-2.0.1/src/qnngds/circuits.py
--rw-r--r--   0        0        0    28386 2024-04-22 18:39:28.969620 qnngds-2.0.1/src/qnngds/design.py
--rw-r--r--   0        0        0      160 2024-04-22 18:39:28.969620 qnngds-2.0.1/src/qnngds/devices/__init__.py
--rw-r--r--   0        0        0       90 2024-04-22 18:39:28.969620 qnngds-2.0.1/src/qnngds/devices/htron.py
--rw-r--r--   0        0        0     1177 2024-04-22 18:39:28.969620 qnngds-2.0.1/src/qnngds/devices/nanowire.py
--rw-r--r--   0        0        0     4453 2024-04-22 18:39:28.969620 qnngds-2.0.1/src/qnngds/devices/ntron.py
--rw-r--r--   0        0        0     5860 2024-04-22 18:39:28.969620 qnngds-2.0.1/src/qnngds/devices/resistor.py
--rw-r--r--   0        0        0     2376 2024-04-22 18:39:28.969620 qnngds-2.0.1/src/qnngds/devices/snspd.py
--rw-r--r--   0        0        0     1237 2024-04-22 18:39:28.969620 qnngds-2.0.1/src/qnngds/geometries.py
--rw-r--r--   0        0        0     6990 2024-04-22 18:39:28.969620 qnngds-2.0.1/src/qnngds/tests.py
--rw-r--r--   0        0        0    21030 2024-04-22 18:39:28.969620 qnngds-2.0.1/src/qnngds/utilities.py
--rw-r--r--   0        0        0     3309 1970-01-01 00:00:00.000000 qnngds-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-04-23 13:35:05.217164 qnngds-2.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     1129 2024-04-23 13:35:05.217164 qnngds-2.0.2/README.md
+-rw-r--r--   0        0        0     1161 2024-04-23 13:35:13.321177 qnngds-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0      508 2024-04-23 13:35:05.233164 qnngds-2.0.2/src/qnngds/__init__.py
+-rw-r--r--   0        0        0      291 2024-04-23 13:35:05.233164 qnngds-2.0.2/src/qnngds/_default_param.py
+-rw-r--r--   0        0        0    22568 2024-04-23 13:35:05.233164 qnngds-2.0.2/src/qnngds/cells.py
+-rw-r--r--   0        0        0    10495 2024-04-23 13:35:05.233164 qnngds-2.0.2/src/qnngds/circuits.py
+-rw-r--r--   0        0        0    28386 2024-04-23 13:35:05.233164 qnngds-2.0.2/src/qnngds/design.py
+-rw-r--r--   0        0        0      160 2024-04-23 13:35:05.233164 qnngds-2.0.2/src/qnngds/devices/__init__.py
+-rw-r--r--   0        0        0       90 2024-04-23 13:35:05.233164 qnngds-2.0.2/src/qnngds/devices/htron.py
+-rw-r--r--   0        0        0     1177 2024-04-23 13:35:05.233164 qnngds-2.0.2/src/qnngds/devices/nanowire.py
+-rw-r--r--   0        0        0     4453 2024-04-23 13:35:05.233164 qnngds-2.0.2/src/qnngds/devices/ntron.py
+-rw-r--r--   0        0        0     5860 2024-04-23 13:35:05.233164 qnngds-2.0.2/src/qnngds/devices/resistor.py
+-rw-r--r--   0        0        0     2376 2024-04-23 13:35:05.233164 qnngds-2.0.2/src/qnngds/devices/snspd.py
+-rw-r--r--   0        0        0     1237 2024-04-23 13:35:05.233164 qnngds-2.0.2/src/qnngds/geometries.py
+-rw-r--r--   0        0        0     6990 2024-04-23 13:35:05.233164 qnngds-2.0.2/src/qnngds/tests.py
+-rw-r--r--   0        0        0    21030 2024-04-23 13:35:05.233164 qnngds-2.0.2/src/qnngds/utilities.py
+-rw-r--r--   0        0        0     3309 1970-01-01 00:00:00.000000 qnngds-2.0.2/PKG-INFO
```

### Comparing `qnngds-2.0.1/LICENSE.txt` & `qnngds-2.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qnngds-2.0.1/README.md` & `qnngds-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `qnngds-2.0.1/pyproject.toml` & `qnngds-2.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "qnngds"
-version = "2.0.1"
+version = "2.0.2"
 authors = [
     { name = "A. Jacquillat", email = "audrey01@mit.edu" },
     { name = "A. Jacquillat", email = "audrey.jacquillat@gmail.com" },
     { name = "R. Foster", email = "reedf@mit.edu" },
 ]
 maintainers = [
     { name = "A. Jacquillat", email = "audrey01@mit.edu" },
```

### Comparing `qnngds-2.0.1/src/qnngds/cells.py` & `qnngds-2.0.2/src/qnngds/cells.py`

 * *Files identical despite different names*

### Comparing `qnngds-2.0.1/src/qnngds/circuits.py` & `qnngds-2.0.2/src/qnngds/circuits.py`

 * *Files identical despite different names*

### Comparing `qnngds-2.0.1/src/qnngds/design.py` & `qnngds-2.0.2/src/qnngds/design.py`

 * *Files identical despite different names*

### Comparing `qnngds-2.0.1/src/qnngds/devices/nanowire.py` & `qnngds-2.0.2/src/qnngds/devices/nanowire.py`

 * *Files identical despite different names*

### Comparing `qnngds-2.0.1/src/qnngds/devices/ntron.py` & `qnngds-2.0.2/src/qnngds/devices/ntron.py`

 * *Files identical despite different names*

### Comparing `qnngds-2.0.1/src/qnngds/devices/resistor.py` & `qnngds-2.0.2/src/qnngds/devices/resistor.py`

 * *Files identical despite different names*

### Comparing `qnngds-2.0.1/src/qnngds/devices/snspd.py` & `qnngds-2.0.2/src/qnngds/devices/snspd.py`

 * *Files identical despite different names*

### Comparing `qnngds-2.0.1/src/qnngds/geometries.py` & `qnngds-2.0.2/src/qnngds/geometries.py`

 * *Files identical despite different names*

### Comparing `qnngds-2.0.1/src/qnngds/tests.py` & `qnngds-2.0.2/src/qnngds/tests.py`

 * *Files identical despite different names*

### Comparing `qnngds-2.0.1/src/qnngds/utilities.py` & `qnngds-2.0.2/src/qnngds/utilities.py`

 * *Files identical despite different names*

### Comparing `qnngds-2.0.1/PKG-INFO` & `qnngds-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qnngds
-Version: 2.0.1
+Version: 2.0.2
 Summary: The QNN library for creating gds files
 Keywords: phidl,nanowire_electronics,nanofabrication,gds
 Author-Email: "A. Jacquillat" <audrey01@mit.edu>, "A. Jacquillat" <audrey.jacquillat@gmail.com>, "R. Foster" <reedf@mit.edu>
 Maintainer-Email: "A. Jacquillat" <audrey01@mit.edu>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
```

