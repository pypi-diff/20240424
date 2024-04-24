# Comparing `tmp/simplepgsql-0.1.7.tar.gz` & `tmp/simplepgsql-0.1.8.tar.gz`

## Comparing `simplepgsql-0.1.7.tar` & `simplepgsql-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 simplepgsql-0.1.7/CHANGELOG.md
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 simplepgsql-0.1.7/requirements.txt
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 simplepgsql-0.1.7/run.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 simplepgsql-0.1.7/setup.cfg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simplepgsql-0.1.7/test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simplepgsql-0.1.7/simplepgsql/README.md
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 simplepgsql-0.1.7/simplepgsql/__init__.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 simplepgsql-0.1.7/simplepgsql/src/__init__.py
--rw-r--r--   0        0        0    16154 2020-02-02 00:00:00.000000 simplepgsql-0.1.7/simplepgsql/src/depr_simplepgsql.py
--rw-r--r--   0        0        0    16275 2020-02-02 00:00:00.000000 simplepgsql-0.1.7/simplepgsql/src/simplepgsql.py
--rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 simplepgsql-0.1.7/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 simplepgsql-0.1.7/LICENSE
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 simplepgsql-0.1.7/README.md
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 simplepgsql-0.1.7/pyproject.toml
--rw-r--r--   0        0        0    42748 2020-02-02 00:00:00.000000 simplepgsql-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 simplepgsql-0.1.8/CHANGELOG.md
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 simplepgsql-0.1.8/requirements.txt
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 simplepgsql-0.1.8/run.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 simplepgsql-0.1.8/setup.cfg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simplepgsql-0.1.8/test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simplepgsql-0.1.8/simplepgsql/README.md
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 simplepgsql-0.1.8/simplepgsql/__init__.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 simplepgsql-0.1.8/simplepgsql/src/__init__.py
+-rw-r--r--   0        0        0    16154 2020-02-02 00:00:00.000000 simplepgsql-0.1.8/simplepgsql/src/depr_simplepgsql.py
+-rw-r--r--   0        0        0    16257 2020-02-02 00:00:00.000000 simplepgsql-0.1.8/simplepgsql/src/simplepgsql.py
+-rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 simplepgsql-0.1.8/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 simplepgsql-0.1.8/LICENSE
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 simplepgsql-0.1.8/README.md
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 simplepgsql-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0    42676 2020-02-02 00:00:00.000000 simplepgsql-0.1.8/PKG-INFO
```

### Comparing `simplepgsql-0.1.7/CHANGELOG.md` & `simplepgsql-0.1.8/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 ## [Unreleased]
 
+## [0.1.8] - 2024-04-24
+
+### Bugfix
+1. Kept Naming Scheme consistent.
+2. Fixed typo for conjuction > conjunction
+
 ## [0.1.7] - 2024-04-16
 
 ### Added
 1. It automatically creates and destroys the cursor. No need to use `with` to enter.
 
 ### Removed/Deprecated
 1. DBConnect Class. It will still exist but new features will not be supported for backwards compatibility of versions. It is replaced by `SimplePgSQL` class.
```

### Comparing `simplepgsql-0.1.7/run.py` & `simplepgsql-0.1.8/run.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         "password": config['DB']['DB_PASSWORD'].strip(),
         "port": config['DB']['DB_PORT'],
     }
     
   
     _query_params = {
         "schema": "public",
-        "table_name": "film_list",
+        "table": "film_list",
         "columns": ["category", "price"],
         "aggregate": {
             "price": "SUM"
         },
         "conditions": {
             "length": (60, ">")
         },
@@ -31,16 +31,25 @@
         "group_by": ["category", "price"],
         "limit": 10,
     }
 
     # Using SimplePgSQL class
     pgsql = SimplePgSQL(conn_params, return_type=pd.DataFrame)
 
-    q_results = pgsql.execute("SELECT category, price FROM film_list LIMIT 10;", columns=["category", "price"])
+    _query = """
+            SELECT category, SUM(price) from public.film_list where length > 60 group by category, price order by price DESC limit 10;
+            """
+
+
+    q_results = pgsql.execute(_query, columns=["category", "price"])
     r_results = pgsql.read(**_query_params)
     print(q_results)
     print(r_results)
     
     # Deprecated method to query data DO NOT USE. For backward compatibility only
     with DBConnect(conn_params, return_type=pd.DataFrame) as cursor:
         q_results = cursor.query("SELECT category, price FROM film_list LIMIT 10;", columns=["category", "price"])
-        r_results = cursor.read(**_query_params)
+        _query_params.pop("table")
+        _query_params["table_name"] = "film_list"
+        r_results = cursor.read(**_query_params)
+        print(r_results)
+        print(q_results)
```

### Comparing `simplepgsql-0.1.7/simplepgsql/src/depr_simplepgsql.py` & `simplepgsql-0.1.8/simplepgsql/src/depr_simplepgsql.py`

 * *Files identical despite different names*

### Comparing `simplepgsql-0.1.7/simplepgsql/src/simplepgsql.py` & `simplepgsql-0.1.8/simplepgsql/src/simplepgsql.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,19 +161,19 @@
         if not isinstance(self.group_by, (list, type(None))):
             raise TypeError("Group must be a list")
         if not isinstance(self.limit, (int, type(None))):
             raise TypeError("Limit must be an integer")
 
     def read(self,
              schema: str,
-             table_name: str,
+             table: str,
              columns: list | None = None,
              aggregate: dict | None = None,
              conditions: dict | None = None,
-             conjuction: str = None,
+             conjunction: str = None,
              order_by: str | tuple | dict | None = None,
              group_by: list | None = None,
              limit: int | None = None) -> dict | list | pd.DataFrame:
         """
         Reads data from a table in the database.
 
         Parameters
@@ -217,25 +217,25 @@
         TypeError
             If the input types are not as expected.
         ValueError
             If group by is not specified for aggregate functions.
         """
         self.query_type = "read"
         self.schema = schema
-        self.table_name = table_name
+        self.table_name = table
         self.conditions = conditions
-        self.conjuction = conjuction
+        self.conjuction = conjunction
         self.order_by = order_by
         self.group_by = group_by
         self.limit = limit
         
         self.validate_query_params()
 
         if not columns:
-            self.columns = self._get_column_names(schema, table_name)
+            self.columns = self._get_column_names(schema, table)
         else:
             self.columns = columns
 
         if aggregate is not None:
             self.aggregate = aggregate
             if not group_by:
                 raise ValueError(
@@ -255,15 +255,15 @@
             columns_sql = [sql.Identifier(column) for column in self.columns]
 
         # Constructing the complete SELECT statement
         query = sql.SQL("SELECT {}").format(sql.SQL(', ').join(columns_sql))
 
         query += sql.SQL(" FROM {}.{}").format(
             sql.Identifier(schema),
-            sql.Identifier(table_name)
+            sql.Identifier(table)
         )
 
         if conditions is not None:
             operators = {_o for _c, (_v, _o) in conditions.items()}
             where_clause = sql.SQL("WHERE ")
             spl_columns = ["BETWEEN"]
```

### Comparing `simplepgsql-0.1.7/.gitignore` & `simplepgsql-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `simplepgsql-0.1.7/LICENSE` & `simplepgsql-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `simplepgsql-0.1.7/README.md` & `simplepgsql-0.1.8/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-# Simple PostgreSQL Interaction in Python
+# Simple PostgreSQL Wrapper for Python
 
 This project contains a Python script (`simplepgsql.py`) that provides a simple interface for interacting with a PostgreSQL database using psycopg2 library.
 
 ## Getting Started
 
 Install via PIP
+`pip install simplepgsql`
 
 ### Dependent Libraries
 
 - Python 3.6+
-- PostgreSQL
 - psycopg2 Python library
 - Pandas
 
 ## Usage
 
 ```python
 from simplepgsql Import DBConnect
@@ -36,24 +36,23 @@
         "conditions": {
             "length": (60, ">")
         },
         "order_by": ("price", "DESC"),
         "group_by": ["category", "price"],
         "limit": 10,
     }
-    with DBConnect(conn_params, return_type=pd.DataFrame) as cursor:
-        results = cursor.read(**_query_params)
-        print(results)
+  results = pgsql.read(**_query_params)
+  print(results)
 
 ```
 
 ### Output
 
 ```cmd
-      category sum: price
+      category  price.sum
 0          New     109.78
 1       Travel     109.78
 2       Family      74.85
 3        Games     129.74
 4  Documentary      69.86
 5    Animation      74.85
 6       Sports     119.76
```

### Comparing `simplepgsql-0.1.7/pyproject.toml` & `simplepgsql-0.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 00000000: 5b62 7569 6c64 2d73 7973 7465 6d5d 0d0a  [build-system]..
 00000010: 7265 7175 6972 6573 203d 205b 2268 6174  requires = ["hat
 00000020: 6368 6c69 6e67 225d 0d0a 6275 696c 642d  chling"]..build-
 00000030: 6261 636b 656e 6420 3d20 2268 6174 6368  backend = "hatch
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 7369 6d70 6c65 7067 7371 6c22 0d0a   "simplepgsql"..
-00000070: 7665 7273 696f 6e20 3d20 2230 2e31 2e37  version = "0.1.7
+00000070: 7665 7273 696f 6e20 3d20 2230 2e31 2e38  version = "0.1.8
 00000080: 220d 0a64 6573 6372 6970 7469 6f6e 203d  "..description =
 00000090: 2022 5772 6170 7065 7220 6172 6f75 6e64   "Wrapper around
 000000a0: 2070 7379 636f 7067 3220 746f 2073 696d   psycopg2 to sim
 000000b0: 706c 6966 7920 7468 6520 7072 6f63 6573  plify the proces
 000000c0: 7320 6f66 2063 6f6e 6e65 6374 696e 6720  s of connecting 
 000000d0: 746f 2061 2050 6f73 7467 7265 5351 4c20  to a PostgreSQL 
 000000e0: 6461 7461 6261 7365 2061 6e64 2065 7865  database and exe
```

### Comparing `simplepgsql-0.1.7/PKG-INFO` & `simplepgsql-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: simplepgsql
-Version: 0.1.7
+Version: 0.1.8
 Summary: Wrapper around psycopg2 to simplify the process of connecting to a PostgreSQL database and executing queries.
 Project-URL: Repository, https://github.com/iamlrk/simple-pgsql
 Author-email: iamlrk <lepakshiramkiran@hotmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -683,26 +683,26 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: SQL
 Description-Content-Type: text/markdown
 
-# Simple PostgreSQL Interaction in Python
+# Simple PostgreSQL Wrapper for Python
 
 This project contains a Python script (`simplepgsql.py`) that provides a simple interface for interacting with a PostgreSQL database using psycopg2 library.
 
 ## Getting Started
 
 Install via PIP
+`pip install simplepgsql`
 
 ### Dependent Libraries
 
 - Python 3.6+
-- PostgreSQL
 - psycopg2 Python library
 - Pandas
 
 ## Usage
 
 ```python
 from simplepgsql Import DBConnect
@@ -725,24 +725,23 @@
         "conditions": {
             "length": (60, ">")
         },
         "order_by": ("price", "DESC"),
         "group_by": ["category", "price"],
         "limit": 10,
     }
-    with DBConnect(conn_params, return_type=pd.DataFrame) as cursor:
-        results = cursor.read(**_query_params)
-        print(results)
+  results = pgsql.read(**_query_params)
+  print(results)
 
 ```
 
 ### Output
 
 ```cmd
-      category sum: price
+      category  price.sum
 0          New     109.78
 1       Travel     109.78
 2       Family      74.85
 3        Games     129.74
 4  Documentary      69.86
 5    Animation      74.85
 6       Sports     119.76
```

