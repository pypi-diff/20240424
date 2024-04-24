# Comparing `tmp/shipyard_sqlserver-0.2.0a6.tar.gz` & `tmp/shipyard_sqlserver-0.2.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_sqlserver-0.2.0a6.tar", max compression
+gzip compressed data, was "shipyard_sqlserver-0.2.1a0.tar", max compression
```

## Comparing `shipyard_sqlserver-0.2.0a6.tar` & `shipyard_sqlserver-0.2.1a0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2023-08-14 16:50:02.446349 shipyard_sqlserver-0.2.0a6/README.md
--rw-r--r--   0        0        0      681 2024-03-25 20:44:34.238427 shipyard_sqlserver-0.2.0a6/pyproject.toml
--rw-r--r--   0        0        0       39 2023-08-14 16:50:02.447093 shipyard_sqlserver-0.2.0a6/shipyard_sqlserver/__init__.py
--rw-r--r--   0        0        0        0 2024-03-08 19:26:39.005282 shipyard_sqlserver-0.2.0a6/shipyard_sqlserver/cli/__init__.py
--rw-r--r--   0        0        0      770 2024-03-25 20:45:07.917157 shipyard_sqlserver-0.2.0a6/shipyard_sqlserver/cli/authtest.py
--rw-r--r--   0        0        0     2059 2024-03-25 20:27:00.253292 shipyard_sqlserver-0.2.0a6/shipyard_sqlserver/cli/execute_sql.py
--rw-r--r--   0        0        0     2991 2024-03-25 20:27:16.630788 shipyard_sqlserver-0.2.0a6/shipyard_sqlserver/cli/store_query_results.py
--rw-r--r--   0        0        0     4149 2024-03-25 20:26:29.621579 shipyard_sqlserver-0.2.0a6/shipyard_sqlserver/cli/upload_file.py
--rw-r--r--   0        0        0      342 2024-03-25 20:25:45.260252 shipyard_sqlserver-0.2.0a6/shipyard_sqlserver/exceptions.py
--rw-r--r--   0        0        0     4652 2024-03-25 20:26:13.511943 shipyard_sqlserver-0.2.0a6/shipyard_sqlserver/sqlserver.py
--rw-r--r--   0        0        0      737 1970-01-01 00:00:00.000000 shipyard_sqlserver-0.2.0a6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-14 16:50:02.446349 shipyard_sqlserver-0.2.1a0/README.md
+-rw-r--r--   0        0        0      679 2024-04-24 20:36:40.925511 shipyard_sqlserver-0.2.1a0/pyproject.toml
+-rw-r--r--   0        0        0       39 2023-08-14 16:50:02.447093 shipyard_sqlserver-0.2.1a0/shipyard_sqlserver/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-08 19:26:39.005282 shipyard_sqlserver-0.2.1a0/shipyard_sqlserver/cli/__init__.py
+-rw-r--r--   0        0        0      947 2024-04-23 20:50:28.200126 shipyard_sqlserver-0.2.1a0/shipyard_sqlserver/cli/authtest.py
+-rw-r--r--   0        0        0     2059 2024-04-18 03:07:13.754478 shipyard_sqlserver-0.2.1a0/shipyard_sqlserver/cli/execute_sql.py
+-rw-r--r--   0        0        0     2991 2024-04-18 03:07:13.754853 shipyard_sqlserver-0.2.1a0/shipyard_sqlserver/cli/store_query_results.py
+-rw-r--r--   0        0        0     4149 2024-04-18 03:07:13.755269 shipyard_sqlserver-0.2.1a0/shipyard_sqlserver/cli/upload_file.py
+-rw-r--r--   0        0        0      342 2024-04-18 03:07:13.755839 shipyard_sqlserver-0.2.1a0/shipyard_sqlserver/exceptions.py
+-rw-r--r--   0        0        0     4652 2024-04-23 20:22:26.196919 shipyard_sqlserver-0.2.1a0/shipyard_sqlserver/sqlserver.py
+-rw-r--r--   0        0        0      735 1970-01-01 00:00:00.000000 shipyard_sqlserver-0.2.1a0/PKG-INFO
```

### Comparing `shipyard_sqlserver-0.2.0a6/pyproject.toml` & `shipyard_sqlserver-0.2.1a0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "shipyard-sqlserver"
-version = "0.2.0a6"
+version = "0.2.1a0"
 description = "A local client for connecting and working with Sql Server Databases"
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{include = "shipyard_sqlserver"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pandas = "^2.0"
-shipyard-templates = "0.8.0a1"
+shipyard-templates = "0.8.0"
 pyodbc = "^5.0.1"
 sqlalchemy = "^2.0.28"
 shipyard-bp-utils = "1.2.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.2.0"
 python-dotenv = "^1.0.1"
```

### Comparing `shipyard_sqlserver-0.2.0a6/shipyard_sqlserver/cli/authtest.py` & `shipyard_sqlserver-0.2.1a0/shipyard_sqlserver/cli/authtest.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,18 +13,22 @@
             pwd=os.getenv("MSSQL_PASSWORD"),
             host=os.getenv("MSSQL_HOST"),
             database=os.getenv("MSSQL_DATABASE"),
             port=os.getenv("MSSQL_PORT"),
         )
         client.connect()
     except Exception as e:
+        logger.error(
+            f"Error in connecting to SQL Server. Message from the server reads: {e}"
+        )
         logger.authtest(
             f"Error in connecting to SQL Server. Message from the server reads: {e}"
         )
         sys.exit(1)
     else:
+        logger.info("Successfully connected to SQL Server")
         logger.authtest("Successfully connected to SQL Server")
         sys.exit(0)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `shipyard_sqlserver-0.2.0a6/shipyard_sqlserver/cli/execute_sql.py` & `shipyard_sqlserver-0.2.1a0/shipyard_sqlserver/cli/execute_sql.py`

 * *Files identical despite different names*

### Comparing `shipyard_sqlserver-0.2.0a6/shipyard_sqlserver/cli/store_query_results.py` & `shipyard_sqlserver-0.2.1a0/shipyard_sqlserver/cli/store_query_results.py`

 * *Files identical despite different names*

### Comparing `shipyard_sqlserver-0.2.0a6/shipyard_sqlserver/cli/upload_file.py` & `shipyard_sqlserver-0.2.1a0/shipyard_sqlserver/cli/upload_file.py`

 * *Files identical despite different names*

### Comparing `shipyard_sqlserver-0.2.0a6/shipyard_sqlserver/sqlserver.py` & `shipyard_sqlserver-0.2.1a0/shipyard_sqlserver/sqlserver.py`

 * *Files identical despite different names*

### Comparing `shipyard_sqlserver-0.2.0a6/PKG-INFO` & `shipyard_sqlserver-0.2.1a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: shipyard-sqlserver
-Version: 0.2.0a6
+Version: 0.2.1a0
 Summary: A local client for connecting and working with Sql Server Databases
 License: Apache 2.0
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pandas (>=2.0,<3.0)
 Requires-Dist: pyodbc (>=5.0.1,<6.0.0)
 Requires-Dist: shipyard-bp-utils (==1.2.0)
-Requires-Dist: shipyard-templates (==0.8.0a1)
+Requires-Dist: shipyard-templates (==0.8.0)
 Requires-Dist: sqlalchemy (>=2.0.28,<3.0.0)
 Description-Content-Type: text/markdown
```

