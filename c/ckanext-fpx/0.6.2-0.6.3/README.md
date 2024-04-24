# Comparing `tmp/ckanext-fpx-0.6.2.tar.gz` & `tmp/ckanext_fpx-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-fpx-0.6.2.tar", last modified: Thu Sep  7 17:45:14 2023, max compression
+gzip compressed data, was "ckanext_fpx-0.6.3.tar", last modified: Wed Apr 24 12:49:56 2024, max compression
```

## Comparing `ckanext-fpx-0.6.2.tar` & `ckanext_fpx-0.6.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-09-07 17:45:14.200456 ckanext-fpx-0.6.2/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2022-09-12 15:43:11.000000 ckanext-fpx-0.6.2/LICENSE
--rw-r--r--   0 sergey    (1000) sergey    (1000)      142 2022-09-12 15:43:11.000000 ckanext-fpx-0.6.2/MANIFEST.in
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1299 2023-09-07 17:45:14.200456 ckanext-fpx-0.6.2/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)      736 2022-09-12 15:43:11.000000 ckanext-fpx-0.6.2/README.md
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-09-07 17:45:14.190456 ckanext-fpx-0.6.2/ckanext/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      221 2022-09-12 15:43:11.000000 ckanext-fpx-0.6.2/ckanext/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-09-07 17:45:14.190456 ckanext-fpx-0.6.2/ckanext/fpx/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-09-12 15:43:11.000000 ckanext-fpx-0.6.2/ckanext/fpx/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-09-07 17:45:14.190456 ckanext-fpx-0.6.2/ckanext/fpx/assets/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-09-07 17:45:14.190456 ckanext-fpx-0.6.2/ckanext/fpx/assets/scripts/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      651 2022-09-12 15:43:11.000000 ckanext-fpx-0.6.2/ckanext/fpx/assets/scripts/fpx-download-starting-toast.js
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1151 2022-09-12 15:43:11.000000 ckanext-fpx-0.6.2/ckanext/fpx/assets/scripts/fpx-position-tracker-toast.js
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3237 2022-09-19 11:33:29.000000 ckanext-fpx-0.6.2/ckanext/fpx/assets/scripts/fpx-queue-manager.js
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-09-07 17:45:14.190456 ckanext-fpx-0.6.2/ckanext/fpx/assets/styles/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      578 2022-09-12 15:43:11.000000 ckanext-fpx-0.6.2/ckanext/fpx/assets/styles/fpx-toast-styles.css
--rw-r--r--   0 sergey    (1000) sergey    (1000)      550 2022-09-12 15:43:11.000000 ckanext-fpx-0.6.2/ckanext/fpx/assets/webassets.yml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2996 2022-09-19 11:59:40.000000 ckanext-fpx-0.6.2/ckanext/fpx/helpers.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2753 2022-09-16 13:43:17.000000 ckanext-fpx-0.6.2/ckanext/fpx/interfaces.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-09-07 17:45:14.190456 ckanext-fpx-0.6.2/ckanext/fpx/logic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-09-12 15:43:11.000000 ckanext-fpx-0.6.2/ckanext/fpx/logic/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2403 2023-09-07 17:41:49.000000 ckanext-fpx-0.6.2/ckanext/fpx/logic/action.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      249 2022-09-12 15:43:11.000000 ckanext-fpx-0.6.2/ckanext/fpx/logic/auth.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      300 2023-09-07 17:24:59.000000 ckanext-fpx-0.6.2/ckanext/fpx/logic/schema.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      564 2023-09-07 17:26:50.000000 ckanext-fpx-0.6.2/ckanext/fpx/logic/validators.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1217 2022-09-16 13:43:17.000000 ckanext-fpx-0.6.2/ckanext/fpx/plugin.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-09-07 17:45:14.190456 ckanext-fpx-0.6.2/ckanext/fpx/templates/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-09-07 17:45:14.190456 ckanext-fpx-0.6.2/ckanext/fpx/templates/fpx/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-09-07 17:45:14.190456 ckanext-fpx-0.6.2/ckanext/fpx/templates/fpx/snippets/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      715 2022-09-12 15:43:11.000000 ckanext-fpx-0.6.2/ckanext/fpx/templates/fpx/snippets/download_starting_toast.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1024 2022-09-12 15:43:11.000000 ckanext-fpx-0.6.2/ckanext/fpx/templates/fpx/snippets/position_tracker_toast.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2022-09-12 15:43:11.000000 ckanext-fpx-0.6.2/ckanext/fpx/templates/fpx/snippets/static.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)      394 2022-09-19 11:22:18.000000 ckanext-fpx-0.6.2/ckanext/fpx/templates/page.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-09-07 17:45:14.200456 ckanext-fpx-0.6.2/ckanext/fpx/tests/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-09-12 15:43:11.000000 ckanext-fpx-0.6.2/ckanext/fpx/tests/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-09-07 17:45:14.200456 ckanext-fpx-0.6.2/ckanext/fpx/tests/logic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-09-12 15:43:11.000000 ckanext-fpx-0.6.2/ckanext/fpx/tests/logic/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      503 2022-09-12 15:43:11.000000 ckanext-fpx-0.6.2/ckanext/fpx/tests/logic/test_action.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1526 2022-09-12 15:43:11.000000 ckanext-fpx-0.6.2/ckanext/fpx/tests/test_helpers.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      142 2022-09-12 15:43:11.000000 ckanext-fpx-0.6.2/ckanext/fpx/tests/test_plugin.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      507 2022-09-12 15:43:11.000000 ckanext-fpx-0.6.2/ckanext/fpx/tests/test_utils.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      926 2022-09-20 10:59:39.000000 ckanext-fpx-0.6.2/ckanext/fpx/utils.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1505 2023-09-07 17:26:30.000000 ckanext-fpx-0.6.2/ckanext/fpx/views.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-09-07 17:45:14.200456 ckanext-fpx-0.6.2/ckanext_fpx.egg-info/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1299 2023-09-07 17:45:14.000000 ckanext-fpx-0.6.2/ckanext_fpx.egg-info/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1290 2023-09-07 17:45:14.000000 ckanext-fpx-0.6.2/ckanext_fpx.egg-info/SOURCES.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-09-07 17:45:14.000000 ckanext-fpx-0.6.2/ckanext_fpx.egg-info/dependency_links.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      107 2023-09-07 17:45:14.000000 ckanext-fpx-0.6.2/ckanext_fpx.egg-info/entry_points.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-09-07 17:45:14.000000 ckanext-fpx-0.6.2/ckanext_fpx.egg-info/namespace_packages.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        6 2023-09-07 17:45:14.000000 ckanext-fpx-0.6.2/ckanext_fpx.egg-info/requires.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-09-07 17:45:14.000000 ckanext-fpx-0.6.2/ckanext_fpx.egg-info/top_level.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       45 2022-09-12 15:43:11.000000 ckanext-fpx-0.6.2/pyproject.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-09-12 15:43:11.000000 ckanext-fpx-0.6.2/requirements.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1433 2023-09-07 17:45:14.200456 ckanext-fpx-0.6.2/setup.cfg
--rw-r--r--   0 sergey    (1000) sergey    (1000)      312 2022-09-12 15:43:11.000000 ckanext-fpx-0.6.2/setup.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 12:49:56.943071 ckanext_fpx-0.6.3/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2024-03-31 18:39:35.000000 ckanext_fpx-0.6.3/LICENSE
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      142 2024-03-31 18:39:35.000000 ckanext_fpx-0.6.3/MANIFEST.in
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1299 2024-04-24 12:49:56.943071 ckanext_fpx-0.6.3/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      736 2024-03-31 18:39:35.000000 ckanext_fpx-0.6.3/README.md
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 12:49:56.939738 ckanext_fpx-0.6.3/ckanext/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      221 2024-03-31 18:39:35.000000 ckanext_fpx-0.6.3/ckanext/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 12:49:56.939738 ckanext_fpx-0.6.3/ckanext/fpx/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-03-31 18:39:35.000000 ckanext_fpx-0.6.3/ckanext/fpx/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 12:49:56.939738 ckanext_fpx-0.6.3/ckanext/fpx/assets/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 12:49:56.939738 ckanext_fpx-0.6.3/ckanext/fpx/assets/scripts/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      651 2024-03-31 18:39:35.000000 ckanext_fpx-0.6.3/ckanext/fpx/assets/scripts/fpx-download-starting-toast.js
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1151 2024-03-31 18:39:35.000000 ckanext_fpx-0.6.3/ckanext/fpx/assets/scripts/fpx-position-tracker-toast.js
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3237 2024-03-31 18:39:35.000000 ckanext_fpx-0.6.3/ckanext/fpx/assets/scripts/fpx-queue-manager.js
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 12:49:56.939738 ckanext_fpx-0.6.3/ckanext/fpx/assets/styles/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      578 2024-03-31 18:39:35.000000 ckanext_fpx-0.6.3/ckanext/fpx/assets/styles/fpx-toast-styles.css
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      550 2024-03-31 18:39:35.000000 ckanext_fpx-0.6.3/ckanext/fpx/assets/webassets.yml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2996 2024-03-31 18:39:35.000000 ckanext_fpx-0.6.3/ckanext/fpx/helpers.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2812 2024-04-24 12:46:58.000000 ckanext_fpx-0.6.3/ckanext/fpx/interfaces.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 12:49:56.939738 ckanext_fpx-0.6.3/ckanext/fpx/logic/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-03-31 18:39:35.000000 ckanext_fpx-0.6.3/ckanext/fpx/logic/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2403 2024-04-24 12:40:17.000000 ckanext_fpx-0.6.3/ckanext/fpx/logic/action.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      249 2024-03-31 18:39:35.000000 ckanext_fpx-0.6.3/ckanext/fpx/logic/auth.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      300 2024-03-31 18:39:35.000000 ckanext_fpx-0.6.3/ckanext/fpx/logic/schema.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      564 2024-03-31 18:39:35.000000 ckanext_fpx-0.6.3/ckanext/fpx/logic/validators.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1217 2024-03-31 18:39:35.000000 ckanext_fpx-0.6.3/ckanext/fpx/plugin.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 12:49:56.939738 ckanext_fpx-0.6.3/ckanext/fpx/templates/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 12:49:56.936404 ckanext_fpx-0.6.3/ckanext/fpx/templates/fpx/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 12:49:56.939738 ckanext_fpx-0.6.3/ckanext/fpx/templates/fpx/snippets/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      715 2024-03-31 18:39:35.000000 ckanext_fpx-0.6.3/ckanext/fpx/templates/fpx/snippets/download_starting_toast.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1024 2024-03-31 18:39:35.000000 ckanext_fpx-0.6.3/ckanext/fpx/templates/fpx/snippets/position_tracker_toast.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2024-03-31 18:39:35.000000 ckanext_fpx-0.6.3/ckanext/fpx/templates/fpx/snippets/static.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      394 2024-03-31 18:39:35.000000 ckanext_fpx-0.6.3/ckanext/fpx/templates/page.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 12:49:56.939738 ckanext_fpx-0.6.3/ckanext/fpx/tests/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-03-31 18:39:35.000000 ckanext_fpx-0.6.3/ckanext/fpx/tests/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 12:49:56.939738 ckanext_fpx-0.6.3/ckanext/fpx/tests/logic/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-03-31 18:39:35.000000 ckanext_fpx-0.6.3/ckanext/fpx/tests/logic/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      503 2024-03-31 18:39:35.000000 ckanext_fpx-0.6.3/ckanext/fpx/tests/logic/test_action.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1526 2024-03-31 18:39:35.000000 ckanext_fpx-0.6.3/ckanext/fpx/tests/test_helpers.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      142 2024-03-31 18:39:35.000000 ckanext_fpx-0.6.3/ckanext/fpx/tests/test_plugin.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      507 2024-03-31 18:39:35.000000 ckanext_fpx-0.6.3/ckanext/fpx/tests/test_utils.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      926 2024-03-31 18:39:35.000000 ckanext_fpx-0.6.3/ckanext/fpx/utils.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1505 2024-03-31 18:39:35.000000 ckanext_fpx-0.6.3/ckanext/fpx/views.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 12:49:56.939738 ckanext_fpx-0.6.3/ckanext_fpx.egg-info/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1299 2024-04-24 12:49:56.000000 ckanext_fpx-0.6.3/ckanext_fpx.egg-info/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1290 2024-04-24 12:49:56.000000 ckanext_fpx-0.6.3/ckanext_fpx.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2024-04-24 12:49:56.000000 ckanext_fpx-0.6.3/ckanext_fpx.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      107 2024-04-24 12:49:56.000000 ckanext_fpx-0.6.3/ckanext_fpx.egg-info/entry_points.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2024-04-24 12:49:56.000000 ckanext_fpx-0.6.3/ckanext_fpx.egg-info/namespace_packages.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        6 2024-04-24 12:49:56.000000 ckanext_fpx-0.6.3/ckanext_fpx.egg-info/requires.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2024-04-24 12:49:56.000000 ckanext_fpx-0.6.3/ckanext_fpx.egg-info/top_level.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       45 2024-03-31 18:39:35.000000 ckanext_fpx-0.6.3/pyproject.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-03-31 18:39:35.000000 ckanext_fpx-0.6.3/requirements.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1433 2024-04-24 12:49:56.943071 ckanext_fpx-0.6.3/setup.cfg
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      312 2024-03-31 18:39:35.000000 ckanext_fpx-0.6.3/setup.py
```

### Comparing `ckanext-fpx-0.6.2/LICENSE` & `ckanext_fpx-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-fpx-0.6.2/PKG-INFO` & `ckanext_fpx-0.6.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-fpx
-Version: 0.6.2
+Version: 0.6.3
 Home-page: https://github.com/DataShades/ckanext-fpx
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ckanext-fpx-0.6.2/README.md` & `ckanext_fpx-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-fpx-0.6.2/ckanext/fpx/assets/scripts/fpx-download-starting-toast.js` & `ckanext_fpx-0.6.3/ckanext/fpx/assets/scripts/fpx-download-starting-toast.js`

 * *Files identical despite different names*

### Comparing `ckanext-fpx-0.6.2/ckanext/fpx/assets/scripts/fpx-position-tracker-toast.js` & `ckanext_fpx-0.6.3/ckanext/fpx/assets/scripts/fpx-position-tracker-toast.js`

 * *Files identical despite different names*

### Comparing `ckanext-fpx-0.6.2/ckanext/fpx/assets/scripts/fpx-queue-manager.js` & `ckanext_fpx-0.6.3/ckanext/fpx/assets/scripts/fpx-queue-manager.js`

 * *Files identical despite different names*

### Comparing `ckanext-fpx-0.6.2/ckanext/fpx/assets/styles/fpx-toast-styles.css` & `ckanext_fpx-0.6.3/ckanext/fpx/assets/styles/fpx-toast-styles.css`

 * *Files identical despite different names*

### Comparing `ckanext-fpx-0.6.2/ckanext/fpx/assets/webassets.yml` & `ckanext_fpx-0.6.3/ckanext/fpx/assets/webassets.yml`

 * *Files identical despite different names*

### Comparing `ckanext-fpx-0.6.2/ckanext/fpx/helpers.py` & `ckanext_fpx-0.6.3/ckanext/fpx/helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-fpx-0.6.2/ckanext/fpx/interfaces.py` & `ckanext_fpx-0.6.3/ckanext/fpx/interfaces.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 import logging
 
 from typing import Any, Optional
-
+from ckan.lib.search.query import solr_literal
 import ckan.plugins.toolkit as tk
 from ckan.plugins.interfaces import Interface
 
 log = logging.getLogger(__name__)
 
 
 class IFpx(Interface):
@@ -55,19 +55,21 @@
             log.warning(
                 "Passing items as scalar value when type set to 'package' is "
                 "deprecated. Use list instead."
             )
             items = [items]
 
         fq_list = [
-            "{!q.op=OR}id:(%s)"
-            % " ".join(['"{}"'.format(item) for item in items])
+            "id:({})".format(
+                " OR ".join([solr_literal(item) for item in items])
+            )
         ]
+
         result = tk.get_action("package_search")(
-            None, {"fq_list": fq_list, "include_private": True}
+            {}, {"fq_list": fq_list, "include_private": True}
         )
 
         items = [
             {"url": self.fpx_url_from_resource(r), "path": pkg["name"]}
             for pkg in result["results"]
             for r in pkg["resources"]
         ]
@@ -77,13 +79,13 @@
     def _fpx_resource_normalizer(
         self, items: list[Any]
     ) -> tuple[list[dict[str, Any]], str]:
         """Normalize items when initial type is "resource" """
         items = [
             {
                 "url": self.fpx_url_from_resource(
-                    tk.get_action("resource_show")(None, {"id": r["id"]})
+                    tk.get_action("resource_show")({}, {"id": r["id"]})
                 )
             }
             for r in items
         ]
         return items, "zip"
```

### Comparing `ckanext-fpx-0.6.2/ckanext/fpx/logic/action.py` & `ckanext_fpx-0.6.3/ckanext/fpx/logic/action.py`

 * *Files identical despite different names*

### Comparing `ckanext-fpx-0.6.2/ckanext/fpx/logic/validators.py` & `ckanext_fpx-0.6.3/ckanext/fpx/logic/validators.py`

 * *Files identical despite different names*

### Comparing `ckanext-fpx-0.6.2/ckanext/fpx/plugin.py` & `ckanext_fpx-0.6.3/ckanext/fpx/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-fpx-0.6.2/ckanext/fpx/templates/fpx/snippets/download_starting_toast.html` & `ckanext_fpx-0.6.3/ckanext/fpx/templates/fpx/snippets/download_starting_toast.html`

 * *Files identical despite different names*

### Comparing `ckanext-fpx-0.6.2/ckanext/fpx/templates/fpx/snippets/position_tracker_toast.html` & `ckanext_fpx-0.6.3/ckanext/fpx/templates/fpx/snippets/position_tracker_toast.html`

 * *Files identical despite different names*

### Comparing `ckanext-fpx-0.6.2/ckanext/fpx/tests/test_helpers.py` & `ckanext_fpx-0.6.3/ckanext/fpx/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-fpx-0.6.2/ckanext/fpx/utils.py` & `ckanext_fpx-0.6.3/ckanext/fpx/utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-fpx-0.6.2/ckanext/fpx/views.py` & `ckanext_fpx-0.6.3/ckanext/fpx/views.py`

 * *Files identical despite different names*

### Comparing `ckanext-fpx-0.6.2/ckanext_fpx.egg-info/PKG-INFO` & `ckanext_fpx-0.6.3/ckanext_fpx.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-fpx
-Version: 0.6.2
+Version: 0.6.3
 Home-page: https://github.com/DataShades/ckanext-fpx
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ckanext-fpx-0.6.2/ckanext_fpx.egg-info/SOURCES.txt` & `ckanext_fpx-0.6.3/ckanext_fpx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-fpx-0.6.2/setup.cfg` & `ckanext_fpx-0.6.3/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ckanext-fpx
-version = 0.6.2
+version = 0.6.3
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/DataShades/ckanext-fpx
 author = Sergey Motornyuk
 author_email = sergey.motornyuk@linkdigital.com.au
 license = AGPL
 classifiers =
```

