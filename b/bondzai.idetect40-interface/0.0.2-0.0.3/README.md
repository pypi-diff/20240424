# Comparing `tmp/bondzai.idetect40-interface-0.0.2.tar.gz` & `tmp/bondzai.idetect40-interface-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bondzai.idetect40-interface-0.0.2.tar", last modified: Wed Apr 24 14:32:44 2024, max compression
+gzip compressed data, was "bondzai.idetect40-interface-0.0.3.tar", last modified: Wed Apr 24 16:03:10 2024, max compression
```

## Comparing `bondzai.idetect40-interface-0.0.2.tar` & `bondzai.idetect40-interface-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 14:32:44.783136 bondzai.idetect40-interface-0.0.2/
--rw-rw-rw-   0        0        0      547 2023-10-17 12:30:45.000000 bondzai.idetect40-interface-0.0.2/NOTICE
--rw-rw-rw-   0        0        0      805 2024-04-24 14:32:44.783687 bondzai.idetect40-interface-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      360 2024-04-24 10:47:45.000000 bondzai.idetect40-interface-0.0.2/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-24 14:32:44.761988 bondzai.idetect40-interface-0.0.2/bondzai/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:32:44.769122 bondzai.idetect40-interface-0.0.2/bondzai/idetect40_interface/
--rw-rw-rw-   0        0        0       22 2024-04-24 14:31:55.000000 bondzai.idetect40-interface-0.0.2/bondzai/idetect40_interface/__init__.py
--rw-rw-rw-   0        0        0     2429 2024-04-24 10:29:44.000000 bondzai.idetect40-interface-0.0.2/bondzai/idetect40_interface/dict.py
--rw-rw-rw-   0        0        0    13464 2024-04-24 14:26:44.000000 bondzai.idetect40-interface-0.0.2/bondzai/idetect40_interface/exchange_table.py
--rw-rw-rw-   0        0        0       66 2024-04-24 13:20:02.000000 bondzai.idetect40-interface-0.0.2/bondzai/idetect40_interface/poc.py
--rw-rw-rw-   0        0        0    11553 2024-04-22 15:43:39.000000 bondzai.idetect40-interface-0.0.2/bondzai/idetect40_interface/socket.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:32:44.782041 bondzai.idetect40-interface-0.0.2/bondzai.idetect40_interface.egg-info/
--rw-rw-rw-   0        0        0      805 2024-04-24 14:32:44.000000 bondzai.idetect40-interface-0.0.2/bondzai.idetect40_interface.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      955 2024-04-24 14:32:44.000000 bondzai.idetect40-interface-0.0.2/bondzai.idetect40_interface.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 14:32:44.000000 bondzai.idetect40-interface-0.0.2/bondzai.idetect40_interface.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-24 14:32:44.000000 bondzai.idetect40-interface-0.0.2/bondzai.idetect40_interface.egg-info/namespace_packages.txt
--rw-rw-rw-   0        0        0       28 2024-04-24 14:32:44.000000 bondzai.idetect40-interface-0.0.2/bondzai.idetect40_interface.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-24 14:32:44.000000 bondzai.idetect40-interface-0.0.2/bondzai.idetect40_interface.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-04-24 14:32:44.000000 bondzai.idetect40-interface-0.0.2/bondzai.idetect40_interface.egg-info/zip-safe
--rw-rw-rw-   0        0        0       71 2023-10-17 12:30:45.000000 bondzai.idetect40-interface-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      733 2024-04-24 14:32:44.784844 bondzai.idetect40-interface-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0       36 2023-10-17 12:30:45.000000 bondzai.idetect40-interface-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:32:44.771000 bondzai.idetect40-interface-0.0.2/tests/
--rw-rw-rw-   0        0        0     2383 2024-04-24 10:29:44.000000 bondzai.idetect40-interface-0.0.2/tests/test_dict.py
--rw-rw-rw-   0        0        0     4578 2024-04-24 14:26:44.000000 bondzai.idetect40-interface-0.0.2/tests/test_exchange_table.py
--rw-rw-rw-   0        0        0     5998 2024-04-24 10:33:37.000000 bondzai.idetect40-interface-0.0.2/tests/test_socket.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:03:10.488548 bondzai.idetect40-interface-0.0.3/
+-rw-rw-rw-   0        0        0      547 2023-10-17 12:30:45.000000 bondzai.idetect40-interface-0.0.3/NOTICE
+-rw-rw-rw-   0        0        0      805 2024-04-24 16:03:10.488548 bondzai.idetect40-interface-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2024-04-24 10:47:45.000000 bondzai.idetect40-interface-0.0.3/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-24 16:03:10.471052 bondzai.idetect40-interface-0.0.3/bondzai/
+drwxrwxrwx   0        0        0        0 2024-04-24 16:03:10.479230 bondzai.idetect40-interface-0.0.3/bondzai/idetect40_interface/
+-rw-rw-rw-   0        0        0       22 2024-04-24 16:02:46.000000 bondzai.idetect40-interface-0.0.3/bondzai/idetect40_interface/__init__.py
+-rw-rw-rw-   0        0        0     2429 2024-04-24 10:29:44.000000 bondzai.idetect40-interface-0.0.3/bondzai/idetect40_interface/dict.py
+-rw-rw-rw-   0        0        0    13464 2024-04-24 14:26:44.000000 bondzai.idetect40-interface-0.0.3/bondzai/idetect40_interface/exchange_table.py
+-rw-rw-rw-   0        0        0    11553 2024-04-22 15:43:39.000000 bondzai.idetect40-interface-0.0.3/bondzai/idetect40_interface/socket.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:03:10.487485 bondzai.idetect40-interface-0.0.3/bondzai.idetect40_interface.egg-info/
+-rw-rw-rw-   0        0        0      805 2024-04-24 16:03:10.000000 bondzai.idetect40-interface-0.0.3/bondzai.idetect40_interface.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      883 2024-04-24 16:03:10.000000 bondzai.idetect40-interface-0.0.3/bondzai.idetect40_interface.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 16:03:10.000000 bondzai.idetect40-interface-0.0.3/bondzai.idetect40_interface.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-24 16:03:10.000000 bondzai.idetect40-interface-0.0.3/bondzai.idetect40_interface.egg-info/namespace_packages.txt
+-rw-rw-rw-   0        0        0       28 2024-04-24 16:03:10.000000 bondzai.idetect40-interface-0.0.3/bondzai.idetect40_interface.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-24 16:03:10.000000 bondzai.idetect40-interface-0.0.3/bondzai.idetect40_interface.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-24 16:03:10.000000 bondzai.idetect40-interface-0.0.3/bondzai.idetect40_interface.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       71 2023-10-17 12:30:45.000000 bondzai.idetect40-interface-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      733 2024-04-24 16:03:10.490719 bondzai.idetect40-interface-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0       36 2023-10-17 12:30:45.000000 bondzai.idetect40-interface-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:03:10.480878 bondzai.idetect40-interface-0.0.3/tests/
+-rw-rw-rw-   0        0        0     2383 2024-04-24 10:29:44.000000 bondzai.idetect40-interface-0.0.3/tests/test_dict.py
+-rw-rw-rw-   0        0        0     4578 2024-04-24 14:26:44.000000 bondzai.idetect40-interface-0.0.3/tests/test_exchange_table.py
+-rw-rw-rw-   0        0        0     5998 2024-04-24 10:33:37.000000 bondzai.idetect40-interface-0.0.3/tests/test_socket.py
```

### Comparing `bondzai.idetect40-interface-0.0.2/NOTICE` & `bondzai.idetect40-interface-0.0.3/NOTICE`

 * *Files identical despite different names*

### Comparing `bondzai.idetect40-interface-0.0.2/PKG-INFO` & `bondzai.idetect40-interface-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.idetect40-interface
-Version: 0.0.2
+Version: 0.0.3
 Summary: Bondzai iDetect 4.0 interface
 Home-page: UNKNOWN
 Author: Bondzai
 License: Apache License 2.0
 Keywords: davinsy,bondzai,idetect40
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.idetect40-interface-0.0.2/bondzai/idetect40_interface/dict.py` & `bondzai.idetect40-interface-0.0.3/bondzai/idetect40_interface/dict.py`

 * *Files identical despite different names*

### Comparing `bondzai.idetect40-interface-0.0.2/bondzai/idetect40_interface/exchange_table.py` & `bondzai.idetect40-interface-0.0.3/bondzai/idetect40_interface/exchange_table.py`

 * *Files identical despite different names*

### Comparing `bondzai.idetect40-interface-0.0.2/bondzai/idetect40_interface/socket.py` & `bondzai.idetect40-interface-0.0.3/bondzai/idetect40_interface/socket.py`

 * *Files identical despite different names*

### Comparing `bondzai.idetect40-interface-0.0.2/bondzai.idetect40_interface.egg-info/PKG-INFO` & `bondzai.idetect40-interface-0.0.3/bondzai.idetect40_interface.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.idetect40-interface
-Version: 0.0.2
+Version: 0.0.3
 Summary: Bondzai iDetect 4.0 interface
 Home-page: UNKNOWN
 Author: Bondzai
 License: Apache License 2.0
 Keywords: davinsy,bondzai,idetect40
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.idetect40-interface-0.0.2/bondzai.idetect40_interface.egg-info/SOURCES.txt` & `bondzai.idetect40-interface-0.0.3/bondzai.idetect40_interface.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -2,27 +2,25 @@
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
 ./bondzai/idetect40_interface/__init__.py
 ./bondzai/idetect40_interface/dict.py
 ./bondzai/idetect40_interface/exchange_table.py
-./bondzai/idetect40_interface/poc.py
 ./bondzai/idetect40_interface/socket.py
 ./tests/test_dict.py
 ./tests/test_exchange_table.py
 ./tests/test_socket.py
 bondzai.idetect40_interface.egg-info/PKG-INFO
 bondzai.idetect40_interface.egg-info/SOURCES.txt
 bondzai.idetect40_interface.egg-info/dependency_links.txt
 bondzai.idetect40_interface.egg-info/namespace_packages.txt
 bondzai.idetect40_interface.egg-info/requires.txt
 bondzai.idetect40_interface.egg-info/top_level.txt
 bondzai.idetect40_interface.egg-info/zip-safe
 bondzai/idetect40_interface/__init__.py
 bondzai/idetect40_interface/dict.py
 bondzai/idetect40_interface/exchange_table.py
-bondzai/idetect40_interface/poc.py
 bondzai/idetect40_interface/socket.py
 tests/test_dict.py
 tests/test_exchange_table.py
 tests/test_socket.py
```

### Comparing `bondzai.idetect40-interface-0.0.2/setup.cfg` & `bondzai.idetect40-interface-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `bondzai.idetect40-interface-0.0.2/tests/test_dict.py` & `bondzai.idetect40-interface-0.0.3/tests/test_dict.py`

 * *Files identical despite different names*

### Comparing `bondzai.idetect40-interface-0.0.2/tests/test_exchange_table.py` & `bondzai.idetect40-interface-0.0.3/tests/test_exchange_table.py`

 * *Files identical despite different names*

### Comparing `bondzai.idetect40-interface-0.0.2/tests/test_socket.py` & `bondzai.idetect40-interface-0.0.3/tests/test_socket.py`

 * *Files identical despite different names*

