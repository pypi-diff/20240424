# Comparing `tmp/jr_connection-0.0.3.tar.gz` & `tmp/jr_connection-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jr_connection-0.0.3.tar", last modified: Tue Apr 23 21:43:14 2024, max compression
+gzip compressed data, was "jr_connection-0.1.0.tar", last modified: Wed Apr 24 15:28:06 2024, max compression
```

## Comparing `jr_connection-0.0.3.tar` & `jr_connection-0.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-23 21:43:14.658854 jr_connection-0.0.3/
--rw-r--r--   0 felipeburry   (501) staff       (20)     1072 2024-04-17 14:52:47.000000 jr_connection-0.0.3/LICENSE
--rw-r--r--   0 felipeburry   (501) staff       (20)     2505 2024-04-23 21:43:14.658591 jr_connection-0.0.3/PKG-INFO
--rw-r--r--   0 felipeburry   (501) staff       (20)       16 2024-04-17 14:49:29.000000 jr_connection-0.0.3/README.md
--rw-r--r--   0 felipeburry   (501) staff       (20)     1124 2024-04-23 21:39:58.000000 jr_connection-0.0.3/pyproject.toml
--rw-r--r--   0 felipeburry   (501) staff       (20)       38 2024-04-23 21:43:14.658911 jr_connection-0.0.3/setup.cfg
--rw-r--r--   0 felipeburry   (501) staff       (20)      737 2024-04-23 21:40:07.000000 jr_connection-0.0.3/setup.py
-drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-23 21:43:14.653769 jr_connection-0.0.3/src/
-drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-23 21:43:14.655313 jr_connection-0.0.3/src/jr_connection/
--rw-r--r--   0 felipeburry   (501) staff       (20)      137 2024-04-17 16:03:22.000000 jr_connection-0.0.3/src/jr_connection/__init__.py
-drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-23 21:43:14.657456 jr_connection-0.0.3/src/jr_connection/classes/
--rw-r--r--   0 felipeburry   (501) staff       (20)       85 2024-04-17 16:02:57.000000 jr_connection-0.0.3/src/jr_connection/classes/__init__.py
--rw-r--r--   0 felipeburry   (501) staff       (20)     4802 2024-04-23 21:38:06.000000 jr_connection-0.0.3/src/jr_connection/classes/connection_class.py
--rw-r--r--   0 felipeburry   (501) staff       (20)     5504 2024-04-17 19:15:46.000000 jr_connection-0.0.3/src/jr_connection/classes/data_handler_class.py
--rw-r--r--   0 felipeburry   (501) staff       (20)      429 2024-04-17 17:59:39.000000 jr_connection-0.0.3/src/jr_connection/classes/dbconfig_class.py
--rwxr-xr-x   0 felipeburry   (501) staff       (20)     2931 2024-04-17 19:01:30.000000 jr_connection-0.0.3/src/jr_connection/first_run.py
--rw-r--r--   0 felipeburry   (501) staff       (20)      154 2024-04-17 18:00:05.000000 jr_connection-0.0.3/src/jr_connection/other_constants.py
-drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-23 21:43:14.656427 jr_connection-0.0.3/src/jr_connection.egg-info/
--rw-r--r--   0 felipeburry   (501) staff       (20)     2505 2024-04-23 21:43:14.000000 jr_connection-0.0.3/src/jr_connection.egg-info/PKG-INFO
--rw-r--r--   0 felipeburry   (501) staff       (20)      627 2024-04-23 21:43:14.000000 jr_connection-0.0.3/src/jr_connection.egg-info/SOURCES.txt
--rw-r--r--   0 felipeburry   (501) staff       (20)        1 2024-04-23 21:43:14.000000 jr_connection-0.0.3/src/jr_connection.egg-info/dependency_links.txt
--rw-r--r--   0 felipeburry   (501) staff       (20)       59 2024-04-23 21:43:14.000000 jr_connection-0.0.3/src/jr_connection.egg-info/entry_points.txt
--rw-r--r--   0 felipeburry   (501) staff       (20)      331 2024-04-23 21:43:14.000000 jr_connection-0.0.3/src/jr_connection.egg-info/requires.txt
--rw-r--r--   0 felipeburry   (501) staff       (20)       14 2024-04-23 21:43:14.000000 jr_connection-0.0.3/src/jr_connection.egg-info/top_level.txt
-drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-23 21:43:14.658016 jr_connection-0.0.3/tests/
--rw-r--r--   0 felipeburry   (501) staff       (20)     2007 2024-04-17 18:31:52.000000 jr_connection-0.0.3/tests/test_connection_class.py
--rw-r--r--   0 felipeburry   (501) staff       (20)     2503 2024-04-17 18:48:40.000000 jr_connection-0.0.3/tests/test_data_handler_class.py
+drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-24 15:28:06.148231 jr_connection-0.1.0/
+-rw-r--r--   0 felipeburry   (501) staff       (20)     1072 2024-04-17 14:52:47.000000 jr_connection-0.1.0/LICENSE
+-rw-r--r--   0 felipeburry   (501) staff       (20)     2536 2024-04-24 15:28:06.147797 jr_connection-0.1.0/PKG-INFO
+-rw-r--r--   0 felipeburry   (501) staff       (20)       16 2024-04-17 14:49:29.000000 jr_connection-0.1.0/README.md
+-rw-r--r--   0 felipeburry   (501) staff       (20)     1148 2024-04-24 15:25:44.000000 jr_connection-0.1.0/pyproject.toml
+-rw-r--r--   0 felipeburry   (501) staff       (20)       38 2024-04-24 15:28:06.148346 jr_connection-0.1.0/setup.cfg
+-rw-r--r--   0 felipeburry   (501) staff       (20)      737 2024-04-24 15:25:47.000000 jr_connection-0.1.0/setup.py
+drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-24 15:28:06.138988 jr_connection-0.1.0/src/
+drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-24 15:28:06.141614 jr_connection-0.1.0/src/jr_connection/
+-rw-r--r--   0 felipeburry   (501) staff       (20)      137 2024-04-17 16:03:22.000000 jr_connection-0.1.0/src/jr_connection/__init__.py
+drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-24 15:28:06.146056 jr_connection-0.1.0/src/jr_connection/classes/
+-rw-r--r--   0 felipeburry   (501) staff       (20)       85 2024-04-17 16:02:57.000000 jr_connection-0.1.0/src/jr_connection/classes/__init__.py
+-rw-r--r--   0 felipeburry   (501) staff       (20)     6132 2024-04-24 15:07:53.000000 jr_connection-0.1.0/src/jr_connection/classes/connection_class.py
+-rw-r--r--   0 felipeburry   (501) staff       (20)     5504 2024-04-17 19:15:46.000000 jr_connection-0.1.0/src/jr_connection/classes/data_handler_class.py
+-rw-r--r--   0 felipeburry   (501) staff       (20)      429 2024-04-17 17:59:39.000000 jr_connection-0.1.0/src/jr_connection/classes/dbconfig_class.py
+-rwxr-xr-x   0 felipeburry   (501) staff       (20)     3118 2024-04-24 15:00:32.000000 jr_connection-0.1.0/src/jr_connection/first_run.py
+-rw-r--r--   0 felipeburry   (501) staff       (20)      154 2024-04-17 18:00:05.000000 jr_connection-0.1.0/src/jr_connection/other_constants.py
+drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-24 15:28:06.143415 jr_connection-0.1.0/src/jr_connection.egg-info/
+-rw-r--r--   0 felipeburry   (501) staff       (20)     2536 2024-04-24 15:28:06.000000 jr_connection-0.1.0/src/jr_connection.egg-info/PKG-INFO
+-rw-r--r--   0 felipeburry   (501) staff       (20)      627 2024-04-24 15:28:06.000000 jr_connection-0.1.0/src/jr_connection.egg-info/SOURCES.txt
+-rw-r--r--   0 felipeburry   (501) staff       (20)        1 2024-04-24 15:28:06.000000 jr_connection-0.1.0/src/jr_connection.egg-info/dependency_links.txt
+-rw-r--r--   0 felipeburry   (501) staff       (20)       59 2024-04-24 15:28:06.000000 jr_connection-0.1.0/src/jr_connection.egg-info/entry_points.txt
+-rw-r--r--   0 felipeburry   (501) staff       (20)      347 2024-04-24 15:28:06.000000 jr_connection-0.1.0/src/jr_connection.egg-info/requires.txt
+-rw-r--r--   0 felipeburry   (501) staff       (20)       14 2024-04-24 15:28:06.000000 jr_connection-0.1.0/src/jr_connection.egg-info/top_level.txt
+drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-24 15:28:06.146867 jr_connection-0.1.0/tests/
+-rw-r--r--   0 felipeburry   (501) staff       (20)     2007 2024-04-17 18:31:52.000000 jr_connection-0.1.0/tests/test_connection_class.py
+-rw-r--r--   0 felipeburry   (501) staff       (20)     2503 2024-04-17 18:48:40.000000 jr_connection-0.1.0/tests/test_data_handler_class.py
```

### Comparing `jr_connection-0.0.3/LICENSE` & `jr_connection-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jr_connection-0.0.3/PKG-INFO` & `jr_connection-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jr_connection
-Version: 0.0.3
+Version: 0.1.0
 Summary: A simple python package to connect to JR servers and get the data
 Home-page: https://github.com/faburry23/JR_Connection
 Author: Felipe Burry
 Author-email: Felipe Burry <felipe.burry@jriveros.cl>
 License: MIT License
         
         Copyright (c) [2024] [Felipe Burry]
@@ -49,9 +49,10 @@
 Requires-Dist: pytz==2024.1
 Requires-Dist: six==1.16.0
 Requires-Dist: SQLAlchemy==2.0.29
 Requires-Dist: typing_extensions==4.10.0
 Requires-Dist: tzdata==2024.1
 Requires-Dist: pytest==7.4.3
 Requires-Dist: pytest-mock==3.14.0
+Requires-Dist: pymssql==2.2.11
 
 # JR_Connection
```

### Comparing `jr_connection-0.0.3/pyproject.toml` & `jr_connection-0.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jr_connection"
-version = "0.0.3"
+version = "0.1.0"
 authors = [
   { name="Felipe Burry", email="felipe.burry@jriveros.cl" },
 ]
 description = "A simple python package to connect to JR servers and get the data"
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.11"
@@ -27,15 +27,16 @@
     "python-dotenv==1.0.1",
     "pytz==2024.1",
     "six==1.16.0",
     "SQLAlchemy==2.0.29",
     "typing_extensions==4.10.0",
     "tzdata==2024.1",
     "pytest==7.4.3",
-    "pytest-mock==3.14.0"
+    "pytest-mock==3.14.0",
+    "pymssql==2.2.11",
 ]
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
```

### Comparing `jr_connection-0.0.3/setup.py` & `jr_connection-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="jr_connection",
-    version="0.0.3",
+    version="0.1.0",
     description="A simple python package to connect to JR servers and get the data",
     long_description="lalala",
     url="https://github.com/faburry23/JR_Connection",
     author="Felipe Burry",
     author_email="felipe.burry@jriveros.cl",
     license="MIT",
     package_dir={"": "src"},
```

### Comparing `jr_connection-0.0.3/src/jr_connection/classes/data_handler_class.py` & `jr_connection-0.1.0/src/jr_connection/classes/data_handler_class.py`

 * *Files identical despite different names*

### Comparing `jr_connection-0.0.3/src/jr_connection/first_run.py` & `jr_connection-0.1.0/src/jr_connection/first_run.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 #!/usr/bin/env python3
 
 import os
+import platform
 
 
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
-    default_db_driver = "ODBC Driver 18 for SQL Server"
-    print(f"The default database driver is '{default_db_driver}'.")
-    db_driver = input(
-        "Press Enter to accept the default, or specify a different driver: "
-    ).strip()
-    db_driver = db_driver if db_driver else default_db_driver
+    platform = platform.system()
+    if platform != "Linux":
+        default_db_driver = "ODBC Driver 18 for SQL Server"
+        print(f"The default database driver is '{default_db_driver}'.")
+        db_driver = input(
+            "Press Enter to accept the default, or specify a different driver: "
+        ).strip()
+        db_driver = db_driver if db_driver else default_db_driver
+    else:
+        default_db_driver = "FreeTDS"
+        db_driver = default_db_driver
     db_host = input("Enter the database host (e.g., localhost): ").strip()
     db_database = input("Enter the database name: ").strip()
     db_username = input("Enter the database username: ").strip()
     db_password = input("Enter the database password: ").strip()
 
     env_content = f"""# Database configuration
                         DB_DRIVER='{db_driver}'
```

### Comparing `jr_connection-0.0.3/src/jr_connection.egg-info/PKG-INFO` & `jr_connection-0.1.0/src/jr_connection.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jr-connection
-Version: 0.0.3
+Version: 0.1.0
 Summary: A simple python package to connect to JR servers and get the data
 Home-page: https://github.com/faburry23/JR_Connection
 Author: Felipe Burry
 Author-email: Felipe Burry <felipe.burry@jriveros.cl>
 License: MIT License
         
         Copyright (c) [2024] [Felipe Burry]
@@ -49,9 +49,10 @@
 Requires-Dist: pytz==2024.1
 Requires-Dist: six==1.16.0
 Requires-Dist: SQLAlchemy==2.0.29
 Requires-Dist: typing_extensions==4.10.0
 Requires-Dist: tzdata==2024.1
 Requires-Dist: pytest==7.4.3
 Requires-Dist: pytest-mock==3.14.0
+Requires-Dist: pymssql==2.2.11
 
 # JR_Connection
```

### Comparing `jr_connection-0.0.3/src/jr_connection.egg-info/SOURCES.txt` & `jr_connection-0.1.0/src/jr_connection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jr_connection-0.0.3/tests/test_connection_class.py` & `jr_connection-0.1.0/tests/test_connection_class.py`

 * *Files identical despite different names*

### Comparing `jr_connection-0.0.3/tests/test_data_handler_class.py` & `jr_connection-0.1.0/tests/test_data_handler_class.py`

 * *Files identical despite different names*

