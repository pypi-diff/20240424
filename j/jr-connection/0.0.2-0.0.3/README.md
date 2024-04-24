# Comparing `tmp/jr_connection-0.0.2.tar.gz` & `tmp/jr_connection-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "jr_connection-0.0.3.tar", last modified: Tue Apr 23 21:43:14 2024, max compression
```

## Comparing `jr_connection-0.0.2.tar` & `jr_connection-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,27 @@
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 jr_connection-0.0.2/requirements.txt
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 jr_connection-0.0.2/setup.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 jr_connection-0.0.2/src/jr_connection/__init__.py
--rwxr-xr-x   0        0        0     2931 2020-02-02 00:00:00.000000 jr_connection-0.0.2/src/jr_connection/first_run.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 jr_connection-0.0.2/src/jr_connection/other_constants.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 jr_connection-0.0.2/src/jr_connection/classes/__init__.py
--rw-r--r--   0        0        0     4801 2020-02-02 00:00:00.000000 jr_connection-0.0.2/src/jr_connection/classes/connection_class.py
--rw-r--r--   0        0        0     5504 2020-02-02 00:00:00.000000 jr_connection-0.0.2/src/jr_connection/classes/data_handler_class.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 jr_connection-0.0.2/src/jr_connection/classes/dbconfig_class.py
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 jr_connection-0.0.2/tests/test_connection_class.py
--rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 jr_connection-0.0.2/tests/test_data_handler_class.py
--rw-r--r--   0        0        0     3558 2020-02-02 00:00:00.000000 jr_connection-0.0.2/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 jr_connection-0.0.2/LICENSE
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 jr_connection-0.0.2/README.md
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 jr_connection-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 jr_connection-0.0.2/PKG-INFO
+drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-23 21:43:14.658854 jr_connection-0.0.3/
+-rw-r--r--   0 felipeburry   (501) staff       (20)     1072 2024-04-17 14:52:47.000000 jr_connection-0.0.3/LICENSE
+-rw-r--r--   0 felipeburry   (501) staff       (20)     2505 2024-04-23 21:43:14.658591 jr_connection-0.0.3/PKG-INFO
+-rw-r--r--   0 felipeburry   (501) staff       (20)       16 2024-04-17 14:49:29.000000 jr_connection-0.0.3/README.md
+-rw-r--r--   0 felipeburry   (501) staff       (20)     1124 2024-04-23 21:39:58.000000 jr_connection-0.0.3/pyproject.toml
+-rw-r--r--   0 felipeburry   (501) staff       (20)       38 2024-04-23 21:43:14.658911 jr_connection-0.0.3/setup.cfg
+-rw-r--r--   0 felipeburry   (501) staff       (20)      737 2024-04-23 21:40:07.000000 jr_connection-0.0.3/setup.py
+drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-23 21:43:14.653769 jr_connection-0.0.3/src/
+drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-23 21:43:14.655313 jr_connection-0.0.3/src/jr_connection/
+-rw-r--r--   0 felipeburry   (501) staff       (20)      137 2024-04-17 16:03:22.000000 jr_connection-0.0.3/src/jr_connection/__init__.py
+drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-23 21:43:14.657456 jr_connection-0.0.3/src/jr_connection/classes/
+-rw-r--r--   0 felipeburry   (501) staff       (20)       85 2024-04-17 16:02:57.000000 jr_connection-0.0.3/src/jr_connection/classes/__init__.py
+-rw-r--r--   0 felipeburry   (501) staff       (20)     4802 2024-04-23 21:38:06.000000 jr_connection-0.0.3/src/jr_connection/classes/connection_class.py
+-rw-r--r--   0 felipeburry   (501) staff       (20)     5504 2024-04-17 19:15:46.000000 jr_connection-0.0.3/src/jr_connection/classes/data_handler_class.py
+-rw-r--r--   0 felipeburry   (501) staff       (20)      429 2024-04-17 17:59:39.000000 jr_connection-0.0.3/src/jr_connection/classes/dbconfig_class.py
+-rwxr-xr-x   0 felipeburry   (501) staff       (20)     2931 2024-04-17 19:01:30.000000 jr_connection-0.0.3/src/jr_connection/first_run.py
+-rw-r--r--   0 felipeburry   (501) staff       (20)      154 2024-04-17 18:00:05.000000 jr_connection-0.0.3/src/jr_connection/other_constants.py
+drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-23 21:43:14.656427 jr_connection-0.0.3/src/jr_connection.egg-info/
+-rw-r--r--   0 felipeburry   (501) staff       (20)     2505 2024-04-23 21:43:14.000000 jr_connection-0.0.3/src/jr_connection.egg-info/PKG-INFO
+-rw-r--r--   0 felipeburry   (501) staff       (20)      627 2024-04-23 21:43:14.000000 jr_connection-0.0.3/src/jr_connection.egg-info/SOURCES.txt
+-rw-r--r--   0 felipeburry   (501) staff       (20)        1 2024-04-23 21:43:14.000000 jr_connection-0.0.3/src/jr_connection.egg-info/dependency_links.txt
+-rw-r--r--   0 felipeburry   (501) staff       (20)       59 2024-04-23 21:43:14.000000 jr_connection-0.0.3/src/jr_connection.egg-info/entry_points.txt
+-rw-r--r--   0 felipeburry   (501) staff       (20)      331 2024-04-23 21:43:14.000000 jr_connection-0.0.3/src/jr_connection.egg-info/requires.txt
+-rw-r--r--   0 felipeburry   (501) staff       (20)       14 2024-04-23 21:43:14.000000 jr_connection-0.0.3/src/jr_connection.egg-info/top_level.txt
+drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-23 21:43:14.658016 jr_connection-0.0.3/tests/
+-rw-r--r--   0 felipeburry   (501) staff       (20)     2007 2024-04-17 18:31:52.000000 jr_connection-0.0.3/tests/test_connection_class.py
+-rw-r--r--   0 felipeburry   (501) staff       (20)     2503 2024-04-17 18:48:40.000000 jr_connection-0.0.3/tests/test_data_handler_class.py
```

### Comparing `jr_connection-0.0.2/setup.py` & `jr_connection-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="jr_connection",
-    version="0.1",
+    version="0.0.3",
     description="A simple python package to connect to JR servers and get the data",
     long_description="lalala",
     url="https://github.com/faburry23/JR_Connection",
     author="Felipe Burry",
     author_email="felipe.burry@jriveros.cl",
     license="MIT",
     package_dir={"": "src"},
```

### Comparing `jr_connection-0.0.2/src/jr_connection/first_run.py` & `jr_connection-0.0.3/src/jr_connection/first_run.py`

 * *Files identical despite different names*

### Comparing `jr_connection-0.0.2/src/jr_connection/classes/connection_class.py` & `jr_connection-0.0.3/src/jr_connection/classes/connection_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import pandas as pd
 from sqlalchemy import create_engine, text
 from sqlalchemy.exc import SQLAlchemyError
 
 # Local Application/Library Specific Imports
 from .dbconfig_class import DBConfig
 
+
 class Connection:
     """
     Gestiona la conexión a la base de datos y las operaciones de recuperación de datos.
 
     Esta clase se encarga de establecer la conexión con la base de datos usando las credenciales
     cargadas y proporciona métodos para obtener datos de la base de datos y almacenarlos localmente.
 
@@ -25,15 +26,15 @@
     Métodos:
     --------
     create_connection_string(credentials): Construye una cadena de conexión usando las credenciales proporcionadas.
     create_db_engine(): Crea y retorna un motor de base de datos.
     test_db_connection(): Verifica y retorna el estado de la conexión a la base de datos.
     get_data(table_name): Recupera datos de una tabla especificada y los almacena como archivos Parquet.
     """
-     
+
     def __init__(self):
         """
         Inicializa la conexión a la base de datos cargando las credenciales, construyendo la cadena
         de conexión, creando el motor de base de datos y verificando la conexión.
         """
         self.credentials = DBConfig.load_credentials()
         self.connection_string = self.create_connection_string(self.credentials)
@@ -100,15 +101,14 @@
                 result.fetchone()
                 self.is_connected = True
                 return self.is_connected
         except Exception as e:
             self.is_connected = False
             return self.is_connected
 
-
     def get_data(self, table_name):
         """
         Recupera datos de la tabla especificada y los almacena localmente en formato Parquet.
 
         Parámetros:
         -----------
         table_name (str): Nombre de la tabla de la cual se recuperarán los datos.
@@ -119,17 +119,16 @@
             DataFrame de pandas que contiene los datos recuperados.
 
         Ejemplo:
         --------
         df = self.get_data('tabla')
         """
         with self.engine.begin() as conn:
-            query = text(f"""
+            query = text(
+                f"""
                     SELECT *
                     FROM {table_name}
                     """
-                )
+            )
             df = pd.read_sql_query(query, conn)
-            df.to_parquet(f"./data/raw/{f"{table_name}.parquet"}")
+            df.to_parquet(f"./data/raw/{table_name}.parquet")
         return df
-
-
```

### Comparing `jr_connection-0.0.2/src/jr_connection/classes/data_handler_class.py` & `jr_connection-0.0.3/src/jr_connection/classes/data_handler_class.py`

 * *Files identical despite different names*

### Comparing `jr_connection-0.0.2/tests/test_connection_class.py` & `jr_connection-0.0.3/tests/test_connection_class.py`

 * *Files identical despite different names*

### Comparing `jr_connection-0.0.2/tests/test_data_handler_class.py` & `jr_connection-0.0.3/tests/test_data_handler_class.py`

 * *Files identical despite different names*

### Comparing `jr_connection-0.0.2/LICENSE` & `jr_connection-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jr_connection-0.0.2/pyproject.toml` & `jr_connection-0.0.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jr_connection"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Felipe Burry", email="felipe.burry@jriveros.cl" },
 ]
 description = "A simple python package to connect to JR servers and get the data"
+license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [
     "cramjam==2.8.3",
     "et-xmlfile==1.1.0",
     "fastparquet==2024.2.0",
     "fsspec==2024.3.1",
```

