# Comparing `tmp/dbrepo-1.4.2rc14.tar.gz` & `tmp/dbrepo-1.4.2rc15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbrepo-1.4.2rc14.tar", last modified: Sat Apr 20 17:48:34 2024, max compression
+gzip compressed data, was "dbrepo-1.4.2rc15.tar", last modified: Wed Apr 24 09:25:02 2024, max compression
```

## Comparing `dbrepo-1.4.2rc14.tar` & `dbrepo-1.4.2rc15.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-20 17:48:34.875832 dbrepo-1.4.2rc14/
--rw-r--r--   0 mweise    (1000) mweise    (1000)    11357 2024-04-12 20:45:40.000000 dbrepo-1.4.2rc14/LICENSE
--rw-r--r--   0 mweise    (1000) mweise    (1000)    18900 2024-04-20 17:48:34.875832 dbrepo-1.4.2rc14/PKG-INFO
--rw-r--r--   0 mweise    (1000) mweise    (1000)     4814 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc14/README.md
-drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-20 17:48:34.871832 dbrepo-1.4.2rc14/dbrepo/
--rw-r--r--   0 mweise    (1000) mweise    (1000)     2940 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc14/dbrepo/AmqpClient.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    75175 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc14/dbrepo/RestClient.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)     1609 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc14/dbrepo/UploadClient.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)        0 2024-04-12 20:45:40.000000 dbrepo-1.4.2rc14/dbrepo/__init__.py
-drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-20 17:48:34.875832 dbrepo-1.4.2rc14/dbrepo/api/
--rw-r--r--   0 mweise    (1000) mweise    (1000)        0 2024-04-12 20:45:40.000000 dbrepo-1.4.2rc14/dbrepo/api/__init__.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    21252 2024-04-20 17:47:57.000000 dbrepo-1.4.2rc14/dbrepo/api/dto.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)      368 2024-04-19 11:42:17.000000 dbrepo-1.4.2rc14/dbrepo/api/encoder.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)     1265 2024-04-12 20:45:40.000000 dbrepo-1.4.2rc14/dbrepo/api/exceptions.py
-drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-20 17:48:34.875832 dbrepo-1.4.2rc14/dbrepo.egg-info/
--rw-r--r--   0 mweise    (1000) mweise    (1000)    18900 2024-04-20 17:48:34.000000 dbrepo-1.4.2rc14/dbrepo.egg-info/PKG-INFO
--rw-r--r--   0 mweise    (1000) mweise    (1000)      582 2024-04-20 17:48:34.000000 dbrepo-1.4.2rc14/dbrepo.egg-info/SOURCES.txt
--rw-r--r--   0 mweise    (1000) mweise    (1000)        1 2024-04-20 17:48:34.000000 dbrepo-1.4.2rc14/dbrepo.egg-info/dependency_links.txt
--rw-r--r--   0 mweise    (1000) mweise    (1000)       42 2024-04-20 17:48:34.000000 dbrepo-1.4.2rc14/dbrepo.egg-info/requires.txt
--rw-r--r--   0 mweise    (1000) mweise    (1000)        7 2024-04-20 17:48:34.000000 dbrepo-1.4.2rc14/dbrepo.egg-info/top_level.txt
--rw-r--r--   0 mweise    (1000) mweise    (1000)     1103 2024-04-20 17:48:31.000000 dbrepo-1.4.2rc14/pyproject.toml
--rw-r--r--   0 mweise    (1000) mweise    (1000)       38 2024-04-20 17:48:34.875832 dbrepo-1.4.2rc14/setup.cfg
--rw-r--r--   0 mweise    (1000) mweise    (1000)      411 2024-04-20 17:48:31.000000 dbrepo-1.4.2rc14/setup.py
-drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-20 17:48:34.875832 dbrepo-1.4.2rc14/tests/
--rw-r--r--   0 mweise    (1000) mweise    (1000)      729 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc14/tests/test_analyse.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)     5565 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc14/tests/test_container.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    26166 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc14/tests/test_database.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    11310 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc14/tests/test_identifier.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)     1083 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc14/tests/test_license.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    14639 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc14/tests/test_query.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)     1308 2024-04-12 20:45:40.000000 dbrepo-1.4.2rc14/tests/test_rest_client.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    29497 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc14/tests/test_table.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    14697 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc14/tests/test_user.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    11997 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc14/tests/test_view.py
+drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-24 09:25:02.775814 dbrepo-1.4.2rc15/
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    11357 2024-04-12 20:45:40.000000 dbrepo-1.4.2rc15/LICENSE
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    18900 2024-04-24 09:25:02.775814 dbrepo-1.4.2rc15/PKG-INFO
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     4814 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc15/README.md
+drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-24 09:25:02.771814 dbrepo-1.4.2rc15/dbrepo/
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     2940 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc15/dbrepo/AmqpClient.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    75175 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc15/dbrepo/RestClient.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     1609 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc15/dbrepo/UploadClient.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)        0 2024-04-12 20:45:40.000000 dbrepo-1.4.2rc15/dbrepo/__init__.py
+drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-24 09:25:02.771814 dbrepo-1.4.2rc15/dbrepo/api/
+-rw-r--r--   0 mweise    (1000) mweise    (1000)        0 2024-04-12 20:45:40.000000 dbrepo-1.4.2rc15/dbrepo/api/__init__.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    21346 2024-04-24 09:24:36.000000 dbrepo-1.4.2rc15/dbrepo/api/dto.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)      368 2024-04-19 11:42:17.000000 dbrepo-1.4.2rc15/dbrepo/api/encoder.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     1265 2024-04-12 20:45:40.000000 dbrepo-1.4.2rc15/dbrepo/api/exceptions.py
+drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-24 09:25:02.775814 dbrepo-1.4.2rc15/dbrepo.egg-info/
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    18900 2024-04-24 09:25:02.000000 dbrepo-1.4.2rc15/dbrepo.egg-info/PKG-INFO
+-rw-r--r--   0 mweise    (1000) mweise    (1000)      582 2024-04-24 09:25:02.000000 dbrepo-1.4.2rc15/dbrepo.egg-info/SOURCES.txt
+-rw-r--r--   0 mweise    (1000) mweise    (1000)        1 2024-04-24 09:25:02.000000 dbrepo-1.4.2rc15/dbrepo.egg-info/dependency_links.txt
+-rw-r--r--   0 mweise    (1000) mweise    (1000)       42 2024-04-24 09:25:02.000000 dbrepo-1.4.2rc15/dbrepo.egg-info/requires.txt
+-rw-r--r--   0 mweise    (1000) mweise    (1000)        7 2024-04-24 09:25:02.000000 dbrepo-1.4.2rc15/dbrepo.egg-info/top_level.txt
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     1103 2024-04-24 09:24:57.000000 dbrepo-1.4.2rc15/pyproject.toml
+-rw-r--r--   0 mweise    (1000) mweise    (1000)       38 2024-04-24 09:25:02.775814 dbrepo-1.4.2rc15/setup.cfg
+-rw-r--r--   0 mweise    (1000) mweise    (1000)      411 2024-04-24 09:24:57.000000 dbrepo-1.4.2rc15/setup.py
+drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-24 09:25:02.775814 dbrepo-1.4.2rc15/tests/
+-rw-r--r--   0 mweise    (1000) mweise    (1000)      729 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc15/tests/test_analyse.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     5565 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc15/tests/test_container.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    26166 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc15/tests/test_database.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    11310 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc15/tests/test_identifier.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     1083 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc15/tests/test_license.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    14639 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc15/tests/test_query.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     1308 2024-04-12 20:45:40.000000 dbrepo-1.4.2rc15/tests/test_rest_client.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    29497 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc15/tests/test_table.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    14697 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc15/tests/test_user.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    11997 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc15/tests/test_view.py
```

### Comparing `dbrepo-1.4.2rc14/LICENSE` & `dbrepo-1.4.2rc15/LICENSE`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc14/PKG-INFO` & `dbrepo-1.4.2rc15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbrepo
-Version: 1.4.2rc14
+Version: 1.4.2rc15
 Summary: DBRepo Python Library
 Home-page: https://www.ifs.tuwien.ac.at/infrastructures/dbrepo//
 Author: Martin Weise
 Author-email: "Martin Weise, TU Wien" <martin.weise@tuwien.ac.at>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
```

### Comparing `dbrepo-1.4.2rc14/README.md` & `dbrepo-1.4.2rc15/README.md`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc14/dbrepo/AmqpClient.py` & `dbrepo-1.4.2rc15/dbrepo/AmqpClient.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc14/dbrepo/RestClient.py` & `dbrepo-1.4.2rc15/dbrepo/RestClient.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc14/dbrepo/UploadClient.py` & `dbrepo-1.4.2rc15/dbrepo/UploadClient.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc14/dbrepo/api/dto.py` & `dbrepo-1.4.2rc15/dbrepo/api/dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -909,14 +909,20 @@
     queue_type: Optional[str] = None
     num_rows: Optional[int] = None
     data_length: Optional[int] = None
     max_data_length: Optional[int] = None
     avg_row_length: Optional[int] = None
 
 
+class TableMinimal(BaseModel):
+    id: int
+    database_id: int
+    name: str
+
+
 class Database(BaseModel):
     id: int
     name: str
     creator: User
     owner: User
     contact: User
     created: Timestamp
@@ -932,22 +938,22 @@
     image: Optional[str] = None
     accesses: Optional[List[DatabaseAccess]] = field(default_factory=list)
     exchange_type: Optional[str] = None
 
 
 class Unique(BaseModel):
     uid: int
-    table: Table
+    table: TableMinimal
     columns: List[Column]
 
 
 class ForeignKey(BaseModel):
     name: str
     columns: List[Column]
-    referenced_table: Table
+    referenced_table: TableMinimal
     referenced_columns: List[Column]
     on_update: Optional[str] = None
     on_delete: Optional[str] = None
 
 
 class CreateForeignKey(BaseModel):
     columns: List[Column]
```

### Comparing `dbrepo-1.4.2rc14/dbrepo/api/exceptions.py` & `dbrepo-1.4.2rc15/dbrepo/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc14/dbrepo.egg-info/PKG-INFO` & `dbrepo-1.4.2rc15/dbrepo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbrepo
-Version: 1.4.2rc14
+Version: 1.4.2rc15
 Summary: DBRepo Python Library
 Home-page: https://www.ifs.tuwien.ac.at/infrastructures/dbrepo//
 Author: Martin Weise
 Author-email: "Martin Weise, TU Wien" <martin.weise@tuwien.ac.at>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
```

### Comparing `dbrepo-1.4.2rc14/dbrepo.egg-info/SOURCES.txt` & `dbrepo-1.4.2rc15/dbrepo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc14/pyproject.toml` & `dbrepo-1.4.2rc15/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dbrepo"
-version = "1.4.2rc14"
+version = "1.4.2rc15"
 description = "DBRepo Python Library"
 keywords = [
     "DBRepo",
     "Database Repository"
 ]
 authors = [
     { name = "Martin Weise, TU Wien", email = "martin.weise@tuwien.ac.at" }
```

### Comparing `dbrepo-1.4.2rc14/tests/test_analyse.py` & `dbrepo-1.4.2rc15/tests/test_analyse.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc14/tests/test_container.py` & `dbrepo-1.4.2rc15/tests/test_container.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc14/tests/test_database.py` & `dbrepo-1.4.2rc15/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc14/tests/test_identifier.py` & `dbrepo-1.4.2rc15/tests/test_identifier.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc14/tests/test_license.py` & `dbrepo-1.4.2rc15/tests/test_license.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc14/tests/test_query.py` & `dbrepo-1.4.2rc15/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc14/tests/test_rest_client.py` & `dbrepo-1.4.2rc15/tests/test_rest_client.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc14/tests/test_table.py` & `dbrepo-1.4.2rc15/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc14/tests/test_user.py` & `dbrepo-1.4.2rc15/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc14/tests/test_view.py` & `dbrepo-1.4.2rc15/tests/test_view.py`

 * *Files identical despite different names*

