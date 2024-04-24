# Comparing `tmp/jr_connection-0.1.0.tar.gz` & `tmp/jr_connection-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jr_connection-0.1.0.tar", last modified: Wed Apr 24 15:28:06 2024, max compression
+gzip compressed data, was "jr_connection-0.1.1.tar", last modified: Wed Apr 24 18:46:43 2024, max compression
```

## Comparing `jr_connection-0.1.0.tar` & `jr_connection-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-24 15:28:06.148231 jr_connection-0.1.0/
--rw-r--r--   0 felipeburry   (501) staff       (20)     1072 2024-04-17 14:52:47.000000 jr_connection-0.1.0/LICENSE
--rw-r--r--   0 felipeburry   (501) staff       (20)     2536 2024-04-24 15:28:06.147797 jr_connection-0.1.0/PKG-INFO
--rw-r--r--   0 felipeburry   (501) staff       (20)       16 2024-04-17 14:49:29.000000 jr_connection-0.1.0/README.md
--rw-r--r--   0 felipeburry   (501) staff       (20)     1148 2024-04-24 15:25:44.000000 jr_connection-0.1.0/pyproject.toml
--rw-r--r--   0 felipeburry   (501) staff       (20)       38 2024-04-24 15:28:06.148346 jr_connection-0.1.0/setup.cfg
--rw-r--r--   0 felipeburry   (501) staff       (20)      737 2024-04-24 15:25:47.000000 jr_connection-0.1.0/setup.py
-drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-24 15:28:06.138988 jr_connection-0.1.0/src/
-drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-24 15:28:06.141614 jr_connection-0.1.0/src/jr_connection/
--rw-r--r--   0 felipeburry   (501) staff       (20)      137 2024-04-17 16:03:22.000000 jr_connection-0.1.0/src/jr_connection/__init__.py
-drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-24 15:28:06.146056 jr_connection-0.1.0/src/jr_connection/classes/
--rw-r--r--   0 felipeburry   (501) staff       (20)       85 2024-04-17 16:02:57.000000 jr_connection-0.1.0/src/jr_connection/classes/__init__.py
--rw-r--r--   0 felipeburry   (501) staff       (20)     6132 2024-04-24 15:07:53.000000 jr_connection-0.1.0/src/jr_connection/classes/connection_class.py
--rw-r--r--   0 felipeburry   (501) staff       (20)     5504 2024-04-17 19:15:46.000000 jr_connection-0.1.0/src/jr_connection/classes/data_handler_class.py
--rw-r--r--   0 felipeburry   (501) staff       (20)      429 2024-04-17 17:59:39.000000 jr_connection-0.1.0/src/jr_connection/classes/dbconfig_class.py
--rwxr-xr-x   0 felipeburry   (501) staff       (20)     3118 2024-04-24 15:00:32.000000 jr_connection-0.1.0/src/jr_connection/first_run.py
--rw-r--r--   0 felipeburry   (501) staff       (20)      154 2024-04-17 18:00:05.000000 jr_connection-0.1.0/src/jr_connection/other_constants.py
-drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-24 15:28:06.143415 jr_connection-0.1.0/src/jr_connection.egg-info/
--rw-r--r--   0 felipeburry   (501) staff       (20)     2536 2024-04-24 15:28:06.000000 jr_connection-0.1.0/src/jr_connection.egg-info/PKG-INFO
--rw-r--r--   0 felipeburry   (501) staff       (20)      627 2024-04-24 15:28:06.000000 jr_connection-0.1.0/src/jr_connection.egg-info/SOURCES.txt
--rw-r--r--   0 felipeburry   (501) staff       (20)        1 2024-04-24 15:28:06.000000 jr_connection-0.1.0/src/jr_connection.egg-info/dependency_links.txt
--rw-r--r--   0 felipeburry   (501) staff       (20)       59 2024-04-24 15:28:06.000000 jr_connection-0.1.0/src/jr_connection.egg-info/entry_points.txt
--rw-r--r--   0 felipeburry   (501) staff       (20)      347 2024-04-24 15:28:06.000000 jr_connection-0.1.0/src/jr_connection.egg-info/requires.txt
--rw-r--r--   0 felipeburry   (501) staff       (20)       14 2024-04-24 15:28:06.000000 jr_connection-0.1.0/src/jr_connection.egg-info/top_level.txt
-drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-24 15:28:06.146867 jr_connection-0.1.0/tests/
--rw-r--r--   0 felipeburry   (501) staff       (20)     2007 2024-04-17 18:31:52.000000 jr_connection-0.1.0/tests/test_connection_class.py
--rw-r--r--   0 felipeburry   (501) staff       (20)     2503 2024-04-17 18:48:40.000000 jr_connection-0.1.0/tests/test_data_handler_class.py
+drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-24 18:46:43.244496 jr_connection-0.1.1/
+-rw-r--r--   0 felipeburry   (501) staff       (20)     1072 2024-04-17 14:52:47.000000 jr_connection-0.1.1/LICENSE
+-rw-r--r--   0 felipeburry   (501) staff       (20)     2536 2024-04-24 18:46:43.244121 jr_connection-0.1.1/PKG-INFO
+-rw-r--r--   0 felipeburry   (501) staff       (20)       16 2024-04-17 14:49:29.000000 jr_connection-0.1.1/README.md
+-rw-r--r--   0 felipeburry   (501) staff       (20)     1148 2024-04-24 18:44:20.000000 jr_connection-0.1.1/pyproject.toml
+-rw-r--r--   0 felipeburry   (501) staff       (20)       38 2024-04-24 18:46:43.244581 jr_connection-0.1.1/setup.cfg
+-rw-r--r--   0 felipeburry   (501) staff       (20)      737 2024-04-24 18:44:27.000000 jr_connection-0.1.1/setup.py
+drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-24 18:46:43.236350 jr_connection-0.1.1/src/
+drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-24 18:46:43.238741 jr_connection-0.1.1/src/jr_connection/
+-rw-r--r--   0 felipeburry   (501) staff       (20)      137 2024-04-17 16:03:22.000000 jr_connection-0.1.1/src/jr_connection/__init__.py
+drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-24 18:46:43.242316 jr_connection-0.1.1/src/jr_connection/classes/
+-rw-r--r--   0 felipeburry   (501) staff       (20)       85 2024-04-17 16:02:57.000000 jr_connection-0.1.1/src/jr_connection/classes/__init__.py
+-rw-r--r--   0 felipeburry   (501) staff       (20)     7514 2024-04-24 18:44:02.000000 jr_connection-0.1.1/src/jr_connection/classes/connection_class.py
+-rw-r--r--   0 felipeburry   (501) staff       (20)     5504 2024-04-17 19:15:46.000000 jr_connection-0.1.1/src/jr_connection/classes/data_handler_class.py
+-rw-r--r--   0 felipeburry   (501) staff       (20)      421 2024-04-24 18:38:17.000000 jr_connection-0.1.1/src/jr_connection/classes/dbconfig_class.py
+-rwxr-xr-x   0 felipeburry   (501) staff       (20)     2932 2024-04-24 18:38:27.000000 jr_connection-0.1.1/src/jr_connection/first_run.py
+-rw-r--r--   0 felipeburry   (501) staff       (20)      154 2024-04-17 18:00:05.000000 jr_connection-0.1.1/src/jr_connection/other_constants.py
+drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-24 18:46:43.240583 jr_connection-0.1.1/src/jr_connection.egg-info/
+-rw-r--r--   0 felipeburry   (501) staff       (20)     2536 2024-04-24 18:46:43.000000 jr_connection-0.1.1/src/jr_connection.egg-info/PKG-INFO
+-rw-r--r--   0 felipeburry   (501) staff       (20)      627 2024-04-24 18:46:43.000000 jr_connection-0.1.1/src/jr_connection.egg-info/SOURCES.txt
+-rw-r--r--   0 felipeburry   (501) staff       (20)        1 2024-04-24 18:46:43.000000 jr_connection-0.1.1/src/jr_connection.egg-info/dependency_links.txt
+-rw-r--r--   0 felipeburry   (501) staff       (20)       59 2024-04-24 18:46:43.000000 jr_connection-0.1.1/src/jr_connection.egg-info/entry_points.txt
+-rw-r--r--   0 felipeburry   (501) staff       (20)      347 2024-04-24 18:46:43.000000 jr_connection-0.1.1/src/jr_connection.egg-info/requires.txt
+-rw-r--r--   0 felipeburry   (501) staff       (20)       14 2024-04-24 18:46:43.000000 jr_connection-0.1.1/src/jr_connection.egg-info/top_level.txt
+drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-24 18:46:43.243207 jr_connection-0.1.1/tests/
+-rw-r--r--   0 felipeburry   (501) staff       (20)     2007 2024-04-17 18:31:52.000000 jr_connection-0.1.1/tests/test_connection_class.py
+-rw-r--r--   0 felipeburry   (501) staff       (20)     2503 2024-04-17 18:48:40.000000 jr_connection-0.1.1/tests/test_data_handler_class.py
```

### Comparing `jr_connection-0.1.0/LICENSE` & `jr_connection-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jr_connection-0.1.0/PKG-INFO` & `jr_connection-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jr_connection
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple python package to connect to JR servers and get the data
 Home-page: https://github.com/faburry23/JR_Connection
 Author: Felipe Burry
 Author-email: Felipe Burry <felipe.burry@jriveros.cl>
 License: MIT License
         
         Copyright (c) [2024] [Felipe Burry]
```

### Comparing `jr_connection-0.1.0/pyproject.toml` & `jr_connection-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jr_connection"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Felipe Burry", email="felipe.burry@jriveros.cl" },
 ]
 description = "A simple python package to connect to JR servers and get the data"
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.11"
```

### Comparing `jr_connection-0.1.0/setup.py` & `jr_connection-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="jr_connection",
-    version="0.1.0",
+    version="0.1.1",
     description="A simple python package to connect to JR servers and get the data",
     long_description="lalala",
     url="https://github.com/faburry23/JR_Connection",
     author="Felipe Burry",
     author_email="felipe.burry@jriveros.cl",
     license="MIT",
     package_dir={"": "src"},
```

### Comparing `jr_connection-0.1.0/src/jr_connection/classes/connection_class.py` & `jr_connection-0.1.1/src/jr_connection/classes/connection_class.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 
 # Related Third Library Imports
 import platform
 import pandas as pd
 import pymssql
 from sqlalchemy import create_engine, text
 from sqlalchemy.exc import SQLAlchemyError
+import os
 
 # Local Application/Library Specific Imports
 from .dbconfig_class import DBConfig
 
 
-class Connection:
+class ConnectionMSServer:
     """
     Gestiona la conexión a la base de datos y las operaciones de recuperación de datos.
 
     Esta clase se encarga de establecer la conexión con la base de datos usando las credenciales
     cargadas y proporciona métodos para obtener datos de la base de datos y almacenarlos localmente.
 
     Atributos:
@@ -34,23 +35,18 @@
     """
 
     def __init__(self):
         """
         Inicializa la conexión a la base de datos cargando las credenciales, construyendo la cadena
         de conexión, creando el motor de base de datos y verificando la conexión.
         """
-        self.platform = platform.system()
         self.credentials = DBConfig.load_credentials()
-        if self.platform == "Linux":
-            self.connection = self.connect_db_raspi()
-            self.is_connected = self.test_db_connection()
-        else:
-            self.connection_string = self.create_connection_string(self.credentials)
-            self.engine = self.create_db_engine()
-            self.is_connected = self.test_db_connection()
+        self.connection_string = self.create_connection_string(self.credentials)
+        self.engine = self.create_db_engine()
+        self.is_connected = self.test_db_connection()
 
     @staticmethod
     def create_connection_string(credentials):
         """
         Construye una cadena de conexión a la base de datos a partir de las credenciales proporcionadas.
 
         Parámetros:
@@ -65,28 +61,14 @@
         Ejemplo:
         --------
         credentials = {'db_username': 'user', 'db_password': 'pass', 'db_host': 'localhost', 'db_name': 'mydb', 'db_driver': 'ODBC Driver 17 for SQL Server'}
         connection_string = Connection.create_connection_string(credentials)
         """
         return f"mssql+pyodbc://{credentials['db_username']}:{credentials['db_password']}@{credentials['db_host']}/{credentials['db_name']}?driver={credentials['db_driver']}&TrustServerCertificate=yes"
 
-    def connect_db_raspi(self):
-        try:
-            connection = pymssql.connect(
-                server=self.credentials["db_host"],
-                user=self.credentials["db_username"],
-                password=self.credentials["db_password"],
-                database=self.credentials["db_name"],
-            )
-            # print("Database connection successful.")
-            return connection
-        except Exception as e:
-            print(f"Error connecting to database: {e}")
-            return None
-
     def create_db_engine(self):
         """
         Intenta crear y retorna un motor de base de datos utilizando la cadena de conexión.
 
         Retorna:
         --------
         sqlalchemy.engine.base.Engine or None
@@ -112,36 +94,24 @@
         bool
             True si la conexión es exitosa, False si falla.
 
         Ejemplo:
         --------
         is_connected = self.test_db_connection()
         """
-        if self.platform == "Linux":
-            # Use pymssql connection for Raspberry Pi
-            try:
-                cursor = self.connection.cursor()
-                cursor.execute("SELECT 1")
-                cursor.fetchone()
+
+        try:
+            with self.engine.begin() as conn:
+                result = conn.execute(text("SELECT 1"))
+                result.fetchone()
                 self.is_connected = True
                 return self.is_connected
-            except Exception as e:
-                print(f"Error testing database connection on Raspberry Pi: {e}")
-                self.is_connected = False
-                return self.is_connected
-        else:
-            try:
-                with self.engine.begin() as conn:
-                    result = conn.execute(text("SELECT 1"))
-                    result.fetchone()
-                    self.is_connected = True
-                    return self.is_connected
-            except Exception as e:
-                self.is_connected = False
-                return self.is_connected
+        except Exception as e:
+            self.is_connected = False
+            return self.is_connected
 
     def get_data(self, table_name):
         """
         Recupera datos de la tabla especificada y los almacena localmente en formato Parquet.
 
         Parámetros:
         -----------
@@ -162,7 +132,88 @@
                     SELECT *
                     FROM {table_name}
                     """
             )
             df = pd.read_sql_query(query, conn)
             df.to_parquet(f"./data/raw/{table_name}.parquet")
         return df
+
+
+class ConnectionFreeTDS:
+    def __init__(self):
+        self.credentials = DBConfig.load_credentials()
+        self.db_server = self.credentials["db_host"]
+        self.db_user_name = self.credentials["db_username"]
+        self.db_password = self.credentials["db_password"]
+        self.db_name = self.credentials["db_name"]
+        self.db_driver = self.credentials["db_driver"]
+        self.is_connected = self.test_connection()
+
+    def connect_db(self):
+        try:
+            connection = pymssql.connect(
+                server=self.db_server,
+                user=self.db_user_name,
+                password=self.db_password,
+                database=self.db_name,
+                tds_version=r"7.0",
+            )
+            return connection
+        except Exception as e:
+            print(f"Error connecting to database: {e}")
+            return None
+
+    def __enter__(self):
+        self.conn = self.connect_db()
+        return self.conn
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        if self.conn:
+            self.conn.close()
+            # print("Database connection closed.")
+
+    def test_connection(self):
+        conn = self.connect_db()
+        if conn is not None:
+            cursor = conn.cursor()
+            cursor.execute("SELECT 1")
+            cursor.close()
+            conn.close()
+            self.is_connected = True
+            return self.is_connected
+        else:
+            self.is_connected = False
+            print("Failed to establish connection.")
+            return self.is_connected
+
+    def get_data(self, table_name):
+        """
+        Recupera datos de la tabla especificada y los almacena localmente en formato Parquet.
+
+        Parámetros:
+        -----------
+        table_name (str): Nombre de la tabla de la cual se recuperarán los datos.
+
+        Retorna:
+        --------
+        pandas.DataFrame
+            DataFrame de pandas que contiene los datos recuperados.
+
+        Ejemplo:
+        --------
+        df = self.get_data('tabla')
+        """
+        with self as conn:
+            if conn is not None:
+                cursor = conn.cursor()
+                query = f"SELECT * FROM {table_name}"
+                cursor.execute(query)
+                # Fetch data and use pandas to create a DataFrame
+                data = cursor.fetchall()
+                df = pd.DataFrame(data)
+                df.columns = [desc[0] for desc in cursor.description]
+                df.to_parquet(f"./data/raw/{table_name}.parquet")
+                cursor.close()
+                return df
+            else:
+                print("Failed to establish connection.")
+                return None
```

### Comparing `jr_connection-0.1.0/src/jr_connection/classes/data_handler_class.py` & `jr_connection-0.1.1/src/jr_connection/classes/data_handler_class.py`

 * *Files identical despite different names*

### Comparing `jr_connection-0.1.0/src/jr_connection/first_run.py` & `jr_connection-0.1.1/src/jr_connection/first_run.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,31 @@
 #!/usr/bin/env python3
 
 import os
-import platform
 
 
 def setup_env_file():
     """
     Configura y crea un archivo .env con las credenciales para la conexión a la base de datos.
 
     Solicita al usuario que introduzca los detalles necesarios para la conexión a la base de datos,
     incluyendo el controlador, host, nombre de la base de datos, usuario y contraseña. Si el usuario
     no especifica un controlador, se utiliza un valor predeterminado.
 
     Ejemplo de uso:
     ---------------
     setup_env_file()  # Pide al usuario los detalles y crea el archivo .env
     """
-    platform = platform.system()
-    if platform != "Linux":
-        default_db_driver = "ODBC Driver 18 for SQL Server"
-        print(f"The default database driver is '{default_db_driver}'.")
-        db_driver = input(
-            "Press Enter to accept the default, or specify a different driver: "
-        ).strip()
-        db_driver = db_driver if db_driver else default_db_driver
-    else:
-        default_db_driver = "FreeTDS"
-        db_driver = default_db_driver
+
+    default_db_driver = "ODBC Driver 18 for SQL Server"
+    print(f"The default database driver is '{default_db_driver}'.")
+    db_driver = input(
+        "Press Enter to accept the default, or specify a different driver: "
+    ).strip()
+    db_driver = db_driver if db_driver else default_db_driver
     db_host = input("Enter the database host (e.g., localhost): ").strip()
     db_database = input("Enter the database name: ").strip()
     db_username = input("Enter the database username: ").strip()
     db_password = input("Enter the database password: ").strip()
 
     env_content = f"""# Database configuration
                         DB_DRIVER='{db_driver}'
```

### Comparing `jr_connection-0.1.0/src/jr_connection.egg-info/PKG-INFO` & `jr_connection-0.1.1/src/jr_connection.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jr-connection
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple python package to connect to JR servers and get the data
 Home-page: https://github.com/faburry23/JR_Connection
 Author: Felipe Burry
 Author-email: Felipe Burry <felipe.burry@jriveros.cl>
 License: MIT License
         
         Copyright (c) [2024] [Felipe Burry]
```

### Comparing `jr_connection-0.1.0/src/jr_connection.egg-info/SOURCES.txt` & `jr_connection-0.1.1/src/jr_connection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jr_connection-0.1.0/tests/test_connection_class.py` & `jr_connection-0.1.1/tests/test_connection_class.py`

 * *Files identical despite different names*

### Comparing `jr_connection-0.1.0/tests/test_data_handler_class.py` & `jr_connection-0.1.1/tests/test_data_handler_class.py`

 * *Files identical despite different names*

