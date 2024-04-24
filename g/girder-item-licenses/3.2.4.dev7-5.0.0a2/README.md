# Comparing `tmp/girder-item-licenses-3.2.4.dev7.tar.gz` & `tmp/girder-item-licenses-5.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girder-item-licenses-3.2.4.dev7.tar", last modified: Wed Apr 24 19:13:25 2024, max compression
+gzip compressed data, was "girder-item-licenses-5.0.0a2.tar", last modified: Fri Apr 12 16:31:03 2024, max compression
```

## Comparing `girder-item-licenses-3.2.4.dev7.tar` & `girder-item-licenses-5.0.0a2.tar`

### file list

```diff
@@ -1,39 +1,25 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:25.438476 girder-item-licenses-3.2.4.dev7/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      519 2024-04-24 19:13:25.438476 girder-item-licenses-3.2.4.dev7/PKG-INFO
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:25.430476 girder-item-licenses-3.2.4.dev7/girder_item_licenses/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2831 2024-04-24 19:11:47.000000 girder-item-licenses-3.2.4.dev7/girder_item_licenses/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      653 2024-04-24 19:11:47.000000 girder-item-licenses-3.2.4.dev7/girder_item_licenses/rest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4514 2024-04-24 19:11:47.000000 girder-item-licenses-3.2.4.dev7/girder_item_licenses/settings.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:25.434476 girder-item-licenses-3.2.4.dev7/girder_item_licenses/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      174 2024-04-24 19:11:47.000000 girder-item-licenses-3.2.4.dev7/girder_item_licenses/web_client/main.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      478 2024-04-24 19:11:47.000000 girder-item-licenses-3.2.4.dev7/girder_item_licenses/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      441 2024-04-24 19:11:47.000000 girder-item-licenses-3.2.4.dev7/girder_item_licenses/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:25.434476 girder-item-licenses-3.2.4.dev7/girder_item_licenses/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       81 2024-04-24 19:11:47.000000 girder-item-licenses-3.2.4.dev7/girder_item_licenses/web_client/stylesheets/configView.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:25.434476 girder-item-licenses-3.2.4.dev7/girder_item_licenses/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      504 2024-04-24 19:11:47.000000 girder-item-licenses-3.2.4.dev7/girder_item_licenses/web_client/templates/configView.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      175 2024-04-24 19:11:47.000000 girder-item-licenses-3.2.4.dev7/girder_item_licenses/web_client/templates/itemLicenseWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      406 2024-04-24 19:11:47.000000 girder-item-licenses-3.2.4.dev7/girder_item_licenses/web_client/templates/selectLicenseWidget.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:25.434476 girder-item-licenses-3.2.4.dev7/girder_item_licenses/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2499 2024-04-24 19:11:47.000000 girder-item-licenses-3.2.4.dev7/girder_item_licenses/web_client/views/ConfigView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1480 2024-04-24 19:11:47.000000 girder-item-licenses-3.2.4.dev7/girder_item_licenses/web_client/views/EditItemWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      815 2024-04-24 19:11:47.000000 girder-item-licenses-3.2.4.dev7/girder_item_licenses/web_client/views/HierarchyWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      471 2024-04-24 19:11:47.000000 girder-item-licenses-3.2.4.dev7/girder_item_licenses/web_client/views/ItemLicenseWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1047 2024-04-24 19:11:47.000000 girder-item-licenses-3.2.4.dev7/girder_item_licenses/web_client/views/ItemView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2024-04-24 19:11:47.000000 girder-item-licenses-3.2.4.dev7/girder_item_licenses/web_client/views/SelectLicenseWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1576 2024-04-24 19:11:47.000000 girder-item-licenses-3.2.4.dev7/girder_item_licenses/web_client/views/UploadWidget.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:25.434476 girder-item-licenses-3.2.4.dev7/girder_item_licenses.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      519 2024-04-24 19:13:25.000000 girder-item-licenses-3.2.4.dev7/girder_item_licenses.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1281 2024-04-24 19:13:25.000000 girder-item-licenses-3.2.4.dev7/girder_item_licenses.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-24 19:13:25.000000 girder-item-licenses-3.2.4.dev7/girder_item_licenses.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       72 2024-04-24 19:13:25.000000 girder-item-licenses-3.2.4.dev7/girder_item_licenses.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-24 19:13:25.000000 girder-item-licenses-3.2.4.dev7/girder_item_licenses.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-04-24 19:13:25.000000 girder-item-licenses-3.2.4.dev7/girder_item_licenses.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2024-04-24 19:13:25.000000 girder-item-licenses-3.2.4.dev7/girder_item_licenses.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       58 2024-04-24 19:11:47.000000 girder-item-licenses-3.2.4.dev7/plugin.cmake
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:25.434476 girder-item-licenses-3.2.4.dev7/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:11:47.000000 girder-item-licenses-3.2.4.dev7/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15913 2024-04-24 19:11:47.000000 girder-item-licenses-3.2.4.dev7/plugin_tests/itemLicensesSpec.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12348 2024-04-24 19:11:47.000000 girder-item-licenses-3.2.4.dev7/plugin_tests/item_licenses_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-24 19:13:25.438476 girder-item-licenses-3.2.4.dev7/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1599 2024-04-24 19:11:47.000000 girder-item-licenses-3.2.4.dev7/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:31:03.800740 girder-item-licenses-5.0.0a2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      174 2024-04-12 16:27:18.000000 girder-item-licenses-5.0.0a2/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      516 2024-04-12 16:31:03.800740 girder-item-licenses-5.0.0a2/PKG-INFO
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:31:03.800740 girder-item-licenses-5.0.0a2/girder_item_licenses/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3127 2024-04-12 16:27:18.000000 girder-item-licenses-5.0.0a2/girder_item_licenses/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      653 2024-04-12 16:27:18.000000 girder-item-licenses-5.0.0a2/girder_item_licenses/rest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4514 2024-04-12 16:27:18.000000 girder-item-licenses-5.0.0a2/girder_item_licenses/settings.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:31:03.796740 girder-item-licenses-5.0.0a2/girder_item_licenses/web_client/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:31:03.800740 girder-item-licenses-5.0.0a2/girder_item_licenses/web_client/dist/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15123 2024-04-12 16:28:23.000000 girder-item-licenses-5.0.0a2/girder_item_licenses/web_client/dist/girder-plugin-item-licenses.umd.cjs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       75 2024-04-12 16:28:23.000000 girder-item-licenses-5.0.0a2/girder_item_licenses/web_client/dist/style.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:31:03.800740 girder-item-licenses-5.0.0a2/girder_item_licenses.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      516 2024-04-12 16:31:03.000000 girder-item-licenses-5.0.0a2/girder_item_licenses.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      617 2024-04-12 16:31:03.000000 girder-item-licenses-5.0.0a2/girder_item_licenses.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 16:31:03.000000 girder-item-licenses-5.0.0a2/girder_item_licenses.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       72 2024-04-12 16:31:03.000000 girder-item-licenses-5.0.0a2/girder_item_licenses.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 16:31:03.000000 girder-item-licenses-5.0.0a2/girder_item_licenses.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-04-12 16:31:03.000000 girder-item-licenses-5.0.0a2/girder_item_licenses.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2024-04-12 16:31:03.000000 girder-item-licenses-5.0.0a2/girder_item_licenses.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       58 2024-04-12 16:27:18.000000 girder-item-licenses-5.0.0a2/plugin.cmake
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:31:03.800740 girder-item-licenses-5.0.0a2/plugin_tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:27:18.000000 girder-item-licenses-5.0.0a2/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12348 2024-04-12 16:27:18.000000 girder-item-licenses-5.0.0a2/plugin_tests/item_licenses_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-12 16:31:03.800740 girder-item-licenses-5.0.0a2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1599 2024-04-12 16:27:18.000000 girder-item-licenses-5.0.0a2/setup.py
```

### Comparing `girder-item-licenses-3.2.4.dev7/PKG-INFO` & `girder-item-licenses-5.0.0a2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-item-licenses
-Version: 3.2.4.dev7
+Version: 5.0.0a2
 Summary: Add a license field to items.
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `girder-item-licenses-3.2.4.dev7/girder_item_licenses/__init__.py` & `girder-item-licenses-5.0.0a2/girder_item_licenses/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+from pathlib import Path
+
 from girder import events
 from girder.constants import AccessType
 from girder.exceptions import ValidationException
 from girder.models.item import Item
 from girder.models.setting import Setting
-from girder.plugin import GirderPlugin
+from girder.plugin import GirderPlugin, registerPluginStaticContent
 
 from .rest import getLicenses
 from .settings import PluginSettings
 
 
 def validateString(value):
     """
@@ -72,15 +74,14 @@
 def validateItem(event):
     item = event.info
     item['license'] = validateString(item.get('license', None))
 
 
 class ItemLicensesPlugin(GirderPlugin):
     DISPLAY_NAME = 'Item Licenses'
-    CLIENT_SOURCE_PATH = 'web_client'
 
     def load(self, info):
         # Bind REST events
         events.bind('rest.post.item.after', 'item_licenses', postItemAfter)
         events.bind('rest.post.item/:id/copy.after', 'item_licenses', postItemCopyAfter)
         events.bind('rest.put.item/:id.after', 'item_licenses', putItemAfter)
 
@@ -88,7 +89,15 @@
         events.bind('model.item.validate', 'item_licenses', validateItem)
 
         # Add license field to item model
         Item().exposeFields(level=AccessType.READ, fields='license')
 
         # Add endpoint to get list of licenses
         info['apiRoot'].item.route('GET', ('licenses',), getLicenses)
+
+        registerPluginStaticContent(
+            plugin='item_licenses',
+            css=['/style.css'],
+            js=['/girder-plugin-item-licenses.umd.cjs'],
+            staticDir=Path(__file__).parent / 'web_client' / 'dist',
+            tree=info['serverRoot'],
+        )
```

### Comparing `girder-item-licenses-3.2.4.dev7/girder_item_licenses/rest.py` & `girder-item-licenses-5.0.0a2/girder_item_licenses/rest.py`

 * *Files identical despite different names*

### Comparing `girder-item-licenses-3.2.4.dev7/girder_item_licenses/settings.py` & `girder-item-licenses-5.0.0a2/girder_item_licenses/settings.py`

 * *Files identical despite different names*

### Comparing `girder-item-licenses-3.2.4.dev7/girder_item_licenses.egg-info/PKG-INFO` & `girder-item-licenses-5.0.0a2/girder_item_licenses.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-item-licenses
-Version: 3.2.4.dev7
+Version: 5.0.0a2
 Summary: Add a license field to items.
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `girder-item-licenses-3.2.4.dev7/plugin_tests/item_licenses_test.py` & `girder-item-licenses-5.0.0a2/plugin_tests/item_licenses_test.py`

 * *Files identical despite different names*

### Comparing `girder-item-licenses-3.2.4.dev7/setup.py` & `girder-item-licenses-5.0.0a2/setup.py`

 * *Files identical despite different names*

