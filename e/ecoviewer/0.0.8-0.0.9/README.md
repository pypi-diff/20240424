# Comparing `tmp/ecoviewer-0.0.8.tar.gz` & `tmp/ecoviewer-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecoviewer-0.0.8.tar", last modified: Wed Apr 10 23:13:02 2024, max compression
+gzip compressed data, was "ecoviewer-0.0.9.tar", last modified: Thu Apr 11 16:53:04 2024, max compression
```

## Comparing `ecoviewer-0.0.8.tar` & `ecoviewer-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:13:02.992032 ecoviewer-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-10 23:12:36.000000 ecoviewer-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-10 23:13:02.992032 ecoviewer-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-10 23:12:36.000000 ecoviewer-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-10 23:12:36.000000 ecoviewer-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-10 23:13:02.992032 ecoviewer-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-10 23:12:36.000000 ecoviewer-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:13:02.988032 ecoviewer-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:13:02.992032 ecoviewer-0.0.8/src/ecoviewer/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-10 23:12:36.000000 ecoviewer-0.0.8/src/ecoviewer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:13:02.992032 ecoviewer-0.0.8/src/ecoviewer/config/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-10 23:12:36.000000 ecoviewer-0.0.8/src/ecoviewer/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-04-10 23:12:36.000000 ecoviewer-0.0.8/src/ecoviewer/config/configutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:13:02.992032 ecoviewer-0.0.8/src/ecoviewer/display/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-10 23:12:36.000000 ecoviewer-0.0.8/src/ecoviewer/display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-10 23:12:36.000000 ecoviewer-0.0.8/src/ecoviewer/display/displayutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18786 2024-04-10 23:12:36.000000 ecoviewer-0.0.8/src/ecoviewer/display/graphutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:13:02.992032 ecoviewer-0.0.8/src/ecoviewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-10 23:13:02.000000 ecoviewer-0.0.8/src/ecoviewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-10 23:13:02.000000 ecoviewer-0.0.8/src/ecoviewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 23:13:02.000000 ecoviewer-0.0.8/src/ecoviewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-10 23:13:02.000000 ecoviewer-0.0.8/src/ecoviewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 23:13:02.000000 ecoviewer-0.0.8/src/ecoviewer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:53:04.004462 ecoviewer-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-11 16:52:37.000000 ecoviewer-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-11 16:53:04.004462 ecoviewer-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-11 16:52:37.000000 ecoviewer-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-11 16:52:37.000000 ecoviewer-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-11 16:53:04.004462 ecoviewer-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-11 16:52:37.000000 ecoviewer-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:53:04.000462 ecoviewer-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:53:04.004462 ecoviewer-0.0.9/src/ecoviewer/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-11 16:52:37.000000 ecoviewer-0.0.9/src/ecoviewer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:53:04.004462 ecoviewer-0.0.9/src/ecoviewer/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-11 16:52:37.000000 ecoviewer-0.0.9/src/ecoviewer/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-04-11 16:52:37.000000 ecoviewer-0.0.9/src/ecoviewer/config/configutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:53:04.004462 ecoviewer-0.0.9/src/ecoviewer/display/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-11 16:52:37.000000 ecoviewer-0.0.9/src/ecoviewer/display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-11 16:52:37.000000 ecoviewer-0.0.9/src/ecoviewer/display/displayutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18786 2024-04-11 16:52:37.000000 ecoviewer-0.0.9/src/ecoviewer/display/graphutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:53:04.004462 ecoviewer-0.0.9/src/ecoviewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-11 16:53:03.000000 ecoviewer-0.0.9/src/ecoviewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-11 16:53:04.000000 ecoviewer-0.0.9/src/ecoviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 16:53:03.000000 ecoviewer-0.0.9/src/ecoviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-11 16:53:03.000000 ecoviewer-0.0.9/src/ecoviewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-11 16:53:03.000000 ecoviewer-0.0.9/src/ecoviewer.egg-info/top_level.txt
```

### Comparing `ecoviewer-0.0.8/LICENSE` & `ecoviewer-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ecoviewer-0.0.8/PKG-INFO` & `ecoviewer-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoviewer
-Version: 0.0.8
+Version: 0.0.9
 Summary: Contains functions for use in HVAC Dash applications
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ecoviewer-0.0.8/setup.cfg` & `ecoviewer-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ecoviewer
-version = 0.0.8
+version = 0.0.9
 authors = ["Ecotope"]
 description = Contains functions for use in HVAC Dash applications
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `ecoviewer-0.0.8/src/ecoviewer/config/configutils.py` & `ecoviewer-0.0.9/src/ecoviewer/config/configutils.py`

 * *Files identical despite different names*

### Comparing `ecoviewer-0.0.8/src/ecoviewer/display/displayutils.py` & `ecoviewer-0.0.9/src/ecoviewer/display/displayutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     df = pd.DataFrame({
         "Detail": detail,
         "Information": info
     })
 
     return html.Div([
-        html.H2("Building Meta Data"),
+        html.H2("Building Metadata"),
         dash_table.DataTable(
             data=df.to_dict('records'),
             columns=[{"name": i, "id": i, "presentation": "markdown"} for i in df.columns],
             style_cell={'textAlign': 'left'},
             style_as_list_view=True,
             style_header={
                 'backgroundColor': 'rgb(230, 230, 230)',
```

### Comparing `ecoviewer-0.0.8/src/ecoviewer/display/graphutils.py` & `ecoviewer-0.0.9/src/ecoviewer/display/graphutils.py`

 * *Files identical despite different names*

### Comparing `ecoviewer-0.0.8/src/ecoviewer.egg-info/PKG-INFO` & `ecoviewer-0.0.9/src/ecoviewer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoviewer
-Version: 0.0.8
+Version: 0.0.9
 Summary: Contains functions for use in HVAC Dash applications
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

