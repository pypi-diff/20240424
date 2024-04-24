# Comparing `tmp/datasette-edit-schema-0.8a0.tar.gz` & `tmp/datasette-edit-schema-0.8a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasette-edit-schema-0.8a0.tar", last modified: Sun Feb 18 22:21:42 2024, max compression
+gzip compressed data, was "datasette-edit-schema-0.8a1.tar", last modified: Thu Mar 14 02:32:45 2024, max compression
```

## Comparing `datasette-edit-schema-0.8a0.tar` & `datasette-edit-schema-0.8a1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 22:21:42.140521 datasette-edit-schema-0.8a0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-18 22:21:29.000000 datasette-edit-schema-0.8a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-02-18 22:21:42.140521 datasette-edit-schema-0.8a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-02-18 22:21:29.000000 datasette-edit-schema-0.8a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 22:21:42.136521 datasette-edit-schema-0.8a0/datasette_edit_schema/
--rw-r--r--   0 runner    (1001) docker     (127)    30553 2024-02-18 22:21:29.000000 datasette-edit-schema-0.8a0/datasette_edit_schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 22:21:42.140521 datasette-edit-schema-0.8a0/datasette_edit_schema/static/
--rw-r--r--   0 runner    (1001) docker     (127)   202242 2024-02-18 22:21:29.000000 datasette-edit-schema-0.8a0/datasette_edit_schema/static/draggable.1.0.0-beta.11.bundle.js
--rw-r--r--   0 runner    (1001) docker     (127)   119723 2024-02-18 22:21:29.000000 datasette-edit-schema-0.8a0/datasette_edit_schema/static/draggable.1.0.0-beta.11.bundle.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 22:21:42.140521 datasette-edit-schema-0.8a0/datasette_edit_schema/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-02-18 22:21:29.000000 datasette-edit-schema-0.8a0/datasette_edit_schema/templates/edit_schema_create_table.html
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-02-18 22:21:29.000000 datasette-edit-schema-0.8a0/datasette_edit_schema/templates/edit_schema_database.html
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-02-18 22:21:29.000000 datasette-edit-schema-0.8a0/datasette_edit_schema/templates/edit_schema_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     9382 2024-02-18 22:21:29.000000 datasette-edit-schema-0.8a0/datasette_edit_schema/templates/edit_schema_table.html
--rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-02-18 22:21:29.000000 datasette-edit-schema-0.8a0/datasette_edit_schema/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 22:21:42.140521 datasette-edit-schema-0.8a0/datasette_edit_schema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-02-18 22:21:42.000000 datasette-edit-schema-0.8a0/datasette_edit_schema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-02-18 22:21:42.000000 datasette-edit-schema-0.8a0/datasette_edit_schema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-18 22:21:42.000000 datasette-edit-schema-0.8a0/datasette_edit_schema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-18 22:21:42.000000 datasette-edit-schema-0.8a0/datasette_edit_schema.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-18 22:21:42.000000 datasette-edit-schema-0.8a0/datasette_edit_schema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-18 22:21:42.000000 datasette-edit-schema-0.8a0/datasette_edit_schema.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-02-18 22:21:29.000000 datasette-edit-schema-0.8a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-18 22:21:42.140521 datasette-edit-schema-0.8a0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 22:21:42.140521 datasette-edit-schema-0.8a0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    38209 2024-02-18 22:21:29.000000 datasette-edit-schema-0.8a0/tests/test_edit_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:32:45.417252 datasette-edit-schema-0.8a1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-14 02:32:39.000000 datasette-edit-schema-0.8a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-03-14 02:32:45.417252 datasette-edit-schema-0.8a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-03-14 02:32:39.000000 datasette-edit-schema-0.8a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:32:45.413252 datasette-edit-schema-0.8a1/datasette_edit_schema/
+-rw-r--r--   0 runner    (1001) docker     (127)    30707 2024-03-14 02:32:39.000000 datasette-edit-schema-0.8a1/datasette_edit_schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:32:45.413252 datasette-edit-schema-0.8a1/datasette_edit_schema/static/
+-rw-r--r--   0 runner    (1001) docker     (127)   202242 2024-03-14 02:32:39.000000 datasette-edit-schema-0.8a1/datasette_edit_schema/static/draggable.1.0.0-beta.11.bundle.js
+-rw-r--r--   0 runner    (1001) docker     (127)   119723 2024-03-14 02:32:39.000000 datasette-edit-schema-0.8a1/datasette_edit_schema/static/draggable.1.0.0-beta.11.bundle.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:32:45.413252 datasette-edit-schema-0.8a1/datasette_edit_schema/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-03-14 02:32:39.000000 datasette-edit-schema-0.8a1/datasette_edit_schema/templates/edit_schema_create_table.html
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-03-14 02:32:39.000000 datasette-edit-schema-0.8a1/datasette_edit_schema/templates/edit_schema_database.html
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-14 02:32:39.000000 datasette-edit-schema-0.8a1/datasette_edit_schema/templates/edit_schema_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     9382 2024-03-14 02:32:39.000000 datasette-edit-schema-0.8a1/datasette_edit_schema/templates/edit_schema_table.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-03-14 02:32:39.000000 datasette-edit-schema-0.8a1/datasette_edit_schema/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:32:45.417252 datasette-edit-schema-0.8a1/datasette_edit_schema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-03-14 02:32:45.000000 datasette-edit-schema-0.8a1/datasette_edit_schema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-03-14 02:32:45.000000 datasette-edit-schema-0.8a1/datasette_edit_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 02:32:45.000000 datasette-edit-schema-0.8a1/datasette_edit_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-14 02:32:45.000000 datasette-edit-schema-0.8a1/datasette_edit_schema.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-14 02:32:45.000000 datasette-edit-schema-0.8a1/datasette_edit_schema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-14 02:32:45.000000 datasette-edit-schema-0.8a1/datasette_edit_schema.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-03-14 02:32:39.000000 datasette-edit-schema-0.8a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 02:32:45.417252 datasette-edit-schema-0.8a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:32:45.417252 datasette-edit-schema-0.8a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    38196 2024-03-14 02:32:39.000000 datasette-edit-schema-0.8a1/tests/test_edit_schema.py
```

### Comparing `datasette-edit-schema-0.8a0/LICENSE` & `datasette-edit-schema-0.8a1/LICENSE`

 * *Files identical despite different names*

### Comparing `datasette-edit-schema-0.8a0/PKG-INFO` & `datasette-edit-schema-0.8a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: datasette-edit-schema
-Version: 0.8a0
+Version: 0.8a1
 Summary: Datasette plugin for modifying table schemas
 Author: Simon Willison
 License: Apache-2.0
 Project-URL: Homepage, https://datasette.io/plugins/datasette-edit-schema
 Project-URL: Changelog, https://github.com/simonw/datasette-edit-schema/releases
 Project-URL: Issues, https://github.com/simonw/datasette-edit-schema/issues
 Project-URL: CI, https://github.com/simonw/datasette-edit-schema/actions
 Classifier: Framework :: Datasette
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: datasette>=1.0a9
+Requires-Dist: datasette>=1.0a13
 Requires-Dist: sqlite-utils>=3.35
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-asyncio; extra == "test"
 Requires-Dist: beautifulsoup4; extra == "test"
 Requires-Dist: html5lib; extra == "test"
```

### Comparing `datasette-edit-schema-0.8a0/README.md` & `datasette-edit-schema-0.8a1/README.md`

 * *Files identical despite different names*

### Comparing `datasette-edit-schema-0.8a0/datasette_edit_schema/__init__.py` & `datasette-edit-schema-0.8a1/datasette_edit_schema/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
             return []
         return [
             {
                 "href": datasette.urls.path(
                     "/-/edit-schema/{}/{}".format(database, quote_plus(table))
                 ),
                 "label": "Edit table schema",
+                "description": "Rename the table, add and remove columns...",
             }
         ]
 
     return inner
 
 
 async def can_create_table(datasette, actor, database):
@@ -102,14 +103,15 @@
             return []
         return [
             {
                 "href": datasette.urls.path(
                     "/-/edit-schema/{}/-/create".format(database)
                 ),
                 "label": "Create a table",
+                "description": "Define a new table with specified columns",
             }
         ]
 
     return inner
 
 
 @hookimpl
```

### Comparing `datasette-edit-schema-0.8a0/datasette_edit_schema/static/draggable.1.0.0-beta.11.bundle.js` & `datasette-edit-schema-0.8a1/datasette_edit_schema/static/draggable.1.0.0-beta.11.bundle.js`

 * *Files identical despite different names*

### Comparing `datasette-edit-schema-0.8a0/datasette_edit_schema/static/draggable.1.0.0-beta.11.bundle.min.js` & `datasette-edit-schema-0.8a1/datasette_edit_schema/static/draggable.1.0.0-beta.11.bundle.min.js`

 * *Files identical despite different names*

### Comparing `datasette-edit-schema-0.8a0/datasette_edit_schema/templates/edit_schema_create_table.html` & `datasette-edit-schema-0.8a1/datasette_edit_schema/templates/edit_schema_create_table.html`

 * *Files identical despite different names*

### Comparing `datasette-edit-schema-0.8a0/datasette_edit_schema/templates/edit_schema_database.html` & `datasette-edit-schema-0.8a1/datasette_edit_schema/templates/edit_schema_database.html`

 * *Files identical despite different names*

### Comparing `datasette-edit-schema-0.8a0/datasette_edit_schema/templates/edit_schema_table.html` & `datasette-edit-schema-0.8a1/datasette_edit_schema/templates/edit_schema_table.html`

 * *Files identical despite different names*

### Comparing `datasette-edit-schema-0.8a0/datasette_edit_schema/utils.py` & `datasette-edit-schema-0.8a1/datasette_edit_schema/utils.py`

 * *Files identical despite different names*

### Comparing `datasette-edit-schema-0.8a0/datasette_edit_schema.egg-info/PKG-INFO` & `datasette-edit-schema-0.8a1/datasette_edit_schema.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: datasette-edit-schema
-Version: 0.8a0
+Version: 0.8a1
 Summary: Datasette plugin for modifying table schemas
 Author: Simon Willison
 License: Apache-2.0
 Project-URL: Homepage, https://datasette.io/plugins/datasette-edit-schema
 Project-URL: Changelog, https://github.com/simonw/datasette-edit-schema/releases
 Project-URL: Issues, https://github.com/simonw/datasette-edit-schema/issues
 Project-URL: CI, https://github.com/simonw/datasette-edit-schema/actions
 Classifier: Framework :: Datasette
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: datasette>=1.0a9
+Requires-Dist: datasette>=1.0a13
 Requires-Dist: sqlite-utils>=3.35
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-asyncio; extra == "test"
 Requires-Dist: beautifulsoup4; extra == "test"
 Requires-Dist: html5lib; extra == "test"
```

### Comparing `datasette-edit-schema-0.8a0/datasette_edit_schema.egg-info/SOURCES.txt` & `datasette-edit-schema-0.8a1/datasette_edit_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datasette-edit-schema-0.8a0/pyproject.toml` & `datasette-edit-schema-0.8a1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [project]
 name = "datasette-edit-schema"
-version = "0.8a0"
+version = "0.8a1"
 description = "Datasette plugin for modifying table schemas"
 readme = "README.md"
 authors = [{name = "Simon Willison"}]
 license = {text = "Apache-2.0"}
 classifiers=[
     "Framework :: Datasette",
     "License :: OSI Approved :: Apache Software License"
 ]
 requires-python = ">=3.8"
 dependencies = [
-    "datasette>=1.0a9",
+    "datasette>=1.0a13",
     "sqlite-utils>=3.35",
 ]
 
 [project.urls]
 Homepage = "https://datasette.io/plugins/datasette-edit-schema"
 Changelog = "https://github.com/simonw/datasette-edit-schema/releases"
 Issues = "https://github.com/simonw/datasette-edit-schema/issues"
```

### Comparing `datasette-edit-schema-0.8a0/tests/test_edit_schema.py` & `datasette-edit-schema-0.8a1/tests/test_edit_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         ),
     ]
     cookies = None
     if actor_id:
         cookies = {"ds_actor": ds.sign({"a": {"id": actor_id}}, "actor")}
     response = await ds.client.get("/data/creatures", cookies=cookies)
     assert response.status_code == 200
-    fragment = '<li><a href="/-/edit-schema/data/creatures">Edit table schema</a></li>'
+    fragment = '<a href="/-/edit-schema/data/creatures">Edit table schema'
     if should_allow:
         # Should have table action
         assert fragment in response.text
     else:
         assert fragment not in response.text
```

