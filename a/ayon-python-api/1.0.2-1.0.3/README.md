# Comparing `tmp/ayon-python-api-1.0.2.tar.gz` & `tmp/ayon-python-api-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ayon-python-api-1.0.2.tar", last modified: Mon Apr 22 08:17:28 2024, max compression
+gzip compressed data, was "ayon-python-api-1.0.3.tar", last modified: Wed Apr 24 13:51:53 2024, max compression
```

## Comparing `ayon-python-api-1.0.2.tar` & `ayon-python-api-1.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:17:28.876161 ayon-python-api-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-22 08:17:20.000000 ayon-python-api-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16210 2024-04-22 08:17:28.876161 ayon-python-api-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-22 08:17:20.000000 ayon-python-api-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:17:28.876161 ayon-python-api-1.0.2/ayon_api/
--rw-r--r--   0 runner    (1001) docker     (127)    10045 2024-04-22 08:17:20.000000 ayon-python-api-1.0.2/ayon_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   123859 2024-04-22 08:17:20.000000 ayon-python-api-1.0.2/ayon_api/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-04-22 08:17:20.000000 ayon-python-api-1.0.2/ayon_api/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    86216 2024-04-22 08:17:20.000000 ayon-python-api-1.0.2/ayon_api/entity_hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-22 08:17:20.000000 ayon-python-api-1.0.2/ayon_api/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-22 08:17:20.000000 ayon-python-api-1.0.2/ayon_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    25889 2024-04-22 08:17:20.000000 ayon-python-api-1.0.2/ayon_api/graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)    21938 2024-04-22 08:17:20.000000 ayon-python-api-1.0.2/ayon_api/graphql_queries.py
--rw-r--r--   0 runner    (1001) docker     (127)    42241 2024-04-22 08:17:20.000000 ayon-python-api-1.0.2/ayon_api/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)   247562 2024-04-22 08:17:20.000000 ayon-python-api-1.0.2/ayon_api/server_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    18155 2024-04-22 08:17:20.000000 ayon-python-api-1.0.2/ayon_api/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-22 08:17:20.000000 ayon-python-api-1.0.2/ayon_api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:17:28.876161 ayon-python-api-1.0.2/ayon_python_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16210 2024-04-22 08:17:28.000000 ayon-python-api-1.0.2/ayon_python_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-22 08:17:28.000000 ayon-python-api-1.0.2/ayon_python_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 08:17:28.000000 ayon-python-api-1.0.2/ayon_python_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-22 08:17:28.000000 ayon-python-api-1.0.2/ayon_python_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-22 08:17:28.000000 ayon-python-api-1.0.2/ayon_python_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-22 08:17:20.000000 ayon-python-api-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 08:17:28.876161 ayon-python-api-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-22 08:17:20.000000 ayon-python-api-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:51:53.367935 ayon-python-api-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 13:51:43.000000 ayon-python-api-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16210 2024-04-24 13:51:53.367935 ayon-python-api-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-24 13:51:43.000000 ayon-python-api-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:51:53.367935 ayon-python-api-1.0.3/ayon_api/
+-rw-r--r--   0 runner    (1001) docker     (127)    10045 2024-04-24 13:51:43.000000 ayon-python-api-1.0.3/ayon_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   123859 2024-04-24 13:51:43.000000 ayon-python-api-1.0.3/ayon_api/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-04-24 13:51:43.000000 ayon-python-api-1.0.3/ayon_api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86216 2024-04-24 13:51:43.000000 ayon-python-api-1.0.3/ayon_api/entity_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-24 13:51:43.000000 ayon-python-api-1.0.3/ayon_api/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-24 13:51:43.000000 ayon-python-api-1.0.3/ayon_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25889 2024-04-24 13:51:43.000000 ayon-python-api-1.0.3/ayon_api/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21938 2024-04-24 13:51:43.000000 ayon-python-api-1.0.3/ayon_api/graphql_queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42241 2024-04-24 13:51:43.000000 ayon-python-api-1.0.3/ayon_api/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)   247665 2024-04-24 13:51:43.000000 ayon-python-api-1.0.3/ayon_api/server_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18155 2024-04-24 13:51:43.000000 ayon-python-api-1.0.3/ayon_api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-24 13:51:43.000000 ayon-python-api-1.0.3/ayon_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:51:53.367935 ayon-python-api-1.0.3/ayon_python_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16210 2024-04-24 13:51:53.000000 ayon-python-api-1.0.3/ayon_python_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-24 13:51:53.000000 ayon-python-api-1.0.3/ayon_python_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:51:53.000000 ayon-python-api-1.0.3/ayon_python_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-24 13:51:53.000000 ayon-python-api-1.0.3/ayon_python_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 13:51:53.000000 ayon-python-api-1.0.3/ayon_python_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-24 13:51:43.000000 ayon-python-api-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 13:51:53.367935 ayon-python-api-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-24 13:51:43.000000 ayon-python-api-1.0.3/setup.py
```

### Comparing `ayon-python-api-1.0.2/LICENSE` & `ayon-python-api-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ayon-python-api-1.0.2/PKG-INFO` & `ayon-python-api-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ayon-python-api
-Version: 1.0.2
+Version: 1.0.3
 Summary: AYON Python API
 Home-page: https://github.com/ynput/ayon-python-api
 Author: ynput.io
 Author-email: "ynput.io" <info@ynput.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `ayon-python-api-1.0.2/README.md` & `ayon-python-api-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ayon-python-api-1.0.2/ayon_api/__init__.py` & `ayon-python-api-1.0.3/ayon_api/__init__.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-1.0.2/ayon_api/_api.py` & `ayon-python-api-1.0.3/ayon_api/_api.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-1.0.2/ayon_api/constants.py` & `ayon-python-api-1.0.3/ayon_api/constants.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-1.0.2/ayon_api/entity_hub.py` & `ayon-python-api-1.0.3/ayon_api/entity_hub.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-1.0.2/ayon_api/events.py` & `ayon-python-api-1.0.3/ayon_api/events.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-1.0.2/ayon_api/exceptions.py` & `ayon-python-api-1.0.3/ayon_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-1.0.2/ayon_api/graphql.py` & `ayon-python-api-1.0.3/ayon_api/graphql.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-1.0.2/ayon_api/graphql_queries.py` & `ayon-python-api-1.0.3/ayon_api/graphql_queries.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-1.0.2/ayon_api/operations.py` & `ayon-python-api-1.0.3/ayon_api/operations.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-1.0.2/ayon_api/server_api.py` & `ayon-python-api-1.0.3/ayon_api/server_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -3532,15 +3532,18 @@
 
         """
         if fields is not None:
             fields = set(fields)
 
         use_rest = self._should_use_rest_project(fields)
         if use_rest:
-            return self.get_rest_project(project_name)
+            project = self.get_rest_project(project_name)
+            if own_attributes:
+                fill_own_attribs(project)
+            return project
 
         self._prepare_project_fields(fields, own_attributes)
 
         query = project_graphql_query(fields)
         query.set_variable_value("projectName", project_name)
 
         parsed_data = query.query(self)
```

### Comparing `ayon-python-api-1.0.2/ayon_api/utils.py` & `ayon-python-api-1.0.3/ayon_api/utils.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-1.0.2/ayon_python_api.egg-info/PKG-INFO` & `ayon-python-api-1.0.3/ayon_python_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ayon-python-api
-Version: 1.0.2
+Version: 1.0.3
 Summary: AYON Python API
 Home-page: https://github.com/ynput/ayon-python-api
 Author: ynput.io
 Author-email: "ynput.io" <info@ynput.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `ayon-python-api-1.0.2/pyproject.toml` & `ayon-python-api-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ayon-python-api"
-version = "1.0.2"
+version = "1.0.3"
 description = "AYON Python API"
 license = {file = "LICENSE"}
 readme = {file = "README.md", content-type = "text/markdown"}
 authors = [
     {name = "ynput.io", email = "info@ynput.io"}
 ]
 keywords = ["AYON", "ynput", "OpenPype", "vfx"]
@@ -27,15 +27,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ayon-python-api"
-version = "1.0.2"
+version = "1.0.3"
 description = "AYON Python API"
 authors = [
     "ynput.io <info@ynput.io>"
 ]
 
 [tool.poetry.dependencies]
 python = ">=2.7,>=3.6.5"
```

### Comparing `ayon-python-api-1.0.2/setup.py` & `ayon-python-api-1.0.3/setup.py`

 * *Files identical despite different names*

