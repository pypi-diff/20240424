# Comparing `tmp/jr_connection-0.1.1.tar.gz` & `tmp/jr_connection-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jr_connection-0.1.1.tar", last modified: Wed Apr 24 18:46:43 2024, max compression
+gzip compressed data, was "jr_connection-0.1.2.tar", last modified: Wed Apr 24 18:52:39 2024, max compression
```

## Comparing `jr_connection-0.1.1.tar` & `jr_connection-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-24 18:46:43.244496 jr_connection-0.1.1/
--rw-r--r--   0 felipeburry   (501) staff       (20)     1072 2024-04-17 14:52:47.000000 jr_connection-0.1.1/LICENSE
--rw-r--r--   0 felipeburry   (501) staff       (20)     2536 2024-04-24 18:46:43.244121 jr_connection-0.1.1/PKG-INFO
--rw-r--r--   0 felipeburry   (501) staff       (20)       16 2024-04-17 14:49:29.000000 jr_connection-0.1.1/README.md
--rw-r--r--   0 felipeburry   (501) staff       (20)     1148 2024-04-24 18:44:20.000000 jr_connection-0.1.1/pyproject.toml
--rw-r--r--   0 felipeburry   (501) staff       (20)       38 2024-04-24 18:46:43.244581 jr_connection-0.1.1/setup.cfg
--rw-r--r--   0 felipeburry   (501) staff       (20)      737 2024-04-24 18:44:27.000000 jr_connection-0.1.1/setup.py
-drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-24 18:46:43.236350 jr_connection-0.1.1/src/
-drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-24 18:46:43.238741 jr_connection-0.1.1/src/jr_connection/
--rw-r--r--   0 felipeburry   (501) staff       (20)      137 2024-04-17 16:03:22.000000 jr_connection-0.1.1/src/jr_connection/__init__.py
-drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-24 18:46:43.242316 jr_connection-0.1.1/src/jr_connection/classes/
--rw-r--r--   0 felipeburry   (501) staff       (20)       85 2024-04-17 16:02:57.000000 jr_connection-0.1.1/src/jr_connection/classes/__init__.py
--rw-r--r--   0 felipeburry   (501) staff       (20)     7514 2024-04-24 18:44:02.000000 jr_connection-0.1.1/src/jr_connection/classes/connection_class.py
--rw-r--r--   0 felipeburry   (501) staff       (20)     5504 2024-04-17 19:15:46.000000 jr_connection-0.1.1/src/jr_connection/classes/data_handler_class.py
--rw-r--r--   0 felipeburry   (501) staff       (20)      421 2024-04-24 18:38:17.000000 jr_connection-0.1.1/src/jr_connection/classes/dbconfig_class.py
--rwxr-xr-x   0 felipeburry   (501) staff       (20)     2932 2024-04-24 18:38:27.000000 jr_connection-0.1.1/src/jr_connection/first_run.py
--rw-r--r--   0 felipeburry   (501) staff       (20)      154 2024-04-17 18:00:05.000000 jr_connection-0.1.1/src/jr_connection/other_constants.py
-drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-24 18:46:43.240583 jr_connection-0.1.1/src/jr_connection.egg-info/
--rw-r--r--   0 felipeburry   (501) staff       (20)     2536 2024-04-24 18:46:43.000000 jr_connection-0.1.1/src/jr_connection.egg-info/PKG-INFO
--rw-r--r--   0 felipeburry   (501) staff       (20)      627 2024-04-24 18:46:43.000000 jr_connection-0.1.1/src/jr_connection.egg-info/SOURCES.txt
--rw-r--r--   0 felipeburry   (501) staff       (20)        1 2024-04-24 18:46:43.000000 jr_connection-0.1.1/src/jr_connection.egg-info/dependency_links.txt
--rw-r--r--   0 felipeburry   (501) staff       (20)       59 2024-04-24 18:46:43.000000 jr_connection-0.1.1/src/jr_connection.egg-info/entry_points.txt
--rw-r--r--   0 felipeburry   (501) staff       (20)      347 2024-04-24 18:46:43.000000 jr_connection-0.1.1/src/jr_connection.egg-info/requires.txt
--rw-r--r--   0 felipeburry   (501) staff       (20)       14 2024-04-24 18:46:43.000000 jr_connection-0.1.1/src/jr_connection.egg-info/top_level.txt
-drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-24 18:46:43.243207 jr_connection-0.1.1/tests/
--rw-r--r--   0 felipeburry   (501) staff       (20)     2007 2024-04-17 18:31:52.000000 jr_connection-0.1.1/tests/test_connection_class.py
--rw-r--r--   0 felipeburry   (501) staff       (20)     2503 2024-04-17 18:48:40.000000 jr_connection-0.1.1/tests/test_data_handler_class.py
+drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-24 18:52:39.013436 jr_connection-0.1.2/
+-rw-r--r--   0 felipeburry   (501) staff       (20)     1072 2024-04-17 14:52:47.000000 jr_connection-0.1.2/LICENSE
+-rw-r--r--   0 felipeburry   (501) staff       (20)     2536 2024-04-24 18:52:39.013028 jr_connection-0.1.2/PKG-INFO
+-rw-r--r--   0 felipeburry   (501) staff       (20)       16 2024-04-17 14:49:29.000000 jr_connection-0.1.2/README.md
+-rw-r--r--   0 felipeburry   (501) staff       (20)     1148 2024-04-24 18:52:13.000000 jr_connection-0.1.2/pyproject.toml
+-rw-r--r--   0 felipeburry   (501) staff       (20)       38 2024-04-24 18:52:39.013533 jr_connection-0.1.2/setup.cfg
+-rw-r--r--   0 felipeburry   (501) staff       (20)      737 2024-04-24 18:52:16.000000 jr_connection-0.1.2/setup.py
+drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-24 18:52:39.006232 jr_connection-0.1.2/src/
+drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-24 18:52:39.008248 jr_connection-0.1.2/src/jr_connection/
+-rw-r--r--   0 felipeburry   (501) staff       (20)      137 2024-04-17 16:03:22.000000 jr_connection-0.1.2/src/jr_connection/__init__.py
+drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-24 18:52:39.011717 jr_connection-0.1.2/src/jr_connection/classes/
+-rw-r--r--   0 felipeburry   (501) staff       (20)      104 2024-04-24 18:51:26.000000 jr_connection-0.1.2/src/jr_connection/classes/__init__.py
+-rw-r--r--   0 felipeburry   (501) staff       (20)     7506 2024-04-24 18:51:19.000000 jr_connection-0.1.2/src/jr_connection/classes/connection_class.py
+-rw-r--r--   0 felipeburry   (501) staff       (20)     5504 2024-04-17 19:15:46.000000 jr_connection-0.1.2/src/jr_connection/classes/data_handler_class.py
+-rw-r--r--   0 felipeburry   (501) staff       (20)      421 2024-04-24 18:38:17.000000 jr_connection-0.1.2/src/jr_connection/classes/dbconfig_class.py
+-rwxr-xr-x   0 felipeburry   (501) staff       (20)     2932 2024-04-24 18:38:27.000000 jr_connection-0.1.2/src/jr_connection/first_run.py
+-rw-r--r--   0 felipeburry   (501) staff       (20)      154 2024-04-17 18:00:05.000000 jr_connection-0.1.2/src/jr_connection/other_constants.py
+drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-24 18:52:39.009821 jr_connection-0.1.2/src/jr_connection.egg-info/
+-rw-r--r--   0 felipeburry   (501) staff       (20)     2536 2024-04-24 18:52:38.000000 jr_connection-0.1.2/src/jr_connection.egg-info/PKG-INFO
+-rw-r--r--   0 felipeburry   (501) staff       (20)      627 2024-04-24 18:52:38.000000 jr_connection-0.1.2/src/jr_connection.egg-info/SOURCES.txt
+-rw-r--r--   0 felipeburry   (501) staff       (20)        1 2024-04-24 18:52:38.000000 jr_connection-0.1.2/src/jr_connection.egg-info/dependency_links.txt
+-rw-r--r--   0 felipeburry   (501) staff       (20)       59 2024-04-24 18:52:38.000000 jr_connection-0.1.2/src/jr_connection.egg-info/entry_points.txt
+-rw-r--r--   0 felipeburry   (501) staff       (20)      347 2024-04-24 18:52:38.000000 jr_connection-0.1.2/src/jr_connection.egg-info/requires.txt
+-rw-r--r--   0 felipeburry   (501) staff       (20)       14 2024-04-24 18:52:38.000000 jr_connection-0.1.2/src/jr_connection.egg-info/top_level.txt
+drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-24 18:52:39.012319 jr_connection-0.1.2/tests/
+-rw-r--r--   0 felipeburry   (501) staff       (20)     2007 2024-04-17 18:31:52.000000 jr_connection-0.1.2/tests/test_connection_class.py
+-rw-r--r--   0 felipeburry   (501) staff       (20)     2503 2024-04-17 18:48:40.000000 jr_connection-0.1.2/tests/test_data_handler_class.py
```

### Comparing `jr_connection-0.1.1/LICENSE` & `jr_connection-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jr_connection-0.1.1/PKG-INFO` & `jr_connection-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jr_connection
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple python package to connect to JR servers and get the data
 Home-page: https://github.com/faburry23/JR_Connection
 Author: Felipe Burry
 Author-email: Felipe Burry <felipe.burry@jriveros.cl>
 License: MIT License
         
         Copyright (c) [2024] [Felipe Burry]
```

### Comparing `jr_connection-0.1.1/pyproject.toml` & `jr_connection-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jr_connection"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Felipe Burry", email="felipe.burry@jriveros.cl" },
 ]
 description = "A simple python package to connect to JR servers and get the data"
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.11"
```

### Comparing `jr_connection-0.1.1/setup.py` & `jr_connection-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="jr_connection",
-    version="0.1.1",
+    version="0.1.2",
     description="A simple python package to connect to JR servers and get the data",
     long_description="lalala",
     url="https://github.com/faburry23/JR_Connection",
     author="Felipe Burry",
     author_email="felipe.burry@jriveros.cl",
     license="MIT",
     package_dir={"": "src"},
```

### Comparing `jr_connection-0.1.1/src/jr_connection/classes/connection_class.py` & `jr_connection-0.1.2/src/jr_connection/classes/connection_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from sqlalchemy.exc import SQLAlchemyError
 import os
 
 # Local Application/Library Specific Imports
 from .dbconfig_class import DBConfig
 
 
-class ConnectionMSServer:
+class Connection:
     """
     Gestiona la conexión a la base de datos y las operaciones de recuperación de datos.
 
     Esta clase se encarga de establecer la conexión con la base de datos usando las credenciales
     cargadas y proporciona métodos para obtener datos de la base de datos y almacenarlos localmente.
 
     Atributos:
```

### Comparing `jr_connection-0.1.1/src/jr_connection/classes/data_handler_class.py` & `jr_connection-0.1.2/src/jr_connection/classes/data_handler_class.py`

 * *Files identical despite different names*

### Comparing `jr_connection-0.1.1/src/jr_connection/first_run.py` & `jr_connection-0.1.2/src/jr_connection/first_run.py`

 * *Files identical despite different names*

### Comparing `jr_connection-0.1.1/src/jr_connection.egg-info/PKG-INFO` & `jr_connection-0.1.2/src/jr_connection.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jr-connection
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple python package to connect to JR servers and get the data
 Home-page: https://github.com/faburry23/JR_Connection
 Author: Felipe Burry
 Author-email: Felipe Burry <felipe.burry@jriveros.cl>
 License: MIT License
         
         Copyright (c) [2024] [Felipe Burry]
```

### Comparing `jr_connection-0.1.1/src/jr_connection.egg-info/SOURCES.txt` & `jr_connection-0.1.2/src/jr_connection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jr_connection-0.1.1/tests/test_connection_class.py` & `jr_connection-0.1.2/tests/test_connection_class.py`

 * *Files identical despite different names*

### Comparing `jr_connection-0.1.1/tests/test_data_handler_class.py` & `jr_connection-0.1.2/tests/test_data_handler_class.py`

 * *Files identical despite different names*

